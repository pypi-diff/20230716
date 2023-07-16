# Comparing `tmp/python-semantic-release-8.0.0rc3.tar.gz` & `tmp/python-semantic-release-8.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0rc3.tar", last modified: Sat Jul  1 23:23:53 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0rc4.tar", last modified: Sun Jul  9 17:01:34 2023, max compression
```

## Comparing `python-semantic-release-8.0.0rc3.tar` & `python-semantic-release-8.0.0rc4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3111 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/README.rst
--rw-r--r--   0 root         (0) root         (0)     4681 2023-07-01 23:23:45.000000 python-semantic-release-8.0.0rc3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3111 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4221 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-01 23:23:45.000000 python-semantic-release-8.0.0rc3/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.737640 python-semantic-release-8.0.0rc3/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.737640 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18649 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    13706 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.729639 python-semantic-release-8.0.0rc3/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10146 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.729639 python-semantic-release-8.0.0rc3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22533 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    23987 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13407 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.730911 python-semantic-release-8.0.0rc4/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-09 17:01:34.730911 python-semantic-release-8.0.0rc4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4696 2023-07-09 17:01:27.000000 python-semantic-release-8.0.0rc4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.706911 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      610 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-09 17:01:34.000000 python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.710911 python-semantic-release-8.0.0rc4/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-09 17:01:27.000000 python-semantic-release-8.0.0rc4/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.710911 python-semantic-release-8.0.0rc4/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.710911 python-semantic-release-8.0.0rc4/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.714911 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18649 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    13706 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.714911 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.702911 python-semantic-release-8.0.0rc4/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.714911 python-semantic-release-8.0.0rc4/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.718911 python-semantic-release-8.0.0rc4/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10146 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.718911 python-semantic-release-8.0.0rc4/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 17:01:34.730911 python-semantic-release-8.0.0rc4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.702911 python-semantic-release-8.0.0rc4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.718911 python-semantic-release-8.0.0rc4/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.722911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.726911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.726911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22533 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    23987 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 17:01:34.730911 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-07-09 17:00:37.000000 python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0rc3/LICENSE` & `python-semantic-release-8.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/PKG-INFO` & `python-semantic-release-8.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0rc3
+Version: 8.0.0rc4
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0rc3/README.rst` & `python-semantic-release-8.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/pyproject.toml` & `python-semantic-release-8.0.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-rc.3"
+version = "8.0.0-rc.4"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
@@ -41,32 +41,32 @@
 
 [project.urls]
 "Project Url" = "http://github.com/python-semantic-release/python-semantic-release"
 Homepage = "https://python-semantic-release.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
-  "Sphinx<=8.0.0",
+  "Sphinx<=6.0.0",
   "sphinxcontrib-apidoc==0.3.0",
   "sphinx-autobuild==2021.03.14",
-  "furo>=2023.5.20",
+  "furo>=2023.3.27",
 ]
 test = [
   "coverage[toml]>=6,<7",
   "pytest>=7,<8",
   "pytest-xdist>=2,<3",
   "pytest-mock>=3,<4",
   "pytest-lazy-fixture~=0.6.3",
   "pytest-cov>=4,<5",
   "responses==0.21.0",
   "requests-mock>=1.10.0,<2",
   "types-pytest-lazy-fixture>=0.6.3.3",
 ]
 dev = ["tox", "isort", "black"]
-mypy = ["mypy", "types-requests"]
+mypy = ["mypy", "types-requests", "types-click"]
 
 [tool.pytest.ini_options]
 addopts = [
   "-nauto",
   "-ra",
   "--cache-clear",
   "--cov=semantic_release",
```

### Comparing `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0rc3
+Version: 8.0.0rc4
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.0rc4/python_semantic_release.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 [dev]
 tox
 isort
 black
 
 [docs]
-Sphinx<=8.0.0
+Sphinx<=6.0.0
 sphinxcontrib-apidoc==0.3.0
 sphinx-autobuild==2021.03.14
-furo>=2023.5.20
+furo>=2023.3.27
 
 [mypy]
 mypy
 types-requests
+types-click
 
 [test]
 coverage[toml]<7,>=6
 pytest<8,>=7
 pytest-xdist<3,>=2
 pytest-mock<4,>=3
 pytest-lazy-fixture~=0.6.3
```

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/__init__.py` & `python-semantic-release-8.0.0rc4/semantic_release/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-rc.3"
+__version__ = "8.0.0-rc.4"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0rc4/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0rc4/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0rc4/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/common.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/config.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/cli/util.py` & `python-semantic-release-8.0.0rc4/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0rc4/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/const.py` & `python-semantic-release-8.0.0rc4/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.0rc4/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/enums.py` & `python-semantic-release-8.0.0rc4/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/errors.py` & `python-semantic-release-8.0.0rc4/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/helpers.py` & `python-semantic-release-8.0.0rc4/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0rc4/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0rc4/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0rc4/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/version/translator.py` & `python-semantic-release-8.0.0rc4/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/semantic_release/version/version.py` & `python-semantic-release-8.0.0rc4/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_help.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_main.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_publish.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/command_line/test_version.py` & `python-semantic-release-8.0.0rc4/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0rc4/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0rc4/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0rc4/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0rc4/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0rc4/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0rc4/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0rc4/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0rc4/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

