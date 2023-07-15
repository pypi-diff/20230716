# Comparing `tmp/check_changelog-0.2.1-py3-none-any.whl.zip` & `tmp/check_changelog-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6596 bytes, number of entries: 9
+Zip file size: 9152 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      160 b- defN 16-Jan-01 00:00 check_changelog/__init__.py
--rw-rw-r--  2.0 unx     1269 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
--rw-rw-r--  2.0 unx     6616 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
+-rw-rw-r--  2.0 unx     3702 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
+-rw-rw-r--  2.0 unx     8027 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
+-rw-rw-r--  2.0 unx     2011 b- defN 16-Jan-01 00:00 check_changelog/git.py
 -rw-rw-r--  2.0 unx       21 b- defN 16-Jan-01 00:00 check_changelog/__version__.py
-?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/WHEEL
-?rw-------  2.0 unx     3245 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/licenses/LICENSE
-?rw-------  2.0 unx      775 b- defN 16-Jan-01 00:00 check_changelog-0.2.1.dist-info/RECORD
-9 files, 13341 bytes uncompressed, 5244 bytes compressed:  60.7%
+?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/WHEEL
+?rw-------  2.0 unx     4385 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/licenses/LICENSE
+?rw-------  2.0 unx      854 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/RECORD
+10 files, 20415 bytes uncompressed, 7680 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: check_changelog/__main__.py
 Comment: 
 
 Filename: check_changelog/changelog.py
 Comment: 
 
+Filename: check_changelog/git.py
+Comment: 
+
 Filename: check_changelog/__version__.py
 Comment: 
 
-Filename: check_changelog-0.2.1.dist-info/entry_points.txt
+Filename: check_changelog-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_changelog-0.2.1.dist-info/WHEEL
+Filename: check_changelog-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: check_changelog-0.2.1.dist-info/METADATA
+Filename: check_changelog-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: check_changelog-0.2.1.dist-info/licenses/LICENSE
+Filename: check_changelog-0.3.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: check_changelog-0.2.1.dist-info/RECORD
+Filename: check_changelog-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_changelog/__main__.py

```diff
@@ -8,52 +8,146 @@
 ```
 check-changelog --file CHANGELOG.md
 ```
 """
 
 
 import logging
+import os
 import sys
 
 import pydevkit.log.config  # noqa: F401
 from pydevkit.argparse import ArgumentParser
 
 from . import __version__
-from .changelog import CLNotFoundError, CLSyntaxError, check_changelog
+from .changelog import check_changelog_main
+from .git import git_check_tags
 
 log = logging.getLogger(__name__)
 
+bool_yes_no = ["yes", "no"]
+
 
 def get_args():
     p = ArgumentParser(help=__doc__, version=__version__)
     p.add_argument(
+        "--check",
+        help=("if value is 'yes', check changelog structure"),
+        choices=bool_yes_no,
+        default="yes",
+    )
+    p.add_argument(
+        "--install",
+        help=("if value is 'yes', installs git 'pre-push' hook"),
+        choices=bool_yes_no,
+        default="no",
+    )
+    p.add_argument(
+        "--tags",
+        help=(
+            "check that specified git tags are documented. "
+            "Value can be 'hook' to read tag "
+            "refs from stdin as pre-push hook would do. Or it can be "
+            "'history:N' for N latest tags, or 'history' to all tags."
+        ),
+        default="",
+    )
+    p.add_argument("-C", help="top project dir", dest="topdir", default=".")
+    p.add_argument(
         "--file", help="changelog file to check", default="CHANGELOG.md"
     )
 
     return p.parse_known_args()
 
 
+def task_status(ttype, tname, status):
+    clrs = {
+        "norm": "\033[0m",
+        "ok": "\033[32;1m",
+        "fail": "\033[31;1m",
+        "starting": "\033[32;1m",
+    }
+    msg = ""
+    rc = {
+        "clr-off": clrs["norm"],
+        "clr-on": clrs[status],
+        "type": ttype,
+        "name": tname,
+        "status": status,
+    }
+    fmt = "%(clr-on)s%(type)s%(clr-off)s %(name)s: %(clr-on)s%(status)s%(clr-off)s"
+    msg += fmt % rc
+    return msg
+
+
+def run_task(ttype, tname, func, *args):
+    _norm = "\033[0m"
+    _ok = "\033[32;1m"
+    _fail = "\033[31;1m"
+    log.info("%s", task_status(ttype, tname, "starting"))
+    try:
+        rc = func(*args)
+    except Exception as exc:
+        rc = False
+        log.error("%s", exc)
+    if rc:
+        log.info("%s", task_status(ttype, tname, "ok"))
+    else:
+        log.error("%s", task_status(ttype, tname, "fail"))
+    return rc
+
+
+def run_all_tasks(args):
+    text = open(args.file, "r").read()
+    rcs = []
+    if args.check == "yes":
+        rc = run_task(
+            "task",
+            "check changelog structure",
+            check_changelog_main,
+            args.file,
+            text,
+        )
+        rcs.append(rc)
+
+    if args.tags:
+        rc = run_task(
+            "task", "check tags documentation", git_check_tags, text, args.tags
+        )
+        rcs.append(rc)
+
+    return all(rcs)
+
+
+def install_git_hook():
+    path = ".git/hooks/pre-push"
+    if os.path.exists(path):
+        log.warning("remove current '%s'", path)
+        os.unlink(path)
+    sh = "#!/bin/bash\n\n" + sys.argv[0] + " --tags=hook --check=no\n"
+    open(path, "w").write(sh)
+    os.chmod(path, 0o755)
+    return True
+
+
 def main():
     args, unknown_args = get_args()
     if unknown_args:
         log.warning("Unknown arguments: %s", unknown_args)
         sys.exit(1)
-    try:
-        text = open(args.file, "r").read()
-        check_changelog(text)
-        sys.exit(0)
-    except (CLSyntaxError, CLNotFoundError) as exp:
-        log.error(
-            "%s:%d: %s; got '%s'%s",
-            args.file,
-            exp.lineno,
-            exp.msg,
-            exp.content,
-            "; " + exp.msg_extra if exp.msg_extra else "",
-        )
-    except Exception as exp:
-        log.error("%s", exp)
-    sys.exit(1)
+    if args.topdir != ".":
+        try:
+            log.info("working dir '%s'", args.topdir)
+            os.chdir(args.topdir)
+        except Exception as exp:
+            log.error("%s", exp)
+            sys.exit(1)
+
+    if args.install == "yes":
+        rc = run_task("hook", "install pre-push", install_git_hook)
+    else:
+        rc = run_task("file", args.file, run_all_tasks, args)
+    sys.exit(0 if rc else 1)
 
 
 if __name__ == "__main__":
     main()
```

