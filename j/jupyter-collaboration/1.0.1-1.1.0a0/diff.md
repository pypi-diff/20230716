# Comparing `tmp/jupyter_collaboration-1.0.1.tar.gz` & `tmp/jupyter_collaboration-1.1.0a0.tar.gz`

## Comparing `jupyter_collaboration-1.0.1.tar` & `jupyter_collaboration-1.1.0a0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.eslintrc.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.gitconfig
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.licenserc.yaml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.npmignore
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.prettierrc
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.yarnrc.yml
--rw-r--r--   0        0        0    45733 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/install.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/lerna.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/package.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/setup.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tsconfig.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tsconfig.test.json
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/typedoc.json
--rw-r--r--   0        0        0   488218 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/yarn.lock
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/make.bat
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/configuration.md
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/index.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/architecture.md
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/contributing.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/javascript_api.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/developer/python_api.rst
--rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/docs/source/images/rtc_shared_cursors.png
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter-config/jupyter_collaboration.json
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/_version.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/app.py
--rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/handlers.py
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/loaders.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/rooms.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/stores.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/utils.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/websocketserver.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/events/session.yaml
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/package.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/252.856eca7b3cd3748103bd.js
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/299.40530f9f1ff8893867f0.js
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js
--rw-r--r--   0        0        0    11293 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/760.44dd9522edcf2585c0a2.js
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
--rw-r--r--   0        0        0    10890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/87.a9066e8e77b73733ee8e.js
--rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/remoteEntry.63a4bd8fd0be235c05a7.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/style.js
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/scripts/bump_version.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/tests/test_loaders.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/README.md
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/LICENSE
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/README.md
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.eslintrc.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.gitconfig
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.licenserc.yaml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.npmignore
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.prettierrc
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.readthedocs.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.yarnrc.yml
+-rw-r--r--   0        0        0    46722 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/RELEASE.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/codecov.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/install.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/lerna.json
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/package.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/setup.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/tsconfig.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/tsconfig.test.json
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/typedoc.json
+-rw-r--r--   0        0        0   488258 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/yarn.lock
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/make.bat
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/configuration.md
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/index.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/developer/contributing.rst
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/developer/javascript_api.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/developer/python_api.rst
+-rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/docs/source/images/rtc_shared_cursors.png
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter-config/jupyter_collaboration.json
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/_version.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/app.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/handlers.py
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/loaders.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/rooms.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/stores.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/utils.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/websocketserver.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/events/session.yaml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/package.json
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/252.d0c7151db0dbf630fd66.js
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/299.e6bd576db486fa2a916e.js
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/760.b5d1c9daae2954d25258.js
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js
+-rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/87.4c5b9b62b8fcc0e00e87.js
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/remoteEntry.e96a4d758c0ec06bbfda.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/style.js
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/scripts/bump_version.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/tests/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/tests/conftest.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/tests/test_loaders.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/README.md
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/sharedlink.ts
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/schema/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/sharedlink.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/README.md
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyter_collaboration-1.1.0a0/PKG-INFO
```

### Comparing `jupyter_collaboration-1.0.1/.eslintrc.js` & `jupyter_collaboration-1.1.0a0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/.licenserc.yaml` & `jupyter_collaboration-1.1.0a0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/.pre-commit-config.yaml` & `jupyter_collaboration-1.1.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/CHANGELOG.md` & `jupyter_collaboration-1.1.0a0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.1.0alpha0
+
+([Full Changelog](https://github.com/jupyterlab/jupyter-collaboration/compare/v1.0.1...7240ef0e0a7ba437c04a7779a903f4eba62cee91))
+
+### Enhancements made
+
+- Backport #177: Adds a flag to disable RTC [#178](https://github.com/jupyterlab/jupyter-collaboration/pull/178) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter-collaboration/graphs/contributors?from=2023-06-29&to=2023-07-16&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Agithub-actions+updated%3A2023-06-29..2023-07-16&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Ahbcarlos+updated%3A2023-06-29..2023-07-16&type=Issues) | [@SylvainCorlay](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3ASylvainCorlay+updated%3A2023-06-29..2023-07-16&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.1
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter-collaboration/compare/@jupyter/collaboration-extension@1.0.0...e97855f7ad4160cc4e6f5dbe9361806d6b9f3c31))
 
 ### Enhancements made
 
 - Support ypy-websocket v0.12 [#168](https://github.com/jupyterlab/jupyter-collaboration/pull/168) ([@davidbrochart](https://github.com/davidbrochart))
@@ -26,16 +42,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter-collaboration/graphs/contributors?from=2023-06-02&to=2023-06-29&type=c))
 
 [@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Acodecov-commenter+updated%3A2023-06-02..2023-06-29&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Adavidbrochart+updated%3A2023-06-02..2023-06-29&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Afcollonval+updated%3A2023-06-02..2023-06-29&type=Issues) | [@fperez](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Afperez+updated%3A2023-06-02..2023-06-29&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Agithub-actions+updated%3A2023-06-02..2023-06-29&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter-collaboration+involves%3Ahbcarlos+updated%3A2023-06-02..2023-06-29&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.9...4da43013daa89869035d77417971a80143b0ac61))
 
 ### Maintenance and upkeep improvements
 
 - Remove spurious `'` [#156](https://github.com/jupyterlab/jupyter_collaboration/pull/156) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyter_collaboration-1.0.1/package.json` & `jupyter_collaboration-1.1.0a0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -59,14 +59,14 @@
         "stylelint:check": "stylelint --cache \"packages/**/style/**/*.css\"",
         "test": "lerna run test",
         "test:cov": "lerna run test:cov",
         "test:debug": "lerna run test:debug",
         "test:debug:watch": "lerna run test:debug:watch",
         "watch": "lerna run watch"
     },
