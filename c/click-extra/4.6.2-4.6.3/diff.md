# Comparing `tmp/click_extra-4.6.2.tar.gz` & `tmp/click_extra-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.6.2.tar", max compression
+gzip compressed data, was "click_extra-4.6.3.tar", max compression
```

## Comparing `click_extra-4.6.2.tar` & `click_extra-4.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6104 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/__init__.py
--rw-r--r--   0        0        0    28997 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/colorize.py
--rw-r--r--   0        0        0    16232 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/commands.py
--rw-r--r--   0        0        0    16405 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/config.py
--rw-r--r--   0        0        0     4069 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/decorators.py
--rw-r--r--   0        0        0     6211 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/docs_update.py
--rw-r--r--   0        0        0    11805 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/logging.py
--rw-r--r--   0        0        0    25392 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/parameters.py
--rw-r--r--   0        0        0    17118 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/py.typed
--rw-r--r--   0        0        0     7676 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/sphinx.py
--rw-r--r--   0        0        0     5969 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tabulate.py
--rw-r--r--   0        0        0     2542 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11504 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    19238 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    15075 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    17059 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7354 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    18184 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8396 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14491 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     6359 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2544 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/timer.py
--rw-r--r--   0        0        0    11757 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/version.py
--rw-r--r--   0        0        0     7641 2023-07-15 09:31:25.196612 click_extra-4.6.2/pyproject.toml
--rw-r--r--   0        0        0     6631 2023-07-15 09:31:25.196612 click_extra-4.6.2/readme.md
--rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.2/PKG-INFO
+-rw-r--r--   0        0        0     6104 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/__init__.py
+-rw-r--r--   0        0        0    28829 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/colorize.py
+-rw-r--r--   0        0        0    16667 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/commands.py
+-rw-r--r--   0        0        0    16255 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/decorators.py
+-rw-r--r--   0        0        0     6211 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11805 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/logging.py
+-rw-r--r--   0        0        0    25267 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/py.typed
+-rw-r--r--   0        0        0     7676 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-07-16 10:20:49.515345 click_extra-4.6.3/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5969 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11504 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    19238 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    15075 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    17059 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7354 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    18184 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8396 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14491 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     6359 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2544 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/timer.py
+-rw-r--r--   0        0        0    11632 2023-07-16 10:20:49.519346 click_extra-4.6.3/click_extra/version.py
+-rw-r--r--   0        0        0     7641 2023-07-16 10:20:49.523346 click_extra-4.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-07-16 10:20:49.523346 click_extra-4.6.3/readme.md
+-rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.3/PKG-INFO
```

### Comparing `click_extra-4.6.2/click_extra/__init__.py` & `click_extra-4.6.3/click_extra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.6.2"
+__version__ = "4.6.3"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `click_extra-4.6.2/click_extra/colorize.py` & `click_extra-4.6.3/click_extra/colorize.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,15 @@
 
         Returns the same instance if the provided styles are the same as the current.
         """
         # Check for unrecognized arguments.
         unrecognized_args = set(kwargs).difference(self.__dataclass_fields__)
         if unrecognized_args:
             msg = f"Got unexpected keyword argument(s): {', '.join(unrecognized_args)}"
-            raise TypeError(
-                msg,
-            )
+            raise TypeError(msg)
 
         # List of styles that are different from the base theme.
         new_styles = {
             field_id: new_style
             for field_id, new_style in kwargs.items()
             if new_style != getattr(self, field_id)
         }
@@ -322,17 +320,14 @@
 
         Exact same behavior as `Click's original @help_option callback
         <https://github.com/pallets/click/blob/d9af5cf/src/click/decorators.py#L555-L560>`_,
         but forces the closing of the context before exiting.
         """
         if value and not ctx.resilient_parsing:
             echo(ctx.get_help(), color=ctx.color)
-            # Do not just ctx.exit() as it will prevent callbacks defined on options
-            # to be called.
-            ctx.close()
             ctx.exit()
 
 
 class ExtraHelpColorsMixin:  # (Command)??
     """Adds extra-keywords highlighting to Click commands.
 
     This mixin for ``click.Command``-like classes intercepts the top-level helper-