## check_changelog/changelog.py

```diff
@@ -138,14 +138,17 @@
     tokens.consume_until(
         lambda x: x.tag == tag
         and x.type == tag2type[tag] + "_close"
         and x.level == t.level
     )
 
 
+ctx = {}
+
+
 def title():
     log.debug("%s", func_name())
     msg = "expected 'Changelog'"
 
     def _validate(msg):
         t = tokens.next()
         log.info("title: %s", t.content)
@@ -154,15 +157,22 @@
             raise CLSyntaxError(m1, t, msg)
 
     do_item("h1", msg, _validate)
 
 
 def notes():
     log.debug("%s", func_name())
-    do_item("p", "", None)
+
+    def _validate(msg):  # noqa: ARG001
+        t = tokens.next()
+        t.content.replace("\n", " ")
+        tlen = len(t.content) + ctx.get("notes", 0)
+        ctx["notes"] = tlen
+
+    do_item("p", "", _validate)
 
 
 def release_header():
     log.debug("%s", func_name())
     msg = "expected '[Unreleased]' or '[ver] - YYYY-MM-DD'"
     msgr = "expected '[ver] - YYYY-MM-DD'"
 
@@ -200,40 +210,54 @@
 
     do_item("h2", msg, _validate)
 
 
 def change():
     log.debug("%s", func_name())
     msg = "expecting list item"
+    idx = ctx["changes"]["idx"]
     do_item("li", msg, None)
+    count = ctx["changes"].get(idx, 0)
+    ctx["changes"][idx] = count + 1
 
 
 def change_list():
     log.debug("%s", func_name())
     msg = "expecting unordered list"
 
     def _validate(msg):  # noqa: ARG001
         tokens.next()
         run(change, narg="+")
 
     do_item("ul", msg, _validate)
 
 
+change_type_names = [
+    "Added",
+    "Changed",
+    "Deprecated",
+    "Removed",
+    "Fixed",
+    "Security",
+]
+change_type_len = max([len(k) for k in change_type_names])
+
+
 def change_type():
     log.debug("%s", func_name())
     msg = "expecting '### <Change Type>'"
 
     def _validate(msg):
         t = tokens.next()
-        log.info("change type: %s", t.content)
+        log.debug("change type: %s", t.content)
         msg += "; got '%s'" % t.content
-        cnames = ["Added", "Changed", "Deprecated", "Removed", "Fixed", "Security"]
-        if t.content not in cnames:
+        if t.content not in change_type_names:
             m1 = "bad change type"
-            raise CLSyntaxError(m1, t, "expected one of %s" % cnames)
+            raise CLSyntaxError(m1, t, "expected one of %s" % change_type_names)
+        ctx["changes"]["idx"] = t.content
 
     do_item("h3", msg, _validate)
 
 
 def change_block():
     log.debug("%s", func_name())
     run(change_type, narg=1)
@@ -242,25 +266,61 @@
     except CLNotFoundError as exp:
         raise CLSyntaxError(exp.msg, exp.token) from exp
 
 
 def release():
     log.debug("%s", func_name())
     run(release_header, narg=1)
+
+    ctx["notes"] = 0
     run(notes, narg="*")
+    nnotes = ctx.get("notes")
+    if nnotes:
+        log.info("  notes: %d chars", nnotes)
+    del ctx["notes"]
+
+    ctx["changes"] = {"idx": "none"}
     run(change_block, narg="*")
+    del ctx["changes"]["idx"]
+    keys = ctx["changes"].keys()
+    if keys:
+        fmt = "  %%-%ds: %%s" % change_type_len
+        for k, v in ctx["changes"].items():
+            log.info(fmt, k.lower(), v)
 
 
 def check_changelog(text):
     log.debug("%s", func_name())
     md = MarkdownIt("commonmark", {"breaks": True, "html": True})
     global tokens  # noqa: PLW0603
     tokens = Tokens(md.parse(text))
 
     run(title, narg=1)
     run(notes, narg="*")
+    nnotes = ctx.get("notes")
+    if nnotes:
+        log.info("  notes: %d chars", nnotes)
+        del ctx["notes"]
     run(release, narg="+")
 
     if tokens.is_empty() or tokens.get().tag == "hr":
-        return
+        return True
     msg = "out of context"
     raise CLSyntaxError(msg, tokens.get())
+
+
+def check_changelog_main(fname, text):
+    try:
+        return check_changelog(text)
+    except (CLSyntaxError, CLNotFoundError) as exp:
+        log.error(
+            "%s:%d: %s; got '%s'%s",
+            fname,
+            exp.lineno,
+            exp.msg,
+            exp.content,
+            "; " + exp.msg_extra if exp.msg_extra else "",
+        )
+        return False
+    except Exception as exp:
+        log.error("%s", exp)
+        raise
```