-    "version": "1.0.1",
+    "version": "1.1.0-alpha.0",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyter_collaboration-1.0.1/typedoc.json` & `jupyter_collaboration-1.1.0a0/typedoc.json`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/yarn.lock` & `jupyter_collaboration-1.1.0a0/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2015,16 +2015,16 @@
   languageName: node
   linkType: hard
 
 "@jupyter/collaboration-extension@workspace:packages/collaboration-extension":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration-extension@workspace:packages/collaboration-extension"
   dependencies:
-    "@jupyter/collaboration": ^1.0.1
-    "@jupyter/docprovider": ^1.0.1
+    "@jupyter/collaboration": ^1.1.0-alpha.0
+    "@jupyter/docprovider": ^1.1.0-alpha.0
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/codemirror": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
@@ -2044,21 +2044,21 @@
     typescript: ~5.0.4
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/collaboration@^1.0.1, @jupyter/collaboration@workspace:packages/collaboration":
+"@jupyter/collaboration@^1.1.0-alpha.0, @jupyter/collaboration@workspace:packages/collaboration":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration@workspace:packages/collaboration"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.7.0
-    "@jupyter/docprovider": ^1.0.1
+    "@jupyter/docprovider": ^1.1.0-alpha.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.1.0
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.0
@@ -2067,15 +2067,15 @@
     rimraf: ^4.1.2
     typescript: ~5.0.4
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/docprovider@^1.0.1, @jupyter/docprovider@workspace:packages/docprovider":
+"@jupyter/docprovider@^1.1.0-alpha.0, @jupyter/docprovider@workspace:packages/docprovider":
   version: 0.0.0-use.local
   resolution: "@jupyter/docprovider@workspace:packages/docprovider"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/testing": ^4.0.0
```

### Comparing `jupyter_collaboration-1.0.1/docs/Makefile` & `jupyter_collaboration-1.1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/make.bat` & `jupyter_collaboration-1.1.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/conf.py` & `jupyter_collaboration-1.1.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/configuration.md` & `jupyter_collaboration-1.1.0a0/docs/source/configuration.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/index.md` & `jupyter_collaboration-1.1.0a0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/_static/jupyter_logo.svg` & `jupyter_collaboration-1.1.0a0/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/_static/logo-icon.png` & `jupyter_collaboration-1.1.0a0/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/developer/contributing.rst` & `jupyter_collaboration-1.1.0a0/docs/source/developer/contributing.rst`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/docs/source/images/rtc_shared_cursors.png` & `jupyter_collaboration-1.1.0a0/docs/source/images/rtc_shared_cursors.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/app.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 from __future__ import annotations
 
 import asyncio
 
 from jupyter_server.extension.application import ExtensionApp
-from traitlets import Float, Type
+from traitlets import Bool, Float, Type
 from ypy_websocket.ystore import BaseYStore
 
 from .handlers import DocSessionHandler, YDocWebSocketHandler
 from .loaders import FileLoaderMapping
 from .stores import SQLiteYStore
 from .utils import EVENTS_SCHEMA_PATH
 from .websocketserver import JupyterWebsocketServer
 
 
 class YDocExtension(ExtensionApp):
     name = "jupyter_collaboration"
+    app_name = "Collaboration"
+    description = """
+    Enables Real Time Collaboration in JupyterLab
+    """
+
+    disable_rtc = Bool(False, config=True, help="Whether to disable real time collaboration.")
 
     file_poll_interval = Float(
         1,
         config=True,
         help="""The period in seconds to check for file changes on disk.
         Defaults to 1s, if 0 then file changes will only be checked when
         saving changes from the front-end.""",
@@ -62,14 +68,18 @@
                 "collaborative_document_cleanup_delay": self.document_cleanup_delay,
                 "collaborative_document_save_delay": self.document_save_delay,
                 "collaborative_ystore_class": self.ystore_class,
             }
         )
 
     def initialize_handlers(self):