```

### Comparing `click_extra-4.6.2/click_extra/commands.py` & `click_extra-4.6.3/click_extra/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 counterparts, but are pre-configured with good and common defaults. You can still
 leverage the mixins in here to build up your own custom variants.
 """
 
 from __future__ import annotations
 
 import logging
-from typing import Any, cast
+from typing import TYPE_CHECKING, Any, cast
 
 import click
 import cloup
 
 from . import Command, Group
 from .colorize import ColorOption, ExtraHelpColorsMixin, HelpExtraFormatter, HelpOption
 from .config import ConfigOption
@@ -38,14 +38,17 @@
     all_envvars,
     normalize_envvar,
     search_params,
 )
 from .timer import TimerOption
 from .version import ExtraVersionOption
 
+if TYPE_CHECKING:
+    from typing import NoReturn
+
 
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
     ``meta`` property at instantiation.
 
     Also inherits ``color`` property from parent context. And sets it to `True` for
     parentless contexts at instantiatiom, so we can always have colorized output.
@@ -95,14 +98,26 @@
         self._color = value
 
     @color.deleter
     def color(self) -> None:
         """Reset the color value so it defaults to inheritance from parent's."""
         self._color = None
 
+    def exit(self, code: int = 0) -> NoReturn:
+        """Exits the application with a given exit code.
+
+        Forces the context to close before exiting, so callbacks attached to parameters
+        will be called to clean up their state.
+
+        .. todo::
+            Propose this fix upstream to Click.
+        """
+        self.close()
+        super().exit(code)
+
 
 def default_extra_params():
     """Default additional options added to ``extra_command`` and ``extra_group``.
 
     .. caution::
         The order of options has been carefully crafted to handle subtle edge-cases and
         avoid leaky states in unittests.
```

### Comparing `click_extra-4.6.2/click_extra/config.py` & `click_extra-4.6.3/click_extra/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,18 +423,14 @@
         ctx.meta["click_extra.conf_full"] = user_conf
 
         # Exit the CLI if no user-provided config file was found.
         if user_conf is None:
             message = "No configuration file found."
             if explicit_conf:
                 logger.critical(message)
-
-                # Do not just ctx.exit() as it will prevent callbacks defined on options
-                # to be called.
-                ctx.close()
                 ctx.exit(2)
             else:
                 logger.debug(message)
 
         else:
             logger.debug(f"Parsed user configuration: {user_conf}")
             logger.debug(f"Initial defaults: {ctx.default_map}")
```

### Comparing `click_extra-4.6.2/click_extra/decorators.py` & `click_extra-4.6.3/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/docs_update.py` & `click_extra-4.6.3/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/logging.py` & `click_extra-4.6.3/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/parameters.py` & `click_extra-4.6.3/click_extra/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,11 +707,8 @@
             sorted(table, key=sort_by_depth),
             headers=header_labels,
             tablefmt="rounded_outline",
             disable_numparse=True,
         )
         echo(output, color=ctx.color)
 
-        # Do not just ctx.exit() as it will prevent callbacks defined on options
-        # to be called.
-        ctx.close()
         ctx.exit()
```

### Comparing `click_extra-4.6.2/click_extra/platforms.py` & `click_extra-4.6.3/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/pygments.py` & `click_extra-4.6.3/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/sphinx.py` & `click_extra-4.6.3/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tabulate.py` & `click_extra-4.6.3/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/telemetry.py` & `click_extra-4.6.3/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/testing.py` & `click_extra-4.6.3/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/__init__.py` & `click_extra-4.6.3/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/conftest.py` & `click_extra-4.6.3/click_extra/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_colorize.py` & `click_extra-4.6.3/click_extra/tests/test_colorize.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_commands.py` & `click_extra-4.6.3/click_extra/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_config.py` & `click_extra-4.6.3/click_extra/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_logging.py` & `click_extra-4.6.3/click_extra/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_parameters.py` & `click_extra-4.6.3/click_extra/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_platforms.py` & `click_extra-4.6.3/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_pygments.py` & `click_extra-4.6.3/click_extra/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_tabulate.py` & `click_extra-4.6.3/click_extra/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_telemetry.py` & `click_extra-4.6.3/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_testing.py` & `click_extra-4.6.3/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_timer.py` & `click_extra-4.6.3/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/tests/test_version.py` & `click_extra-4.6.3/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/timer.py` & `click_extra-4.6.3/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/click_extra/version.py` & `click_extra-4.6.3/click_extra/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,12 +304,9 @@
         ctx.meta["click_extra.env_info"] = self.env_info
 
         if not value or ctx.resilient_parsing:
             return
 
         echo(self.render_message(), color=ctx.color)
 
-        # Do not just ctx.exit() as it will prevent callbacks defined on options
-        # to be called.
-        ctx.close()
         ctx.exit()
         return  # type: ignore[unreachable]
```

### Comparing `click_extra-4.6.2/pyproject.toml` & `click_extra-4.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.6.2"
+version = "4.6.3"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -183,15 +183,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.6.2"
+current_version = "4.6.3"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./click_extra/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "./pyproject.toml"
```

### Comparing `click_extra-4.6.2/readme.md` & `click_extra-4.6.3/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.2/PKG-INFO` & `click_extra-4.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.6.2
+Version: 4.6.3
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.6.2 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.6.3 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
```

