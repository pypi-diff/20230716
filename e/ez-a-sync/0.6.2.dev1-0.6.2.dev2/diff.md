# Comparing `tmp/ez-a-sync-0.6.2.dev1.tar.gz` & `tmp/ez-a-sync-0.6.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.6.2.dev1.tar", last modified: Fri Jul 14 22:11:30 2023, max compression
+gzip compressed data, was "ez-a-sync-0.6.2.dev2.tar", last modified: Sun Jul 16 17:19:58 2023, max compression
```

## Comparing `ez-a-sync-0.6.2.dev1.tar` & `ez-a-sync-0.6.2.dev2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.801978 ez-a-sync-0.6.2.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.793978 ez-a-sync-0.6.2.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-14 22:11:30.801978 ez-a-sync-0.6.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     6362 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/prio_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.797978 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-14 22:11:30.000000 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-14 22:11:30.000000 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 22:11:30.000000 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-14 22:11:30.000000 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-14 22:11:30.000000 ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 22:11:30.801978 ez-a-sync-0.6.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:30.801978 ez-a-sync-0.6.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-14 22:11:17.000000 ez-a-sync-0.6.2.dev1/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.279464 ez-a-sync-0.6.2.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.263463 ez-a-sync-0.6.2.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.267463 ez-a-sync-0.6.2.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-16 17:19:58.279464 ez-a-sync-0.6.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/TODO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.271463 ez-a-sync-0.6.2.dev2/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4982 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.271463 ez-a-sync-0.6.2.dev2/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.275463 ez-a-sync-0.6.2.dev2/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.275463 ez-a-sync-0.6.2.dev2/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7252 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.275463 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.279464 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-16 17:19:58.000000 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-16 17:19:58.000000 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 17:19:58.000000 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-16 17:19:58.000000 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-16 17:19:58.000000 ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-16 17:19:58.279464 ez-a-sync-0.6.2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:58.279464 ez-a-sync-0.6.2.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-07-16 17:19:45.000000 ez-a-sync-0.6.2.dev2/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.6.2.dev1/.github/workflows/codeql.yaml` & `ez-a-sync-0.6.2.dev2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/.github/workflows/mypy.yaml` & `ez-a-sync-0.6.2.dev2/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/.github/workflows/pytest.yaml` & `ez-a-sync-0.6.2.dev2/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/.github/workflows/release.yaml` & `ez-a-sync-0.6.2.dev2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/LICENSE.txt` & `ez-a-sync-0.6.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/README.md` & `ez-a-sync-0.6.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/__init__.py` & `ez-a-sync-0.6.2.dev2/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_bound.py` & `ez-a-sync-0.6.2.dev2/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_flags.py` & `ez-a-sync-0.6.2.dev2/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_helpers.py` & `ez-a-sync-0.6.2.dev2/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_kwargs.py` & `ez-a-sync-0.6.2.dev2/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_meta.py` & `ez-a-sync-0.6.2.dev2/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/_typing.py` & `ez-a-sync-0.6.2.dev2/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/abstract.py` & `ez-a-sync-0.6.2.dev2/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/base.py` & `ez-a-sync-0.6.2.dev2/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/config.py` & `ez-a-sync-0.6.2.dev2/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/decorator.py` & `ez-a-sync-0.6.2.dev2/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/exceptions.py` & `ez-a-sync-0.6.2.dev2/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modified.py` & `ez-a-sync-0.6.2.dev2/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/__init__.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/limiter.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/manager.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.6.2.dev2/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/_debug.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/executor.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/counter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/event.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/prio_semaphore.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/prio_semaphore.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             manager._wake_up_next()
             if len(manager):
                 # There are still waiters, put the manager back
                 heapq.heappush(self._waiters, manager)  # type: ignore [misc]
             else:
                 # There are no more waiters, get rid of the empty manager
                 self._context_managers.pop(manager._priority)
-            break
+            return
         logger.debug("%s has no waiters to wake", self)
 
 class _AbstractPrioritySemaphoreContextManager(Semaphore, Generic[PT]):
     _loop: asyncio.AbstractEventLoop
     _waiters: List[asyncio.Future]  # type: ignore [assignment]
     
     @property
```

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.6.2.dev2/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/a_sync/property.py` & `ez-a-sync-0.6.2.dev2/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.6.2.dev2/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/setup.py` & `ez-a-sync-0.6.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/fixtures.py` & `ez-a-sync-0.6.2.dev2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_base.py` & `ez-a-sync-0.6.2.dev2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_cache.py` & `ez-a-sync-0.6.2.dev2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_decorator.py` & `ez-a-sync-0.6.2.dev2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_executor.py` & `ez-a-sync-0.6.2.dev2/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_limiter.py` & `ez-a-sync-0.6.2.dev2/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_meta.py` & `ez-a-sync-0.6.2.dev2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.6.2.dev1/tests/test_semaphore.py` & `ez-a-sync-0.6.2.dev2/tests/test_semaphore.py`

 * *Files identical despite different names*