+        self.serverapp.web_app.settings.setdefault(
+            "page_config_data", {"disableRTC": self.disable_rtc}
+        )
+
         # Set configurable parameters to YStore class
         for k, v in self.config.get(self.ystore_class.__name__, {}).items():
             setattr(self.ystore_class, k, v)
 
         self.ywebsocket_server = JupyterWebsocketServer(
             rooms_ready=False,
             auto_clean_rooms=False,
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/handlers.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/loaders.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/rooms.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/rooms.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/stores.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/stores.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/utils.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/websocketserver.py` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/websocketserver.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/events/session.yaml` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/events/session.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/package.json` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758748196248196%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.1.0-alpha.0', '@jupyter/docprovider': "*

 * *                   "'^1.1.0-alpha.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e96a4d758c0ec06bbfda.js'}}",*

 * * "'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.1",
-        "@jupyter/docprovider": "^1.0.1",
+        "@jupyter/collaboration": "^1.1.0-alpha.0",
+        "@jupyter/docprovider": "^1.1.0-alpha.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -45,15 +45,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter_collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.63a4bd8fd0be235c05a7.js",
+            "load": "static/remoteEntry.e96a4d758c0ec06bbfda.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser"
         ],
         "extension": true,
         "outputDir": "../../jupyter_collaboration/labextension",
@@ -129,9 +129,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0-alpha.0"
 }
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.1.0-alpha.0', '@jupyter/docprovider': "*

 * *                   "'^1.1.0-alpha.0'}",*

 * * "'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.1",
-        "@jupyter/docprovider": "^1.0.1",
+        "@jupyter/collaboration": "^1.1.0-alpha.0",
+        "@jupyter/docprovider": "^1.1.0-alpha.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -124,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0-alpha.0"
 }
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/252.856eca7b3cd3748103bd.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/252.d0c7151db0dbf630fd66.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                     const s = i.Mf();
                     i.uE(s, o.CHAT), i.uw(s, e), this.ws.send(i._f(s))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(9993),
-                d = t(4238),
-                l = t(5350),
+            var h = t(5987),
+                d = t(2790),
+                l = t(3172),
                 _ = t(7930);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
@@ -107,14 +107,15 @@
                         awareness: this._awareness
                     }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
+            const u = "true" === h.PageConfig.getOption("disableRTC");
             class y extends d.Drive {
                 constructor(e, s) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, s) => {
                         if ("string" == typeof e.format) try {
                             const t = new p({
@@ -130,15 +131,15 @@
                             this._providers.set(o, t), s.disposed.connect((() => {
                                 const e = this._providers.get(o);
                                 e && (e.dispose(), this._providers.delete(o))
                             }))
                         } catch (s) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${s}`)
                         }
-                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new u(this._onCreate)
+                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new g(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
                 }
                 async get(e, s) {
                     if (s && s.format && s.type) {
                         const t = `${s.format}:${s.type}:${e}`,
@@ -160,25 +161,25 @@
                             ...s,
                             content: !1
                         })
                     }
                     return super.save(e, s)
                 }
             }