## check_changelog/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.2.1'
+__version__ = '0.3.0'
```

## Comparing `check_changelog-0.2.1.dist-info/METADATA` & `check_changelog-0.3.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-changelog
-Version: 0.2.1
+Version: 0.3.0
 Summary: check that changelog conforms to 'Keep A Changelog' style
 Author-email: Anatoly Asviyan <aanatoly@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -22,42 +22,44 @@
 # check-changelog
 
 [![pkg - version][pkg-version]][pkg-link]
 [![pkg - python versions][pkg-pyversions]][pkg-link]
 [![pkg - license][pkg-license]][pkg-link]
 
 ---
-
-check that changelog conforms to [Keep A Changelog][kacl] and
-[Common Changelog][ccl] styles.
+The project's aims are:
+ - validate `CHANGELOG.md`. Check that it conforms to
+   [Keep A Changelog][kacl] and [Common Changelog][ccl] styles.
+ - ensure git tags are documented in `CHANGELOG.md`
+ - block pushing tags without changelog. See [git pre-push](#git-pre-push-hook) section
 
 Main features:
- * check that changelog conforms to [Keep A Changelog][kacl] style
- * allow release notes. Add them between the release header and change list
+ - check that changelog conforms to [Keep A Changelog][kacl] style
+ - allow release notes. Add them between the release header and change list
    ([Common Changelog][ccl] addition)
 
    ```markdown
    ## [1.0.0] - 2023-05-05
    Release notes
 
    ### Added
     - add feature ...
    ```
 
- * allow custom footer to keep things from being verified. Useful for legal
+ - allow custom footer to keep things from being verified. Useful for legal
    notes, text used by other scripts, HTML comments, etc
 
    ```markdown
    -----
    Linter will ignore this section.
    <!--- message for some script -->
    [my site]: http://mysite.com
    ```
 
- * `gcc` style error reports
+ - `gcc` style error reports
    ```text
    CHANGELOG.md:10: bad release title: [0.2.1]; expected '[Unreleased]' or '[ver] - YYYY-MM-DD'
    CHANGELOG.md:12: bad change type: Changed2; expected one of ['Added', 'Changed', ...]
     ```
 
 ## Installation
 
@@ -67,28 +69,60 @@
 
 ## Usage
 From command line
 
 ```sh
 # check CHANGELOG.md in a current dir
 check-changelog
-# check specific CHANGELOG.md
-check-changelog -f path/to/changelog.md
+check-changelog --check=yes --tags=   # default settings
+# check CHANGELOG.md and git tags
+check-changelog --check=yes --tags=history
 ```
 
 As a [pre-commit](https://pre-commit.com/) hook.
 Add this section to your `.pre-commit-config.yaml`
 
 ```yml
 - repo: https://github.com/aanatoly/check-changelog
-  rev: '0.2.1'
+  rev: '0.3.0'
   hooks:
     - id: check-changelog
 ```
 
+### git pre-push hook
+As a git `pre-push` hook, `check-changelog` can block `git` from pushing
+tags without changelog. To install it that way, run the following commmands
+
+```sh
+# backup existing hook
+mv .git/hooks/pre-push  .git/hooks/pre-push.bak
+# install new hook
+check-changelog --install=yes
+```
+
+and let's test it
+
+```sh
+git tag -a -m "abc.7.7" "abc.7.7"
+git tag -a -m "abc.7.8" "abc.7.8"
+git push --tags --dry-run
+
+# check-changelog :: INFO  :: file CHANGELOG.md: starting
+# check-changelog :: INFO  :: task check tags documentation: starting
+# check-changelog :: INFO  :: scan 2 tags from 'hook' source
+# check-changelog :: ERROR :: tag 'abc.7.7' not found
+# check-changelog :: ERROR :: tag 'abc.7.8' not found
+# check-changelog :: ERROR :: task check tags documentation: fail
+# check-changelog :: ERROR :: file CHANGELOG.md: fail
+
+git tag -d "abc.7.7"
+git tag -d "abc.7.8"
+
+```
+
 ## Alternatives
 `check-changelog` is a minimalistic tool by design. It checks the Changelog
 structure and does nothing else.
 
 If you are looking for more, check [python-kacl][py-kacl]. It is a feature-rich tool
 capable of linting, fixing errors, and automating Changelog maintenance.
```

## Comparing `check_changelog-0.2.1.dist-info/licenses/LICENSE` & `check_changelog-0.3.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `check_changelog-0.2.1.dist-info/RECORD` & `check_changelog-0.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 check_changelog/__init__.py,sha256=z6wfs6rLKrBxFKviVD4mhopUYd8p9VKRhEIsCmVDZ1I,160
-check_changelog/__main__.py,sha256=pI6QEHOoy4CXz8vSYdsdLuBo3FBHM_dJJj9i7FpwIiA,1269
-check_changelog/changelog.py,sha256=xGu7AMEna96mdZaQoA_WvdGlcDbdRVwr90hM-u4hSwQ,6616
-check_changelog/__version__.py,sha256=nx8uT9NOkkA2KzjU9Q36cvZlTi-7bCHVPIkXCQkwZf8,21
-check_changelog-0.2.1.dist-info/entry_points.txt,sha256=QO_7CfyUIWuIRCmlmoZQpMzme-MWBAtLL1oToAsuhbI,65
-check_changelog-0.2.1.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
-check_changelog-0.2.1.dist-info/METADATA,sha256=PBcP0lSWKAgZPLEa_YXUbIKoH-XpCPCU_FZN7EcmWMk,3245
-check_changelog-0.2.1.dist-info/licenses/LICENSE,sha256=TZ52n6XUyJFPMHXZ2evCCSYnunrYn-7LRPZV8n4FvSw,1103
-check_changelog-0.2.1.dist-info/RECORD,,
+check_changelog/__main__.py,sha256=xvC6NrViTLn0_b3CARQN1EHeFO2eSWSPhJIuO0bA9ys,3702
+check_changelog/changelog.py,sha256=sN8jZQ38r4f_Hec_2LC7bUrpPzfq_nw3FVooz-5wCKI,8027
+check_changelog/git.py,sha256=PHCRUvTTrDwO5lnfi0hAJtGKn0uhU3UqTQ9Ql_mse_c,2011
+check_changelog/__version__.py,sha256=gTggO06fb2c9XKEwlQYUSPlUfy82yVlM9pzLMOUqVcY,21
+check_changelog-0.3.0.dist-info/entry_points.txt,sha256=QO_7CfyUIWuIRCmlmoZQpMzme-MWBAtLL1oToAsuhbI,65
+check_changelog-0.3.0.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+check_changelog-0.3.0.dist-info/METADATA,sha256=AuPlYT8Q-KLsx34Tz_fgNYSncEEedLG9P4nFbb2g1xs,4385
+check_changelog-0.3.0.dist-info/licenses/LICENSE,sha256=TZ52n6XUyJFPMHXZ2evCCSYnunrYn-7LRPZV8n4FvSw,1103
+check_changelog-0.3.0.dist-info/RECORD,,
```

