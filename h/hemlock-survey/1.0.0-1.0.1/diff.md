# Comparing `tmp/hemlock-survey-1.0.0.tar.gz` & `tmp/hemlock-survey-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hemlock-survey-1.0.0.tar", last modified: Sun Feb 27 16:51:41 2022, max compression
+gzip compressed data, was "hemlock-survey-1.0.1.tar", last modified: Sun Jul 16 12:00:02 2023, max compression
```

## Comparing `hemlock-survey-1.0.0.tar` & `hemlock-survey-1.0.1.tar`

### file list

```diff
@@ -1,76 +1,89 @@
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.912052 hemlock-survey-1.0.0/
--rw-rw-rw-   0        0        0      260 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      324 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1403 2022-02-27 16:51:41.912052 hemlock-survey-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      879 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1173 2022-02-27 16:51:41.922053 hemlock-survey-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.602051 hemlock-survey-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.713052 hemlock-survey-1.0.0/src/hemlock/
--rw-rw-rw-   0        0        0      407 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/__init__.py
--rw-rw-rw-   0        0        0     5746 2022-01-22 17:07:45.000000 hemlock-survey-1.0.0/src/hemlock/_admin_routes.py
--rw-rw-rw-   0        0        0     2085 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_custom_types.py
--rw-rw-rw-   0        0        0     5092 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_data_frame.py
--rw-rw-rw-   0        0        0     7832 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_display_navigation.py
--rw-rw-rw-   0        0        0     3874 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_navbar.py
--rw-rw-rw-   0        0        0      308 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_page_css.html
--rw-rw-rw-   0        0        0      365 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_page_js.html
--rw-rw-rw-   0        0        0     4848 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/_user_routes.py
--rw-rw-rw-   0        0        0     2055 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/admin_route_utils.py
--rw-rw-rw-   0        0        0     3967 2022-01-05 17:46:24.000000 hemlock-survey-1.0.0/src/hemlock/app.py
--rw-rw-rw-   0        0        0     3673 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/data.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.730066 hemlock-survey-1.0.0/src/hemlock/functional/
--rw-rw-rw-   0        0        0       92 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/functional/__init__.py
--rw-rw-rw-   0        0        0     2632 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/functional/base.py
--rw-rw-rw-   0        0        0     3052 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/functional/compile.py
--rw-rw-rw-   0        0        0     7973 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/functional/test_response.py
--rw-rw-rw-   0        0        0     5635 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/functional/validate.py
--rw-rw-rw-   0        0        0    22132 2022-01-02 14:29:11.000000 hemlock-survey-1.0.0/src/hemlock/page.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.763053 hemlock-survey-1.0.0/src/hemlock/questions/
--rw-rw-rw-   0        0        0      164 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/__init__.py
--rw-rw-rw-   0        0        0    14390 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/base.py
--rw-rw-rw-   0        0        0     2228 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/check.py
--rw-rw-rw-   0        0        0     7327 2022-01-18 00:29:56.000000 hemlock-survey-1.0.0/src/hemlock/questions/choice_base.py
--rw-rw-rw-   0        0        0     7933 2022-01-18 14:36:20.000000 hemlock-survey-1.0.0/src/hemlock/questions/input.py
--rw-rw-rw-   0        0        0     1626 2022-01-18 00:29:56.000000 hemlock-survey-1.0.0/src/hemlock/questions/label.py
--rw-rw-rw-   0        0        0     2337 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/range.py
--rw-rw-rw-   0        0        0     1383 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/select.py
--rw-rw-rw-   0        0        0     4171 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/questions/textarea.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.596053 hemlock-survey-1.0.0/src/hemlock/templates/
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.796053 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/
--rw-rw-rw-   0        0        0     1015 2022-01-02 02:59:15.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/check.html
--rw-rw-rw-   0        0        0      687 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/input.html
--rw-rw-rw-   0        0        0      122 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/label.html
--rw-rw-rw-   0        0        0     5016 2022-01-22 17:12:44.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/page.html
--rw-rw-rw-   0        0        0      588 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/range.html
--rw-rw-rw-   0        0        0      483 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/range.js
--rw-rw-rw-   0        0        0     1070 2022-01-02 02:59:29.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/select.html
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.805053 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/statics/
--rw-rw-rw-   0        0        0     2208 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/statics/auto_advance.html
--rw-rw-rw-   0        0        0      315 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/statics/figure.html
--rw-rw-rw-   0        0        0      470 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/statics/recompile_at_interval.js
--rw-rw-rw-   0        0        0     1407 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/textarea.html
--rw-rw-rw-   0        0        0     1882 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/textarea.js
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.835052 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/
--rw-rw-rw-   0        0        0      413 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/card.html
--rw-rw-rw-   0        0        0      144 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/feedback.html
--rw-rw-rw-   0        0        0      104 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/form_text.html
--rw-rw-rw-   0        0        0      879 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/input_group.html
--rw-rw-rw-   0        0        0      191 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/label.html
--rw-rw-rw-   0        0        0     1196 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/loading_page.html
--rw-rw-rw-   0        0        0     2700 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/navbar.html
--rw-rw-rw-   0        0        0     2612 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/timer.py
--rw-rw-rw-   0        0        0     8248 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/tree.py
--rw-rw-rw-   0        0        0    24619 2022-01-18 00:09:37.000000 hemlock-survey-1.0.0/src/hemlock/user.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.858054 hemlock-survey-1.0.0/src/hemlock/utils/
--rw-rw-rw-   0        0        0     1290 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/utils/__init__.py
--rw-rw-rw-   0        0        0     1981 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/utils/format.py
--rw-rw-rw-   0        0        0     4849 2022-02-10 19:47:15.000000 hemlock-survey-1.0.0/src/hemlock/utils/random.py
--rw-rw-rw-   0        0        0     3940 2022-01-01 21:12:05.000000 hemlock-survey-1.0.0/src/hemlock/utils/statics.py
-drwxrwxrwx   0        0        0        0 2022-02-27 16:51:41.910055 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/
--rw-rw-rw-   0        0        0     1403 2022-02-27 16:51:40.000000 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2143 2022-02-27 16:51:41.000000 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-27 16:51:41.000000 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2022-02-27 16:51:41.000000 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-02-27 16:51:41.000000 hemlock-survey-1.0.0/src/hemlock_survey.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.700016 hemlock-survey-1.0.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1062 2023-07-16 10:59:22.000000 hemlock-survey-1.0.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      318 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1329 2023-07-16 12:00:02.700613 hemlock-survey-1.0.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      859 2023-07-16 11:56:38.000000 hemlock-survey-1.0.1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2023-07-16 12:00:02.705378 hemlock-survey-1.0.1/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.006769 hemlock-survey-1.0.1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.246229 hemlock-survey-1.0.1/src/hemlock/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      393 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5555 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_admin_routes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2017 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_custom_types.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4941 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_data_frame.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7580 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_display_navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3761 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_navbar.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      307 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_page_css.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      364 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_page_js.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4693 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/_user_routes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1979 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/admin_route_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3819 2023-07-16 10:29:02.000000 hemlock-survey-1.0.1/src/hemlock/app.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3635 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/data.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.304355 hemlock-survey-1.0.1/src/hemlock/functional/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/functional/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2552 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/functional/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2951 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/functional/compile.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7808 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/functional/test_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5448 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/functional/validate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    21544 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/page.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.374869 hemlock-survey-1.0.1/src/hemlock/questions/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      158 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14023 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2167 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/check.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7112 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/choice_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7726 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/input.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1580 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/label.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2271 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/range.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/select.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4053 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/questions/textarea.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:01.994128 hemlock-survey-1.0.1/src/hemlock/templates/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.445348 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      983 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/check.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      667 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/input.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      118 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/label.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4886 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/page.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      574 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/range.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      470 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/range.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1037 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/select.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.466678 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/statics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2157 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/statics/auto_advance.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      308 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/statics/figure.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      455 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/statics/recompile_at_interval.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1374 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/textarea.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1822 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/textarea.js
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.535082 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/card.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      140 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/feedback.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      100 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/form_text.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      851 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/input_group.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      186 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/label.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1158 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/loading_page.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2649 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/navbar.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2527 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/timer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8011 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/tree.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24902 2023-07-16 11:27:50.000000 hemlock-survey-1.0.1/src/hemlock/user.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.566634 hemlock-survey-1.0.1/src/hemlock/utils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1248 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/utils/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1914 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/utils/format.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4750 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/utils/random.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3811 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/src/hemlock/utils/statics.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.594072 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1329 2023-07-16 12:00:01.000000 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2426 2023-07-16 12:00:01.000000 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-16 12:00:01.000000 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      156 2023-07-16 12:00:01.000000 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-16 12:00:01.000000 hemlock-survey-1.0.1/src/hemlock_survey.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 12:00:02.697057 hemlock-survey-1.0.1/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3661 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test__admin_routes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      883 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test__data_frame.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6054 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test__display_navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3083 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test__navbar.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4193 2023-07-16 11:19:30.000000 hemlock-survey-1.0.1/tests/test__user_routes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      660 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_admin_route_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      581 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_app.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1446 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10146 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_page.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1017 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_timer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5587 2023-07-16 10:15:17.000000 hemlock-survey-1.0.1/tests/test_tree.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11023 2023-07-16 10:42:38.000000 hemlock-survey-1.0.1/tests/test_user.py
```

### Comparing `hemlock-survey-1.0.0/PKG-INFO` & `hemlock-survey-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1
-Name: hemlock-survey
-Version: 1.0.0
-Summary: A python framework for creating online surveys and experiments.
-Home-page: https://dsbowen.gitlab.io/hemlock
-Author: Dillon Bowen
-Author-email: dsbowen@wharton.upenn.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hemlock
-
-[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
-<!-- [![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE) -->
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
-
-
+Metadata-Version: 2.1
+Name: hemlock-survey
+Version: 1.0.1
+Summary: A python framework for creating online surveys and experiments.
+Home-page: https://dsbowen.gitlab.io/hemlock
+Author: Dillon Bowen
+Author-email: dsbowen@wharton.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hemlock
+
+[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
```

### Comparing `hemlock-survey-1.0.0/README.md` & `hemlock-survey-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Hemlock
-
-[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
-<!-- [![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE) -->
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
+# Hemlock
+
+[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
```

### Comparing `hemlock-survey-1.0.0/setup.cfg` & `hemlock-survey-1.0.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,71 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2068 656d 6c6f 636b 2d73 7572 7665   = hemlock-surve
-00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
-00000030: 2e30 0d0a 6175 7468 6f72 203d 2044 696c  .0..author = Dil
-00000040: 6c6f 6e20 426f 7765 6e0d 0a61 7574 686f  lon Bowen..autho
-00000050: 725f 656d 6169 6c20 3d20 6473 626f 7765  r_email = dsbowe
-00000060: 6e40 7768 6172 746f 6e2e 7570 656e 6e2e  n@wharton.upenn.
-00000070: 6564 750d 0a64 6573 6372 6970 7469 6f6e  edu..description
-00000080: 203d 2041 2070 7974 686f 6e20 6672 616d   = A python fram
-00000090: 6577 6f72 6b20 666f 7220 6372 6561 7469  ework for creati
-000000a0: 6e67 206f 6e6c 696e 6520 7375 7276 6579  ng online survey
-000000b0: 7320 616e 6420 6578 7065 7269 6d65 6e74  s and experiment
-000000c0: 732e 0d0a 6c6f 6e67 5f64 6573 6372 6970  s...long_descrip
-000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000120: 7073 3a2f 2f64 7362 6f77 656e 2e67 6974  ps://dsbowen.git
-00000130: 6c61 622e 696f 2f68 656d 6c6f 636b 0d0a  lab.io/hemlock..
-00000140: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000150: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000160: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000170: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
-00000180: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000190: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001c0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-000001d0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-000001e0: 5f64 6174 6120 3d20 5472 7565 0d0a 7061  _data = True..pa
-000001f0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000200: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000210: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000220: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-00000230: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000240: 7320 3d20 0d0a 0949 5079 7468 6f6e 0d0a  s = ...IPython..
-00000250: 0966 6c61 736b 0d0a 0966 6c61 736b 2d6c  .flask...flask-l
-00000260: 6f67 696e 0d0a 0966 6c61 736b 2d73 6f63  ogin...flask-soc
-00000270: 6b65 7469 6f0d 0a09 666c 6173 6b2d 7371  ketio...flask-sq
-00000280: 6c61 6c63 6865 6d79 0d0a 096d 6172 6b64  lalchemy...markd
-00000290: 6f77 6e0d 0a09 6d61 7470 6c6f 746c 6962  own...matplotlib
-000002a0: 0d0a 096e 6574 776f 726b 780d 0a09 7061  ...networkx...pa
-000002b0: 6e64 6173 0d0a 0973 696d 706c 652d 7765  ndas...simple-we
-000002c0: 6273 6f63 6b65 740d 0a09 7371 6c61 6c63  bsocket...sqlalc
-000002d0: 6865 6d79 2d6d 7574 6162 6c65 203e 3d20  hemy-mutable >= 
-000002e0: 312e 302e 320d 0a0d 0a5b 6f70 7469 6f6e  1.0.2....[option
-000002f0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000300: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000310: 0a5b 6275 696c 645f 7370 6869 6e78 5d0d  .[build_sphinx].
-00000320: 0a70 726f 6a65 6374 203d 2048 656d 6c6f  .project = Hemlo
-00000330: 636b 0d0a 636f 7079 7269 6768 7420 3d20  ck..copyright = 
-00000340: 3230 3231 2c20 4469 6c6c 6f6e 2042 6f77  2021, Dillon Bow
-00000350: 656e 0d0a 7265 6c65 6173 6520 3d20 312e  en..release = 1.
-00000360: 302e 300d 0a73 6f75 7263 652d 6469 7220  0.0..source-dir 
-00000370: 3d20 646f 6373 0d0a 0d0a 5b63 6f76 6572  = docs....[cover
-00000380: 6167 653a 7265 706f 7274 5d0d 0a65 7863  age:report]..exc
-00000390: 6c75 6465 5f6c 696e 6573 203d 200d 0a09  lude_lines = ...
-000003a0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-000003b0: 0d0a 090d 0a09 7261 6973 6520 4173 7365  ......raise Asse
-000003c0: 7274 696f 6e45 7272 6f72 0d0a 0972 6169  rtionError...rai
-000003d0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000003e0: 6445 7272 6f72 0d0a 090d 0a09 6966 2054  dError......if T
-000003f0: 5950 455f 4348 4543 4b49 4e47 3a0d 0a09  YPE_CHECKING:...
-00000400: 6966 2030 3a0d 0a09 6966 205f 5f6e 616d  if 0:...if __nam
-00000410: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00000420: 223a 0d0a 6f6d 6974 203d 200d 0a09 7465  ":..omit = ...te
-00000430: 7374 732f 2a0d 0a09 7665 6e76 2f2a 0d0a  sts/*...venv/*..
-00000440: 0d0a 5b6d 7970 795d 0d0a 6967 6e6f 7265  ..[mypy]..ignore
-00000450: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
-00000460: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
-00000470: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000480: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000490: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6865 6d6c 6f63 6b2d 7375 7276 6579  = hemlock-survey
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e31  .version = 1.0.1
+00000030: 0a61 7574 686f 7220 3d20 4469 6c6c 6f6e  .author = Dillon
+00000040: 2042 6f77 656e 0a61 7574 686f 725f 656d   Bowen.author_em
+00000050: 6169 6c20 3d20 6473 626f 7765 6e40 7768  ail = dsbowen@wh
+00000060: 6172 746f 6e2e 7570 656e 6e2e 6564 750a  arton.upenn.edu.
+00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
+00000080: 7079 7468 6f6e 2066 7261 6d65 776f 726b  python framework
+00000090: 2066 6f72 2063 7265 6174 696e 6720 6f6e   for creating on
+000000a0: 6c69 6e65 2073 7572 7665 7973 2061 6e64  line surveys and
+000000b0: 2065 7870 6572 696d 656e 7473 2e0a 6c6f   experiments..lo
+000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000d0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000f0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+00000100: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
+00000110: 726c 203d 2068 7474 7073 3a2f 2f64 7362  rl = https://dsb
+00000120: 6f77 656e 2e67 6974 6c61 622e 696f 2f68  owen.gitlab.io/h
+00000130: 656d 6c6f 636b 0a63 6c61 7373 6966 6965  emlock.classifie
+00000140: 7273 203d 200a 0950 726f 6772 616d 6d69  rs = ..Programmi
+00000150: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000160: 7974 686f 6e20 3a3a 2033 0a09 4c69 6365  ython :: 3..Lice
+00000170: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000180: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000190: 7365 0a09 4f70 6572 6174 696e 6720 5379  se..Operating Sy
+000001a0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001b0: 656e 6465 6e74 0a0a 5b6f 7074 696f 6e73  endent..[options
+000001c0: 5d0a 696e 636c 7564 655f 7061 636b 6167  ].include_packag
+000001d0: 655f 6461 7461 203d 2054 7275 650a 7061  e_data = True.pa
+000001e0: 636b 6167 655f 6469 7220 3d20 0a09 3d20  ckage_dir = ..= 
+000001f0: 7372 630a 7061 636b 6167 6573 203d 2066  src.packages = f
+00000200: 696e 643a 0a70 7974 686f 6e5f 7265 7175  ind:.python_requ
+00000210: 6972 6573 203d 203e 3d33 2e38 0a69 6e73  ires = >=3.8.ins
+00000220: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000230: 0a09 4950 7974 686f 6e0a 0966 6c61 736b  ..IPython..flask
+00000240: 0a09 666c 6173 6b2d 6c6f 6769 6e0a 0966  ..flask-login..f
+00000250: 6c61 736b 2d73 6f63 6b65 7469 6f0a 0966  lask-socketio..f
+00000260: 6c61 736b 2d73 716c 616c 6368 656d 790a  lask-sqlalchemy.
+00000270: 096d 6172 6b64 6f77 6e0a 096d 6174 706c  .markdown..matpl
+00000280: 6f74 6c69 620a 096e 6574 776f 726b 780a  otlib..networkx.
+00000290: 0970 616e 6461 730a 0973 696d 706c 652d  .pandas..simple-
+000002a0: 7765 6273 6f63 6b65 740a 0973 716c 616c  websocket..sqlal
+000002b0: 6368 656d 7920 3c3d 2031 2e34 2e34 390a  chemy <= 1.4.49.
+000002c0: 0973 716c 616c 6368 656d 792d 6d75 7461  .sqlalchemy-muta
+000002d0: 626c 6520 3e3d 2031 2e30 2e32 0a0a 5b6f  ble >= 1.0.2..[o
+000002e0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000002f0: 6669 6e64 5d0a 7768 6572 6520 3d20 7372  find].where = sr
+00000300: 630a 0a5b 6275 696c 645f 7370 6869 6e78  c..[build_sphinx
+00000310: 5d0a 7072 6f6a 6563 7420 3d20 4865 6d6c  ].project = Heml
+00000320: 6f63 6b0a 636f 7079 7269 6768 7420 3d20  ock.copyright = 
+00000330: 3230 3231 2c20 4469 6c6c 6f6e 2042 6f77  2021, Dillon Bow
+00000340: 656e 0a72 656c 6561 7365 203d 2031 2e30  en.release = 1.0
+00000350: 2e31 0a73 6f75 7263 652d 6469 7220 3d20  .1.source-dir = 
+00000360: 646f 6373 0a0a 5b63 6f76 6572 6167 653a  docs..[coverage:
+00000370: 7265 706f 7274 5d0a 6578 636c 7564 655f  report].exclude_
+00000380: 6c69 6e65 7320 3d20 0a09 7072 6167 6d61  lines = ..pragma
+00000390: 3a20 6e6f 2063 6f76 6572 0a09 0a09 7261  : no cover....ra
+000003a0: 6973 6520 4173 7365 7274 696f 6e45 7272  ise AssertionErr
+000003b0: 6f72 0a09 7261 6973 6520 4e6f 7449 6d70  or..raise NotImp
+000003c0: 6c65 6d65 6e74 6564 4572 726f 720a 090a  lementedError...
+000003d0: 0969 6620 5459 5045 5f43 4845 434b 494e  .if TYPE_CHECKIN
+000003e0: 473a 0a09 6966 2030 3a0a 0969 6620 5f5f  G:..if 0:..if __
+000003f0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+00000400: 6e5f 5f22 3a0a 6f6d 6974 203d 200a 0974  n__":.omit = ..t
+00000410: 6573 7473 2f2a 0a09 7665 6e76 2f2a 0a0a  ests/*..venv/*..
+00000420: 5b6d 7970 795d 0a69 676e 6f72 655f 6d69  [mypy].ignore_mi
+00000430: 7373 696e 675f 696d 706f 7274 7320 3d20  ssing_imports = 
+00000440: 5472 7565 0a0a 5b65 6767 5f69 6e66 6f5d  True..[egg_info]
+00000450: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
+00000460: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/_custom_types.py` & `hemlock-survey-1.0.1/src/hemlock/_custom_types.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from __future__ import annotations
-
-from typing import Any, Mapping
-
-from sqlalchemy_mutable import Mutable, MutableDict, MutableList as MutableListBase
-from sqlalchemy_mutable.types import MutableJSONType, MutablePickleType
-from sqlalchemy_mutable.utils import is_instance
-
-
-class MutableList(MutableListBase):
-    def convert_object(self, obj, root):
-        if obj is None:
-            obj = []
-        if not is_instance(obj, list):
-            obj = [obj]
-        return super().convert_object(obj, root)
-
-
-class MutableListJSONType(MutableJSONType):
-    pass
-
-
-MutableList.associate_with(MutableListJSONType)
-
-
-class MutableListPickleType(MutablePickleType):
-    pass
-
-
-MutableList.associate_with(MutableListPickleType)
-
-
-class MutableChoiceList(MutableList):
-    def _convert_item(self, item: Any, root: Mutable = None) -> MutableDict:
-        """Convert a choice item to a dictionary.
-
-        The converted item is an attributes dictionary with at least "value" and
-        "label" keys. Items that are not mappings will be converted to a dictionary.
-        If the item is a tuple, the item is interpreted as a (value, label) tuple.
-        Otherwise, the item is interpreted as both the value and label.
-
-        Args:
-            item (Any): Choice.
-            root (Mutable, optional): Root mutable object. Defaults to None.
-
-        Returns:
-            MutableDict: Converted choice object.
-        """
-        if is_instance(item, Mapping):
-            item = dict(item)
-            item.setdefault("value", None)
-            item.setdefault("label", item["value"])
-            return super()._convert_item(item, root)
-
-        if item is None:
-            value = label = None
-        elif is_instance(item, tuple):
-            value, label = item
-        else:
-            value = label = item
-        return super()._convert_item({"value": value, "label": label}, root)
-
-
-class MutableChoiceListType(MutableJSONType):
-    cache_ok = False
-
-
-MutableChoiceList.associate_with(MutableChoiceListType)
+from __future__ import annotations
+
+from typing import Any, Mapping
+
+from sqlalchemy_mutable import Mutable, MutableDict, MutableList as MutableListBase
+from sqlalchemy_mutable.types import MutableJSONType, MutablePickleType
+from sqlalchemy_mutable.utils import is_instance
+
+
+class MutableList(MutableListBase):
+    def convert_object(self, obj, root):
+        if obj is None:
+            obj = []
+        if not is_instance(obj, list):
+            obj = [obj]
+        return super().convert_object(obj, root)
+
+
+class MutableListJSONType(MutableJSONType):
+    pass
+
+
+MutableList.associate_with(MutableListJSONType)
+
+
+class MutableListPickleType(MutablePickleType):
+    pass
+
+
+MutableList.associate_with(MutableListPickleType)
+
+
+class MutableChoiceList(MutableList):
+    def _convert_item(self, item: Any, root: Mutable = None) -> MutableDict:
+        """Convert a choice item to a dictionary.
+
+        The converted item is an attributes dictionary with at least "value" and
+        "label" keys. Items that are not mappings will be converted to a dictionary.
+        If the item is a tuple, the item is interpreted as a (value, label) tuple.
+        Otherwise, the item is interpreted as both the value and label.
+
+        Args:
+            item (Any): Choice.
+            root (Mutable, optional): Root mutable object. Defaults to None.
+
+        Returns:
+            MutableDict: Converted choice object.
+        """
+        if is_instance(item, Mapping):
+            item = dict(item)
+            item.setdefault("value", None)
+            item.setdefault("label", item["value"])
+            return super()._convert_item(item, root)
+
+        if item is None:
+            value = label = None
+        elif is_instance(item, tuple):
+            value, label = item
+        else:
+            value = label = item
+        return super()._convert_item({"value": value, "label": label}, root)
+
+
+class MutableChoiceListType(MutableJSONType):
+    cache_ok = False
+
+
+MutableChoiceList.associate_with(MutableChoiceListType)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/_data_frame.py` & `hemlock-survey-1.0.1/src/hemlock/_data_frame.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-"""Data frame.
-"""
-from __future__ import annotations
-
-from collections import defaultdict
-from datetime import datetime
-from typing import TYPE_CHECKING, Any, List, Mapping
-
-if TYPE_CHECKING:
-    from .page import Page
-
-from sqlalchemy_mutable.utils import is_instance
-
-
-class DataFrame(defaultdict):
-    """Data frame.
-
-    Subclasses :class:`defaultdict`.
-
-    Args:
-        data (Mapping, optional): Data contained in the dataframe. Defaults to None.
-        fill_rows (bool, optional): Indicates that rows should be filled. Defaults to
-            False.
-
-    Notes:
-
-        "Indicates that rows should be filled" means that, when the data frame is
-        extended, columns with ``filled == True`` should fill the additional rows with
-        the last entry in that column, as opposed to None.
-
-        .. doctest::
-
-            >>> from hemlock._data_frame import DataFrame
-            >>> df = DataFrame({"variable": "data"})
-            >>> df.pad(3)
-            >>> dict(df)
-            {'variable': ['data', None, None]}
-            >>> df = DataFrame({"variable": "data"}, fill_rows=True)
-            >>> df.pad(3)
-            >>> dict(df)
-            {'variable': ['data', 'data', 'data']}
-    """
-
-    def __init__(self, data: Mapping = None, fill_rows: bool = False):
-        super().__init__(lambda: Variable())
-        if data is not None:
-            self.add_data(data, fill_rows)
-
-    def __setitem__(self, key, value):
-        return super().__setitem__(key, Variable(value))
-
-    def add_branch(self, branch: List["Page"]) -> None:
-        """Add data from a given branch to the data frame.
-
-        Args:
-            branch (List[Page]): Branch.
-        """
-        for page in branch:
-            self.add_page(page)
-
-    def add_page(self, page: "Page") -> None:
-        """Add data from a given page to the data frame.
-
-        Args:
-            page (Page): Page.
-        """
-        data_items = [page.timer] + page.data + page.questions
-        for item in data_items:
-            if item.variable:
-                self.add_data(item.pack_data(), item.fill_rows)
-        if page.branch:
-            self.add_branch(page.branch)
-
-    def add_data(self, data: Mapping[Any, Any], fill_rows: bool = False) -> None:
-        """Add data from a mapping to the data frame.
-
-        Args:
-            data (Mapping[Any, Any]): Data.
-            fill_rows (bool, optional): Indicates that rows should be filled. Defaults
-                to False.
-        """
-        if not is_instance(data, dict):
-            data = dict(data)
-        pad_to_row = max([len(self[key]) for key in data.keys()])
-        for key, item in data.items():
-            self[key].add_data(item, fill_rows, pad_to_row)
-
-    def pad(self, min_rows: int = None) -> None:
-        """Pad the data frame so that all variables have the same number of rows.
-
-        Args:
-            min_rows (int, optional): Minimum number of rows to pad the variables to.
-                Defaults to None.
-        """
-        if self:
-            pad_to_row = max([len(item) for item in self.values()])
-            if min_rows is not None:
-                pad_to_row = max(min_rows, pad_to_row)
-            [item.pad(pad_to_row) for item in self.values()]
-
-
-class Variable(list):
-    """Stores the data for one variable (column) of the :class:`DataFrame`.
-
-    Subclasses :class:`list`.
-
-    Attributes:
-        fill_rows (bool): Indicates that rows should be filled.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fill_rows = False
-
-    def add_data(
-        self, data: Any, fill_rows: bool = False, pad_to_row: int = None
-    ) -> None:
-        """Add data to this column.
-
-        Args:
-            data (Any): Data to add.
-            fill_rows (bool, optional): Indicates that rows should be filled. Defaults
-                to False.
-            pad_to_row (int, optional): If not None, pad the data to this number of
-                rows before inserting new data. Defaults to None.
-        """
-        if pad_to_row is not None:
-            self.pad(pad_to_row)
-
-        if not is_instance(data, list):
-            data = [data]
-        self += [str(item) if isinstance(item, datetime) else item for item in data]
-
-        self.fill_rows = fill_rows
-
-    def pad(self, pad_to_row: int) -> None:
-        """Pad the column to a given length.
-
-        Args:
-            pad_to_row (int): Length of the column after padding.
-
-        Raises:
-            ValueError: ``pad_to_row`` must be at least the current column length.
-        """
-        n_additional_rows = pad_to_row - len(self)
-        if n_additional_rows < 0:
-            raise ValueError(
-                f"Attempted to pad variable in {pad_to_row} but the variable has {len(self)} rows already."
-            )
-        padding_data = self[-1] if self.fill_rows and len(self) > 0 else None
-        self += n_additional_rows * [padding_data]
+"""Data frame.
+"""
+from __future__ import annotations
+
+from collections import defaultdict
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, List, Mapping
+
+if TYPE_CHECKING:
+    from .page import Page
+
+from sqlalchemy_mutable.utils import is_instance
+
+
+class DataFrame(defaultdict):
+    """Data frame.
+
+    Subclasses :class:`defaultdict`.
+
+    Args:
+        data (Mapping, optional): Data contained in the dataframe. Defaults to None.
+        fill_rows (bool, optional): Indicates that rows should be filled. Defaults to
+            False.
+
+    Notes:
+
+        "Indicates that rows should be filled" means that, when the data frame is
+        extended, columns with ``filled == True`` should fill the additional rows with
+        the last entry in that column, as opposed to None.
+
+        .. doctest::
+
+            >>> from hemlock._data_frame import DataFrame
+            >>> df = DataFrame({"variable": "data"})
+            >>> df.pad(3)
+            >>> dict(df)
+            {'variable': ['data', None, None]}
+            >>> df = DataFrame({"variable": "data"}, fill_rows=True)
+            >>> df.pad(3)
+            >>> dict(df)
+            {'variable': ['data', 'data', 'data']}
+    """
+
+    def __init__(self, data: Mapping = None, fill_rows: bool = False):
+        super().__init__(lambda: Variable())
+        if data is not None:
+            self.add_data(data, fill_rows)
+
+    def __setitem__(self, key, value):
+        return super().__setitem__(key, Variable(value))
+
+    def add_branch(self, branch: List["Page"]) -> None:
+        """Add data from a given branch to the data frame.
+
+        Args:
+            branch (List[Page]): Branch.
+        """
+        for page in branch:
+            self.add_page(page)
+
+    def add_page(self, page: "Page") -> None:
+        """Add data from a given page to the data frame.
+
+        Args:
+            page (Page): Page.
+        """
+        data_items = [page.timer] + page.data + page.questions
+        for item in data_items:
+            if item.variable:
+                self.add_data(item.pack_data(), item.fill_rows)
+        if page.branch:
+            self.add_branch(page.branch)
+
+    def add_data(self, data: Mapping[Any, Any], fill_rows: bool = False) -> None:
+        """Add data from a mapping to the data frame.
+
+        Args:
+            data (Mapping[Any, Any]): Data.
+            fill_rows (bool, optional): Indicates that rows should be filled. Defaults
+                to False.
+        """
+        if not is_instance(data, dict):
+            data = dict(data)
+        pad_to_row = max([len(self[key]) for key in data.keys()])
+        for key, item in data.items():
+            self[key].add_data(item, fill_rows, pad_to_row)
+
+    def pad(self, min_rows: int = None) -> None:
+        """Pad the data frame so that all variables have the same number of rows.
+
+        Args:
+            min_rows (int, optional): Minimum number of rows to pad the variables to.
+                Defaults to None.
+        """
+        if self:
+            pad_to_row = max([len(item) for item in self.values()])
+            if min_rows is not None:
+                pad_to_row = max(min_rows, pad_to_row)
+            [item.pad(pad_to_row) for item in self.values()]
+
+
+class Variable(list):
+    """Stores the data for one variable (column) of the :class:`DataFrame`.
+
+    Subclasses :class:`list`.
+
+    Attributes:
+        fill_rows (bool): Indicates that rows should be filled.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fill_rows = False
+
+    def add_data(
+        self, data: Any, fill_rows: bool = False, pad_to_row: int = None
+    ) -> None:
+        """Add data to this column.
+
+        Args:
+            data (Any): Data to add.
+            fill_rows (bool, optional): Indicates that rows should be filled. Defaults
+                to False.
+            pad_to_row (int, optional): If not None, pad the data to this number of
+                rows before inserting new data. Defaults to None.
+        """
+        if pad_to_row is not None:
+            self.pad(pad_to_row)
+
+        if not is_instance(data, list):
+            data = [data]
+        self += [str(item) if isinstance(item, datetime) else item for item in data]
+
+        self.fill_rows = fill_rows
+
+    def pad(self, pad_to_row: int) -> None:
+        """Pad the column to a given length.
+
+        Args:
+            pad_to_row (int): Length of the column after padding.
+
+        Raises:
+            ValueError: ``pad_to_row`` must be at least the current column length.
+        """
+        n_additional_rows = pad_to_row - len(self)
+        if n_additional_rows < 0:
+            raise ValueError(
+                f"Attempted to pad variable in {pad_to_row} but the variable has {len(self)} rows already."
+            )
+        padding_data = self[-1] if self.fill_rows and len(self) > 0 else None
+        self += n_additional_rows * [padding_data]
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/_display_navigation.py` & `hemlock-survey-1.0.1/src/hemlock/_display_navigation.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-"""Navigation display.
-
-Displays possible user navigation through a tree.
-"""
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple
-
-import matplotlib.pyplot as plt
-import networkx as nx
-
-if TYPE_CHECKING:  # pragma: no cover
-    from .tree import Tree
-    from .page import Page
-
-Y_INCREMENT = 0.015
-
-DEFAULT_NODE_COLOR = "#cfe2ff"
-CURRENT_NODE_COLOR = "#d1e7dd"
-TERMINAL_NODE_COLOR = "#f8d7da"
-
-DEFAULT_EDGE_COLOR = "#b6d4fe"
-CURRENT_EDGE_COLOR = "#badbcc"
-TERMINAL_EDGE_COLOR = "#f5c2c7"
-
-EdgeType = Tuple["Page", "Page"]
-# tuple of (list of edges), connection style (str)
-EdgelistType = Tuple[List[EdgeType], str]
-
-
-class Node:
-    """Node of the navigation graph.
-
-    Args:
-        page (Page): Page represented by this node.
-        pos (Tuple[float, float]): Position of the node in graph.
-
-    Attributes:
-        page (Page): Page represented by this node.
-        pos (Tuple[float, float]): Position of the node in graph.
-        children (List[Node]): Nodes to which the user can navigate from this node.
-        color (str): Color of this node.
-        edgecolor (str): Color of the edge of this node.
-        subgraph (Graph): Graph representing this page's branch.
-    """
-
-    def __init__(self, page: Page, pos: Tuple[float, float]):
-        self.page = page
-        self.children: List[Node] = []
-        self.pos = pos
-
-        self.color = DEFAULT_NODE_COLOR
-        if page.is_last_page:
-            self.color = TERMINAL_NODE_COLOR
-
-        self.edgecolor = DEFAULT_EDGE_COLOR
-        if page.is_last_page:
-            self.edgecolor = TERMINAL_EDGE_COLOR
-
-        if page.branch:
-            self.subgraph = Graph(page.branch, self)
-        else:
-            self.subgraph = None  # type: ignore
-
-    def __len__(self):
-        return 1 + (0 if self.subgraph is None else len(self.subgraph))
-
-    def connect(self, prev_node: Node) -> None:
-        """Draw a connection from the prev_node to this node.
-
-        Args:
-            prev_node (Node): Node to connect.
-        """
-        if prev_node.subgraph is None:
-            if prev_node.page.forward and prev_node.page.next_page is None:
-                prev_node.children.append(self)
-            if self.page.back and self.page.prev_page is None:
-                self.children.append(prev_node)
-        else:
-            self.connect(prev_node.subgraph.nodes[-1])
-
-    def get_attributes(self) -> Dict[str, Any]:
-        """Get attributes of this node and its subgraph.
-
-        Returns:
-            Dict[str, Any]: Attributes.
-        """
-        attrs = dict(
-            nodes=[self.page],
-            labels={self.page: self.page.get_position()},
-            pos={self.page: self.pos},
-            node_color=[self.color],
-            edgecolors=[self.edgecolor],
-            edges=[(self.page, child.page) for child in self.children],
-        )
-        if self.subgraph is not None:
-            for key, value in self.subgraph.get_attributes().items():
-                if key in ("labels", "pos"):
-                    attrs[key].update(value)  # type: ignore
-                else:
-                    attrs[key] += value
-
-        return attrs
-
-
-class Graph:
-    """Graph representing a branch.
-
-    Args:
-        branch (List[Page]): Branch represented by this graph.
-        origin_node (Node, optional): Root node for this branch. Defaults to None.
-
-    Attributes:
-        branch (List[Page]): Branch represented by this graph.
-        nodes (List[Node]): Nodes representing the pages of this branch.
-    """
-
-    def __init__(self, branch: List[Page], origin_node: Node = None):
-        self.branch = branch
-        self.nodes: List[Node] = []
-
-        start_x, start_y = 0.0, 0.0
-        if origin_node is not None:
-            start_x = origin_node.pos[0] + 1
-            start_y = origin_node.pos[1] + Y_INCREMENT
-
-        i = 0
-        for page in branch:
-            node = Node(page, (start_x + i, start_y))
-            i += len(node)
-            if self.nodes:
-                node.connect(self.nodes[-1])
-            self.nodes.append(node)
-
-        if origin_node is not None:
-            if origin_node.page.forward:
-                origin_node.children.append(self.nodes[0])
-            if branch[0].back:
-                self.nodes[0].children.append(origin_node)
-
-    def __len__(self):
-        return sum([len(node) for node in self.nodes])
-
-    def get_attributes(self) -> Dict[str, Any]:
-        """Get attributes of this graph's nodes and their subgraphs.
-
-        Returns:
-            Dict[str, Any]: Attributes.
-        """
-        attrs: Dict[str, Any] = dict(
-            nodes=[],
-            labels={},
-            pos={},
-            node_color=[],
-            edgecolors=[],
-            edges=[],
-        )
-        for node in self.nodes:
-            for key, value in node.get_attributes().items():
-                if key in ("labels", "pos"):
-                    attrs[key].update(value)  # type: ignore
-                else:
-                    attrs[key] += value
-
-        return attrs
-
-
-def make_digraph(
-    tree: Tree,
-) -> Tuple[
-    nx.classes.digraph.DiGraph, Dict[str, Any], Tuple[EdgelistType, EdgelistType]
-]:
-    """Create a networkx digraph based on a tree.
-
-    Args:
-        tree (Tree): Tree to represent as a graph.
-
-    Returns:
-        Tuple[
-            nx.classes.digraph.DiGraph,
-            Dict[str, Any],
-            Tuple[EdgelistType, EdgelistType]
-        ]: Digraph, graph attributes, tuple of straight and curved edges.
-    """
-    graph = Graph(tree.branch)
-    attrs = graph.get_attributes()
-    for i, page in enumerate(attrs["nodes"]):
-        if page is tree.page:
-            attrs["node_color"][i] = CURRENT_NODE_COLOR
-            if not page.is_last_page:
-                attrs["edgecolors"][i] = CURRENT_EDGE_COLOR
-
-    curved_edges = []
-    for page in attrs["nodes"]:
-        if page.forward and page.next_page is not None:
-            curved_edges.append((page, page.next_page))
-
-        if page.back and page.prev_page is not None:
-            curved_edges.append((page, page.prev_page))
-
-    edgelist_connectionstyle = (
-        (attrs["edges"], "arc3"),
-        (curved_edges, "arc3,rad=-.4"),
-    )
-
-    nx_graph = nx.DiGraph()
-    nx_graph.add_nodes_from(attrs["nodes"])
-    nx_graph.add_edges_from(attrs["edges"] + curved_edges)
-
-    return nx_graph, attrs, edgelist_connectionstyle
-
-
-def display_navigation(
-    tree: Tree, ax=None, node_size: int = 1200, **subplots_kwargs: Any
-):
-    """Display the navigation graph of a given tree.
-
-    Args:
-        tree (Tree): Tree to display.
-        ax (AxesSubplot): Axis on which to draw the graph.
-        node_size (int, optional): Size of the nodes in the graph. Defaults to 1200.
-
-    Returns:
-        AxesSubplot: Graph.
-    """
-    if ax is None:
-        _, ax = plt.subplots(**subplots_kwargs)
-        ax.set_facecolor("whitesmoke")
-
-    nx_graph, attrs, edgelist_connectionstyle = make_digraph(tree)
-    nx.draw_networkx_nodes(
-        nx_graph,
-        attrs["pos"],
-        ax=ax,
-        node_color=attrs["node_color"],
-        edgecolors=attrs["edgecolors"],
-        linewidths=3,
-        node_size=node_size,
-    )
-    for edgelist, connectionstyle in edgelist_connectionstyle:
-        nx.draw_networkx_edges(
-            nx_graph,
-            attrs["pos"],
-            edgelist=edgelist,
-            connectionstyle=connectionstyle,
-            ax=ax,
-            arrowsize=20,
-            node_size=node_size,
-        )
-    nx.draw_networkx_labels(nx_graph, attrs["pos"], ax=ax, labels=attrs["labels"])
-
-    return ax
+"""Navigation display.
+
+Displays possible user navigation through a tree.
+"""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple
+
+import matplotlib.pyplot as plt
+import networkx as nx
+
+if TYPE_CHECKING:  # pragma: no cover
+    from .tree import Tree
+    from .page import Page
+
+Y_INCREMENT = 0.015
+
+DEFAULT_NODE_COLOR = "#cfe2ff"
+CURRENT_NODE_COLOR = "#d1e7dd"
+TERMINAL_NODE_COLOR = "#f8d7da"
+
+DEFAULT_EDGE_COLOR = "#b6d4fe"
+CURRENT_EDGE_COLOR = "#badbcc"
+TERMINAL_EDGE_COLOR = "#f5c2c7"
+
+EdgeType = Tuple["Page", "Page"]
+# tuple of (list of edges), connection style (str)
+EdgelistType = Tuple[List[EdgeType], str]
+
+
+class Node:
+    """Node of the navigation graph.
+
+    Args:
+        page (Page): Page represented by this node.
+        pos (Tuple[float, float]): Position of the node in graph.
+
+    Attributes:
+        page (Page): Page represented by this node.
+        pos (Tuple[float, float]): Position of the node in graph.
+        children (List[Node]): Nodes to which the user can navigate from this node.
+        color (str): Color of this node.
+        edgecolor (str): Color of the edge of this node.
+        subgraph (Graph): Graph representing this page's branch.
+    """
+
+    def __init__(self, page: Page, pos: Tuple[float, float]):
+        self.page = page
+        self.children: List[Node] = []
+        self.pos = pos
+
+        self.color = DEFAULT_NODE_COLOR
+        if page.is_last_page:
+            self.color = TERMINAL_NODE_COLOR
+
+        self.edgecolor = DEFAULT_EDGE_COLOR
+        if page.is_last_page:
+            self.edgecolor = TERMINAL_EDGE_COLOR
+
+        if page.branch:
+            self.subgraph = Graph(page.branch, self)
+        else:
+            self.subgraph = None  # type: ignore
+
+    def __len__(self):
+        return 1 + (0 if self.subgraph is None else len(self.subgraph))
+
+    def connect(self, prev_node: Node) -> None:
+        """Draw a connection from the prev_node to this node.
+
+        Args:
+            prev_node (Node): Node to connect.
+        """
+        if prev_node.subgraph is None:
+            if prev_node.page.forward and prev_node.page.next_page is None:
+                prev_node.children.append(self)
+            if self.page.back and self.page.prev_page is None:
+                self.children.append(prev_node)
+        else:
+            self.connect(prev_node.subgraph.nodes[-1])
+
+    def get_attributes(self) -> Dict[str, Any]:
+        """Get attributes of this node and its subgraph.
+
+        Returns:
+            Dict[str, Any]: Attributes.
+        """
+        attrs = dict(
+            nodes=[self.page],
+            labels={self.page: self.page.get_position()},
+            pos={self.page: self.pos},
+            node_color=[self.color],
+            edgecolors=[self.edgecolor],
+            edges=[(self.page, child.page) for child in self.children],
+        )
+        if self.subgraph is not None:
+            for key, value in self.subgraph.get_attributes().items():
+                if key in ("labels", "pos"):
+                    attrs[key].update(value)  # type: ignore
+                else:
+                    attrs[key] += value
+
+        return attrs
+
+
+class Graph:
+    """Graph representing a branch.
+
+    Args:
+        branch (List[Page]): Branch represented by this graph.
+        origin_node (Node, optional): Root node for this branch. Defaults to None.
+
+    Attributes:
+        branch (List[Page]): Branch represented by this graph.
+        nodes (List[Node]): Nodes representing the pages of this branch.
+    """
+
+    def __init__(self, branch: List[Page], origin_node: Node = None):
+        self.branch = branch
+        self.nodes: List[Node] = []
+
+        start_x, start_y = 0.0, 0.0
+        if origin_node is not None:
+            start_x = origin_node.pos[0] + 1
+            start_y = origin_node.pos[1] + Y_INCREMENT
+
+        i = 0
+        for page in branch:
+            node = Node(page, (start_x + i, start_y))
+            i += len(node)
+            if self.nodes:
+                node.connect(self.nodes[-1])
+            self.nodes.append(node)
+
+        if origin_node is not None:
+            if origin_node.page.forward:
+                origin_node.children.append(self.nodes[0])
+            if branch[0].back:
+                self.nodes[0].children.append(origin_node)
+
+    def __len__(self):
+        return sum([len(node) for node in self.nodes])
+
+    def get_attributes(self) -> Dict[str, Any]:
+        """Get attributes of this graph's nodes and their subgraphs.
+
+        Returns:
+            Dict[str, Any]: Attributes.
+        """
+        attrs: Dict[str, Any] = dict(
+            nodes=[],
+            labels={},
+            pos={},
+            node_color=[],
+            edgecolors=[],
+            edges=[],
+        )
+        for node in self.nodes:
+            for key, value in node.get_attributes().items():
+                if key in ("labels", "pos"):
+                    attrs[key].update(value)  # type: ignore
+                else:
+                    attrs[key] += value
+
+        return attrs
+
+
+def make_digraph(
+    tree: Tree,
+) -> Tuple[
+    nx.classes.digraph.DiGraph, Dict[str, Any], Tuple[EdgelistType, EdgelistType]
+]:
+    """Create a networkx digraph based on a tree.
+
+    Args:
+        tree (Tree): Tree to represent as a graph.
+
+    Returns:
+        Tuple[
+            nx.classes.digraph.DiGraph,
+            Dict[str, Any],
+            Tuple[EdgelistType, EdgelistType]
+        ]: Digraph, graph attributes, tuple of straight and curved edges.
+    """
+    graph = Graph(tree.branch)
+    attrs = graph.get_attributes()
+    for i, page in enumerate(attrs["nodes"]):
+        if page is tree.page:
+            attrs["node_color"][i] = CURRENT_NODE_COLOR
+            if not page.is_last_page:
+                attrs["edgecolors"][i] = CURRENT_EDGE_COLOR
+
+    curved_edges = []
+    for page in attrs["nodes"]:
+        if page.forward and page.next_page is not None:
+            curved_edges.append((page, page.next_page))
+
+        if page.back and page.prev_page is not None:
+            curved_edges.append((page, page.prev_page))
+
+    edgelist_connectionstyle = (
+        (attrs["edges"], "arc3"),
+        (curved_edges, "arc3,rad=-.4"),
+    )
+
+    nx_graph = nx.DiGraph()
+    nx_graph.add_nodes_from(attrs["nodes"])
+    nx_graph.add_edges_from(attrs["edges"] + curved_edges)
+
+    return nx_graph, attrs, edgelist_connectionstyle
+
+
+def display_navigation(
+    tree: Tree, ax=None, node_size: int = 1200, **subplots_kwargs: Any
+):
+    """Display the navigation graph of a given tree.
+
+    Args:
+        tree (Tree): Tree to display.
+        ax (AxesSubplot): Axis on which to draw the graph.
+        node_size (int, optional): Size of the nodes in the graph. Defaults to 1200.
+
+    Returns:
+        AxesSubplot: Graph.
+    """
+    if ax is None:
+        _, ax = plt.subplots(**subplots_kwargs)
+        ax.set_facecolor("whitesmoke")
+
+    nx_graph, attrs, edgelist_connectionstyle = make_digraph(tree)
+    nx.draw_networkx_nodes(
+        nx_graph,
+        attrs["pos"],
+        ax=ax,
+        node_color=attrs["node_color"],
+        edgecolors=attrs["edgecolors"],
+        linewidths=3,
+        node_size=node_size,
+    )
+    for edgelist, connectionstyle in edgelist_connectionstyle:
+        nx.draw_networkx_edges(
+            nx_graph,
+            attrs["pos"],
+            edgelist=edgelist,
+            connectionstyle=connectionstyle,
+            ax=ax,
+            arrowsize=20,
+            node_size=node_size,
+        )
+    nx.draw_networkx_labels(nx_graph, attrs["pos"], ax=ax, labels=attrs["labels"])
+
+    return ax
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/_navbar.py` & `hemlock-survey-1.0.1/src/hemlock/_navbar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-"""Navbar.
-"""
-from __future__ import annotations
-
-from typing import Dict, Iterable, List, Mapping, Tuple, Union
-
-RawDropdownItem = Union[str, Tuple[str, str], Mapping[str, Union[str, bool]]]
-DropdownItem = Dict[str, str]
-RawNavitemTuple = Tuple[str, Union[str, Iterable[DropdownItem]]]
-RawNavitem = Union[
-    str, RawNavitemTuple, Mapping[str, Union[str, bool, RawNavitemTuple]]
-]
-Navitem = Dict[str, Union[str, List[DropdownItem]]]
-RawBrand = Union[str, Tuple[str, str], Mapping[str, str]]
-Brand = Dict[str, str]
-Navbar = Dict[str, Union[str, Brand, List[Navitem]]]
-
-
-def convert_brand(brand: RawBrand) -> Brand:
-    """Convert navbar brand.
-
-    Args:
-        brand (RawBrand): Brand. If a string, this is the brand label. If a tuple, the
-            brand will be interpreted as a (label, href) tuple.
-
-    Raises:
-        ValueError: Brand must be a string, tuple, or mapping.
-
-    Returns:
-        Brand: Converted brand.
-    """
-    converted = {"label": "", "href": "#", "raw_html": ""}
-    if isinstance(brand, str):
-        converted["label"] = brand
-    elif isinstance(brand, tuple):
-        converted.update({"label": brand[0], "href": brand[1]})
-    elif isinstance(brand, Mapping):
-        converted.update(brand)
-    else:
-        raise ValueError(f"brand must be a string, tuple, or mapping, got {brand}.")
-
-    return converted
-
-
-def convert_navitem(item: RawNavitem) -> Navitem:
-    """Convert a navitem.
-
-    Args:
-        item (RawNavitem): Navitem. If a string, this is the navitem label. If a tuple,
-            the navitem will either be interpreted as a (label, href) tuple or a (label,
-            dropdown items) tuple.
-
-    Raises:
-        ValueError: If a tuple, the second element must be an href (str) or dropdown
-            items (iterable).
-        ValueError: Navitem must be a string, tuple, or mapping.
-
-    Returns:
-        Navitem: Converted navitem.
-    """
-    converted = {
-        "label": "",
-        "href": "#",
-        "dropdown_items": [],
-        "disabled": False,
-        "raw_html": "",
-    }
-    if isinstance(item, str):
-        converted["label"] = item
-    elif isinstance(item, tuple):
-        converted["label"] = item[0]
-        if isinstance(item[1], str):
-            converted["href"] = item[1]
-        elif isinstance(item[1], (list, tuple)):
-            converted["dropdown_items"] = [convert_dropdown_item(i) for i in item[1]]
-        else:
-            raise ValueError(
-                f"Second element of item should be a string (href) or a list or tuple of dropdown items, got {item[1]}"
-            )
-    elif isinstance(item, Mapping):
-        converted.update(item)
-    else:
-        raise ValueError(f"navitem must be a string, tuple, or mapping, got {item}")
-
-    converted["disabled"] = "disabled" if converted["disabled"] else ""
-    return converted  # type: ignore
-
-
-def convert_dropdown_item(item: RawDropdownItem) -> DropdownItem:
-    """Convert a dropdown item.
-
-    Args:
-        item (RawDropdownItem): Dropdown item. If a string, this is the item label. If a
-            tuple, this is interpreted as a (label, href) tuple.
-
-    Raises:
-        ValueError: Item must be a string, tuple, or mapping.
-
-    Returns:
-        DropdownItem: Converted dropdown item.
-    """
-    converted = {"label": "", "href": "#", "disabled": False, "raw_html": ""}
-    if isinstance(item, str):
-        converted["label"] = item
-    elif isinstance(item, tuple):
-        converted.update({"label": item[0], "href": item[1]})
-    elif isinstance(item, Mapping):
-        converted.update(item)
-    else:
-        raise ValueError(f"item must be a string, tuple, or mapping, got {item}.")
-
-    converted["disabled"] = "disabled" if converted["disabled"] else ""
-    return converted  # type: ignore
+"""Navbar.
+"""
+from __future__ import annotations
+
+from typing import Dict, Iterable, List, Mapping, Tuple, Union
+
+RawDropdownItem = Union[str, Tuple[str, str], Mapping[str, Union[str, bool]]]
+DropdownItem = Dict[str, str]
+RawNavitemTuple = Tuple[str, Union[str, Iterable[DropdownItem]]]
+RawNavitem = Union[
+    str, RawNavitemTuple, Mapping[str, Union[str, bool, RawNavitemTuple]]
+]
+Navitem = Dict[str, Union[str, List[DropdownItem]]]
+RawBrand = Union[str, Tuple[str, str], Mapping[str, str]]
+Brand = Dict[str, str]
+Navbar = Dict[str, Union[str, Brand, List[Navitem]]]
+
+
+def convert_brand(brand: RawBrand) -> Brand:
+    """Convert navbar brand.
+
+    Args:
+        brand (RawBrand): Brand. If a string, this is the brand label. If a tuple, the
+            brand will be interpreted as a (label, href) tuple.
+
+    Raises:
+        ValueError: Brand must be a string, tuple, or mapping.
+
+    Returns:
+        Brand: Converted brand.
+    """
+    converted = {"label": "", "href": "#", "raw_html": ""}
+    if isinstance(brand, str):
+        converted["label"] = brand
+    elif isinstance(brand, tuple):
+        converted.update({"label": brand[0], "href": brand[1]})
+    elif isinstance(brand, Mapping):
+        converted.update(brand)
+    else:
+        raise ValueError(f"brand must be a string, tuple, or mapping, got {brand}.")
+
+    return converted
+
+
+def convert_navitem(item: RawNavitem) -> Navitem:
+    """Convert a navitem.
+
+    Args:
+        item (RawNavitem): Navitem. If a string, this is the navitem label. If a tuple,
+            the navitem will either be interpreted as a (label, href) tuple or a (label,
+            dropdown items) tuple.
+
+    Raises:
+        ValueError: If a tuple, the second element must be an href (str) or dropdown
+            items (iterable).
+        ValueError: Navitem must be a string, tuple, or mapping.
+
+    Returns:
+        Navitem: Converted navitem.
+    """
+    converted = {
+        "label": "",
+        "href": "#",
+        "dropdown_items": [],
+        "disabled": False,
+        "raw_html": "",
+    }
+    if isinstance(item, str):
+        converted["label"] = item
+    elif isinstance(item, tuple):
+        converted["label"] = item[0]
+        if isinstance(item[1], str):
+            converted["href"] = item[1]
+        elif isinstance(item[1], (list, tuple)):
+            converted["dropdown_items"] = [convert_dropdown_item(i) for i in item[1]]
+        else:
+            raise ValueError(
+                f"Second element of item should be a string (href) or a list or tuple of dropdown items, got {item[1]}"
+            )
+    elif isinstance(item, Mapping):
+        converted.update(item)
+    else:
+        raise ValueError(f"navitem must be a string, tuple, or mapping, got {item}")
+
+    converted["disabled"] = "disabled" if converted["disabled"] else ""
+    return converted  # type: ignore
+
+
+def convert_dropdown_item(item: RawDropdownItem) -> DropdownItem:
+    """Convert a dropdown item.
+
+    Args:
+        item (RawDropdownItem): Dropdown item. If a string, this is the item label. If a
+            tuple, this is interpreted as a (label, href) tuple.
+
+    Raises:
+        ValueError: Item must be a string, tuple, or mapping.
+
+    Returns:
+        DropdownItem: Converted dropdown item.
+    """
+    converted = {"label": "", "href": "#", "disabled": False, "raw_html": ""}
+    if isinstance(item, str):
+        converted["label"] = item
+    elif isinstance(item, tuple):
+        converted.update({"label": item[0], "href": item[1]})
+    elif isinstance(item, Mapping):
+        converted.update(item)
+    else:
+        raise ValueError(f"item must be a string, tuple, or mapping, got {item}.")
+
+    converted["disabled"] = "disabled" if converted["disabled"] else ""
+    return converted  # type: ignore
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/_user_routes.py` & `hemlock-survey-1.0.1/src/hemlock/_user_routes.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-"""User routes.
-"""
-from __future__ import annotations
-
-import copy
-from typing import Tuple, Union
-from urllib.parse import urlparse, parse_qs
-
-from flask import current_app, request, url_for
-from flask_login import current_user, login_required, logout_user
-from werkzeug.wrappers import Response
-
-from .app import bp, db, static_pages
-from .page import Page
-from .questions import Label
-from .user import User
-from .utils import redirect
-
-
-@bp.route("/")
-def index() -> Response:
-    """Redirect the client.
-
-    The client may be redirected to the screenout page, the restart page, or the first
-    page of the study.
-
-    Returns:
-        Response: Redirect.
-    """
-
-    def matching_record_found(mapping):
-        return any([value in mapping.get(key, []) for key, value in meta_data.items()])
-
-    if "next" in request.args:
-        # get querystring arguments from the redirect
-        parsed_url = urlparse(request.args["next"])
-        meta_data = dict(parse_qs(parsed_url.query))
-        meta_data = {
-            key: (value[0] if len(value) == 1 else value)
-            for key, value in meta_data.items()
-        }
-        meta_data["next"] = parsed_url.path
-    else:
-        meta_data = dict(request.args)
-
-    meta_data["ipv4"] = request.remote_addr  # type: ignore
-
-    if matching_record_found(current_app.config["SCREENOUT_RECORDS"]):
-        return redirect(url_for("hemlock.screenout"))
-
-    if current_user.is_authenticated:
-        if (
-            current_user.get_tree().page.is_first_page
-            or not current_app.config["ALLOW_USERS_TO_RESTART"]
-        ):
-            return redirect(User.default_url_rule)  # type: ignore
-        return redirect(url_for("hemlock.restart"))
-
-    if matching_record_found(user_metadata := current_app.config["USER_METADATA"]):
-        return redirect(url_for("hemlock.screenout"))
-
-    for key, value in meta_data.items():
-        if key in current_app.config["BLOCK_DUPLICATE_KEYS"]:
-            user_metadata[key].append(value)
-
-    User(meta_data=meta_data)
-    db.session.commit()
-    return redirect(User.default_url_rule)  # type: ignore
-
-
-@bp.route("/screenout")
-def screenout() -> str:
-    """Screenout page.
-
-    Returns:
-        str: Screenout page.
-    """
-    screenout_page_key = "screenout"
-    if screenout_page_key not in static_pages:
-        static_pages[screenout_page_key] = Page(
-            Label(
-                """
-                Our records indicate that you have already participated in this or 
-                similar surveys.
-                
-                Thank you for your continuing interest in our research!
-                """
-            ),
-            navbar=None,
-            back=False,
-            forward=False,
-        ).render()
-
-    return static_pages[screenout_page_key]
-
-
-@bp.route("/restart", methods=["GET", "POST"])
-@login_required
-def restart() -> Union[str, Response]:
-    """Restart page.
-
-    Returns:
-        Union[str, Response]: Restart page or redirect to study.
-    """
-    if request.method == "POST":
-        if request.form.get("direction") == "forward":
-            meta_data = copy.deepcopy(current_user.meta_data)
-            logout_user()
-            User(meta_data=meta_data)
-            db.session.commit()
-
-        return redirect(User.default_url_rule)  # type: ignore
-
-    restart_page_key = "restart"
-    if restart_page_key not in static_pages:
-        static_pages[restart_page_key] = Page(
-            Label(
-                """
-                You have already started this survey. Click "Resume" to pick up where 
-                you left off or "Restart" to start the survey from the beginning.
-
-                If you restart the survey, your responses will not be saved.
-                """
-            ),
-            back="Resume",
-            forward="Restart",
-        ).render()
-
-    return static_pages[restart_page_key]
-
-
-@bp.errorhandler(500)
-def internal_server_error(error) -> Tuple[str, int]:
-    """Handle internal server error."""
-    current_user.errored = True
-    db.session.commit()
-
-    internal_server_error_page_key = "500"
-    if internal_server_error_page_key not in static_pages:
-        static_pages[internal_server_error_page_key] = Page(
-            Label(
-                """
-                The application encountered an error. Please contact the survey 
-                administrator.
-
-                We apologize for the inconvenience and thank you for your patience as we 
-                work to resolve this issue.
-                """
-            ),
-            navbar=None,
-            back=False,
-            forward=False,
-        ).render()
-
-    return static_pages[internal_server_error_page_key], 500
+"""User routes.
+"""
+from __future__ import annotations
+
+import copy
+from typing import Tuple, Union
+from urllib.parse import urlparse, parse_qs
+
+from flask import current_app, request, url_for
+from flask_login import current_user, login_required, logout_user
+from werkzeug.wrappers import Response
+
+from .app import bp, db, static_pages
+from .page import Page
+from .questions import Label
+from .user import User
+from .utils import redirect
+
+
+@bp.route("/")
+def index() -> Response:
+    """Redirect the client.
+
+    The client may be redirected to the screenout page, the restart page, or the first
+    page of the study.
+
+    Returns:
+        Response: Redirect.
+    """
+
+    def matching_record_found(mapping):
+        return any([value in mapping.get(key, []) for key, value in meta_data.items()])
+
+    if "next" in request.args:
+        # get querystring arguments from the redirect
+        parsed_url = urlparse(request.args["next"])
+        meta_data = dict(parse_qs(parsed_url.query))
+        meta_data = {
+            key: (value[0] if len(value) == 1 else value)
+            for key, value in meta_data.items()
+        }
+        meta_data["next"] = parsed_url.path
+    else:
+        meta_data = dict(request.args)
+
+    meta_data["ipv4"] = request.remote_addr  # type: ignore
+
+    if matching_record_found(current_app.config["SCREENOUT_RECORDS"]):
+        return redirect(url_for("hemlock.screenout"))
+
+    if current_user.is_authenticated:
+        if (
+            current_user.get_tree().page.is_first_page
+            or not current_app.config["ALLOW_USERS_TO_RESTART"]
+        ):
+            return redirect(User.default_url_rule)  # type: ignore
+        return redirect(url_for("hemlock.restart"))
+
+    if matching_record_found(user_metadata := current_app.config["USER_METADATA"]):
+        return redirect(url_for("hemlock.screenout"))
+
+    for key, value in meta_data.items():
+        if key in current_app.config["BLOCK_DUPLICATE_KEYS"]:
+            user_metadata[key].append(value)
+
+    User(meta_data=meta_data)
+    db.session.commit()
+    return redirect(User.default_url_rule)  # type: ignore
+
+
+@bp.route("/screenout")
+def screenout() -> str:
+    """Screenout page.
+
+    Returns:
+        str: Screenout page.
+    """
+    screenout_page_key = "screenout"
+    if screenout_page_key not in static_pages:
+        static_pages[screenout_page_key] = Page(
+            Label(
+                """
+                Our records indicate that you have already participated in this or 
+                similar surveys.
+                
+                Thank you for your continuing interest in our research!
+                """
+            ),
+            navbar=None,
+            back=False,
+            forward=False,
+        ).render()
+
+    return static_pages[screenout_page_key]
+
+
+@bp.route("/restart", methods=["GET", "POST"])
+@login_required
+def restart() -> Union[str, Response]:
+    """Restart page.
+
+    Returns:
+        Union[str, Response]: Restart page or redirect to study.
+    """
+    if request.method == "POST":
+        if request.form.get("direction") == "forward":
+            meta_data = copy.deepcopy(current_user.meta_data)
+            logout_user()
+            User(meta_data=meta_data)
+            db.session.commit()
+
+        return redirect(User.default_url_rule)  # type: ignore
+
+    restart_page_key = "restart"
+    if restart_page_key not in static_pages:
+        static_pages[restart_page_key] = Page(
+            Label(
+                """
+                You have already started this survey. Click "Resume" to pick up where 
+                you left off or "Restart" to start the survey from the beginning.
+
+                If you restart the survey, your responses will not be saved.
+                """
+            ),
+            back="Resume",
+            forward="Restart",
+        ).render()
+
+    return static_pages[restart_page_key]
+
+
+@bp.errorhandler(500)
+def internal_server_error(error) -> Tuple[str, int]:
+    """Handle internal server error."""
+    current_user.errored = True
+    db.session.commit()
+
+    internal_server_error_page_key = "500"
+    if internal_server_error_page_key not in static_pages:
+        static_pages[internal_server_error_page_key] = Page(
+            Label(
+                """
+                The application encountered an error. Please contact the survey 
+                administrator.
+
+                We apologize for the inconvenience and thank you for your patience as we 
+                work to resolve this issue.
+                """
+            ),
+            navbar=None,
+            back=False,
+            forward=False,
+        ).render()
+
+    return static_pages[internal_server_error_page_key], 500
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/app.py` & `hemlock-survey-1.0.1/src/hemlock/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""Application utilities.
-"""
-from __future__ import annotations
-
-import os
-from collections import defaultdict
-from typing import Any, Dict, List, Mapping, Union
-
-from flask import Blueprint, Flask
-from flask_login import LoginManager
-from flask_socketio import SocketIO
-from flask_sqlalchemy import SQLAlchemy
-from sqlalchemy_mutable import Mutable
-from werkzeug.security import generate_password_hash
-
-# create blueprint and extensions
-bp = Blueprint(
-    "hemlock",
-    __name__,
-    template_folder="templates",
-    static_folder="static",
-    static_url_path="/hemlock/static",
-)
-
-db = SQLAlchemy()
-Mutable.set_session(db.session)
-
-login_manager = LoginManager()
-login_manager.login_view = "hemlock.index"
-login_manager.login_message = None
-
-socketio = SocketIO()
-
-# for caching static pages
-static_pages: Dict[str, str] = {}
-
-
-class Config:
-    """Default configuration file."""
-
-    ALLOW_USERS_TO_RESTART: bool = True
-    SCREENOUT_RECORDS: Dict[str, List[str]] = {}
-    BLOCK_DUPLICATE_KEYS: List[str] = []
-    SQLALCHEMY_TRACK_MODIFICATIONS: bool = False
-    USER_METADATA: defaultdict[str, List[str]] = defaultdict(list)
-
-    @property
-    def PASSWORD(self) -> str:
-        return os.getenv("PASSWORD", "")
-
-    @property
-    def PASSWORD_HASH(self) -> str:
-        if not hasattr(self, "_PASSWORD_HASH"):
-            self._PASSWORD_HASH = generate_password_hash(self.PASSWORD)
-        return self._PASSWORD_HASH
-
-    @property
-    def SECRET_KEY(self) -> str:
-        return os.getenv("SECRET_KEY", "secret")
-
-    @property
-    def SQLALCHEMY_DATABASE_URI(self) -> str:
-        uri = os.getenv("DATABASE_URL", "sqlite://")
-        if uri.startswith("postgres://"):
-            # see https://help.heroku.com/ZKNTJQSK/why-is-sqlalchemy-1-4-x-not-connecting-to-heroku-postgres
-            return uri.replace("postgres://", "postgresql://", 1)
-
-        return uri
-
-    @property
-    def SQLALCHEMY_ENGINE_OPTIONS(self) -> Dict[str, Any]:
-        if self.SQLALCHEMY_DATABASE_URI.startswith("sqlite"):
-            return {}
-
-        return {"pool_size": 1, "pool_recycle": 10, "max_overflow": 0}
-
-
-@bp.before_app_first_request
-def init_app() -> None:
-    """Create database."""
-    db.create_all()
-
-
-def create_app(
-    *config: Union[Mapping, Config],
-    static_folder: str = None,
-    template_folder: str = None,
-    **kwargs: Any
-) -> Flask:
-    """Create application.
-
-    See :class:`hemlock.app.Config` for default configuration.
-
-    Args:
-        *config (Union[Mapping, Config]): Configuration objects. Defaults to None.
-        static_folder (str, optional): Static folder argument for ``flask.Flask``.
-        template_folder (str, optional): Template folder argument for ``flask.Flask``.
-        **kwargs (Any): Passed to ``flask.Flask``.
-
-    Returns:
-        Flask: Application.
-    """
-    if static_folder is None:
-        static_folder = os.path.join(os.getcwd(), "static")
-
-    if template_folder is None:
-        template_folder = os.path.join(os.getcwd(), "templates")
-
-    app = Flask(
-        __name__, static_folder=static_folder, template_folder=template_folder, **kwargs
-    )
-
-    # set up configuration
-    for item in config or (Config(),):
-        if isinstance(item, Mapping):
-            app.config.update(item)
-        else:
-            app.config.from_object(item)
-
-    app.register_blueprint(bp)
-
-    # initialize extensions
-    db.init_app(app)
-    login_manager.init_app(app)
-    socketio.init_app(app)
-
-    return app
-
-
-def create_test_app(*args: Any, **kwargs: Any) -> Flask:
-    """Create a test application.
-
-    Arguments and keywords arguments passed to :func:`hemlock.app.create_app`.
-
-    Returns:
-        Flask: Test application.
-    """
-    app = create_app(*args, **kwargs)
-    app.config["TESTING"] = True
-    app.app_context().push()
-    init_app()
-
-    return app
+"""Application utilities.
+"""
+from __future__ import annotations
+
+import os
+from collections import defaultdict
+from typing import Any, Dict, List, Mapping, Union
+
+from flask import Blueprint, Flask
+from flask_login import LoginManager
+from flask_socketio import SocketIO
+from flask_sqlalchemy import SQLAlchemy
+from sqlalchemy_mutable import Mutable
+from werkzeug.security import generate_password_hash
+
+# create blueprint and extensions
+bp = Blueprint(
+    "hemlock",
+    __name__,
+    template_folder="templates",
+    static_folder="static",
+    static_url_path="/hemlock/static",
+)
+
+db = SQLAlchemy()
+Mutable.set_session(db.session)
+
+login_manager = LoginManager()
+login_manager.login_view = "hemlock.index"
+login_manager.login_message = None
+
+socketio = SocketIO()
+
+# for caching static pages
+static_pages: Dict[str, str] = {}
+
+
+class Config:
+    """Default configuration file."""
+
+    ALLOW_USERS_TO_RESTART: bool = True
+    SCREENOUT_RECORDS: Dict[str, List[str]] = {}
+    BLOCK_DUPLICATE_KEYS: List[str] = []
+    SQLALCHEMY_TRACK_MODIFICATIONS: bool = False
+    USER_METADATA: defaultdict[str, List[str]] = defaultdict(list)
+
+    @property
+    def PASSWORD(self) -> str:
+        return os.getenv("PASSWORD", "")
+
+    @property
+    def PASSWORD_HASH(self) -> str:
+        if not hasattr(self, "_PASSWORD_HASH"):
+            self._PASSWORD_HASH = generate_password_hash(self.PASSWORD)
+        return self._PASSWORD_HASH
+
+    @property
+    def SECRET_KEY(self) -> str:
+        return os.getenv("SECRET_KEY", "secret")
+
+    @property
+    def SQLALCHEMY_DATABASE_URI(self) -> str:
+        uri = os.getenv("DATABASE_URL", "sqlite://")
+        if uri.startswith("postgres://"):
+            # see https://help.heroku.com/ZKNTJQSK/why-is-sqlalchemy-1-4-x-not-connecting-to-heroku-postgres
+            return uri.replace("postgres://", "postgresql://", 1)
+
+        return uri
+
+    @property
+    def SQLALCHEMY_ENGINE_OPTIONS(self) -> Dict[str, Any]:
+        if self.SQLALCHEMY_DATABASE_URI.startswith("sqlite"):
+            return {}
+
+        return {"pool_size": 1, "pool_recycle": 10, "max_overflow": 0}
+
+
+@bp.before_app_request
+def init_app() -> None:
+    """Create database."""
+    db.create_all()
+
+
+def create_app(
+    *config: Union[Mapping, Config],
+    static_folder: str = None,
+    template_folder: str = None,
+    **kwargs: Any,
+) -> Flask:
+    """Create application.
+
+    See :class:`hemlock.app.Config` for default configuration.
+
+    Args:
+        *config (Union[Mapping, Config]): Configuration objects. Defaults to None.
+        static_folder (str, optional): Static folder argument for ``flask.Flask``.
+        template_folder (str, optional): Template folder argument for ``flask.Flask``.
+        **kwargs (Any): Passed to ``flask.Flask``.
+
+    Returns:
+        Flask: Application.
+    """
+    if static_folder is None:
+        static_folder = os.path.join(os.getcwd(), "static")
+
+    if template_folder is None:
+        template_folder = os.path.join(os.getcwd(), "templates")
+
+    app = Flask(
+        __name__, static_folder=static_folder, template_folder=template_folder, **kwargs
+    )
+
+    # set up configuration
+    for item in config or (Config(),):
+        if isinstance(item, Mapping):
+            app.config.update(item)
+        else:
+            app.config.from_object(item)
+
+    app.register_blueprint(bp)
+
+    # initialize extensions
+    db.init_app(app)
+    login_manager.init_app(app)
+    socketio.init_app(app)
+
+    return app
+
+
+def create_test_app(*args: Any, **kwargs: Any) -> Flask:
+    """Create a test application.
+
+    Arguments and keywords arguments passed to :func:`hemlock.app.create_app`.
+
+    Returns:
+        Flask: Test application.
+    """
+    app = create_app(*args, **kwargs)
+    app.config["TESTING"] = True
+    app.app_context().push()
+    init_app()
+
+    return app
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/data.py` & `hemlock-survey-1.0.1/src/hemlock/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,102 @@
-"""Data containers.
-"""
-from __future__ import annotations
-
-from typing import Any
-
-from sqlalchemy_mutable.types import MutablePickleType
-
-from ._data_frame import DataFrame
-from .app import db
-
-
-class Data(db.Model):  # type: ignore
-    """Data containers record data from a user's survey.
-
-    Args:
-        variable (str, optional): Name of the variable. Defaults to None.
-        data (Any, optional): Value of the data. Defaults to None.
-        n_rows (int, optional): Number of rows over which this data will be repeated.
-            Defaults to 1.
-        fill_rows (bool, optional): Indicates that empty rows in the data frame
-            following this data should be filled in with this data. Defaults to False.
-        record_index (bool, optional): Indicates that this data object's index should
-            be recorded in the data frame. Defaults to False.
-
-    Attributes:
-        variable (str): Name of the variable.
-        data (Any): Value of the data.
-        n_rows (int): Number of rows over which this data will be repeated.
-        fill_rows (bool): Indicates that empty rows in the data frame following this
-            data should be filled in with this data.
-        record_index (bool): Indicates that this data object's index should be recorded
-            in the data frame.
-
-    Examples:
-
-        .. doctest::
-
-            >>> from hemlock import Data
-            >>> dict(Data("variable_name", 1).pack_data())
-            {'variable_name': [1]}
-            >>> dict(Data("variable_name", 1, n_rows=3).pack_data())
-            {'variable_name': [1, 1, 1]}
-            >>> dict(Data("variable_name", [0, 1, 2]).pack_data())
-            {'variable_name': [0, 1, 2]}
-            >>> dict(Data("prefix", {"suffix0": 0, "suffix1": [1, 2]}).pack_data())
-            {'prefix_suffix0': [0, 0], 'prefix_suffix1': [1, 2]}
-    """
-
-    id = db.Column(db.Integer, primary_key=True)
-    data_type = db.Column(db.String)
-    __mapper_args__ = {"polymorphic_identity": "data", "polymorphic_on": data_type}
-
-    _page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
-
-    variable = db.Column(db.String)
-    data = db.Column(MutablePickleType)
-    n_rows = db.Column(db.Integer)
-    fill_rows = db.Column(db.Boolean)
-    index = db.Column(db.Integer)
-    record_index = db.Column(db.Boolean)
-
-    def __init__(
-        self,
-        variable: str = None,
-        data: Any = None,
-        n_rows: int = 1,
-        fill_rows: bool = False,
-        record_index: bool = False,
-    ):
-        self.variable = variable
-        self.data = data
-        self.n_rows = n_rows
-        self.fill_rows = fill_rows
-        self.record_index = record_index
-
-    def __repr__(self):
-        return f"<{self.__class__.__qualname__} {self.variable} {self.data}>"
-
-    def pack_data(self) -> DataFrame:
-        """Package the data for insertion into a data frame.
-
-        Returns:
-            DataFrame: Mapping of variable names to values.
-        """
-        if self.variable is None:
-            return DataFrame()
-
-        # if self.data is None it won't have a `get_object` method
-        data = None if self.data is None else self.data.get_object()
-        if isinstance(data, dict):
-            packed_data = {f"{self.variable}_{key}": item for key, item in data.items()}
-        else:
-            packed_data = {self.variable: data}
-
-        if self.record_index:
-            packed_data[f"{self.variable}_index"] = self.index
-
-        dataframe = DataFrame(packed_data, fill_rows=True)
-        dataframe.pad(min_rows=self.n_rows)
-        return dataframe
+"""Data containers.
+"""
+from __future__ import annotations
+
+from typing import Any
+
+from sqlalchemy_mutable.types import MutablePickleType
+
+from ._data_frame import DataFrame
+from .app import db
+
+
+class Data(db.Model):  # type: ignore
+    """Data containers record data from a user's survey.
+
+    Args:
+        variable (str, optional): Name of the variable. Defaults to None.
+        data (Any, optional): Value of the data. Defaults to None.
+        n_rows (int, optional): Number of rows over which this data will be repeated.
+            Defaults to 1.
+        fill_rows (bool, optional): Indicates that empty rows in the data frame
+            following this data should be filled in with this data. Defaults to False.
+        record_index (bool, optional): Indicates that this data object's index should
+            be recorded in the data frame. Defaults to False.
+
+    Attributes:
+        variable (str): Name of the variable.
+        data (Any): Value of the data.
+        n_rows (int): Number of rows over which this data will be repeated.
+        fill_rows (bool): Indicates that empty rows in the data frame following this
+            data should be filled in with this data.
+        record_index (bool): Indicates that this data object's index should be recorded
+            in the data frame.
+
+    Examples:
+
+        .. doctest::
+
+            >>> from hemlock import Data
+            >>> dict(Data("variable_name", 1).pack_data())
+            {'variable_name': [1]}
+            >>> dict(Data("variable_name", 1, n_rows=3).pack_data())
+            {'variable_name': [1, 1, 1]}
+            >>> dict(Data("variable_name", [0, 1, 2]).pack_data())
+            {'variable_name': [0, 1, 2]}
+            >>> dict(Data("prefix", {"suffix0": 0, "suffix1": [1, 2]}).pack_data())
+            {'prefix_suffix0': [0, 0], 'prefix_suffix1': [1, 2]}
+    """
+
+    id = db.Column(db.Integer, primary_key=True)
+    data_type = db.Column(db.String)
+    __mapper_args__ = {"polymorphic_identity": "data", "polymorphic_on": data_type}
+
+    _user_id = db.Column(db.Integer, db.ForeignKey("user.id"))
+    _page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
+
+    variable = db.Column(db.String)
+    data = db.Column(MutablePickleType)
+    n_rows = db.Column(db.Integer)
+    fill_rows = db.Column(db.Boolean)
+    index = db.Column(db.Integer)
+    record_index = db.Column(db.Boolean)
+
+    def __init__(
+        self,
+        variable: str = None,
+        data: Any = None,
+        n_rows: int = 1,
+        fill_rows: bool = False,
+        record_index: bool = False,
+    ):
+        self.variable = variable
+        self.data = data
+        self.n_rows = n_rows
+        self.fill_rows = fill_rows
+        self.record_index = record_index
+
+    def __repr__(self):
+        return f"<{self.__class__.__qualname__} {self.variable} {self.data}>"
+
+    def pack_data(self) -> DataFrame:
+        """Package the data for insertion into a data frame.
+
+        Returns:
+            DataFrame: Mapping of variable names to values.
+        """
+        if self.variable is None:
+            return DataFrame()
+
+        # if self.data is None it won't have a `get_object` method
+        data = None if self.data is None else self.data.get_object()
+        if isinstance(data, dict):
+            packed_data = {f"{self.variable}_{key}": item for key, item in data.items()}
+        else:
+            packed_data = {self.variable: data}
+
+        if self.record_index:
+            packed_data[f"{self.variable}_index"] = self.index
+
+        dataframe = DataFrame(packed_data, fill_rows=True)
+        dataframe.pad(min_rows=self.n_rows)
+        return dataframe
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/functional/base.py` & `hemlock-survey-1.0.1/src/hemlock/functional/base.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-"""A class for registering functions.
-"""
-from __future__ import annotations
-
-import functools
-from typing import Any, Callable, List, Tuple, Union
-
-from sqlalchemy_mutable.utils import partial
-
-
-class Functional(dict):
-    """A class for registering functions.
-
-    Attributes:
-        functions (Dict[str, Callable]): Registered functions.
-
-    Examples:
-        Accessing registered functions is similar to accessing columns in a pandas
-        DataFrame. If you access a function with a tuple, the first item of the tuple is
-        understood as the key, while the rest of tuple items are passed to the function
-        as arguments.
-
-        .. code-block::
-
-            >>> from hemlock.functional import Functional
-            >>> functional = Functional()
-            >>> @functional.register
-            ... def foo(*args):
-            ...     pass
-            ...
-            >>> functional.foo("Hello, world!")
-            <foo('Hello, world!')>
-            >>> functional["foo"]
-            <foo()>
-            >>> functional[["foo", "foo"]]
-            [<foo()>, <foo()>]
-            >>> functional[("foo", "Hello, world!")]
-            <foo('Hello, world!')>
-            >>> functional[[("foo", "Hello, world!"), ("foo", "Goodbye, world!")]]
-            [<foo('Hello, world!')>, <foo('Goodbye, world!')>]
-    """
-
-    def register(self, func: Callable) -> Callable:
-        """Decorator to register a new function.
-
-        Args:
-            func (Callable): Function to be registered.
-
-        Returns:
-            Callable: Original function.
-        """
-
-        @functools.wraps(func)
-        def make_partial(*args, **kwargs):
-            return partial(func, *args, **kwargs)
-
-        self[func.__name__] = make_partial
-        return func
-
-    def __getattribute__(self, name: str) -> Any:
-        try:
-            return super().__getattribute__(name)
-        except AttributeError:
-            return super().__getitem__(name)
-
-    def __getitem__(
-        self, keys: Union[str, Tuple, List[str], List[Tuple]]
-    ) -> Union[partial, List[partial]]:
-        if isinstance(keys, list):
-            return_value = []
-            for key in keys:
-                if isinstance(key, tuple):
-                    return_value.append(super().__getitem__(key[0])(*key[1:]))
-                else:
-                    return_value.append(super().__getitem__(key)())
-            return return_value
-
-        if isinstance(keys, tuple):
-            return super().__getitem__(keys[0])(*keys[1:])
-        return super().__getitem__(keys)()
+"""A class for registering functions.
+"""
+from __future__ import annotations
+
+import functools
+from typing import Any, Callable, List, Tuple, Union
+
+from sqlalchemy_mutable.utils import partial
+
+
+class Functional(dict):
+    """A class for registering functions.
+
+    Attributes:
+        functions (Dict[str, Callable]): Registered functions.
+
+    Examples:
+        Accessing registered functions is similar to accessing columns in a pandas
+        DataFrame. If you access a function with a tuple, the first item of the tuple is
+        understood as the key, while the rest of tuple items are passed to the function
+        as arguments.
+
+        .. code-block::
+
+            >>> from hemlock.functional import Functional
+            >>> functional = Functional()
+            >>> @functional.register
+            ... def foo(*args):
+            ...     pass
+            ...
+            >>> functional.foo("Hello, world!")
+            <foo('Hello, world!')>
+            >>> functional["foo"]
+            <foo()>
+            >>> functional[["foo", "foo"]]
+            [<foo()>, <foo()>]
+            >>> functional[("foo", "Hello, world!")]
+            <foo('Hello, world!')>
+            >>> functional[[("foo", "Hello, world!"), ("foo", "Goodbye, world!")]]
+            [<foo('Hello, world!')>, <foo('Goodbye, world!')>]
+    """
+
+    def register(self, func: Callable) -> Callable:
+        """Decorator to register a new function.
+
+        Args:
+            func (Callable): Function to be registered.
+
+        Returns:
+            Callable: Original function.
+        """
+
+        @functools.wraps(func)
+        def make_partial(*args, **kwargs):
+            return partial(func, *args, **kwargs)
+
+        self[func.__name__] = make_partial
+        return func
+
+    def __getattribute__(self, name: str) -> Any:
+        try:
+            return super().__getattribute__(name)
+        except AttributeError:
+            return super().__getitem__(name)
+
+    def __getitem__(
+        self, keys: Union[str, Tuple, List[str], List[Tuple]]
+    ) -> Union[partial, List[partial]]:
+        if isinstance(keys, list):
+            return_value = []
+            for key in keys:
+                if isinstance(key, tuple):
+                    return_value.append(super().__getitem__(key[0])(*key[1:]))
+                else:
+                    return_value.append(super().__getitem__(key)())
+            return return_value
+
+        if isinstance(keys, tuple):
+            return super().__getitem__(keys[0])(*keys[1:])
+        return super().__getitem__(keys)()
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/functional/compile.py` & `hemlock-survey-1.0.1/src/hemlock/functional/compile.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""Built-in compile functions.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import TYPE_CHECKING, Union
-
-from flask.templating import render_template
-
-from .base import Functional
-
-if TYPE_CHECKING:
-    from ..page import Page
-    from ..questions.base import Question
-
-compile = Functional()
-
-
-@compile.register
-def auto_advance(
-    obj: Union["Page", "Question"],
-    after: int,
-    clock_id: str = None,
-    clock_update_interval: int = 1000,
-) -> None:
-    """Automatically advance to the next page after a given amount of time.
-
-    Args:
-        obj (Union[): Page or question.
-        after (int): Time after which the user will automatically advance
-            (milliseconds).
-        clock_id (str, optional): ID of an HTML element whose text will be updated with
-            the countdown. Defaults to None.
-        clock_update_interval (int, optional): Interval of time with which the countdown
-            should be updated (milliseconds). Defaults to 1000.
-
-    Examples:
-        Copy and paste the following into a python file, then run it. This will display
-        a countdown and automatically advance the user after 10 seconds (10000
-        milliseconds).
-
-        .. code-block::
-
-            from hemlock import User, Page, create_app
-            from hemlock.functional import compile
-            from hemlock.questions import Label
-
-            @User.route("/survey")
-            def seed():
-                return [
-                    Page(
-                        Label(
-                            "Remaining time: <span id='clock-id'></span>",
-                            compile=compile.auto_advance(10000, clock_id="clock-id")
-                        ),
-                    ),
-                    Page(
-                        Label("The End."),
-                    )
-                ]
-
-            app = create_app()
-
-            if __name__ == "__main__":
-                app.run()
-    """
-    # remove any auto-advance javascript from running this function previously
-    obj.html_settings["js"] = [
-        js
-        for js in obj.html_settings["js"]
-        if not js.startswith('<script id="auto-advance"')
-    ]
-    obj.html_settings["js"].append(
-        render_template(
-            "hemlock/statics/auto_advance.html",
-            start_time=datetime.utcnow().isoformat(),
-            after=after,
-            clock_id=clock_id,
-            clock_update_interval=clock_update_interval,
-        )
-    )
-
-
-@compile.register
-def clear_feedback(obj: Union["Page", "Question"]) -> None:
-    """Clear feedback.
-
-    Args:
-        obj (Union[Page, Question]): Page or question whose feedback will be cleared.
-    """
-    obj.clear_feedback()
-
-
-@compile.register
-def clear_response(obj: Union["Page", "Question"]) -> None:
-    """Clear response.
-
-    Args:
-        obj (Union[Page, Question]): Page or question whose responses will be cleared.
-    """
-    obj.clear_response()
+"""Built-in compile functions.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import TYPE_CHECKING, Union
+
+from flask.templating import render_template
+
+from .base import Functional
+
+if TYPE_CHECKING:
+    from ..page import Page
+    from ..questions.base import Question
+
+compile = Functional()
+
+
+@compile.register
+def auto_advance(
+    obj: Union["Page", "Question"],
+    after: int,
+    clock_id: str = None,
+    clock_update_interval: int = 1000,
+) -> None:
+    """Automatically advance to the next page after a given amount of time.
+
+    Args:
+        obj (Union[): Page or question.
+        after (int): Time after which the user will automatically advance
+            (milliseconds).
+        clock_id (str, optional): ID of an HTML element whose text will be updated with
+            the countdown. Defaults to None.
+        clock_update_interval (int, optional): Interval of time with which the countdown
+            should be updated (milliseconds). Defaults to 1000.
+
+    Examples:
+        Copy and paste the following into a python file, then run it. This will display
+        a countdown and automatically advance the user after 10 seconds (10000
+        milliseconds).
+
+        .. code-block::
+
+            from hemlock import User, Page, create_app
+            from hemlock.functional import compile
+            from hemlock.questions import Label
+
+            @User.route("/survey")
+            def seed():
+                return [
+                    Page(
+                        Label(
+                            "Remaining time: <span id='clock-id'></span>",
+                            compile=compile.auto_advance(10000, clock_id="clock-id")
+                        ),
+                    ),
+                    Page(
+                        Label("The End."),
+                    )
+                ]
+
+            app = create_app()
+
+            if __name__ == "__main__":
+                app.run()
+    """
+    # remove any auto-advance javascript from running this function previously
+    obj.html_settings["js"] = [
+        js
+        for js in obj.html_settings["js"]
+        if not js.startswith('<script id="auto-advance"')
+    ]
+    obj.html_settings["js"].append(
+        render_template(
+            "hemlock/statics/auto_advance.html",
+            start_time=datetime.utcnow().isoformat(),
+            after=after,
+            clock_id=clock_id,
+            clock_update_interval=clock_update_interval,
+        )
+    )
+
+
+@compile.register
+def clear_feedback(obj: Union["Page", "Question"]) -> None:
+    """Clear feedback.
+
+    Args:
+        obj (Union[Page, Question]): Page or question whose feedback will be cleared.
+    """
+    obj.clear_feedback()
+
+
+@compile.register
+def clear_response(obj: Union["Page", "Question"]) -> None:
+    """Clear response.
+
+    Args:
+        obj (Union[Page, Question]): Page or question whose responses will be cleared.
+    """
+    obj.clear_response()
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/functional/test_response.py` & `hemlock-survey-1.0.1/src/hemlock/functional/test_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,231 +1,233 @@
-"""Built-in functions for generating test responses.
-"""
-from __future__ import annotations
-
-import math
-import random
-from datetime import datetime, timedelta
-from string import digits, ascii_letters
-from typing import TYPE_CHECKING, Any, Dict, Optional
-
-import numpy as np
-from sqlalchemy_mutable.utils import is_instance
-
-from .base import Functional
-
-if TYPE_CHECKING:
-    from ..page import Page
-    from ..questions.base import Question
-    from ..questions.choice_base import ChoiceQuestion
-
-CHARACTERS = digits + ascii_letters
-TEXT_INPUT_TYPE = "text"
-RANGE_INPUT_TYPE = "range"
-NUMBER_INPUT_TYPE = "number"
-
-test_response = Functional()
-
-# map input types to (HTML format, datetime format)
-# where HTML format is the raw format from the post request
-# and datetime format is the format expected by python's datetime module
-datetime_input_types = {
-    "date": ("yyyy-mm-dd", "%Y-%m-%d"),
-    "datetime": ("yyyy-mm-ddTHH:MM", "%Y-%m-%dT%H:%M"),
-    "datetime-local": ("yyyy-mm-ddTHH:MM", "%Y-%m-%dT%H:%M"),
-    "month": ("yyyy-mm", "%Y-%m"),
-    "time": ("HH:MM", "%H:%M"),
-}
-
-
-@test_response.register
-def random_direction(page: "Page", pr_back: float = 0.2) -> str:
-    """Chooses a random direction for navigation.
-
-    Args:
-        page (Page): Page to navigate from.
-        pr_back (float, optional): Probability of going back if both forward and back
-            navigation are available. This parameter is ignored if it is only possible
-            to navigate in one direction. Defaults to 0.2.
-
-    Raises:
-        ValueError: If it is impossible to navigate from this page.
-
-    Returns:
-        str: "forward" or "back"
-    """
-    forward = bool(page.forward) and not page.is_last_page
-    back = bool(page.back) and not page.is_first_page
-
-    if not (forward or back):
-        raise ValueError(f"Navigation is not possible from page {page}.")
-
-    if forward and not back:
-        return "forward"
-
-    if back and not forward:
-        return "back"
-
-    return "back" if random.random() < pr_back else "forward"
-
-
-@test_response.register
-def random_input(input: Question, **kwargs: Any) -> Any:
-    """Generate a random response for an input-like question.
-
-    Args:
-        input (Question): Input question.
-        **kwargs (Any): Passed to :func:`random_text`, :func:`random_number`, or
-            :func:`random_datetime`, depending on the input type.
-
-    Returns:
-        Any: Response.
-    """
-    input_type = input.input_tag.get("type", TEXT_INPUT_TYPE)
-
-    if input_type in (NUMBER_INPUT_TYPE, RANGE_INPUT_TYPE):
-        return random_number(input, **kwargs)
-
-    if input_type in datetime_input_types:
-        return random_datetime(input, **kwargs)
-
-    return random_text(input, **kwargs)
-
-
-@test_response.register
-def random_text(question: "Question", pr_no_response: float = 0.2) -> Optional[str]:
-    """Generate a random text response for an input-like question.
-
-    Args:
-        question (Question): Question, usually a :class:`hemlock.questions.input.Input`
-            or :class:`hemlock.questions.textarea.Textarea`.
-        pr_no_response (float, optional): Probability that the user doesn't respond.
-            Defaults to .2.
-
-    Returns:
-        Optional[str]: Response.
-    """
-    # get the input or textarea HTML attributes
-    tag: Dict[Any, Any] = {}
-    if hasattr(question, "input_tag"):
-        tag = question.input_tag
-    elif hasattr(question, "textarea_tag"):
-        tag = question.textarea_tag
-
-    if not tag.get("required") and random.random() < pr_no_response:
-        return None
-
-    length = random.randint(tag.get("minlength", 1), tag.get("maxlength", 20))
-    n_words = random.randint(tag.get("minwords", 1), tag.get("maxwords", 5))
-    n_words = min(n_words, math.ceil(length / 2))
-    n_whitespace_characters = n_words - 1
-    word_length = int((length - n_whitespace_characters) / n_words)
-
-    words = []
-    for _ in range(n_words):
-        words.append("".join(random.choices(CHARACTERS, k=word_length)))
-    response = " ".join(words)
-
-    if len(response) < length:
-        # add additional characters if the response is too short
-        response += "".join(random.choices(CHARACTERS, k=length - len(response)))
-    return response
-
-
-@test_response.register
-def random_number(input: "Question", pr_no_response: float = 0.2) -> Optional[float]:
-    """Generate a random number response for an input-like question.
-
-    Args:
-        input (Question): Input question.
-        pr_no_response (float, optional): Probability that the user doesn't respond.
-            Defaults to .2.
-
-    Returns:
-        Optional[float]: Response.
-    """
-    if not input.input_tag.get("required") and random.random() < pr_no_response:
-        return None
-
-    input_tag = input.input_tag
-    start = input_tag.get("min", -10000)
-    stop = input_tag.get("max", 10000)
-    step = input_tag.get("step", 1)
-    value = np.random.choice(np.arange(start, stop, step))
-    if is_instance(start, int) and is_instance(stop, int) and is_instance(step, int):
-        return int(value)
-    # with a small step, you may encounter floating-point issues.
-    # this rounds the response to the correct number of decimal places.
-    # TODO: This isn't exactly correct. What about cases where min=1.01 and step=1?
-    # Flagging for followup.
-    return round(value, math.ceil(-math.log10(step)))
-
-
-@test_response.register
-def random_datetime(
-    input: "Question", pr_no_response: float = 0.2
-) -> Optional[datetime]:
-    """Generate a random datetime response for an input-like question.
-
-    Args:
-        input (Question): Input question.
-        pr_no_response (float, optional): Probability that the user doesn't respond.
-            Defaults to .2.
-
-    Returns:
-        Optional[datetime]: Response.
-    """
-    if not input.input_tag.get("required") and random.random() < pr_no_response:
-        return None
-
-    def get_datetime(key):
-        raw_value = input_tag.get(key)
-        if raw_value is None:
-            delta = timedelta(weeks=100 * 52)  # 100 years
-            if key == "min":
-                return datetime.utcnow() - delta
-            return datetime.utcnow() + delta
-        return datetime.strptime(raw_value, datetime_format)
-
-    input_tag = input.input_tag
-    input_type = input_tag["type"]
-    _, datetime_format = datetime_input_types[input_type]
-    start, stop = get_datetime("min"), get_datetime("max")
-    return start + timedelta(seconds=np.random.uniform((stop - start).total_seconds()))
-
-
-@test_response.register
-def random_choices(
-    question: "ChoiceQuestion",
-    pr_no_response: float = 0.2,
-    min_choices: int = 0,
-    max_choices: int = None,
-) -> Any:
-    """Select random choices as a test response.
-
-    Args:
-        question (ChoiceQuestion): Choice question.
-        pr_no_response (float, optional): Probability that the user selects none of the
-            choices. Defaults to 0.2.
-        min_choices (int, optional): Minimum number of choices the user selects. Only
-            relevant if the user can select multiple choices. Defaults to 0.
-        max_choices (int, optional): Maximum number of choices the user selects. Only
-            relevant if the user can select multiple choices. Defaults to None.
-
-    Returns:
-        Any: Choice value or set of choice values.
-    """
-    if random.random() < pr_no_response:
-        return None
-
-    choice_values = [
-        choice["value"] for choice in question.choices if not choice.get("disabled")
-    ]
-
-    if question.multiple:
-        if max_choices is None:
-            max_choices = len(choice_values)
-
-        n_choices = random.randint(min_choices, max_choices)
-        return set(random.sample(choice_values, k=n_choices))
-
-    return random.choice(choice_values)
+"""Built-in functions for generating test responses.
+"""
+from __future__ import annotations
+
+import math
+import random
+from datetime import datetime, timedelta
+from string import digits, ascii_letters
+from typing import TYPE_CHECKING, Any, Dict, Optional
+
+import numpy as np
+from sqlalchemy_mutable.utils import is_instance
+
+from .base import Functional
+
+if TYPE_CHECKING:
+    from ..page import Page
+    from ..questions.base import Question
+    from ..questions.choice_base import ChoiceQuestion
+
+CHARACTERS = digits + ascii_letters
+TEXT_INPUT_TYPE = "text"
+RANGE_INPUT_TYPE = "range"
+NUMBER_INPUT_TYPE = "number"
+
+test_response = Functional()
+
+# map input types to (HTML format, datetime format)
+# where HTML format is the raw format from the post request
+# and datetime format is the format expected by python's datetime module
+datetime_input_types = {
+    "date": ("yyyy-mm-dd", "%Y-%m-%d"),
+    "datetime": ("yyyy-mm-ddTHH:MM", "%Y-%m-%dT%H:%M"),
+    "datetime-local": ("yyyy-mm-ddTHH:MM", "%Y-%m-%dT%H:%M"),
+    "month": ("yyyy-mm", "%Y-%m"),
+    "time": ("HH:MM", "%H:%M"),
+}
+
+
+@test_response.register
+def random_direction(page: "Page", pr_back: float = 0.2) -> str:
+    """Chooses a random direction for navigation.
+
+    Args:
+        page (Page): Page to navigate from.
+        pr_back (float, optional): Probability of going back if both forward and back
+            navigation are available. This parameter is ignored if it is only possible
+            to navigate in one direction. Defaults to 0.2.
+
+    Raises:
+        ValueError: If it is impossible to navigate from this page.
+
+    Returns:
+        str: "forward" or "back"
+    """
+    forward = bool(page.forward) and not page.is_last_page
+    back = bool(page.back) and not page.is_first_page
+
+    if not (forward or back):
+        raise ValueError(f"Navigation is not possible from page {page}.")
+
+    if forward and not back:
+        return "forward"
+
+    if back and not forward:
+        return "back"
+
+    return "back" if random.random() < pr_back else "forward"
+
+
+@test_response.register
+def random_input(input: Question, **kwargs: Any) -> Any:
+    """Generate a random response for an input-like question.
+
+    Args:
+        input (Question): Input question.
+        **kwargs (Any): Passed to :func:`random_text`, :func:`random_number`, or
+            :func:`random_datetime`, depending on the input type.
+
+    Returns:
+        Any: Response.
+    """
+    input_type = input.input_tag.get("type", TEXT_INPUT_TYPE)
+
+    if input_type in (NUMBER_INPUT_TYPE, RANGE_INPUT_TYPE):
+        return random_number(input, **kwargs)
+
+    if input_type in datetime_input_types:
+        return random_datetime(input, **kwargs)
+
+    return random_text(input, **kwargs)
+
+
+@test_response.register
+def random_text(question: "Question", pr_no_response: float = 0.2) -> Optional[str]:
+    """Generate a random text response for an input-like question.
+
+    Args:
+        question (Question): Question, usually a :class:`hemlock.questions.input.Input`
+            or :class:`hemlock.questions.textarea.Textarea`.
+        pr_no_response (float, optional): Probability that the user doesn't respond.
+            Defaults to .2.
+
+    Returns:
+        Optional[str]: Response.
+    """
+    # get the input or textarea HTML attributes
+    tag: Dict[Any, Any] = {}
+    if hasattr(question, "input_tag"):
+        tag = question.input_tag
+    elif hasattr(question, "textarea_tag"):
+        tag = question.textarea_tag
+
+    if not tag.get("required") and random.random() < pr_no_response:
+        return None
+
+    length = random.randint(tag.get("minlength", 1), tag.get("maxlength", 20))
+    n_words = random.randint(tag.get("minwords", 1), tag.get("maxwords", 5))
+    n_words = min(n_words, math.ceil(length / 2))
+    n_whitespace_characters = n_words - 1
+    word_length = int((length - n_whitespace_characters) / n_words)
+
+    words = []
+    for _ in range(n_words):
+        words.append("".join(random.choices(CHARACTERS, k=word_length)))
+    response = " ".join(words)
+
+    if len(response) < length:
+        # add additional characters if the response is too short
+        response += "".join(random.choices(CHARACTERS, k=length - len(response)))
+    return response
+
+
+@test_response.register
+def random_number(input: "Question", pr_no_response: float = 0.2) -> Optional[float]:
+    """Generate a random number response for an input-like question.
+
+    Args:
+        input (Question): Input question.
+        pr_no_response (float, optional): Probability that the user doesn't respond.
+            Defaults to .2.
+
+    Returns:
+        Optional[float]: Response.
+    """
+    if not input.input_tag.get("required") and random.random() < pr_no_response:
+        return None
+
+    input_tag = input.input_tag
+    start = input_tag.get("min", -10000)
+    stop = input_tag.get("max", 10000)
+    step = input_tag.get("step", 1)
+    if step == "any":
+        step = random.choice((1., .1, .01))
+    value = np.random.choice(np.arange(start, stop, step))
+    if is_instance(start, int) and is_instance(stop, int) and is_instance(step, int):
+        return int(value)
+    # with a small step, you may encounter floating-point issues.
+    # this rounds the response to the correct number of decimal places.
+    # TODO: This isn't exactly correct. What about cases where min=1.01 and step=1?
+    # Flagging for followup.
+    return round(value, math.ceil(-math.log10(step)))
+
+
+@test_response.register
+def random_datetime(
+    input: "Question", pr_no_response: float = 0.2
+) -> Optional[datetime]:
+    """Generate a random datetime response for an input-like question.
+
+    Args:
+        input (Question): Input question.
+        pr_no_response (float, optional): Probability that the user doesn't respond.
+            Defaults to .2.
+
+    Returns:
+        Optional[datetime]: Response.
+    """
+    if not input.input_tag.get("required") and random.random() < pr_no_response:
+        return None
+
+    def get_datetime(key):
+        raw_value = input_tag.get(key)
+        if raw_value is None:
+            delta = timedelta(weeks=100 * 52)  # 100 years
+            if key == "min":
+                return datetime.utcnow() - delta
+            return datetime.utcnow() + delta
+        return datetime.strptime(raw_value, datetime_format)
+
+    input_tag = input.input_tag
+    input_type = input_tag["type"]
+    _, datetime_format = datetime_input_types[input_type]
+    start, stop = get_datetime("min"), get_datetime("max")
+    return start + timedelta(seconds=np.random.uniform((stop - start).total_seconds()))
+
+
+@test_response.register
+def random_choices(
+    question: "ChoiceQuestion",
+    pr_no_response: float = 0.2,
+    min_choices: int = 0,
+    max_choices: int = None,
+) -> Any:
+    """Select random choices as a test response.
+
+    Args:
+        question (ChoiceQuestion): Choice question.
+        pr_no_response (float, optional): Probability that the user selects none of the
+            choices. Defaults to 0.2.
+        min_choices (int, optional): Minimum number of choices the user selects. Only
+            relevant if the user can select multiple choices. Defaults to 0.
+        max_choices (int, optional): Maximum number of choices the user selects. Only
+            relevant if the user can select multiple choices. Defaults to None.
+
+    Returns:
+        Any: Choice value or set of choice values.
+    """
+    if random.random() < pr_no_response:
+        return None
+
+    choice_values = [
+        choice["value"] for choice in question.choices if not choice.get("disabled")
+    ]
+
+    if question.multiple:
+        if max_choices is None:
+            max_choices = len(choice_values)
+
+        n_choices = random.randint(min_choices, max_choices)
+        return set(random.sample(choice_values, k=n_choices))
+
+    return random.choice(choice_values)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/functional/validate.py` & `hemlock-survey-1.0.1/src/hemlock/functional/validate.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-"""Built-in validate functions.
-"""
-from __future__ import annotations
-
-import operator
-import re
-from decimal import Decimal
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Tuple, Union
-
-from sqlalchemy_mutable.utils import get_object, is_instance
-
-from .base import Functional
-
-if TYPE_CHECKING:
-    from ..questions.base import Question
-
-HOW_TO_TRANSFORM = {
-    "value": lambda question: question.response,
-    "length": lambda question: len(question.response),
-    "word count": lambda question: len(
-        re.findall("\w+", get_object(question.response))
-    ),
-    "decimals": lambda question: -Decimal(get_object(question.raw_response))
-    .as_tuple()
-    .exponent,
-}
-
-ComparisonType = Union[str, Callable[[Any, Any], bool]]
-FeedbackType = Optional[Union[bool, Tuple[bool, Optional[str]]]]
-HowType = Union[str, Callable[["Question"], Any]]
-
-validate = Functional()
-
-
-@validate.register
-def require_response(question: "Question", feedback: str = None) -> FeedbackType:
-    """Require a response.
-
-    Args:
-        question (Question): Question.
-        feedback (str, optional): Feedback if the user didn't respond. Defaults to None.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    if question.response in (None, set()):
-        return False, feedback
-    return None
-
-
-@validate.register
-def response_in(
-    question: "Question", valid_set: Iterable, feedback: str = None
-) -> FeedbackType:
-    """Require that the user's response be in a given set.
-
-    Args:
-        question (Question): Question.
-        valid_set (Iterable): Set of valid responses.
-        feedback (str, optional): Feedback if the user's response isn't in the valid
-            set. Defaults to None.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    if question.response not in valid_set:
-        return False, feedback
-    return None
-
-
-@validate.register
-def response_not_in(
-    question: "Question", invalid_set: Iterable, feedback: str = None
-) -> FeedbackType:
-    """Require that the user's response not be in a given set.
-
-    Args:
-        question (Question): Question.
-        invalid_set (Iterable): Set of invalid responses.
-        feedback (str, optional): Feedback if the user's response is in the invalid
-            set. Defaults to None.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    if question.response in invalid_set:
-        return False, feedback
-    return None
-
-
-@validate.register
-def compare_response(
-    question: "Question",
-    value: Any,
-    feedback: str = None,
-    comparison: ComparisonType = "==",
-    how: HowType = "value",
-) -> FeedbackType:
-    """Require that the user's response satsify a comparison.
-
-    Args:
-        question (Question): Question.
-        value (Any): Value to which the response will be compared.
-        feedback (str, optional): Feedback if the comparison fails. Defaults to None.
-        comparison (ComparisonType, optional): Comparison operator. Defaults to ==.
-        how (HowType, optional): How the response should be assessed ("value",
-            "length", "word count", or "decimals"). Defaults to value.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    from ..questions.base import Question
-
-    string_to_operator = {
-        "<": operator.lt,
-        "<=": operator.le,
-        "==": operator.eq,
-        "!=": operator.ne,
-        ">=": operator.ge,
-        ">": operator.gt,
-    }
-    transform_response = HOW_TO_TRANSFORM[how] if is_instance(how, str) else how  # type: ignore
-
-    response = transform_response(question)  # type: ignore
-
-    if is_instance(value, Question):
-        value = transform_response(value)  # type: ignore
-
-    if is_instance(comparison, str):
-        comparison = string_to_operator[comparison]  # type: ignore
-
-    if not comparison(response, value):  # type: ignore
-        return False, feedback
-    return None
-
-
-@validate.register
-def response_in_range(
-    question: "Question",
-    min_value: Any,
-    max_value: Any,
-    feedback: str = None,
-    how: HowType = "value",
-) -> FeedbackType:
-    """Require the user's response to be in a given range of values.
-
-    Args:
-        question (Question): Question.
-        min_value (Any): Minimum value.
-        max_value (Any): Maximum value.
-        feedback (str, optional): Feedback if the response is not in the required
-            range. Defaults to None.
-        how (HowType, optional): How the response should be assessed ("value",
-            "length", "word count", or "decimals"). Defaults to value.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    response = HOW_TO_TRANSFORM[how](question)  # type: ignore
-    if not (min_value <= response <= max_value):
-        return False, feedback
-    return None
-
-
-@validate.register
-def re_full_match(
-    question: "Question",
-    pattern: str,
-    feedback: str = None,
-    flags: Any = 0,
-) -> FeedbackType:
-    """Require that the user's response match a regular expression.
-
-    Args:
-        question (Question): Question.
-        pattern (str): Regular expression pattern.
-        feedback (str, optional): Feedback if the response does not match the pattern.
-            Defaults to None.
-        flags (Any, optional): Flags (see python documentation on ``re.fullmatch``).
-            Defaults to 0.
-
-    Returns:
-        FeedbackType: Feedback.
-    """
-    if not re.fullmatch(pattern, question.response, flags):
-        return False, feedback
-    return None
+"""Built-in validate functions.
+"""
+from __future__ import annotations
+
+import operator
+import re
+from decimal import Decimal
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Tuple, Union
+
+from sqlalchemy_mutable.utils import get_object, is_instance
+
+from .base import Functional
+
+if TYPE_CHECKING:
+    from ..questions.base import Question
+
+HOW_TO_TRANSFORM = {
+    "value": lambda question: question.response,
+    "length": lambda question: len(question.response),
+    "word count": lambda question: len(
+        re.findall("\w+", get_object(question.response))
+    ),
+    "decimals": lambda question: -Decimal(get_object(question.raw_response))
+    .as_tuple()
+    .exponent,
+}
+
+ComparisonType = Union[str, Callable[[Any, Any], bool]]
+FeedbackType = Optional[Union[bool, Tuple[bool, Optional[str]]]]
+HowType = Union[str, Callable[["Question"], Any]]
+
+validate = Functional()
+
+
+@validate.register
+def require_response(question: "Question", feedback: str = None) -> FeedbackType:
+    """Require a response.
+
+    Args:
+        question (Question): Question.
+        feedback (str, optional): Feedback if the user didn't respond. Defaults to None.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    if question.response in (None, set()):
+        return False, feedback
+    return None
+
+
+@validate.register
+def response_in(
+    question: "Question", valid_set: Iterable, feedback: str = None
+) -> FeedbackType:
+    """Require that the user's response be in a given set.
+
+    Args:
+        question (Question): Question.
+        valid_set (Iterable): Set of valid responses.
+        feedback (str, optional): Feedback if the user's response isn't in the valid
+            set. Defaults to None.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    if question.response not in valid_set:
+        return False, feedback
+    return None
+
+
+@validate.register
+def response_not_in(
+    question: "Question", invalid_set: Iterable, feedback: str = None
+) -> FeedbackType:
+    """Require that the user's response not be in a given set.
+
+    Args:
+        question (Question): Question.
+        invalid_set (Iterable): Set of invalid responses.
+        feedback (str, optional): Feedback if the user's response is in the invalid
+            set. Defaults to None.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    if question.response in invalid_set:
+        return False, feedback
+    return None
+
+
+@validate.register
+def compare_response(
+    question: "Question",
+    value: Any,
+    feedback: str = None,
+    comparison: ComparisonType = "==",
+    how: HowType = "value",
+) -> FeedbackType:
+    """Require that the user's response satsify a comparison.
+
+    Args:
+        question (Question): Question.
+        value (Any): Value to which the response will be compared.
+        feedback (str, optional): Feedback if the comparison fails. Defaults to None.
+        comparison (ComparisonType, optional): Comparison operator. Defaults to ==.
+        how (HowType, optional): How the response should be assessed ("value",
+            "length", "word count", or "decimals"). Defaults to value.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    from ..questions.base import Question
+
+    string_to_operator = {
+        "<": operator.lt,
+        "<=": operator.le,
+        "==": operator.eq,
+        "!=": operator.ne,
+        ">=": operator.ge,
+        ">": operator.gt,
+    }
+    transform_response = HOW_TO_TRANSFORM[how] if is_instance(how, str) else how  # type: ignore
+
+    response = transform_response(question)  # type: ignore
+
+    if is_instance(value, Question):
+        value = transform_response(value)  # type: ignore
+
+    if is_instance(comparison, str):
+        comparison = string_to_operator[comparison]  # type: ignore
+
+    if not comparison(response, value):  # type: ignore
+        return False, feedback
+    return None
+
+
+@validate.register
+def response_in_range(
+    question: "Question",
+    min_value: Any,
+    max_value: Any,
+    feedback: str = None,
+    how: HowType = "value",
+) -> FeedbackType:
+    """Require the user's response to be in a given range of values.
+
+    Args:
+        question (Question): Question.
+        min_value (Any): Minimum value.
+        max_value (Any): Maximum value.
+        feedback (str, optional): Feedback if the response is not in the required
+            range. Defaults to None.
+        how (HowType, optional): How the response should be assessed ("value",
+            "length", "word count", or "decimals"). Defaults to value.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    response = HOW_TO_TRANSFORM[how](question)  # type: ignore
+    if not (min_value <= response <= max_value):
+        return False, feedback
+    return None
+
+
+@validate.register
+def re_full_match(
+    question: "Question",
+    pattern: str,
+    feedback: str = None,
+    flags: Any = 0,
+) -> FeedbackType:
+    """Require that the user's response match a regular expression.
+
+    Args:
+        question (Question): Question.
+        pattern (str): Regular expression pattern.
+        feedback (str, optional): Feedback if the response does not match the pattern.
+            Defaults to None.
+        flags (Any, optional): Flags (see python documentation on ``re.fullmatch``).
+            Defaults to 0.
+
+    Returns:
+        FeedbackType: Feedback.
+    """
+    if not re.fullmatch(pattern, question.response, flags):
+        return False, feedback
+    return None
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/page.py` & `hemlock-survey-1.0.1/src/hemlock/page.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,588 +1,588 @@
-"""Page.
-"""
-from __future__ import annotations
-
-import copy
-import os
-import textwrap
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    Tuple,
-    Union,
-)
-
-from IPython import display
-from flask import render_template, request
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.ext.orderinglist import ordering_list
-from sqlalchemy.orm import validates
-from sqlalchemy_mutable.html import HTMLSettingType
-from sqlalchemy_mutable.types import (
-    HTMLSettingsType,
-    MutablePickleType,
-    MutableDictJSONType,
-)
-from sqlalchemy_mutable.utils import is_instance
-
-from ._custom_types import MutableListPickleType
-from ._navbar import Navbar, RawBrand, RawNavitem, convert_brand, convert_navitem
-from .app import db
-from .data import Data
-from .functional.test_response import random_direction
-from .timer import Timer
-from .utils.random import make_hash
-
-if TYPE_CHECKING:
-    from .questions.base import Question
-
-HASH_LENGTH = 10
-DIR_PATH = os.path.dirname(os.path.realpath(__file__))
-
-CompileType = Callable[["Page"], None]
-SubmitType = Callable[["Page"], None]
-NavigateType = Callable[["Page"], List["Page"]]
-
-
-class Page(db.Model):  # type: ignore
-    """Page.
-
-    A page's primary function is to present users with a list of questions then allow
-    them to navigate to other pages in the survey.
-
-    Args:
-        *questions (Question): Questions for the user.
-        timer (Union[str, Timer], optional): Records the amount of time the user spent
-            on this page. A string is interpreted as the timer's variable name.
-            Defaults to None.
-        data (List[Union[Data, Tuple]], optional): Additional data items. Tuple inputs
-            are used as arguments to the :class:`hemlock.data.Data` constructor.
-            Defaults to None.
-        navbar (Navbar, optional): Navigation bar. Defaults to None.
-        back (Union[bool, str], optional): If a bool, indicates that the user can go
-            back. If a string, this is the text of the back button. Defaults to None.
-        prev_page (Page, optional): The page to which the back button takes the user.
-            If None, the back button takes the user to the previous page. Defaults to
-            None.
-        forward (Union[bool, str], optional): If a bool, indicates that the user can
-            go forward. If a string, this is the text of the forward button. Defaults
-            to None.
-        next_page (Page, optional): The page to which the forward button takes the
-            user. If None, the forward button takes the user to the next page.
-            Defaults to None.
-        template (str, optional): Template used to render the page. Defaults to
-            "hemlock/page.html".
-        compile (Union[CompileType, List[CompileType]], optional): Functions run
-            before this page renders its HTML. Defaults to None.
-        rerun_compile_functions (bool, optional): Indicates that compile functions
-            should be rerun when the user goes back to this page or if the user's
-            responses to this page were invalid. By default, the compile functions are
-            only run when the user goes forward to this page. Defaults to None.
-        submit (Union[SubmitType, List[SubmitType]], optional): Functions run after
-            the user submits his responses. Defaults to None.
-        test_direction (Union[str, Callable[[Page], str]], optional): The direction
-            ("forward" or "back") to navigate from this page during testing. This may
-            also be a function that takes a page and returns a direction. Defaults to
-            None.
-        navigate (NavigateType, optional): This function runs after the submit
-            functions and creates a branch off of this page. Defaults to None.
-        terminal (bool, optional): Indicates that this is the last page of the survey.
-            Defaults to False.
-        params (Any, optional): Additional parameters. Defaults to None.
-        extra_html_settings (Mapping[str, HTMLSettingType], optional): Additional HTML
-            settings. Defaults to None.
-
-    Attributes:
-        tree (Tree): Tree to which this page belongs.
-        branch (List[Page]): Pages that branch off of the current page.
-        root (Page): The page to whose branch this page belongs.
-        index (int): This page's position on its root's branch.
-        questions (List[Question]): Questions for the user.
-        timer (Timer): Records the amount of time the user spent on this page.
-        data (List[Data], optional): Additional data items.
-        navbar (Navbar, optional): Navigation bar.
-        back (Optional[str]): The text of the back button. If None, the user cannot go
-            back from this page.
-        prev_page (Page): The page to which the back button takes the user.
-        forward (Optional[str]): The text of the forward button. If None, the user
-            cannot go forward from this page.
-        next_page (Page, optional): The page to which the forward button takes the
-            user.
-        template (str): Template used to render the page.
-        compile (List[CompileType]): Functions run before this page renders its HTML.
-        rerun_compile_functions (bool): Indicates that compile functions should be
-            rerun when the user goes back to this page or if the user's responses to
-            this page were invalid.
-        submit (List[SubmitType]): Functions run after the user submits his responses.
-        navigate (NavigateType): This function runs after the submit functions and
-            creates a branch off of this page.
-        test_direction (Union[str, Callable[[Page], str]]): The direction ("forward" or
-            "back") to navigate from this page during testing. This may also be a
-            function that takes a page and returns a direction.
-        terminal (bool): Indicates that this is the last page of the survey.
-        params (Any): Additional parameters.
-        html_settings (Mapping[str, HTMLSettingType]): HTML settings.
-        direction_from (Optional[str]): Direction which the user is navigating from
-            this page. Either "forward", "back", or "invalid".
-        direction_to (Optional[str]): Direction which the user navigated to this page.
-            Either "forward", "back", or "invalid".
-
-    Examples:
-
-        .. doctest::
-
-            >>> from hemlock import Page
-            >>> from hemlock.questions import Input, Label
-            >>> Page(
-            ...     Label("Hello, world!"),
-            ...     Input("What's your name?")
-            ... )
-            <Page None>
-                <Label Hello, world! - default: None>
-                <Input What's your name? - default: None>
-
-    Notes:
-
-        Data can be input as :class:`hemlock.data.Data` objects or as tuples. Tuple
-        inputs are used as arguments for the ``Data`` constructor.
-
-        .. doctest::
-
-            >>> from hemlock import User, Page, Data, create_test_app
-            >>> def seed():
-            ...     return Page(data=[("variable0", 0), Data("variable1", 1)])
-            ...
-            >>> app = create_test_app()
-            >>> user = User.make_test_user(seed)
-            >>> _ = user.test_get()
-            >>> user.get_data()[["variable0", "variable1"]]
-               variable0  variable1
-            0          0          1
-    """
-
-    id = db.Column(db.Integer, primary_key=True)
-
-    defaults: Dict[str, Any] = dict(
-        navbar=None,
-        error=None,
-        back=False,
-        forward=True,
-        template="hemlock/page.html",
-        compile=[],
-        submit=[],
-        navigate=None,
-        test_direction=random_direction,
-        rerun_compile_functions=False,
-        params=None,
-        html_settings={
-            "css": open(os.path.join(DIR_PATH, "_page_css.html"), "r")
-            .read()
-            .splitlines(),
-            "js": open(os.path.join(DIR_PATH, "_page_js.html"), "r")
-            .read()
-            .splitlines(),
-            "div": {
-                "class": ["container", "min-vh-100", "d-flex", "align-items-center"],
-                "style": {"padding-bottom": "20px"},
-            },
-            "back-button": {
-                "id": "back-button",
-                "class": ["btn", "btn-primary"],
-                "name": "direction",
-                "value": "back",
-                "type": "submit",
-                "style": {"float": "left"},
-            },
-            "forward-button": {
-                "id": "forward-button",
-                "class": ["btn", "btn-primary"],
-                "name": "direction",
-                "value": "forward",
-                "type": "submit",
-                "style": {"float": "right"},
-            },
-        },
-        banner="""
-        <div class="text-center">
-            <img src="https://dsbowen.gitlab.io/hemlock/_static/banner.png" style="max-width: 200px;" alt="Banner">
-        </div>
-        """,
-    )
-
-    _tree_id = db.Column(db.Integer, db.ForeignKey("tree.id"))
-    _tree_head_id = db.Column(db.Integer, db.ForeignKey("tree.id"))
-
-    _branch_id = db.Column(db.Integer, db.ForeignKey("page.id"))
-    branch = db.relationship(
-        "Page",
-        backref=db.backref("root", remote_side=[id]),
-        order_by="Page.index",
-        collection_class=ordering_list("index"),
-        foreign_keys=_branch_id,
-    )
-
-    questions = db.relationship(
-        "Question",
-        backref="page",
-        order_by="Question.index",
-        collection_class=ordering_list("index"),
-        foreign_keys="Question._page_question_id",
-    )
-
-    _prev_page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
-    prev_page = db.relationship("Page", foreign_keys=_prev_page_id, remote_side=[id])
-
-    _next_page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
-    next_page = db.relationship("Page", foreign_keys=_next_page_id, remote_side=[id])
-
-    data = db.relationship(
-        "Data",
-        order_by="Data.index",
-        collection_class=ordering_list("index"),
-        foreign_keys="Data._page_id",
-    )
-
-    @validates("data")
-    def _validate_data(self, key: str, data: Union[Data, Tuple]) -> Data:
-        """Data can be input as a :class:`hemlock.data.Data` object or a tuple.
-
-        Tuple inputs are used as arguments for the ``Data`` constructor.
-        """
-        return data if isinstance(data, Data) else Data(*data)
-
-    timer = db.relationship("Timer", uselist=False, foreign_keys="Timer._page_timer_id")
-
-    # HTML attributes
-    hash = db.Column(db.String(HASH_LENGTH))
-    navbar = db.Column(MutableDictJSONType)
-    back = db.Column(db.String)
-    forward = db.Column(db.String)
-    template = db.Column(db.String)
-    html_settings = db.Column(HTMLSettingsType)
-
-    @validates("navbar")
-    def _validate_navbar(
-        self, key: str, value: Optional[Tuple[RawBrand, Iterable[RawNavitem]]]
-    ) -> Optional[Navbar]:
-        if value is None:
-            return None
-
-        brand, navitems = value
-        return {
-            "hash": make_hash(),
-            "brand": convert_brand(brand),
-            "navitems": [convert_navitem(item) for item in navitems],
-        }
-
-    @validates("back", "forward")
-    def _validate_direction(
-        self, key: str, value: Union[str, bool, None]
-    ) -> Optional[str]:
-        if not value:
-            return None
-
-        if value is True:
-            return ">>" if key == "forward" else "<<"
-
-        # value is str
-        return value  # type: ignore
-
-    # Function attributes
-    compile = db.Column(MutableListPickleType)
-    submit = db.Column(MutableListPickleType)
-    navigate = db.Column(MutablePickleType)
-    test_direction = db.Column(MutablePickleType)
-
-    # Additional attributes
-    params = db.Column(MutablePickleType)
-    direction_from = db.Column(db.String(8))
-    direction_to = db.Column(db.String(8))
-    index = db.Column(db.Integer)
-    terminal = db.Column(db.Boolean, default=False)
-    rerun_compile_functions = db.Column(db.Boolean)
-
-    @hybrid_property
-    def root_branch(self) -> List[Page]:
-        """Get the branch to which this page belongs.
-
-        The root branch is this page's root's branch (implying that this page is on the
-        returned branch). The root is either a tree or a root page.
-
-        Returns:
-            List[Page]: Branch.
-        """
-        return (self.tree or self.root).branch
-
-    @hybrid_property
-    def is_first_page(self) -> bool:
-        """Indicates that this page is the first page (of its tree).
-
-        Returns:
-            bool: Indicator.
-        """
-        # this page is the zeroth of the pages directly connected to the tree
-        return self.tree is not None and self.index == 0
-
-    @hybrid_property
-    def is_last_page(self) -> bool:
-        """Indicates that this page is the last page (of its tree).
-
-        Returns:
-            bool: Indicator.
-        """
-        if self.terminal:
-            return True
-
-        if self.tree is None and self.root is None:
-            # this page is not connected to a tree or root page
-            # this will most often occur during testing
-            return False
-
-        if self.branch or self.navigate is not None:
-            # this page either already has a branch
-            # or will get a new branch when submitted
-            return False
-
-        page = self
-        while page is page.root_branch[-1]:
-            page = page.root
-            if page is None:
-                return True
-
-        return False
-
-    @hybrid_property
-    def is_valid(self) -> bool:
-        """Indicates that the user's responses to all questions on this page are valid.
-
-        Returns:
-            bool: Indicator.
-        """
-        return all([question.is_valid in (True, None) for question in self.questions])
-
-    def __init__(
-        self,
-        *questions: "Question",
-        timer: Union[str, Timer] = None,
-        data: List[Data] = None,
-        navbar=None,  # TODO: typehint for navbar
-        back: Union[bool, str] = None,
-        prev_page: Page = None,
-        forward: Union[bool, str] = None,
-        next_page: Page = None,
-        template: str = "hemlock/page.html",
-        compile: Union[CompileType, List[CompileType]] = None,
-        rerun_compile_functions: bool = None,
-        submit: Union[SubmitType, List[SubmitType]] = None,
-        navigate: NavigateType = None,
-        test_direction: Union[str, Callable[[Page], str]] = None,
-        terminal: bool = False,
-        params: Any = None,
-        extra_html_settings: Mapping[str, HTMLSettingType] = None,
-    ):
-        def set_default_attribute(name, value, copy_default=False):
-            if value is None:
-                value = self.defaults[name]
-                if copy_default:
-                    value = copy.deepcopy(value)
-
-            setattr(self, name, value)
-
-        self.hash = make_hash(HASH_LENGTH)
-
-        self.questions = list(questions)
-        self.data = [] if data is None else data
-        if timer is None:
-            self.timer = Timer()
-        elif is_instance(timer, str):
-            self.timer = Timer(variable=timer)
-        else:
-            self.timer = timer
-
-        set_default_attribute("navbar", navbar, True)
-        set_default_attribute("back", back)
-        self.prev_page = prev_page
-        set_default_attribute("forward", forward)
-        self.next_page = next_page
-        set_default_attribute("template", template)
-
-        set_default_attribute("compile", compile, True)
-        set_default_attribute("rerun_compile_functions", rerun_compile_functions)
-        set_default_attribute("submit", submit, True)
-        set_default_attribute("navigate", navigate, True)
-        set_default_attribute("test_direction", test_direction, True)
-
-        self.terminal = terminal
-        set_default_attribute("params", params, True)
-
-        self.html_settings = copy.deepcopy(self.defaults["html_settings"])
-        if extra_html_settings is not None:
-            self.html_settings.update_settings(extra_html_settings)  # type: ignore
-
-    def __repr__(self):
-        return self.print()
-
-    def print(
-        self,
-        test_responses: Dict[Question, Any] = None,
-        direction: str = None,
-    ) -> str:
-        """Print the page.
-
-        Args:
-            test_responses (Dict[, optional): Maps questions on the page to test
-                responses. Defaults to None.
-            direction (str, optional): Test direction. Defaults to None.
-
-        Returns:
-            str: Page representation.
-        """
-        initial_indent = ""
-        subsequent_indent = 4 * " "
-
-        if not self.questions:
-            question_text = ""
-        else:
-            if test_responses is None:
-                question_text = "\n".join(
-                    [str(question) for question in self.questions]
-                )
-            else:
-                question_texts = []
-                for question in self.questions:
-                    test_response = test_responses.get(question)
-                    question_texts.append(
-                        f"{question}\n{subsequent_indent}test response: {repr(test_response)}"
-                    )
-                question_text = "\n".join(question_texts)
-
-            question_text = f"\n{textwrap.indent(question_text, subsequent_indent)}"
-
-        if direction is None:
-            direction_text = ""
-        else:
-            direction_text = f"\n{subsequent_indent}test direction: {repr(direction)}"
-
-        terminal = " terminal" if self.is_last_page else ""
-        return textwrap.indent(
-            f"<{self.__class__.__qualname__} {self.get_position()}{terminal}>{question_text}{direction_text}",
-            initial_indent,
-        )
-
-    def get_position(self) -> str:
-        """Get this page's position on its tree.
-
-        Returns:
-            str: Position.
-        """
-        indices = []
-        page = self
-        while page is not None:
-            indices.append(str(page.index))
-            page = page.root
-        indices.reverse()
-        return ".".join(indices)
-
-    def display(self):
-        # we remove the min-vh-100 class from the div tag wrapping the form and add it back
-        # after displaying in a notebook.
-        # the min-vh-100 class makes sure the form extends from the top to the botton of
-        # the screen, but we don't want this when displaying in a notebook
-        div_class = self.html_settings["div"]["class"]
-        vh_100 = "min-vh-100" in div_class
-        if vh_100:
-            div_class = self.html_settings["div"]["class"].copy()
-            self.html_settings["div"]["class"].remove("min-vh-100")
-
-        return_value = display.HTML(self.render(for_notebook_display=True))
-
-        if vh_100:
-            self.html_settings["div"]["class"] = div_class
-
-        return return_value
-
-    def clear_feedback(self) -> None:
-        """Clear feedback on all of this page's questions."""
-        [question.clear_feedback() for question in self.questions]
-
-    def clear_response(self) -> None:
-        """Clear the user's responses (and feedback) to all of this page's questions."""
-        [question.clear_response() for question in self.questions]
-
-    def render(self, for_notebook_display=False) -> str:
-        """Render the HTML.
-
-        Returns:
-            str: HTML.
-        """
-        return render_template(
-            self.template,
-            page=self,
-            navbar=None,
-            for_notebook_display=for_notebook_display,
-        )
-
-    def get(self, for_notebook_display=False) -> str:
-        """Process a GET request.
-
-        Args:
-            for_notebook_display (bool, optional): Indicates that this is a test
-                user's request and the output will displayed in a notebook. Defaults
-                to False.
-
-        Returns:
-            str: Rendered HTML.
-        """
-        if self.direction_to in ("forward", None) or self.rerun_compile_functions:
-            [func(self) for func in self.compile]
-            [question.run_compile_functions() for question in self.questions]
-
-        html = self.render(for_notebook_display)
-        self.timer.start()
-        return html
-
-    def post(self) -> str:
-        """Process a POST request.
-
-        Returns:
-            str: The direction the user should go from this page ("forward", "back",
-                or "invalid").
-        """
-        self.timer.pause()
-
-        # record form data
-        self.direction_from = request.form["direction"]
-        for question in self.questions:
-            question.record_response()
-
-        if self.direction_from == "forward":
-            # validate user responses
-            self.clear_feedback()
-            for question in self.questions:
-                question.run_validate_functions()
-
-            if self.is_valid:
-                # record data and run submit and navigate functions
-                for question in self.questions:
-                    question.record_data()
-
-                for func in self.submit:
-                    func(self)
-                for question in self.questions:
-                    question.run_submit_functions()
-
-                if self.navigate is not None:
-                    branch = self.navigate(self)
-                    if not is_instance(branch, list):
-                        branch = [branch]
-                    self.branch = branch
-            else:
-                self.direction_from = "invalid"
-
-        return self.direction_from
+"""Page.
+"""
+from __future__ import annotations
+
+import copy
+import os
+import textwrap
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    Union,
+)
+
+from IPython import display
+from flask import render_template, request
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.ext.orderinglist import ordering_list
+from sqlalchemy.orm import validates
+from sqlalchemy_mutable.html import HTMLSettingType
+from sqlalchemy_mutable.types import (
+    HTMLSettingsType,
+    MutablePickleType,
+    MutableDictJSONType,
+)
+from sqlalchemy_mutable.utils import is_instance
+
+from ._custom_types import MutableListPickleType
+from ._navbar import Navbar, RawBrand, RawNavitem, convert_brand, convert_navitem
+from .app import db
+from .data import Data
+from .functional.test_response import random_direction
+from .timer import Timer
+from .utils.random import make_hash
+
+if TYPE_CHECKING:
+    from .questions.base import Question
+
+HASH_LENGTH = 10
+DIR_PATH = os.path.dirname(os.path.realpath(__file__))
+
+CompileType = Callable[["Page"], None]
+SubmitType = Callable[["Page"], None]
+NavigateType = Callable[["Page"], List["Page"]]
+
+
+class Page(db.Model):  # type: ignore
+    """Page.
+
+    A page's primary function is to present users with a list of questions then allow
+    them to navigate to other pages in the survey.
+
+    Args:
+        *questions (Question): Questions for the user.
+        timer (Union[str, Timer], optional): Records the amount of time the user spent
+            on this page. A string is interpreted as the timer's variable name.
+            Defaults to None.
+        data (List[Union[Data, Tuple]], optional): Additional data items. Tuple inputs
+            are used as arguments to the :class:`hemlock.data.Data` constructor.
+            Defaults to None.
+        navbar (Navbar, optional): Navigation bar. Defaults to None.
+        back (Union[bool, str], optional): If a bool, indicates that the user can go
+            back. If a string, this is the text of the back button. Defaults to None.
+        prev_page (Page, optional): The page to which the back button takes the user.
+            If None, the back button takes the user to the previous page. Defaults to
+            None.
+        forward (Union[bool, str], optional): If a bool, indicates that the user can
+            go forward. If a string, this is the text of the forward button. Defaults
+            to None.
+        next_page (Page, optional): The page to which the forward button takes the
+            user. If None, the forward button takes the user to the next page.
+            Defaults to None.
+        template (str, optional): Template used to render the page. Defaults to
+            "hemlock/page.html".
+        compile (Union[CompileType, List[CompileType]], optional): Functions run
+            before this page renders its HTML. Defaults to None.
+        rerun_compile_functions (bool, optional): Indicates that compile functions
+            should be rerun when the user goes back to this page or if the user's
+            responses to this page were invalid. By default, the compile functions are
+            only run when the user goes forward to this page. Defaults to None.
+        submit (Union[SubmitType, List[SubmitType]], optional): Functions run after
+            the user submits his responses. Defaults to None.
+        test_direction (Union[str, Callable[[Page], str]], optional): The direction
+            ("forward" or "back") to navigate from this page during testing. This may
+            also be a function that takes a page and returns a direction. Defaults to
+            None.
+        navigate (NavigateType, optional): This function runs after the submit
+            functions and creates a branch off of this page. Defaults to None.
+        terminal (bool, optional): Indicates that this is the last page of the survey.
+            Defaults to False.
+        params (Any, optional): Additional parameters. Defaults to None.
+        extra_html_settings (Mapping[str, HTMLSettingType], optional): Additional HTML
+            settings. Defaults to None.
+
+    Attributes:
+        tree (Tree): Tree to which this page belongs.
+        branch (List[Page]): Pages that branch off of the current page.
+        root (Page): The page to whose branch this page belongs.
+        index (int): This page's position on its root's branch.
+        questions (List[Question]): Questions for the user.
+        timer (Timer): Records the amount of time the user spent on this page.
+        data (List[Data], optional): Additional data items.
+        navbar (Navbar, optional): Navigation bar.
+        back (Optional[str]): The text of the back button. If None, the user cannot go
+            back from this page.
+        prev_page (Page): The page to which the back button takes the user.
+        forward (Optional[str]): The text of the forward button. If None, the user
+            cannot go forward from this page.
+        next_page (Page, optional): The page to which the forward button takes the
+            user.
+        template (str): Template used to render the page.
+        compile (List[CompileType]): Functions run before this page renders its HTML.
+        rerun_compile_functions (bool): Indicates that compile functions should be
+            rerun when the user goes back to this page or if the user's responses to
+            this page were invalid.
+        submit (List[SubmitType]): Functions run after the user submits his responses.
+        navigate (NavigateType): This function runs after the submit functions and
+            creates a branch off of this page.
+        test_direction (Union[str, Callable[[Page], str]]): The direction ("forward" or
+            "back") to navigate from this page during testing. This may also be a
+            function that takes a page and returns a direction.
+        terminal (bool): Indicates that this is the last page of the survey.
+        params (Any): Additional parameters.
+        html_settings (Mapping[str, HTMLSettingType]): HTML settings.
+        direction_from (Optional[str]): Direction which the user is navigating from
+            this page. Either "forward", "back", or "invalid".
+        direction_to (Optional[str]): Direction which the user navigated to this page.
+            Either "forward", "back", or "invalid".
+
+    Examples:
+
+        .. doctest::
+
+            >>> from hemlock import Page
+            >>> from hemlock.questions import Input, Label
+            >>> Page(
+            ...     Label("Hello, world!"),
+            ...     Input("What's your name?")
+            ... )
+            <Page None>
+                <Label Hello, world! - default: None>
+                <Input What's your name? - default: None>
+
+    Notes:
+
+        Data can be input as :class:`hemlock.data.Data` objects or as tuples. Tuple
+        inputs are used as arguments for the ``Data`` constructor.
+
+        .. doctest::
+
+            >>> from hemlock import User, Page, Data, create_test_app
+            >>> def seed():
+            ...     return Page(data=[("variable0", 0), Data("variable1", 1)])
+            ...
+            >>> app = create_test_app()
+            >>> user = User.make_test_user(seed)
+            >>> _ = user.test_get()
+            >>> user.get_data()[["variable0", "variable1"]]
+               variable0  variable1
+            0          0          1
+    """
+
+    id = db.Column(db.Integer, primary_key=True)
+
+    defaults: Dict[str, Any] = dict(
+        navbar=None,
+        error=None,
+        back=False,
+        forward=True,
+        template="hemlock/page.html",
+        compile=[],
+        submit=[],
+        navigate=None,
+        test_direction=random_direction,
+        rerun_compile_functions=False,
+        params=None,
+        html_settings={
+            "css": open(os.path.join(DIR_PATH, "_page_css.html"), "r")
+            .read()
+            .splitlines(),
+            "js": open(os.path.join(DIR_PATH, "_page_js.html"), "r")
+            .read()
+            .splitlines(),
+            "div": {
+                "class": ["container", "min-vh-100", "d-flex", "align-items-center"],
+                "style": {"padding-bottom": "20px"},
+            },
+            "back-button": {
+                "id": "back-button",
+                "class": ["btn", "btn-primary"],
+                "name": "direction",
+                "value": "back",
+                "type": "submit",
+                "style": {"float": "left"},
+            },
+            "forward-button": {
+                "id": "forward-button",
+                "class": ["btn", "btn-primary"],
+                "name": "direction",
+                "value": "forward",
+                "type": "submit",
+                "style": {"float": "right"},
+            },
+        },
+        banner="""
+        <div class="text-center">
+            <img src="https://dsbowen.gitlab.io/hemlock/_static/banner.png" style="max-width: 200px;" alt="Banner">
+        </div>
+        """,
+    )
+
+    _tree_id = db.Column(db.Integer, db.ForeignKey("tree.id"))
+    _tree_head_id = db.Column(db.Integer, db.ForeignKey("tree.id"))
+
+    _branch_id = db.Column(db.Integer, db.ForeignKey("page.id"))
+    branch = db.relationship(
+        "Page",
+        backref=db.backref("root", remote_side=[id]),
+        order_by="Page.index",
+        collection_class=ordering_list("index"),
+        foreign_keys=_branch_id,
+    )
+
+    questions = db.relationship(
+        "Question",
+        backref="page",
+        order_by="Question.index",
+        collection_class=ordering_list("index"),
+        foreign_keys="Question._page_question_id",
+    )
+
+    _prev_page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
+    prev_page = db.relationship("Page", foreign_keys=_prev_page_id, remote_side=[id])
+
+    _next_page_id = db.Column(db.Integer, db.ForeignKey("page.id"))
+    next_page = db.relationship("Page", foreign_keys=_next_page_id, remote_side=[id])
+
+    data = db.relationship(
+        "Data",
+        order_by="Data.index",
+        collection_class=ordering_list("index"),
+        foreign_keys="Data._page_id",
+    )
+
+    @validates("data")
+    def _validate_data(self, key: str, data: Union[Data, Tuple]) -> Data:
+        """Data can be input as a :class:`hemlock.data.Data` object or a tuple.
+
+        Tuple inputs are used as arguments for the ``Data`` constructor.
+        """
+        return data if isinstance(data, Data) else Data(*data)
+
+    timer = db.relationship("Timer", uselist=False, foreign_keys="Timer._page_timer_id")
+
+    # HTML attributes
+    hash = db.Column(db.String(HASH_LENGTH))
+    navbar = db.Column(MutableDictJSONType)
+    back = db.Column(db.String)
+    forward = db.Column(db.String)
+    template = db.Column(db.String)
+    html_settings = db.Column(HTMLSettingsType)
+
+    @validates("navbar")
+    def _validate_navbar(
+        self, key: str, value: Optional[Tuple[RawBrand, Iterable[RawNavitem]]]
+    ) -> Optional[Navbar]:
+        if value is None:
+            return None
+
+        brand, navitems = value
+        return {
+            "hash": make_hash(),
+            "brand": convert_brand(brand),
+            "navitems": [convert_navitem(item) for item in navitems],
+        }
+
+    @validates("back", "forward")
+    def _validate_direction(
+        self, key: str, value: Union[str, bool, None]
+    ) -> Optional[str]:
+        if not value:
+            return None
+
+        if value is True:
+            return ">>" if key == "forward" else "<<"
+
+        # value is str
+        return value  # type: ignore
+
+    # Function attributes
+    compile = db.Column(MutableListPickleType)
+    submit = db.Column(MutableListPickleType)
+    navigate = db.Column(MutablePickleType)
+    test_direction = db.Column(MutablePickleType)
+
+    # Additional attributes
+    params = db.Column(MutablePickleType)
+    direction_from = db.Column(db.String(8))
+    direction_to = db.Column(db.String(8))
+    index = db.Column(db.Integer)
+    terminal = db.Column(db.Boolean, default=False)
+    rerun_compile_functions = db.Column(db.Boolean)
+
+    @hybrid_property
+    def root_branch(self) -> List[Page]:
+        """Get the branch to which this page belongs.
+
+        The root branch is this page's root's branch (implying that this page is on the
+        returned branch). The root is either a tree or a root page.
+
+        Returns:
+            List[Page]: Branch.
+        """
+        return (self.tree or self.root).branch
+
+    @hybrid_property
+    def is_first_page(self) -> bool:
+        """Indicates that this page is the first page (of its tree).
+
+        Returns:
+            bool: Indicator.
+        """
+        # this page is the zeroth of the pages directly connected to the tree
+        return self.tree is not None and self.index == 0
+
+    @hybrid_property
+    def is_last_page(self) -> bool:
+        """Indicates that this page is the last page (of its tree).
+
+        Returns:
+            bool: Indicator.
+        """
+        if self.terminal:
+            return True
+
+        if self.tree is None and self.root is None:
+            # this page is not connected to a tree or root page
+            # this will most often occur during testing
+            return False
+
+        if self.branch or self.navigate is not None:
+            # this page either already has a branch
+            # or will get a new branch when submitted
+            return False
+
+        page = self
+        while page is page.root_branch[-1]:
+            page = page.root
+            if page is None:
+                return True
+
+        return False
+
+    @hybrid_property
+    def is_valid(self) -> bool:
+        """Indicates that the user's responses to all questions on this page are valid.
+
+        Returns:
+            bool: Indicator.
+        """
+        return all([question.is_valid in (True, None) for question in self.questions])
+
+    def __init__(
+        self,
+        *questions: "Question",
+        timer: Union[str, Timer] = None,
+        data: List[Data] = None,
+        navbar=None,  # TODO: typehint for navbar
+        back: Union[bool, str] = None,
+        prev_page: Page = None,
+        forward: Union[bool, str] = None,
+        next_page: Page = None,
+        template: str = "hemlock/page.html",
+        compile: Union[CompileType, List[CompileType]] = None,
+        rerun_compile_functions: bool = None,
+        submit: Union[SubmitType, List[SubmitType]] = None,
+        navigate: NavigateType = None,
+        test_direction: Union[str, Callable[[Page], str]] = None,
+        terminal: bool = False,
+        params: Any = None,
+        extra_html_settings: Mapping[str, HTMLSettingType] = None,
+    ):
+        def set_default_attribute(name, value, copy_default=False):
+            if value is None:
+                value = self.defaults[name]
+                if copy_default:
+                    value = copy.deepcopy(value)
+
+            setattr(self, name, value)
+
+        self.hash = make_hash(HASH_LENGTH)
+
+        self.questions = list(questions)
+        self.data = [] if data is None else data
+        if timer is None:
+            self.timer = Timer()
+        elif is_instance(timer, str):
+            self.timer = Timer(variable=timer)
+        else:
+            self.timer = timer
+
+        set_default_attribute("navbar", navbar, True)
+        set_default_attribute("back", back)
+        self.prev_page = prev_page
+        set_default_attribute("forward", forward)
+        self.next_page = next_page
+        set_default_attribute("template", template)
+
+        set_default_attribute("compile", compile, True)
+        set_default_attribute("rerun_compile_functions", rerun_compile_functions)
+        set_default_attribute("submit", submit, True)
+        set_default_attribute("navigate", navigate, True)
+        set_default_attribute("test_direction", test_direction, True)
+
+        self.terminal = terminal
+        set_default_attribute("params", params, True)
+
+        self.html_settings = copy.deepcopy(self.defaults["html_settings"])
+        if extra_html_settings is not None:
+            self.html_settings.update_settings(extra_html_settings)  # type: ignore
+
+    def __repr__(self):
+        return self.print()
+
+    def print(
+        self,
+        test_responses: Dict[Question, Any] = None,
+        direction: str = None,
+    ) -> str:
+        """Print the page.
+
+        Args:
+            test_responses (Dict[, optional): Maps questions on the page to test
+                responses. Defaults to None.
+            direction (str, optional): Test direction. Defaults to None.
+
+        Returns:
+            str: Page representation.
+        """
+        initial_indent = ""
+        subsequent_indent = 4 * " "
+
+        if not self.questions:
+            question_text = ""
+        else:
+            if test_responses is None:
+                question_text = "\n".join(
+                    [str(question) for question in self.questions]
+                )
+            else:
+                question_texts = []
+                for question in self.questions:
+                    test_response = test_responses.get(question)
+                    question_texts.append(
+                        f"{question}\n{subsequent_indent}test response: {repr(test_response)}"
+                    )
+                question_text = "\n".join(question_texts)
+
+            question_text = f"\n{textwrap.indent(question_text, subsequent_indent)}"
+
+        if direction is None:
+            direction_text = ""
+        else:
+            direction_text = f"\n{subsequent_indent}test direction: {repr(direction)}"
+
+        terminal = " terminal" if self.is_last_page else ""
+        return textwrap.indent(
+            f"<{self.__class__.__qualname__} {self.get_position()}{terminal}>{question_text}{direction_text}",
+            initial_indent,
+        )
+
+    def get_position(self) -> str:
+        """Get this page's position on its tree.
+
+        Returns:
+            str: Position.
+        """
+        indices = []
+        page = self
+        while page is not None:
+            indices.append(str(page.index))
+            page = page.root
+        indices.reverse()
+        return ".".join(indices)
+
+    def display(self):
+        # we remove the min-vh-100 class from the div tag wrapping the form and add it back
+        # after displaying in a notebook.
+        # the min-vh-100 class makes sure the form extends from the top to the botton of
+        # the screen, but we don't want this when displaying in a notebook
+        div_class = self.html_settings["div"]["class"]
+        vh_100 = "min-vh-100" in div_class
+        if vh_100:
+            div_class = self.html_settings["div"]["class"].copy()
+            self.html_settings["div"]["class"].remove("min-vh-100")
+
+        return_value = display.HTML(self.render(for_notebook_display=True))
+
+        if vh_100:
+            self.html_settings["div"]["class"] = div_class
+
+        return return_value
+
+    def clear_feedback(self) -> None:
+        """Clear feedback on all of this page's questions."""
+        [question.clear_feedback() for question in self.questions]
+
+    def clear_response(self) -> None:
+        """Clear the user's responses (and feedback) to all of this page's questions."""
+        [question.clear_response() for question in self.questions]
+
+    def render(self, for_notebook_display=False) -> str:
+        """Render the HTML.
+
+        Returns:
+            str: HTML.
+        """
+        return render_template(
+            self.template,
+            page=self,
+            navbar=None,
+            for_notebook_display=for_notebook_display,
+        )
+
+    def get(self, for_notebook_display=False) -> str:
+        """Process a GET request.
+
+        Args:
+            for_notebook_display (bool, optional): Indicates that this is a test
+                user's request and the output will displayed in a notebook. Defaults
+                to False.
+
+        Returns:
+            str: Rendered HTML.
+        """
+        if self.direction_to in ("forward", None) or self.rerun_compile_functions:
+            [func(self) for func in self.compile]
+            [question.run_compile_functions() for question in self.questions]
+
+        html = self.render(for_notebook_display)
+        self.timer.start()
+        return html
+
+    def post(self) -> str:
+        """Process a POST request.
+
+        Returns:
+            str: The direction the user should go from this page ("forward", "back",
+                or "invalid").
+        """
+        self.timer.pause()
+
+        # record form data
+        self.direction_from = request.form["direction"]
+        for question in self.questions:
+            question.record_response()
+
+        if self.direction_from == "forward":
+            # validate user responses
+            self.clear_feedback()
+            for question in self.questions:
+                question.run_validate_functions()
+
+            if self.is_valid:
+                # record data and run submit and navigate functions
+                for question in self.questions:
+                    question.record_data()
+
+                for func in self.submit:
+                    func(self)
+                for question in self.questions:
+                    question.run_submit_functions()
+
+                if self.navigate is not None:
+                    branch = self.navigate(self)
+                    if not is_instance(branch, list):
+                        branch = [branch]
+                    self.branch = branch
+            else:
+                self.direction_from = "invalid"
+
+        return self.direction_from
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/check.py` & `hemlock-survey-1.0.1/src/hemlock/questions/check.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""Check.
-"""
-from __future__ import annotations
-
-import copy
-from typing import Any
-
-from ..app import db
-from .choice_base import ChoiceQuestion
-
-
-class Check(ChoiceQuestion):
-    """Check.
-
-    A check question allows users to select one or more choices by checking a box.
-
-    Subclasses :class:`hemlock.questions.choice_base.ChoiceQuestion`.
-
-    Args:
-        *args (Any): Passed to :class:`hemlock.questions.choice_base.ChoiceQuestion` constructor.
-        inline (bool, optional): Indicates that the choices will appear inline. Defaults
-            to None.
-        switch (bool, optional): Indicates that the check or radio button will be a
-            switch. Defaults to None.
-        **kwargs (Any): Passed to :class:`hemlock.questions.choice_base.ChoiceQuestion` constructor.
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "check"}
-
-    defaults = copy.deepcopy(ChoiceQuestion.defaults)
-    defaults["template"] = "hemlock/check.html"
-    defaults["html_settings"]["div"] = {"class": ["form-check"]}
-
-    def __init__(
-        self, *args: Any, inline: bool = None, switch: bool = None, **kwargs: Any
-    ):
-        super().__init__(*args, **kwargs)
-        if inline is not None:
-            self.set_inline(inline)
-        if switch is not None:
-            self.set_switch(switch)
-
-    def set_inline(self, inline: bool = True) -> None:
-        """Sets the choices to appear inline.
-
-        Args:
-            inline (bool, optional): Indicates that the choices will appear inline. If
-                False, the choices will be stacked. Defaults to True.
-        """
-        self._add_or_remove_class("div", "form-check-inline", inline)
-
-    def set_switch(self, switch: bool = True) -> None:
-        """Indicates that the check or radio button will be a switch.
-
-        Args:
-            switch (bool, optional): Indicates that the check or radio button will be a
-                switch. If False, the buttons will be ordinary check or radio buttons.
-                Defaults to True.
-        """
-        self._add_or_remove_class("div", "form-switch", switch)
+"""Check.
+"""
+from __future__ import annotations
+
+import copy
+from typing import Any
+
+from ..app import db
+from .choice_base import ChoiceQuestion
+
+
+class Check(ChoiceQuestion):
+    """Check.
+
+    A check question allows users to select one or more choices by checking a box.
+
+    Subclasses :class:`hemlock.questions.choice_base.ChoiceQuestion`.
+
+    Args:
+        *args (Any): Passed to :class:`hemlock.questions.choice_base.ChoiceQuestion` constructor.
+        inline (bool, optional): Indicates that the choices will appear inline. Defaults
+            to None.
+        switch (bool, optional): Indicates that the check or radio button will be a
+            switch. Defaults to None.
+        **kwargs (Any): Passed to :class:`hemlock.questions.choice_base.ChoiceQuestion` constructor.
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "check"}
+
+    defaults = copy.deepcopy(ChoiceQuestion.defaults)
+    defaults["template"] = "hemlock/check.html"
+    defaults["html_settings"]["div"] = {"class": ["form-check"]}
+
+    def __init__(
+        self, *args: Any, inline: bool = None, switch: bool = None, **kwargs: Any
+    ):
+        super().__init__(*args, **kwargs)
+        if inline is not None:
+            self.set_inline(inline)
+        if switch is not None:
+            self.set_switch(switch)
+
+    def set_inline(self, inline: bool = True) -> None:
+        """Sets the choices to appear inline.
+
+        Args:
+            inline (bool, optional): Indicates that the choices will appear inline. If
+                False, the choices will be stacked. Defaults to True.
+        """
+        self._add_or_remove_class("div", "form-check-inline", inline)
+
+    def set_switch(self, switch: bool = True) -> None:
+        """Indicates that the check or radio button will be a switch.
+
+        Args:
+            switch (bool, optional): Indicates that the check or radio button will be a
+                switch. If False, the buttons will be ordinary check or radio buttons.
+                Defaults to True.
+        """
+        self._add_or_remove_class("div", "form-switch", switch)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/choice_base.py` & `hemlock-survey-1.0.1/src/hemlock/questions/choice_base.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-"""Mixin for question objects with choice.
-"""
-from __future__ import annotations
-
-import copy
-import textwrap
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Tuple, Union
-
-from flask import request
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy_mutable.utils import is_instance
-
-from .._custom_types import MutableChoiceListType
-from ..app import db
-from ..functional.test_response import random_choices
-from .base import Question
-
-if TYPE_CHECKING:
-    from .._data_frame import DataFrame
-
-ChoiceType = Union[str, Tuple[Any, str], Mapping[Any, Any]]
-
-
-class ChoiceQuestion(Question):
-    """Mixin for questions with choices.
-
-    Subclasses :class:`hemlock.questions.base.Question`.
-
-    Args:
-        label (str, optional): Question label, prompt, or instructions. Defaults to
-            None.
-        choices (List[ChoiceType], optional): Choices that the user can select.
-            Defaults to None.
-        multiple (bool, optional): Indicates that the user can select multiple
-            choices. Defaults to None.
-        record_choice_indices (bool, optional): Indicates that the choice order should
-        be recorded in the data frame. Defaults to None.
-        **kwargs (Any): Additional keyword arguments passed to the
-            :class:`hemlock.questions.base.Question` constructor.
-
-    Attributes:
-        choices (List[Dict[Any, Any]]): Choices that the user can select.
-        multiple (bool): Indicates that the user can select multiple choices.
-        record_choice_indices (bool): Indicates that the choice order should be recorded
-            in the data frame.
-
-    """
-
-    defaults = copy.deepcopy(Question.defaults)
-    defaults.update(
-        {
-            "choices": [],
-            "multiple": False,
-            "test_response": random_choices,
-            "record_choice_indices": False,
-        }
-    )
-
-    choices = db.Column(MutableChoiceListType)
-    choice_template = db.Column(db.String)
-    multiple = db.Column(db.Boolean)
-    record_choice_indices = db.Column(db.Boolean)
-
-    @hybrid_property
-    def response(self) -> Any:
-        """Returns the user's response based on the user's raw response.
-
-        Returns:
-            Any: User's response.
-        """
-        if not self.raw_response and not self.multiple:
-            return None
-
-        return self.raw_response if self.multiple else next(iter(self.raw_response))
-
-    def __init__(
-        self,
-        label: str = None,
-        choices: List[ChoiceType] = None,
-        multiple: bool = None,
-        record_choice_indices: bool = None,
-        **kwargs: Any,
-    ):
-        super().__init__(label, **kwargs)
-        self._set_default_attribute("choices", choices, True)
-        self._set_default_attribute("multiple", multiple)
-        self._set_default_attribute("record_choice_indices", record_choice_indices)
-
-    def __repr__(self):
-        initial_indent = ""
-        subsequent_indent = 4 * " "
-        max_choices = 4
-        placeholder = "[...]"
-        question_text = super().__repr__()
-
-        if not self.choices:
-            choice_text = ""
-        else:
-            choice_values = [
-                f"- {choice['value']}" for choice in self.choices[:max_choices]
-            ]
-            if len(choice_values) == max_choices:
-                choice_values.append(placeholder)
-            choice_text = "\n".join(choice_values)
-            choice_text = f"\n{textwrap.indent(choice_text, subsequent_indent)}"
-
-        return textwrap.indent(question_text + choice_text, initial_indent)
-
-    def is_default(self, value: Any) -> bool:
-        """Indicates that a given choice value is a default.
-
-        Args:
-            value (Any): Value to check.
-
-        Returns:
-            bool: Indicator that the choice value is a default.
-
-        Examples:
-
-            .. doctest::
-
-                >>> from hemlock.questions.choice_base import ChoiceQuestion
-                >>> question = ChoiceQuestion(choices=["Yes", "No"], default="Yes")
-                >>> question.is_default("Yes")
-                True
-                >>> question.is_default("No")
-                False
-
-            Use a ``list`` to indicate that there are multiple default values.
-
-            .. doctest::
-
-                >>> from hemlock.questions.choice_base import ChoiceQuestion
-                >>> question = ChoiceQuestion(choices=["Red", "Green", "Blue"], multiple=True, default=["Red", "Green"])
-                >>> question.is_default("Red")
-                True
-                >>> question.is_default("Green")
-                True
-                >>> question.is_default("Blue")
-                False
-        """
-        default = self.get_default()
-
-        if default is None:
-            return False
-
-        if is_instance(default, (list, set)):
-            return value in default
-
-        return value == default
-
-    def record_response(self) -> None:
-        """Record the user's raw response.
-
-        The raw response is a set of choice values.
-        """
-        # Note: jinja template loop indices start at 1, so we need to subtract 1 for 0 indexing
-        self.raw_response = {
-            self.choices[int(i) - 1]["value"] for i in request.form.getlist(self.hash)
-        }
-
-    def record_data(self) -> None:
-        """Record data based on the user's response."""
-        if self.multiple:
-            self.data = {
-                choice["value"]: int(choice["value"] in self.raw_response)
-                for choice in self.choices
-            }
-            return
-
-        return super().record_data()
-
-    def pack_data(self) -> DataFrame:
-        """Pack the data for insertion into a data frame."""
-        dataframe = super().pack_data()
-        if self.variable is None or not self.record_choice_indices:
-            return dataframe
-
-        choice_indices = {}
-        for i, choice in enumerate(self.choices):
-            choice_indices[f"{self.variable}_{choice['value']}_index"] = i
-        dataframe.add_data(choice_indices, fill_rows=True)
-        dataframe.pad()
-        return dataframe
-
-    def make_raw_test_response(self, response: Any) -> List[Any]:
-        """Create a raw test response from a given test response.
-
-        Args:
-            response (Any): Test response. Must be either a choice value or a set of
-                choice values.
-
-        Returns:
-            List[Any]: List of indices of given choice values.
-        """
-        if response is None:
-            return []
-
-        if not is_instance(response, (list, set)):
-            response = {response}
-
-        # check that test responses are valid choices
-        if invalid_responses := set(response) - set(
-            choice["value"] for choice in self.choices
-        ):
-            raise ValueError(
-                f"Test user chose invalid choices {invalid_responses} for\n{self}."
-            )
-
-        # Note: jinja template loop indices start at 1, so we need to add 1 for 1 indexing
-        return [
-            str(i + 1)
-            for i, choice in enumerate(self.choices)
-            if choice["value"] in response
-        ]
+"""Mixin for question objects with choice.
+"""
+from __future__ import annotations
+
+import copy
+import textwrap
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Tuple, Union
+
+from flask import request
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy_mutable.utils import is_instance
+
+from .._custom_types import MutableChoiceListType
+from ..app import db
+from ..functional.test_response import random_choices
+from .base import Question
+
+if TYPE_CHECKING:
+    from .._data_frame import DataFrame
+
+ChoiceType = Union[str, Tuple[Any, str], Mapping[Any, Any]]
+
+
+class ChoiceQuestion(Question):
+    """Mixin for questions with choices.
+
+    Subclasses :class:`hemlock.questions.base.Question`.
+
+    Args:
+        label (str, optional): Question label, prompt, or instructions. Defaults to
+            None.
+        choices (List[ChoiceType], optional): Choices that the user can select.
+            Defaults to None.
+        multiple (bool, optional): Indicates that the user can select multiple
+            choices. Defaults to None.
+        record_choice_indices (bool, optional): Indicates that the choice order should
+        be recorded in the data frame. Defaults to None.
+        **kwargs (Any): Additional keyword arguments passed to the
+            :class:`hemlock.questions.base.Question` constructor.
+
+    Attributes:
+        choices (List[Dict[Any, Any]]): Choices that the user can select.
+        multiple (bool): Indicates that the user can select multiple choices.
+        record_choice_indices (bool): Indicates that the choice order should be recorded
+            in the data frame.
+
+    """
+
+    defaults = copy.deepcopy(Question.defaults)
+    defaults.update(
+        {
+            "choices": [],
+            "multiple": False,
+            "test_response": random_choices,
+            "record_choice_indices": False,
+        }
+    )
+
+    choices = db.Column(MutableChoiceListType)
+    choice_template = db.Column(db.String)
+    multiple = db.Column(db.Boolean)
+    record_choice_indices = db.Column(db.Boolean)
+
+    @hybrid_property
+    def response(self) -> Any:
+        """Returns the user's response based on the user's raw response.
+
+        Returns:
+            Any: User's response.
+        """
+        if not self.raw_response and not self.multiple:
+            return None
+
+        return self.raw_response if self.multiple else next(iter(self.raw_response))
+
+    def __init__(
+        self,
+        label: str = None,
+        choices: List[ChoiceType] = None,
+        multiple: bool = None,
+        record_choice_indices: bool = None,
+        **kwargs: Any,
+    ):
+        super().__init__(label, **kwargs)
+        self._set_default_attribute("choices", choices, True)
+        self._set_default_attribute("multiple", multiple)
+        self._set_default_attribute("record_choice_indices", record_choice_indices)
+
+    def __repr__(self):
+        initial_indent = ""
+        subsequent_indent = 4 * " "
+        max_choices = 4
+        placeholder = "[...]"
+        question_text = super().__repr__()
+
+        if not self.choices:
+            choice_text = ""
+        else:
+            choice_values = [
+                f"- {choice['value']}" for choice in self.choices[:max_choices]
+            ]
+            if len(choice_values) == max_choices:
+                choice_values.append(placeholder)
+            choice_text = "\n".join(choice_values)
+            choice_text = f"\n{textwrap.indent(choice_text, subsequent_indent)}"
+
+        return textwrap.indent(question_text + choice_text, initial_indent)
+
+    def is_default(self, value: Any) -> bool:
+        """Indicates that a given choice value is a default.
+
+        Args:
+            value (Any): Value to check.
+
+        Returns:
+            bool: Indicator that the choice value is a default.
+
+        Examples:
+
+            .. doctest::
+
+                >>> from hemlock.questions.choice_base import ChoiceQuestion
+                >>> question = ChoiceQuestion(choices=["Yes", "No"], default="Yes")
+                >>> question.is_default("Yes")
+                True
+                >>> question.is_default("No")
+                False
+
+            Use a ``list`` to indicate that there are multiple default values.
+
+            .. doctest::
+
+                >>> from hemlock.questions.choice_base import ChoiceQuestion
+                >>> question = ChoiceQuestion(choices=["Red", "Green", "Blue"], multiple=True, default=["Red", "Green"])
+                >>> question.is_default("Red")
+                True
+                >>> question.is_default("Green")
+                True
+                >>> question.is_default("Blue")
+                False
+        """
+        default = self.get_default()
+
+        if default is None:
+            return False
+
+        if is_instance(default, (list, set)):
+            return value in default
+
+        return value == default
+
+    def record_response(self) -> None:
+        """Record the user's raw response.
+
+        The raw response is a set of choice values.
+        """
+        # Note: jinja template loop indices start at 1, so we need to subtract 1 for 0 indexing
+        self.raw_response = {
+            self.choices[int(i) - 1]["value"] for i in request.form.getlist(self.hash)
+        }
+
+    def record_data(self) -> None:
+        """Record data based on the user's response."""
+        if self.multiple:
+            self.data = {
+                choice["value"]: int(choice["value"] in self.raw_response)
+                for choice in self.choices
+            }
+            return
+
+        return super().record_data()
+
+    def pack_data(self) -> DataFrame:
+        """Pack the data for insertion into a data frame."""
+        dataframe = super().pack_data()
+        if self.variable is None or not self.record_choice_indices:
+            return dataframe
+
+        choice_indices = {}
+        for i, choice in enumerate(self.choices):
+            choice_indices[f"{self.variable}_{choice['value']}_index"] = i
+        dataframe.add_data(choice_indices, fill_rows=True)
+        dataframe.pad()
+        return dataframe
+
+    def make_raw_test_response(self, response: Any) -> List[Any]:
+        """Create a raw test response from a given test response.
+
+        Args:
+            response (Any): Test response. Must be either a choice value or a set of
+                choice values.
+
+        Returns:
+            List[Any]: List of indices of given choice values.
+        """
+        if response is None:
+            return []
+
+        if not is_instance(response, (list, set)):
+            response = {response}
+
+        # check that test responses are valid choices
+        if invalid_responses := set(response) - set(
+            choice["value"] for choice in self.choices
+        ):
+            raise ValueError(
+                f"Test user chose invalid choices {invalid_responses} for\n{self}."
+            )
+
+        # Note: jinja template loop indices start at 1, so we need to add 1 for 1 indexing
+        return [
+            str(i + 1)
+            for i, choice in enumerate(self.choices)
+            if choice["value"] in response
+        ]
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/input.py` & `hemlock-survey-1.0.1/src/hemlock/questions/input.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-"""Input.
-"""
-from __future__ import annotations
-
-import copy
-from datetime import datetime
-
-from typing import Any, Mapping
-
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy_mutable.html import HTMLAttrType
-from sqlalchemy_mutable.utils import is_instance
-
-from ..app import db
-from ..functional.test_response import datetime_input_types, random_input
-from .base import Question
-
-TEXT_INPUT_TYPE = "text"
-NUMBER_INPUT_TYPE = "number"
-
-
-class Input(Question):
-    """Input.
-
-    An input question allows users to enter a free text response.
-
-    Subclasses :class:`hemlock.questions.base.Question`.
-
-    Args:
-        *args (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
-        input_tag (Mapping[str, HTMLAttrType], optional): Additional attributes of the
-            HTML input tag. Defaults to None.
-        **kwargs (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
-
-    Examples:
-        The most common use of the ``input_tag`` attribute is for setting the input
-        type. For example, let's require users to enter a number.
-
-        .. doctest::
-
-            >>> from hemlock.questions import Input
-            >>> question = Input(input_tag={"type": "number"})
-            >>> question.input_tag["type"]
-            'number'
-
-        Let's require users to enter a number between 0 and 10.
-
-        .. doctest::
-
-            >>> from hemlock.questions import Input
-            >>> question = Input(input_tag={"type": "number", "min": 0, "max": 10})
-            >>> question.input_tag["min"], question.input_tag["max"]
-            (0, 10)
-
-        You can also require users to enter a certain input length.
-
-        .. doctest::
-
-            >>> from hemlock.questions import Input
-            >>> question = Input(input_tag={"minlength": 5, "maxlength": 10})
-            >>> question.input_tag["minlength"], question.input_tag["maxlength"]
-            (5, 10)
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "input"}
-
-    defaults = copy.deepcopy(Question.defaults)
-    defaults["template"] = "hemlock/input.html"  # type: ignore
-    defaults["html_settings"]["input"] = {"type": TEXT_INPUT_TYPE, "class": ["form-control"]}  # type: ignore
-    defaults["test_response"] = random_input
-
-    @property
-    def input_tag(self) -> HTMLAttrType:
-        """Attributes of the HTML input tag.
-
-        Returns:
-            HTMLAttrType: HTML attributes.
-        """
-        return self.html_settings["input"]
-
-    @hybrid_property
-    def response(self) -> Any:
-        """Converts the raw response to the appropriate type based on the input type."""
-        if self.raw_response in ("", None):
-            return None
-
-        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
-
-        if input_type == NUMBER_INPUT_TYPE:
-            return float(self.raw_response)
-
-        if input_type in datetime_input_types:
-            _, datetime_format = datetime_input_types[input_type]
-            return datetime.strptime(self.raw_response.get_object(), datetime_format)
-
-        return str(self.raw_response)
-
-    def __init__(
-        self, *args: Any, input_tag: Mapping[str, HTMLAttrType] = None, **kwargs: Any
-    ):
-        super().__init__(*args, **kwargs)
-        if input_tag is not None:
-            self.input_tag.update_attrs(input_tag)
-
-    def set_is_valid(self, is_valid: bool = None) -> None:
-        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
-
-        Additionally adds appropriate validation classes to the input tag.
-        """
-        return_value = super().set_is_valid(is_valid)
-        self._add_or_remove_class("input", "is-valid", is_valid is True)
-        self._add_or_remove_class("input", "is-invalid", is_valid is False)
-        return return_value
-
-    def run_validate_functions(self) -> bool:
-        """See :meth:`hemlock.questions.base.Question.run_validate_functions`.
-
-        Additionally, this method validates that the user's response matches the input
-        type.
-        """
-        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
-
-        # tests if the raw response can be converted to the expected type
-        try:
-            self.response
-        except ValueError:
-            if input_type == NUMBER_INPUT_TYPE:
-                self.feedback = "Please enter a number."
-            elif input_type in datetime_input_types:
-                html_format, datetime_format = datetime_input_types[input_type]
-                self.feedback = f"Please use the format {html_format}. For example, right now it is {datetime.utcnow().strftime(datetime_format)}."
-            else:
-                self.feedback = "Please enter the correct type of response."
-
-            self.set_is_valid(False)
-            return False
-
-        return super().run_validate_functions()
-
-    def make_raw_test_response(self, response: Any) -> str:
-        """Make a raw test response from the given response.
-
-        Args:
-            response (Any): Given response.
-
-        Raises:
-            ValueError: If the input is a number, the response must be convertible to
-                float.
-            ValueError: If the input is a date or time, the response must be in the
-                correct datetime format.
-
-        Returns:
-            str: Raw response
-        """
-        if response is None:
-            return ""
-
-        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
-
-        # make sure the raw response is in the expected format
-        if input_type == NUMBER_INPUT_TYPE:
-            try:
-                float_response = float(response)
-            except ValueError:
-                raise ValueError(
-                    f"Response {repr(response)} to input {self} cannot be converted to a float."
-                )
-            # make sure raw response is in the correct value range
-            if (
-                min_value := self.input_tag.get("min")
-            ) is not None and float_response < float(min_value):
-                raise ValueError(f"Reponse {response} is less than min {min_value}.")
-            if (
-                max_value := self.input_tag.get("max")
-            ) is not None and float_response > float(max_value):
-                raise ValueError(f"Response {response} is greater than max {max_value}")
-            return str(response)
-
-        if input_type in datetime_input_types:
-            # raw response can either be a string in HTML format or a datetime object
-            html_format, datetime_format = datetime_input_types[input_type]
-            if isinstance(response, datetime):
-                return response.strftime(datetime_format)
-
-            try:
-                datetime.strptime(response, datetime_format)
-            except ValueError:
-                raise ValueError(
-                    f"Response {repr(response)} to input {self}"
-                    f" does not match format {html_format}."
-                    " For example, right now it is"
-                    f" {datetime.utcnow().strftime(datetime_format)}."
-                )
-            return response
-
-        if input_type == TEXT_INPUT_TYPE and not is_instance(response, str):
-            raise ValueError(
-                f"Error on input {self}"
-                f"\nThis input accepts any text but the test response was {response} of"
-                f" type {type(response)}. A common cause of this error is that you want"
-                " users to enter a number but didn't require the input type to be a"
-                " number. You can do this with:"
-                '\n>>> Input(input_tag={"type": "number"})'
-            )
-
-        return str(response)
+"""Input.
+"""
+from __future__ import annotations
+
+import copy
+from datetime import datetime
+
+from typing import Any, Mapping
+
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy_mutable.html import HTMLAttrType
+from sqlalchemy_mutable.utils import is_instance
+
+from ..app import db
+from ..functional.test_response import datetime_input_types, random_input
+from .base import Question
+
+TEXT_INPUT_TYPE = "text"
+NUMBER_INPUT_TYPE = "number"
+
+
+class Input(Question):
+    """Input.
+
+    An input question allows users to enter a free text response.
+
+    Subclasses :class:`hemlock.questions.base.Question`.
+
+    Args:
+        *args (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
+        input_tag (Mapping[str, HTMLAttrType], optional): Additional attributes of the
+            HTML input tag. Defaults to None.
+        **kwargs (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
+
+    Examples:
+        The most common use of the ``input_tag`` attribute is for setting the input
+        type. For example, let's require users to enter a number.
+
+        .. doctest::
+
+            >>> from hemlock.questions import Input
+            >>> question = Input(input_tag={"type": "number"})
+            >>> question.input_tag["type"]
+            'number'
+
+        Let's require users to enter a number between 0 and 10.
+
+        .. doctest::
+
+            >>> from hemlock.questions import Input
+            >>> question = Input(input_tag={"type": "number", "min": 0, "max": 10})
+            >>> question.input_tag["min"], question.input_tag["max"]
+            (0, 10)
+
+        You can also require users to enter a certain input length.
+
+        .. doctest::
+
+            >>> from hemlock.questions import Input
+            >>> question = Input(input_tag={"minlength": 5, "maxlength": 10})
+            >>> question.input_tag["minlength"], question.input_tag["maxlength"]
+            (5, 10)
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "input"}
+
+    defaults = copy.deepcopy(Question.defaults)
+    defaults["template"] = "hemlock/input.html"  # type: ignore
+    defaults["html_settings"]["input"] = {"type": TEXT_INPUT_TYPE, "class": ["form-control"]}  # type: ignore
+    defaults["test_response"] = random_input
+
+    @property
+    def input_tag(self) -> HTMLAttrType:
+        """Attributes of the HTML input tag.
+
+        Returns:
+            HTMLAttrType: HTML attributes.
+        """
+        return self.html_settings["input"]
+
+    @hybrid_property
+    def response(self) -> Any:
+        """Converts the raw response to the appropriate type based on the input type."""
+        if self.raw_response in ("", None):
+            return None
+
+        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
+
+        if input_type == NUMBER_INPUT_TYPE:
+            return float(self.raw_response)
+
+        if input_type in datetime_input_types:
+            _, datetime_format = datetime_input_types[input_type]
+            return datetime.strptime(self.raw_response.get_object(), datetime_format)
+
+        return str(self.raw_response)
+
+    def __init__(
+        self, *args: Any, input_tag: Mapping[str, HTMLAttrType] = None, **kwargs: Any
+    ):
+        super().__init__(*args, **kwargs)
+        if input_tag is not None:
+            self.input_tag.update_attrs(input_tag)
+
+    def set_is_valid(self, is_valid: bool = None) -> None:
+        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
+
+        Additionally adds appropriate validation classes to the input tag.
+        """
+        return_value = super().set_is_valid(is_valid)
+        self._add_or_remove_class("input", "is-valid", is_valid is True)
+        self._add_or_remove_class("input", "is-invalid", is_valid is False)
+        return return_value
+
+    def run_validate_functions(self) -> bool:
+        """See :meth:`hemlock.questions.base.Question.run_validate_functions`.
+
+        Additionally, this method validates that the user's response matches the input
+        type.
+        """
+        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
+
+        # tests if the raw response can be converted to the expected type
+        try:
+            self.response
+        except ValueError:
+            if input_type == NUMBER_INPUT_TYPE:
+                self.feedback = "Please enter a number."
+            elif input_type in datetime_input_types:
+                html_format, datetime_format = datetime_input_types[input_type]
+                self.feedback = f"Please use the format {html_format}. For example, right now it is {datetime.utcnow().strftime(datetime_format)}."
+            else:
+                self.feedback = "Please enter the correct type of response."
+
+            self.set_is_valid(False)
+            return False
+
+        return super().run_validate_functions()
+
+    def make_raw_test_response(self, response: Any) -> str:
+        """Make a raw test response from the given response.
+
+        Args:
+            response (Any): Given response.
+
+        Raises:
+            ValueError: If the input is a number, the response must be convertible to
+                float.
+            ValueError: If the input is a date or time, the response must be in the
+                correct datetime format.
+
+        Returns:
+            str: Raw response
+        """
+        if response is None:
+            return ""
+
+        input_type = self.input_tag.get("type", TEXT_INPUT_TYPE)
+
+        # make sure the raw response is in the expected format
+        if input_type == NUMBER_INPUT_TYPE:
+            try:
+                float_response = float(response)
+            except ValueError:
+                raise ValueError(
+                    f"Response {repr(response)} to input {self} cannot be converted to a float."
+                )
+            # make sure raw response is in the correct value range
+            if (
+                min_value := self.input_tag.get("min")
+            ) is not None and float_response < float(min_value):
+                raise ValueError(f"Reponse {response} is less than min {min_value}.")
+            if (
+                max_value := self.input_tag.get("max")
+            ) is not None and float_response > float(max_value):
+                raise ValueError(f"Response {response} is greater than max {max_value}")
+            return str(response)
+
+        if input_type in datetime_input_types:
+            # raw response can either be a string in HTML format or a datetime object
+            html_format, datetime_format = datetime_input_types[input_type]
+            if isinstance(response, datetime):
+                return response.strftime(datetime_format)
+
+            try:
+                datetime.strptime(response, datetime_format)
+            except ValueError:
+                raise ValueError(
+                    f"Response {repr(response)} to input {self}"
+                    f" does not match format {html_format}."
+                    " For example, right now it is"
+                    f" {datetime.utcnow().strftime(datetime_format)}."
+                )
+            return response
+
+        if input_type == TEXT_INPUT_TYPE and not is_instance(response, str):
+            raise ValueError(
+                f"Error on input {self}"
+                f"\nThis input accepts any text but the test response was {response} of"
+                f" type {type(response)}. A common cause of this error is that you want"
+                " users to enter a number but didn't require the input type to be a"
+                " number. You can do this with:"
+                '\n>>> Input(input_tag={"type": "number"})'
+            )
+
+        return str(response)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/label.py` & `hemlock-survey-1.0.1/src/hemlock/questions/label.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""Label.
-"""
-from __future__ import annotations
-
-import copy
-
-from flask import render_template, request
-
-from ..app import db
-from ..utils.format import convert_markdown
-from .base import Question
-
-
-class Label(Question):
-    """A label question contains only text and does not permit a user response.
-
-    Subclasses :class:`hemlock.questions.base.Question`.
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "label"}
-
-    defaults = copy.deepcopy(Question.defaults)
-    defaults["template"] = "hemlock/label.html"  # type: ignore
-    # form-label adds a margin after the text, which we don't want unless there's a
-    # question below to respond to
-    defaults["html_settings"]["label"]["class"].remove("form-label")  # type: ignore
-
-    def render(self) -> str:  # pylint disable=missing-function-docstring
-        # renders the label, stripping the last <p> tag from the label text for a
-        # cleaner look
-        return render_template(
-            self.template,
-            question=self,
-            label=None
-            if self.label is None
-            else convert_markdown(self.label, strip_last_paragraph=True),
-        )
-
-    def make_raw_test_response(
-        self, response: str = None
-    ) -> str:  # pylint disable=missing-function-docstring
-        # test users cannot respond to a Label
-        if response not in (None, ""):
-            raise ValueError(f"{self} does not take a response; got {response}")
-        return super().make_raw_test_response(response)
+"""Label.
+"""
+from __future__ import annotations
+
+import copy
+
+from flask import render_template, request
+
+from ..app import db
+from ..utils.format import convert_markdown
+from .base import Question
+
+
+class Label(Question):
+    """A label question contains only text and does not permit a user response.
+
+    Subclasses :class:`hemlock.questions.base.Question`.
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "label"}
+
+    defaults = copy.deepcopy(Question.defaults)
+    defaults["template"] = "hemlock/label.html"  # type: ignore
+    # form-label adds a margin after the text, which we don't want unless there's a
+    # question below to respond to
+    defaults["html_settings"]["label"]["class"].remove("form-label")  # type: ignore
+
+    def render(self) -> str:  # pylint disable=missing-function-docstring
+        # renders the label, stripping the last <p> tag from the label text for a
+        # cleaner look
+        return render_template(
+            self.template,
+            question=self,
+            label=None
+            if self.label is None
+            else convert_markdown(self.label, strip_last_paragraph=True),
+        )
+
+    def make_raw_test_response(
+        self, response: str = None
+    ) -> str:  # pylint disable=missing-function-docstring
+        # test users cannot respond to a Label
+        if response not in (None, ""):
+            raise ValueError(f"{self} does not take a response; got {response}")
+        return super().make_raw_test_response(response)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/select.py` & `hemlock-survey-1.0.1/src/hemlock/questions/select.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""Select.
-"""
-from __future__ import annotations
-
-import copy
-
-from sqlalchemy_mutable.html import HTMLAttrType
-
-from ..app import db
-from .choice_base import ChoiceQuestion
-
-
-class Select(ChoiceQuestion):
-    """Select.
-
-    A select question allows users to select one or more choices using a dropdown menu.
-
-    Subclasses :class:`hemlock.questions.choice_base.ChoiceQuestion`.
-
-    Attributes:
-        select_tag (HTMLAttrsType): Attributes of the HTML select tag.
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "select"}
-
-    defaults = copy.deepcopy(ChoiceQuestion.defaults)
-    defaults["template"] = "hemlock/select.html"
-    defaults["html_settings"]["select"] = {"class": ["form-select"]}
-
-    @property
-    def select_tag(self) -> HTMLAttrType:
-        return self.html_settings["select"]
-
-    def set_is_valid(self, is_valid: bool = None) -> None:
-        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
-
-        Additionally adds appropriate validation classes to the select tag.
-        """
-        return_value = super().set_is_valid(is_valid)
-        self._add_or_remove_class("select", "is-valid", is_valid is True)
-        self._add_or_remove_class("select", "is-invalid", is_valid is False)
-        return return_value
+"""Select.
+"""
+from __future__ import annotations
+
+import copy
+
+from sqlalchemy_mutable.html import HTMLAttrType
+
+from ..app import db
+from .choice_base import ChoiceQuestion
+
+
+class Select(ChoiceQuestion):
+    """Select.
+
+    A select question allows users to select one or more choices using a dropdown menu.
+
+    Subclasses :class:`hemlock.questions.choice_base.ChoiceQuestion`.
+
+    Attributes:
+        select_tag (HTMLAttrsType): Attributes of the HTML select tag.
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "select"}
+
+    defaults = copy.deepcopy(ChoiceQuestion.defaults)
+    defaults["template"] = "hemlock/select.html"
+    defaults["html_settings"]["select"] = {"class": ["form-select"]}
+
+    @property
+    def select_tag(self) -> HTMLAttrType:
+        return self.html_settings["select"]
+
+    def set_is_valid(self, is_valid: bool = None) -> None:
+        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
+
+        Additionally adds appropriate validation classes to the select tag.
+        """
+        return_value = super().set_is_valid(is_valid)
+        self._add_or_remove_class("select", "is-valid", is_valid is True)
+        self._add_or_remove_class("select", "is-invalid", is_valid is False)
+        return return_value
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/questions/textarea.py` & `hemlock-survey-1.0.1/src/hemlock/questions/textarea.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-"""Textarea.
-"""
-from __future__ import annotations
-
-import copy
-from typing import Any, Mapping
-
-import numpy as np
-from flask import render_template
-from sqlalchemy_mutable.html import HTMLAttrType
-
-from ..app import db
-from ..functional.test_response import random_text
-from ..functional.validate import response_in_range
-from .base import Question
-
-
-class Textarea(Question):
-    """Textarea.
-
-    An textarea question allows users to enter a long free text response.
-
-    Subclasses :class:`hemlock.questions.base.Question`.
-
-    Args:
-        *args (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
-        textarea_tag (Mapping[str, HTMLAttrType], optional): Additional attributes of
-            the HTML textarea tag. Defaults to None.
-        **kwargs (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
-
-    Attributes:
-        textarea_tag (HTMLAttrsType): Attributes of the HTML textarea tag.
-
-    Examples:
-        In addition to requiring a certain input length, we can require a certain number
-        of words.
-
-        .. doctest::
-
-            >>> from hemlock import create_test_app
-            >>> from hemlock.questions import Textarea
-            >>> app = create_test_app()
-            >>> question = Textarea(textarea_tag={"minwords": 5, "maxwords": 10})
-            >>> question.textarea_tag["minwords"], question.textarea_tag["maxwords"]
-            (5, 10)
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "textarea"}
-
-    defaults = copy.deepcopy(Question.defaults)
-    defaults["template"] = "hemlock/textarea.html"  # type: ignore
-    defaults["test_response"] = random_text
-    defaults["html_settings"]["textarea"] = {
-        "class": ["form-control w-100"],
-        "style": {"height": "100px"},
-    }
-
-    @property
-    def textarea_tag(self):
-        return self.html_settings["textarea"]
-
-    def __init__(
-        self,
-        *args: Any,
-        textarea_tag: Mapping[str, HTMLAttrType] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(*args, **kwargs)
-        self.html_settings["js"].append(
-            render_template("hemlock/textarea.js", question=self)
-        )
-        if textarea_tag is not None:
-            self.textarea_tag.update_attrs(textarea_tag)
-
-    def set_is_valid(self, is_valid: bool = None) -> None:
-        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
-
-        Additionally adds appropriate validation classes to the textarea tag.
-        """
-        return_value = super().set_is_valid(is_valid)
-        self._add_or_remove_class("textarea", "is-valid", is_valid is True)
-        self._add_or_remove_class("textarea", "is-invalid", is_valid is False)
-        return return_value
-
-    def run_validate_functions(self) -> bool:
-        """See :meth:`hemlock.questions.base.Question.run_validate_functions`.
-
-        Additionally, this method validates that the user's response has the correct
-        word count.
-        """
-        if self.response is not None:
-            minwords = self.textarea_tag.get("minwords")
-            if minwords is None:
-                minwords = 0
-
-            maxwords = self.textarea_tag.get("maxwords")
-            if maxwords is None:
-                maxwords = np.inf
-
-            if (
-                response_in_range(self, minwords, maxwords, how="word count")
-                is not None
-            ):
-                if minwords == 0:
-                    self.feedback = f"Please shorten your response to {maxwords} words."
-                elif maxwords == np.inf:
-                    self.feedback = f"Please write at least {minwords} words."
-                else:
-                    # both minwords and maxwords are defined
-                    self.feedback = (
-                        f"Please write between {minwords} and {maxwords} words."
-                    )
-
-                self.set_is_valid(False)
-                return False
-
-        return super().run_validate_functions()
+"""Textarea.
+"""
+from __future__ import annotations
+
+import copy
+from typing import Any, Mapping
+
+import numpy as np
+from flask import render_template
+from sqlalchemy_mutable.html import HTMLAttrType
+
+from ..app import db
+from ..functional.test_response import random_text
+from ..functional.validate import response_in_range
+from .base import Question
+
+
+class Textarea(Question):
+    """Textarea.
+
+    An textarea question allows users to enter a long free text response.
+
+    Subclasses :class:`hemlock.questions.base.Question`.
+
+    Args:
+        *args (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
+        textarea_tag (Mapping[str, HTMLAttrType], optional): Additional attributes of
+            the HTML textarea tag. Defaults to None.
+        **kwargs (Any): Passed to :class:`hemlock.questions.base.Question` constructor.
+
+    Attributes:
+        textarea_tag (HTMLAttrsType): Attributes of the HTML textarea tag.
+
+    Examples:
+        In addition to requiring a certain input length, we can require a certain number
+        of words.
+
+        .. doctest::
+
+            >>> from hemlock import create_test_app
+            >>> from hemlock.questions import Textarea
+            >>> app = create_test_app()
+            >>> question = Textarea(textarea_tag={"minwords": 5, "maxwords": 10})
+            >>> question.textarea_tag["minwords"], question.textarea_tag["maxwords"]
+            (5, 10)
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("question.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "textarea"}
+
+    defaults = copy.deepcopy(Question.defaults)
+    defaults["template"] = "hemlock/textarea.html"  # type: ignore
+    defaults["test_response"] = random_text
+    defaults["html_settings"]["textarea"] = {
+        "class": ["form-control w-100"],
+        "style": {"height": "100px"},
+    }
+
+    @property
+    def textarea_tag(self):
+        return self.html_settings["textarea"]
+
+    def __init__(
+        self,
+        *args: Any,
+        textarea_tag: Mapping[str, HTMLAttrType] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+        self.html_settings["js"].append(
+            render_template("hemlock/textarea.js", question=self)
+        )
+        if textarea_tag is not None:
+            self.textarea_tag.update_attrs(textarea_tag)
+
+    def set_is_valid(self, is_valid: bool = None) -> None:
+        """See :meth:`hemlock.questions.base.Question.set_is_valid`.
+
+        Additionally adds appropriate validation classes to the textarea tag.
+        """
+        return_value = super().set_is_valid(is_valid)
+        self._add_or_remove_class("textarea", "is-valid", is_valid is True)
+        self._add_or_remove_class("textarea", "is-invalid", is_valid is False)
+        return return_value
+
+    def run_validate_functions(self) -> bool:
+        """See :meth:`hemlock.questions.base.Question.run_validate_functions`.
+
+        Additionally, this method validates that the user's response has the correct
+        word count.
+        """
+        if self.response is not None:
+            minwords = self.textarea_tag.get("minwords")
+            if minwords is None:
+                minwords = 0
+
+            maxwords = self.textarea_tag.get("maxwords")
+            if maxwords is None:
+                maxwords = np.inf
+
+            if (
+                response_in_range(self, minwords, maxwords, how="word count")
+                is not None
+            ):
+                if minwords == 0:
+                    self.feedback = f"Please shorten your response to {maxwords} words."
+                elif maxwords == np.inf:
+                    self.feedback = f"Please write at least {minwords} words."
+                else:
+                    # both minwords and maxwords are defined
+                    self.feedback = (
+                        f"Please write between {minwords} and {maxwords} words."
+                    )
+
+                self.set_is_valid(False)
+                return False
+
+        return super().run_validate_functions()
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/check.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/check.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{% extends "hemlock/utils/card.html" %}
-
-{% block content %}
-{% if question.multiple %}
-    {% set type = "checkbox" %}
-{% else %}
-    {% set type = "radio" %}
-{% endif %}
-
-{% for choice in question.choices %}
-    {% set index = loop.index | string() %}
-    {% set id = question.hash + index %}
-
-    {% if question.is_default(choice["value"]) %}
-        {% set checked = " checked" %}
-    {% else %}
-        {% set checked = "" %}
-    {% endif %}
-
-    {% if choice.get("disabled") %}
-        {% set disabled = " disabled" %}
-    {% else %}
-        {% set disabled = "" %}
-    {% endif %}
-
-    <div {{ question.html_settings["div"].get_attrs() | safe }}>
-        <input id="{{ id }}" name="{{ question.hash }}" class="form-check-input" type="{{ type }}" value="{{ loop.index }}"{{ disabled }}{{ checked }}>
-        <label class="form-check-label custom-check-label w-100" for="{{ id }}">
-            {{ choice["label"] | safe }}
-        </label>
-    </div>
-{% endfor %}
+{% extends "hemlock/utils/card.html" %}
+
+{% block content %}
+{% if question.multiple %}
+    {% set type = "checkbox" %}
+{% else %}
+    {% set type = "radio" %}
+{% endif %}
+
+{% for choice in question.choices %}
+    {% set index = loop.index | string() %}
+    {% set id = question.hash + index %}
+
+    {% if question.is_default(choice["value"]) %}
+        {% set checked = " checked" %}
+    {% else %}
+        {% set checked = "" %}
+    {% endif %}
+
+    {% if choice.get("disabled") %}
+        {% set disabled = " disabled" %}
+    {% else %}
+        {% set disabled = "" %}
+    {% endif %}
+
+    <div {{ question.html_settings["div"].get_attrs() | safe }}>
+        <input id="{{ id }}" name="{{ question.hash }}" class="form-check-input" type="{{ type }}" value="{{ loop.index }}"{{ disabled }}{{ checked }}>
+        <label class="form-check-label custom-check-label w-100" for="{{ id }}">
+            {{ choice["label"] | safe }}
+        </label>
+    </div>
+{% endfor %}
 {% endblock %}
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/input.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/input.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-{% extends "hemlock/utils/input_group.html" %}
-
-{% macro input(add_placeholder) %}
-    {% set default = question.get_default(alt_value="") %}
-
-    {% if add_placeholder is sameas true %}
-        {% set placeholder = " placeholder='placeholder'" | safe %}
-    {% else %}
-        {% set placeholder = "" %}
-    {% endif %}
-
-    <input id="{{ question.hash }}" name="{{ question.hash }}" {{ question.input_tag.get_attrs() | safe }} value="{{ default }}"{{ placeholder }}>
-{% endmacro %}
-
-{% block content %}
-    {% if question.floating_label is not none %}
-        {{ form_floating(input(true)) }}
-    {% else %}
-        {{ input(false) }}
-    {% endif %}
+{% extends "hemlock/utils/input_group.html" %}
+
+{% macro input(add_placeholder) %}
+    {% set default = question.get_default(alt_value="") %}
+
+    {% if add_placeholder is sameas true %}
+        {% set placeholder = " placeholder='placeholder'" | safe %}
+    {% else %}
+        {% set placeholder = "" %}
+    {% endif %}
+
+    <input id="{{ question.hash }}" name="{{ question.hash }}" {{ question.input_tag.get_attrs() | safe }} value="{{ default }}"{{ placeholder }}>
+{% endmacro %}
+
+{% block content %}
+    {% if question.floating_label is not none %}
+        {{ form_floating(input(true)) }}
+    {% else %}
+        {{ input(false) }}
+    {% endif %}
 {% endblock %}
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/page.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/page.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-<!DOCTYPE html>
-
-<html lang="en">
-    <head>
-        {% block head %}
-        <meta charset="utf-8">
-        <meta name="viewport" content="width=device-width, initial-scale=1.0">
-        <link rel="shortcut icon" href="https://dsbowen.gitlab.io/hemlock/_static/favicon.png">
-        {{ page.html_settings.get_css() | safe}}
-        {% for question in page.questions %}
-            {{ question.html_settings.get_css() | safe }}
-        {% endfor %}
-        <style>
-            input[type="checkbox"]:hover + label {
-                background-color: rgb(224,224,224);
-            }
-            input[type="radio"]:hover + label {
-                background-color: rgb(224,224,224);
-            }
-            input:checked + label {
-                background-color: rgb(206, 206, 206);
-            }
-            input[type="checkbox"]:checked:hover + label {
-                background-color: gainsboro;
-            }
-            .custom-check-label {
-                padding-left: 3px;
-                padding-right: 3px;
-                border-radius: 3px;
-                background-clip: padding-box;
-            }
-            .loading {
-                display: none;
-                position: fixed;
-                align-items: center;
-                justify-content: center;
-                background: rgba(0, 0, 0, .2);
-                height: 100vh;
-                width: 100%;
-                top: 0;
-                left: 0;
-                z-index: 9999;
-            }
-            /* @media (prefers-color-scheme: dark) {
-                body {
-                    background-color: black;
-                    color: white;
-                }
-                .card {
-                    background-color: #4A4A4A;
-                }
-            } */
-        </style>
-        {% if for_notebook_display is defined and for_notebook_display is sameas true %}
-        <style>
-            body {
-                background-color: inherit;
-                color: inherit;
-            }
-        </style>
-        {% endif %}
-        {% endblock %}
-    </head>
-    <body>
-        <div class="loading">
-            <div class="spinner-border" role="status">
-                <span class="visually-hidden">Loading...</span>
-            </div>
-        </div>
-
-        {% block body %}
-        {% if for_notebook_display is not defined or for_notebook_display is sameas false %}
-            {% block navbar %}
-                {% if page.navbar is not none %}
-                    {% set navbar = page.navbar %}
-                    {% include "hemlock/utils/navbar.html" %}
-                {% endif %}
-            {% endblock %}
-        {% endif %}
-
-        <div {{ page.html_settings["div"].get_attrs() | safe }}>
-            <form method="POST" class="w-100" style="margin-top:80px;" enctype="multipart/form-data">
-                <input id="page-hash" name="page-hash" type="hidden" value="{{ page.hash }}">
-            {% block form %}                
-                {% for question in page.questions %}
-                    {{ question.render() | safe}}
-                {% endfor %}
-    
-                {% if page.forward is not none and not page.is_last_page %}
-                <button {{ page.html_settings["forward-button"].get_attrs() | safe }}{% if for_notebook_display is sameas true %} disabled{% endif %}>
-                    {{ page.forward }}
-                </button>
-                {% endif %}
-                {% if page.back is not none and not page.is_first_page %}
-                <button {{ page.html_settings["back-button"].get_attrs() | safe }}{% if for_notebook_display is sameas true %} disabled{% endif %}>
-                    {{ page.back }}
-                </button>
-                {% endif %}
-                <p style="clear:both;"><br></p>
-    
-                {% if for_notebook_display is sameas false %}
-                    {{ page.defaults["banner"] | safe }}
-                {% endif %}
-            {% endblock %}
-            </form>
-        </div>
-
-        {{ page.html_settings.get_js() | safe }}
-        {% for question in page.questions %}
-            {{ question.html_settings.get_js() | safe }}
-        {% endfor %}
-        <script>
-            $(document).ready(function() {
-                var submitted_class = "submitted";
-                $("form").submit( function(e) {
-                    if ($(this).hasClass(submitted_class)) {
-                        e.preventDefault();
-                    }
-                    else {
-                        $(this).addClass(submitted_class);
-                        $(".loading").css("display", "flex");
-                        $("input").prop("readonly", true);
-                        $("select").prop("readonly", true);
-                        $("textarea").prop("readonly", true);
-                    }
-                });
-            })
-        </script>
-    {% endblock %}
-    </body>
+<!DOCTYPE html>
+
+<html lang="en">
+    <head>
+        {% block head %}
+        <meta charset="utf-8">
+        <meta name="viewport" content="width=device-width, initial-scale=1.0">
+        <link rel="shortcut icon" href="https://dsbowen.gitlab.io/hemlock/_static/favicon.png">
+        {{ page.html_settings.get_css() | safe}}
+        {% for question in page.questions %}
+            {{ question.html_settings.get_css() | safe }}
+        {% endfor %}
+        <style>
+            input[type="checkbox"]:hover + label {
+                background-color: rgb(224,224,224);
+            }
+            input[type="radio"]:hover + label {
+                background-color: rgb(224,224,224);
+            }
+            input:checked + label {
+                background-color: rgb(206, 206, 206);
+            }
+            input[type="checkbox"]:checked:hover + label {
+                background-color: gainsboro;
+            }
+            .custom-check-label {
+                padding-left: 3px;
+                padding-right: 3px;
+                border-radius: 3px;
+                background-clip: padding-box;
+            }
+            .loading {
+                display: none;
+                position: fixed;
+                align-items: center;
+                justify-content: center;
+                background: rgba(0, 0, 0, .2);
+                height: 100vh;
+                width: 100%;
+                top: 0;
+                left: 0;
+                z-index: 9999;
+            }
+            /* @media (prefers-color-scheme: dark) {
+                body {
+                    background-color: black;
+                    color: white;
+                }
+                .card {
+                    background-color: #4A4A4A;
+                }
+            } */
+        </style>
+        {% if for_notebook_display is defined and for_notebook_display is sameas true %}
+        <style>
+            body {
+                background-color: inherit;
+                color: inherit;
+            }
+        </style>
+        {% endif %}
+        {% endblock %}
+    </head>
+    <body>
+        <div class="loading">
+            <div class="spinner-border" role="status">
+                <span class="visually-hidden">Loading...</span>
+            </div>
+        </div>
+
+        {% block body %}
+        {% if for_notebook_display is not defined or for_notebook_display is sameas false %}
+            {% block navbar %}
+                {% if page.navbar is not none %}
+                    {% set navbar = page.navbar %}
+                    {% include "hemlock/utils/navbar.html" %}
+                {% endif %}
+            {% endblock %}
+        {% endif %}
+
+        <div {{ page.html_settings["div"].get_attrs() | safe }}>
+            <form method="POST" class="w-100" style="margin-top:80px;" enctype="multipart/form-data">
+                <input id="page-hash" name="page-hash" type="hidden" value="{{ page.hash }}">
+            {% block form %}                
+                {% for question in page.questions %}
+                    {{ question.render() | safe}}
+                {% endfor %}
+    
+                {% if page.forward is not none and not page.is_last_page %}
+                <button {{ page.html_settings["forward-button"].get_attrs() | safe }}{% if for_notebook_display is sameas true %} disabled{% endif %}>
+                    {{ page.forward }}
+                </button>
+                {% endif %}
+                {% if page.back is not none and not page.is_first_page %}
+                <button {{ page.html_settings["back-button"].get_attrs() | safe }}{% if for_notebook_display is sameas true %} disabled{% endif %}>
+                    {{ page.back }}
+                </button>
+                {% endif %}
+                <p style="clear:both;"><br></p>
+    
+                {% if for_notebook_display is sameas false %}
+                    {{ page.defaults["banner"] | safe }}
+                {% endif %}
+            {% endblock %}
+            </form>
+        </div>
+
+        {{ page.html_settings.get_js() | safe }}
+        {% for question in page.questions %}
+            {{ question.html_settings.get_js() | safe }}
+        {% endfor %}
+        <script>
+            $(document).ready(function() {
+                var submitted_class = "submitted";
+                $("form").submit( function(e) {
+                    if ($(this).hasClass(submitted_class)) {
+                        e.preventDefault();
+                    }
+                    else {
+                        $(this).addClass(submitted_class);
+                        $(".loading").css("display", "flex");
+                        $("input").prop("readonly", true);
+                        $("select").prop("readonly", true);
+                        $("textarea").prop("readonly", true);
+                    }
+                });
+            })
+        </script>
+    {% endblock %}
+    </body>
 </html>
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/select.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/select.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-{% extends "hemlock/utils/input_group.html" %}
-
-{% macro select() %}
-    {% if question.multiple %}
-        {% set multiple = " multiple" %}
-    {% else %}
-        {% set multiple = "" %}
-    {% endif %}
-
-    <select id="{{ question.hash }}" name="{{ question.hash }}" {{ question.select_tag.get_attrs() | safe }}{{ multiple }}>
-        {% for choice in question.choices %}
-            {% set index = loop.index | string() %}
-            {% set id = question.hash + index %}
-
-            {% if question.is_default(choice["value"]) %}
-                {% set selected = "selected" %}
-            {% else %}
-                {% set selected = "" %}
-            {% endif %}
-
-            <option id="{{ id }}" value="{{ loop.index }}"{{ selected }}>
-                {{ choice["label"] | safe }}
-            </option>
-        {% endfor %}
-    </select>
-{% endmacro %}
-
-{% block content %}
-    {% if question.floating_label is not none %}
-        {{ form_floating(select()) }}
-    {% else %}
-        {{ select() }}
-    {% endif %}
+{% extends "hemlock/utils/input_group.html" %}
+
+{% macro select() %}
+    {% if question.multiple %}
+        {% set multiple = " multiple" %}
+    {% else %}
+        {% set multiple = "" %}
+    {% endif %}
+
+    <select id="{{ question.hash }}" name="{{ question.hash }}" {{ question.select_tag.get_attrs() | safe }}{{ multiple }}>
+        {% for choice in question.choices %}
+            {% set index = loop.index | string() %}
+            {% set id = question.hash + index %}
+
+            {% if question.is_default(choice["value"]) %}
+                {% set selected = "selected" %}
+            {% else %}
+                {% set selected = "" %}
+            {% endif %}
+
+            <option id="{{ id }}" value="{{ loop.index }}"{{ selected }}>
+                {{ choice["label"] | safe }}
+            </option>
+        {% endfor %}
+    </select>
+{% endmacro %}
+
+{% block content %}
+    {% if question.floating_label is not none %}
+        {{ form_floating(select()) }}
+    {% else %}
+        {{ select() }}
+    {% endif %}
 {% endblock %}
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/textarea.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/textarea.html`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-{% extends "hemlock/utils/input_group.html" %}
-
-{% macro textarea(add_placeholder) %}
-    {% set default = question.get_default(alt_value="") %}
-
-    {% if add_placeholder is sameas true %}
-        {% set placeholder = " placeholder='placeholder'" | safe %}
-    {% else %}
-        {% set placeholder = "" %}
-    {% endif %}
-
-    <textarea id="{{ question.hash }}" name="{{ question.hash }}" {{ question.html_settings["textarea"].get_attrs() | safe }}{{ placeholder }}>{{ default }}</textarea>
-{% endmacro %}
-
-{% block card_body %}
-    {% include "hemlock/utils/label.html" %}
-    <div class="input-group">
-        {{ input_group_text(question.prepend) }}
-        {% if question.floating_label is not none %}
-            {{ form_floating(textarea(true)) }}
-        {% else %}
-            {{ textarea(false) }}
-        {% endif %}
-        {{ input_group_text(question.append) }}
-        <div id="{{ question.hash }}-characters-parent" class="form-text w-100" style="display:block;">
-            Characters: <span id="{{ question.hash }}-characters"></span>
-        </div>
-        <div id="{{ question.hash }}-words-parent" class="form-text w-100" style="display:block;">
-            Words: <span id="{{ question.hash }}-words"></span>
-        </div>
-        {% include "hemlock/utils/feedback.html" %}
-    </div>
-    {% include "hemlock/utils/form_text.html" %}
+{% extends "hemlock/utils/input_group.html" %}
+
+{% macro textarea(add_placeholder) %}
+    {% set default = question.get_default(alt_value="") %}
+
+    {% if add_placeholder is sameas true %}
+        {% set placeholder = " placeholder='placeholder'" | safe %}
+    {% else %}
+        {% set placeholder = "" %}
+    {% endif %}
+
+    <textarea id="{{ question.hash }}" name="{{ question.hash }}" {{ question.html_settings["textarea"].get_attrs() | safe }}{{ placeholder }}>{{ default }}</textarea>
+{% endmacro %}
+
+{% block card_body %}
+    {% include "hemlock/utils/label.html" %}
+    <div class="input-group">
+        {{ input_group_text(question.prepend) }}
+        {% if question.floating_label is not none %}
+            {{ form_floating(textarea(true)) }}
+        {% else %}
+            {{ textarea(false) }}
+        {% endif %}
+        {{ input_group_text(question.append) }}
+        <div id="{{ question.hash }}-characters-parent" class="form-text w-100" style="display:block;">
+            Characters: <span id="{{ question.hash }}-characters"></span>
+        </div>
+        <div id="{{ question.hash }}-words-parent" class="form-text w-100" style="display:block;">
+            Words: <span id="{{ question.hash }}-words"></span>
+        </div>
+        {% include "hemlock/utils/feedback.html" %}
+    </div>
+    {% include "hemlock/utils/form_text.html" %}
 {% endblock %}
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/textarea.js` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/textarea.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,58 @@
-$(document).ready(function() {
-    function updateCount(question) {
-        var response = question.val();
-
-        setText(
-            "{{ question.hash }}-characters",
-            response.length,
-            "minlength",
-            "maxlength"
-        );
-
-        if (response.length == 0) {
-            word_count = 0;
-        } else {
-            word_count = response.trim().split(/\w+/).length - 1;
-        }
-        setText("{{ question.hash }}-words", word_count, "minwords", "maxwords");
-    }
-
-    function setText(object_id, count, minattr_name, maxattr_name) {
-        var object = $("#" + object_id);
-        var parent = $("#" + object_id + "-parent");
-        var valid_count = true;
-        var text = count.toString();
-
-        // add feedback based on maximum allowable count
-        var maxattr = question.attr(maxattr_name);
-        if (typeof maxattr != "undefined" && maxattr != false) {
-            var text = text + " / " + maxattr;
-            if (count > 0 && count > parseInt(maxattr)) {
-                var valid_count = false;
-            }
-        }
-
-        // add feedback based on minimum allowable count
-        var minattr = question.attr(minattr_name);
-        if (typeof minattr != "undefined" && minattr != false) {
-            var text = text + " (min " + minattr + ")";
-            if (count > 0 && count < parseInt(minattr)) {
-                var valid_count = false;
-            }
-        }
-
-        object.text(text);
-        var invalid_class = "text-danger";
-        if (valid_count) {
-            parent.removeClass(invalid_class);
-        } else {
-            parent.addClass(invalid_class);
-        }
-    }
-
-    var question = $("#{{ question.hash }}");
-    updateCount(question);
-    question.on("input", function() {
-        updateCount($(this));
-    });
+$(document).ready(function() {
+    function updateCount(question) {
+        var response = question.val();
+
+        setText(
+            "{{ question.hash }}-characters",
+            response.length,
+            "minlength",
+            "maxlength"
+        );
+
+        if (response.length == 0) {
+            word_count = 0;
+        } else {
+            word_count = response.trim().split(/\w+/).length - 1;
+        }
+        setText("{{ question.hash }}-words", word_count, "minwords", "maxwords");
+    }
+
+    function setText(object_id, count, minattr_name, maxattr_name) {
+        var object = $("#" + object_id);
+        var parent = $("#" + object_id + "-parent");
+        var valid_count = true;
+        var text = count.toString();
+
+        // add feedback based on maximum allowable count
+        var maxattr = question.attr(maxattr_name);
+        if (typeof maxattr != "undefined" && maxattr != false) {
+            var text = text + " / " + maxattr;
+            if (count > 0 && count > parseInt(maxattr)) {
+                var valid_count = false;
+            }
+        }
+
+        // add feedback based on minimum allowable count
+        var minattr = question.attr(minattr_name);
+        if (typeof minattr != "undefined" && minattr != false) {
+            var text = text + " (min " + minattr + ")";
+            if (count > 0 && count < parseInt(minattr)) {
+                var valid_count = false;
+            }
+        }
+
+        object.text(text);
+        var invalid_class = "text-danger";
+        if (valid_count) {
+            parent.removeClass(invalid_class);
+        } else {
+            parent.addClass(invalid_class);
+        }
+    }
+
+    var question = $("#{{ question.hash }}");
+    updateCount(question);
+    question.on("input", function() {
+        updateCount($(this));
+    });
 });
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/input_group.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/input_group.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-{% extends "hemlock/utils/card.html" %}
-
-{% macro input_group_text(texts) %}
-    {% if texts is not none %}
-        {% for text in texts %}
-            <span class="input-group-text">{{ text }}</span>
-        {% endfor %}
-    {% endif %}
-{% endmacro %}
-
-{% macro form_floating(content) %}
-    <div class="form-floating flex-grow-1">
-        {{ content }}
-        <label for="{{ question.hash }}">
-            {{ question.floating_label | safe}}
-        </label>
-    </div>
-{% endmacro %}
-
-{% block card_body %}
-    {% include "hemlock/utils/label.html" %}
-    <div class="input-group">
-        {{ input_group_text(question.prepend) }}
-        {% block content %}{% endblock %}
-        {{ input_group_text(question.append) }}
-        {% include "hemlock/utils/feedback.html" %}
-    </div>
-    {% include "hemlock/utils/form_text.html" %}
+{% extends "hemlock/utils/card.html" %}
+
+{% macro input_group_text(texts) %}
+    {% if texts is not none %}
+        {% for text in texts %}
+            <span class="input-group-text">{{ text }}</span>
+        {% endfor %}
+    {% endif %}
+{% endmacro %}
+
+{% macro form_floating(content) %}
+    <div class="form-floating flex-grow-1">
+        {{ content }}
+        <label for="{{ question.hash }}">
+            {{ question.floating_label | safe}}
+        </label>
+    </div>
+{% endmacro %}
+
+{% block card_body %}
+    {% include "hemlock/utils/label.html" %}
+    <div class="input-group">
+        {{ input_group_text(question.prepend) }}
+        {% block content %}{% endblock %}
+        {{ input_group_text(question.append) }}
+        {% include "hemlock/utils/feedback.html" %}
+    </div>
+    {% include "hemlock/utils/form_text.html" %}
 {% endblock %}
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/templates/hemlock/utils/loading_page.html` & `hemlock-survey-1.0.1/src/hemlock/templates/hemlock/utils/loading_page.html`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-<!DOCTYPE html>
-
-<html lang="en">
-    <head>
-        <meta charset="utf-8">
-        <meta name="viewport" content="width=device-width, initial-scale=1.0">
-        {{ page.html_settings.get_css() | safe }}
-        <style>
-            .loading {
-                display: flex;
-                position: fixed;
-                align-items: center;
-                justify-content: center;
-                background: rgba(0, 0, 0, .2);
-                height: 100vh;
-                width: 100%;
-                top: 0;
-                left: 0;
-                z-index: 9999;
-            }
-        </style>
-    </head>
-    <body>
-        <div class="loading">
-            <div class="spinner-border" role="status">
-                <span class="visually-hidden">Loading...</span>
-            </div>
-        </div>
-        {{ page.html_settings.get_js() | safe }}
-        <script>
-            $(document).ready( function() {
-                setInterval(function() {
-                    console.log("Trying refresh");
-                    window.location.replace(window.location.href);
-                }, 2000);
-            });
-        </script>
-    </body>
+<!DOCTYPE html>
+
+<html lang="en">
+    <head>
+        <meta charset="utf-8">
+        <meta name="viewport" content="width=device-width, initial-scale=1.0">
+        {{ page.html_settings.get_css() | safe }}
+        <style>
+            .loading {
+                display: flex;
+                position: fixed;
+                align-items: center;
+                justify-content: center;
+                background: rgba(0, 0, 0, .2);
+                height: 100vh;
+                width: 100%;
+                top: 0;
+                left: 0;
+                z-index: 9999;
+            }
+        </style>
+    </head>
+    <body>
+        <div class="loading">
+            <div class="spinner-border" role="status">
+                <span class="visually-hidden">Loading...</span>
+            </div>
+        </div>
+        {{ page.html_settings.get_js() | safe }}
+        <script>
+            $(document).ready( function() {
+                setInterval(function() {
+                    console.log("Trying refresh");
+                    window.location.replace(window.location.href);
+                }, 2000);
+            });
+        </script>
+    </body>
 </html>
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/timer.py` & `hemlock-survey-1.0.1/src/hemlock/timer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-"""Timer.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-
-from sqlalchemy.ext.hybrid import hybrid_property
-
-from .app import db
-from .data import Data
-
-
-class Timer(Data):
-    """Timer.
-
-    Subclasses :class:`hemlock.data.Data`.
-
-    Attributes:
-        is_running (bool): Indicates that the timer is running.
-        start_time (datetime): The most recent time the timer was started.
-        total_seconds (float): The total number of seconds the timer has been running.
-
-    Examples:
-
-        .. code-block::
-
-            >>> import time
-            >>> from hemlock.timer import Timer
-            >>> timer = Timer("my_timer_variable")
-            >>> timer
-            <Timer my_timer_variable paused 0 seconds>
-            >>> timer.start()
-            >>> time.sleep(1)
-            >>> timer
-            <Timer my_timer_variable running 1.015078 seconds>
-            >>> timer.pause()
-            >>> timer
-            <Timer my_timer_variable paused 5.425622 seconds>
-            >>> timer.pack_data()
-            {'my_timer_variable': [5.425622]}
-    """
-
-    id = db.Column(db.Integer, db.ForeignKey("data.id"), primary_key=True)
-    __mapper_args__ = {"polymorphic_identity": "timer"}
-
-    _page_timer_id = db.Column(db.Integer, db.ForeignKey("page.id"))
-
-    is_running = db.Column(db.Boolean)
-    start_time = db.Column(db.DateTime)
-
-    @hybrid_property
-    def total_seconds(self) -> float:
-        """Get the total number of seconds the timer has been running.
-
-        Returns:
-            float: Total seconds.
-        """
-        if self.is_running:
-            return self.data + (datetime.utcnow() - self.start_time).total_seconds()
-        return self.data
-
-    @total_seconds.setter  # type: ignore
-    def total_seconds(self, total_seconds):
-        self.data = total_seconds
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.is_running = False
-        self.total_seconds = 0
-
-    def __repr__(self):
-        running = "running" if self.is_running else "paused"
-        return f"<{self.__class__.__qualname__} {self.variable} {running} {self.total_seconds} seconds>"
-
-    def start(self):
-        """Start the timer."""
-        if not self.is_running:
-            self.is_running = True
-            self.start_time = datetime.utcnow()
-
-    def pause(self):
-        """Pause the timer."""
-        if self.is_running:
-            self.data += (datetime.utcnow() - self.start_time).total_seconds()
-            self.is_running = False
+"""Timer.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+
+from sqlalchemy.ext.hybrid import hybrid_property
+
+from .app import db
+from .data import Data
+
+
+class Timer(Data):
+    """Timer.
+
+    Subclasses :class:`hemlock.data.Data`.
+
+    Attributes:
+        is_running (bool): Indicates that the timer is running.
+        start_time (datetime): The most recent time the timer was started.
+        total_seconds (float): The total number of seconds the timer has been running.
+
+    Examples:
+
+        .. code-block::
+
+            >>> import time
+            >>> from hemlock.timer import Timer
+            >>> timer = Timer("my_timer_variable")
+            >>> timer
+            <Timer my_timer_variable paused 0 seconds>
+            >>> timer.start()
+            >>> time.sleep(1)
+            >>> timer
+            <Timer my_timer_variable running 1.015078 seconds>
+            >>> timer.pause()
+            >>> timer
+            <Timer my_timer_variable paused 5.425622 seconds>
+            >>> timer.pack_data()
+            {'my_timer_variable': [5.425622]}
+    """
+
+    id = db.Column(db.Integer, db.ForeignKey("data.id"), primary_key=True)
+    __mapper_args__ = {"polymorphic_identity": "timer"}
+
+    _page_timer_id = db.Column(db.Integer, db.ForeignKey("page.id"))
+
+    is_running = db.Column(db.Boolean)
+    start_time = db.Column(db.DateTime)
+
+    @hybrid_property
+    def total_seconds(self) -> float:
+        """Get the total number of seconds the timer has been running.
+
+        Returns:
+            float: Total seconds.
+        """
+        if self.is_running:
+            return self.data + (datetime.utcnow() - self.start_time).total_seconds()
+        return self.data
+
+    @total_seconds.setter  # type: ignore
+    def total_seconds(self, total_seconds):
+        self.data = total_seconds
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.is_running = False
+        self.total_seconds = 0
+
+    def __repr__(self):
+        running = "running" if self.is_running else "paused"
+        return f"<{self.__class__.__qualname__} {self.variable} {running} {self.total_seconds} seconds>"
+
+    def start(self):
+        """Start the timer."""
+        if not self.is_running:
+            self.is_running = True
+            self.start_time = datetime.utcnow()
+
+    def pause(self):
+        """Pause the timer."""
+        if self.is_running:
+            self.data += (datetime.utcnow() - self.start_time).total_seconds()
+            self.is_running = False
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/tree.py` & `hemlock-survey-1.0.1/src/hemlock/tree.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-"""Tree.
-"""
-from __future__ import annotations
-
-import textwrap
-from typing import TYPE_CHECKING, Any, Callable, List, Union, TypeVar
-
-import matplotlib.pyplot as plt
-from IPython import display
-from flask import render_template, request, url_for
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.ext.orderinglist import ordering_list
-from werkzeug.wrappers.response import Response
-
-from ._display_navigation import display_navigation
-from .app import db, static_pages
-from .page import Page
-from .utils import redirect
-
-if TYPE_CHECKING:
-    from .page import Page
-
-TreeType = TypeVar("TreeType", bound="Tree")
-
-
-class Tree(db.Model):
-    """Tree.
-
-    The tree contains a main branch of pages. (Pages may also have their own branches).
-    Trees control which page the user navigates to next in response to a request.
-
-    Args:
-        seed_func (Callable[[], List[Page]]): The "seed function" initializes the
-            tree's branch.
-
-    Attributes:
-        user (User): The user to which this tree belongs.
-        index (int): Position of this tree relative to other trees belonging to the
-            same user.
-        branch (List[Page]): A list of pages returned by the seed function.
-        page (Page): The page this tree is currently on.
-        request_in_progress (bool): Indicates that this tree is currently processing
-            its user's request.
-        prev_request_method (str): The request method of the user's previous request.
-            Either "GET" or "POST".
-        cached_page_html (str): Cached HTML from the user's last GET request.
-    """
-
-    id = db.Column(db.Integer, primary_key=True)
-
-    _user_id = db.Column(db.Integer, db.ForeignKey("user.id"))
-
-    branch = db.relationship(
-        "Page",
-        backref="tree",
-        order_by="Page.index",
-        collection_class=ordering_list("index"),
-        foreign_keys="Page._tree_id",
-    )
-
-    page = db.relationship("Page", uselist=False, foreign_keys="Page._tree_head_id")
-
-    _seed_func_name = db.Column(db.String)
-    _url_rule = db.Column(db.String)
-    request_in_progress = db.Column(db.Boolean, default=False)
-    prev_request_method = db.Column(db.String(4))
-    cached_page_html = db.Column(db.Text)
-    index = db.Column(db.Integer)
-
-    @hybrid_property
-    def url_rule(self) -> str:
-        """Get the URL rule associated with requests to this tree.
-
-        Returns:
-            str: URL rule.
-        """
-        if self._url_rule is not None:
-            return self._url_rule
-
-        return url_for(f"hemlock.{self._seed_func_name}")
-
-    def __init__(
-        self,
-        seed_func: Callable[[], Union[Page, List[Page]]],
-        url_rule: str = None,
-    ):
-        self._seed_func_name = seed_func.__name__
-        self._url_rule = url_rule
-        branch = seed_func()
-        self.branch = branch if isinstance(branch, list) else [branch]
-        self.page = self.branch[0]
-
-    def __repr__(self):
-        initial_indent = ""
-        subsequent_indent = 4 * " "
-
-        branch_text = "\n".join([str(page) for page in self.branch])
-        branch_text = f"\n{textwrap.indent(branch_text, subsequent_indent)}"
-
-        return textwrap.indent(
-            f"<{self.__class__.__qualname__} id: {self.id}>{branch_text}",
-            initial_indent,
-        )
-
-    def display(
-        self,
-        ax: plt.axes._subplots.AxesSubplot = None,
-        node_size: int = 1200,
-        **subplots_kwargs: Any,
-    ) -> None:
-        """Display the tree's navigation graph and its current page.
-
-        Args:
-            ax (plt.axes._subplots.AxesSubplot, optional): Plot on which to write the
-                tree's navigation graph. Defaults to None.
-            node_size (int, optional): Size of nodes in the navigation graph. Defaults
-                to 1200.
-            **subplots_kwargs (Any): Keyword arguments for ``plt.subplots``.
-        """
-        ax = display_navigation(self, ax, node_size, **subplots_kwargs)
-        plt.show()
-        display.display(self.page.display())
-
-    def go_forward(self: TreeType) -> TreeType:
-        """Go forward from the current page.
-
-        Raises:
-            RuntimeError: Users cannot go forward from the last page.
-
-        Returns:
-            TreeType: self.
-        """
-        if self.page.next_page is not None:
-            self.page = self.page.next_page
-            return self
-
-        if self.page.branch:
-            self.page = self.page.branch[0]
-            return self
-
-        page = self.page
-        while page is page.root_branch[-1]:
-            page = page.root
-            if page is None:
-                raise RuntimeError(
-                    f"Cannot find a page to go forward to from \n{self.page}."
-                )
-        self.page = page.root_branch[page.index + 1]
-        return self
-
-    def go_back(self: TreeType) -> TreeType:
-        """Go back from the current page.
-
-        Raises:
-            RuntimeError: Users cannot go back from the first page.
-
-        Returns:
-            TreeType: self.
-        """
-        if self.page.prev_page is not None:
-            self.page = self.page.prev_page
-            return self
-
-        if self.page is self.page.root_branch[0]:
-            if self.page.root is None:
-                raise RuntimeError(
-                    f"Cannot find a page to go back to from \n{self.page}"
-                )
-            self.page = self.page.root
-            return self
-
-        self.page = self.page.root_branch[self.page.index - 1]
-        while self.page.branch:
-            self.page = self.page.branch[-1]
-        return self
-
-    def process_request(self) -> Union[str, Response]:
-        """Process a user's request and navigate in the appropriate direction.
-
-        Returns:
-            Union[str, Response]: HTML of the next page.
-        """
-        # TODO: remove logging after pilots
-        import logging
-
-        # return a loading page if a request is in progress
-        # or the client submits 2 consecutive POST requests
-        if (
-            self.request_in_progress
-            or request.method == self.prev_request_method == "POST"
-        ):
-            if request.method == self.prev_request_method == "POST":
-                logging.info(
-                    "Prevented double submit via request.method == self.prev_request_methd == 'POST'"
-                )
-            loading_page_key = "loading_page"
-            if loading_page_key not in static_pages:
-                static_pages[loading_page_key] = render_template(
-                    "hemlock/utils/loading_page.html", page=Page()
-                )
-
-            return static_pages[loading_page_key]
-
-        # return the HTML for the current page if the POST request is for another page
-        # (e.g., the POST request is a double submit from a previous page)
-        # or the user refreshed the page
-        if (
-            request.method == "POST" and request.form["page-hash"] != self.page.hash
-        ) or request.method == self.prev_request_method == "GET":
-            if request.method == "POST" and request.form["page-hash"] != self.page.hash:
-                logging.info(
-                    "Prevented double submit via request.form['page-hash'] != self.page.hash"
-                )
-            return self.cached_page_html
-
-        self.request_in_progress = True
-        self.prev_request_method = request.method
-        db.session.commit()
-
-        # handle GET request
-        if request.method == "GET":
-            page_html = self.page.get()
-            self.cached_page_html = page_html
-            self.request_in_progress = False
-            return page_html
-
-        # handle POST request
-        direction_from = self.page.post()
-        if direction_from == "forward":
-            self.go_forward()
-        elif direction_from == "back":
-            self.go_back()
-        self.page.direction_to = direction_from
-
-        self.request_in_progress = False
-        self.redirecting = True
-        return redirect(self.url_rule)
+"""Tree.
+"""
+from __future__ import annotations
+
+import textwrap
+from typing import TYPE_CHECKING, Any, Callable, List, Union, TypeVar
+
+import matplotlib.pyplot as plt
+from IPython import display
+from flask import render_template, request, url_for
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.ext.orderinglist import ordering_list
+from werkzeug.wrappers.response import Response
+
+from ._display_navigation import display_navigation
+from .app import db, static_pages
+from .page import Page
+from .utils import redirect
+
+if TYPE_CHECKING:
+    from .page import Page
+
+TreeType = TypeVar("TreeType", bound="Tree")
+
+
+class Tree(db.Model):
+    """Tree.
+
+    The tree contains a main branch of pages. (Pages may also have their own branches).
+    Trees control which page the user navigates to next in response to a request.
+
+    Args:
+        seed_func (Callable[[], List[Page]]): The "seed function" initializes the
+            tree's branch.
+
+    Attributes:
+        user (User): The user to which this tree belongs.
+        index (int): Position of this tree relative to other trees belonging to the
+            same user.
+        branch (List[Page]): A list of pages returned by the seed function.
+        page (Page): The page this tree is currently on.
+        request_in_progress (bool): Indicates that this tree is currently processing
+            its user's request.
+        prev_request_method (str): The request method of the user's previous request.
+            Either "GET" or "POST".
+        cached_page_html (str): Cached HTML from the user's last GET request.
+    """
+
+    id = db.Column(db.Integer, primary_key=True)
+
+    _user_id = db.Column(db.Integer, db.ForeignKey("user.id"))
+
+    branch = db.relationship(
+        "Page",
+        backref="tree",
+        order_by="Page.index",
+        collection_class=ordering_list("index"),
+        foreign_keys="Page._tree_id",
+    )
+
+    page = db.relationship("Page", uselist=False, foreign_keys="Page._tree_head_id")
+
+    _seed_func_name = db.Column(db.String)
+    _url_rule = db.Column(db.String)
+    request_in_progress = db.Column(db.Boolean, default=False)
+    prev_request_method = db.Column(db.String(4))
+    cached_page_html = db.Column(db.Text)
+    index = db.Column(db.Integer)
+
+    @hybrid_property
+    def url_rule(self) -> str:
+        """Get the URL rule associated with requests to this tree.
+
+        Returns:
+            str: URL rule.
+        """
+        if self._url_rule is not None:
+            return self._url_rule
+
+        return url_for(f"hemlock.{self._seed_func_name}")
+
+    def __init__(
+        self,
+        seed_func: Callable[[], Union[Page, List[Page]]],
+        url_rule: str = None,
+    ):
+        self._seed_func_name = seed_func.__name__
+        self._url_rule = url_rule
+        branch = seed_func()
+        self.branch = branch if isinstance(branch, list) else [branch]
+        self.page = self.branch[0]
+
+    def __repr__(self):
+        initial_indent = ""
+        subsequent_indent = 4 * " "
+
+        branch_text = "\n".join([str(page) for page in self.branch])
+        branch_text = f"\n{textwrap.indent(branch_text, subsequent_indent)}"
+
+        return textwrap.indent(
+            f"<{self.__class__.__qualname__} id: {self.id}>{branch_text}",
+            initial_indent,
+        )
+
+    def display(
+        self,
+        ax: plt.axes._subplots.AxesSubplot = None,
+        node_size: int = 1200,
+        **subplots_kwargs: Any,
+    ) -> None:
+        """Display the tree's navigation graph and its current page.
+
+        Args:
+            ax (plt.axes._subplots.AxesSubplot, optional): Plot on which to write the
+                tree's navigation graph. Defaults to None.
+            node_size (int, optional): Size of nodes in the navigation graph. Defaults
+                to 1200.
+            **subplots_kwargs (Any): Keyword arguments for ``plt.subplots``.
+        """
+        ax = display_navigation(self, ax, node_size, **subplots_kwargs)
+        plt.show()
+        display.display(self.page.display())
+
+    def go_forward(self: TreeType) -> TreeType:
+        """Go forward from the current page.
+
+        Raises:
+            RuntimeError: Users cannot go forward from the last page.
+
+        Returns:
+            TreeType: self.
+        """
+        if self.page.next_page is not None:
+            self.page = self.page.next_page
+            return self
+
+        if self.page.branch:
+            self.page = self.page.branch[0]
+            return self
+
+        page = self.page
+        while page is page.root_branch[-1]:
+            page = page.root
+            if page is None:
+                raise RuntimeError(
+                    f"Cannot find a page to go forward to from \n{self.page}."
+                )
+        self.page = page.root_branch[page.index + 1]
+        return self
+
+    def go_back(self: TreeType) -> TreeType:
+        """Go back from the current page.
+
+        Raises:
+            RuntimeError: Users cannot go back from the first page.
+
+        Returns:
+            TreeType: self.
+        """
+        if self.page.prev_page is not None:
+            self.page = self.page.prev_page
+            return self
+
+        if self.page is self.page.root_branch[0]:
+            if self.page.root is None:
+                raise RuntimeError(
+                    f"Cannot find a page to go back to from \n{self.page}"
+                )
+            self.page = self.page.root
+            return self
+
+        self.page = self.page.root_branch[self.page.index - 1]
+        while self.page.branch:
+            self.page = self.page.branch[-1]
+        return self
+
+    def process_request(self) -> Union[str, Response]:
+        """Process a user's request and navigate in the appropriate direction.
+
+        Returns:
+            Union[str, Response]: HTML of the next page.
+        """
+        # TODO: remove logging after pilots
+        import logging
+
+        # return a loading page if a request is in progress
+        # or the client submits 2 consecutive POST requests
+        if (
+            self.request_in_progress
+            or request.method == self.prev_request_method == "POST"
+        ):
+            if request.method == self.prev_request_method == "POST":
+                logging.info(
+                    "Prevented double submit via request.method == self.prev_request_methd == 'POST'"
+                )
+            loading_page_key = "loading_page"
+            if loading_page_key not in static_pages:
+                static_pages[loading_page_key] = render_template(
+                    "hemlock/utils/loading_page.html", page=Page()
+                )
+
+            return static_pages[loading_page_key]
+
+        # return the HTML for the current page if the POST request is for another page
+        # (e.g., the POST request is a double submit from a previous page)
+        # or the user refreshed the page
+        if (
+            request.method == "POST" and request.form["page-hash"] != self.page.hash
+        ) or request.method == self.prev_request_method == "GET":
+            if request.method == "POST" and request.form["page-hash"] != self.page.hash:
+                logging.info(
+                    "Prevented double submit via request.form['page-hash'] != self.page.hash"
+                )
+            return self.cached_page_html
+
+        self.request_in_progress = True
+        self.prev_request_method = request.method
+        db.session.commit()
+
+        # handle GET request
+        if request.method == "GET":
+            page_html = self.page.get()
+            self.cached_page_html = page_html
+            self.request_in_progress = False
+            return page_html
+
+        # handle POST request
+        direction_from = self.page.post()
+        if direction_from == "forward":
+            self.go_forward()
+        elif direction_from == "back":
+            self.go_back()
+        self.page.direction_to = direction_from
+
+        self.request_in_progress = False
+        self.redirecting = True
+        return redirect(self.url_rule)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/user.py` & `hemlock-survey-1.0.1/src/hemlock/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,672 +1,697 @@
-"""User.
-"""
-from __future__ import annotations
-
-import functools
-import logging
-import warnings
-from collections import defaultdict
-from datetime import datetime
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Mapping,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
-
-import pandas as pd
-from flask import current_app, request
-from flask_login import UserMixin, current_user, login_required, login_user
-from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.ext.orderinglist import ordering_list
-from sqlalchemy.types import JSON
-from sqlalchemy_mutable.types import MutablePickleType, MutableDictJSONType
-from sqlalchemy_mutable.utils import get_object, is_callable
-from werkzeug.wrappers.response import Response
-
-from ._data_frame import DataFrame
-from .app import bp, db, login_manager
-from .tree import Tree
-from .utils.random import make_hash
-
-if TYPE_CHECKING:  # pragma: no cover
-    from .page import Page
-    from .questions.base import Question
-
-HASH_LENGTH = 90
-
-BranchType = List["Page"]
-SeedFunctionType = Callable[[], BranchType]
-UserType = TypeVar("UserType", bound="User")
-ResponsesType = Union[List[Any], Dict["Question", Any]]
-
-logging.basicConfig(level=logging.INFO)
-
-
-@login_manager.user_loader
-def load_user(user_id: int) -> User:
-    """Load user.
-
-    Args:
-        user_id (int): User id.
-
-    Returns:
-        User: Loaded user.
-    """
-    return User.query.get(user_id)
-
-
-class User(UserMixin, db.Model):
-    """User.
-
-    The user has the following responsibilities:
-
-    1. The user object contains a list of branches. Based on the URL rule of a request, the user determines which of its trees should process the request.
-    2. The user object stores the data for individual users and can collect the data for all users.
-    3. The user provides testing utilities.
-
-    Args:
-        meta_data (Mapping, optional): User metadata. In an online study, this records
-            the user's IP address and any request arguments. Defaults to None.
-
-    Attributes:
-        trees (List[Tree]): Trees that the user can navigate to.
-        start_time (datetime.datetime): Time at which the user started the study.
-        end_time (datetime.datetime): Time at which the user ended the study.
-        completed (bool): Indicates that the user completed the study.
-        failed (bool): Indicates that the user failed the study.
-        errored (bool): Indicates that the user experienced an error.
-        in_progress (bool): Indicates that the user is working on the study.
-        params (Any): Additional parameters.
-        meta_data (Dict[str, Any]): User metadata. In most studies, this will contain
-            the IP address.
-
-    Examples:
-
-        .. code-block::
-
-            >>> from hemlock import User, Page, create_test_app
-            >>> from hemlock.questions import Input, Label
-            >>> from sqlalchemy_mutable.utils import partial
-            >>> def greet_user(greeting_label, name_input):
-            ...     greeting_label.label = f"Hello, {name_input.response}!"
-            ...
-            >>> def seed():
-            ...     return [
-            ...         Page(
-            ...             name_input:=Input("What's your name?")
-            ...         ),
-            ...         Page(
-            ...             Label(compile=partial(greet_user, name_input))
-            ...         )
-            ...     ]
-            ...
-            >>> app = create_test_app()
-            >>> user = User.make_test_user(seed)
-            >>> user.test_get().page
-            <Page 0>
-                <Input What's your name? - default: None>
-            >>> user.test_request(["World"]).page
-            <Page 1 terminal>
-                <Label Hello, World! - default: None>
-    """
-
-    _seed_funcs: Dict[str, Tuple[int, SeedFunctionType]] = {}
-    default_url_rule: Optional[str] = None
-
-    id = db.Column(db.Integer, primary_key=True)
-
-    trees = db.relationship(
-        "Tree", order_by="Tree.index", collection_class=ordering_list("index")
-    )
-
-    @classmethod
-    def route(
-        cls, url_rule: str, default: bool = False
-    ) -> Callable[[SeedFunctionType], SeedFunctionType]:
-        """Register a user route.
-
-        Args:
-            url_rule (str): URL rule associated with this route.
-            default (bool, optional): Indicates that this should be the user's default
-                route. Defaults to False.
-
-        Returns:
-            Callable[[SeedFunctionType], SeedFunctionType]: Route decorator.
-
-        Examples:
-
-            .. doctest::
-
-                >>> from hemlock import User, Page, create_test_app
-                >>> @User.route("/survey")
-                ... def seed():
-                ...     return Page(
-                ...         Label("Hello, world!")
-                ...     )
-                ...
-                >>> app = create_test_app()
-                >>> user = User.make_test_user()
-                >>> user.test_get().page
-                <Page 0 terminal>
-                    <Label Hello, world! - default: None>
-        """
-
-        def register(seed_func: SeedFunctionType) -> SeedFunctionType:
-            if url_rule in cls._seed_funcs:
-                warnings.warn(
-                    f"The url rule '{url_rule}' has already been registered.",
-                    RuntimeWarning,
-                )
-                cls._seed_funcs[url_rule] = cls._seed_funcs[url_rule][0], seed_func
-                return seed_func
-
-            @bp.route(url_rule, methods=["GET", "POST"])
-            @login_required
-            @functools.wraps(seed_func)
-            def view_function():
-                return current_user.process_request(url_rule)
-
-            index = 0
-            if cls._seed_funcs:
-                index = list(cls._seed_funcs.values())[-1][0] + 1
-            cls._seed_funcs[url_rule] = index, seed_func
-
-            return seed_func
-
-        if default or cls.default_url_rule is None:
-            cls.default_url_rule = url_rule
-
-        return register
-
-    hash = db.Column(db.String(HASH_LENGTH))
-    start_time = db.Column(db.DateTime)
-    end_time = db.Column(db.DateTime)
-    params = db.Column(MutablePickleType)
-    meta_data = db.Column(MutableDictJSONType)
-    errored = db.Column(db.Boolean)
-    _cached_data = db.Column(JSON)
-
-    _completed = db.Column(db.Boolean)
-
-    @hybrid_property
-    def completed(self) -> Optional[bool]:
-        """Indicates that the user completed the study."""
-        return self._completed
-
-    @completed.setter  # type: ignore
-    def completed(self, completed: bool) -> None:
-        """Set the completion status. Cache the user's data when he completes the study."""
-        # Note: We need to set completed first so the meta_data reflect that the user
-        # has completed the survey when caching the metadata.
-        self._completed = completed
-        if completed:
-            if self.failed:
-                warnings.warn(
-                    "Indicating that the user completed the study,"
-                    " but the user has already failed the study.",
-                    RuntimeWarning,
-                )
-            self.cache_data()
-
-    _failed = db.Column(db.Boolean)
-
-    @hybrid_property
-    def failed(self) -> bool:
-        """Indicate that the user failed the study."""
-        return self._failed
-
-    @failed.setter  # type: ignore
-    def failed(self, failed: bool) -> None:
-        """Set the failed status. Cache the user's data when he fails the study."""
-        self._failed = failed
-        if failed:
-            if self.completed:
-                warnings.warn(
-                    "Indicating that the user failed the study,"
-                    " but the user has already completed the study.",
-                    RuntimeWarning,
-                )
-            self.cache_data()
-
-    @hybrid_property
-    def in_progress(self):
-        return not (self.completed or self.failed or self.errored)
-
-    def __init__(self, meta_data: Mapping = None):
-        self.hash = make_hash(HASH_LENGTH)
-        self.start_time = self.end_time = datetime.utcnow()
-        self.completed = self.failed = self.errored = False  # type: ignore
-        self.meta_data = meta_data or {}
-
-        # need to login user before initializing trees so that the current_user object
-        # will be available in the seed functions
-        db.session.add(self)
-        db.session.commit()
-        self._cached_data = self.get_data(to_pandas=False)
-        login_user(self)
-        self.trees = [Tree(func) for _, func in self._seed_funcs.values()]
-
-    def __repr__(self):
-        return f"<{self.__class__.__qualname__} {self.get_meta_data(True)}>"
-
-    def get_tree(self, url_rule: str = None) -> Tree:
-        """Get the tree associated with the given URL rule.
-
-        Args:
-            url_rule (str, optional): URL rule. Defaults to None.
-
-        Returns:
-            Tree: Tree associated with the URL rule.
-        """
-        # get the index of the requested tree
-        index = self._seed_funcs[url_rule or self.default_url_rule][0]  # type: ignore
-        return self.trees[index]
-
-    def cache_data(self) -> None:
-        """Cache the user's data."""
-        self._cached_data = self.get_data(to_pandas=False, use_cached_data=False)
-
-    def get_meta_data(self, convert_to_string: bool = False) -> Dict[str, Any]:
-        """Get the user's metadata.
-
-        Args:
-            convert_to_string (bool, optional): Indicates that the user's start and end
-                times should be converted to a string. Defaults to False.
-
-        Returns:
-            Dict[str, Any]: User's metadata. This is the ``user.meta_data`` attribute
-                plus other metadata such as the start and end time.
-        """
-        metadata = {
-            "id": self.id,
-            "completed": self.completed,
-            "failed": self.failed,
-            "errored": self.errored,
-            "in_progress": self.in_progress,
-            "start_time": self.start_time,
-            "end_time": self.end_time,
-            "total_seconds": (self.end_time - self.start_time).total_seconds(),
-        }
-        if convert_to_string:
-            metadata["start_time"] = str(metadata["start_time"])
-            metadata["end_time"] = str(metadata["end_time"])
-
-        metadata.update(self.meta_data)
-        for key, item in metadata.items():
-            metadata[key] = get_object(item)
-
-        return metadata
-
-    def get_data(
-        self, to_pandas: bool = True, use_cached_data: bool = True
-    ) -> Union[pd.DataFrame, DataFrame]:
-        """Get the user's data.
-
-        Args:
-            to_pandas (bool, optional): Indicates that the data should be returned as a
-                pandas dataframe. Defaults to True.
-            use_cached_data (bool, optional): Indicates that cached data should be used
-                instead of re-collecting the data if possible. Defaults to True.
-
-        Returns:
-            Union[pd.DataFrame, DataFrame]: User's data.
-        """
-        if use_cached_data and self._cached_data is not None:
-            df = self._cached_data
-        else:
-            meta_data = self.get_meta_data(convert_to_string=True)
-            meta_data = {key: [item] for key, item in meta_data.items()}
-            df = DataFrame(meta_data, fill_rows=True)
-            [df.add_branch(tree.branch) for tree in self.trees]
-            df.pad()
-
-        return pd.DataFrame(df) if to_pandas else df
-
-    @staticmethod
-    def get_all_data(
-        to_pandas: bool = True, refresh_if_in_progress: bool = False
-    ) -> Union[pd.DataFrame, DataFrame]:
-        """Get the data for all users.
-
-        Args:
-            to_pandas (bool, optional): Indicates. Defaults to True.
-            refresh_if_in_progress (bool, optional): Refresh data for in progress users
-                when getting their data. Setting this to True can greatly increase the
-                runtime. Defaults to False.
-
-        Returns:
-            Union[pd.DataFrame, DataFrame]: Data from all users.
-        """
-        df = DataFrame()
-        for user in User.query.all():
-            if refresh_if_in_progress and user.in_progress:
-                df.add_data(user.get_data(to_pandas=False, use_cached_data=False))
-            else:
-                df.add_data(user.get_data(to_pandas=False))
-            df.pad()
-
-        return pd.DataFrame(df) if to_pandas else df
-
-    def process_request(self, url_rule: str) -> Union[str, Response]:
-        """Process a request.
-
-        Args:
-            url_rule (str): Requested URL rule.
-
-        Returns:
-            Union[str, Response]: HTML of the next page.
-        """
-        if request.method == "POST":
-            self.end_time = datetime.utcnow()
-
-        current_tree = self.get_tree(url_rule)
-        return_value = current_tree.process_request()
-
-        if (
-            not self.failed
-            and current_tree.page.is_last_page
-            and [tree.page.is_last_page for tree in self.trees]
-        ):
-            self.completed = True  # type: ignore
-
-        db.session.commit()
-        return return_value
-
-    @classmethod
-    def make_test_user(
-        cls: Type[UserType],
-        seed_func: SeedFunctionType = None,
-        url_rule: str = "/test",
-        **kwargs: Any,
-    ) -> UserType:
-        """Create a user object for testing.
-
-        Args:
-            seed_func (SeedFunctionType, optional): Function that returns the user's
-                first branch. Defaults to None.
-            url_rule (str, optional): Default URL rule for the test user. Defaults to
-                "/test".
-            kwargs (Any): Passed to :class:`User` constructor.
-
-        Returns:
-            UserType: Test user object.
-
-        Examples:
-
-            .. doctest::
-
-                >>> from hemlock import User, Page, create_test_app
-                >>> from hemlock.questions import Label
-                >>> app = create_test_app()
-                >>> def seed():
-                ...     return Page(
-                ...         Label("Hello, world!")
-                ...     )
-                ...
-                >>> user = User.make_test_user(seed)
-                >>> user.test_get().page
-                <Page 0 terminal>
-                    <Label Hello, world! - default: None>
-        """
-        with current_app.test_request_context():
-            user = cls(**kwargs)
-
-            if seed_func is not None:
-                index = 0
-                if user._seed_funcs:
-                    index = list(user._seed_funcs.values())[-1][0] + 1
-                user._seed_funcs = user._seed_funcs.copy()
-                user._seed_funcs[url_rule] = index, seed_func
-                user.default_url_rule = url_rule
-                user.trees.append(Tree(seed_func, url_rule))
-
-        return user
-
-    @classmethod
-    def test_multiple_users(
-        cls,
-        n_users: int = 1,
-        seed_func: SeedFunctionType = None,
-        user_kwargs: Mapping[str, Any] = None,
-        test_kwargs: Mapping[str, Any] = None,
-    ) -> None:
-        """Run multiple test users through a study.
-
-        Args:
-            n_users (int, optional): Number of users to run. Defaults to 1.
-            seed_func (SeedFunctionType, optional): Function that returns the user's
-                first branch. Defaults to None.
-            user_kwargs (Mapping[str, Any], optional): Passed to
-                :meth:`User.make_test_user`. Defaults to None.
-            test_kwargs (Mapping[str, Any], optional): Passed to :meth:`User.test`.
-                Defaults to None.
-
-        Examples:
-
-            .. code-block::
-
-                >>> from hemlock import User, Page, create_test_app
-                >>> from hemlock.questions import Label
-                >>> def seed():
-                ...     return [
-                ...         Page(
-                ...             Label("Hello, world!")
-                ...         ),
-                ...         Page()
-                ...     ]
-                ...
-                >>> app = create_test_app()
-                >>> User.test_multiple_users(2, seed)
-                INFO:root:TESTING USER 1
-                INFO:root:<Page 0>
-                    <Label Hello, world! - default: None>
-                        test response: None
-                    test direction: 'forward'
-                INFO:root:<Page 1 terminal>
-                INFO:root:FINISHED TESTING USER 1
-
-                INFO:root:TESTING USER 2
-                INFO:root:<Page 0>
-                    <Label Hello, world! - default: None>
-                        test response: None
-                    test direction: 'forward'
-                INFO:root:<Page 1 terminal>
-                INFO:root:FINISHED TESTING USER 2
-        """
-        user_kwargs = dict(user_kwargs or {})
-        user_kwargs["seed_func"] = seed_func
-        test_kwargs = dict(test_kwargs or {})
-        test_kwargs.setdefault("verbosity", 1)
-
-        for _ in range(n_users):
-            user = cls.make_test_user(**user_kwargs)
-            logging.info(f"TESTING USER {user.id}")
-            user.test(**test_kwargs)
-            logging.info(f"FINISHED TESTING USER {user.id}\n")
-
-    def test(
-        self, url_rule: str = None, verbosity: int = 2, max_page_visits: int = 10
-    ) -> None:
-        """Run the test user through the entire study.
-
-        Args:
-            url_rule (str, optional): URL rule to test. Defaults to None.
-            verbosity (int, optional): Verbosity 0 gives no output. Verbosity 1
-                displays pages and test responses as text. Verbosity 2 additionally
-                displays the navigation graph and pages as HTML. Defaults to 2.
-            max_page_visits (int, optional): Maximum number of times the user can visit
-                the same page before an error is raised. Defaults to 10.
-
-        Raises:
-            RuntimeError: If the user visits the same page more times than allowed.
-                Likely causes include validate functions that always return False and
-                infinite loops.
-
-        Examples:
-
-            .. code-block::
-
-                >>> from hemlock import User, Page, create_test_app
-                >>> from hemlock.questions import Label
-                >>> def seed():
-                ...     return [
-                ...         Page(
-                ...             Label("Hello, world!")
-                ...         ),
-                ...         Page()
-                ...     ]
-                ...
-                >>> app = create_test_app()
-                >>> User.make_test_user(seed).test(verbosity=1)
-                INFO:root:<Page 0>
-                    <Label Hello, world! - default: None>
-                        test response: None
-                    test direction: 'forward'
-                INFO:root:<Page 1 terminal>
-        """
-        page_visits: defaultdict[str, int] = defaultdict(int)
-
-        tree = self.test_get(url_rule=url_rule)
-        page_visits[tree.page.get_position()] += 1
-        if verbosity == 2:
-            tree.display()
-
-        while not tree.page.is_last_page:
-            tree = self.test_request(url_rule=url_rule, verbose=verbosity >= 1)
-            page_visits[tree.page.get_position()] += 1
-            if page_visits[tree.page.get_position()] > max_page_visits:
-                raise RuntimeError(
-                    f"The test user has visited the same page more than {max_page_visits} times."
-                    " Check that your validate functions don't always return False"
-                    " and that your survey doesn't contain an infinite loop."
-                    " The page is\n{tree.page}"
-                )
-            if verbosity == 2:
-                tree.display()
-
-        if verbosity >= 1:
-            logging.info(tree.page.print())
-
-    def test_request(
-        self,
-        responses: ResponsesType = None,
-        direction: str = None,
-        url_rule: str = None,
-        **kwargs,
-    ) -> Tree:
-        """Test a request.
-
-        This simulates posting responses for the current page and getting the next page.
-
-        Args:
-            responses (ResponsesType, optional): Test responses. Defaults to None.
-            direction (str, optional): Requested direction. Defaults to "forward".
-            url_rule (str, optional): URL rule of the request. Defaults to None.
-            **kwargs (Any): Passed to :meth:`User.test_post`.
-
-        Returns:
-            Tree: Tree associated with the URL rule.
-        """
-        self.test_post(
-            responses=responses, direction=direction, url_rule=url_rule, **kwargs
-        )
-        return self.test_get(url_rule)
-
-    def test_get(self, url_rule: str = None) -> Tree:
-        """Test a get request.
-
-        Args:
-            url_rule (str, optional): URL rule of the request. Defaults to None.
-
-        Returns:
-            Tree: Tree associated with the URL rule.
-        """
-        url_rule = url_rule or self.default_url_rule
-        with current_app.test_request_context():
-            login_user(self)
-            self.process_request(url_rule)  # type: ignore
-        return self.get_tree(url_rule)
-
-    def test_post(
-        self,
-        responses: ResponsesType = None,
-        direction: str = None,
-        url_rule: str = None,
-        verbose: bool = True,
-    ) -> Tree:
-        """Test a post request.
-
-        Args:
-            responses (ResponsesType, optional): Test responses. Defaults to None.
-            direction (str, optional): Requested direction. Defaults to "forward".
-            url_rule (str, optional): URL rule of the request. Defaults to None.
-            verbose (bool, optional): When True, logs the current page and responses.
-                Defaults to True.
-
-        Returns:
-            Tree: Tree associated with the URL rule.
-        """
-        url_rule = url_rule or self.default_url_rule
-        tree = self.get_tree(url_rule)
-        page = tree.page
-
-        # collect manually input responses
-        if responses is None:
-            responses = {}
-        elif isinstance(responses, (list, tuple)):
-            if len(page.questions) != len(responses):
-                raise ValueError(
-                    "Number of responses does not match number of questions\n"
-                    f"Responses: {responses}\n"
-                    f"Page: {page}"
-                )
-            responses = {
-                question: response
-                for question, response in zip(page.questions, responses)
-            }
-        elif isinstance(responses, Mapping):
-            responses = dict(responses)
-        else:
-            raise ValueError(
-                f"Responses should be a list, tuple, or mapping, got {repr(responses)}."
-            )
-
-        # add automatic responses
-        for question in page.questions:
-            if question not in responses:
-                if is_callable(question.test_response):
-                    responses[question] = question.test_response(question)
-                else:
-                    responses[question] = question.test_response
-
-        # convert responses to raw responses
-        data = {
-            question.hash: question.make_raw_test_response(response)
-            for question, response in responses.items()
-        }
-
-        # set the requested direction and page hash
-        if direction is None:
-            if is_callable(page.test_direction):
-                direction = page.test_direction(page)
-            else:
-                direction = page.test_direction
-        data["direction"] = direction
-        data["page-hash"] = page.hash
-
-        # log the page and planned responses
-        if verbose:
-            logging.info(page.print(responses, direction))
-
-        with current_app.test_request_context(method="POST", data=data):
-            login_user(self)
-            self.process_request(url_rule)  # type: ignore
-        return tree
+"""User.
+"""
+from __future__ import annotations
+
+import functools
+import logging
+import warnings
+from collections import defaultdict
+from datetime import datetime
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+import pandas as pd
+from flask import current_app, request
+from flask_login import UserMixin, current_user, login_required, login_user
+from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.ext.orderinglist import ordering_list
+from sqlalchemy.orm import validates
+from sqlalchemy.types import JSON
+from sqlalchemy_mutable.types import MutablePickleType, MutableDictJSONType
+from sqlalchemy_mutable.utils import get_object, is_callable
+from werkzeug.wrappers.response import Response
+
+from ._data_frame import DataFrame
+from .app import bp, db, login_manager
+from .data import Data
+from .tree import Tree
+from .utils.random import make_hash
+
+if TYPE_CHECKING:  # pragma: no cover
+    from .page import Page
+    from .questions.base import Question
+
+HASH_LENGTH = 90
+
+BranchType = List["Page"]
+SeedFunctionType = Callable[[], BranchType]
+UserType = TypeVar("UserType", bound="User")
+ResponsesType = Union[List[Any], Dict["Question", Any]]
+
+logging.basicConfig(level=logging.INFO)
+
+
+@login_manager.user_loader
+def load_user(user_id: int) -> User:
+    """Load user.
+
+    Args:
+        user_id (int): User id.
+
+    Returns:
+        User: Loaded user.
+    """
+    return User.query.get(user_id)
+
+
+class User(UserMixin, db.Model):
+    """User.
+
+    The user has the following responsibilities:
+
+    1. The user object contains a list of branches. Based on the URL rule of a request, the user determines which of its trees should process the request.
+    2. The user object stores the data for individual users and can collect the data for all users.
+    3. The user provides testing utilities.
+
+    Args:
+        meta_data (Mapping, optional): User metadata. In an online study, this records
+            the user's IP address and any request arguments. Defaults to None.
+
+    Attributes:
+        trees (List[Tree]): Trees that the user can navigate to.
+        start_time (datetime.datetime): Time at which the user started the study.
+        end_time (datetime.datetime): Time at which the user ended the study.
+        completed (bool): Indicates that the user completed the study.
+        failed (bool): Indicates that the user failed the study.
+        errored (bool): Indicates that the user experienced an error.
+        in_progress (bool): Indicates that the user is working on the study.
+        params (Any): Additional parameters.
+        meta_data (Dict[str, Any]): User metadata. In most studies, this will contain
+            the IP address.
+
+    Examples:
+
+        .. code-block::
+
+            >>> from hemlock import User, Page, create_test_app
+            >>> from hemlock.questions import Input, Label
+            >>> from sqlalchemy_mutable.utils import partial
+            >>> def greet_user(greeting_label, name_input):
+            ...     greeting_label.label = f"Hello, {name_input.response}!"
+            ...
+            >>> def seed():
+            ...     return [
+            ...         Page(
+            ...             name_input:=Input("What's your name?")
+            ...         ),
+            ...         Page(
+            ...             Label(compile=partial(greet_user, name_input))
+            ...         )
+            ...     ]
+            ...
+            >>> app = create_test_app()
+            >>> user = User.make_test_user(seed)
+            >>> user.test_get().page
+            <Page 0>
+                <Input What's your name? - default: None>
+            >>> user.test_request(["World"]).page
+            <Page 1 terminal>
+                <Label Hello, World! - default: None>
+    """
+
+    _seed_funcs: Dict[str, Tuple[int, SeedFunctionType]] = {}
+    default_url_rule: Optional[str] = None
+
+    id = db.Column(db.Integer, primary_key=True)
+
+    trees = db.relationship(
+        "Tree", order_by="Tree.index", collection_class=ordering_list("index")
+    )
+
+    data = db.relationship(
+        "Data",
+        order_by="Data.index",
+        collection_class=ordering_list("index"),
+        foreign_keys="Data._user_id",
+    )
+
+    @validates("data")
+    def _validate_data(self, key: str, data: Union[Data, Tuple]) -> Data:
+        """Data can be input as a :class:`hemlock.data.Data` object or a tuple.
+
+        Tuple inputs are used as arguments for the ``Data`` constructor.
+        """
+        return data if isinstance(data, Data) else Data(*data)
+
+    @classmethod
+    def route(
+        cls, url_rule: str, default: bool = False
+    ) -> Callable[[SeedFunctionType], SeedFunctionType]:
+        """Register a user route.
+
+        Args:
+            url_rule (str): URL rule associated with this route.
+            default (bool, optional): Indicates that this should be the user's default
+                route. Defaults to False.
+
+        Returns:
+            Callable[[SeedFunctionType], SeedFunctionType]: Route decorator.
+
+        Examples:
+
+            .. code-block::
+
+                >>> from hemlock import User, Page, create_test_app
+                >>> @User.route("/survey")
+                ... def seed():
+                ...     return Page(
+                ...         Label("Hello, world!")
+                ...     )
+                ...
+                >>> app = create_test_app()
+                >>> user = User.make_test_user()
+                >>> user.test_get().page
+                <Page 0 terminal>
+                    <Label Hello, world! - default: None>
+        """
+
+        def register(seed_func: SeedFunctionType) -> SeedFunctionType:
+            if url_rule in cls._seed_funcs:
+                warnings.warn(
+                    f"The url rule '{url_rule}' has already been registered.",
+                    RuntimeWarning,
+                )
+                cls._seed_funcs[url_rule] = cls._seed_funcs[url_rule][0], seed_func
+                return seed_func
+
+            @bp.route(url_rule, methods=["GET", "POST"])
+            @login_required
+            @functools.wraps(seed_func)
+            def view_function():
+                return current_user.process_request(url_rule)
+
+            index = 0
+            if cls._seed_funcs:
+                index = list(cls._seed_funcs.values())[-1][0] + 1
+            cls._seed_funcs[url_rule] = index, seed_func
+
+            return seed_func
+
+        if default or cls.default_url_rule is None:
+            cls.default_url_rule = url_rule
+
+        return register
+
+    hash = db.Column(db.String(HASH_LENGTH))
+    start_time = db.Column(db.DateTime)
+    end_time = db.Column(db.DateTime)
+    params = db.Column(MutablePickleType)
+    meta_data = db.Column(MutableDictJSONType)
+    errored = db.Column(db.Boolean)
+    _cached_data = db.Column(JSON)
+
+    _completed = db.Column(db.Boolean)
+
+    @hybrid_property
+    def completed(self) -> Optional[bool]:
+        """Indicates that the user completed the study."""
+        return self._completed
+
+    @completed.setter  # type: ignore
+    def completed(self, completed: bool) -> None:
+        """Set the completion status. Cache the user's data when he completes the study."""
+        # Note: We need to set completed first so the meta_data reflect that the user
+        # has completed the survey when caching the metadata.
+        self._completed = completed
+        if completed:
+            if self.failed:
+                warnings.warn(
+                    "Indicating that the user completed the study,"
+                    " but the user has already failed the study.",
+                    RuntimeWarning,
+                )
+            self.cache_data()
+
+    _failed = db.Column(db.Boolean)
+
+    @hybrid_property
+    def failed(self) -> bool:
+        """Indicate that the user failed the study."""
+        return self._failed
+
+    @failed.setter  # type: ignore
+    def failed(self, failed: bool) -> None:
+        """Set the failed status. Cache the user's data when he fails the study."""
+        self._failed = failed
+        if failed:
+            if self.completed:
+                warnings.warn(
+                    "Indicating that the user failed the study,"
+                    " but the user has already completed the study.",
+                    RuntimeWarning,
+                )
+            self.cache_data()
+
+    @hybrid_property
+    def in_progress(self):
+        return not (self.completed or self.failed or self.errored)
+
+    def __init__(self, meta_data: Mapping = None):
+        self.hash = make_hash(HASH_LENGTH)
+        self.start_time = self.end_time = datetime.utcnow()
+        self.completed = self.failed = self.errored = False  # type: ignore
+        self.meta_data = meta_data or {}
+
+        # need to login user before initializing trees so that the current_user object
+        # will be available in the seed functions
+        db.session.add(self)
+        db.session.commit()
+        self._cached_data = self.get_data(to_pandas=False)
+        login_user(self)
+        self.trees = [Tree(func) for _, func in self._seed_funcs.values()]
+
+    def __repr__(self):
+        return f"<{self.__class__.__qualname__} {self.get_meta_data(True)}>"
+
+    def get_tree(self, url_rule: str = None) -> Tree:
+        """Get the tree associated with the given URL rule.
+
+        Args:
+            url_rule (str, optional): URL rule. Defaults to None.
+
+        Returns:
+            Tree: Tree associated with the URL rule.
+        """
+        # get the index of the requested tree
+        index = self._seed_funcs[url_rule or self.default_url_rule][0]  # type: ignore
+        return self.trees[index]
+
+    def cache_data(self) -> None:
+        """Cache the user's data."""
+        self._cached_data = self.get_data(to_pandas=False, use_cached_data=False)
+
+    def get_meta_data(self, convert_to_string: bool = False) -> Dict[str, Any]:
+        """Get the user's metadata.
+
+        Args:
+            convert_to_string (bool, optional): Indicates that the user's start and end
+                times should be converted to a string. Defaults to False.
+
+        Returns:
+            Dict[str, Any]: User's metadata. This is the ``user.meta_data`` attribute
+                plus other metadata such as the start and end time.
+        """
+        metadata = {
+            "id": self.id,
+            "completed": self.completed,
+            "failed": self.failed,
+            "errored": self.errored,
+            "in_progress": self.in_progress,
+            "start_time": self.start_time,
+            "end_time": self.end_time,
+            "total_seconds": (self.end_time - self.start_time).total_seconds(),
+        }
+        if convert_to_string:
+            metadata["start_time"] = str(metadata["start_time"])
+            metadata["end_time"] = str(metadata["end_time"])
+
+        metadata.update(self.meta_data)
+        for key, item in metadata.items():
+            metadata[key] = get_object(item)
+
+        return metadata
+
+    def get_data(
+        self, to_pandas: bool = True, use_cached_data: bool = True
+    ) -> Union[pd.DataFrame, DataFrame]:
+        """Get the user's data.
+
+        Args:
+            to_pandas (bool, optional): Indicates that the data should be returned as a
+                pandas dataframe. Defaults to True.
+            use_cached_data (bool, optional): Indicates that cached data should be used
+                instead of re-collecting the data if possible. Defaults to True.
+
+        Returns:
+            Union[pd.DataFrame, DataFrame]: User's data.
+        """
+        if use_cached_data and self._cached_data is not None:
+            df = self._cached_data
+        else:
+            meta_data = self.get_meta_data(convert_to_string=True)
+            meta_data = {key: [item] for key, item in meta_data.items()}
+            df = DataFrame(meta_data, fill_rows=True)
+            for item in self.data:
+                if item.variable:
+                    df.add_data(item.pack_data(), item.fill_rows)
+            [df.add_branch(tree.branch) for tree in self.trees]
+            df.pad()
+
+        return pd.DataFrame(df) if to_pandas else df
+
+    @staticmethod
+    def get_all_data(
+        to_pandas: bool = True, refresh_if_in_progress: bool = False
+    ) -> Union[pd.DataFrame, DataFrame]:
+        """Get the data for all users.
+
+        Args:
+            to_pandas (bool, optional): Indicates. Defaults to True.
+            refresh_if_in_progress (bool, optional): Refresh data for in progress users
+                when getting their data. Setting this to True can greatly increase the
+                runtime. Defaults to False.
+
+        Returns:
+            Union[pd.DataFrame, DataFrame]: Data from all users.
+        """
+        df = DataFrame()
+        for user in User.query.all():
+            if refresh_if_in_progress and user.in_progress:
+                df.add_data(user.get_data(to_pandas=False, use_cached_data=False))
+            else:
+                df.add_data(user.get_data(to_pandas=False))
+            df.pad()
+
+        return pd.DataFrame(df) if to_pandas else df
+
+    def process_request(self, url_rule: str) -> Union[str, Response]:
+        """Process a request.
+
+        Args:
+            url_rule (str): Requested URL rule.
+
+        Returns:
+            Union[str, Response]: HTML of the next page.
+        """
+        if request.method == "POST":
+            self.end_time = datetime.utcnow()
+
+        current_tree = self.get_tree(url_rule)
+        return_value = current_tree.process_request()
+
+        if (
+            not self.failed
+            and current_tree.page.is_last_page
+            and [tree.page.is_last_page for tree in self.trees]
+        ):
+            self.completed = True  # type: ignore
+
+        db.session.commit()
+        return return_value
+
+    @classmethod
+    def make_test_user(
+        cls: Type[UserType],
+        seed_func: SeedFunctionType = None,
+        url_rule: str = "/test",
+        **kwargs: Any,
+    ) -> UserType:
+        """Create a user object for testing.
+
+        Args:
+            seed_func (SeedFunctionType, optional): Function that returns the user's
+                first branch. Defaults to None.
+            url_rule (str, optional): Default URL rule for the test user. Defaults to
+                "/test".
+            kwargs (Any): Passed to :class:`User` constructor.
+
+        Returns:
+            UserType: Test user object.
+
+        Examples:
+
+            .. doctest::
+
+                >>> from hemlock import User, Page, create_test_app
+                >>> from hemlock.questions import Label
+                >>> app = create_test_app()
+                >>> def seed():
+                ...     return Page(
+                ...         Label("Hello, world!")
+                ...     )
+                ...
+                >>> user = User.make_test_user(seed)
+                >>> user.test_get().page
+                <Page 0 terminal>
+                    <Label Hello, world! - default: None>
+        """
+        with current_app.test_request_context():
+            user = cls(**kwargs)
+
+            if seed_func is not None:
+                index = 0
+                if user._seed_funcs:
+                    index = list(user._seed_funcs.values())[-1][0] + 1
+                user._seed_funcs = user._seed_funcs.copy()
+                user._seed_funcs[url_rule] = index, seed_func
+                user.default_url_rule = url_rule
+                user.trees = user.trees + [Tree(seed_func, url_rule)]
+                # Note: can't use
+                # >>> user.trees.append(Tree(seed_func, url_rule))
+                # or else you get a collection class issue if you run
+                # >>> db.session.commit()
+                # in the seed function
+
+        return user
+
+    @classmethod
+    def test_multiple_users(
+        cls,
+        n_users: int = 1,
+        seed_func: SeedFunctionType = None,
+        user_kwargs: Mapping[str, Any] = None,
+        test_kwargs: Mapping[str, Any] = None,
+    ) -> None:
+        """Run multiple test users through a study.
+
+        Args:
+            n_users (int, optional): Number of users to run. Defaults to 1.
+            seed_func (SeedFunctionType, optional): Function that returns the user's
+                first branch. Defaults to None.
+            user_kwargs (Mapping[str, Any], optional): Passed to
+                :meth:`User.make_test_user`. Defaults to None.
+            test_kwargs (Mapping[str, Any], optional): Passed to :meth:`User.test`.
+                Defaults to None.
+
+        Examples:
+
+            .. code-block::
+
+                >>> from hemlock import User, Page, create_test_app
+                >>> from hemlock.questions import Label
+                >>> def seed():
+                ...     return [
+                ...         Page(
+                ...             Label("Hello, world!")
+                ...         ),
+                ...         Page()
+                ...     ]
+                ...
+                >>> app = create_test_app()
+                >>> User.test_multiple_users(2, seed)
+                INFO:root:TESTING USER 1
+                INFO:root:<Page 0>
+                    <Label Hello, world! - default: None>
+                        test response: None
+                    test direction: 'forward'
+                INFO:root:<Page 1 terminal>
+                INFO:root:FINISHED TESTING USER 1
+
+                INFO:root:TESTING USER 2
+                INFO:root:<Page 0>
+                    <Label Hello, world! - default: None>
+                        test response: None
+                    test direction: 'forward'
+                INFO:root:<Page 1 terminal>
+                INFO:root:FINISHED TESTING USER 2
+        """
+        user_kwargs = dict(user_kwargs or {})
+        user_kwargs["seed_func"] = seed_func
+        test_kwargs = dict(test_kwargs or {})
+        test_kwargs.setdefault("verbosity", 1)
+
+        for _ in range(n_users):
+            user = cls.make_test_user(**user_kwargs)
+            logging.info(f"TESTING USER {user.id}")
+            user.test(**test_kwargs)
+            logging.info(f"FINISHED TESTING USER {user.id}\n")
+
+    def test(
+        self, url_rule: str = None, verbosity: int = 2, max_page_visits: int = 10
+    ) -> None:
+        """Run the test user through the entire study.
+
+        Args:
+            url_rule (str, optional): URL rule to test. Defaults to None.
+            verbosity (int, optional): Verbosity 0 gives no output. Verbosity 1
+                displays pages and test responses as text. Verbosity 2 additionally
+                displays the navigation graph and pages as HTML. Defaults to 2.
+            max_page_visits (int, optional): Maximum number of times the user can visit
+                the same page before an error is raised. Defaults to 10.
+
+        Raises:
+            RuntimeError: If the user visits the same page more times than allowed.
+                Likely causes include validate functions that always return False and
+                infinite loops.
+
+        Examples:
+
+            .. code-block::
+
+                >>> from hemlock import User, Page, create_test_app
+                >>> from hemlock.questions import Label
+                >>> def seed():
+                ...     return [
+                ...         Page(
+                ...             Label("Hello, world!")
+                ...         ),
+                ...         Page()
+                ...     ]
+                ...
+                >>> app = create_test_app()
+                >>> User.make_test_user(seed).test(verbosity=1)
+                INFO:root:<Page 0>
+                    <Label Hello, world! - default: None>
+                        test response: None
+                    test direction: 'forward'
+                INFO:root:<Page 1 terminal>
+        """
+        page_visits: defaultdict[str, int] = defaultdict(int)
+
+        tree = self.test_get(url_rule=url_rule)
+        page_visits[tree.page.get_position()] += 1
+        if verbosity == 2:
+            tree.display()
+
+        while not tree.page.is_last_page:
+            tree = self.test_request(url_rule=url_rule, verbose=verbosity >= 1)
+            page_visits[tree.page.get_position()] += 1
+            if page_visits[tree.page.get_position()] > max_page_visits:
+                raise RuntimeError(
+                    f"The test user has visited the same page more than {max_page_visits} times."
+                    " Check that your validate functions don't always return False"
+                    " and that your survey doesn't contain an infinite loop."
+                    " The page is\n{tree.page}"
+                )
+            if verbosity == 2:
+                tree.display()
+
+        if verbosity >= 1:
+            logging.info(tree.page.print())
+
+    def test_request(
+        self,
+        responses: ResponsesType = None,
+        direction: str = None,
+        url_rule: str = None,
+        **kwargs,
+    ) -> Tree:
+        """Test a request.
+
+        This simulates posting responses for the current page and getting the next page.
+
+        Args:
+            responses (ResponsesType, optional): Test responses. Defaults to None.
+            direction (str, optional): Requested direction. Defaults to "forward".
+            url_rule (str, optional): URL rule of the request. Defaults to None.
+            **kwargs (Any): Passed to :meth:`User.test_post`.
+
+        Returns:
+            Tree: Tree associated with the URL rule.
+        """
+        self.test_post(
+            responses=responses, direction=direction, url_rule=url_rule, **kwargs
+        )
+        return self.test_get(url_rule)
+
+    def test_get(self, url_rule: str = None) -> Tree:
+        """Test a get request.
+
+        Args:
+            url_rule (str, optional): URL rule of the request. Defaults to None.
+
+        Returns:
+            Tree: Tree associated with the URL rule.
+        """
+        url_rule = url_rule or self.default_url_rule
+        with current_app.test_request_context():
+            login_user(self)
+            self.process_request(url_rule)  # type: ignore
+        return self.get_tree(url_rule)
+
+    def test_post(
+        self,
+        responses: ResponsesType = None,
+        direction: str = None,
+        url_rule: str = None,
+        verbose: bool = True,
+    ) -> Tree:
+        """Test a post request.
+
+        Args:
+            responses (ResponsesType, optional): Test responses. Defaults to None.
+            direction (str, optional): Requested direction. Defaults to "forward".
+            url_rule (str, optional): URL rule of the request. Defaults to None.
+            verbose (bool, optional): When True, logs the current page and responses.
+                Defaults to True.
+
+        Returns:
+            Tree: Tree associated with the URL rule.
+        """
+        url_rule = url_rule or self.default_url_rule
+        tree = self.get_tree(url_rule)
+        page = tree.page
+
+        # collect manually input responses
+        if responses is None:
+            responses = {}
+        elif isinstance(responses, (list, tuple)):
+            if len(page.questions) != len(responses):
+                raise ValueError(
+                    "Number of responses does not match number of questions\n"
+                    f"Responses: {responses}\n"
+                    f"Page: {page}"
+                )
+            responses = {
+                question: response
+                for question, response in zip(page.questions, responses)
+            }
+        elif isinstance(responses, Mapping):
+            responses = dict(responses)
+        else:
+            raise ValueError(
+                f"Responses should be a list, tuple, or mapping, got {repr(responses)}."
+            )
+
+        # add automatic responses
+        for question in page.questions:
+            if question not in responses:
+                if is_callable(question.test_response):
+                    responses[question] = question.test_response(question)
+                else:
+                    responses[question] = question.test_response
+
+        # convert responses to raw responses
+        data = {
+            question.hash: question.make_raw_test_response(response)
+            for question, response in responses.items()
+        }
+
+        # set the requested direction and page hash
+        if direction is None:
+            if is_callable(page.test_direction):
+                direction = page.test_direction(page)
+            else:
+                direction = page.test_direction
+        data["direction"] = direction
+        data["page-hash"] = page.hash
+
+        # log the page and planned responses
+        if verbose:
+            logging.info(page.print(responses, direction))
+
+        with current_app.test_request_context(method="POST", data=data):
+            login_user(self)
+            self.process_request(url_rule)  # type: ignore
+        return tree
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/utils/__init__.py` & `hemlock-survey-1.0.1/src/hemlock/utils/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""Utilities.
-"""
-from __future__ import annotations
-
-import os
-import subprocess
-from typing import Any
-
-import flask
-from flask import request
-from werkzeug.wrappers.response import Response
-
-
-def redirect(location: str, *args: Any, **kwargs: Any) -> Response:
-    """Custom redirect for compatibility with Gitpod.
-
-    Replace `flask.redirect` with this function.
-
-    Args:
-        location (str): Original redirect URL.
-        *args (Any): Passed to `flask.redirect`.
-        **kwargs (Any): Passed to `flask.redirect`.
-
-    Returns:
-        Response: Redirect response.
-    """
-    if (
-        location.startswith("/")
-        and "GITPOD_HOST" in os.environ
-        and os.environ.get("VS_CODE_REMOTE", "False").lower() != "true"
-    ):  # pragma: no cover
-        # change URL root to gitpod workspace url
-        url_root = request.url_root
-        if "http" in url_root:
-            url_root = url_root.lstrip("http://")
-
-        index = url_root.index(":") + 1
-        port = url_root[index : index + 4]  # port is the 4 numbers after ":"
-        gp_url_port = subprocess.check_output(f"gp url {port}", shell=True)
-        location = gp_url_port.decode("utf-8").strip() + location
-
-    return flask.redirect(location, *args, **kwargs)
+"""Utilities.
+"""
+from __future__ import annotations
+
+import os
+import subprocess
+from typing import Any
+
+import flask
+from flask import request
+from werkzeug.wrappers.response import Response
+
+
+def redirect(location: str, *args: Any, **kwargs: Any) -> Response:
+    """Custom redirect for compatibility with Gitpod.
+
+    Replace `flask.redirect` with this function.
+
+    Args:
+        location (str): Original redirect URL.
+        *args (Any): Passed to `flask.redirect`.
+        **kwargs (Any): Passed to `flask.redirect`.
+
+    Returns:
+        Response: Redirect response.
+    """
+    if (
+        location.startswith("/")
+        and "GITPOD_HOST" in os.environ
+        and os.environ.get("VS_CODE_REMOTE", "False").lower() != "true"
+    ):  # pragma: no cover
+        # change URL root to gitpod workspace url
+        url_root = request.url_root
+        if "http" in url_root:
+            url_root = url_root.lstrip("http://")
+
+        index = url_root.index(":") + 1
+        port = url_root[index : index + 4]  # port is the 4 numbers after ":"
+        gp_url_port = subprocess.check_output(f"gp url {port}", shell=True)
+        location = gp_url_port.decode("utf-8").strip() + location
+
+    return flask.redirect(location, *args, **kwargs)
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/utils/format.py` & `hemlock-survey-1.0.1/src/hemlock/utils/format.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""Utilities for formatting text.
-"""
-from __future__ import annotations
-
-from markdown import markdown  # type: ignore
-
-
-def convert_markdown(value: str, strip_last_paragraph: bool = False) -> str:
-    """Convert markdown to HTML.
-
-    Args:
-        value (str): Raw markdown.
-        strip_last_paragraph (bool, optional): Strip the ``<p>`` tag from the last
-        paragraph. This improves the look for label questions. Defaults to False.
-
-    Returns:
-        str: HTML.
-    """
-    if not strip_last_paragraph:
-        return markdown(value)
-
-    # remove single newline white spaces
-    lines = value.splitlines()
-    new_line, new_lines = [], []
-    for line in lines:
-        if line:
-            new_line.append(line)
-        else:
-            new_lines.append(" ".join(new_line))
-            new_line.clear()
-    new_lines.append(" ".join(new_line))
-    value = "\n\n".join(new_lines)
-
-    # remove <p> tag from last line of HTML
-    lines = markdown(value).splitlines()
-    if lines[-1].startswith("<p>"):
-        lines[-1] = lines[-1][len("<p>") : -len("</p>")]
-    return "\n".join(lines)
-
-
-def plural(number: float, singular_form: str, plural_form: str = None) -> str:
-    """Make a word singular or plural depending on the quantity.
-
-    Args:
-        number (float): Number of things.
-        singular_form (str): Singular form of the word.
-        plural_form (str, optional): Plural form of the word. Defaults to None.
-
-    Returns:
-        str: Singular or plural form of the word.
-
-    Examples:
-
-        .. doctest::
-
-            >>> from hemlock.utils.format import plural
-            >>> plural(1, "dollar")
-            'dollar'
-            >>> plural(2, "dollar")
-            'dollars'
-            >>> plural(2, "octopus", "octopodes")
-            'octopodes'
-    """
-    if number == 1:
-        return singular_form
-
-    return f"{singular_form}s" if plural_form is None else plural_form
+"""Utilities for formatting text.
+"""
+from __future__ import annotations
+
+from markdown import markdown  # type: ignore
+
+
+def convert_markdown(value: str, strip_last_paragraph: bool = False) -> str:
+    """Convert markdown to HTML.
+
+    Args:
+        value (str): Raw markdown.
+        strip_last_paragraph (bool, optional): Strip the ``<p>`` tag from the last
+        paragraph. This improves the look for label questions. Defaults to False.
+
+    Returns:
+        str: HTML.
+    """
+    if not strip_last_paragraph:
+        return markdown(value)
+
+    # remove single newline white spaces
+    lines = value.splitlines()
+    new_line, new_lines = [], []
+    for line in lines:
+        if line:
+            new_line.append(line)
+        else:
+            new_lines.append(" ".join(new_line))
+            new_line.clear()
+    new_lines.append(" ".join(new_line))
+    value = "\n\n".join(new_lines)
+
+    # remove <p> tag from last line of HTML
+    lines = markdown(value).splitlines()
+    if lines[-1].startswith("<p>"):
+        lines[-1] = lines[-1][len("<p>") : -len("</p>")]
+    return "\n".join(lines)
+
+
+def plural(number: float, singular_form: str, plural_form: str = None) -> str:
+    """Make a word singular or plural depending on the quantity.
+
+    Args:
+        number (float): Number of things.
+        singular_form (str): Singular form of the word.
+        plural_form (str, optional): Plural form of the word. Defaults to None.
+
+    Returns:
+        str: Singular or plural form of the word.
+
+    Examples:
+
+        .. doctest::
+
+            >>> from hemlock.utils.format import plural
+            >>> plural(1, "dollar")
+            'dollar'
+            >>> plural(2, "dollar")
+            'dollars'
+            >>> plural(2, "octopus", "octopodes")
+            'octopodes'
+    """
+    if number == 1:
+        return singular_form
+
+    return f"{singular_form}s" if plural_form is None else plural_form
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/utils/random.py` & `hemlock-survey-1.0.1/src/hemlock/utils/random.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,145 @@
-"""Randomization.
-"""
-from __future__ import annotations
-
-from itertools import product
-from random import choice, choices
-from string import digits, ascii_letters
-from typing import TYPE_CHECKING, Any, Mapping
-
-import numpy as np
-import pandas as pd
-from flask_login import current_user
-
-if TYPE_CHECKING:
-    from ..user import User
-
-CHARACTERS = digits + ascii_letters
-
-
-def make_hash(length: int = 10) -> str:
-    """Make a random hash (can be used as HTML tag id).
-
-    Args:
-        length (int, optional): Length of the hash. Defaults to 10.
-
-    Returns:
-        str: Hash.
-    """
-    # the first character must be a letter to be a valid HTML tag id
-    return f"{choice(ascii_letters)}{''.join(choices(CHARACTERS, k=length-1))}"
-
-
-class Assigner:
-    """Random assigner.
-
-    Args:
-        conditions (Mapping): Maps factor names to possible factor values.
-
-    Attributes:
-        factor_names (list): Factor names.
-        possible_assignments (list[tuple]): Possible factor values to which users may be assigned.
-
-    Examples:
-
-        .. code-block::
-
-            >>> from hemlock import User, Page, create_test_app
-            >>> from hemlock.utils.random import Assigner
-            >>> assigner = Assigner(
-            ...     {"factor0": (0, 1), "factor1": ("low", "medium", "high")}
-            ... )
-            >>> def seed():
-            ...     assignment = assigner.assign_user()
-            ...     print("This user was assigned to conditions", assignment)
-            ...     return Page()
-            ...
-            >>> app = create_test_app()
-            >>> user = User.make_test_user(seed)
-            This user was assigned to conditions {'factor0': 1, 'factor1': 'high'}
-            >>> # the user's conditions are automatically stored in their metadata
-            >>> user.get_meta_data()["factor0"], user.get_meta_data()["factor1"]
-            (1, 'high')
-    """
-
-    def __init__(self, conditions: Mapping):
-        conditions = dict(conditions)
-        self.factor_names: list = list(conditions.keys())
-        self.possible_assignments: list[tuple] = list(product(*conditions.values()))
-
-    def _decode_numpy(self, value: Any) -> Any:
-        """Converts numpy values for JSON serialization.
-
-        Args:
-            value (Any): Value to be decoded.
-
-        Returns:
-            Any: Decoded value.
-        """
-        if isinstance(value, np.integer):
-            return int(value)
-        if isinstance(value, np.ndarray):
-            return list(value)
-        return value
-
-    def assign_user(self, user: User = None, df: pd.DataFrame = None) -> dict[Any, Any]:
-        """Assign a user to conditions.
-
-        Args:
-            user (User, optional): User to assign. If None, this method assigns the
-                current user. Defaults to None.
-            df (pd.DataFrame, optional): Passed to `:meth:Assigner.get_cum_assigned`.
-
-        Returns:
-            dict[Any, Any]: Maps factor names to assignment values.
-        """
-        if user is None:
-            user = current_user
-
-        # randomly select a condition with the fewest users
-        cum_assigned = self.get_cum_assigned(df)
-        values = (
-            cum_assigned[cum_assigned["count"] == cum_assigned["count"].min()]
-            .sample()
-            .index[0]
-        )
-        if len(self.factor_names) == 1:
-            values = [values]
-        assignment = {
-            key: self._decode_numpy(value)
-            for key, value in zip(self.factor_names, values)
-        }
-        user.meta_data.update(assignment)
-        return assignment
-
-    def get_cum_assigned(self, df: pd.DataFrame = None) -> pd.DataFrame:
-        """Get cumulative number of users assigned to each condition.
-
-        Args:
-            df (pd.DataFrame, optional): Dataframe of user data. If None, uses the
-                `:class:hemlock.user.User` metdata. Defaults to None.
-
-        Returns:
-            pd.DataFrame: Cumulative number of users in each condition.
-        """
-        if df is None:
-            from ..user import User
-
-            df = pd.DataFrame([user.get_meta_data() for user in User.query.all()])
-
-        if len(self.factor_names) == 1:
-            index = [value[0] for value in self.possible_assignments]
-        else:
-            index = pd.MultiIndex.from_tuples(
-                self.possible_assignments, names=self.factor_names
-            )
-
-        count_df = pd.DataFrame(index=index)
-        if len(df) > 0 and all([name in df for name in self.factor_names]):
-            count_df["count"] = df.groupby(self.factor_names)["id"].count()
-            count_df.fillna(0, inplace=True)
-        else:
-            count_df["count"] = 0
-
-        return count_df
+"""Randomization.
+"""
+from __future__ import annotations
+
+from itertools import product
+from random import choice, choices
+from string import digits, ascii_letters
+from typing import TYPE_CHECKING, Any, Mapping
+
+import numpy as np
+import pandas as pd
+from flask_login import current_user
+
+if TYPE_CHECKING:
+    from ..user import User
+
+CHARACTERS = digits + ascii_letters
+
+
+def make_hash(length: int = 10) -> str:
+    """Make a random hash (can be used as HTML tag id).
+
+    Args:
+        length (int, optional): Length of the hash. Defaults to 10.
+
+    Returns:
+        str: Hash.
+    """
+    # the first character must be a letter to be a valid HTML tag id
+    return f"{choice(ascii_letters)}{''.join(choices(CHARACTERS, k=length-1))}"
+
+
+class Assigner:
+    """Random assigner.
+
+    Args:
+        conditions (Mapping): Maps factor names to possible factor values.
+
+    Attributes:
+        factor_names (list): Factor names.
+        possible_assignments (list[tuple]): Possible factor values to which users may be assigned.
+
+    Examples:
+
+        .. code-block::
+
+            >>> from hemlock import User, Page, create_test_app
+            >>> from hemlock.utils.random import Assigner
+            >>> assigner = Assigner(
+            ...     {"factor0": (0, 1), "factor1": ("low", "medium", "high")}
+            ... )
+            >>> def seed():
+            ...     assignment = assigner.assign_user()
+            ...     print("This user was assigned to conditions", assignment)
+            ...     return Page()
+            ...
+            >>> app = create_test_app()
+            >>> user = User.make_test_user(seed)
+            This user was assigned to conditions {'factor0': 1, 'factor1': 'high'}
+            >>> # the user's conditions are automatically stored in their metadata
+            >>> user.get_meta_data()["factor0"], user.get_meta_data()["factor1"]
+            (1, 'high')
+    """
+
+    def __init__(self, conditions: Mapping):
+        conditions = dict(conditions)
+        self.factor_names: list = list(conditions.keys())
+        self.possible_assignments: list[tuple] = list(product(*conditions.values()))
+
+    def _decode_numpy(self, value: Any) -> Any:
+        """Converts numpy values for JSON serialization.
+
+        Args:
+            value (Any): Value to be decoded.
+
+        Returns:
+            Any: Decoded value.
+        """
+        if isinstance(value, np.integer):
+            return int(value)
+        if isinstance(value, np.ndarray):
+            return list(value)
+        return value
+
+    def assign_user(self, user: User = None, df: pd.DataFrame = None) -> dict[Any, Any]:
+        """Assign a user to conditions.
+
+        Args:
+            user (User, optional): User to assign. If None, this method assigns the
+                current user. Defaults to None.
+            df (pd.DataFrame, optional): Passed to `:meth:Assigner.get_cum_assigned`.
+
+        Returns:
+            dict[Any, Any]: Maps factor names to assignment values.
+        """
+        if user is None:
+            user = current_user
+
+        # randomly select a condition with the fewest users
+        cum_assigned = self.get_cum_assigned(df)
+        values = (
+            cum_assigned[cum_assigned["count"] == cum_assigned["count"].min()]
+            .sample()
+            .index[0]
+        )
+        if len(self.factor_names) == 1:
+            values = [values]
+        assignment = {
+            key: self._decode_numpy(value)
+            for key, value in zip(self.factor_names, values)
+        }
+        user.meta_data.update(assignment)
+        return assignment
+
+    def get_cum_assigned(self, df: pd.DataFrame = None) -> pd.DataFrame:
+        """Get cumulative number of users assigned to each condition.
+
+        Args:
+            df (pd.DataFrame, optional): Dataframe of user data. If None, uses the
+                :class:`hemlock.user.User` metdata. Defaults to None.
+
+        Returns:
+            pd.DataFrame: Cumulative number of users in each condition.
+        """
+        if df is None:
+            from ..user import User
+
+            df = pd.DataFrame([user.get_meta_data() for user in User.query.all()])
+
+        df = df.drop_duplicates(subset="id")
+        if len(self.factor_names) == 1:
+            index = [value[0] for value in self.possible_assignments]
+        else:
+            index = pd.MultiIndex.from_tuples(
+                self.possible_assignments, names=self.factor_names
+            )
+
+        count_df = pd.DataFrame(index=index)
+        if len(df) > 0 and all([name in df for name in self.factor_names]):
+            count_df["count"] = df.groupby(self.factor_names)["id"].count()
+            count_df.fillna(0, inplace=True)
+        else:
+            count_df["count"] = 0
+
+        return count_df
```

### Comparing `hemlock-survey-1.0.0/src/hemlock/utils/statics.py` & `hemlock-survey-1.0.1/src/hemlock/utils/statics.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-"""Tools for creating static objects.
-
-Static objects include figures, javascript, and HTML.
-"""
-from __future__ import annotations
-
-import warnings
-from typing import TYPE_CHECKING, Any, Dict
-
-import pandas as pd
-from flask import render_template
-from flask_socketio import emit
-
-from ..app import db, socketio
-
-if TYPE_CHECKING:
-    from ..questions.base import Question
-
-
-def make_figure(
-    src: str,
-    caption: str = None,
-    alt: str = "alt",
-    figure_align: str = "start",
-    caption_align: str = "start",
-    template: str = "hemlock/statics/figure.html",
-) -> str:
-    """Insert an figure.
-
-    Args:
-        src (str): Image URL.
-        caption (str, optional): Caption. Defaults to None.
-        alt (str, optional): Alternative text displayed if the image fails to load.
-            Defaults to "alt".
-        figure_align (str, optional): Figure alignment ("start", "center", "end").
-            Defaults to "start".
-        caption_align (str, optional): Caption alignment ("start", "center", "end").
-            Defaults to "start".
-        template (str, optional): Path to Jinja template. Defaults to
-            "hemlock/statics/img.html".
-
-    Returns:
-        str: Figure tag.
-
-    Examples:
-
-        .. code-block::
-
-            >>> from hemlock import create_test_app
-            >>> from hemlock.utils.statics import make_figure
-            >>> create_test_app()
-            >>> make_figure("https://link-to-image.html")
-    """
-    return render_template(
-        template,
-        src=src,
-        caption=caption,
-        alt=alt,
-        figure_align=figure_align,
-        caption_align=caption_align,
-    )
-
-
-def pandas_to_html(dataframe: pd.DataFrame, *args: Any, **kwargs: Any) -> str:
-    """Convert pandas dataframe to HTML.
-
-    While pandas dataframes have a built-in ``to_html`` method, it doesn't take
-    advantage of the additional stylings provided by hemlock pages.
-
-    Args:
-        dataframe (pd.DataFrame): Dataframe.
-        *args (Any): Passed to ``pd.DataFrame.to_html``.
-        **kwargs (Any): Passed to ``pd.DataFrame.to_html``.
-
-    Returns:
-        str: HTML.
-    """
-    default_kwargs = {
-        "classes": ["table", "table-striped", "table-hover"],
-        "border": 0,
-        "justify": "match-parent",
-    }
-    default_kwargs.update(kwargs)
-    return dataframe.to_html(*args, **default_kwargs)
-
-
-def recompile_at_interval(interval: int, question: "Question") -> "Question":
-    """Add javascript to recompile this question at regular intervals.
-
-    That is, at regular intervals, the question's compile functions will be rerun and
-    its HTML re-rendered for the user.
-
-    Args:
-        interval (int): Recompile interval (milliseconds).
-        question (Question): Question which should be recompiled.
-
-    Returns:
-        Question: Question from the arguments.
-    """
-    question.html_settings["js"] += [
-        {"src": "https://cdn.socket.io/4.2.0/socket.io.min.js"},
-        render_template(
-            "hemlock/statics/recompile_at_interval.js",
-            hash=question.hash,
-            interval=interval,
-        ),
-    ]
-    return question
-
-
-@socketio.on("recompile-question-event")
-def recompile_question(question_hash: Dict[str, str]) -> None:
-    """Rerun a question's compile functions.
-
-    Args:
-        question_hash (Dict[str, str]): Hash of the question to be recompiled
-            ({"data": question.hash}).
-    """
-    from ..questions.base import Question
-
-    hash = question_hash["data"]
-    question = Question.query.filter_by(hash=hash).first()
-    if question is None:
-        warnings.warn(f"Question with hash {hash} does not exist.", RuntimeWarning)
-        return None
-
-    question.run_compile_functions()
-    db.session.commit()
-    emit("recompile-question-response", {"data": question.render()})
+"""Tools for creating static objects.
+
+Static objects include figures, javascript, and HTML.
+"""
+from __future__ import annotations
+
+import warnings
+from typing import TYPE_CHECKING, Any, Dict
+
+import pandas as pd
+from flask import render_template
+from flask_socketio import emit
+
+from ..app import db, socketio
+
+if TYPE_CHECKING:
+    from ..questions.base import Question
+
+
+def make_figure(
+    src: str,
+    caption: str = None,
+    alt: str = "alt",
+    figure_align: str = "start",
+    caption_align: str = "start",
+    template: str = "hemlock/statics/figure.html",
+) -> str:
+    """Insert an figure.
+
+    Args:
+        src (str): Image URL.
+        caption (str, optional): Caption. Defaults to None.
+        alt (str, optional): Alternative text displayed if the image fails to load.
+            Defaults to "alt".
+        figure_align (str, optional): Figure alignment ("start", "center", "end").
+            Defaults to "start".
+        caption_align (str, optional): Caption alignment ("start", "center", "end").
+            Defaults to "start".
+        template (str, optional): Path to Jinja template. Defaults to
+            "hemlock/statics/img.html".
+
+    Returns:
+        str: Figure tag.
+
+    Examples:
+
+        .. code-block::
+
+            >>> from hemlock import create_test_app
+            >>> from hemlock.utils.statics import make_figure
+            >>> create_test_app()
+            >>> make_figure("https://link-to-image.html")
+    """
+    return render_template(
+        template,
+        src=src,
+        caption=caption,
+        alt=alt,
+        figure_align=figure_align,
+        caption_align=caption_align,
+    )
+
+
+def pandas_to_html(dataframe: pd.DataFrame, *args: Any, **kwargs: Any) -> str:
+    """Convert pandas dataframe to HTML.
+
+    While pandas dataframes have a built-in ``to_html`` method, it doesn't take
+    advantage of the additional stylings provided by hemlock pages.
+
+    Args:
+        dataframe (pd.DataFrame): Dataframe.
+        *args (Any): Passed to ``pd.DataFrame.to_html``.
+        **kwargs (Any): Passed to ``pd.DataFrame.to_html``.
+
+    Returns:
+        str: HTML.
+    """
+    default_kwargs = {
+        "classes": ["table", "table-striped", "table-hover"],
+        "border": 0,
+        "justify": "match-parent",
+    }
+    default_kwargs.update(kwargs)
+    return dataframe.to_html(*args, **default_kwargs)
+
+
+def recompile_at_interval(interval: int, question: "Question") -> "Question":
+    """Add javascript to recompile this question at regular intervals.
+
+    That is, at regular intervals, the question's compile functions will be rerun and
+    its HTML re-rendered for the user.
+
+    Args:
+        interval (int): Recompile interval (milliseconds).
+        question (Question): Question which should be recompiled.
+
+    Returns:
+        Question: Question from the arguments.
+    """
+    question.html_settings["js"] += [
+        {"src": "https://cdn.socket.io/4.2.0/socket.io.min.js"},
+        render_template(
+            "hemlock/statics/recompile_at_interval.js",
+            hash=question.hash,
+            interval=interval,
+        ),
+    ]
+    return question
+
+
+@socketio.on("recompile-question-event")
+def recompile_question(question_hash: Dict[str, str]) -> None:
+    """Rerun a question's compile functions.
+
+    Args:
+        question_hash (Dict[str, str]): Hash of the question to be recompiled
+            ({"data": question.hash}).
+    """
+    from ..questions.base import Question
+
+    hash = question_hash["data"]
+    question = Question.query.filter_by(hash=hash).first()
+    if question is None:
+        warnings.warn(f"Question with hash {hash} does not exist.", RuntimeWarning)
+        return None
+
+    question.run_compile_functions()
+    db.session.commit()
+    emit("recompile-question-response", {"data": question.render()})
```

### Comparing `hemlock-survey-1.0.0/src/hemlock_survey.egg-info/PKG-INFO` & `hemlock-survey-1.0.1/src/hemlock_survey.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1
-Name: hemlock-survey
-Version: 1.0.0
-Summary: A python framework for creating online surveys and experiments.
-Home-page: https://dsbowen.gitlab.io/hemlock
-Author: Dillon Bowen
-Author-email: dsbowen@wharton.upenn.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hemlock
-
-[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
-[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
-<!-- [![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE) -->
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
-
-
+Metadata-Version: 2.1
+Name: hemlock-survey
+Version: 1.0.1
+Summary: A python framework for creating online surveys and experiments.
+Home-page: https://dsbowen.gitlab.io/hemlock
+Author: Dillon Bowen
+Author-email: dsbowen@wharton.upenn.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hemlock
+
+[![pipeline status](https://gitlab.com/dsbowen/hemlock/badges/master/pipeline.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![coverage report](https://gitlab.com/dsbowen/hemlock/badges/master/coverage.svg)](https://gitlab.com/dsbowen/hemlock/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/hemlock-survey.svg)](https://badge.fury.io/py/hemlock)
+[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://gitlab.com/dsbowen/hemlock/-/blob/master/LICENSE)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/dsbowen%2Fhemlock/HEAD?urlpath=lab/tree/examples)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A framework for creating online surveys and experiments. [Read the docs](https://dsbowen.gitlab.io/hemlock).
```

### Comparing `hemlock-survey-1.0.0/src/hemlock_survey.egg-info/SOURCES.txt` & `hemlock-survey-1.0.1/src/hemlock_survey.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -57,8 +57,20 @@
 src/hemlock/utils/format.py
 src/hemlock/utils/random.py
 src/hemlock/utils/statics.py
 src/hemlock_survey.egg-info/PKG-INFO
 src/hemlock_survey.egg-info/SOURCES.txt
 src/hemlock_survey.egg-info/dependency_links.txt
 src/hemlock_survey.egg-info/requires.txt
-src/hemlock_survey.egg-info/top_level.txt
+src/hemlock_survey.egg-info/top_level.txt
+tests/test__admin_routes.py
+tests/test__data_frame.py
+tests/test__display_navigation.py
+tests/test__navbar.py
+tests/test__user_routes.py
+tests/test_admin_route_utils.py
+tests/test_app.py
+tests/test_data.py
+tests/test_page.py
+tests/test_timer.py
+tests/test_tree.py
+tests/test_user.py
```