-            class u {
+            class g {
                 constructor(e) {
-                    this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
+                    this._onCreate = e, this.collaborative = !u, this._documentFactories = new Map
                 }
                 registerDocumentFactory(e, s) {
                     if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
                     this._documentFactories.set(e, s)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
-                        if (e.collaborative && this._documentFactories.has(e.contentType)) {
+                        if (this.collaborative && e.collaborative && this._documentFactories.has(e.contentType)) {
                             const s = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, s), s
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
             const v = new _.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/299.40530f9f1ff8893867f0.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/299.e6bd576db486fa2a916e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                     const s = i.Mf();
                     i.uE(s, o.CHAT), i.uw(s, e), this.ws.send(i._f(s))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(9993),
-                d = t(4238),
-                l = t(5350),
+            var h = t(5987),
+                d = t(2790),
+                l = t(3172),
                 _ = t(7930);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
@@ -107,14 +107,15 @@
                         awareness: this._awareness
                     }), this._yWebsocketProvider.on("sync", this._onSync), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
+            const u = "true" === h.PageConfig.getOption("disableRTC");
             class y extends d.Drive {
                 constructor(e, s) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, s) => {
                         if ("string" == typeof e.format) try {
                             const t = new p({
@@ -130,15 +131,15 @@
                             this._providers.set(o, t), s.disposed.connect((() => {
                                 const e = this._providers.get(o);
                                 e && (e.dispose(), this._providers.delete(o))
                             }))
                         } catch (s) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${s}`)
                         }
-                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new u(this._onCreate)
+                    }, this._user = e, this._trans = s, this._providers = new Map, this.sharedModelFactory = new g(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
                 }
                 async get(e, s) {
                     if (s && s.format && s.type) {
                         const t = `${s.format}:${s.type}:${e}`,
@@ -160,25 +161,25 @@
                             ...s,
                             content: !1
                         })
                     }
                     return super.save(e, s)
                 }
             }
-            class u {
+            class g {
                 constructor(e) {
-                    this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
+                    this._onCreate = e, this.collaborative = !u, this._documentFactories = new Map
                 }
                 registerDocumentFactory(e, s) {
                     if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
                     this._documentFactories.set(e, s)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
-                        if (e.collaborative && this._documentFactories.has(e.contentType)) {
+                        if (this.collaborative && e.collaborative && this._documentFactories.has(e.contentType)) {
                             const s = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, s), s
                         }
                     } else console.warn(`Only defined format are supported; got ${e.format}.`)
                 }
             }
             const v = new _.Token("@jupyter/collaboration-extension:ICollaborativeDrive")
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/413.c23fa684c321e1bc178c.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/760.44dd9522edcf2585c0a2.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/760.b5d1c9daae2954d25258.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 showSharedLinkDialog: () => L
             });
             var r = n(7930);
             const s = new r.Token("@jupyter/collaboration:IUserMenu"),
                 o = new r.Token("@jupyter/collaboration:IGlobalAwareness");
             var a = n(6029),
                 i = n(8778),
-                l = n(5350),
-                c = n(9993);
+                l = n(3172),
+                c = n(5987);
             const d = "jp-Collaborator";
             class u extends i.Panel {
                 constructor(e, t, n) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, n) => {
@@ -248,15 +248,15 @@
                         parent: document.body
                     })]
                 });
 
             function x(e) {
                 return [f.of(e), C]
             }
-            var j = n(2189),
+            var j = n(1580),
                 A = n(4059);
             class I extends i.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -292,15 +292,15 @@
                 }
             }
             class P extends i.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var E = n(926);
+            var E = n(5354);
             async function L({
                 translator: e
             }) {
                 const t = (null != e ? e : E.nullTranslator).load("collaboration"),
                     n = c.PageConfig.getToken(),
                     r = new URL(c.URLExt.normalize(c.PageConfig.getUrl({
                         workspace: c.PageConfig.defaultWorkspace
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/839.14d748171b9c87a422f9.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/87.a9066e8e77b73733ee8e.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/87.4c5b9b62b8fcc0e00e87.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -180,24 +180,24 @@
                     }, o])
                 }
         },
         5087: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => E
             });
-            var a, s = o(4163),
-                r = o(5350),
-                n = o(2164),
-                i = o(8486),
-                l = o(9350),
-                c = o(1919),
-                d = o(56),
-                u = o(926),
+            var a, s = o(4004),
+                r = o(3172),
+                n = o(6154),
+                i = o(7785),
+                l = o(42),
+                c = o(7861),
+                d = o(8663),
+                u = o(5354),
                 h = o(2293),
-                p = o(4822);
+                p = o(8027);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
             }(a || (a = {}));
             const g = {
                     id: "@jupyter/collaboration-extension:drive",
                     description: "The default collaborative drive provider",
                     provides: p.ICollaborativeDrive,
@@ -318,21 +318,21 @@
                             path: l.browser,
                             dontShowBrowser: !0
                         })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(n), (null == r ? void 0 : r.isEmpty("main")) && t.execute("launcher:create")
                     };
                     o.routed.connect(i)
                 }
             }(w || (w = {}));
-            var f = o(2927),
-                I = o(1255),
-                _ = o(2189),
+            var f = o(6408),
+                I = o(7349),
+                _ = o(1580),
                 S = o(8778),
-                k = o(9993),
-                x = o(4238),
-                D = o(1617),
+                k = o(5987),
+                x = o(2790),
+                D = o(3007),
                 M = o(981),
                 j = o(6493);
             const U = {
                     id: "@jupyter/collaboration-extension:userMenu",
                     description: "Provide connected user menu.",
                     requires: [],
                     provides: I.IUserMenu,
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/899.d8ce2a60114cd6e1ebea.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/remoteEntry.63a4bd8fd0be235c05a7.js` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/remoteEntry.e96a4d758c0ec06bbfda.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, f, d, c, s, p, b, h, v, y, m, g, j = {
-            6746: (e, r, t) => {
+    var e, r, t, a, o, n, l, i, u, f, d, c, s, p, b, h, v, y, m, g, j = {
+            5432: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(899), t.e(981), t.e(662), t.e(46), t.e(238), t.e(87)]).then((() => () => t(5087))),
-                        "./extension": () => Promise.all([t.e(899), t.e(981), t.e(662), t.e(46), t.e(238), t.e(87)]).then((() => () => t(5087))),
+                        "./index": () => Promise.all([t.e(899), t.e(981), t.e(738), t.e(80), t.e(790), t.e(87)]).then((() => () => t(5087))),
+                        "./extension": () => Promise.all([t.e(899), t.e(981), t.e(738), t.e(80), t.e(790), t.e(87)]).then((() => () => t(5087))),
                         "./style": () => t.e(839).then((() => () => t(8839)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,71 +43,71 @@
         }), r
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
-        46: "208d560cd92dfb43b720",
-        87: "a9066e8e77b73733ee8e",
-        238: "86e88a3059c9a5a0803f",
-        252: "856eca7b3cd3748103bd",
-        299: "40530f9f1ff8893867f0",
+        80: "bfe2ae9640edadf1b2bf",
+        87: "4c5b9b62b8fcc0e00e87",
+        252: "d0c7151db0dbf630fd66",
+        299: "e6bd576db486fa2a916e",
         314: "352e97cabfe87ffaafa9",
         413: "c23fa684c321e1bc178c",
-        662: "a45c67772b045e9d4102",
-        760: "44dd9522edcf2585c0a2",
+        738: "f38212808e42bfc27026",
+        760: "b5d1c9daae2954d25258",
+        790: "589efecc3bfc7f71f9e1",
         839: "14d748171b9c87a422f9",
         899: "d8ce2a60114cd6e1ebea",
         930: "50b2067c71cf2a3ca014",
         981: "9b18765371d0668dbc59"
     } [e] + ".js?v=" + {
-        46: "208d560cd92dfb43b720",
-        87: "a9066e8e77b73733ee8e",
-        238: "86e88a3059c9a5a0803f",
-        252: "856eca7b3cd3748103bd",
-        299: "40530f9f1ff8893867f0",
+        80: "bfe2ae9640edadf1b2bf",
+        87: "4c5b9b62b8fcc0e00e87",
+        252: "d0c7151db0dbf630fd66",
+        299: "e6bd576db486fa2a916e",
         314: "352e97cabfe87ffaafa9",
         413: "c23fa684c321e1bc178c",
-        662: "a45c67772b045e9d4102",
-        760: "44dd9522edcf2585c0a2",
+        738: "f38212808e42bfc27026",
+        760: "b5d1c9daae2954d25258",
+        790: "589efecc3bfc7f71f9e1",
         839: "14d748171b9c87a422f9",
         899: "d8ce2a60114cd6e1ebea",
         930: "50b2067c71cf2a3ca014",
         981: "9b18765371d0668dbc59"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/collaboration-extension:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var i, l;
+            var l, i;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
                     var d = u[f];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                        l = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, P.nc && l.setAttribute("nonce", P.nc), l.setAttribute("data-webpack", r + o), l.src = t), e[t] = [a];
             var c = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(s);
+                    l.onerror = l.onload = null, clearTimeout(s);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
+                    if (delete e[t], l.parentNode && l.parentNode.removeChild(l), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: l
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            l.onerror = c.bind(null, l.onerror), l.onload = c.bind(null, l.onload), i && document.head.appendChild(l)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -118,26 +118,26 @@
         P.I = (t, a) => {
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 P.o(P.S, t) || (P.S[t] = {});
                 var n = P.S[t],
-                    i = "@jupyter/collaboration-extension",
-                    l = (e, r, t, a) => {
+                    l = "@jupyter/collaboration-extension",
+                    i = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
+                            i = o[r];
+                        (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
-                            from: i,
+                            from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/collaboration-extension", "1.0.1", (() => Promise.all([P.e(899), P.e(981), P.e(662), P.e(46), P.e(238), P.e(87)]).then((() => () => P(5087))))), l("@jupyter/collaboration", "1.0.1", (() => Promise.all([P.e(981), P.e(930), P.e(662), P.e(760), P.e(46)]).then((() => () => P(4760))))), l("@jupyter/docprovider", "1.0.1", (() => Promise.all([P.e(899), P.e(930), P.e(662), P.e(314), P.e(238), P.e(299)]).then((() => () => P(4299))))), l("y-websocket", "1.5.0", (() => Promise.all([P.e(899), P.e(413), P.e(981)]).then((() => () => P(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@jupyter/collaboration-extension", "1.1.0-alpha.0", (() => Promise.all([P.e(899), P.e(981), P.e(738), P.e(80), P.e(790), P.e(87)]).then((() => () => P(5087))))), i("@jupyter/collaboration", "1.1.0-alpha.0", (() => Promise.all([P.e(981), P.e(930), P.e(738), P.e(760), P.e(80)]).then((() => () => P(4760))))), i("@jupyter/docprovider", "1.1.0-alpha.0", (() => Promise.all([P.e(899), P.e(930), P.e(738), P.e(314), P.e(790), P.e(299)]).then((() => () => P(4299))))), i("y-websocket", "1.5.0", (() => Promise.all([P.e(899), P.e(413), P.e(981)]).then((() => () => P(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -155,128 +155,128 @@
     }, a = (e, r) => {
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
-            var i = r[a],
-                l = (typeof i)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
-            if ("o" != n && "u" != n && o != i) return o < i;
+            var l = r[a],
+                i = (typeof l)[0];
+            if (n != i) return "o" == n && "n" == i || "s" == i || "u" == n;
+            if ("o" != n && "u" != n && o != l) return o < l;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(i = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
             return t
         }
-        var i = [];
+        var l = [];
         for (n = 1; n < e.length; n++) {
-            var l = e[n];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+            var i = e[n];
+            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : o(i))
         }
         return u();
 
         function u() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return l.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == c ? l > a && !o : "" == c != o);
+            for (var l = 0, i = 1, u = !0;; i++, l++) {
+                var f, d, c = i < e.length ? (typeof e[i])[0] : "";
+                if (l >= r.length || "o" == (d = (typeof(f = r[l]))[0])) return !u || ("u" == c ? i > a && !o : "" == c != o);
                 if ("u" == d) {
                     if (!u || "u" != c) return !1
                 } else if (u)
                     if (c == d)
-                        if (l <= a) {
-                            if (f != e[l]) return !1
+                        if (i <= a) {
+                            if (f != e[i]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (o ? f > e[i] : f < e[i]) return !1;
+                            f != e[i] && (u = !1)
                         }
                 else if ("s" != c && "n" != c) {
-                    if (o || l <= a) return !1;
-                    u = !1, l--
+                    if (o || i <= a) return !1;
+                    u = !1, i--
                 } else {
-                    if (l <= a || d < c != o) return !1;
+                    if (i <= a || d < c != o) return !1;
                     u = !1
-                } else "s" != c && "n" != c && (u = !1, l--)
+                } else "s" != c && "n" != c && (u = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
-        for (i = 1; i < e.length; i++) {
-            var b = e[i];
+        for (l = 1; l < e.length; l++) {
+            var b = e[l];
             s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
         }
         return !!p()
-    }, i = (e, r) => {
+    }, l = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, l = (e, r) => {
+    }, i = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", f = (e, r, t, a) => {
-        var o = l(e, t);
+        var o = i(e, t);
         return n(a, o) || c(u(e, t, o, a)), s(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, s = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, o) {
         var n = P.I(r);
         return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
-    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), h = p(((e, r, t, a, o) => r && P.o(r, t) ? f(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
+    })(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), h = p(((e, r, t, a, o) => r && P.o(r, t) ? f(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
         var n = r && P.o(r, t) && d(r, t, a);
         return n ? s(n) : o()
     })), y = {}, m = {
         981: () => b("default", "yjs", [1, 13, 5, 40]),
-        5350: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
-        9993: () => b("default", "@jupyterlab/coreutils", [1, 6, 0, 2]),
-        926: () => b("default", "@jupyterlab/translation", [1, 4, 0, 2]),
-        2189: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 2]),
+        3172: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
+        5987: () => b("default", "@jupyterlab/coreutils", [1, 6, 0, 3]),
+        1580: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
+        5354: () => b("default", "@jupyterlab/translation", [1, 4, 0, 3]),
         8778: () => b("default", "@lumino/widgets", [1, 2, 0, 1]),
-        4238: () => b("default", "@jupyterlab/services", [1, 7, 0, 2]),
-        56: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
-        1255: () => h("default", "@jupyter/collaboration", [1, 1, 0, 1], (() => Promise.all([P.e(930), P.e(760)]).then((() => () => P(4760))))),
-        1617: () => b("default", "@jupyterlab/statedb", [1, 4, 0, 2]),
-        1919: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 2]),
-        2164: () => b("default", "@jupyterlab/filebrowser", [1, 4, 0, 2]),
+        2790: () => b("default", "@jupyterlab/services", [1, 7, 0, 3]),
+        42: () => b("default", "@jupyterlab/logconsole", [1, 4, 0, 3]),
         2293: () => b("default", "@jupyter/ydoc", [1, 1, 0, 2]),
-        2927: () => b("default", "@jupyterlab/codemirror", [1, 4, 0, 2]),
-        4163: () => b("default", "@jupyterlab/application", [1, 4, 0, 2]),
-        4822: () => h("default", "@jupyter/docprovider", [1, 1, 0, 1], (() => Promise.all([P.e(930), P.e(314), P.e(252)]).then((() => () => P(4299))))),
-        8486: () => b("default", "@jupyterlab/fileeditor", [1, 4, 0, 2]),
-        9350: () => b("default", "@jupyterlab/logconsole", [1, 4, 0, 2]),
+        3007: () => b("default", "@jupyterlab/statedb", [1, 4, 0, 3]),
+        4004: () => b("default", "@jupyterlab/application", [1, 4, 0, 3]),
+        6154: () => b("default", "@jupyterlab/filebrowser", [1, 4, 0, 3]),
+        6408: () => b("default", "@jupyterlab/codemirror", [1, 4, 0, 3]),
+        7349: () => h("default", "@jupyter/collaboration", [1, 1, 1, 0, , "alpha", 0], (() => Promise.all([P.e(930), P.e(760)]).then((() => () => P(4760))))),
+        7785: () => b("default", "@jupyterlab/fileeditor", [1, 4, 0, 3]),
+        7861: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
+        8027: () => h("default", "@jupyter/docprovider", [1, 1, 1, 0, , "alpha", 0], (() => Promise.all([P.e(930), P.e(314), P.e(252)]).then((() => () => P(4299))))),
+        8663: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
         7930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4059: () => b("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         6029: () => b("default", "react", [1, 18, 2, 0]),
         6211: () => b("default", "@codemirror/view", [1, 6, 9, 6]),
         8204: () => b("default", "@codemirror/state", [1, 6, 2, 0]),
         4901: () => b("default", "@lumino/signaling", [1, 2, 0, 0]),
         7099: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([P.e(413), P.e(981)]).then((() => () => P(413)))))
     }, g = {
-        46: [926, 2189, 8778],
-        87: [56, 1255, 1617, 1919, 2164, 2293, 2927, 4163, 4822, 8486, 9350],
-        238: [4238],
+        80: [1580, 5354, 8778],
+        87: [42, 2293, 3007, 4004, 6154, 6408, 7349, 7785, 7861, 8027, 8663],
         314: [4901, 7099],
-        662: [5350, 9993],
+        738: [3172, 5987],
         760: [4059, 6029, 6211, 8204],
+        790: [2790],
         930: [7930],
         981: [981]
     }, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, P.m[e] = t => {
@@ -299,37 +299,37 @@
         var e = {
             510: 0
         };
         P.f.j = (r, t) => {
             var a = P.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(238|314|46|662|930|981)$/.test(r)) e[r] = 0;
+                else if (/^((79|8|93)0|314|738|981)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = P.p + P.u(r),
-                    i = new Error;
+                    l = new Error;
                 P.l(n, (t => {
                     if (P.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             n = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
+                        l.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", l.name = "ChunkLoadError", l.type = o, l.request = n, a[1](l)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, l] = t,
+                var a, o, [n, l, i] = t,
                     u = 0;
                 if (n.some((r => 0 !== e[r]))) {
-                    for (a in i) P.o(i, a) && (P.m[a] = i[a]);
-                    l && l(P)
+                    for (a in l) P.o(l, a) && (P.m[a] = l[a]);
+                    i && i(P)
                 }
                 for (r && r(t); u < n.length; u++) o = n[u], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
-    var S = P(6746);
+    var S = P(5432);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/collaboration-extension"] = S
 })();
```

### Comparing `jupyter_collaboration-1.0.1/jupyter_collaboration/labextension/static/third-party-licenses.json` & `jupyter_collaboration-1.1.0a0/jupyter_collaboration/labextension/static/third-party-licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.1.0-alpha.0'}, 1: {'versionInfo': '1.1.0-alpha.0'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "1.0.1"
+            "versionInfo": "1.1.0-alpha.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "1.0.1"
+            "versionInfo": "1.1.0-alpha.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.7.3"
         },
```

### Comparing `jupyter_collaboration-1.0.1/scripts/bump_version.py` & `jupyter_collaboration-1.1.0a0/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/tests/test_loaders.py` & `jupyter_collaboration-1.1.0a0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/package.json` & `jupyter_collaboration-1.1.0a0/packages/collaboration/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740384615384615%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^1.1.0-alpha.0'}", "'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.7.0",
-        "@jupyter/docprovider": "^1.0.1",
+        "@jupyter/docprovider": "^1.1.0-alpha.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/ui-components": "^4.0.0",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/virtualdom": "^2.0.0",
         "@lumino/widgets": "^2.1.0",
@@ -63,9 +63,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0-alpha.0"
 }
```

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/collaboratorspanel.tsx` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/components.tsx` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/cursors.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/cursors.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/menu.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/sharedlink.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/tokens.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/src/userinfopanel.tsx` & `jupyter_collaboration-1.1.0a0/packages/collaboration/src/userinfopanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/style/menu.css` & `jupyter_collaboration-1.1.0a0/packages/collaboration/style/menu.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration-1.1.0a0/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration-extension/package.json` & `jupyter_collaboration-1.1.0a0/packages/collaboration-extension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.1.0-alpha.0', '@jupyter/docprovider': "*

 * *                   "'^1.1.0-alpha.0'}",*

 * * "'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.1",
-        "@jupyter/docprovider": "^1.0.1",
+        "@jupyter/collaboration": "^1.1.0-alpha.0",
+        "@jupyter/docprovider": "^1.1.0-alpha.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/fileeditor": "^4.0.0",
@@ -124,9 +124,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0-alpha.0"
 }
```

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/collaboration.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/collaboration.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/filebrowser.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/filebrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/collaboration-extension/src/sharedlink.ts` & `jupyter_collaboration-1.1.0a0/packages/collaboration-extension/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/jest.config.js` & `jupyter_collaboration-1.1.0a0/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/package.json` & `jupyter_collaboration-1.1.0a0/packages/docprovider/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'1.1.0-alpha.0'"}*

```diff
@@ -61,9 +61,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0-alpha.0"
 }
```

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/src/awareness.ts` & `jupyter_collaboration-1.1.0a0/packages/docprovider/src/awareness.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/src/requests.ts` & `jupyter_collaboration-1.1.0a0/packages/docprovider/src/requests.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/src/tokens.ts` & `jupyter_collaboration-1.1.0a0/packages/docprovider/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration-1.1.0a0/packages/docprovider/src/ydrive.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
-import { URLExt } from '@jupyterlab/coreutils';
+import { PageConfig, URLExt } from '@jupyterlab/coreutils';
 import { TranslationBundle } from '@jupyterlab/translation';
 import { Contents, Drive, User } from '@jupyterlab/services';
 
 import { DocumentChange, ISharedDocument, YDocument } from '@jupyter/ydoc';
 
 import { WebSocketProvider } from './yprovider';
 import {
   ICollaborativeDrive,
   ISharedModelFactory,
   SharedDocumentFactory
 } from './tokens';
 
+const DISABLE_RTC =
+  PageConfig.getOption('disableRTC') === 'true' ? true : false;
+
 /**
  * The url for the default drive service.
  */
 const DOCUMENT_PROVIDER_URL = 'api/collaboration/room';
 
 /**
  * A Collaborative implementation for an `IDrive`, talking to the
@@ -173,15 +176,15 @@
   ) {
     this._documentFactories = new Map();
   }
 
   /**
    * Whether the IDrive supports real-time collaboration or not.
    */
-  readonly collaborative = true;
+  readonly collaborative = !DISABLE_RTC;
 
   /**
    * Register a SharedDocumentFactory.
    *
    * @param type Document type
    * @param factory Document factory
    */
@@ -204,15 +207,15 @@
     options: Contents.ISharedFactoryOptions
   ): ISharedDocument | undefined {
     if (typeof options.format !== 'string') {
       console.warn(`Only defined format are supported; got ${options.format}.`);
       return;
     }
 
-    if (!options.collaborative) {
+    if (!this.collaborative || !options.collaborative) {
       // Bail if the document model does not support collaboration
       // the `sharedModel` will be the default one.
       return;
     }
 
     if (this._documentFactories.has(options.contentType)) {
       const factory = this._documentFactories.get(options.contentType)!;
```

### Comparing `jupyter_collaboration-1.0.1/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration-1.1.0a0/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/.gitignore` & `jupyter_collaboration-1.1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/LICENSE` & `jupyter_collaboration-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/README.md` & `jupyter_collaboration-1.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.1/pyproject.toml` & `jupyter_collaboration-1.1.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
 ]
 dependencies = [
     "jupyter_server>=2.0.0,<3.0.0",
     "jupyter_ydoc>=1.0.1,<2.0.0",
     "ypy-websocket>=0.12.1,<0.13.0",
     "jupyter_events",
-    "jupyter_server_fileid>=0.6.0,<1"
+    "jupyter_server_fileid>=0.6.0,<1",
+    "jsonschema[format-nongpl,format_nongpl]<4.18.0" # https://github.com/jupyter/jupyter_events/pull/80
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 dev = [
     "click",
     "pre-commit",
```

### Comparing `jupyter_collaboration-1.0.1/PKG-INFO` & `jupyter_collaboration-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_collaboration
-Version: 1.0.1
+Version: 1.1.0a0
 Summary: JupyterLab Extension enabling Real-Time Collaboration
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter_collaboration
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter_collaboration/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter_collaboration.git
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
@@ -77,14 +77,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: jsonschema[format-nongpl]<4.18.0
 Requires-Dist: jupyter-events
 Requires-Dist: jupyter-server-fileid<1,>=0.6.0
 Requires-Dist: jupyter-server<3.0.0,>=2.0.0
 Requires-Dist: jupyter-ydoc<2.0.0,>=1.0.1
 Requires-Dist: ypy-websocket<0.13.0,>=0.12.1
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
```

