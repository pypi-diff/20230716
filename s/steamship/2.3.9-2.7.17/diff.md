# Comparing `tmp/steamship-2.3.9.tar.gz` & `tmp/steamship-2.7.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamship-2.3.9.tar", last modified: Wed Jan 25 21:13:28 2023, max compression
+gzip compressed data, was "steamship-2.7.17.tar", last modified: Fri Jul 14 05:18:03 2023, max compression
```

## Comparing `steamship-2.3.9.tar` & `steamship-2.7.17.tar`

### file list

```diff
@@ -1,407 +1,619 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.293581 steamship-2.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.253581 steamship-2.3.9/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/.devcontainer/library-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    18654 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/common-debian.sh
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/meta.env
--rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/node-debian.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    14982 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/python-debian.sh
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-25 21:13:15.000000 steamship-2.3.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.249581 steamship-2.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/test-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/test-staging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-25 21:13:15.000000 steamship-2.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-01-25 21:13:15.000000 steamship-2.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-25 21:13:15.000000 steamship-2.3.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-25 21:13:15.000000 steamship-2.3.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-01-25 21:13:15.000000 steamship-2.3.9/DEVELOPING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-25 21:13:15.000000 steamship-2.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 21:13:28.293581 steamship-2.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-25 21:13:15.000000 steamship-2.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-25 21:13:15.000000 steamship-2.3.9/TESTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/Steamship-symbol-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/Steamship-symbol-light.png
--rw-r--r--   0 runner    (1001) docker     (123)   227249 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.invocable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.blockifier.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.inputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.outputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/changelog._rst
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/deploying.rst
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/environment-setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/project-creation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/steamship-manifest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/storing-secrets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/updating-web-listing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/cookbook/
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/adding-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/article-tagging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/collecting-and-querying-sentiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/modifying-an-existing-package.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/receiving-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-audio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-text.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/developing/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/plugins/blockifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/async-plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/blockifiers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/embedders.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/importers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/taggers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/embedders/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/embedders/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/embedders/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/importers/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/importers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/importers/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/taggers/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/taggers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/taggers/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/blockifying.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/creating.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/importing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/queries/
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/queries/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-25 21:13:15.000000 steamship-2.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-25 21:13:15.000000 steamship-2.3.9/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-25 21:13:15.000000 steamship-2.3.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-01-25 21:13:15.000000 steamship-2.3.9/scripts/build-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-25 21:13:15.000000 steamship-2.3.9/scripts/create_engine_test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 21:13:28.293581 steamship-2.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.249581 steamship-2.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/src/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/base/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/package_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/request.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/manifest_init_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/ship_spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/client/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/skill_to_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/skills.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/steamship.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/vendors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/package/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/data/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/index_plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/prompt_generation_plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/data/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/tag_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/invocable/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/package_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/paramater_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/blockifier/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/file_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/block_and_tag_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/export_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/file_import_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/raw_data_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/train_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/training_parameter_plugin_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/src/steamship/plugin/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/block_and_tag_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/embedded_items_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/raw_data_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/train_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/training_parameter_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/trainable_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/src/steamship/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/huggingface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/kv_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/signed_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/zip_archives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/src/steamship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/empty_json.json
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/one_string_one_int.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/single_integer.json
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/demo_package_spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/bad_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/configurable_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/demo_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/fancy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/optional_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/returns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/safe_loaded_bad_import.pyignore
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/safe_loaded_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/signed_url_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/palm_tree.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/blockifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/async_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/csv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/tsv_blockifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/importers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_by_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_python_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/taggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_configurable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_logging_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/utterances.csv
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/utterances.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_configurable_package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_package_error_visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_returns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_signed_url_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_use_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_config_template_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_demo_app_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_training_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_steamship_error_serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/client/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_blockify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_convert_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_tag_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/test_task_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/data/tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/tags/test_file_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_app_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_img.png
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_task_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/utterances.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_corpus_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_config_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_response_post_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/test_package_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/test_task_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.293581 steamship-2.3.9/tests/steamship_tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/deployables.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_camel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_kv_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_signed_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_static_instance_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_zip_archives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.352723 steamship-2.7.17/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.280716 steamship-2.7.17/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.280716 steamship-2.7.17/.devcontainer/library-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/library-scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18654 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/library-scripts/common-debian.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/library-scripts/meta.env
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/library-scripts/node-debian.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14982 2023-07-14 05:17:45.000000 steamship-2.7.17/.devcontainer/library-scripts/python-debian.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 05:17:45.000000 steamship-2.7.17/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.268715 steamship-2.7.17/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.280716 steamship-2.7.17/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-14 05:17:45.000000 steamship-2.7.17/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-14 05:17:45.000000 steamship-2.7.17/.github/workflows/notify-of-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-14 05:17:45.000000 steamship-2.7.17/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-14 05:17:45.000000 steamship-2.7.17/.github/workflows/test-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-14 05:17:45.000000 steamship-2.7.17/.github/workflows/test-staging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-14 05:17:45.000000 steamship-2.7.17/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-14 05:17:45.000000 steamship-2.7.17/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 05:17:45.000000 steamship-2.7.17/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 05:17:45.000000 steamship-2.7.17/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-14 05:17:45.000000 steamship-2.7.17/DEVELOPING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 05:17:45.000000 steamship-2.7.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 05:18:03.352723 steamship-2.7.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 05:17:45.000000 steamship-2.7.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-14 05:17:45.000000 steamship-2.7.17/TESTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-07-14 05:17:45.000000 steamship-2.7.17/badge.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.280716 steamship-2.7.17/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.284717 steamship-2.7.17/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/_static/Steamship-symbol-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/_static/Steamship-symbol-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   227249 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.284717 steamship-2.7.17/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.284717 steamship-2.7.17/docs/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/agents/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.288717 steamship-2.7.17/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.llms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.mixins.transports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.react.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.audio_transcription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.conversation_starters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.image_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.question_answering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.search.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.speech_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.text_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.agents.tools.video_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.cli.local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.experimental.easy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.experimental.package_starters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.invocable.mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.invocable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.plugin.blockifier.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.plugin.inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.plugin.outputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/api/steamship.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/changelog._rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.288717 steamship-2.7.17/docs/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/configuration/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/configuration/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/configuration/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/configuration/http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/configuration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.288717 steamship-2.7.17/docs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/file-lifecycle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.288717 steamship-2.7.17/docs/data/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/queries/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/data/workspaces.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/deploying.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/environment-setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   134722 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/logs-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/project-creation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/steamship-manifest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/storing-secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   138786 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/tasks-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    73459 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/developing/usage-example.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/embedding-search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/embedding-search/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/packages/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/adding-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/article-tagging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/collecting-and-querying-sentiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/modifying-an-existing-package.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/receiving-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/return-audio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/return-image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/return-json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/cookbook/return-text.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/packages/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/developing/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/packages/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.292717 steamship-2.7.17/docs/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/async-plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/blockifiers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/embedders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/importers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/developing/taggers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/blockifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/blockifiers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/blockifiers/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/embedders/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/embedders/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/generators/dalle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/generators/gpt4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/generators/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/importers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/importers/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/docs/plugins/using/taggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/taggers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/taggers/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/plugins/using/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-14 05:17:45.000000 steamship-2.7.17/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-14 05:17:45.000000 steamship-2.7.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-14 05:17:45.000000 steamship-2.7.17/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 05:17:45.000000 steamship-2.7.17/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-14 05:17:45.000000 steamship-2.7.17/scripts/build-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-14 05:17:45.000000 steamship-2.7.17/scripts/create_engine_test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:18:03.352723 steamship-2.7.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.268715 steamship-2.7.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/src/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/document_qa_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/example_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/example_react_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/fact_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/examples/telegram_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/functional/functions_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/functional/output_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/mixins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/mixins/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/mixins/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/mixins/transports/steamship_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/mixins/transports/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/mixins/transports/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.300718 steamship-2.7.17/src/steamship/agents/react/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/react/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/react/react.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/chathistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/message_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/text_splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/schema/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/service/agent_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/audio_transcription/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/audio_transcription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/audio_transcription/assembly_speech_to_text_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/audio_transcription/fetch_audio_urls_from_rss_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/audio_transcription/whisper_speech_to_text_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/base_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/classification/sentiment_analysis_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/classification/zero_shot_classifier_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/conversation_starters/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/conversation_starters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/conversation_starters/knock_knock_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/image_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/image_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/image_generation/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/image_generation/google_image_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/image_generation/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/question_answering/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/question_answering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/question_answering/prompt_database_question_answerer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/question_answering/vector_search_learner_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/question_answering/vector_search_qa_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/question_answering/vector_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.304718 steamship-2.7.17/src/steamship/agents/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.308719 steamship-2.7.17/src/steamship/agents/tools/speech_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/speech_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/speech_generation/generate_speech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.308719 steamship-2.7.17/src/steamship/agents/tools/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/image_prompt_generator_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/json_object_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/personality_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/summarize_text_with_prompt_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/text_rewrite_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/text_generation/text_translation_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.308719 steamship-2.7.17/src/steamship/agents/tools/video_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/video_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/tools/video_generation/did_video_generator_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.308719 steamship-2.7.17/src/steamship/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27136 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/package_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/base/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/create_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/cli/local_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/local_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/local_server/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/local_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/manifest_init_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/requirements_init_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/ship_spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/client/skill_to_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/client/skills.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/client/steamship.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/client/vendors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/invocable_init_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/data/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/operations/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/operations/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/operations/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/operations/tagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.312719 steamship-2.7.17/src/steamship/data/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/package/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/package/package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/package/package_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/data/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/index_plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/plugin/prompt_generation_plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/data/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/tags/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/tags/tag_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/data/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/experimental/easy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/experimental/easy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/experimental/easy/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/experimental/package_starters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/experimental/package_starters/telegram_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/experimental/package_starters/web_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.316720 steamship-2.7.17/src/steamship/invocable/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/dev_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/invocable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/invocable_localhost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/invocable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/invocable_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.320720 steamship-2.7.17/src/steamship/invocable/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/mixins/blockifier_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/mixins/file_importer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/mixins/indexer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/mixins/indexer_pipeline_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/package_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/package_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/paramater_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/invocable/plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.320720 steamship-2.7.17/src/steamship/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.320720 steamship-2.7.17/src/steamship/plugin/blockifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/blockifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/blockifier/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/blockifier/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.320720 steamship-2.7.17/src/steamship/plugin/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/block_and_tag_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/export_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/file_import_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/raw_block_and_tag_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/raw_data_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/train_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/inputs/training_parameter_plugin_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.324720 steamship-2.7.17/src/steamship/plugin/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/block_and_tag_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/embedded_items_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/raw_block_and_tag_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/raw_data_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/train_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/outputs/training_parameter_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/plugin/trainable_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.324720 steamship-2.7.17/src/steamship/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/context_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/file_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/huggingface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/kv_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/signed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 05:17:45.000000 steamship-2.7.17/src/steamship/utils/zip_archives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.296718 steamship-2.7.17/src/steamship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23055 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 05:18:03.000000 steamship-2.7.17/src/steamship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.324720 steamship-2.7.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.324720 steamship-2.7.17/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.324720 steamship-2.7.17/tests/assets/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/configs/empty_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/configs/one_string_one_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/configs/single_integer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/demo_package_spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.328721 steamship-2.7.17/tests/assets/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/adding_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/article_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/bad_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/configurable_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28340 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/demo_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/example_project_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/fancy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/optional_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_verifying_instance_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_with_failing_instance_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_with_instance_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_with_mixin_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_with_mixin_indexer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/package_with_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/requirement_isolation_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/returns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/safe_loaded_bad_import.pyignore
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/safe_loaded_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/signed_url_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.328721 steamship-2.7.17/tests/assets/packages/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/transports/mock_telegram_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/transports/test_telegram_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/packages/transports/test_web_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/palm_tree.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.328721 steamship-2.7.17/tests/assets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.332721 steamship-2.7.17/tests/assets/plugins/blockifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/blockifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/blockifiers/async_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/blockifiers/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/blockifiers/csv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/blockifiers/tsv_blockifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.332721 steamship-2.7.17/tests/assets/plugins/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/generators/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/generators/plugin_with_instance_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/generators/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/generators/test_generator_returns_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/generators/test_image_to_text_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.332721 steamship-2.7.17/tests/assets/plugins/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_by_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_python_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.332721 steamship-2.7.17/tests/assets/plugins/taggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_configurable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_logging_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/utterances.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/assets/utterances.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.332721 steamship-2.7.17/tests/steamship_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.336721 steamship-2.7.17/tests/steamship_tests/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_function_agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_functions_based_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_message_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_qa_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_react_parse_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.336721 steamship-2.7.17/tests/steamship_tests/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/agents/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.336721 steamship-2.7.17/tests/steamship_tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.336721 steamship-2.7.17/tests/steamship_tests/app/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_adding_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_article_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_configurable_package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_e2e_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_e2e_mixins_importer_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_e2e_mixins_indexer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_example_project_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_instance_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_package_error_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_requirements_installation_isolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_returns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_safe_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_signed_url_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/integration/test_use_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.340722 steamship-2.7.17/tests/steamship_tests/app/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_config_template_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_demo_app_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_document_qa_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_indexer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_indexer_pipeline_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_multi_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_routes_on_superclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/app/unit/test_training_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.340722 steamship-2.7.17/tests/steamship_tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/test_binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/test_steamship_error_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/base/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.340722 steamship-2.7.17/tests/steamship_tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.340722 steamship-2.7.17/tests/steamship_tests/client/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_blockify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_convert_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_embed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_embedding_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/operations/test_tag_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/client/test_task_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.344722 steamship-2.7.17/tests/steamship_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.344722 steamship-2.7.17/tests/steamship_tests/data/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/tags/test_file_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_task_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/data/utterances.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.344722 steamship-2.7.17/tests/steamship_tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.344722 steamship-2.7.17/tests/steamship_tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.348722 steamship-2.7.17/tests/steamship_tests/plugin/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_corpus_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_use_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/integration/test_use_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.348722 steamship-2.7.17/tests/steamship_tests/plugin/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_config_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_response_post_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.348722 steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.348722 steamship-2.7.17/tests/steamship_tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/server/test_package_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/server/test_task_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:18:03.352723 steamship-2.7.17/tests/steamship_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/deployables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_camel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_kv_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_signed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_static_instance_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-14 05:17:45.000000 steamship-2.7.17/tests/steamship_tests/utils/test_zip_archives.py
```

### Comparing `steamship-2.3.9/.devcontainer/Dockerfile` & `steamship-2.7.17/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.devcontainer/base.Dockerfile` & `steamship-2.7.17/.devcontainer/base.Dockerfile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.devcontainer/devcontainer.json` & `steamship-2.7.17/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.devcontainer/library-scripts/common-debian.sh` & `steamship-2.7.17/.devcontainer/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.devcontainer/library-scripts/node-debian.sh` & `steamship-2.7.17/.devcontainer/library-scripts/node-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.devcontainer/library-scripts/python-debian.sh` & `steamship-2.7.17/.devcontainer/library-scripts/python-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.github/workflows/docs-publish.yml` & `steamship-2.7.17/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.github/workflows/python-publish.yml` & `steamship-2.7.17/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/.github/workflows/test-main.yml` & `steamship-2.7.17/.github/workflows/test-main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 on:
   pull_request:
     branches:
       - main
   push:
     branches:
       - main
+  workflow_dispatch:
 
 jobs:
   test:
     name: Run test suite
     runs-on: ubuntu-latest
     timeout-minutes: 60
     strategy:
```

### Comparing `steamship-2.3.9/.github/workflows/test-staging.yml` & `steamship-2.7.17/.github/workflows/test-staging.yml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 on:
   pull_request:
     branches:
       - staging
   push:
     branches:
       - staging
+  workflow_dispatch:
 
 jobs:
   test:
     name: Run test suite
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
@@ -58,8 +59,8 @@
         run: python -m pip install -e .
 
       - name: Test against Steamship Staging
         run: pytest
         env:
           STEAMSHIP_API_KEY: ${{ secrets.STEAMSHIP_STAGING_TEST_KEY }}
           STEAMSHIP_API_BASE: ${{ secrets.STEAMSHIP_STAGING_TEST_API_BASE }}
-          STEAMSHIP_APP_BASE: ${{ secrets.STEAMSHIP_STAGING_TEST_APP_BASE }}
+          STEAMSHIP_APP_BASE: ${{ secrets.STEAMSHIP_STAGING_TEST_APP_BASE }}
```

### Comparing `steamship-2.3.9/.gitignore` & `steamship-2.7.17/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -102,8 +102,9 @@
 # Tox
 .tox/
 
 # Coverage
 .coverage/
 
 # Generated website
-docs/_build
+docs/_build
+venv
```

### Comparing `steamship-2.3.9/.pre-commit-config.yaml` & `steamship-2.7.17/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/DEVELOPING.md` & `steamship-2.7.17/DEVELOPING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Steamship
 
 We are excited to have you on board!
 
-These instructions contain the setup for contributors fo the Steamship client library. 
+These instructions contain the setup for contributors to the Steamship client library. 
 
 For information about *using* this library, please see README.md
 
 ## Basic Information
 
 * 🐍 The project targets Python 3
 * ✍️ Code formatting is performed with black and isort
```

### Comparing `steamship-2.3.9/LICENSE` & `steamship-2.7.17/LICENSE`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/TESTING.md` & `steamship-2.7.17/TESTING.md`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/Makefile` & `steamship-2.7.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/README.txt` & `steamship-2.7.17/docs/README.txt`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/_static/Steamship-symbol-dark.png` & `steamship-2.7.17/docs/_static/Steamship-symbol-dark.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/_static/Steamship-symbol-light.png` & `steamship-2.7.17/docs/_static/Steamship-symbol-light.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/_static/favicon.ico` & `steamship-2.7.17/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/_templates/base.html` & `steamship-2.7.17/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/api/steamship.base.rst` & `steamship-2.7.17/docs/api/steamship.base.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 -----------------------------------
 
 .. automodule:: steamship.base.configuration
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.base.environments module
+----------------------------------
+
+.. automodule:: steamship.base.environments
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.base.error module
 ---------------------------
 
 .. automodule:: steamship.base.error
    :members:
    :undoc-members:
    :show-inheritance:
@@ -72,22 +80,14 @@
 ---------------------------
 
 .. automodule:: steamship.base.tasks
    :members:
    :undoc-members:
    :show-inheritance:
 
-steamship.base.utils module
----------------------------
-
-.. automodule:: steamship.base.utils
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 Module contents
 ---------------
 
 .. automodule:: steamship.base
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/api/steamship.client.rst` & `steamship-2.7.17/docs/api/steamship.client.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/api/steamship.invocable.rst` & `steamship-2.7.17/docs/api/steamship.invocable.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 steamship.invocable package
 ===========================
 
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   steamship.invocable.mixins
+
 Submodules
 ----------
 
 steamship.invocable.config module
 ---------------------------------
 
 .. automodule:: steamship.invocable.config
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.invocable.dev\_logging\_handler module
+------------------------------------------------
+
+.. automodule:: steamship.invocable.dev_logging_handler
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.invocable.entrypoint module
 -------------------------------------
 
 .. automodule:: steamship.invocable.entrypoint
    :members:
    :undoc-members:
    :show-inheritance:
@@ -24,14 +40,22 @@
 ------------------------------------
 
 .. automodule:: steamship.invocable.invocable
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.invocable.invocable\_localhost module
+-----------------------------------------------
+
+.. automodule:: steamship.invocable.invocable_localhost
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.invocable.invocable\_request module
 ---------------------------------------------
 
 .. automodule:: steamship.invocable.invocable_request
    :members:
    :undoc-members:
    :show-inheritance:
@@ -48,14 +72,22 @@
 ------------------------------------------
 
 .. automodule:: steamship.invocable.lambda_handler
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.invocable.package\_mixin module
+-----------------------------------------
+
+.. automodule:: steamship.invocable.package_mixin
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.invocable.package\_service module
 -------------------------------------------
 
 .. automodule:: steamship.invocable.package_service
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/api/steamship.plugin.blockifier.rst` & `steamship-2.7.17/docs/api/steamship.plugin.blockifier.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/api/steamship.plugin.inputs.rst` & `steamship-2.7.17/docs/api/steamship.plugin.inputs.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 ----------------------------------------------------------
 
 .. automodule:: steamship.plugin.inputs.file_import_plugin_input
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.plugin.inputs.raw\_block\_and\_tag\_plugin\_input module
+------------------------------------------------------------------
+
+.. automodule:: steamship.plugin.inputs.raw_block_and_tag_plugin_input
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.plugin.inputs.raw\_data\_plugin\_input module
 -------------------------------------------------------
 
 .. automodule:: steamship.plugin.inputs.raw_data_plugin_input
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/api/steamship.plugin.outputs.rst` & `steamship-2.7.17/docs/api/steamship.plugin.outputs.rst`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,30 @@
 -------------------------------------------------
 
 .. automodule:: steamship.plugin.outputs.model_checkpoint
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.plugin.outputs.plugin\_output module
+----------------------------------------------
+
+.. automodule:: steamship.plugin.outputs.plugin_output
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+steamship.plugin.outputs.raw\_block\_and\_tag\_plugin\_output module
+--------------------------------------------------------------------
+
+.. automodule:: steamship.plugin.outputs.raw_block_and_tag_plugin_output
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.plugin.outputs.raw\_data\_plugin\_output module
 ---------------------------------------------------------
 
 .. automodule:: steamship.plugin.outputs.raw_data_plugin_output
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/api/steamship.plugin.rst` & `steamship-2.7.17/docs/api/steamship.plugin.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 --------------------------------------
 
 .. automodule:: steamship.plugin.file_importer
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.plugin.generator module
+---------------------------------
+
+.. automodule:: steamship.plugin.generator
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.plugin.request module
 -------------------------------
 
 .. automodule:: steamship.plugin.request
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/api/steamship.utils.rst` & `steamship-2.7.17/docs/api/steamship.utils.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,30 @@
 ------------------------------------
 
 .. automodule:: steamship.utils.binary_utils
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.utils.context\_length module
+--------------------------------------
+
+.. automodule:: steamship.utils.context_length
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+steamship.utils.file\_tags module
+---------------------------------
+
+.. automodule:: steamship.utils.file_tags
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.utils.huggingface\_helper module
 ------------------------------------------
 
 .. automodule:: steamship.utils.huggingface_helper
    :members:
    :undoc-members:
    :show-inheritance:
@@ -32,14 +48,22 @@
 -------------------------------
 
 .. automodule:: steamship.utils.metadata
    :members:
    :undoc-members:
    :show-inheritance:
 
+steamship.utils.repl module
+---------------------------
+
+.. automodule:: steamship.utils.repl
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 steamship.utils.signed\_urls module
 -----------------------------------
 
 .. automodule:: steamship.utils.signed_urls
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `steamship-2.3.9/docs/conf.py` & `steamship-2.7.17/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,21 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv"]
+exclude_patterns = [
+    "_build",
+    "Thumbs.db",
+    ".DS_Store",
+    ".venv",
+    "packages/cookbook/article-tagging.rst",
+]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
@@ -165,17 +171,23 @@
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "light_logo": "Steamship-symbol-dark.png",
     "dark_logo": "Steamship-symbol-light.png",
-    "light_css_variables": {"color-brand-primary": "#202b45", "color-brand-content": "#333333"},
+    "light_css_variables": {
+        "color-brand-primary": "#202B45",
+        "color-brand-content": "#9558FC",
+        "font-stack": "Albert Sans, sans-serif",
+        "font-stack--monospace": "Courier, monospace",
+    },
     "dark_css_variables": {
-        "color-brand-content": "#EEEEEE",
+        "color-brand-primary": "#9558FC",
+        "color-brand-content": "#F6B938",
     },
     "footer_icons": [
         {
             "name": "GitHub",
             "url": "https://github.com/steamship-core/python-client",
             "html": """
             <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 16 16">
```

### Comparing `steamship-2.3.9/docs/configuration/authentication.rst` & `steamship-2.7.17/docs/configuration/authentication.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _Auth
+
 Authentication
 --------------
 
 Steamship uses API Keys to authenticate our CLI and client libraries.
 These keys can be stored in a configuration file, in environment variables, or passed manually to our client libraries.
 
 Steamship Configuration File
```

### Comparing `steamship-2.3.9/docs/configuration/clients.rst` & `steamship-2.7.17/docs/configuration/clients.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/configuration/http.rst` & `steamship-2.7.17/docs/configuration/http.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/developing/configuration.rst` & `steamship-2.7.17/docs/developing/configuration.rst`

 * *Files 24% similar despite different names*

```diff
@@ -3,85 +3,59 @@
 
 Your package or plugin may need to accept configuration to be usable.
 Examples might include:
 
 - An API key to invoke a third-party service
 - A parameter setting, such as a threshold or output class
 
-Your package or plugin's :ref:`Steamship Manifest<Steamship Manifest Files>` file contains a property
-called ``configTemplate`` which enables you to define and strongly type this configuration.
-
-.. _configTemplate Schema:
-
-Declaring your configuration template
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``configTemplate`` property in your ``steamship.json`` file defines a schema
-for your package or plugin's configuration.
-This configuration is provided upon each new instance creation, and it is
-frozen and saved with the instance for reuse.
-
-The value of the ``configTemplate`` block takes the following form:
-
-.. code-block:: json
-
-   {
-     "configTemplate": {
-       "param_name": {
-         "type": "boolean",
-         "description": "Whether something should be enabled..",
-         "default": false
-       },
-       "param_name_2": {
-         "type": "string",
-         "description": "Some string parameter.",
-       }
-
-     }
-   }
-
-In the above code, you can see that the parameter name is the key of the
-object, and details about that parameter are in the associated body.
-Those details are:
-
+A configuration parameter has:
 -  ``type`` - Either ``boolean``, ``string``, or ``number``.
 -  ``description`` - A short description of the parameter.
 -  ``default`` - A default value if the user does not provide one.
 
 If a parameter does not have a default value, and a Steamship user tries
 to create a new instance without specifying it, that instance creation
 will fail. Similarly, provided values with incorrect types will be rejected. This
-means that your package or plugin is guaranteed to receive a config that structurally
-matches your ``configTemplate``.
+means that your package or plugin is guaranteed to receive a config that structurally matches.
+
+.. note::
+    There is currently no such thing as an optional configuration parameter. All parameters that do
+    not have a default value must have a value provided by the user at Package instantiation.
+
 
-Defining and using configuration in your code
+.. _Accepting Configuration:
+
+Defining and Accepting configuration in your code
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-After defining your ``configTemplate``, you must create a matching object in your package or plugin's Python implementation.
-This object should extend the ``steamship.invocable.Config`` class.
+
+To define the configuration for your Package, create a class that inherits from Config:
 
 .. code-block:: python
 
-   from steamship.invocable import Config
+   class MyPackageConfig(Config):
+        my_string_config_param: str = Field("my-default-value",
+                                    description="A param this package needs which is a string.")
+        my_numeric_config_param: float = Field(description="A numeric param this package needs.")
+
+and then return this class from your package or plugin's ``config_cls`` class method:
 
-   class MyPluginConfig(Config):
-       """Config object containing required parameters to initialize
-       a MyPlugin object."""
+.. code-block:: python
 
-       param_name: bool = False
-       param_name_2: str
+   class MyPackageClass(PackageService):
+       config: MyPackageConfig
+
+       @classmethod
+       def config_cls(cls) -> Type[Config]:
+            return MyPackageConfig
+
+This will guarantee that ``my_string_config_param`` and ``my_numeric_config_param`` are set for all invocations
+of your package or plugin.  Since ``my_strong_config_param`` provides a default value, the user can omit it
+from their configuration and the value ``"my-default-value"`` will be used.  Since ``my_numeric_config_param``
+does not have a default value, a user *must* supply a value to create an instance of your package or plugin.
+
+To use the config values within your code, you can then refer to them from ``self.config``,
+as in ``self.config.my_numeric_config_param``.  They will be automatically populated with the user's
+data by Steamship when invoking your package or plugin.
 
-In your class, you will also have to return this object from the abstract ``config_cls`` method.
-This enables the package or plugin loader to construct the correct configuration object.
 
-.. code-block:: python
 
-   class MyPlugin(Blockifier):
-      def config_cls(self) -> Type[Config]:=
-         return MyPluginConfig
-
-Finally, your package or plugin's base class will always make available a ``self.config`` object whose type
-matches the type returned by ``config_cls``.
-
-When users create new instances of your package plugin, the configuration will be type checked against the
-schema provided in ``steamship.json``. When the instance is invoked, the configuration will be
-loaded at runtime into ``self.config``.
```

### Comparing `steamship-2.3.9/docs/developing/deploying.rst` & `steamship-2.7.17/docs/developing/deploying.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 ---------
 
 Packages and plugins must be deployed before they can be used.
 
 New versions of your project automatically become the “default” version when new instances are created.
 Unless an instance specifically requests a version, this new default version will be used.
 
-Before you deploy, make sure the ``handle`` and ``version`` fields in your ``steamship.json`` file are set:
 
--  The ``handle`` property of ``steamship.json``
--  The ``version`` property of ``steamship.json``
 
 Deploying with the Steamship CLI
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can deploy a package or plugin with the Steamship CLI with single command from
-the project root:
+the project root (make sure your python environment is active):
 
 .. code-block:: bash
 
    ship deploy
 
-After the command exits, wait a few minutes for your new infrastructure to be ready in the cloud.
+If you don't have a ``steamship.json`` yet, the deploy process will create one. After the command exits, wait a few minutes for your new infrastructure to be ready in the cloud.
 New instances of your project will then be directed to the new version.
 
 Deploying via GitHub Actions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Each package and plugin project is created from a a template that has been pre-configured to
 auto-deploy within GitHub Actions when certain situations occur.
 
+Before you deploy, make sure the ``handle`` and ``version`` fields in your ``steamship.json`` file are set:
+
+-  The ``handle`` property of ``steamship.json``
+-  The ``version`` property of ``steamship.json``
+
 Production deployments occur upon:
 
 -  Pushes to ``main``
 -  Pushes to SemVer-style tags, prefixed with ``v`` (``vA.B.C``)
 
 Staging deployments occur upon:
```

### Comparing `steamship-2.3.9/docs/developing/environment-setup.rst` & `steamship-2.7.17/docs/developing/environment-setup.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/developing/index.rst` & `steamship-2.7.17/docs/developing/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 -  :ref:`Packages` expose endpoints that can do work on an associated :ref:`workspace<Workspaces>`
 -  :ref:`Plugins` conform to interfaces defined by the Steamship Engine to perform common tasks.
 
 .. warning::
     Third-party plugin development is currently in Alpha and the interface may change.
     If you want to build a plugin, we are eager to chat!
-    Just email hello@steamship.com
+    Just email hello@steamship.com or hop on our `Discord <http://steamship.com/discord>`_
 
 Steamship is designed from the ground up to support building, modifying, and sharing both packages and plugins.
 Each one you create is cloned from an existing template of your choosing.
 That template contains everything you need for a great development lifecycle:
 
 1.  A manifest file with metadata and statically-typed configuration
 2.  Unit tests with pre-configured GitHub Actions integration
@@ -30,11 +30,12 @@
    :maxdepth: 1
 
    Cloning a Starter Project <project-creation>
    The Steamship Manifest file <steamship-manifest>
    Python Environment Setup <environment-setup>
    Accepting Configuration <configuration>
    Storing Secrets <storing-secrets>
+   Running on Localhost <running>
    Writing Tests <testing>
    Deploying <deploying>
-   Updating your Web Listing <updating-web-listing>
+   Monitoring your Instances <monitoring>
```

### Comparing `steamship-2.3.9/docs/developing/steamship-manifest.rst` & `steamship-2.7.17/docs/developing/steamship-manifest.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/developing/storing-secrets.rst` & `steamship-2.7.17/docs/developing/storing-secrets.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/developing/testing.rst` & `steamship-2.7.17/docs/developing/testing.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/adding-configuration.rst` & `steamship-2.7.17/docs/packages/cookbook/adding-configuration.rst`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,17 @@
 
 Next, we tell the Steamship handler how to find our config class:
 
 .. code-block:: python
 
     class ConfigurableFavoritesPackage(PackageService):
         ...
-        def config_cls(self) -> Type[Config]:
-            return self.FavoritesConfig
+        @classmethod
+        def config_cls(cls) -> Type[Config]:
+            return cls.FavoritesConfig
 
 Now when implementing a method, we can use the config fields via ``self.config.<field_name>``!
 
 .. code-block:: python
 
     @post("my_faves")
     def my_faves(self) -> str:
@@ -96,40 +97,40 @@
 
     """
     This package demonstrates how configuration works in Steamship.
     """
     from typing import Dict, Any, Type
 
     from steamship import Steamship
-    from steamship.invocable import PackageService, Config, post, create_handler
+    from steamship.invocable import PackageService, Config, post
 
 
     class ConfigurableFavoritesPackage(PackageService):
         class FavoritesConfig(Config):
             """Configuration required to instantiate this package."""
 
             name: str
             favorite_color: str
             lucky_number: float
             favorite_true_false_value: bool
 
-        def __init__(self, client: Steamship, config: Dict[str, Any] = None):
+        def __init__(self, client: Steamship, config: Dict[str, Any] = None, context: InvocationContext = None):
             # The superclass init method turns the config param (a Dict)
             # into the self.config object (here, a FavoritesConfig)
             super().__init__(client, config)
 
 
         # The config_cls method allows your package to return a class
         # that defines its required configuration.
         # See Developer Reference -> Accepting Configuration
         # for more details. This package uses a few configuration fields
         # to record the package user's favorite things.
-        def config_cls(self) -> Type[Config]:
-            """Return our config object"""
-            return self.FavoritesConfig
+        @classmethod
+        def config_cls(cls) -> Type[Config]:
+            return cls.FavoritesConfig
 
         # This method defines the package user's endpoint for adding content
         # The @post annotation automatically makes the method available as
         # an HTTP Post request. The name in the annotation defines the HTTP
         # route suffix, see Packages -> Package Project Structure.
         @post("my_faves")
         def my_faves(self) -> str:
@@ -139,12 +140,7 @@
             Hey {self.config.name}!
             I can remind you of your favorites.
             Your favorite color is {self.config.favorite_color}.
             Your lucky number is {self.config.lucky_number}.
             Your favorite true/false value is {self.config.favorite_true_false_value}.
             Wow, mine too!
             """
-
-
-    # This line connects our Package implementation class to the surrounding
-    # Steamship handler code.
-    handler = create_handler(ConfigurableFavoritesPackage)
```

### Comparing `steamship-2.3.9/docs/packages/cookbook/article-tagging.rst` & `steamship-2.7.17/docs/packages/cookbook/article-tagging.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     """
     This package accepts text documents, stores them, labels them with tags,
     and retrieves them based on those tags.
     """
     from typing import Type, Dict, Any
 
     from steamship import Block, File, Steamship, Tag
-    from steamship.invocable import Config, create_handler, post, PackageService
+    from steamship.invocable import Config, InvocationContext, post, PackageService
 
 
     class ArticleTaggerPackage(PackageService):
         class ArticleTaggerConfig(Config):
             """Configuration required to instantiate this package."""
 
             labels: str  # A comma-separated list of tags to apply to articles
 
-        def __init__(self, client: Steamship, config: Dict[str, Any] = None):
+        def __init__(self, client: Steamship, config: Dict[str, Any] = None, context: InvocationContext = None):
             super().__init__(client, config)
 
             # Instantiate a zero-shot classifier plugin
             self.classifier_instance = client.use_plugin(
                 plugin_handle="zero-shot-tagger-default",
                 instance_handle="my-classifier",
                 config={"tag_kind": "tags",  # The tag.kind we want in the output
@@ -37,32 +37,33 @@
             )
 
         # The config_cls method allows your package to return a class
         # that defines its required configuration.
         # See Developer Reference -> Accepting Configuration
         # for more details. This package doesn't have any specific
         # required configuration, so we return the default Config object.
-        def config_cls(self) -> Type[Config]:
+        @classmethod
+        def config_cls(cls) -> Type[Config]:
             """Return our specific config type."""
-            return self.ArticleTaggerConfig
+            return cls.ArticleTaggerConfig
 
         # This method defines the package user's endpoint for adding content
         # The @post annotation automatically makes the method available as
         # an HTTP Post request. The name in the annotation defines the HTTP
         # route suffix, see Packages -> Package Project Structure.
         @post("add_document")
         def add_document(self, content: str, url: str) -> str:
             """Accept a new document in plaintext and start sentiment analysis"""
 
             # Upload the content of the file into Steamship.
             # Put the content directly into a Block, since we assume it is plaintext.
             # Create a tag with the URL so we can get it back later.
             file = File.create(self.client,
-                               blocks=[Block.CreateRequest(text=content)],
-                               tags=[Tag.CreateRequest(kind="url", name=url)])
+                               blocks=[Block(text=content)],
+                               tags=[Tag(kind="url", name=url)])
 
             # Tag the file with the sentiment analysis plugin
             # Using a plugin is an asynchronous call within Steamship. The
             # operation may not be complete when this method completes,
             # but that's ok. The other methods will query over whatever is
             # currently available.
             file.tag(self.classifier_instance.handle)
@@ -77,16 +78,11 @@
 
         @post("documents_by_tag")
         def documents_by_tag(self, tag: str, threshold: float = 0.7) -> [str]:
             """Query the stored documents for tagged articles"""
 
             # Query our documents for Positive sentiment tags
             matching_files = File.query(self.client,
-                f'kind "tags" and name "{tag}" and value("score") > {threshold}').files
+                                        f'kind "tags" and name "{tag}" and value("score") > {threshold}').files
 
             return [self._find_url(file) for file in matching_files]
 
-
-    # This line connects our Package implementation class to the surrounding
-    # Steamship handler code.
-    handler = create_handler(ArticleTaggerPackage)
-
```

### Comparing `steamship-2.3.9/docs/packages/cookbook/collecting-and-querying-sentiment.rst` & `steamship-2.7.17/docs/packages/cookbook/collecting-and-querying-sentiment.rst`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         @post("add_document")
         def add_document(self, content: str = None) -> str:
             """Accept a new document in plaintext and start sentiment analysis"""
 
             # Upload the content of the file into Steamship.
             # Put the content directly into a Block, since we assume it is plaintext.
             file = File.create(self.client,
-                               blocks=[Block.CreateRequest(text=content)])
+                               blocks=[Block(text=content)])
 
             # Tag the file with the sentiment analysis plugin
             # Using a plugin is an asynchronous call within Steamship. The
             # operation may not be complete when this method completes,
             # but that's ok. The other methods will query over whatever is
             # currently available.
             file.tag(self.sentiment_plugin_instance.handle)
@@ -72,15 +72,8 @@
             # Query our documents for Negative sentiment tags
             negative_files = File.query(self.client,
                 f"kind \"{TagKind.SENTIMENT}\" and name \"{SentimentTag.NEGATIVE}\"").files
 
             return [file.blocks[0].text for file in negative_files]
 
 
-    # This line connects our Package implementation class to the surrounding
-    # Steamship handler code.
-    handler = create_handler(SimpleSentimentPackage)
-
-
-
-
```

### Comparing `steamship-2.3.9/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst` & `steamship-2.7.17/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/index.rst` & `steamship-2.7.17/docs/packages/cookbook/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/modifying-an-existing-package.rst` & `steamship-2.7.17/docs/packages/cookbook/modifying-an-existing-package.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/receiving-webhooks.rst` & `steamship-2.7.17/docs/packages/cookbook/receiving-webhooks.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/return-audio.rst` & `steamship-2.7.17/docs/packages/cookbook/return-audio.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/return-image.rst` & `steamship-2.7.17/docs/packages/cookbook/return-image.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/return-json.rst` & `steamship-2.7.17/docs/packages/cookbook/return-json.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/cookbook/return-text.rst` & `steamship-2.7.17/docs/packages/cookbook/return-text.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/packages/developing/project-structure.rst` & `steamship-2.7.17/docs/packages/developing/project-structure.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Package Project Structure
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Your main implementation lives in the  ``src/api.py`` file of your project.
 This file will have been created for you by the template you selected when starting your project.
 
-- If you are developing a package, you will find a class that derives from the ``Invocable`` base class
+- If you are developing a package, you will find a class that derives from the ``PackageService`` base class
 - If you are developing a plugin, you will find a class that derives from a base class specific to the plugin type.
 
-In both cases, this ``src/api.py`` template concludes by setting a ``handler`` variable that is required by the Steamship bootloader for cloud operation.
-
 From the implementation perspective, think of a package as a Flask app.
 It looks and feels like a regular Python class,
 but its methods are decorated with decorators bind them to HTTP endpoints.
 You can call instances of your package over HTTP, or you can use a Steamship client library wrapper.
 
 Consider the following package:
 
 .. code-block:: python
 
-   class MyPackage(App):
-       @get("say_hello")
-       def _method_name_need_not_match(self, name: str = None) -> Response:
-           return Response(string=f"Hello, {name}")
-
-       @post("do_something")
-       def do_something(self, number: int = None) -> Response:
-           return Response(json={"number": number})
+    class MyPackage(PackageService):
+        @get("say_hello")
+        def _method_name_need_not_match(self, name: str = None) -> InvocableResponse:
+            return InvocableResponse(string=f"Hello, {name}")
+
+        @post("do_something")
+        def do_something(self, number: int = None) -> InvocableResponse:
+            return InvocableResponse(json={"number": number})
 
 Once deployed to Steamship, every new instance of this package would be associated with two HTTP endpoints:
 
 - Expose an HTTP GET endpoint at ``/say_hello`` that accepts a URL Querystring argument named ``name`` and returns a string response
 - Expose an HTTP POST endpoint at ``/do_something`` that accepts a random number and returns it in a JSON object
 
 These per-instance endpoints could also be called using convenience functions in the Steamship Python client:
@@ -48,7 +46,9 @@
 - The ``@get`` and ``@post`` decorators declare HTTP ``GET`` and ``POST`` endpoints, respectively
 - All method arguments **must be** kwargs with defaults
 - The method's kwargs will be supplied by merging URL query parameters, form-encoded POST data, and JSON-encoded POST data.
 - Binary input isn't yet supported. (Email us at hello@steamship.com for workarounds if you need one).
 - All methods must return a ``Response`` object
 
 For more examples of writing package endpoints, see the `example app <https://github.com/steamship-core/python-client/blob/main/tests/assets/apps/demo_app.py>`_ from our unit testing suite.
+
+You can also :ref:`define configuration parameters<Accepting Configuration>` for your package.
```

### Comparing `steamship-2.3.9/docs/packages/index.rst` & `steamship-2.7.17/docs/packages/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Packages
 ========
 
 `Steamship Packages <https://www.steamship.com/packages>`_ are cloud-hosted software libraries you can use in any programming environment.
 
 Think of them as regular software libraries with an upgrade:
 
-- **Packages bundle a full-lifecycle Language AI stack.**
+- **Packages bundle a full-lifecycle AI stack.**
   Everything necessary to go from demo to production in minutes: code, models, data, and infrastructure.
 
 - **Packages auto-manage their own infrastructure.**
   If a package depends on an embedding index or a fine-tuned model, you don't have to care.
 
 - **Packages are stateful.**
   You can create as many instances as you want: one per user, one per chat room, one per document folder. They remember their context.
```

### Comparing `steamship-2.3.9/docs/packages/using.rst` & `steamship-2.7.17/docs/packages/using.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 .. _UsingPackages:
 
 Using Packages
 --------------
 
 .. note::
-   Before you begin, make sure you've created your Steamship keys with:
-
-   .. code-block:: bash
-
-      npm install -g @steamship/cli && ship login
+   Before you begin, make sure you've set up your :ref:`authentication<Auth>`
 
    And installed a Steamship client library with:
 
     .. tab:: Python
 
         .. code-block:: bash
```

### Comparing `steamship-2.3.9/docs/plugins/blockifiers/developing.rst` & `steamship-2.7.17/docs/plugins/developing/blockifiers.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/plugins/blockifiers/index.rst` & `steamship-2.7.17/docs/plugins/using/blockifiers/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 All data imported into Steamship must be first blockified before it can be used.
 
 You can use blockifiers when developing Steamship :ref:`packages`, in your own Python app code,
 or as one-off functions that convert data in the cloud.
 
 .. include:: ./using.rst
-.. include:: ./developing.rst
+
```

### Comparing `steamship-2.3.9/docs/plugins/developing/async-plugins.rst` & `steamship-2.7.17/docs/plugins/developing/async-plugins.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/docs/plugins/developing/project-structure.rst` & `steamship-2.7.17/docs/plugins/developing/project-structure.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Plugin Project Structure
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Your main implementation lives in the  ``src/api.py`` file of your project.
 This file will have been created for you by the template you selected when starting your project.
 
 Inside this file, you will find a class that derives from a base class specific to the plugin type.
-At the end of this file you will find a ``handler`` export that is required by the Steamship bootloader for cloud operation.
 
 From the implementation perspective, think of a plugin as a class that implements an Abstract Base Class that the Steamship Engine knows how to communicate with.
 Each plugin type implements an abstract base class with a different contract.
 
 Consider the following tagger plugin:
 
 .. code-block:: python
@@ -20,7 +19,9 @@
         file.tags.append(
           Tag.CreateRequest(kind="Demo", name="You've been tagged!")
         )
         return BlockAndTagPluginOutput(file=file)
 
 Once deployed to Steamship, this plugin can be applied to files in Steamship, leaving each one with a tag that can be
 queried later.
+
+You can also :ref:`define configuration parameters<Accepting Configuration>` for your plugin.
```

### Comparing `steamship-2.3.9/docs/workspaces/data_model/tags.rst` & `steamship-2.7.17/docs/data/tags.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .. _Tags:
 
 Tags
 ~~~~
 
-Steamship uses Tags to represent all commentary about text.
+Steamship uses Tags to represent all commentary about content.
 
 - The intent of a chat message
 - The embedding of a sentence
 - The sentiment of a phase
-- THe markdown semantics of a region of text
+- The markdown semantics of a region of text
+- Identified object regions of an image
 
-Steamship Files and Blocks are mostly semantics-free containers.
-Tags are where all the action is.
+Steamship Files and Blocks contain content. Tags hold all data **about** the content.
 
 The full :py:class:`Tag PyDoc spec is here<steamship.data.tags.tag.Tag>`, but it's useful to look at a summarized version:
 
 .. code-block:: python
 
    class Tag:
      """Subset of the Tag object -- within the context of a Block"""
@@ -26,17 +26,16 @@
      value: Optional[Dict]
 
      # The span of text the tag is commenting upon.
      # Indices are relative to the block's text.
      start_idx: Optional[int] # Start inclusive
      end_idx: Optional[int]   # End exclusive
 
-This design results in an extraordinarily flexible data storage scheme that can be adapted to a number of
-different scenarios.
-In the Engine, we optimize our data storage so that you can query over tags and their contents.
+This design results in a flexible data storage scheme that can be adapted to a number of
+different scenarios. We optimize our data storage so that you can query over tags and their contents.
 
 Ways to use Tags
 ^^^^^^^^^^^^^^^^
 
 Here are a few examples to help you think of how tags are used.
 The ``start_idx`` and ``end_idx`` have been left out of the pseudo-code below.
 
@@ -78,33 +77,34 @@
 
 Tag Schemas
 ^^^^^^^^^^^
 
 Steamship brings together many models under one roof using tags as the common representation for interoperation.
 But doesn't fully solve the model interop problem: how do we make sure all models use the same tags?
 
-Our answer to this is to converge -- where possible -- upon a common schema for the ``kind``, ``name``, and ``value`` properties of a tag.
-If all sentiment models emit a tag with kind ``sentiment`` and a range of names ``[positive, neutral, negative]``, for example, then we can swap them in and out as it suits us.
+Where possible, we use a common schema for the ``kind``, ``name``, and ``value`` properties of a tag.
+If all sentiment models produce tags with kind ``sentiment`` and a range of names ``[positive, neutral, negative]``, for example, then we can swap them in and out as needed.
 
 Our ongoing pursuit of this can be found in the `tag_constants.py file <https://github.com/steamship-core/python-client/blob/main/src/steamship/data/tags/tag_constants.py>`_
 in Github.
-There you will find Python Enum classes that we curate as we encounter common domains across our plugins.
+There you will find Python Enum classes that have common tags across our plugins.
 
 - :py:class:`TagKind class<steamship.data.tags.tag_constants.TagKind>` contains suggested values for the ``kind`` field of a Tag.
 - :py:class:`TagValue class<steamship.data.tags.tag_constants.TagValue>` contains suggested keys for the ``valu`` dictionary of a Tag.
 - The following classes contain suggested values for the ``name`` field:
 
   - :py:class:`DocTag<steamship.data.tags.tag_constants.DocTag>` for document semantics (HTML, Markdown, OCR, etc)
   - :py:class:`EmotionTag<steamship.data.tags.tag_constants.EmotionTag>` for emotion tagging tag
   - :py:class:`EntityTag<steamship.data.tags.tag_constants.EntityTag>` for entity tagging tags
   - :py:class:`GenerationTag<steamship.data.tags.tag_constants.GenerationTag>` for models which generate new data from the covered span as input
   - :py:class:`IntentTag<steamship.data.tags.tag_constants.IntentTag>` for intent classification
   - :py:class:`SentimentTag<steamship.data.tags.tag_constants.SentimentTag>` for sentiment classification
+  - :py:class:`RoleTag<steamship.data.tags.tag_constants.RoleTag>` for role classification
 
-These constants are by no means required, but using them increases the chance that what you build will
+These constants are not required, but using them increases the chance that what you build will
 interoperate cleanly with everyone else that uses them.
 
 Here is what some of the above tag examples would look like using these enum classes.
 Notice how it is a combination of standard constant and "magic string" depending on whether a constant exists for that concept.
 
 - An entity
 
@@ -159,15 +159,13 @@
 - They are attached to the :ref:`File<Files>` object (``file.tags``)
 - Their ``block_id``, ``start_idx``, and ``end_idx`` are always null.
 - They are referenced via the ``filetag`` keyword in our query system.
 
 **Block Tags** annotate text within a :ref:`Block<Blocks>` object:
 
 - They are attached to the :ref:`Block<Blocks>` object (``block.tags``)
-- Their ``start_idx`` and ``end_idx`` fields are non-null. They  represent offsets into the text that is spanned by that block.
-- They are referenced via the ``blocktag`` keyword in our query system.
+- Their ``start_idx`` and ``end_idx`` fields are either both null or both non-null. If both are null, the ``Tag is assumed to apply to the whole ``Block``. They  represent offsets into the text that is spanned by that block.
+- They are referenced via the ``blocktag`` keyword in our :ref:`query system<queries>`.
 
-There are a few edge cases important to call out here:
+Notes:
 
-- Whereas file tags annotate the file itself, block tags do not annotate the block: they annotate text within the block.
-- A block tag that covers the entire text of the block always has ``start_idx = 0`` and ``end_idx = len(block.text)``
-- It is impossible for a tag to cover text spanning multiple blocks. This is a limitation of our current data model.
+- It is impossible for a tag to cover text spanning multiple blocks.
```

### Comparing `steamship-2.3.9/docs/workspaces/importing.rst` & `steamship-2.7.17/src/steamship/invocable/mixins/indexer_pipeline_mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,89 @@
-.. _Importing Data:
+from typing import Optional
 
-Importing Data
---------------
+from steamship import File, Steamship, Task
+from steamship.invocable import PackageService, post
+from steamship.invocable.mixins.blockifier_mixin import BlockifierMixin
+from steamship.invocable.mixins.file_importer_mixin import FileImporterMixin
+from steamship.invocable.mixins.indexer_mixin import IndexerMixin
+from steamship.invocable.package_mixin import PackageMixin
+from steamship.utils.file_tags import update_file_status
+
+
+class IndexerPipelineMixin(PackageMixin):
+    """Provides a complete set of endpoints & async workflow for Document Question Answering.
+
+    This Mixin is an async orchestrator of other mixins:
+    - Importer Mixin:       to import files, e.g. YouTube videos, PDF urls
+    - Blockifier Mixin:     to convert files to Blocks -- whether that's s2t or PDF parsing, etc.
+    - Indexer Mixin:        to convert Steamship Files to embedded sharts
+
+    """
+
+    client: Steamship
+    invocable: PackageService
+    blockifier_mixin: BlockifierMixin
+    importer_mixin: FileImporterMixin
+    indexer_mixin: IndexerMixin
+
+    def __init__(self, client: Steamship, invocable: PackageService):
+        self.client = client
+        self.invocable = invocable
+
+        self.importer_mixin = FileImporterMixin(client)
+        self.invocable.add_mixin(self.importer_mixin)
+
+        self.blockifier_mixin = BlockifierMixin(client)
+        self.invocable.add_mixin(self.blockifier_mixin)
+
+        self.indexer_mixin = IndexerMixin(client)
+        self.invocable.add_mixin(self.indexer_mixin)
+
+    @post("/set_file_status")
+    def set_file_status(self, file_id: str, status: str) -> bool:
+        """Set the status bit of a file. Intended to be scheduled after import."""
+        file = File.get(self.client, _id=file_id)
+        update_file_status(self.client, file, status)
+        return True
+
+    @post("/index_url")
+    def index_url(
+        self,
+        url: str,
+        metadata: Optional[dict] = None,
+        index_handle: Optional[str] = None,
+        mime_type: Optional[str] = None,
+    ) -> Task:
+        # Step 1: Import the URL
+        file, task = self.importer_mixin.import_url_to_file_and_task(url)
+
+        # Step 2: Blockify the File
+        importer_task_id = None
+        if task and task.task_id:
+            importer_task_id = task.task_id
+
+        blockify_task = self.blockifier_mixin.blockify(
+            file_id=file.id, mime_type=mime_type, after_task_id=importer_task_id
+        )
+
+        # Step 3: Index the File
+        index_task = self.invocable.invoke_later(
+            method="index_file",
+            wait_on_tasks=[blockify_task],
+            arguments={
+                "file_id": file.id,
+                "index_handle": index_handle,
+            },
+        )
+
+        # Step 4: Set the File Status to 'indexed'
+        self.invocable.invoke_later(
+            method="set_file_status",
+            wait_on_tasks=[index_task],
+            arguments={
+                "file_id": file.id,
+                "status": "Indexed",
+            },
+        )
 
-Importing content to your Workspace is the first step to processing it.
-Here are some ways to do it:
-
-- :ref:`Import content directly<Import content directly>`
-- :ref:`Import content via a Plugin<Import content via a Plugin>`
-
-Each of these methods always results in a new  :ref:`File<Files>` object.
-**But you can't use it yet!**
-After you import a File, you must :ref:`Blockify<Blockifying Data>` to transform it into Steamship format.
-
-.. _Import content directly:
-
-Import content directly
-^^^^^^^^^^^^^^^^^^^^^^^
-
-Import a file on disk with the ``File.create`` method.
-
-If you pass a ``content`` argument to this method, a file will be created from the provided string.
-An optional ``mime_type`` argument can also be provided.
-
-.. tab:: Python
-
-    .. code-block:: python
-
-       import { Steamship, MimeTypes } from "@steamship/client"
-       client = Steamship()
-
-       file = File.create(
-          client=client,
-          content="String content",
-          mime_type=MimeTypes.MKD
-       )
-
-
-For local files, ``content`` can be supplied via` ``read()``. If the file is a binary file, you may want to supply
-a custom MIME type, via the ``mime_type`` parameter.
-
-If you pass a ``blocks`` argument to this method, you can provided structured, pre-created :ref:`Blocks`,
-removing the need to :ref:`blockify<Blockifiers>` your file later.
-
-.. tab:: Python
-
-    .. code-block:: python
-
-       import { Steamship, MimeTypes } from "@steamship/client"
-       client = Steamship()
-
-       file = File.create(
-          client=client,
-          blocks=Block.CreateRequest(...)
-       )
-
-.. _Import content via a Plugin:
-
-Import content via a Plugin
-^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-:ref:`Importer Plugins<File Importers>` provide a way to perform more complex imports to Steamship.
-
-For example, a Notion File Importer might implement the logic necessary to authenticate against Notion and fetch the data corresponding to a particular page.
-This might be paired with a Notion File Blockifier that converts Notion's API response format into :ref:`Steamship Block Format<Data Model>`
-
-To import a file via a Plugin, first create an instance of the plugin in your workspace and then provide that instance to the ``File.create_with_plugin`` command.
-Unlike importing a file directly, importing a file via an :ref:`Importer plugins<File Importers>` returns a ``Task`` object.
-
-.. tab:: Python
-
-    .. code-block:: python
-
-       import { Steamship } from "@steamship/client"
-       client = Steamship()
-
-       importer = client.use_plugin("importer-plugin-handle")
-       task = File.create_with_plugin(
-          client=client,
-          plugin_instance=importer.handle
-       )
-       task.wait()
-
-       # Refresh the file from remote
-       file = file.refresh()
+        # We return the index task instead of the file set task just to safe a few seconds.
+        return index_task
```

### Comparing `steamship-2.3.9/docs/workspaces/queries/index.rst` & `steamship-2.7.17/docs/data/queries/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Queries
 -------
 
 Steamship contains a query language, **ShipQL**, designed to help you fetch Files, Blocks, and Tags.
 ShipQL enables you to query the results of multiple AI models applied to the same text, to find files or sections identified by language AI features.
 
-ShipQL Version 1 supports only the criteria on which objects are matched (like a SQL WHERE clause).
+ShipQL currently supports only the criteria on which objects are matched (like a SQL WHERE clause).
 It does not yet support projection and selection (like the SQL SELECT clause).
 
 Usage
 ~~~~~
 
 File, Block, and Tag objects are all queryable via ShipQL.
 Their objects in the Python Client have a static ``query`` method which accepts a ShipQL string.
```

### Comparing `steamship-2.3.9/pyproject.toml` & `steamship-2.7.17/pyproject.toml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/requirements.dev.txt` & `steamship-2.7.17/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/__init__.py` & `steamship-2.7.17/src/steamship/__init__.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/base/client.py` & `steamship-2.7.17/src/steamship/base/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 import logging
 import typing
 from abc import ABC
+from datetime import datetime, timedelta
 from inspect import isclass
-from typing import Any, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import inflection
 from pydantic import BaseModel, PrivateAttr
 from requests import Session
 
 from steamship.base.configuration import Configuration
 from steamship.base.error import SteamshipError
 from steamship.base.mime_types import MimeTypes
 from steamship.base.model import CamelModel, to_camel
 from steamship.base.request import Request
 from steamship.base.tasks import Task, TaskState
 from steamship.utils.url import Verb, is_local
 
-_logger = logging.getLogger(__name__)
-
 T = TypeVar("T")  # TODO (enias): Do we need this?
 
 
 def _multipart_name(path: str, val: Any) -> List[Tuple[Optional[str], str, Optional[str]]]:
     """Decode any object into a series of HTTP Multi-part segments that Vapor will consume.
 
     https://github.com/vapor/multipart-kit
@@ -184,20 +183,36 @@
         logging.info(f"[Client] Switched to workspace {return_handle}/{return_id}")
 
     def dict(self, **kwargs) -> dict:
         # Because of the trick we do to hack these in as both static and member methods (with different
         # implementations), Pydantic will try to include them by default. So we have to suppress that otherwise
         # downstream serialization into JSON will fail.
         if "exclude" not in kwargs:
-            kwargs["exclude"] = {"use", "use_plugin", "_instance_use", "_instance_use_plugin"}
+            kwargs["exclude"] = {
+                "use": True,
+                "use_plugin": True,
+                "_instance_use": True,
+                "_instance_use_plugin": True,
+                "config": {"api_key"},
+            }
         elif isinstance(kwargs["exclude"], set):
             kwargs["exclude"].add("use")
             kwargs["exclude"].add("use_plugin")
             kwargs["exclude"].add("_instance_use")
             kwargs["exclude"].add("_instance_use_plugin")
+            kwargs["exclude"].add(
+                "config"
+            )  # the set version cannot exclude subcomponents; we must remove all config
+        elif isinstance(kwargs["exclude"], dict):
+            kwargs["exclude"]["use"] = True
+            kwargs["exclude"]["use_plugin"] = True
+            kwargs["exclude"]["_instance_use"] = True
+            kwargs["exclude"]["_instance_use_plugin"] = True
+            kwargs["exclude"]["config"] = {"api_key"}
+
         return super().dict(**kwargs)
 
     def _url(
         self,
         is_package_call: bool = False,
         package_owner: str = None,
         operation: str = None,
@@ -232,47 +247,65 @@
         self,
         is_package_call: bool = False,
         package_owner: str = None,
         package_id: str = None,
         package_instance_id: str = None,
         as_background_task: bool = False,
         wait_on_tasks: List[Union[str, Task]] = None,
+        task_delay_ms: Optional[int] = None,
     ):
-        headers = {"Authorization": f"Bearer {self.config.api_key}"}
+        headers = {"Authorization": f"Bearer {self.config.api_key.get_secret_value()}"}
 
         if self.config.workspace_id:
             headers["X-Workspace-Id"] = self.config.workspace_id
         elif self.config.workspace_handle:
             headers["X-Workspace-Handle"] = self.config.workspace_handle
 
         if is_package_call:
             if package_owner:
                 headers["X-Package-Owner-Handle"] = package_owner
             if package_id:
                 headers["X-Package-Id"] = package_id
             if package_instance_id:
                 headers["X-Package-Instance-Id"] = package_instance_id
 
-        if wait_on_tasks:
+        if task_delay_ms and task_delay_ms < 0:
+            raise SteamshipError(
+                message=f"Unable to wait a negative duration of time (task_delay_ms={task_delay_ms})"
+            )
+
+        if wait_on_tasks or (task_delay_ms and task_delay_ms > 0):
             # Will result in the engine persisting the inbound HTTP request as a Task for deferred
             # execution. Additionally, the task will be scheduled to first wait on the other tasks
             # provided in the list of IDs. Accepts a list of EITHER Task objects OR task_id strings.
             as_background_task = True
-            task_ids = []
-            for task_or_id in wait_on_tasks:
-                if isinstance(task_or_id, str):
-                    task_ids.append(task_or_id)
-                elif isinstance(task_or_id, Task):
-                    task_ids.append(task_or_id.task_id)
-                else:
-                    raise SteamshipError(
-                        message=f"`wait_on_tasks` should only contain Task or str objects. Got a {type(task_or_id)}."
-                    )
+            if wait_on_tasks:
+                task_ids = []
+                for task_or_id in wait_on_tasks:
+                    if isinstance(task_or_id, str):
+                        task_ids.append(task_or_id)
+                    elif isinstance(task_or_id, Task):
+                        task_ids.append(task_or_id.task_id)
+                    else:
+                        raise SteamshipError(
+                            message=f"`wait_on_tasks` should only contain Task or str objects. Got a {type(task_or_id)}."
+                        )
+                headers["X-Task-Dependency"] = ",".join(task_ids)
 
-            headers["X-Task-Dependency"] = ",".join(task_ids)
+            if task_delay_ms and task_delay_ms > 0:
+                # Note: we're calling utcnow so that a few lines below we can add +00:00 without worrying about TZ
+                current_date_utc = datetime.utcnow()
+                future_date = current_date_utc + timedelta(milliseconds=task_delay_ms)
+
+                # The engine won't parse it if it includes microseconds.
+                future_date = future_date.replace(microsecond=0)
+
+                # Python doesn't add the +00:00 UTC string, which violates the standard; the Engine will refuse.
+                future_date_str = f"{future_date.isoformat()}+00:00"
+                headers["X-Task-Run-After"] = future_date_str
 
         if as_background_task:
             # Will result in the engine persisting the inbound HTTP request as a Task for deferred
             # execution. The client will receive task information back instead of the synchronous API response.
             # That task can be polled for eventual completion.
             headers["X-Task-Background"] = "true"
 
@@ -378,14 +411,16 @@
         raw_response: bool = False,
         is_package_call: bool = False,
         package_owner: str = None,
         package_id: str = None,
         package_instance_id: str = None,
         as_background_task: bool = False,
         wait_on_tasks: List[Union[str, Task]] = None,
+        timeout_s: Optional[float] = None,
+        task_delay_ms: Optional[int] = None,
     ) -> Union[
         Any, Task
     ]:  # TODO (enias): I would like to list all possible return types using interfaces instead of Any
         """Post to the Steamship API.
 
         All responses have the format::
 
@@ -409,29 +444,30 @@
         headers = self._headers(
             is_package_call=is_package_call,
             package_owner=package_owner,
             package_id=package_id,
             package_instance_id=package_instance_id,
             as_background_task=as_background_task,
             wait_on_tasks=wait_on_tasks,
+            task_delay_ms=task_delay_ms,
         )
 
         data = self._prepare_data(payload=payload)
 
         logging.debug(
             f"Making {verb} to {url} in workspace {self.config.workspace_handle}/{self.config.workspace_id}"
         )
         if verb == Verb.POST:
             if file is not None:
                 files = self._prepare_multipart_data(data, file)
-                resp = self._session.post(url, files=files, headers=headers)
+                resp = self._session.post(url, files=files, headers=headers, timeout=timeout_s)
             else:
-                resp = self._session.post(url, json=data, headers=headers)
+                resp = self._session.post(url, json=data, headers=headers, timeout=timeout_s)
         elif verb == Verb.GET:
-            resp = self._session.get(url, params=data, headers=headers)
+            resp = self._session.get(url, params=data, headers=headers, timeout=timeout_s)
         else:
             raise Exception(f"Unsupported verb: {verb}")
 
         logging.debug(f"From {verb} to {url} got HTTP {resp.status_code}")
 
         if debug is True:
             logging.debug(f"Got response {resp}")
@@ -488,16 +524,30 @@
         else:
             data = response_data
 
         if error is not None:
             logging.warning(f"Client received error from server: {error}", exc_info=error)
             raise error
 
+        if not resp.ok:
+            raise SteamshipError(
+                f"API call did not complete successfully.  Server returned: {response_data}"
+            )
+
         elif task is not None:
             return task
+        elif data is not None and expect is not None:
+            # if we have data AND we expect it to be of a certain type,
+            # we should probably make sure that expectation is met.
+            if not isinstance(data, expect):
+                raise SteamshipError(
+                    message=f"Inconsistent response from server (data does not match expected type: {expect}.)",
+                    suggestion="Please contact support via hello@steamship.com and report what caused this error.",
+                )
+            return data
         elif data is not None:
             return data
         else:
             raise SteamshipError("Inconsistent response from server. Please contact support.")
 
     def post(
         self,
@@ -509,14 +559,16 @@
         raw_response: bool = False,
         is_package_call: bool = False,
         package_owner: str = None,
         package_id: str = None,
         package_instance_id: str = None,
         as_background_task: bool = False,
         wait_on_tasks: List[Union[str, Task]] = None,
+        timeout_s: Optional[float] = None,
+        task_delay_ms: Optional[int] = None,
     ) -> Union[
         Any, Task
     ]:  # TODO (enias): I would like to list all possible return types using interfaces instead of Any
         return self.call(
             verb=Verb.POST,
             operation=operation,
             payload=payload,
@@ -526,14 +578,16 @@
             raw_response=raw_response,
             is_package_call=is_package_call,
             package_owner=package_owner,
             package_id=package_id,
             package_instance_id=package_instance_id,
             as_background_task=as_background_task,
             wait_on_tasks=wait_on_tasks,
+            timeout_s=timeout_s,
+            task_delay_ms=task_delay_ms,
         )
 
     def get(
         self,
         operation: str,
         payload: Union[Request, dict] = None,
         file: Any = None,
@@ -542,14 +596,16 @@
         raw_response: bool = False,
         is_package_call: bool = False,
         package_owner: str = None,
         package_id: str = None,
         package_instance_id: str = None,
         as_background_task: bool = False,
         wait_on_tasks: List[Union[str, Task]] = None,
+        timeout_s: Optional[float] = None,
+        task_delay_ms: Optional[int] = None,
     ) -> Union[
         Any, Task
     ]:  # TODO (enias): I would like to list all possible return types using interfaces instead of Any
         return self.call(
             verb=Verb.GET,
             operation=operation,
             payload=payload,
@@ -559,8 +615,48 @@
             raw_response=raw_response,
             is_package_call=is_package_call,
             package_owner=package_owner,
             package_id=package_id,
             package_instance_id=package_instance_id,
             as_background_task=as_background_task,
             wait_on_tasks=wait_on_tasks,
+            timeout_s=timeout_s,
+            task_delay_ms=task_delay_ms,
         )
+
+    def logs(
+        self,
+        offset: int = 0,
+        number: int = 50,
+        invocable_handle: Optional[str] = None,
+        instance_handle: Optional[str] = None,
+        invocable_version_handle: Optional[str] = None,
+        path: Optional[str] = None,
+        field_values: Optional[Dict[str, str]] = None,
+    ) -> Dict[str, Any]:
+        """Return generated logs for a client.
+
+        The logs will be workspace-scoped. You will only receive logs
+        for packages and plugins that you own.
+
+        :param offset: The index of the first log entry to return. This can be used with `number` to page through logs.
+        :param number: The number of log entries to return. This can be used with `offset` to page through logs.
+        :param invocable_handle: Enables optional filtering based on the handle of package or plugin. Example: `my-package`
+        :param instance_handle: Enables optional filtering based on the handle of package instance or plugin instance. Example: `my-instance`
+        :param invocable_version_handle: Enables optional filtering based on the version handle of package or plugin. Example: `0.0.2`
+        :param path: Enables optional filtering based on request path. Example: `/generate`.
+        :param field_values: Enables optional filtering based on user-provided field values.
+        :return: Returns a dictionary containing the offset and number of log entries as well as a list of `entries` that match the specificed filters.
+        """
+        args = {"from": offset, "size": number}
+        if invocable_handle:
+            args["invocableHandle"] = invocable_handle
+        if instance_handle:
+            args["invocableInstanceHandle"] = instance_handle
+        if invocable_version_handle:
+            args["invocableVersionHandle"] = invocable_version_handle
+        if path:
+            args["invocablePath"] = path
+        if field_values:
+            args["fieldValues"] = field_values
+
+        return self.post("logs/list", args)
```

### Comparing `steamship-2.3.9/src/steamship/base/configuration.py` & `steamship-2.7.17/src/steamship/base/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import json
 import os
 from pathlib import Path
 from typing import Optional
 
 import inflection
-from pydantic import HttpUrl
+from pydantic import HttpUrl, SecretStr
 
-from steamship.base.model import CamelModel
+from steamship.base.model import CamelModel, to_camel
 from steamship.cli.login import login
 from steamship.utils.utils import format_uri
 
 DEFAULT_WEB_BASE = "https://steamship.com/"
 DEFAULT_APP_BASE = "https://steamship.run/"
 DEFAULT_API_BASE = "https://api.steamship.com/api/v1/"
 
@@ -33,15 +33,15 @@
     "client": True,
     "blocks": {"__all__": {"client": True, "tags": {"__all__": {"client": True}}}},
     "tags": {"__all__": {"client": True}},
 }
 
 
 class Configuration(CamelModel):
-    api_key: str
+    api_key: SecretStr
     api_base: HttpUrl = DEFAULT_API_BASE
     app_base: HttpUrl = DEFAULT_APP_BASE
     web_base: HttpUrl = DEFAULT_WEB_BASE
     workspace_id: str = None
     workspace_handle: str = None
     profile: Optional[str] = None
 
@@ -57,28 +57,29 @@
         config_dict = self._load_from_file(
             config_file or DEFAULT_CONFIG_FILE,
             profile,
             raise_on_exception=config_file is not None,
         )
         config_dict.update(self._get_config_dict_from_environment())
         kwargs.update({k: v for k, v in config_dict.items() if kwargs.get(k) is None})
+        kwargs = {to_camel(k): v for k, v in kwargs.items()}
 
-        kwargs["api_base"] = format_uri(kwargs.get("api_base"))
-        kwargs["app_base"] = format_uri(kwargs.get("app_base"))
-        kwargs["web_base"] = format_uri(kwargs.get("web_base"))
+        kwargs["apiBase"] = format_uri(kwargs.get("apiBase"))
+        kwargs["appBase"] = format_uri(kwargs.get("appBase"))
+        kwargs["webBase"] = format_uri(kwargs.get("webBase"))
 
-        if not kwargs.get("api_key") and not kwargs.get("apiKey"):
+        if not kwargs.get("apiKey"):
             api_key = login(
-                kwargs.get("api_base") or DEFAULT_API_BASE,
-                kwargs.get("web_base") or DEFAULT_WEB_BASE,
+                kwargs.get("apiBase") or DEFAULT_API_BASE,
+                kwargs.get("webBase") or DEFAULT_WEB_BASE,
             )
             Configuration._save_api_key_to_file(
                 api_key, profile, config_file or DEFAULT_CONFIG_FILE
             )
-            kwargs["api_key"] = api_key
+            kwargs["apiKey"] = api_key
 
         super().__init__(**kwargs)
 
     @staticmethod
     def _load_from_file(
         file: Path, profile: str = None, raise_on_exception: bool = False
     ) -> Optional[dict]:
```

### Comparing `steamship-2.3.9/src/steamship/base/environments.py` & `steamship-2.7.17/src/steamship/base/environments.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/base/error.py` & `steamship-2.7.17/src/steamship/base/error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/base/model.py` & `steamship-2.7.17/src/steamship/base/model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/base/tasks.py` & `steamship-2.7.17/src/steamship/base/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import time
-from typing import Any, Dict, Generic, List, Optional, Set, Type, TypeVar
+from typing import Any, Callable, Dict, Generic, List, Optional, Set, Type, TypeVar
 
 from pydantic import BaseModel, Field
 
 from steamship.base.error import SteamshipError
 from steamship.base.model import CamelModel, GenericCamelModel
-from steamship.base.request import DeleteRequest, IdentifierRequest, Request
+from steamship.base.request import DeleteRequest, IdentifierRequest, ListRequest, Request, SortOrder
 from steamship.utils.metadata import metadata_to_str, str_to_metadata
 
+from .response import ListResponse
+
 T = TypeVar("T")
 
 
 class CreateTaskCommentRequest(Request):
     task_id: str
     external_id: str = None
     external_type: str = None
     external_group: str = None
     metadata: str = None
 
 
-class ListTaskCommentRequest(Request):
+class ListTaskCommentRequest(ListRequest):
     task_id: str = None
     external_id: str = None
     external_type: str = None
     external_group: str = None
 
 
 class TaskComment(CamelModel):
@@ -74,20 +76,26 @@
     @staticmethod
     def list(
         client: Client,
         task_id: str = None,
         external_id: str = None,
         external_type: str = None,
         external_group: str = None,
+        page_size: Optional[int] = None,
+        page_token: Optional[str] = None,
+        sort_order: Optional[SortOrder] = SortOrder.DESC,
     ) -> TaskCommentList:
         req = ListTaskCommentRequest(
             taskId=task_id,
             external_id=external_id,
             external_type=external_type,
             externalGroup=external_group,
+            page_size=page_size,
+            page_token=page_token,
+            sort_order=sort_order,
         )
         return client.post(
             "task/comment/list",
             req,
             expect=TaskCommentList,
         )
 
@@ -96,15 +104,15 @@
         return self.client.post(
             "task/comment/delete",
             req,
             expect=TaskComment,
         )
 
 
-class TaskCommentList(CamelModel):
+class TaskCommentList(ListResponse):
     comments: List[TaskComment]
 
 
 class TaskState:
     waiting = "waiting"
     running = "running"
     succeeded = "succeeded"
@@ -220,29 +228,54 @@
     def post_update(self, fields: Set[str] = None) -> Task:
         """Updates this task in the Steamship Engine."""
         if not isinstance(fields, set):
             raise RuntimeError(f'Unexpected type of "fields": {type(fields)}. Expected type set.')
         body = self.dict(by_alias=True, include={*fields, "task_id"})
         return self.client.post("task/update", body, expect=Task)
 
-    def wait(self, max_timeout_s: float = 60, retry_delay_s: float = 1):
-        """Polls and blocks until the task has succeeded or failed (or timeout reached)."""
+    def wait(
+        self,
+        max_timeout_s: float = 180,
+        retry_delay_s: float = 1,
+        on_each_refresh: "Optional[Callable[[int, float, Task], None]]" = None,
+    ):
+        """Polls and blocks until the task has succeeded or failed (or timeout reached).
+
+        Parameters
+        ----------
+        max_timeout_s : int
+            Max timeout in seconds. Default: 180s. After this timeout, an exception will be thrown.
+        retry_delay_s : float
+            Delay between status checks. Default: 1s.
+        on_each_refresh : Optional[Callable[[int, float, Task], None]]
+            Optional call back you can get after each refresh is made, including success state refreshes.
+            The signature represents: (refresh #, total elapsed time, task)
+
+            WARNING: Do not pass a long-running function to this variable. It will block the update polling.
+        """
         t0 = time.perf_counter()
+        refresh_count = 0
         while time.perf_counter() - t0 < max_timeout_s and self.state not in (
             TaskState.succeeded,
             TaskState.failed,
         ):
-            self.refresh()
             time.sleep(retry_delay_s)
+            self.refresh()
+            refresh_count += 1
+
+            # Possibly make a callback so the caller knows we've tried again
+            if on_each_refresh:
+                on_each_refresh(refresh_count, time.perf_counter() - t0, self)
 
         # If the task did not complete within the timeout, throw an error
         if self.state not in (TaskState.succeeded, TaskState.failed):
             raise SteamshipError(
-                message=f"Task {self.task_id} did not complete within requested timeout of {max_timeout_s}s"
+                message=f"Task {self.task_id} did not complete within requested timeout of {max_timeout_s}s. The task is still running on the server. You can retrieve its status via Task.get() or try waiting again with wait()."
             )
+        return self.output
 
     def refresh(self):
         if self.task_id is None:
             raise SteamshipError(message="Unable to refresh task because `task_id` is None")
 
         req = TaskStatusRequest(taskId=self.task_id)
         # TODO (enias): A status call can return both data and task
```

### Comparing `steamship-2.3.9/src/steamship/cli/cli.py` & `steamship-2.7.17/src/steamship/agents/mixins/transports/transport.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,87 @@
 import logging
-import sys
-from os import path
-
-import click
-
-import steamship
-from steamship import Steamship
-from steamship.base.configuration import Configuration
-from steamship.cli.deploy import PackageDeployer, bundle_deployable, update_config_template
-from steamship.cli.manifest_init_wizard import manifest_init_wizard
-from steamship.data.user import User
-from steamship.invocable.manifest import DeployableType, Manifest
-
-
-@click.group()
-def cli():
-    pass
-
-
-def initialize():
-    logging.root.setLevel(logging.FATAL)
-    click.echo(f"Steamship PYTHON cli version {steamship.__version__}")
-
-
-@click.command()
-def login():
-    initialize()
-    click.echo("Logging into Steamship.")
-    if sys.argv[1] == "login":
-        if Configuration.default_config_file_has_api_key():
-            overwrite = click.confirm(
-                text="You already have an API key in your .steamship.json file.  Do you want to remove it and login?",
-                default=False,
-            )
-            if not overwrite:
-                sys.exit(0)
-            Configuration.remove_api_key_from_default_config()
-
-        # Carry on with login
-        client = Steamship()
-        user = User.current(client)
-        click.secho(f"🚢🚢🚢 Hooray! You're logged in with user handle: {user.handle} 🚢🚢🚢", fg="green")
-
-
-@click.command()
-def deploy():
-    initialize()
-    client = Steamship()
-    user = User.current(client)
-    if path.exists("steamship.json"):
-        manifest = Manifest.load_manifest()
-    else:
-        manifest = manifest_init_wizard(client)
-        manifest.save()
-
-    deployable_type = manifest.type
-
-    update_config_template(manifest)
-
-    deployer = None
-    if deployable_type == DeployableType.PACKAGE:
-        deployer = PackageDeployer()
-    else:
-        click.secho(
-            "Sorry, this version of Steamship CLI can only deploy packages right now.", fg="red"
+import time
+from abc import ABC, abstractmethod
+from typing import List, Optional
+
+from steamship import Block, Steamship
+from steamship.agents.schema import AgentContext, Metadata
+from steamship.agents.tools.audio_transcription.assembly_speech_to_text_tool import (
+    AssemblySpeechToTextTool,
+)
+from steamship.invocable.package_mixin import PackageMixin
+
+
+class Transport(PackageMixin, ABC):
+    client = Steamship
+    """ Base class to encapsulate a communication channel mixin
+
+    Intended use is:
+
+        class MyBot(PackageService):
+
+               def __init__(
+                    self, client: Steamship, config: Dict[str, Any] = None, context: InvocationContext = None
+                ):
+                    super().__init__(client=client, config=config, context=context)
+                    self.agent = TestAgent()
+                self.add_mixin(
+                    TelegramTransport(
+                        client=client, config=self.config, agent_service=self, agent=self.agent
+                    )
+                )
+
+    """
+
+    def __init__(self, client):
+        self.client = client
+
+    def send(self, blocks: List[Block], metadata: Optional[Metadata] = None):
+        metadata = metadata or {}
+        if blocks is None or len(blocks) == 0:
+            logging.info(f"Skipping send of 0 blocks: {self.__class__.__name__}")
+            return
+
+        logging.info(f"Sending {len(blocks)} blocks: {self.__class__.__name__}")
+        start = time.time()
+        self._send(blocks, metadata)
+        end = time.time()
+        logging.info(
+            f"Sending {len(blocks)} blocks in {end - start} seconds: {self.__class__.__name__}"
         )
-        click.get_current_context().abort()
-
-    deployable = deployer.create_or_fetch_deployable(client, user, manifest)
-
-    click.echo("Bundling content... ", nl=False)
-    bundle_deployable(manifest)
-    click.echo("Done. 📦")
-
-    _ = deployer.create_version(client, manifest, deployable.id)
-
-    thing_url = f"{client.config.web_base}{deployable_type}s/{manifest.handle}"
-    click.echo(
-        f"Deployment was successful. View and share your new {deployable_type} here:\n\n{thing_url}\n"
-    )
-
-    # Common error conditions:
-    # - Package/plugin handle already taken. [handled; asks user for new]
-    # - Version handle already deployed. [handled; asks user for new]
-    # - Bad parameter configuration. [mitigated by deriving template from Config object]
-    # - Package content fails health check (ex. bad import) [Error caught while checking config object]
-
-
-cli.add_command(deploy)
-cli.add_command(login)
 
-if __name__ == "__main__":
-    deploy([])
+    @abstractmethod
+    def _send(self, blocks: List[Block], metadata: Metadata):
+        raise NotImplementedError
+
+    def parse_inbound(self, payload: dict, context: Optional[dict] = None) -> Optional[Block]:
+        message = self._parse_inbound(payload, context)
+
+        if message.url and not message.text:
+            context = AgentContext()
+            context.client = self.client
+            transcriptions = AssemblySpeechToTextTool(
+                blockifier_plugin_config={
+                    "enable_audio_intelligence": False,
+                    "speaker_detection": False,
+                }
+            ).run([Block(text=message.url)], context=context)
+            message.text = transcriptions[0].text
+        return message
+
+    @abstractmethod
+    def _parse_inbound(self, payload: dict, context: Optional[dict] = None) -> Optional[Block]:
+        raise NotImplementedError
+
+    def response_for_exception(
+        self, e: Optional[Exception], chat_id: Optional[str] = None
+    ) -> Block:
+        return_text = f"An error happened while creating a response: {e}"
+        if e is None:
+            return_text = "An unknown error happened. Please reach out to support@steamship.com or on our discord at https://steamship.com/discord"
+
+        if "usage limit" in f"{e}":
+            return_text = "You have reached the introductory limit of Steamship. Visit https://steamship.com/account/plan to sign up for a plan."
+
+        result = Block(text=return_text)
+        result.set_chat_id(chat_id)
+        return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `steamship-2.3.9/src/steamship/cli/deploy.py` & `steamship-2.7.17/src/steamship/cli/deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import importlib
 import os
-import traceback
 import zipfile
 from abc import ABC, abstractmethod
 from pathlib import Path
 
 import click
 from semver import VersionInfo
 
-from steamship import Package, PackageVersion, Steamship, SteamshipError
+from steamship import Package, PackageVersion, PluginVersion, Steamship, SteamshipError
 from steamship.cli.manifest_init_wizard import validate_handle, validate_version_handle
 from steamship.cli.ship_spinner import ship_spinner
+from steamship.cli.utils import find_api_py, get_api_module
+from steamship.data import Plugin
+from steamship.data.manifest import Manifest
 from steamship.data.user import User
 from steamship.invocable.lambda_handler import get_class_from_module
-from steamship.invocable.manifest import Manifest
 
 DEFAULT_BUILD_IGNORE = [
     "build",
     ".git",
     ".venv",
     ".ipynb_checkpoints",
     ".DS_Store",
@@ -26,33 +26,17 @@
     "examples",
     ".idea",
     "__pycache__",
 ]
 
 
 def update_config_template(manifest: Manifest):
-
-    path = Path("src/api.py")
-    if not path.exists():
-        path = Path("api.py")
-        if not path.exists():
-            raise SteamshipError("Could not find api.py either in root directory or in src.")
-
-    module = None
-    try:
-        module = importlib.machinery.SourceFileLoader("api", str(path)).load_module()
-    except Exception:
-        click.secho(
-            "An error occurred while loading your api.py to check configuration parameters. Full stack trace below.",
-            fg="red",
-        )
-        traceback.print_exc()
-        click.get_current_context().abort()
-
-    invocable_type = get_class_from_module(module)
+    path = find_api_py()
+    api_module = get_api_module(path)
+    invocable_type = get_class_from_module(api_module)
 
     config_parameters = invocable_type.config_cls().get_config_parameters()
 
     if manifest.configTemplate != config_parameters:
         if len(config_parameters) > 0:
             click.secho("Config parameters changed; updating steamship.json.", fg="cyan")
             for param_name, param in config_parameters.items():
@@ -107,18 +91,25 @@
         pass
 
     @abstractmethod
     def create_object(self, client: Steamship, manifest: Manifest):
         pass
 
     @abstractmethod
+    def update_object(self, deployable, client: Steamship, manifest: Manifest):
+        pass
+
+    @abstractmethod
     def deployable_type(self):
         pass
 
     def create_or_fetch_deployable(self, client: Steamship, user: User, manifest: Manifest):
+        if not manifest.handle or len(manifest.handle) == 0:
+            self.ask_for_new_handle(manifest, was_missing=True)
+
         deployable = None
         while deployable is None:
             click.echo(
                 f"Creating / fetching {self.deployable_type()} with handle [{manifest.handle}]... ",
                 nl=False,
             )
             try:
@@ -131,88 +122,143 @@
                     self.ask_for_new_handle(manifest)
                 else:
                     click.secho(
                         f"Unable to create / fetch {self.deployable_type()}. Server returned message: {e.message}"
                     )
                     click.get_current_context().abort()
 
+        self.update_object(deployable, client, manifest)
+
         click.echo("Done.")
         return deployable
 
-    def ask_for_new_handle(self, manifest: Manifest):
-        try_again = click.confirm(
-            click.style(
-                f"\nIt looks like that handle [{manifest.handle}] is already in use. Would you like to change the handle and try again?",
-                fg="yellow",
-            ),
-            default=True,
-        )
-        if try_again:
-            new_handle = click.prompt(
-                f"What handle would you like to use for your {self.deployable_type()}? Valid characters are a-z and -",
-                value_proc=validate_handle,
+    def ask_for_new_handle(self, manifest: Manifest, was_missing: bool = False):
+        if not was_missing:
+            try_again = click.confirm(
+                click.style(
+                    f"\nIt looks like that handle [{manifest.handle}] is already in use. Would you like to change the handle and try again?",
+                    fg="yellow",
+                ),
+                default=True,
             )
-            manifest.handle = new_handle
-            manifest.save()
-        else:
-            click.get_current_context().abort()
+            if not try_again:
+                click.get_current_context().abort()
+
+        new_handle = click.prompt(
+            f"What handle would you like to use for your {self.deployable_type()}? Valid characters are a-z and -",
+            value_proc=validate_handle,
+        )
+        manifest.handle = new_handle
+        manifest.save()
 
     def create_version(self, client: Steamship, manifest: Manifest, thing_id: str):
         version = None
+
+        if not manifest.version or len(manifest.version) == 0:
+            self.ask_for_new_version_handle(manifest, was_missing=True)
+
         while version is None:
             click.echo(f"Deploying version {manifest.version} of [{manifest.handle}]... ", nl=False)
             try:
                 with ship_spinner():
                     version = self._create_version(client, manifest, thing_id)
             except SteamshipError as e:
-                if e.message == "The object you are trying to create already exists.":
+                if "The object you are trying to create already exists." in e.message:
                     self.ask_for_new_version_handle(manifest)
                 else:
-                    click.secho(
-                        f"Unable to create / fetch {self.deployable_type()}. Server returned message: {e.message}"
-                    )
+                    click.secho(f"\nUnable to deploy {self.deployable_type()} version.", fg="red")
+                    click.secho(f"Server returned message: {e.message}")
+                    if "ModuleNotFoundError" in e.message:
+                        click.secho(
+                            "It looks like you may be missing a dependency in your requirements.txt.",
+                            fg="yellow",
+                        )
                     click.get_current_context().abort()
         click.echo("\nDone. 🚢")
 
-    def ask_for_new_version_handle(self, manifest: Manifest):
-        try_again = click.confirm(
-            click.style(
-                f"\nIt looks like that version [{manifest.version}] has already been deployed. Would you like to change the version handle and try again?",
-                fg="yellow",
-            ),
-            default=True,
-        )
-        if try_again:
-            default_new = "1.0.0"
-            try:
-                default_new = str(VersionInfo.parse(manifest.version).bump_prerelease())
-            except ValueError:
-                pass
-            old_archive_path = get_archive_path(manifest)
-            new_version_handle = click.prompt(
-                "What should the new version be? Valid characters are a-z, 0-9, . and -",
-                value_proc=validate_version_handle,
-                default=default_new,
+    def ask_for_new_version_handle(self, manifest: Manifest, was_missing: bool = False):
+        if not was_missing:
+            try_again = click.confirm(
+                click.style(
+                    f"\nIt looks like that version [{manifest.version}] has already been deployed. Would you like to change the version handle and try again?",
+                    fg="yellow",
+                ),
+                default=True,
             )
-            manifest.version = new_version_handle
-            manifest.save()
-            new_archive_path = get_archive_path(manifest)
-            old_archive_path.rename(new_archive_path)
-        else:
-            click.get_current_context().abort()
+            if not try_again:
+                click.get_current_context().abort()
+
+        default_new = "1.0.0"
+        try:
+            default_new = str(VersionInfo.parse(manifest.version).next_version("prerelease"))
+        except ValueError:
+            pass
+        old_archive_path = get_archive_path(manifest)
+        new_version_handle = click.prompt(
+            "What should the new version be? Valid characters are a-z, 0-9, . and -",
+            value_proc=validate_version_handle,
+            default=default_new,
+        )
+        manifest.version = new_version_handle
+        manifest.save()
+        new_archive_path = get_archive_path(manifest)
+        old_archive_path.rename(new_archive_path)
 
 
 class PackageDeployer(DeployableDeployer):
     def _create_version(self, client: Steamship, manifest: Manifest, thing_id: str):
         return PackageVersion.create(
             client=client,
             config_template=manifest.config_template_as_dict(),
             handle=manifest.version,
             filename=f"build/archives/{manifest.handle}_v{manifest.version}.zip",
             package_id=thing_id,
         )
 
     def create_object(self, client: Steamship, manifest: Manifest):
-        return Package.create(client, handle=manifest.handle, fetch_if_exists=True)
+        return Package.create(
+            client,
+            handle=manifest.handle,
+            profile=manifest,
+            is_public=manifest.public,
+            fetch_if_exists=True,
+        )
+
+    def update_object(self, deployable, client: Steamship, manifest: Manifest):
+        deployable.profile = manifest
+
+        package = deployable.update(client)
+        return package
 
     def deployable_type(self):
         return "package"
+
+
+class PluginDeployer(DeployableDeployer):
+    def _create_version(self, client: Steamship, manifest: Manifest, thing_id: str):
+        return PluginVersion.create(
+            client=client,
+            config_template=manifest.config_template_as_dict(),
+            handle=manifest.version,
+            filename=f"build/archives/{manifest.handle}_v{manifest.version}.zip",
+            plugin_id=thing_id,
+        )
+
+    def create_object(self, client: Steamship, manifest: Manifest):
+        return Plugin.create(
+            client,
+            description=manifest.description,
+            is_public=manifest.public,
+            transport=manifest.plugin.transport,
+            type_=manifest.plugin.type,
+            handle=manifest.handle,
+            fetch_if_exists=True,
+        )
+
+    def update_object(self, deployable, client: Steamship, manifest: Manifest):
+        deployable.profile = manifest
+
+        plugin = deployable.update(client)
+        return plugin
+
+    def deployable_type(self):
+        return "plugin"
```

### Comparing `steamship-2.3.9/src/steamship/cli/login.py` & `steamship-2.7.17/src/steamship/cli/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import webbrowser
 
 import requests
 
 from steamship.base.error import SteamshipError
+from steamship.cli.utils import is_in_replit
 
 
 def login(api_base: str, web_base: str) -> str:  # noqa: C901
 
     # create login token
     try:
         token_result = requests.post(api_base + "account/create_login_attempt")
@@ -21,22 +22,33 @@
     if token is None:
         raise SteamshipError("Could not create login token when attempting login.")
 
     # Launch login attempt in browser
     login_browser_url = (
         f"{web_base}account/client-login?attemptToken={token}&client=pycli&version=0.0.1"
     )
-    try:
-        opened_browser = webbrowser.open(login_browser_url)
-    except Exception as e:
-        raise SteamshipError("Exception attempting to launch browser for login.", error=e)
+
+    opened_browser = False
+    if not is_in_replit():
+        try:
+            opened_browser = webbrowser.open(login_browser_url)
+        except Exception as e:
+            raise SteamshipError("Exception attempting to launch browser for login.", error=e)
 
     if not opened_browser:
         raise SteamshipError(
-            "Could not launch browser for login flow. If you are in Replit or another headless environment, please set your Steamship API key as an environment variable or in steamship.json.  See more here: https://docs.steamship.com/configuration/authentication.html"
+            """Could not launch browser to log in to Steamship.
+
+If you are in Replit:
+
+1) Get an API key at https://steamship.com/account/api
+2) Set the STEAMSHIP_API_KEY Replit Secret
+3) Close and reopen this shell so that secrets refresh
+
+If you are in a different headless environment, visit https://docs.steamship.com/configuration/authentication.html"""
         )
 
     # Wait on result
     total_poll_time_s = 0
     time_between_polls_s = 1
     api_key = None
     while total_poll_time_s < 300:  # Five minutes
```

### Comparing `steamship-2.3.9/src/steamship/cli/manifest_init_wizard.py` & `steamship-2.7.17/src/steamship/cli/manifest_init_wizard.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 import click
 from click import BadParameter
 
 from steamship import Steamship
+from steamship.data.manifest import Manifest, PluginConfig, SteamshipRegistry
 from steamship.data.user import User
-from steamship.invocable.manifest import Manifest, SteamshipRegistry
 
 
 def validate_handle(handle: str) -> str:
     if re.fullmatch(r"[a-z\-]+", handle) is not None:
         return handle
     else:
         raise BadParameter("Handle must only include lowercase letters and -")
@@ -40,14 +40,30 @@
         value_proc=validate_handle,
     )
 
     # TODO: claim the handle right here!
 
     version_handle = "0.0.1"
 
+    plugin_detail = None
+    if deployable_type == "plugin":
+        plugin_type = click.prompt(
+            "What type of plugin is this?",
+            default="tagger",
+            type=click.Choice(
+                ["tagger", "blockifier", "exporter", "fileImporter", "corpusImporter", "generator"]
+            ),
+            show_choices=True,
+        )
+        if plugin_type == "tagger":
+            trainable = click.confirm("Is the plugin trainable?", default=False)
+        else:
+            trainable = False
+        plugin_detail = PluginConfig(isTrainable=trainable, type=plugin_type)
+
     public = click.confirm(f"Do you want this {deployable_type} to be public?", default=True)
 
     user = User.current(client)
 
     author = click.prompt("How should we list your author name?", default=user.handle)
 
     tagline = None
@@ -55,19 +71,26 @@
     if public:
         tagline = click.prompt(f"Want to give the {deployable_type} a tagline?", default="")
         author_github = click.prompt(
             "If you'd like this associated with your github account, please your github username",
             default="",
         )
 
+    tag_string = click.prompt(
+        f"Want to give the {deployable_type} some tags? (comma separated)", default="Prompt API"
+    )
+    tags = [tag.strip() for tag in tag_string.split(",")]
+
     return Manifest(
         type=deployable_type,
         handle=handle,
         version=version_handle,
+        description="",
         author=author,
         public=public,
+        plugin=plugin_detail,
         build_config={"ignore": ["tests", "examples"]},
         configTemplate={},
         steamshipRegistry=SteamshipRegistry(
-            tagline=tagline, authorGithub=author_github, authorName=author, tags=[]
+            tagline=tagline, authorGithub=author_github, authorName=author, tags=tags
         ),
     )
```

### Comparing `steamship-2.3.9/src/steamship/cli/ship_spinner.py` & `steamship-2.7.17/src/steamship/cli/ship_spinner.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/client/skill_to_provider.py` & `steamship-2.7.17/src/steamship/client/skill_to_provider.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/client/steamship.py` & `steamship-2.7.17/src/steamship/client/steamship.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 import logging
 import uuid
 from contextlib import contextmanager
 from typing import Any, Dict, Generator, List, Optional
 
 from pydantic import BaseModel
 
-from steamship import Configuration, PackageInstance, PluginInstance, SteamshipError, Workspace
 from steamship.base.client import Client
+from steamship.base.configuration import Configuration
+from steamship.base.error import SteamshipError
 from steamship.client.skill_to_provider import SKILL_TO_PROVIDER
 from steamship.client.skills import Skill
 from steamship.client.vendors import Vendor
 from steamship.data.embeddings import EmbedAndSearchRequest, QueryResults
+from steamship.data.package.package_instance import PackageInstance
 from steamship.data.plugin.index_plugin_instance import EmbeddingIndexPluginInstance
+from steamship.data.plugin.plugin_instance import PluginInstance
 from steamship.data.plugin.prompt_generation_plugin_instance import PromptGenerationPluginInstance
-
-_logger = logging.getLogger(__name__)
+from steamship.data.workspace import Workspace
+from steamship.utils.metadata import hash_dict
+from steamship.utils.utils import create_instance_handle
 
 
 class Steamship(Client):
     """Steamship Python Client."""
 
     # Some plugin instances use special subclasses which provide helper methods and/or more complex
     # behavior than typical PluginInstance subclass permits. Examples are:
@@ -28,14 +32,15 @@
     # - Embedding indices (which much coordinate both embedding taggers & vector indices)
     # - Prompt generators (which benefit from supporting, prompt-specific, methods)
     _PLUGIN_INSTANCE_SUBCLASS_OVERRIDES = {
         "prompt-generation-default": PromptGenerationPluginInstance,
         "prompt-generation-trainable-default": PromptGenerationPluginInstance,
         "gpt3": PromptGenerationPluginInstance,
         "gpt-3": PromptGenerationPluginInstance,
+        "cerebrium": PromptGenerationPluginInstance,
         "embedding-index": EmbeddingIndexPluginInstance,
     }
 
     def __init__(
         self,
         api_key: str = None,
         api_base: str = None,
@@ -121,14 +126,15 @@
     def use(
         package_handle: str,
         instance_handle: Optional[str] = None,
         config: Optional[Dict[str, Any]] = None,
         version: Optional[str] = None,
         fetch_if_exists: bool = True,
         workspace_handle: Optional[str] = None,
+        wait_for_init: bool = True,
         **kwargs,
     ) -> PackageInstance:
         """Creates/loads an instance of package `package_handle`.
 
         The instance is named `instance_handle` and located in the Workspace named `instance_handle`. If no
         `instance_handle` is provided, the default is `package_handle`.
 
@@ -154,48 +160,61 @@
         client = Steamship(**kwargs)
         return client._instance_use(
             package_handle=package_handle,
             instance_handle=instance_handle,
             config=config,
             version=version,
             fetch_if_exists=fetch_if_exists,
+            wait_for_init=wait_for_init,
         )
 
     def _instance_use(
         self,
         package_handle: str,
         instance_handle: Optional[str] = None,
         config: Optional[Dict[str, Any]] = None,
         version: Optional[str] = None,
         fetch_if_exists: bool = True,
+        wait_for_init: bool = True,
     ) -> PackageInstance:
         """Creates/loads an instance of package `package_handle`.
 
         The instance is named `instance_handle` and located in the workspace this client is anchored to.
         If no `instance_handle` is provided, the default is `package_handle`.
         """
+
         if instance_handle is None:
-            instance_handle = package_handle
-        return PackageInstance.create(
+            if config is None:
+                instance_handle = package_handle
+            else:
+                instance_handle = create_instance_handle(
+                    invocable_handle=package_handle, version_handle=version, invocable_config=config
+                )
+
+        result = PackageInstance.create(
             self,
             package_handle=package_handle,
             package_version_handle=version,
             handle=instance_handle,
             config=config,
             fetch_if_exists=fetch_if_exists,
         )
+        if wait_for_init:
+            result.wait_for_init()
+        return result
 
     @staticmethod
     def use_plugin(
         plugin_handle: str,
         instance_handle: Optional[str] = None,
         config: Optional[Dict[str, Any]] = None,
         version: Optional[str] = None,
         fetch_if_exists: bool = True,
         workspace_handle: Optional[str] = None,
+        wait_for_init: bool = True,
         **kwargs,
     ) -> PluginInstance:
         """Creates/loads an instance of plugin `plugin_handle`.
 
         The instance is named `instance_handle` and located in the Workspace named `instance_handle`.
         If no `instance_handle` is provided, the default is `plugin_handle`.
 
@@ -218,14 +237,15 @@
         client = Steamship(**kwargs)
         return client._instance_use_plugin(
             plugin_handle=plugin_handle,
             instance_handle=instance_handle,
             config=config,
             version=version,
             fetch_if_exists=fetch_if_exists,
+            wait_for_init=wait_for_init,
         )
 
     def use_skill(
         self,
         skill: Skill,
         provider: Optional[Vendor] = None,
         instance_handle: Optional[str] = None,
@@ -260,42 +280,49 @@
     def _instance_use_plugin(
         self,
         plugin_handle: str,
         instance_handle: Optional[str] = None,
         config: Optional[Dict[str, Any]] = None,
         version: Optional[str] = None,
         fetch_if_exists: Optional[bool] = True,
+        wait_for_init: bool = True,
     ) -> PluginInstance:
         """Creates/loads an instance of plugin `plugin_handle`.
 
         The instance is named `instance_handle` and located in the workspace this client is anchored to.
         If no `instance_handle` is provided, the default is `plugin_handle`.
         """
 
         if instance_handle is None:
-            instance_handle = plugin_handle
+            if config is None:
+                instance_handle = plugin_handle
+            else:
+                instance_handle = f"{plugin_handle}-{hash_dict({**config, 'version': version})}"
 
         if plugin_handle in Steamship._PLUGIN_INSTANCE_SUBCLASS_OVERRIDES:
-            return Steamship._PLUGIN_INSTANCE_SUBCLASS_OVERRIDES[plugin_handle].create(
+            result = Steamship._PLUGIN_INSTANCE_SUBCLASS_OVERRIDES[plugin_handle].create(
                 self,
                 plugin_handle=plugin_handle,
                 plugin_version_handle=version,
                 handle=instance_handle,
                 config=config,
                 fetch_if_exists=fetch_if_exists,
             )
-
-        return PluginInstance.create(
-            self,
-            plugin_handle=plugin_handle,
-            plugin_version_handle=version,
-            handle=instance_handle,
-            config=config,
-            fetch_if_exists=fetch_if_exists,
-        )
+        else:
+            result = PluginInstance.create(
+                self,
+                plugin_handle=plugin_handle,
+                plugin_version_handle=version,
+                handle=instance_handle,
+                config=config,
+                fetch_if_exists=fetch_if_exists,
+            )
+        if wait_for_init:
+            result.wait_for_init()
+        return result
 
     def get_workspace(self) -> Workspace:
         # We should probably add a hard-coded way to get this. The client in a Steamship Plugin/App comes
         # pre-configured with an API key and the Workspace in which this client should be operating.
         # This is a way to load the model object for that workspace.
         logging.info(
             f"get_workspace() called on client with config workspace {self.config.workspace_handle}/{self.config.workspace_id}"
```

### Comparing `steamship-2.3.9/src/steamship/data/__init__.py` & `steamship-2.7.17/src/steamship/data/__init__.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/data/embeddings.py` & `steamship-2.7.17/src/steamship/data/embeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import json
 from typing import Any, Dict, List, Optional, Type, Union
 
 from pydantic import BaseModel, Field
 
+from steamship import SteamshipError
 from steamship.base import Task
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
-from steamship.base.request import DeleteRequest, Request
-from steamship.base.response import Response
+from steamship.base.request import DeleteRequest, ListRequest, Request, SortOrder
+from steamship.base.response import ListResponse, Response
 from steamship.data.search import Hit
 from steamship.utils.metadata import metadata_to_str
 
+MAX_RECOMMENDED_ITEM_LENGTH = 5000
+
 
 class EmbedAndSearchRequest(Request):
     query: str
     docs: List[str]
     plugin_instance: str
     k: int = 1
 
@@ -106,51 +109,25 @@
     id: str
     query: str = None
     queries: List[str] = None
     k: int = 1
     include_metadata: bool = False
 
 
-class IndexSnapshotRequest(Request):
-    index_id: str
-    window_size: int = None  # Used for unit testing
-
-
-class IndexSnapshotResponse(Response):
-    id: Optional[str] = None
-    snapshot_id: str
-
-
-class ListSnapshotsRequest(Request):
-    id: str = None
-
-
-class ListSnapshotsResponse(Response):
-    snapshots: List[IndexSnapshotResponse]
-
-
-class ListItemsRequest(Request):
+class ListItemsRequest(ListRequest):
     id: str = None
     file_id: str = None
     block_id: str = None
     span_id: str = None
 
 
-class ListItemsResponse(Response):
+class ListItemsResponse(ListResponse):
     items: List[EmbeddedItem]
 
 
-class DeleteSnapshotsRequest(Request):
-    snapshot_id: str = None
-
-
-class DeleteSnapshotsResponse(Response):
-    snapshot_id: str = None
-
-
 class EmbeddingIndex(CamelModel):
     """A persistent, read-optimized index over embeddings."""
 
     client: Client = Field(None, exclude=True)
     id: str = None
     handle: str = None
     name: str = None
@@ -191,54 +168,80 @@
         )
         return self.client.post(
             "embedding-index/item/create",
             req,
             expect=IndexInsertResponse,
         )
 
+    def _check_input(self, request: IndexInsertRequest, allow_long_records: bool):
+        if not allow_long_records:
+            if request.value is not None and len(request.value) > MAX_RECOMMENDED_ITEM_LENGTH:
+                raise SteamshipError(
+                    f"Inserted item of length {len(request.value)} exceeded maximum recommended length of {MAX_RECOMMENDED_ITEM_LENGTH} characters. You may insert it anyway by passing allow_long_records=True."
+                )
+            if request.items is not None:
+                for i, item in enumerate(request.items):
+                    if item is not None:
+                        if isinstance(item, str) and len(item) > MAX_RECOMMENDED_ITEM_LENGTH:
+                            raise SteamshipError(
+                                f"Inserted item {i} of length {len(item)} exceeded maximum recommended length of {MAX_RECOMMENDED_ITEM_LENGTH} characters. You may insert it anyway by passing allow_long_records=True."
+                            )
+                        if (
+                            isinstance(item, EmbeddedItem)
+                            and item.value is not None
+                            and len(item.value) > MAX_RECOMMENDED_ITEM_LENGTH
+                        ):
+                            raise SteamshipError(
+                                f"Inserted item {i} of length {len(item.value)} exceeded maximum recommended length of {MAX_RECOMMENDED_ITEM_LENGTH} characters. You may insert it anyway by passing allow_long_records=True."
+                            )
+
     def insert_many(
         self,
         items: List[Union[EmbeddedItem, str]],
         reindex: bool = True,
+        allow_long_records=False,
     ) -> IndexInsertResponse:
         new_items = []
         for item in items:
             if isinstance(item, str):
                 new_items.append(EmbeddedItem(value=item))
             else:
                 new_items.append(item)
 
         req = IndexInsertRequest(
             index_id=self.id,
             items=[item.clone_for_insert() for item in new_items],
             reindex=reindex,
         )
+        self._check_input(req, allow_long_records)
         return self.client.post(
             "embedding-index/item/create",
             req,
             expect=IndexInsertResponse,
         )
 
     def insert(
         self,
         value: str,
         external_id: str = None,
         external_type: str = None,
         metadata: Union[int, float, bool, str, List, Dict] = None,
         reindex: bool = True,
+        allow_long_records=False,
     ) -> IndexInsertResponse:
 
         req = IndexInsertRequest(
             index_id=self.id,
             value=value,
             external_id=external_id,
             external_type=external_type,
             metadata=metadata_to_str(metadata),
             reindex=reindex,
         )
+        self._check_input(req, allow_long_records)
         return self.client.post(
             "embedding-index/item/create",
             req,
             expect=IndexInsertResponse,
         )
 
     def embed(
@@ -247,54 +250,38 @@
         req = IndexEmbedRequest(id=self.id)
         return self.client.post(
             "embedding-index/embed",
             req,
             expect=IndexEmbedResponse,
         )
 
-    def create_snapshot(self) -> IndexSnapshotResponse:
-        req = IndexSnapshotRequest(index_id=self.id)
-        return self.client.post(
-            "embedding-index/snapshot/create",
-            req,
-            expect=IndexSnapshotResponse,
-        )
-
-    def list_snapshots(self) -> ListSnapshotsResponse:
-        req = ListSnapshotsRequest(id=self.id)
-        return self.client.post(
-            "embedding-index/snapshot/list",
-            req,
-            expect=ListSnapshotsResponse,
-        )
-
     def list_items(
         self,
         file_id: str = None,
         block_id: str = None,
         span_id: str = None,
+        page_size: Optional[int] = None,
+        page_token: Optional[str] = None,
+        sort_order: Optional[SortOrder] = SortOrder.DESC,
     ) -> ListItemsResponse:
-        req = ListItemsRequest(id=self.id, file_id=file_id, block_id=block_id, spanId=span_id)
+        req = ListItemsRequest(
+            id=self.id,
+            file_id=file_id,
+            block_id=block_id,
+            spanId=span_id,
+            page_size=page_size,
+            page_token=page_token,
+            sort_order=sort_order,
+        )
         return self.client.post(
             "embedding-index/item/list",
             req,
             expect=ListItemsResponse,
         )
 
-    def delete_snapshot(
-        self,
-        snapshot_id: str,
-    ) -> DeleteSnapshotsResponse:
-        req = DeleteSnapshotsRequest(snapshotId=snapshot_id)
-        return self.client.post(
-            "embedding-index/snapshot/delete",
-            req,
-            expect=DeleteSnapshotsResponse,
-        )
-
     def delete(self) -> EmbeddingIndex:
         return self.client.post(
             "embedding-index/delete",
             DeleteRequest(id=self.id),
             expect=EmbeddingIndex,
         )
```

### Comparing `steamship-2.3.9/src/steamship/data/file.py` & `steamship-2.7.17/src/steamship/invocable/invocable_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,262 +1,231 @@
 from __future__ import annotations
 
 import io
-from enum import Enum
-from typing import TYPE_CHECKING, Any, List, Type, Union
+import json
+import logging
+from typing import Any, Dict, Generic, Optional, TypeVar, Union
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
+from pydantic.generics import GenericModel
 
-from steamship import MimeTypes, SteamshipError
+from steamship.base import MimeTypes, SteamshipError, Task, TaskState
 from steamship.base.client import Client
+from steamship.base.error import DEFAULT_ERROR_MESSAGE
+from steamship.base.mime_types import ContentEncodings
 from steamship.base.model import CamelModel
-from steamship.base.request import GetRequest, IdentifierRequest, Request
-from steamship.base.response import Response
-from steamship.base.tasks import Task
-from steamship.data.block import Block
-from steamship.data.embeddings import EmbeddingIndex
-from steamship.data.tags import Tag
 from steamship.utils.binary_utils import flexi_create
 
-if TYPE_CHECKING:
-    from steamship.data.operations.tagger import TagResponse
 
+class Http(CamelModel):
+    status: int = None
+    # If true, we're signaling to the Steamship Proxy that the `data` field of the SteamshipResponse object
+    # has been wrapped in base64. In this situation, we can return the bytes within directly to the Proxy
+    # caller without interpreting it.
+    base64_wrapped: bool = None
+    headers: Dict[str, str] = None
 
-class FileUploadType(str, Enum):
-    FILE = "file"  # A file uploaded as bytes or a string
-    FILE_IMPORTER = "fileImporter"  # A fileImporter will be used to create the file
-    BLOCKS = "blocks"  # Blocks are sent to create a file
 
+T = TypeVar("T")
 
-class FileClearResponse(Response):
-    id: str
 
+class InvocableResponse(GenericModel, Generic[T]):
+    """Mirrors the Response object in the Steamship server."""
 
-class ListFileRequest(Request):
-    pass
+    data: T = None  # Data for successful or synchronous requests.
+    status: Task = None  # Reporting for errors and async status
+    http: Http = None  # Additional HTTP information for Steamship Proxy (headers, etc)
 
+    def __init__(
+        self,
+        status: Task = None,
+        error: SteamshipError = None,
+        http: Http = None,
+        data: Any = None,
+        string: str = None,
+        json: Any = None,
+        _bytes: Union[bytes, io.BytesIO] = None,
+        mime_type=None,
+    ):
+        super().__init__()
+        # Note:
+        # This function has to be very defensively coded since Any errors thrown here will not be returned
+        # to the end-user via our proxy (as this is the constructor for the response itself!)
+        if http is not None:
+            self.http = http
+        else:
+            self.http = Http(status=200, headers={})
 
-class ListFileResponse(Response):
-    files: List[File]
-
-
-class FileQueryRequest(Request):
-    tag_filter_query: str
-
-
-class File(CamelModel):
-    """A file."""
-
-    client: Client = Field(None, exclude=True)
-    id: str = None
-    handle: str = None
-    mime_type: MimeTypes = None
-    workspace_id: str = None
-    blocks: List[Block] = []
-    tags: List[Tag] = []
-    filename: str = None
-
-    class CreateResponse(Response):
-        data_: Any = None
-        mime_type: str = None
+        try:
+            self.set_data(data=data, string=string, json=json, _bytes=_bytes, mime_type=mime_type)
+        except Exception as ex:
+            logging.error("Exception within Response.__init__.", exc_info=ex)
+            if error is not None:
+                if error.message:
+                    error.message = f"{error.message}. Also found error - unable to serialize data to response. {ex}"
+                else:
+                    error.message = f"Unable to serialize data to response. {ex}"
+            else:
+                error = SteamshipError(message=f"Unable to serialize data to response. {ex}")
+            logging.error(error, exc_info=error)
 
-        def __init__(
-            self,
-            data: Any = None,
-            string: str = None,
-            _bytes: Union[bytes, io.BytesIO] = None,
-            json: io.BytesIO = None,
-            mime_type: str = None,
-        ):
-            super().__init__()
-            data, mime_type, encoding = flexi_create(
-                data=data, string=string, json=json, _bytes=_bytes, mime_type=mime_type
+        # Handle the task provided
+        if status is None:
+            self.status = Task()
+        elif isinstance(status, Task):
+            self.status = status
+        else:
+            self.status = Task()
+            self.status.state = TaskState.failed
+            self.status.status_message = (
+                f"Status field of response should be of type Task. "
+                f"Instead was of type {type(status)} and had value {status}."
             )
-            self.data_ = data
-            self.mime_type = mime_type
 
-        @classmethod
-        def parse_obj(cls: Type[BaseModel], obj: Any) -> Response:
-            obj["data"] = obj.get("data") or obj.get("data_")
-            if "data_" in obj:
-                del obj["data_"]
-            return super().parse_obj(obj)
-
-    @classmethod
-    def parse_obj(cls: Type[BaseModel], obj: Any) -> BaseModel:
-        # TODO (enias): This needs to be solved at the engine side
-        obj = obj["file"] if "file" in obj else obj
-        return super().parse_obj(obj)
-
-    def delete(self) -> File:
-        return self.client.post(
-            "file/delete",
-            IdentifierRequest(id=self.id),
-            expect=File,
-        )
-
-    @staticmethod
-    def get(
-        client: Client,
-        _id: str = None,
-        handle: str = None,
-    ) -> File:
-        return client.post(
-            "file/get",
-            IdentifierRequest(id=_id, handle=handle),
-            expect=File,
-        )
-
-    @staticmethod
-    def create(
-        client: Client,
-        content: Union[str, bytes] = None,
-        mime_type: MimeTypes = None,
-        handle: str = None,
-        blocks: List[Block] = None,
-        tags: List[Tag] = None,
-    ) -> File:
-
-        if content is None and blocks is None:
-            if tags is None:
-                raise SteamshipError(message="Either filename, content, or tags must be provided.")
-            else:
-                content = ""
-        if content is not None and blocks is not None:
-            raise SteamshipError(
-                message="Please provide only `blocks` or `content` to `File.create`."
+        if error:
+            self.status.state = TaskState.failed
+            self.status.status_message = error.message
+            self.status.status_suggestion = error.suggestion
+            self.status.status_code = error.code
+            logging.error(
+                "steamship.invocable.response - Response created with error.", exc_info=error
             )
-
-        if blocks is not None:
-            upload_type = FileUploadType.BLOCKS
-        elif content is not None:
-            upload_type = FileUploadType.FILE
         else:
-            raise Exception("Unable to determine upload type.")
+            if self.status.state is None:
+                self.status.state = TaskState.succeeded
 
-        req = {
-            "handle": handle,
-            "type": upload_type,
-            "mimeType": mime_type,
-            "blocks": [
-                block.dict(by_alias=True, exclude_unset=True, exclude_none=True)
-                for block in blocks or []
-            ],
-            "tags": [
-                tag.dict(by_alias=True, exclude_unset=True, exclude_none=True) for tag in tags or []
-            ],
-        }
-
-        file_data = (
-            ("file-part", content, "multipart/form-data")
-            if upload_type != FileUploadType.BLOCKS
-            else None
-        )
-
-        # Defaulting this here, as opposed to in the Engine, because it is processed by Vapor
-        return client.post(
-            "file/create",
-            payload=req,
-            file=file_data,
-            expect=File,
-        )
-
-    @staticmethod
-    def create_with_plugin(
-        client: Client,
-        plugin_instance: str,
-        url: str = None,
-        mime_type: str = None,
-    ) -> Task[File]:
-
-        req = {
-            "type": FileUploadType.FILE_IMPORTER,
-            "url": url,
-            "mimeType": mime_type,
-            "pluginInstance": plugin_instance,
-        }
-
-        return client.post("file/create", payload=req, expect=File, as_background_task=True)
-
-    def refresh(self) -> File:
-        refreshed = File.get(self.client, self.id)
-        self.__init__(**refreshed.dict())
-        self.client = refreshed.client
-        return self
-
-    @staticmethod
-    def query(
-        client: Client,
-        tag_filter_query: str,
-    ) -> FileQueryResponse:
-
-        req = FileQueryRequest(tag_filter_query=tag_filter_query)
-        res = client.post(
-            "file/query",
-            payload=req,
-            expect=FileQueryResponse,
-        )
-        return res
-
-    def raw(self):
-        return self.client.post(
-            "file/raw",
-            payload=GetRequest(
-                id=self.id,
-            ),
-            raw_response=True,
-        )
-
-    def blockify(self, plugin_instance: str = None, wait_on_tasks: List[Task] = None) -> Task:
-        from steamship.data.operations.blockifier import BlockifyRequest
-        from steamship.plugin.outputs.block_and_tag_plugin_output import BlockAndTagPluginOutput
-
-        req = BlockifyRequest(type="file", id=self.id, plugin_instance=plugin_instance)
-
-        return self.client.post(
-            "plugin/instance/blockify",
-            payload=req,
-            expect=BlockAndTagPluginOutput,
-            wait_on_tasks=wait_on_tasks,
-        )
-
-    def tag(
+    def set_data(
         self,
-        plugin_instance: str = None,
-        wait_on_tasks: List[Task] = None,
-    ) -> Task[TagResponse]:
-        from steamship.data.operations.tagger import TagRequest, TagResponse
-        from steamship.data.plugin import PluginTargetType
-
-        req = TagRequest(type=PluginTargetType.FILE, id=self.id, plugin_instance=plugin_instance)
-        return self.client.post(
-            "plugin/instance/tag", payload=req, expect=TagResponse, wait_on_tasks=wait_on_tasks
+        data: Any = None,
+        string: str = None,
+        json: Any = None,
+        _bytes: Union[bytes, io.BytesIO] = None,
+        mime_type=None,
+    ):
+        data, mime_type, encoding = flexi_create(
+            data=data, string=string, json=json, _bytes=_bytes, mime_type=mime_type
         )
 
-    def index(self, plugin_instance: Any = None) -> EmbeddingIndex:
-        """Index every block in the file.
+        self.data = data
+
+        self.http.headers = self.http.headers or {}
+        self.http.headers["Content-Type"] = mime_type or MimeTypes.BINARY
 
-        TODO(ted): Enable indexing the results of a tag query.
-        TODO(ted): It's hard to load the EmbeddingIndexPluginInstance with just a handle because of the chain
-        of things that need to be created to it to function."""
-
-        # Preserve the prior behavior of embedding the full text of each block.
-        tags = [
-            Tag(text=block.text, file_id=self.id, block_id=block.id, kind="block")
-            for block in self.blocks or []
-        ]
-        return plugin_instance.insert(tags)
+        if encoding == ContentEncodings.BASE64:
+            self.http.base64_wrapped = True
 
     @staticmethod
-    def list(client: Client) -> ListFileResponse:
-        return client.post(
-            "file/list",
-            ListFileRequest(),
-            expect=ListFileResponse,
-        )
+    def error(
+        code: int,
+        message: Optional[str] = None,
+        error: Optional[SteamshipError] = None,
+        exception: Optional[Exception] = None,
+        prefix: Optional[str] = None,
+    ) -> InvocableResponse[T]:
+        """Merges a number of error channels into one unified Response object.
+
+        Aggregates all possible messages into a single " | "-delimeted error message.
+
+        If the final resulting error message is non-null, prefixes with the provided `prefix`
+        """
+        # Use or create the return error
+        error = error or SteamshipError()
+
+        messages = []
+        if error.message != DEFAULT_ERROR_MESSAGE:
+            messages.append(error.message)
+
+        # Set or append the additional message
+        if message is not None and message not in messages:
+            messages.append(message)
+
+        # Set or append the exception
+        if exception is not None:
+            exception_str = f"{exception}"
+            if exception_str not in messages:
+                messages.append(exception_str)
+
+        messages = [m.strip() for m in messages if m is not None and len(m.strip())]
+        if len(messages) > 0:
+            error.message = " | ".join(messages)
+
+        # Finally, add the prefix if requested.
+        if prefix and error.message:
+            error.message = f"{prefix}{error.message}"
 
+        return InvocableResponse(error=error, http=Http(status=code))
 
-class FileQueryResponse(Response):
-    files: List[File]
+    @staticmethod
+    def from_obj(obj: Any) -> InvocableResponse:  # noqa: C901
+        if obj is None:
+            return InvocableResponse.error(500, "Handler provided no response.")
+
+        if isinstance(obj, InvocableResponse):
+            return obj
+        elif isinstance(obj, SteamshipError):
+            return InvocableResponse.error(500, error=obj)
+        elif isinstance(obj, Exception):
+            return InvocableResponse.error(500, error=SteamshipError(error=obj))
+        elif isinstance(obj, io.BytesIO):
+            return InvocableResponse(_bytes=obj)
+        elif isinstance(obj, dict):
+            return InvocableResponse(json=obj)
+        elif isinstance(obj, list):
+            return InvocableResponse(json=obj)
+        elif isinstance(obj, str):
+            return InvocableResponse(string=obj)
+        elif isinstance(obj, (float, int, bool)):
+            return InvocableResponse(json=obj)
+        elif isinstance(obj, CamelModel):
+            return InvocableResponse(json=obj.dict(by_alias=True))
+        elif isinstance(obj, BaseModel):
+            return InvocableResponse(json=obj.dict())
+
+        return InvocableResponse.error(
+            500, message=f"Handler provided unknown response type: {type(obj)}"
+        )
+
+    def post_update(self, client: Client):
+        """Pushes this response object to the corresponding Task on the Steamship Engine.
+
+        Typically apps and plugins return their results to the Engine synchronously via HTTP.
+        But sometimes that's not practice -- for example:
+
+        - Microsoft's OCR endpoint returns a Job Token that can be exchanged for updates, and eventually a result.
+        - Google's AutoML can take 20-30 minutes to train.
+        - Fine-tuning BERT on ECS can take an arbitrarily long amount of time.
+
+        In these cases, it can be useful for the package/plugin to occasionally post updates to the Engine outside
+        of the Engine's initial synchronous request-response conversation.
+        """
+        if self.status is None or self.status.task_id is None:
+            raise SteamshipError(
+                message="An App/Plugin response can only be pushed to the Steamship Engine if "
+                + "it is associated with a Task. Please set the `status.task_id` field."
+            )
+        if client is None:
+            raise SteamshipError(
+                message="Unable to push Response to Steamship: Associated client is None"
+            )
 
+        # Create a task object
+        task = Task(client=client, task_id=self.status.task_id)
+        update_fields = set()
+
+        if self.status.state is not None:
+            task.state = self.status.state
+            update_fields.add("state")
+
+        if self.status.status_message is not None:
+            task.status_message = self.status.status_message
+            update_fields.add("status_message")
+
+        if self.status.status_suggestion is not None:
+            task.status_suggestion = self.status.status_suggestion
+            update_fields.add("status_suggestion")
+
+        if self.data is not None:
+            # This object itself should always be the output of the Training Task object.
+            task.output = json.dumps(self.data)
+            update_fields.add("output")
 
-ListFileResponse.update_forward_refs()
+        task.post_update(fields=update_fields)
```

### Comparing `steamship-2.3.9/src/steamship/data/package/package.py` & `steamship-2.7.17/src/steamship/data/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,24 @@
-#
-# This is the CLIENT-side abstraction for an invocable.
-#
-# If you are implementing a package, see: steamship.invocable.server.App
-#
-
 from __future__ import annotations
 
 from typing import Any, Type
 
 from pydantic import BaseModel, Field
 
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
-from steamship.base.request import CreateRequest, GetRequest
-
-
-class PackageCreateRequest(CreateRequest):
-    fetch_if_exists = False
 
 
-class Package(CamelModel):
+class User(CamelModel):
     client: Client = Field(None, exclude=True)
     id: str = None
     handle: str = None
-    user_id: str = None
 
     @classmethod
     def parse_obj(cls: Type[BaseModel], obj: Any) -> BaseModel:
         # TODO (enias): This needs to be solved at the engine side
-        obj = obj["package"] if "package" in obj else obj
+        obj = obj["user"] if "user" in obj else obj
         return super().parse_obj(obj)
 
     @staticmethod
-    def create(client: Client, handle: str = None, fetch_if_exists=False) -> Package:
-        req = PackageCreateRequest(handle=handle, fetch_if_exists=fetch_if_exists)
-        return client.post("package/create", payload=req, expect=Package)
-
-    @staticmethod
-    def get(client: Client, handle: str) -> Package:
-        return client.post("package/get", GetRequest(handle=handle), expect=Package)
+    def current(client: Client) -> User:
+        return client.get("account/current", expect=User)
```

### Comparing `steamship-2.3.9/src/steamship/data/package/package_version.py` & `steamship-2.7.17/src/steamship/data/package/package_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from typing import Any, Dict, Type
 
 from pydantic import BaseModel, Field
 
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
-from steamship.base.request import Request
+from steamship.base.request import IdentifierRequest, Request
 
 
 class CreatePackageVersionRequest(Request):
     package_id: str = None
     handle: str = None
     type: str = "file"
     hosting_handler: str = None
@@ -63,7 +63,17 @@
             "package/version/create",
             payload=req,
             file=("package.zip", filebytes, "multipart/form-data"),
             expect=PackageVersion,
         )
         task.wait()
         return task.output
+
+    def delete(self) -> PackageVersion:
+        """Delete this package version. If this package is public and another user has created an instance of this version,
+        this method will throw an error and the PackageVersion will not be deleted. Deleting the PackageVersion will delete any
+        instances of it that you have created."""
+        return self.client.post(
+            "package/version/delete",
+            IdentifierRequest(id=self.id),
+            expect=PackageVersion,
+        )
```

### Comparing `steamship-2.3.9/src/steamship/data/plugin/hosting.py` & `steamship-2.7.17/src/steamship/data/plugin/hosting.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/data/plugin/index_plugin_instance.py` & `steamship-2.7.17/src/steamship/data/plugin/index_plugin_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 from pydantic import Field
 
-from steamship import SteamshipError, Tag, Task
+from steamship import Block
 from steamship.base.client import Client
+from steamship.base.error import SteamshipError
 from steamship.base.model import CamelModel
+from steamship.base.tasks import Task
 from steamship.data.embeddings import EmbeddedItem, EmbeddingIndex, QueryResult, QueryResults
 from steamship.data.plugin.plugin_instance import PluginInstance
+from steamship.data.tags.tag import Tag
 
 
 class EmbedderInvocation(CamelModel):
     """The parameters capable of creating/fetching an Embedder (Tagger) Plugin Instance."""
 
     plugin_handle: str
     instance_handle: Optional[str] = None
@@ -24,15 +27,15 @@
 
     This class is intended to eventually replace the QueryResult object currently used with the Embedding layer."""
 
     tag: Optional[Tag] = None
     score: Optional[float] = None
 
     @staticmethod
-    def from_query_result(query_result: QueryResult) -> "SearchResult":
+    def from_query_result(query_result: QueryResult, client: Client) -> "SearchResult":
         hit = query_result.value
         value = hit.metadata or {}
 
         # To make this change Python-only, some fields are stached in `hit.metadata`.
         # This has the temporary consequence of these keys not being safe. This will be resolved when we spread
         # this refactor to the engine.
         block_id = None
@@ -47,14 +50,15 @@
 
         tag_id = None
         if "_tag_id" in value:
             tag_id = value.get("_tag_id")
         del value["_tag_id"]
 
         tag = Tag(
+            client=client,
             id=hit.id,
             kind=hit.external_type,
             name=hit.external_id,
             block_id=block_id,
             tag_id=tag_id,
             file_id=file_id,
             text=hit.value,
@@ -68,39 +72,56 @@
 
     This class is intended to eventually replace the QueryResults object currently used with the Embedding layer.
     TODO: add in paging support."""
 
     items: List[SearchResult] = None
 
     @staticmethod
-    def from_query_results(query_results: QueryResults) -> "SearchResults":
-        items = [SearchResult.from_query_result(qr) for qr in query_results.items or []]
+    def from_query_results(query_results: QueryResults, client: Client) -> "SearchResults":
+        items = [
+            SearchResult.from_query_result(qr, client=client) for qr in query_results.items or []
+        ]
         return SearchResults(items=items)
 
+    def to_ranked_blocks(self) -> List[Block]:
+        blocks = []
+        for result in self.items:
+            tag = result.tag
+            blocks.append(Block.get(tag.client, tag.block_id))
+        return blocks
+
 
 class EmbeddingIndexPluginInstance(PluginInstance):
     """A persistent, read-optimized index over embeddings.
 
     This is currently implemented as an object which behaves like a PluginInstance even though
     it isn't from an implementation perspective on the back-end.
     """
 
-    client: Client = Field(None, exclude=True)
     embedder: PluginInstance = Field(None, exclude=True)
     index: EmbeddingIndex = Field(None, exclude=True)
 
+    def reset(self):
+        self.index.delete()
+        self.index = EmbeddingIndex.create(
+            client=self.client,
+            handle=self.handle,
+            embedder_plugin_instance_handle=self.embedder.handle,
+            fetch_if_exists=False,
+        )
+
     def delete(self):
         """Delete the EmbeddingIndexPluginInstnace.
 
         For now, we will have this correspond to deleting the `index` but not the `embedder`. This is likely
         a temporary design.
         """
         return self.index.delete()
 
-    def insert(self, tags: Union[Tag, List[Tag]]):
+    def insert(self, tags: Union[Tag, List[Tag]], allow_long_records: bool = False):
         """Insert tags into the embedding index."""
 
         # Make a list if a single tag was provided
         if isinstance(tags, Tag):
             tags = [tags]
 
         for tag in tags:
@@ -113,15 +134,15 @@
             metadata = tag.value or {}
             if not isinstance(metadata, dict):
                 raise SteamshipError(
                     "Only Tags with a dict or None value can be embedded. "
                     + f"This tag had a value of type: {type(tag.value)}"
                 )
 
-            # To make this change Python-only, some fields are stached in `hit.metadata`.
+            # To make this change Python-only, some fields are stashed in `hit.metadata`.
             # This has the temporary consequence of these keys not being safe. This will be resolved when we spread
             # this refactor to the engine.
             metadata["_file_id"] = tag.file_id
             metadata["_tag_id"] = tag.id
             metadata["_block_id"] = tag.block_id
             tag.value = metadata
 
@@ -131,21 +152,17 @@
                 external_id=tag.name,
                 external_type=tag.kind,
                 metadata=tag.value,
             )
             for tag in tags
         ]
 
-        # We always reindex in this new style; to not do so is to expose details (when embedding occurrs) we'd rather
+        # We always reindex in this new style; to not do so is to expose details (when embedding occurs) we'd rather
         # not have users exercise control over.
-        self.index.insert_many(embedded_items, reindex=True)
-
-        # We always snapshot in this new style; to not do so is to expose details we'd rather not have
-        # users exercise control over.
-        self.index.create_snapshot()
+        self.index.insert_many(embedded_items, reindex=True, allow_long_records=allow_long_records)
 
     def search(self, query: str, k: Optional[int] = None) -> Task[SearchResults]:
         """Search the embedding index.
 
         This wrapper implementation simply projects the `Hit` data structure into a `Tag`
         """
         if query is None or len(query.strip()) == 0:
@@ -154,15 +171,15 @@
         # Metadata will always be included; this is the equivalent of Tag.value
         wrapped_result = self.index.search(query, k=k, include_metadata=True)
 
         # For now, we'll have to do this synchronously since we're trying to avoid changing things on the engine.
         wrapped_result.wait()
 
         # We're going to do a switcheroo on the output type of Task here.
-        search_results = SearchResults.from_query_results(wrapped_result.output)
+        search_results = SearchResults.from_query_results(wrapped_result.output, client=self.client)
         wrapped_result.output = search_results
 
         # Return the index's search result, but projected into the data structure of Tags
         return cast(Task[SearchResults], wrapped_result)
 
     @staticmethod
     def create(
@@ -185,20 +202,21 @@
             )
 
         # Just for pydantic validation.
         embedder_invocation = EmbedderInvocation.parse_obj(config["embedder"])
 
         # Create the embedder
         embedder = client.use_plugin(**embedder_invocation.dict())
+        embedder.wait_for_init()
 
         # Create the index
         index = EmbeddingIndex.create(
             client=client,
             handle=handle,
             embedder_plugin_instance_handle=embedder.handle,
             fetch_if_exists=fetch_if_exists,
         )
 
         # Now return the plugin wrapper
         return EmbeddingIndexPluginInstance(
-            id=index.id, handle=index.handle, index=index, embedder=embedder
+            client=client, id=index.id, handle=index.handle, index=index, embedder=embedder
         )
```

### Comparing `steamship-2.3.9/src/steamship/data/plugin/plugin_version.py` & `steamship-2.7.17/src/steamship/data/plugin/plugin_version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import json
 from typing import Any, Dict, List, Optional, Type
 
 from pydantic import BaseModel, Field
 
-from steamship.base import Task
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
-from steamship.base.request import Request
+from steamship.base.request import IdentifierRequest, Request
 from steamship.base.response import Response
 from steamship.data.plugin import HostingMemory, HostingTimeout
 
 
 class CreatePluginVersionRequest(Request):
     plugin_id: str = None
     handle: str = None
@@ -62,15 +61,15 @@
         filebytes: bytes = None,
         hosting_memory: Optional[HostingMemory] = None,
         hosting_timeout: Optional[HostingTimeout] = None,
         hosting_handler: str = None,
         is_public: bool = None,
         is_default: bool = None,
         config_template: Dict[str, Any] = None,
-    ) -> Task[PluginVersion]:
+    ) -> PluginVersion:
 
         if filename is None and filebytes is None:
             raise Exception("Either filename or filebytes must be provided.")
         if filename is not None and filebytes is not None:
             raise Exception("Only either filename or filebytes should be provided.")
 
         if filename is not None:
@@ -103,7 +102,17 @@
         client: Client, plugin_id: str = None, handle: str = None, public: bool = True
     ) -> ListPluginVersionsResponse:
         return client.post(
             f"plugin/version/{'public' if public else 'private'}",
             ListPluginVersionsRequest(handle=handle, plugin_id=plugin_id),
             expect=ListPluginVersionsResponse,
         )
+
+    def delete(self) -> PluginVersion:
+        """Delete this plugin version. If this plugin is public and another user has created an instance of this version,
+        this method will throw an error and the PluginVersion will not be deleted. Deleting the PluginVersion will delete any
+        instances of it that you have created."""
+        return self.client.post(
+            "plugin/version/delete",
+            IdentifierRequest(id=self.id),
+            expect=PluginVersion,
+        )
```

### Comparing `steamship-2.3.9/src/steamship/data/plugin/prompt_generation_plugin_instance.py` & `steamship-2.7.17/src/steamship/data/plugin/prompt_generation_plugin_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, Optional
 
-from steamship import PluginInstance, SteamshipError
 from steamship.base.client import Client
-from steamship.data.plugin.plugin_instance import CreatePluginInstanceRequest
+from steamship.base.error import SteamshipError
+from steamship.data.plugin.plugin_instance import CreatePluginInstanceRequest, PluginInstance
 from steamship.data.tags.tag_constants import TagKind, TagValueKey
 
 
 class PromptGenerationPluginInstance(PluginInstance):
     """An instance of a configured prompt completion service such as GPT-3.
 
     The `generate` method synchronously invokes the prompt against a set of variables that parameterize it.
```

### Comparing `steamship-2.3.9/src/steamship/data/search.py` & `steamship-2.7.17/src/steamship/data/search.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/data/tags/tag.py` & `steamship-2.7.17/src/steamship/data/tags/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Type, Union
 
 from pydantic import Field
+from pydantic.main import BaseModel
 
 from steamship import SteamshipError
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
 from steamship.base.request import Request
 from steamship.base.response import Response
 from steamship.data.tags.tag_constants import GenerationTag, TagKind, TagValueKey
@@ -63,14 +64,20 @@
     class ListRequest(Request):
         file_id: str = None
         block_id: str = None
 
     class ListResponse(Response):
         tags: List[Tag] = None
 
+    @classmethod
+    def parse_obj(cls: Type[BaseModel], obj: Any) -> BaseModel:
+        # TODO (enias): This needs to be solved at the engine side
+        obj = obj["tag"] if "tag" in obj else obj
+        return super().parse_obj(obj)
+
     @staticmethod
     def create(
         client: Client,
         file_id: str = None,
         block_id: str = None,
         kind: str = None,
         name: str = None,
```

### Comparing `steamship-2.3.9/src/steamship/data/tags/tag_constants.py` & `steamship-2.7.17/src/steamship/data/tags/tag_constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 
 class TagKind(str, Enum):
     """A set of `kind` constants for Tags.
 
     These define broad categories of tags. Suggested `name` values for each category are found in
-    separate enums. For example: kind=TagKind.DOCUMENT, name=DocumentTag.H1
+    separate enums. For example: kind=TagKind.DOCUMENT, name=DocTag.H1
     """
 
     PART_OF_SPEECH = "part-of-speech"
     DEPENDENCY = "dependency"
     SENTIMENT = "sentiment"
     EMOTION = "emotion"
     ENTITY = "entity"
@@ -21,30 +21,36 @@
     GENERATION = "generation"
     PROVENANCE = "provenance"
     TOPIC = "topic"
     TOKENIZATION = "tokenization"
     KIND = "summary"
     TIMESTAMP = "timestamp"
     SUMMARY = "summary"
+    SEARCH_RESULT = "search-result"
+    ROLE = "role"
+    CHAT = "chat"
+    CHAT_HISTORY_CONTEXT = "chat-history-context"
+    MESSAGE_ID = "message-id"
 
 
 class DocTag(str, Enum):
-    """A set of `name` constants for for Tags with a `kind` of `TagKind.doc`; appropriate for HTML and Markdown ideas."""
+    """A set of `name` constants for Tags with a `kind` of `TagKind.doc`; appropriate for HTML and Markdown ideas."""
 
     DOCUMENT = "document"
     PAGE = "page"  # E.g. in a PDF
     REGION = "region"  # E.g., abstract catchall region in a document
     HEADER = "header"
     H1 = "h1"
     H2 = "h2"
     H3 = "h3"
     H4 = "h4"
     H5 = "h5"
     LINE = "line"
     TITLE = "title"
+    SOURCE = "source"
     SUBTITLE = "subtitle"
     FOOTER = "footer"
     PARAGRAPH = "paragraph"
     ORDERED_LIST = "ordered-list"
     UNORDERED_LIST = "unordered-list"
     LIST_ITEM = "list-item"
     LINK = "link"
@@ -62,14 +68,15 @@
     EMPHASIZED = "emphasized"
     UNDERLINED = "underlined"
     TELETYPE = "teletype"
     ARTICLE = "article"
     MAIN = "main"
     CHAPTER = "chapter"
     TEXT = "text"
+    CHAT = "chat"
 
     @staticmethod
     def from_html_tag(tagname: Optional[str]) -> Optional["DocTag"]:  # noqa: C901
         if tagname is None:
             return None
 
         name = tagname.lower().strip()
@@ -162,15 +169,15 @@
     LIKE_EMAIL = "like-email"
     IS_OUT_OF_VOCABULARY = "is-out-of-vocabulary"
     IS_STOPWORD = "is-stopword"
     LANGUAGE = "language"
 
 
 class TagValueKey(str, Enum):
-    """A set of key constants for the `value` object within a tag.."""
+    """A set of key constants for the `value` object within a tag."""
 
     # Catch-all for confidence, score, ranking
     SCORE = "score"
 
     # Catch-all for values of different types such as integers, floats, booleans, and strings
     VALUE = "value"
 
@@ -194,14 +201,17 @@
 
     # End time of a region of a document, in some other medium (seconds)
     END_TIME_S = "end-time-s"
 
     # The normalized name of an entity
     ENTITY_NAME = "entity_name"
 
+    # Timestamp. Can be used to provide a time-based sort-ordering for tags.
+    TIMESTAMP_VALUE = "timestamp-value"
+
 
 class GenerationTag(str, Enum):
     """A set of `name` constants for Tags with a `kind` of `TagKind.generation`."""
 
     # A generated summary of some region of a document
     SUMMARY = "summary"
 
@@ -222,7 +232,48 @@
     SPEAKER = "speaker"
 
     # The URL from which some section of a document was sourced
     URL = "url"
 
     # The File from which some section of a document was sourced
     FILE = "file"
+
+
+class RoleTag(str, Enum):
+    """A set of `name` constants for Tags with a `kind` of `TagKind.ROLE`."""
+
+    # This block's content was created by the System; likely instructional text on how to respond
+    SYSTEM = "system"
+
+    # This block's content was created by an end user
+    USER = "user"
+
+    # This block's content was created by the generative AI assistant
+    ASSISTANT = "assistant"
+
+    # This block's content was created by a non-human agent participating in the chat
+    AGENT = "agent"
+
+    # This block was created by a Tool, as selected by an OpenAI Function call
+    FUNCTION = "function"
+
+
+class ChatTag(str, Enum):
+    """A set of `name` constants for Tags with a `kind` of `TagKind.CHAT`."""
+
+    # The chat id in which a message happened
+    CHAT_ID = "chat-id"
+
+    # The message id of a message
+    MESSAGE_ID = "message-id"
+
+    # The role of a message
+    ROLE = "role"
+
+    # The keys to look up a context
+    CONTEXT_KEYS = "context-keys"
+
+    # The handle of an embedding index
+    INDEX_HANDLE = "index-handle"
+
+    # A chunk of text for indexing
+    CHUNK = "chunk"
```

### Comparing `steamship-2.3.9/src/steamship/data/workspace.py` & `steamship-2.7.17/src/steamship/data/workspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from enum import Enum
 from typing import Any, List, Optional, Type
 
 from pydantic import BaseModel, Field
 
 from steamship.base.client import Client
 from steamship.base.model import CamelModel
-from steamship.base.request import GetRequest, IdentifierRequest
-from steamship.base.request import Request
+from steamship.base.request import GetRequest, IdentifierRequest, ListRequest
 from steamship.base.request import Request as SteamshipRequest
-from steamship.base.response import Response
+from steamship.base.request import SortOrder
+from steamship.base.response import ListResponse
 from steamship.base.response import Response as SteamshipResponse
 
 
-class ListWorkspacesRequest(Request):
+class ListWorkspacesRequest(ListRequest):
     pass
 
 
-class ListWorkspacesResponse(Response):
+class ListWorkspacesResponse(ListResponse):
     workspaces: List[Workspace]
 
 
 class Workspace(CamelModel):
     client: Client = Field(None, exclude=True)
     id: str = None
     handle: str = None
@@ -75,18 +75,26 @@
         ret = self.client.post(
             "workspace/createSignedUrl", payload=request, expect=SignedUrl.Response
         )
         logging.debug(f"Got signed URL: {ret}")
         return ret
 
     @staticmethod
-    def list(client: Client, t: str = None) -> ListWorkspacesResponse:
+    def list(
+        client: Client,
+        t: str = None,
+        page_size: Optional[int] = None,
+        page_token: Optional[str] = None,
+        sort_order: Optional[SortOrder] = SortOrder.DESC,
+    ) -> ListWorkspacesResponse:
         return client.post(
             "workspace/list",
-            ListWorkspacesRequest(type=t),
+            ListWorkspacesRequest(
+                type=t, page_size=page_size, page_token=page_token, sort_order=sort_order
+            ),
             expect=ListWorkspacesResponse,
         )
 
 
 class SignedUrl:
     class Bucket(str, Enum):
         EXPORTS = "exports"
```

### Comparing `steamship-2.3.9/src/steamship/invocable/__init__.py` & `steamship-2.7.17/src/steamship/invocable/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .config import Config
 from .invocable import Invocable, get, post
 from .invocable_request import InvocableRequest, Invocation, InvocationContext, LoggingConfig
 from .invocable_response import InvocableResponse
 from .lambda_handler import create_handler, safe_handler
 from .package_service import PackageService
-from .paramater_types import longstr
+from .paramater_types import fileurl, longstr
 
 __all__ = [
     "Invocable",
     "create_handler",
     "Config",
     "Invocation",
     "InvocableRequest",
@@ -16,8 +16,9 @@
     "get",
     "post",
     "InvocationContext",
     "LoggingConfig",
     "PackageService",
     "safe_handler",
     "longstr",
+    "fileurl",
 ]
```

### Comparing `steamship-2.3.9/src/steamship/invocable/config.py` & `steamship-2.7.17/src/steamship/invocable/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,15 @@
 import json
 from enum import Enum
 from pathlib import Path
-from typing import Dict, Optional, Type, Union
+from typing import Dict
 
-from pydantic import BaseModel
-
-from steamship import SteamshipError
+from steamship.base.error import SteamshipError
 from steamship.base.model import CamelModel
-
-
-class ConfigParameterType(str, Enum):
-    NUMBER = "number"
-    STRING = "string"
-    BOOLEAN = "boolean"
-
-    @staticmethod
-    def from_python_type(t: Type):
-        if issubclass(t, str):
-            return ConfigParameterType.STRING
-        elif issubclass(t, bool):  # bool is a subclass of int, so must do this first!
-            return ConfigParameterType.BOOLEAN
-        elif issubclass(t, float) or issubclass(t, int):
-            return ConfigParameterType.NUMBER
-        else:
-            raise SteamshipError(f"Unknown value type in Config: {t}")
-
-    @staticmethod
-    def parse_default_value(default_value: str, t: Type):
-        if default_value is None:
-            return None
-        elif issubclass(t, str):
-            return default_value
-        elif issubclass(t, bool):  # bool is a subclass of int, so must do this first!
-            return default_value == "True"
-        elif issubclass(t, int):
-            return int(default_value)
-        elif issubclass(t, float):
-            return float(default_value)
-        else:
-            raise SteamshipError(f"Unknown value type in Config: {t}")
-
-
-class ConfigParameter(BaseModel):
-    type: ConfigParameterType
-    description: Optional[str] = None
-
-    # Note order is important here in the union; Pydantic will coerce values into the first union type that fits!
-    default: Optional[Union[bool, float, str]] = None
+from steamship.data.manifest import ConfigParameter, ConfigParameterType
 
 
 class Config(CamelModel):
     """Base class Steamship Package and Plugin configuration objects."""
 
     def __init__(self, **kwargs):
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
@@ -79,20 +38,27 @@
             data = json.load(f)
             if not isinstance(data, dict):
                 raise SteamshipError(
                     message=f"Attempted to extend Config object with {path}, but the file did not contain a JSON `dict` object."
                 )
             self.extend_with_dict(data, overwrite)
 
+    @staticmethod
+    def strip_enum(default_value):
+        if issubclass(type(default_value), Enum):
+            return default_value.value
+        else:
+            return default_value
+
     @classmethod
     def get_config_parameters(cls) -> Dict[str, ConfigParameter]:
         result = {}
         for field_name, field in cls.__fields__.items():
             description = field.field_info.description
             type_ = ConfigParameterType.from_python_type(field.type_)
             result[field_name] = ConfigParameter(
                 type=type_,
-                default=field.default,
+                default=cls.strip_enum(field.default),
                 description=description,
             )
 
         return result
```

### Comparing `steamship-2.3.9/src/steamship/invocable/entrypoint.py` & `steamship-2.7.17/src/steamship/invocable/entrypoint.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/invocable/invocable.py` & `steamship-2.7.17/src/steamship/invocable/invocable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Please see https://docs.steamship.com/ for information about building a Steamship Package"""
 import inspect
 import logging
 import pathlib
 import time
 from abc import ABC
-from collections import defaultdict
 from functools import wraps
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union
 
 import toml
+from pydantic import BaseModel
 
+from steamship import SteamshipError
 from steamship.base.package_spec import MethodSpec, PackageSpec
-from steamship.client import Steamship
+from steamship.client.steamship import Steamship
 from steamship.invocable import Config
 from steamship.invocable.config import ConfigParameter
 from steamship.invocable.invocable_request import InvocableRequest, InvocationContext
 from steamship.invocable.invocable_response import InvocableResponse
 from steamship.utils.url import Verb
 
 
@@ -81,46 +82,97 @@
     return endpoint(verb=Verb.GET, path=path, **kwargs)
 
 
 def post(path: str, **kwargs):
     return endpoint(verb=Verb.POST, path=path, **kwargs)
 
 
+class RouteMethod(BaseModel):
+    attribute: Any
+    verb: Optional[Verb]
+    path: str
+    config: Dict[str, Any]
+
+
+def find_route_methods(on_class: Type) -> List[RouteMethod]:
+    base_route_methods = [
+        route_method
+        for base_cls in on_class.__bases__
+        for route_method in find_route_methods(base_cls)
+    ]
+
+    this_class_route_methods: List[RouteMethod] = []
+    for attribute in list(on_class.__dict__.values()):
+        decorator = getattr(attribute, "decorator", None)
+        if decorator:
+            if getattr(decorator, "__is_endpoint__", False):
+                path = getattr(attribute, "__path__", None)
+                verb = getattr(attribute, "__verb__", None)
+                config = getattr(attribute, "__endpoint_config__", {})
+                this_class_route_methods.append(
+                    RouteMethod(attribute=attribute, verb=verb, path=path, config=config)
+                )
+
+    return merge_routes_respecting_override(base_route_methods, this_class_route_methods)
+
+
+def merge_routes_respecting_override(
+    base_routes: List[RouteMethod], this_class_routes: List[RouteMethod]
+) -> List[RouteMethod]:
+    """Merge routes from base classes into the routes from this class. If this class already has verb/path combo,
+    ignore the one from the superclass, since it has now been overridden."""
+    for route_method in base_routes:
+        if not route_list_contains(route_method, this_class_routes):
+            this_class_routes.append(route_method)
+    return this_class_routes
+
+
+def route_list_contains(route_method: RouteMethod, routes: List[RouteMethod]):
+    for other in routes:
+        if other.path == route_method.path and other.verb == route_method.verb:
+            return True
+    return False
+
+
 class Invocable(ABC):
     """A Steamship microservice.
 
     This model.py class:
 
       1. Provide a pre-authenticated instance of the Steamship client
       2. Provides a Lambda handler that routes to registered functions
       3. Provides useful methods connecting functions to the router.
     """
 
-    _method_mappings = defaultdict(dict)
     _package_spec: PackageSpec
     config: Config
     context: InvocationContext
 
     def __init__(
         self,
         client: Steamship = None,
         config: Dict[str, Any] = None,
         context: InvocationContext = None,
     ):
+        # Create an instance-level clone of the PackageSpec so that any route registrations to not impact other
+        # instance that may exist.
+        if self.__class__._package_spec:
+            self._package_spec = self.__class__._package_spec.clone()
+
         self.context = context
 
         try:
             secret_kwargs = toml.load(".steamship/secrets.toml")
-        except FileNotFoundError:  # Support local secret loading
+        except OSError:  # Support local secret loading
             try:
                 local_secrets_file = (
                     pathlib.Path(inspect.getfile(type(self))).parent / ".steamship" / "secrets.toml"
                 )
                 secret_kwargs = toml.load(str(local_secrets_file))
-            except (TypeError, FileNotFoundError):
+            except (TypeError, OSError):  # Support collab usage
                 secret_kwargs = {}
 
         # The configuration for the Invocable is the union of:
         #
         # 1) The `secret_kwargs` dict, read in from .steamship/secrets.toml, if it exists, and
         # 2) The `config` dict, provided upon instantiation.
         #
@@ -139,44 +191,63 @@
 
         self.client = client
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         start_time = time.time()
-        cls._package_spec = PackageSpec(name=cls.__name__, doc=cls.__doc__, methods=[])
-        cls._method_mappings = defaultdict(dict)
-        base_fn_list = [
-            may_be_decorated
-            for base_cls in cls.__bases__
-            for may_be_decorated in base_cls.__dict__.values()
-        ]
-        for attribute in base_fn_list + list(cls.__dict__.values()):
-            decorator = getattr(attribute, "decorator", None)
-            if decorator:
-                if getattr(decorator, "__is_endpoint__", False):
-                    path = getattr(attribute, "__path__", None)
-                    verb = getattr(attribute, "__verb__", None)
-                    config = getattr(attribute, "__endpoint_config__", {})
-                    method_spec = cls._register_mapping(
-                        name=attribute.__name__, verb=verb, path=path, config=config
-                    )
-                    cls._package_spec.methods.append(method_spec)
+
+        # The subclass takes care to extend what the superclass may have set here by copying it.
+        _package_spec = PackageSpec(name=cls.__name__, doc=cls.__doc__, methods=[])
+        if hasattr(cls, "_package_spec"):
+            _package_spec.import_parent_methods(cls._package_spec)
+            _package_spec.used_mixins = cls._package_spec.used_mixins or []
+
+        # The subclass always overrides whatever the superclass set here, having cloned its data.
+        cls._package_spec = _package_spec
+
+        for route_method in find_route_methods(cls):
+            cls._register_mapping(
+                name=route_method.attribute.__name__,
+                verb=route_method.verb,
+                path=route_method.path,
+                config=route_method.config,
+            )
 
         # Add the HTTP GET /__dir__ method which returns a serialization of the PackageSpec.
-        # Wired up to both GET and POST for convenience (since POST is the default from the Python client, but
-        # GET is the default if using from a browser).
+        # Wired up to both GET and POST for convenience (POST is Steamship default; GET is browser friendly)
         cls._register_mapping(name="__steamship_dir__", verb=Verb.GET, path="/__dir__")
         cls._register_mapping(name="__steamship_dir__", verb=Verb.POST, path="/__dir__")
+        cls._register_mapping(
+            name="invocable_instance_init", verb=Verb.POST, path="/__instance_init__", config={}
+        )
         end_time = time.time()
         logging.info(f"Registered package functions in {end_time - start_time} seconds.")
 
     def __steamship_dir__(self) -> dict:
         """Return this Invocable's PackageSpec for remote inspection -- e.g. documentation or OpenAPI generation."""
-        return self._package_spec.dict()
+        return self._package_spec.dict(by_alias=True)
+
+    def invocable_instance_init(self) -> InvocableResponse:
+        self.instance_init()
+        return InvocableResponse(data=True)
+
+    def add_api_route(self, method_spec: MethodSpec, permit_overwrite_of_existing: bool = False):
+        """Add an API route to this Invocable instance."""
+        if self._package_spec is None:
+            raise SteamshipError(
+                message=f"Unable to add API route {method_spec}. Reason: _package_spec on Invocable was None."
+            )
+        self._package_spec.add_method(
+            method_spec, permit_overwrite_of_existing=permit_overwrite_of_existing
+        )
+
+    def instance_init(self):
+        """The instance init method will be called ONCE by the engine when a new instance of a package or plugin has been created. By default, this does nothing."""
+        pass
 
     @classmethod
     def config_cls(cls) -> Type[Config]:
         """Returns the configuration object for the Invocable.
 
         By default, Steamship packages and plugins will not take any configuration. Steamship packages and plugins may
         declare a configuration object which extends from Config, if needed, as follows:
@@ -195,70 +266,53 @@
     def _register_mapping(
         cls,
         name: str,
         verb: Optional[Verb] = None,
         path: str = "",
         config: Dict[str, Union[int, float, bool, str]] = None,
     ) -> MethodSpec:
-        """Registering a mapping permits the method to be invoked via HTTP."""
-        method_spec = MethodSpec(cls, name, path=path, verb=verb, config=config)
-        # It's important to use method_spec.path below since that's the CLEANED path.
-        cls._method_mappings[verb][method_spec.path] = name
-        logging.info(f"[{cls.__name__}] {verb} {path} => {name}")
+        """Register a mapping that permits a method to be invoked via HTTP."""
+        method_spec = MethodSpec.from_class(
+            cls, name, path=path, verb=verb, config=config, func_binding=name
+        )
+        cls._package_spec.add_method(method_spec, permit_overwrite_of_existing=True)
         return method_spec
 
     def __call__(self, request: InvocableRequest, context: Any = None) -> InvocableResponse:
         """Invokes a method call if it is registered."""
-        if not hasattr(self.__class__, "_method_mappings"):
-            logging.error("__call__: No mappings available on invocable.")
-            return InvocableResponse.error(
-                code=HTTPStatus.NOT_FOUND, message="No mappings available for invocable."
-            )
-
         if request.invocation is None:
             logging.error("__call__: No invocation on request.")
             return InvocableResponse.error(
                 code=HTTPStatus.NOT_FOUND, message="No invocation was found."
             )
 
-        verb = Verb(request.invocation.http_verb.strip().upper())
+        verb = request.invocation.http_verb
         path = request.invocation.invocation_path
+        logging.info(f"REQUEST [{verb}] {path}")
 
-        path = MethodSpec.clean_path(path)
-
-        logging.info(f"[{verb}] {path}")
-
-        method_mappings = self.__class__._method_mappings
-
-        if verb not in method_mappings:
-            logging.error(f"__call__: Verb '{verb}' not found in method_mappings.")
-            return InvocableResponse.error(
-                code=HTTPStatus.NOT_FOUND,
-                message=f"No methods for verb {verb} available.",
-            )
-
-        if path not in method_mappings[verb]:
-            logging.error(f"__call__: Path '{path}' not found in method_mappings[{verb}].")
+        method_spec = self._package_spec.get_method(verb, path)
+        if method_spec is None:
             return InvocableResponse.error(
                 code=HTTPStatus.NOT_FOUND,
                 message=f"No handler for {verb} {path} available.",
             )
 
-        method = method_mappings[verb][path]
-        if not (hasattr(self, method) and callable(getattr(self, method))):
+        bound_function = method_spec.get_bound_function(self)
+
+        if not bound_function:
             logging.error(
                 f"__call__: Method not found or not callable for '{path}' in method_mappings[{verb}]."
             )
             return InvocableResponse.error(
                 code=HTTPStatus.INTERNAL_SERVER_ERROR,
                 message=f"Handler for {verb} {path} not callable.",
             )
 
         arguments = request.invocation.arguments
         if arguments is None:
-            return getattr(self, method)()
+            return bound_function()
         else:
-            return getattr(self, method)(**arguments)
+            return bound_function(**arguments)
 
     @classmethod
     def get_config_parameters(cls) -> Dict[str, ConfigParameter]:
         return cls.config_cls().get_config_parameters()
```

### Comparing `steamship-2.3.9/src/steamship/invocable/invocable_request.py` & `steamship-2.7.17/src/steamship/invocable/invocable_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from steamship.base import Configuration
 from steamship.base.model import CamelModel
 
 
 class Invocation(CamelModel):
     http_verb: str = None
@@ -23,14 +23,17 @@
     user_id: str = None
     workspace_id: str = None
     invocable_handle: str = None
     invocable_version_handle: str = None
     invocable_instance_handle: str = None
     invocable_type: str = None
     invocable_owner_id: str = None
+    invocable_url: str = None
+    invocable_owner_handle: Optional[str] = None
+    workspace_handle: Optional[str] = None
 
 
 class InvocableRequest(CamelModel):
     """A request as the Steamship Hosting Framework receives it from the Engine.
 
     This class is different from the other `Request` class:
      * `steamship.base.request` represents a request from the Steamship Client
```

### Comparing `steamship-2.3.9/src/steamship/invocable/invocable_response.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_trainable_tagger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,231 +1,208 @@
-from __future__ import annotations
-
-import io
 import json
 import logging
-from typing import Any, Dict, Generic, Optional, TypeVar, Union
+from pathlib import Path
+from typing import List, Optional, Type
 
-from pydantic import BaseModel
-from pydantic.generics import GenericModel
+from steamship import File, SteamshipError, Tag
+from steamship.base import Task, TaskState
+from steamship.invocable import Config, InvocableResponse, create_handler
+from steamship.plugin.inputs.block_and_tag_plugin_input import BlockAndTagPluginInput
+from steamship.plugin.inputs.train_plugin_input import TrainPluginInput
+from steamship.plugin.inputs.training_parameter_plugin_input import TrainingParameterPluginInput
+from steamship.plugin.outputs.block_and_tag_plugin_output import BlockAndTagPluginOutput
+from steamship.plugin.outputs.train_plugin_output import TrainPluginOutput
+from steamship.plugin.outputs.training_parameter_plugin_output import TrainingParameterPluginOutput
+from steamship.plugin.request import PluginRequest
+from steamship.plugin.tagger import TrainableTagger
+from steamship.plugin.trainable_model import TrainableModel
 
-from steamship.base import MimeTypes, SteamshipError, Task, TaskState
-from steamship.base.client import Client
-from steamship.base.error import DEFAULT_ERROR_MESSAGE
-from steamship.base.mime_types import ContentEncodings
-from steamship.base.model import CamelModel
-from steamship.utils.binary_utils import flexi_create
+TRAINING_PARAMETERS = TrainingParameterPluginOutput(
+    training_epochs=3,
+    testing_holdout_percent=0.3,
+    training_params={"keywords": ["chocolate", "roses", "champagne"]},
+)
 
 
-class Http(CamelModel):
-    status: int = None
-    # If true, we're signaling to the Steamship Proxy that the `data` field of the SteamshipResponse object
-    # has been wrapped in base64. In this situation, we can return the bytes within directly to the Proxy
-    # caller without interpreting it.
-    base64_wrapped: bool = None
-    headers: Dict[str, str] = None
+def make_train_response():
+    return InvocableResponse(data=TrainPluginOutput())
 
 
-T = TypeVar("T")
+class EmptyConfig(Config):
+    pass
 
 
-class InvocableResponse(GenericModel, Generic[T]):
-    """Mirrors the Response object in the Steamship server."""
+class TestTrainableTaggerModel(TrainableModel[EmptyConfig]):
+    """Example of a trainable model.
 
-    data: T = None  # Data for successful or synchronous requests.
-    status: Task = None  # Reporting for errors and async status
-    http: Http = None  # Additional HTTP information for Steamship Proxy (headers, etc)
+    At some point, may want to evolve this into an abstract base class, but for the time being, here is the
+    design of what a "Model" ought to look like:
 
-    def __init__(
-        self,
-        status: Task = None,
-        error: SteamshipError = None,
-        http: Http = None,
-        data: Any = None,
-        string: str = None,
-        json: Any = None,
-        _bytes: Union[bytes, io.BytesIO] = None,
-        mime_type=None,
-    ):
-        super().__init__()
-        # Note:
-        # This function has to be very defensively coded since Any errors thrown here will not be returned
-        # to the end-user via our proxy (as this is the constructor for the response itself!)
-        if http is not None:
-            self.http = http
-        else:
-            self.http = Http(status=200, headers={})
-
-        try:
-            self.set_data(data=data, string=string, json=json, _bytes=_bytes, mime_type=mime_type)
-        except Exception as ex:
-            logging.error("Exception within Response.__init__.", exc_info=ex)
-            if error is not None:
-                if error.message:
-                    error.message = f"{error.message}. Also found error - unable to serialize data to response. {ex}"
-                else:
-                    error.message = f"Unable to serialize data to response. {ex}"
-            else:
-                error = SteamshipError(message=f"Unable to serialize data to response. {ex}")
-            logging.error(error, exc_info=error)
-
-        # Handle the task provided
-        if status is None:
-            self.status = Task()
-        elif isinstance(status, Task):
-            self.status = status
-        else:
-            self.status = Task()
-            self.status.state = TaskState.failed
-            self.status.status_message = (
-                f"Status field of response should be of type Task. "
-                f"Instead was of type {type(status)} and had value {status}."
-            )
+    TRAINING:
 
-        if error:
-            self.status.state = TaskState.failed
-            self.status.status_message = error.message
-            self.status.status_suggestion = error.suggestion
-            self.status.status_code = error.code
-            logging.error(
-                "steamship.invocable.response - Response created with error.", exc_info=error
-            )
-        else:
-            if self.status.state is None:
-                self.status.state = TaskState.succeeded
+        - Save all results to the folder provided during initialization. The zipfile of this folder
+            is the ModelCheckpoint that gets saved to steamship.
+        - Note that we'll likely want to iterate on this, e.g. Does the model create the checkpoint or simply receive a
+            folder into which to save data, etc etc.
 
-    def set_data(
-        self,
-        data: Any = None,
-        string: str = None,
-        json: Any = None,
-        _bytes: Union[bytes, io.BytesIO] = None,
-        mime_type=None,
-    ):
-        data, mime_type, encoding = flexi_create(
-            data=data, string=string, json=json, _bytes=_bytes, mime_type=mime_type
-        )
-
-        self.data = data
-
-        self.http.headers = self.http.headers or {}
-        self.http.headers["Content-Type"] = mime_type or MimeTypes.BINARY
-
-        if encoding == ContentEncodings.BASE64:
-            self.http.base64_wrapped = True
-
-    @staticmethod
-    def error(
-        code: int,
-        message: Optional[str] = None,
-        error: Optional[SteamshipError] = None,
-        exception: Optional[Exception] = None,
-        prefix: Optional[str] = None,
-    ) -> InvocableResponse[T]:
-        """Merges a number of error channels into one unified Response object.
 
-        Aggregates all possible messages into a single " | "-delimeted error message.
+    LOADING:
+    - Offer a constructor that loads the model with a provided path. This path is assumed to contain the unzipped
+    ModelCheckpoint that was requested.
 
-        If the final resulting error message is non-null, prefixes with the provided `prefix`
-        """
-        # Use or create the return error
-        error = error or SteamshipError()
+      In this example model, the `from_disk(path: Path)` method provides this functionality.
+    """
+
+    KEYWORD_LIST_FILE = (
+        "keyword_list.json"  # File, relative to the checkpoint, to save/load features from.
+    )
+    keyword_list: List[str] = None  # Contents of the KEYWORD_LIST_FILE file
+    path: Optional[Path] = None  # Save the effective path for testing
+
+    def __init__(self):
+        self.path = None
+        self.keyword_list = []
+
+    def load_from_folder(self, checkpoint_path: Path):
+        """[Required by TrainableModel] Load state from the provided path."""
+        logging.info(f"Model:save_to_folder {checkpoint_path}")
+        self.path = checkpoint_path
+        with open(self.path / TestTrainableTaggerModel.KEYWORD_LIST_FILE, "r") as f:
+            self.keyword_list = json.loads(f.read())
 
-        messages = []
-        if error.message != DEFAULT_ERROR_MESSAGE:
-            messages.append(error.message)
-
-        # Set or append the additional message
-        if message is not None and message not in messages:
-            messages.append(message)
-
-        # Set or append the exception
-        if exception is not None:
-            exception_str = f"{exception}"
-            if exception_str not in messages:
-                messages.append(exception_str)
-
-        messages = [m.strip() for m in messages if m is not None and len(m.strip())]
-        if len(messages) > 0:
-            error.message = " | ".join(messages)
-
-        # Finally, add the prefix if requested.
-        if prefix and error.message:
-            error.message = f"{prefix}{error.message}"
-
-        return InvocableResponse(error=error, http=Http(status=code))
-
-    @staticmethod
-    def from_obj(obj: Any) -> InvocableResponse:  # noqa: C901
-        if obj is None:
-            return InvocableResponse.error(500, "Handler provided no response.")
-
-        if isinstance(obj, InvocableResponse):
-            return obj
-        elif isinstance(obj, SteamshipError):
-            return InvocableResponse.error(500, error=obj)
-        elif isinstance(obj, Exception):
-            return InvocableResponse.error(500, error=SteamshipError(error=obj))
-        elif isinstance(obj, io.BytesIO):
-            return InvocableResponse(_bytes=obj)
-        elif isinstance(obj, dict):
-            return InvocableResponse(json=obj)
-        elif isinstance(obj, list):
-            return InvocableResponse(json=obj)
-        elif isinstance(obj, str):
-            return InvocableResponse(string=obj)
-        elif isinstance(obj, (float, int, bool)):
-            return InvocableResponse(json=obj)
-        elif isinstance(obj, CamelModel):
-            return InvocableResponse(json=obj.dict(by_alias=True))
-        elif isinstance(obj, BaseModel):
-            return InvocableResponse(json=obj.dict())
-
-        return InvocableResponse.error(
-            500, message=f"Handler provided unknown response type: {type(obj)}"
-        )
-
-    def post_update(self, client: Client):
-        """Pushes this response object to the corresponding Task on the Steamship Engine.
-
-        Typically apps and plugins return their results to the Engine synchronously via HTTP.
-        But sometimes that's not practice -- for example:
-
-        - Microsoft's OCR endpoint returns a Job Token that can be exchanged for updates, and eventually a result.
-        - Google's AutoML can take 20-30 minutes to train.
-        - Fine-tuning BERT on ECS can take an arbitrarily long amount of time.
+    def save_to_folder(self, checkpoint_path: Path):
+        """[Required by TrainableModel] Save state to the provided path."""
+        logging.info(f"Model:save_to_folder {checkpoint_path}")
+        self.path = checkpoint_path
+        with open(checkpoint_path / TestTrainableTaggerModel.KEYWORD_LIST_FILE, "w") as f:
+            f.write(json.dumps(self.keyword_list))
 
-        In these cases, it can be useful for the package/plugin to occasionally post updates to the Engine outside
-        of the Engine's initial synchronous request-response conversation.
+    def train(self, input: PluginRequest[TrainPluginInput]) -> InvocableResponse[TrainPluginOutput]:
+        """Training for this model is to set the parameters to those provided in the input object.
+
+        This allows us to test that we're properly passing through the training parameters to the train process.
+
+        This training happens synchronously -- the train_status call should never happen!
         """
-        if self.status is None or self.status.task_id is None:
-            raise SteamshipError(
-                message="An App/Plugin response can only be pushed to the Steamship Engine if "
-                + "it is associated with a Task. Please set the `status.task_id` field."
-            )
-        if client is None:
-            raise SteamshipError(
-                message="Unable to push Response to Steamship: Associated client is None"
+        logging.info("TestTrainableTaggerModel:train()")
+        self.keyword_list = input.data.training_params.get("keyword_list", [])
+        return make_train_response()
+
+    def train_status(
+        self, input: PluginRequest[TrainPluginInput]
+    ) -> InvocableResponse[TrainPluginOutput]:
+        """Training for this model is to set the parameters to those provided in the input object.
+
+        This allows us to test that we're properly passing through the training parameters to the train process.
+        """
+        raise SteamshipError(
+            message="The train_status method should never be called on this tagger!"
+        )
+
+    def run(
+        self, request: PluginRequest[BlockAndTagPluginInput]
+    ) -> InvocableResponse[BlockAndTagPluginOutput]:
+        """Tags the incoming data for any instance of the keywords in the parameter file."""
+        logging.info(f"TestTrainableTaggerModel:run() - My keyword list is {self.keyword_list}")
+        response = InvocableResponse(
+            data=BlockAndTagPluginOutput(
+                file=File(tags=[Tag(kind=word) for word in self.keyword_list])
             )
+        )
+        logging.info(f"TestTrainableTaggerModel:run() returning {response}")
+        return response
+
+
+class TestTrainableTaggerPlugin(TrainableTagger):
+    """Tests the Trainable Tagger lifecycle.
+
+    - This tagger produces a FIXED set of trainable parameters.
+    - These parameters (and not the trainable data!) fully parameterize the trained model.
+    - The trained model (and not the trainable parameters!) fully parameterize the running model.
+    - The model simply tags keywords that it finds in the text.
+
+    Taken together, this plugin can be seen as a reference implementation of the data/process lifecycle of a trainable
+    model, regardless of where the actual work occurs:
+
+    - It could occur here, running in Lambda.
+    - It could occur here, running in ECS.
+    - It could be orchestrated from here, but runs in HuggingFace / SageMaker / or elsewhere
+
+    """
+
+    @classmethod
+    def config_cls(cls) -> Type[Config]:
+        return EmptyConfig
+
+    def model_cls(self) -> Type[TestTrainableTaggerModel]:
+        return TestTrainableTaggerModel
+
+    def run_with_model(
+        self,
+        request: PluginRequest[BlockAndTagPluginInput],
+        model: TestTrainableTaggerModel,
+    ) -> InvocableResponse[BlockAndTagPluginOutput]:
+        """Downloads the model file from the provided workspace"""
+        logging.debug(f"run_with_model {request} {model}")
+        logging.info(
+            f"TestTrainableTaggerPlugin:run_with_model() got request {request} and model {model}"
+        )
+        return model.run(request)
+
+    def get_training_parameters(
+        self, request: PluginRequest[TrainingParameterPluginInput]
+    ) -> InvocableResponse[TrainingParameterPluginOutput]:
+        ret = InvocableResponse[TrainingParameterPluginOutput](data=TRAINING_PARAMETERS)
+        return ret
+
+    def train(
+        self, request: PluginRequest[TrainPluginInput], model: TestTrainableTaggerModel
+    ) -> InvocableResponse[TrainPluginOutput]:
+        """Since trainable can't be assumed to be asynchronous, the trainer is responsible for uploading its own model file."""
+        logging.info(f"TestTrainableTaggerPlugin:train() {request}")
+
+        # Create a Response object at the top with a Task attached. This will let us stream back updates
+        # TODO: This is very non-intuitive. We should improve this.
+        response = InvocableResponse(status=Task(state=TaskState.running))
+
+        # Example of recording training progress
+        # response.status.status_message = "About to train!"
+        # response.post_update(client=self.client)
+
+        # Train the model
+        train_plugin_output = model.train(request)
+
+        # Save the model with the `default` handle.
+        archive_path_in_steamship = model.save_remote(
+            client=self.client, plugin_instance_id=request.context.plugin_instance_id
+        )
+
+        # Set the model location on the plugin output.
+        logging.info(
+            f"TestTrainableTaggerPlugin:train() setting model archive path to {archive_path_in_steamship}"
+        )
+        train_plugin_output.data.archive_path = archive_path_in_steamship
+
+        # Set the response on the `data` field of the object
+        response.set_data(json=train_plugin_output.data)
+        response.status.state = TaskState.succeeded
+        response.status.status_message = "Done!"
+
+        # If we want we can post this to the Engine
+        # response.status.status_message = "Done!"
+        # response.status.state = TaskState.succeeded
+        # response.post_update(client=self.client)
+
+        # Or, if this training really did happen synchronously, we return it.
+        logging.info(
+            f"TestTrainableTaggerPlugin:train() returning ###{json.dumps(response.dict(by_alias=True))}###--"
+        )
+        return response
+
+    def train_status(
+        self, request: PluginRequest[TrainPluginInput], model: TrainableModel
+    ) -> InvocableResponse[TrainPluginOutput]:
+        # This plugin never keeps a training task going beyond one function call.  This method should not be called.
+        raise SteamshipError(message="The train_status call should not happen on this model.")
 
-        # Create a task object
-        task = Task(client=client, task_id=self.status.task_id)
-        update_fields = set()
-
-        if self.status.state is not None:
-            task.state = self.status.state
-            update_fields.add("state")
-
-        if self.status.status_message is not None:
-            task.status_message = self.status.status_message
-            update_fields.add("status_message")
-
-        if self.status.status_suggestion is not None:
-            task.status_suggestion = self.status.status_suggestion
-            update_fields.add("status_suggestion")
-
-        if self.data is not None:
-            # This object itself should always be the output of the Training Task object.
-            task.output = json.dumps(self.data)
-            update_fields.add("output")
 
-        task.post_update(fields=update_fields)
+handler = create_handler(TestTrainableTaggerPlugin)
```

### Comparing `steamship-2.3.9/src/steamship/invocable/lambda_handler.py` & `steamship-2.7.17/src/steamship/invocable/lambda_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 def internal_handler(  # noqa: C901
     invocable_cls_func: Callable[[], Type[Invocable]],
     event: Dict,
     client: Steamship,
     invocation_context: InvocationContext,
+    call_instance_init: bool = False,
 ) -> InvocableResponse:
 
     try:
         request = InvocableRequest.parse_obj(event)
     except SteamshipError as se:
         logging.exception(se)
         return InvocableResponse.from_obj(se)
@@ -56,16 +57,16 @@
         )
     else:
         error_prefix = "[ERROR - ?VERB ?PATH] "
 
     if request.invocation.invocation_path == "/__dir__":
         # Return the DIR result without (1) Constructing invocable_cls or (2) Parsing its config (in the constructor)
         try:
-            cls = invocable_cls_func()
-            return InvocableResponse(json=cls.__steamship_dir__(cls))
+            invocable_class: Type[Invocable] = invocable_cls_func()
+            return InvocableResponse(json=invocable_class.__steamship_dir__(invocable_class))
         except SteamshipError as se:
             logging.exception(se)
             return InvocableResponse.from_obj(se)
         except Exception as ex:
             logging.exception(ex)
             return InvocableResponse.error(
                 code=HTTPStatus.INTERNAL_SERVER_ERROR,
@@ -74,14 +75,18 @@
                 exception=ex,
             )
 
     try:
         invocable = invocable_cls_func()(
             client=client, config=request.invocation.config, context=invocation_context
         )
+        if call_instance_init:
+            # TODO: We don't want to run this every time, but for now we are.
+            logging.info("Running __instance_init__")
+            invocable.instance_init()
     except SteamshipError as se:
         logging.exception(se)
         return InvocableResponse.from_obj(se)
     except Exception as ex:
         logging.exception(ex)
         return InvocableResponse.error(
             code=HTTPStatus.INTERNAL_SERVER_ERROR,
@@ -109,78 +114,67 @@
         return InvocableResponse.error(
             code=HTTPStatus.INTERNAL_SERVER_ERROR,
             prefix=error_prefix,
             exception=ex,
         )
 
 
-def handler(internal_handler, event: Dict, _: Dict = None) -> dict:  # noqa: C901
-    logging_config = event.get("loggingConfig")
+def handler(  # noqa: C901
+    bound_internal_handler, event: Dict, _: Dict = None, running_locally: bool = False
+) -> dict:
+    if not running_locally:
+        logging_config = event.get("loggingConfig")
 
-    if logging_config is None:
-        return InvocableResponse.error(
-            code=HTTPStatus.INTERNAL_SERVER_ERROR,
-            message="Plugin/App handler did not receive a remote logging config.",
-        ).dict(by_alias=True)
+        if logging_config is None:
+            return InvocableResponse.error(
+                code=HTTPStatus.INTERNAL_SERVER_ERROR,
+                message="Plugin/App handler did not receive a remote logging config.",
+            ).dict(by_alias=True)
 
-    logging_host = logging_config.get("loggingHost")
-    logging_port = logging_config.get("loggingPort")
+        logging_host = logging_config.get("loggingHost")
+        logging_port = logging_config.get("loggingPort")
 
-    logging.basicConfig(level=logging.INFO)
-    logging_handler = None
+        logging.basicConfig(level=logging.INFO)
+        logging_handler = None
 
     invocation_context_dict = event.get("invocationContext")
     if invocation_context_dict is None:
         return InvocableResponse.error(
             code=HTTPStatus.INTERNAL_SERVER_ERROR,
             message="Plugin/App handler did not receive an invocation context.",
         ).dict(by_alias=True)
 
     invocation_context = InvocationContext.parse_obj(invocation_context_dict)
+
+    # At the point in the code, the root log level seems to default to WARNING unless set to INFO, even with
+    # the BasicConfig setting to INFO above.
+    logging.root.setLevel(logging.INFO)
+
     # These log statements intentionally go to the logging handler pre-remote attachment, to debug logging configuration issues
-    logging.info(f"Logging host: {logging_host} Logging port: {logging_port}")
+    if not running_locally:
+        logging.info(f"Logging host: {logging_host} Logging port: {logging_port}")
     logging.info(f"Invocation context: {invocation_context}")
 
     if (
-        logging_host != "none"
+        not running_locally and logging_host != "none"
     ):  # Key off the string none, not 'is None', to avoid config errors where remote host isn't passed
         # Configure remote logging
         if logging_host is None:
             return InvocableResponse.error(
                 code=HTTPStatus.INTERNAL_SERVER_ERROR,
                 message="Plugin/App handler did receive a remote logging config, but it did not include a loggingHost.",
             ).dict(by_alias=True)
 
         if logging_port is None:
             return InvocableResponse.error(
                 code=HTTPStatus.INTERNAL_SERVER_ERROR,
                 message="Plugin/App handler did receive a remote logging config, but it did not include a loggingPort.",
             ).dict(by_alias=True)
 
-        custom_format = {
-            "level": "%(levelname)s",
-            "host": "%(hostname)s",
-            "where": "%(module)s.%(filename)s.%(funcName)s:%(lineno)s",
-            "type": "%(levelname)s",
-            "stack_trace": "%(exc_text)s",
-            "component": "package-plugin-lambda",
-            "userId": invocation_context.user_id,
-            "workspaceId": invocation_context.workspace_id,
-            "tenantId": invocation_context.tenant_id,
-            "invocableHandle": invocation_context.invocable_handle,
-            "invocableVersionHandle": invocation_context.invocable_version_handle,
-            "invocableInstanceHandle": invocation_context.invocable_instance_handle,
-            "invocableType": invocation_context.invocable_type,
-            "invocableOwnerId": invocation_context.invocable_owner_id,
-            "path": event.get("invocation", {}).get("invocationPath"),
-        }
-
-        # At the point in the code, the root log level seems to default to WARNING unless set to INFO, even with
-        # the BasicConfig setting to INFO above.
-        logging.root.setLevel(logging.INFO)
+        custom_format = create_custom_format(invocation_context=invocation_context, event=event)
 
         logging_handler = fluenthandler.FluentHandler(
             "steamship.deployed_lambda",
             host=logging_host,
             port=logging_port,
             nanosecond_precision=True,
             msgpack_kwargs={"default": encode_exception},
@@ -206,16 +200,17 @@
     except Exception as ex:
         logging.exception(ex)
         return InvocableResponse.error(
             code=HTTPStatus.INTERNAL_SERVER_ERROR,
             message="Plugin/App handler was unable to create Steamship client.",
             exception=ex,
         ).dict(by_alias=True)
-    logging.info(f"Localstack hostname: {environ.get('LOCALSTACK_HOSTNAME')}.")
-    response = internal_handler(event, client, invocation_context)
+    if not running_locally:
+        logging.info(f"Localstack hostname: {environ.get('LOCALSTACK_HOSTNAME')}.")
+    response = bound_internal_handler(event, client, invocation_context)
 
     result = response.dict(by_alias=True, exclude={"client"})
     # When created with data > 4MB, data is uploaded to a bucket.
     # This is a very ugly way to get the deep size of this object
     data = json.dumps(result.get("data", None)).encode("UTF-8")
     data_size = sys.getsizeof(data)
     logging.info(f"Response data size {data_size}")
@@ -240,20 +235,52 @@
         upload_to_signed_url(signed_url, data)
 
         # Now remove raw data and replace with bucket
         del result["data"]
         result["dataBucket"] = SignedUrl.Bucket.PLUGIN_DATA.value
         result["dataFilepath"] = filepath
 
-    if logging_handler is not None:
+    if not running_locally and logging_handler is not None:
         logging_handler.close()
 
     return result
 
 
+def create_custom_format(
+    invocation_context: InvocationContext, event: Dict
+) -> Callable[[logging.LogRecord], Dict]:
+    def custom_format(record: logging.LogRecord) -> Dict:
+        result = {
+            "level": str(record.levelname),
+            "where": f"{record.module}.{record.filename}.{record.funcName}:{record.lineno}",
+            "type": str(record.levelname),
+            "stack_trace": record.exc_text,
+            "component": "package-plugin-lambda",
+            "userId": invocation_context.user_id,
+            "workspaceId": invocation_context.workspace_id,
+            "tenantId": invocation_context.tenant_id,
+            "invocableHandle": invocation_context.invocable_handle,
+            "invocableVersionHandle": invocation_context.invocable_version_handle,
+            "invocableInstanceHandle": invocation_context.invocable_instance_handle,
+            "invocableType": invocation_context.invocable_type,
+            "invocableOwnerId": invocation_context.invocable_owner_id,
+            "path": event.get("invocation", {}).get("invocationPath"),
+        }
+        # if isinstance(record.args, dict):
+        for key, value in record.__dict__.items():
+            if key not in result:
+                result[key] = str(value)
+        return result
+
+    # Giving the callable a callable attribute is very odd, but required
+    # for the FluentRecordFormatter to work
+    custom_format.usesTime = lambda: True
+    return custom_format
+
+
 def create_handler(invocable_cls: Type[Invocable]):
     """Deprecated wrapper function for a Steamship invocable within an AWS Lambda function. Called by code within a
     plugin or package.
     """
     logging.warning(
         "Creating deprecated (unsafe imports) create_handler. This is no longer necessary. Please remove handler = create_handler(...) from your package or plugin."
     )
```

### Comparing `steamship-2.3.9/src/steamship/invocable/package_service.py` & `steamship-2.7.17/src/steamship/agents/mixins/transports/steamship_widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,89 @@
-from __future__ import annotations
+import uuid
+from typing import List, Optional
 
-import logging
-from typing import Any, Dict, List
+from steamship import Block, Steamship, SteamshipError
+from steamship.agents.llms import OpenAI
+from steamship.agents.mixins.transports.transport import Transport
+from steamship.agents.schema import Agent, AgentContext, Metadata
+from steamship.agents.service.agent_service import AgentService
+from steamship.agents.utils import with_llm
+from steamship.invocable import Config, InvocationContext, post
 
-from steamship import SteamshipError, Task
-from steamship.invocable import Invocable
+API_BASE = "https://api.telegram.org/bot"
 
-# Note!
-# =====
-#
-# This the files in this package are for Package Implementors.
-# If you are using the Steamship Client, you probably are looking for either steamship.client or steamship.data
-#
-from steamship.utils.url import Verb
-
-
-class PackageService(Invocable):
-    """The Abstract Base Class of a Steamship Package.
-
-    Packages may implement whatever methods they like.  To expose these methods as invocable HTTP routes,
-    annotate the method with @get or @post and the route name.
-
-    Package *implementations* are effectively stateless, though they will have stateful
-
-    """
-
-    def invoke_later(
-        self,
-        method: str,
-        verb: Verb = Verb.POST,
-        wait_on_tasks: List[Task] = None,
-        arguments: Dict[str, Any] = None,
-    ) -> Task[Any]:
-        """Schedule a method for future invocation.
-
-        Parameters
-        ----------
-        method: str
-                The method to invoke, as registered with Steamship in the @get or @post decorator.
-        verb:   Verb
-                The HTTP Verb to use. Default is POST.
-        wait_on_tasks: List[Task]
-                A list of Task objects (or task IDs) that should be waited upon before invocation.
-        arguments: Dict[str, Any]
-                The keyword arguments of the invoked   method
-
-        Returns
-        -------
-        Task[Any]
-                A Task representing the future work
-        """
 
-        if self.context is None:
-            raise SteamshipError(
-                message="Unable to call invoke_later because the InvocationContext was None"
-            )
-        if self.context.invocable_instance_handle is None:
-            raise SteamshipError(
-                message="Unable to call invoke_later because the invocable_instance_handle on InvocationContext was None"
-            )
-
-        payload = {
-            "instanceHandle": self.context.invocable_instance_handle,
-            "payload": {
-                "httpVerb": verb.value,
-                "invocationPath": method,
-                "arguments": arguments or {},
-            },
-        }
-        operation = "package/instance/invoke"
+class SteamshipWidgetTransport(Transport):
+    """Experimental base class to encapsulate a Steamship web widget communication channel."""
 
-        logging.info(
-            f"Scheduling {verb} {method} for future invocation on me ({self.context.invocable_handle})"
-        )
+    message_output: List[Block]
+
+    def __init__(self, client: Steamship, agent_service: AgentService, agent: Agent):
+        super().__init__(client=client)
+        self.agent = agent
+        self.agent_service = agent_service
+
+    def instance_init(self, config: Config, context: InvocationContext):
+        pass
+
+    def _instance_deinit(self, *args, **kwargs):
+        """Unsubscribe from updates."""
+        pass
+
+    def _send(self, blocks: [Block], metadata: Metadata):
+        """Send a response to the client.
 
-        resp = self.client.post(
-            operation,
-            payload,
-            expect=Task[Task],  # This operation should return a task
-            as_background_task=True,  # This operation should always be asynchronous
-            wait_on_tasks=wait_on_tasks,  # This operation might await other tasks first
+        TODO: Since this isn't a push, but rather an API return, we need to figure out how to model this.
+        """
+        pass
+
+    @post("info")
+    def info(self) -> dict:
+        return {}
+
+    def _parse_inbound(self, payload: dict, context: Optional[dict] = None) -> Optional[Block]:
+        """Parses an inbound Steamship widget message."""
+
+        message_text = payload.get("question")
+        if message_text is None:
+            raise SteamshipError(f"No 'question' found in Steamship widget message: {payload}")
+
+        chat_id = payload.get("chat_session_id", "default")
+
+        message_id = str(uuid.uuid4())
+
+        result = Block(text=message_text)
+        result.set_chat_id(str(chat_id))
+        result.set_message_id(str(message_id))
+        return result
+
+    @post("answer", public=True)
+    def answer(self, **payload) -> List[Block]:
+        """Endpoint that implements the contract for Steamship embeddable chat widgets. This is a PUBLIC endpoint since these webhooks do not pass a token."""
+        incoming_message = self.parse_inbound(payload)
+        context = AgentContext.get_or_create(
+            self.client, context_keys={"chat_id": incoming_message.chat_id}
+        )
+        context.chat_history.append_user_message(
+            text=incoming_message.text, tags=incoming_message.tags
         )
-        return resp
+        context.emit_funcs = [self.save_for_emit]
+
+        # Add an LLM to the context, using the Agent's if it exists.
+        llm = None
+        if hasattr(self.agent, "llm"):
+            llm = self.agent.llm
+        else:
+            llm = OpenAI(client=self.client)
+
+        context = with_llm(context=context, llm=llm)
+
+        try:
+            self.agent_service.run_agent(self.agent, context)
+        except Exception as e:
+            self.message_output = [self.response_for_exception(e, chat_id=incoming_message.chat_id)]
+
+        # We don't call self.steamship_widget_transport.send because the result is the return value
+        return self.message_output
+
+    def save_for_emit(self, blocks: List[Block], metadata: Metadata):
+        self.message_output = blocks
```

### Comparing `steamship-2.3.9/src/steamship/invocable/plugin_service.py` & `steamship-2.7.17/src/steamship/invocable/plugin_service.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/blockifier/blockifier.py` & `steamship-2.7.17/src/steamship/plugin/blockifier/blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/blockifier/transcriber.py` & `steamship-2.7.17/src/steamship/plugin/blockifier/transcriber.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/embedder.py` & `steamship-2.7.17/src/steamship/plugin/embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/file_importer.py` & `steamship-2.7.17/src/steamship/plugin/file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/inputs/block_and_tag_plugin_input.py` & `steamship-2.7.17/src/steamship/plugin/inputs/block_and_tag_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/inputs/raw_data_plugin_input.py` & `steamship-2.7.17/src/steamship/plugin/inputs/raw_data_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/inputs/train_plugin_input.py` & `steamship-2.7.17/src/steamship/plugin/inputs/train_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/inputs/training_parameter_plugin_input.py` & `steamship-2.7.17/src/steamship/plugin/inputs/training_parameter_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/outputs/model_checkpoint.py` & `steamship-2.7.17/src/steamship/plugin/outputs/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/outputs/raw_data_plugin_output.py` & `steamship-2.7.17/src/steamship/plugin/outputs/raw_data_plugin_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import io
 from typing import Any, Optional, Type, Union
 
 from pydantic import BaseModel
 
 from steamship.base import MimeTypes
-from steamship.base.model import CamelModel
+from steamship.plugin.outputs.plugin_output import PluginOutput
 from steamship.utils.binary_utils import flexi_create
 
 
-class RawDataPluginOutput(CamelModel):
+class RawDataPluginOutput(PluginOutput):
     """Represents mime-typed raw data (or a URL pointing to raw data) that can be returned to the engine.
 
     As a few examples, you can return:
     - Raw text: RawDataPluginOutput(string=raw_text, MimeTypes.TXT)
     - Markdown text: RawDataPluginOutput(string=markdown_text, MimeTypes.MKD)
     - A PNG image: RawDataPluginOutput(bytes=png_bytes, MimeTypes.PNG)
     - A JSON-serializable Dataclass: RawDataPluginOutput(json=dataclass, MimeTypes.JSON)
```

### Comparing `steamship-2.3.9/src/steamship/plugin/outputs/train_plugin_output.py` & `steamship-2.7.17/src/steamship/plugin/outputs/train_plugin_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-from steamship.base.model import CamelModel
+from steamship.plugin.outputs.plugin_output import PluginOutput
 
 
-class TrainPluginOutput(CamelModel):
+class TrainPluginOutput(PluginOutput):
     """
     This is the object produced by a completed trainable operation, stored as the `output` field of a `train` task.
     """
 
     # The PluginInstance ID being trained
     plugin_instance_id: str = None
```

### Comparing `steamship-2.3.9/src/steamship/plugin/outputs/training_parameter_plugin_output.py` & `steamship-2.7.17/src/steamship/plugin/outputs/training_parameter_plugin_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional, Type
 
 from pydantic import BaseModel
 
-from steamship.base.model import CamelModel
 from steamship.plugin.inputs.export_plugin_input import ExportPluginInput
 from steamship.plugin.inputs.training_parameter_plugin_input import TrainingParameterPluginInput
+from steamship.plugin.outputs.plugin_output import PluginOutput
 
 
-class TrainingParameterPluginOutput(CamelModel):
+class TrainingParameterPluginOutput(PluginOutput):
     machine_type: Optional[str] = None
     training_epochs: int = None
     testing_holdout_percent: float = None
     test_split_seed: int = None
     training_params: Dict[str, Any] = None
     inference_params: Dict[str, Any] = None
     export_request: ExportPluginInput = None
```

### Comparing `steamship-2.3.9/src/steamship/plugin/request.py` & `steamship-2.7.17/src/steamship/plugin/request.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/tagger.py` & `steamship-2.7.17/src/steamship/plugin/tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/plugin/trainable_model.py` & `steamship-2.7.17/src/steamship/plugin/trainable_model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/binary_utils.py` & `steamship-2.7.17/src/steamship/utils/binary_utils.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/huggingface_helper.py` & `steamship-2.7.17/src/steamship/utils/huggingface_helper.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/kv_store.py` & `steamship-2.7.17/src/steamship/utils/kv_store.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/signed_urls.py` & `steamship-2.7.17/src/steamship/utils/signed_urls.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/url.py` & `steamship-2.7.17/src/steamship/utils/url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship/utils/zip_archives.py` & `steamship-2.7.17/src/steamship/utils/zip_archives.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/src/steamship.egg-info/SOURCES.txt` & `steamship-2.7.17/src/steamship.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,67 +3,108 @@
 .pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 DEVELOPING.md
 LICENSE
 README.md
 TESTING.md
+badge.svg
 pyproject.toml
 requirements.dev.txt
 requirements.txt
 .devcontainer/Dockerfile
 .devcontainer/base.Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/library-scripts/README.md
 .devcontainer/library-scripts/common-debian.sh
 .devcontainer/library-scripts/meta.env
 .devcontainer/library-scripts/node-debian.sh
 .devcontainer/library-scripts/python-debian.sh
 .github/workflows/docs-publish.yml
+.github/workflows/notify-of-release.yml
 .github/workflows/python-publish.yml
 .github/workflows/test-main.yml
 .github/workflows/test-staging.yml
 docs/.nojekyll
+docs/Dockerfile
 docs/Makefile
 docs/README.txt
 docs/authors.rst
 docs/changelog._rst
 docs/conf.py
+docs/favicon.ico
 docs/index.rst
 docs/license.rst
 docs/requirements.txt
 docs/_static/.gitignore
 docs/_static/Steamship-symbol-dark.png
 docs/_static/Steamship-symbol-light.png
 docs/_static/favicon.ico
 docs/_templates/base.html
+docs/agents/index.rst
 docs/api/modules.rst
+docs/api/steamship.agents.examples.rst
+docs/api/steamship.agents.llms.rst
+docs/api/steamship.agents.mixins.rst
+docs/api/steamship.agents.mixins.transports.rst
+docs/api/steamship.agents.react.rst
+docs/api/steamship.agents.rst
+docs/api/steamship.agents.schema.rst
+docs/api/steamship.agents.service.rst
+docs/api/steamship.agents.tools.audio_transcription.rst
+docs/api/steamship.agents.tools.classification.rst
+docs/api/steamship.agents.tools.conversation_starters.rst
+docs/api/steamship.agents.tools.image_generation.rst
+docs/api/steamship.agents.tools.question_answering.rst
+docs/api/steamship.agents.tools.rst
+docs/api/steamship.agents.tools.search.rst
+docs/api/steamship.agents.tools.speech_generation.rst
+docs/api/steamship.agents.tools.text_generation.rst
+docs/api/steamship.agents.tools.video_generation.rst
 docs/api/steamship.base.rst
+docs/api/steamship.cli.local_server.rst
+docs/api/steamship.cli.rst
 docs/api/steamship.client.rst
+docs/api/steamship.experimental.easy.rst
+docs/api/steamship.experimental.package_starters.rst
+docs/api/steamship.experimental.rst
+docs/api/steamship.invocable.mixins.rst
 docs/api/steamship.invocable.rst
 docs/api/steamship.plugin.blockifier.rst
 docs/api/steamship.plugin.inputs.rst
 docs/api/steamship.plugin.outputs.rst
 docs/api/steamship.plugin.rst
 docs/api/steamship.rst
 docs/api/steamship.utils.rst
 docs/configuration/authentication.rst
 docs/configuration/cli.rst
 docs/configuration/clients.rst
 docs/configuration/http.rst
 docs/configuration/index.rst
+docs/data/blocks.rst
+docs/data/file-lifecycle.png
+docs/data/files.rst
+docs/data/index.rst
+docs/data/tags.rst
+docs/data/workspaces.rst
+docs/data/queries/index.rst
 docs/developing/configuration.rst
 docs/developing/deploying.rst
 docs/developing/environment-setup.rst
 docs/developing/index.rst
+docs/developing/logs-example.png
+docs/developing/monitoring.rst
 docs/developing/project-creation.rst
+docs/developing/running.rst
 docs/developing/steamship-manifest.rst
 docs/developing/storing-secrets.rst
+docs/developing/tasks-example.png
 docs/developing/testing.rst
-docs/developing/updating-web-listing.rst
+docs/developing/usage-example.png
+docs/embedding-search/index.rst
 docs/packages/index.rst
 docs/packages/using.rst
 docs/packages/cookbook/adding-configuration.rst
 docs/packages/cookbook/article-tagging.rst
 docs/packages/cookbook/collecting-and-querying-sentiment.rst
 docs/packages/cookbook/how-to-extract-outline-from-markdown.rst
 docs/packages/cookbook/index.rst
@@ -72,81 +113,152 @@
 docs/packages/cookbook/return-audio.rst
 docs/packages/cookbook/return-image.rst
 docs/packages/cookbook/return-json.rst
 docs/packages/cookbook/return-text.rst
 docs/packages/developing/index.rst
 docs/packages/developing/project-structure.rst
 docs/plugins/index.rst
-docs/plugins/blockifiers/developing.rst
-docs/plugins/blockifiers/index.rst
-docs/plugins/blockifiers/using.rst
 docs/plugins/developing/async-plugins.rst
 docs/plugins/developing/blockifiers.rst
 docs/plugins/developing/embedders.rst
+docs/plugins/developing/generators.rst
 docs/plugins/developing/importers.rst
 docs/plugins/developing/index.rst
 docs/plugins/developing/project-structure.rst
 docs/plugins/developing/taggers.rst
-docs/plugins/embedders/index.rst
-docs/plugins/embedders/using.rst
-docs/plugins/importers/index.rst
-docs/plugins/importers/using.rst
-docs/plugins/taggers/index.rst
-docs/plugins/taggers/using.rst
-docs/workspaces/blockifying.rst
-docs/workspaces/creating.rst
-docs/workspaces/importing.rst
-docs/workspaces/index.rst
-docs/workspaces/data_model/blocks.rst
-docs/workspaces/data_model/files.rst
-docs/workspaces/data_model/index.rst
-docs/workspaces/data_model/tags.rst
-docs/workspaces/queries/index.rst
+docs/plugins/using/index.rst
+docs/plugins/using/tasks.rst
+docs/plugins/using/blockifiers/index.rst
+docs/plugins/using/blockifiers/using.rst
+docs/plugins/using/embedders/index.rst
+docs/plugins/using/generators/dalle.rst
+docs/plugins/using/generators/gpt4.rst
+docs/plugins/using/generators/index.rst
+docs/plugins/using/importers/index.rst
+docs/plugins/using/importers/using.rst
+docs/plugins/using/taggers/index.rst
+docs/plugins/using/taggers/using.rst
 scripts/build-docs.sh
 scripts/create_engine_test_assets.py
 src/steamship/__init__.py
 src/steamship.egg-info/PKG-INFO
 src/steamship.egg-info/SOURCES.txt
 src/steamship.egg-info/dependency_links.txt
 src/steamship.egg-info/entry_points.txt
 src/steamship.egg-info/requires.txt
 src/steamship.egg-info/top_level.txt
+src/steamship/agents/__init__.py
+src/steamship/agents/logging.py
+src/steamship/agents/utils.py
+src/steamship/agents/examples/__init__.py
+src/steamship/agents/examples/document_qa_agent.py
+src/steamship/agents/examples/example_assistant.py
+src/steamship/agents/examples/example_react_assistant.py
+src/steamship/agents/examples/fact_learner.py
+src/steamship/agents/examples/telegram_bot.py
+src/steamship/agents/functional/__init__.py
+src/steamship/agents/functional/functions_based.py
+src/steamship/agents/functional/output_parser.py
+src/steamship/agents/llms/__init__.py
+src/steamship/agents/llms/openai.py
+src/steamship/agents/mixins/__init__.py
+src/steamship/agents/mixins/transports/__init__.py
+src/steamship/agents/mixins/transports/steamship_widget.py
+src/steamship/agents/mixins/transports/telegram.py
+src/steamship/agents/mixins/transports/transport.py
+src/steamship/agents/react/__init__.py
+src/steamship/agents/react/output_parser.py
+src/steamship/agents/react/react.py
+src/steamship/agents/schema/__init__.py
+src/steamship/agents/schema/action.py
+src/steamship/agents/schema/agent.py
+src/steamship/agents/schema/chathistory.py
+src/steamship/agents/schema/context.py
+src/steamship/agents/schema/functions.py
+src/steamship/agents/schema/llm.py
+src/steamship/agents/schema/message_selectors.py
+src/steamship/agents/schema/output_parser.py
+src/steamship/agents/schema/text_splitters.py
+src/steamship/agents/schema/tool.py
+src/steamship/agents/service/__init__.py
+src/steamship/agents/service/agent_service.py
+src/steamship/agents/tools/__init__.py
+src/steamship/agents/tools/base_tools.py
+src/steamship/agents/tools/audio_transcription/__init__.py
+src/steamship/agents/tools/audio_transcription/assembly_speech_to_text_tool.py
+src/steamship/agents/tools/audio_transcription/fetch_audio_urls_from_rss_tool.py
+src/steamship/agents/tools/audio_transcription/whisper_speech_to_text_tool.py
+src/steamship/agents/tools/classification/__init__.py
+src/steamship/agents/tools/classification/sentiment_analysis_tool.py
+src/steamship/agents/tools/classification/zero_shot_classifier_tool.py
+src/steamship/agents/tools/conversation_starters/__init__.py
+src/steamship/agents/tools/conversation_starters/knock_knock_tool.py
+src/steamship/agents/tools/image_generation/__init__.py
+src/steamship/agents/tools/image_generation/dalle.py
+src/steamship/agents/tools/image_generation/google_image_search.py
+src/steamship/agents/tools/image_generation/stable_diffusion.py
+src/steamship/agents/tools/question_answering/__init__.py
+src/steamship/agents/tools/question_answering/prompt_database_question_answerer.py
+src/steamship/agents/tools/question_answering/vector_search_learner_tool.py
+src/steamship/agents/tools/question_answering/vector_search_qa_tool.py
+src/steamship/agents/tools/question_answering/vector_search_tool.py
+src/steamship/agents/tools/search/__init__.py
+src/steamship/agents/tools/search/search.py
+src/steamship/agents/tools/speech_generation/__init__.py
+src/steamship/agents/tools/speech_generation/generate_speech.py
+src/steamship/agents/tools/text_generation/__init__.py
+src/steamship/agents/tools/text_generation/image_prompt_generator_tool.py
+src/steamship/agents/tools/text_generation/json_object_generator.py
+src/steamship/agents/tools/text_generation/personality_tool.py
+src/steamship/agents/tools/text_generation/summarize_text_with_prompt_tool.py
+src/steamship/agents/tools/text_generation/text_rewrite_tool.py
+src/steamship/agents/tools/text_generation/text_translation_tool.py
+src/steamship/agents/tools/video_generation/__init__.py
+src/steamship/agents/tools/video_generation/did_video_generator_tool.py
 src/steamship/base/__init__.py
 src/steamship/base/client.py
 src/steamship/base/configuration.py
 src/steamship/base/environments.py
 src/steamship/base/error.py
 src/steamship/base/mime_types.py
 src/steamship/base/model.py
 src/steamship/base/package_spec.py
 src/steamship/base/request.py
 src/steamship/base/response.py
 src/steamship/base/tasks.py
-src/steamship/base/utils.py
 src/steamship/cli/__init__.py
 src/steamship/cli/cli.py
+src/steamship/cli/create_instance.py
 src/steamship/cli/deploy.py
 src/steamship/cli/login.py
 src/steamship/cli/manifest_init_wizard.py
+src/steamship/cli/requirements_init_wizard.py
 src/steamship/cli/ship_spinner.py
+src/steamship/cli/utils.py
+src/steamship/cli/local_server/__init__.py
+src/steamship/cli/local_server/handler.py
+src/steamship/cli/local_server/server.py
 src/steamship/client/__init__.py
 src/steamship/client/skill_to_provider.py
 src/steamship/client/skills.py
 src/steamship/client/steamship.py
 src/steamship/client/vendors.py
 src/steamship/data/__init__.py
 src/steamship/data/block.py
 src/steamship/data/embeddings.py
 src/steamship/data/file.py
+src/steamship/data/invocable_init_status.py
+src/steamship/data/manifest.py
 src/steamship/data/search.py
 src/steamship/data/user.py
 src/steamship/data/workspace.py
 src/steamship/data/operations/__init__.py
 src/steamship/data/operations/blockifier.py
 src/steamship/data/operations/embedder.py
+src/steamship/data/operations/generator.py
 src/steamship/data/operations/tagger.py
 src/steamship/data/package/__init__.py
 src/steamship/data/package/package.py
 src/steamship/data/package/package_instance.py
 src/steamship/data/package/package_version.py
 src/steamship/data/plugin/__init__.py
 src/steamship/data/plugin/hosting.py
@@ -154,84 +266,123 @@
 src/steamship/data/plugin/plugin.py
 src/steamship/data/plugin/plugin_instance.py
 src/steamship/data/plugin/plugin_version.py
 src/steamship/data/plugin/prompt_generation_plugin_instance.py
 src/steamship/data/tags/__init__.py
 src/steamship/data/tags/tag.py
 src/steamship/data/tags/tag_constants.py
+src/steamship/experimental/__init__.py
+src/steamship/experimental/easy/__init__.py
+src/steamship/experimental/easy/tags.py
+src/steamship/experimental/package_starters/telegram_agent.py
+src/steamship/experimental/package_starters/web_agent.py
 src/steamship/invocable/__init__.py
 src/steamship/invocable/config.py
+src/steamship/invocable/dev_logging_handler.py
 src/steamship/invocable/entrypoint.py
 src/steamship/invocable/invocable.py
+src/steamship/invocable/invocable_localhost.py
 src/steamship/invocable/invocable_request.py
 src/steamship/invocable/invocable_response.py
 src/steamship/invocable/lambda_handler.py
-src/steamship/invocable/manifest.py
+src/steamship/invocable/package_mixin.py
 src/steamship/invocable/package_service.py
 src/steamship/invocable/paramater_types.py
 src/steamship/invocable/plugin_service.py
+src/steamship/invocable/mixins/__init__.py
+src/steamship/invocable/mixins/blockifier_mixin.py
+src/steamship/invocable/mixins/file_importer_mixin.py
+src/steamship/invocable/mixins/indexer_mixin.py
+src/steamship/invocable/mixins/indexer_pipeline_mixin.py
 src/steamship/plugin/__init__.py
 src/steamship/plugin/embedder.py
 src/steamship/plugin/file_importer.py
+src/steamship/plugin/generator.py
 src/steamship/plugin/request.py
 src/steamship/plugin/tagger.py
 src/steamship/plugin/trainable_model.py
 src/steamship/plugin/blockifier/__init__.py
 src/steamship/plugin/blockifier/blockifier.py
 src/steamship/plugin/blockifier/transcriber.py
 src/steamship/plugin/inputs/__init__.py
 src/steamship/plugin/inputs/block_and_tag_plugin_input.py
 src/steamship/plugin/inputs/export_plugin_input.py
 src/steamship/plugin/inputs/file_import_plugin_input.py
+src/steamship/plugin/inputs/raw_block_and_tag_plugin_input.py
 src/steamship/plugin/inputs/raw_data_plugin_input.py
 src/steamship/plugin/inputs/train_plugin_input.py
 src/steamship/plugin/inputs/training_parameter_plugin_input.py
 src/steamship/plugin/outputs/__init__.py
 src/steamship/plugin/outputs/block_and_tag_plugin_output.py
 src/steamship/plugin/outputs/embedded_items_plugin_output.py
 src/steamship/plugin/outputs/model_checkpoint.py
+src/steamship/plugin/outputs/plugin_output.py
+src/steamship/plugin/outputs/raw_block_and_tag_plugin_output.py
 src/steamship/plugin/outputs/raw_data_plugin_output.py
 src/steamship/plugin/outputs/train_plugin_output.py
 src/steamship/plugin/outputs/training_parameter_plugin_output.py
 src/steamship/utils/__init__.py
 src/steamship/utils/binary_utils.py
+src/steamship/utils/context_length.py
+src/steamship/utils/file_tags.py
 src/steamship/utils/huggingface_helper.py
 src/steamship/utils/kv_store.py
 src/steamship/utils/metadata.py
+src/steamship/utils/repl.py
 src/steamship/utils/signed_urls.py
 src/steamship/utils/url.py
 src/steamship/utils/utils.py
 src/steamship/utils/zip_archives.py
 tests/__init__.py
 tests/conftest.py
 tests/assets/__init__.py
 tests/assets/demo_package_spec.json
 tests/assets/palm_tree.png
+tests/assets/test.pdf
 tests/assets/utterances.csv
 tests/assets/utterances.tsv
 tests/assets/configs/empty_json.json
 tests/assets/configs/one_string_one_int.json
 tests/assets/configs/single_integer.json
 tests/assets/packages/__init__.py
+tests/assets/packages/adding_configuration.py
+tests/assets/packages/article_tagging.py
 tests/assets/packages/bad_package.py
 tests/assets/packages/configurable_hello_world.py
 tests/assets/packages/demo_package.py
+tests/assets/packages/example_project_structure.py
 tests/assets/packages/fancy_types.py
 tests/assets/packages/hello_world.py
 tests/assets/packages/optional_params.py
+tests/assets/packages/package_verifying_instance_init.py
+tests/assets/packages/package_with_failing_instance_init.py
+tests/assets/packages/package_with_instance_init.py
+tests/assets/packages/package_with_mixin_importer.py
+tests/assets/packages/package_with_mixin_indexer_pipeline.py
+tests/assets/packages/package_with_mixins.py
+tests/assets/packages/requirement_isolation_package.py
 tests/assets/packages/returns_list.py
 tests/assets/packages/safe_loaded_bad_import.pyignore
 tests/assets/packages/safe_loaded_hello_world.py
 tests/assets/packages/signed_url_package.py
+tests/assets/packages/transports/__init__.py
+tests/assets/packages/transports/mock_telegram_package.py
+tests/assets/packages/transports/test_telegram_agent.py
+tests/assets/packages/transports/test_web_agent.py
 tests/assets/plugins/__init__.py
 tests/assets/plugins/blockifiers/__init__.py
 tests/assets/plugins/blockifiers/async_blockifier.py
 tests/assets/plugins/blockifiers/blockifier.py
 tests/assets/plugins/blockifiers/csv_blockifier.py
 tests/assets/plugins/blockifiers/tsv_blockifier.py
+tests/assets/plugins/generators/async_generator.py
+tests/assets/plugins/generators/plugin_with_instance_init.py
+tests/assets/plugins/generators/test_generator.py
+tests/assets/plugins/generators/test_generator_returns_bytes.py
+tests/assets/plugins/generators/test_image_to_text_generator.py
 tests/assets/plugins/importers/__init__.py
 tests/assets/plugins/importers/plugin_file_importer.py
 tests/assets/plugins/importers/plugin_file_importer_by_url.py
 tests/assets/plugins/importers/plugin_file_importer_python_error.py
 tests/assets/plugins/importers/plugin_file_importer_steamship_error.py
 tests/assets/plugins/taggers/__init__.py
 tests/assets/plugins/taggers/plugin_configurable_tagger.py
@@ -240,28 +391,53 @@
 tests/assets/plugins/taggers/plugin_parser.py
 tests/assets/plugins/taggers/plugin_prompt_generator.py
 tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore
 tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py
 tests/assets/plugins/taggers/plugin_trainable_tagger.py
 tests/assets/plugins/taggers/plugin_trainable_tagger_config.py
 tests/steamship_tests/__init__.py
+tests/steamship_tests/agents/__init__.py
+tests/steamship_tests/agents/test_chat_history.py
+tests/steamship_tests/agents/test_function_agent_output_parser.py
+tests/steamship_tests/agents/test_functions_based_agent.py
+tests/steamship_tests/agents/test_message_formatting.py
+tests/steamship_tests/agents/test_openai.py
+tests/steamship_tests/agents/test_qa_agent.py
+tests/steamship_tests/agents/test_react_parse_output.py
+tests/steamship_tests/agents/test_telegram.py
+tests/steamship_tests/agents/test_web.py
+tests/steamship_tests/agents/tools/__init__.py
 tests/steamship_tests/app/__init__.py
 tests/steamship_tests/app/integration/__init__.py
+tests/steamship_tests/app/integration/test_adding_configuration.py
+tests/steamship_tests/app/integration/test_article_tagging.py
 tests/steamship_tests/app/integration/test_configurable_package_instance.py
+tests/steamship_tests/app/integration/test_e2e_mixins.py
+tests/steamship_tests/app/integration/test_e2e_mixins_importer_blockifier.py
+tests/steamship_tests/app/integration/test_e2e_mixins_indexer_pipeline.py
+tests/steamship_tests/app/integration/test_example_project_structure.py
+tests/steamship_tests/app/integration/test_instance_init.py
 tests/steamship_tests/app/integration/test_package_error_visibility.py
 tests/steamship_tests/app/integration/test_package_instance.py
+tests/steamship_tests/app/integration/test_requirements_installation_isolation.py
 tests/steamship_tests/app/integration/test_returns_list.py
 tests/steamship_tests/app/integration/test_safe_hello_world.py
 tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py
 tests/steamship_tests/app/integration/test_signed_url_package.py
 tests/steamship_tests/app/integration/test_use_package.py
 tests/steamship_tests/app/unit/__init__.py
 tests/steamship_tests/app/unit/test_config_template_extraction.py
 tests/steamship_tests/app/unit/test_demo_app_spec.py
+tests/steamship_tests/app/unit/test_document_qa_example.py
+tests/steamship_tests/app/unit/test_indexer_mixin.py
+tests/steamship_tests/app/unit/test_indexer_pipeline_mixin.py
+tests/steamship_tests/app/unit/test_mixins.py
+tests/steamship_tests/app/unit/test_multi_inheritance.py
 tests/steamship_tests/app/unit/test_response.py
+tests/steamship_tests/app/unit/test_routes_on_superclasses.py
 tests/steamship_tests/app/unit/test_training_input.py
 tests/steamship_tests/base/__init__.py
 tests/steamship_tests/base/test_binary_utils.py
 tests/steamship_tests/base/test_configuration.py
 tests/steamship_tests/base/test_serialization.py
 tests/steamship_tests/base/test_steamship_error_serializable.py
 tests/steamship_tests/base/test_task.py
@@ -271,41 +447,44 @@
 tests/steamship_tests/client/operations/__init__.py
 tests/steamship_tests/client/operations/test_blockify.py
 tests/steamship_tests/client/operations/test_classify.py
 tests/steamship_tests/client/operations/test_convert_ocr.py
 tests/steamship_tests/client/operations/test_embed.py
 tests/steamship_tests/client/operations/test_embed_file.py
 tests/steamship_tests/client/operations/test_embedding_index.py
-tests/steamship_tests/client/operations/test_embedding_index_snapshot.py
 tests/steamship_tests/client/operations/test_tag.py
 tests/steamship_tests/client/operations/test_tag_file.py
 tests/steamship_tests/data/__init__.py
 tests/steamship_tests/data/test_app_version.py
 tests/steamship_tests/data/test_block.py
+tests/steamship_tests/data/test_chat.py
 tests/steamship_tests/data/test_file.py
 tests/steamship_tests/data/test_img.png
 tests/steamship_tests/data/test_package.py
 tests/steamship_tests/data/test_package_version.py
 tests/steamship_tests/data/test_plugins.py
 tests/steamship_tests/data/test_task_comments.py
 tests/steamship_tests/data/test_workspace.py
 tests/steamship_tests/data/utterances.csv
 tests/steamship_tests/data/tags/__init__.py
 tests/steamship_tests/data/tags/test_file_tags.py
+tests/steamship_tests/experimental/__init__.py
 tests/steamship_tests/plugin/__init__.py
 tests/steamship_tests/plugin/integration/__init__.py
 tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py
+tests/steamship_tests/plugin/integration/test_e2e_async_generator.py
 tests/steamship_tests/plugin/integration/test_e2e_blockifier.py
 tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py
 tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py
 tests/steamship_tests/plugin/integration/test_e2e_corpus_importer.py
 tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py
 tests/steamship_tests/plugin/integration/test_e2e_embedder.py
 tests/steamship_tests/plugin/integration/test_e2e_file_importer.py
 tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py
+tests/steamship_tests/plugin/integration/test_e2e_generator.py
 tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py
 tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py
 tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py
 tests/steamship_tests/plugin/integration/test_e2e_tagger.py
 tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py
 tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py
 tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py
@@ -324,14 +503,15 @@
 tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py
 tests/steamship_tests/plugin/unit/trainable/util.py
 tests/steamship_tests/server/__init__.py
 tests/steamship_tests/server/test_package_local.py
 tests/steamship_tests/server/test_task_timeout.py
 tests/steamship_tests/utils/__init__.py
 tests/steamship_tests/utils/client.py
+tests/steamship_tests/utils/context.py
 tests/steamship_tests/utils/deployables.py
 tests/steamship_tests/utils/file.py
 tests/steamship_tests/utils/fixtures.py
 tests/steamship_tests/utils/random.py
 tests/steamship_tests/utils/test_camel_model.py
 tests/steamship_tests/utils/test_client.py
 tests/steamship_tests/utils/test_enums.py
```

### Comparing `steamship-2.3.9/tests/assets/packages/configurable_hello_world.py` & `steamship-2.7.17/tests/assets/packages/configurable_hello_world.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/packages/demo_package.py` & `steamship-2.7.17/tests/assets/packages/demo_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,22 @@
     def greet1(self, name: str = "Person") -> InvocableResponse[str]:
         return InvocableResponse(string=f"Hello, {name}!")
 
     @post("greet")
     def greet2(self, name: str = "Person") -> InvocableResponse[str]:
         return InvocableResponse(string=f"Hello, {name}!")
 
+    @post("public_post_greet", public=True)
+    def public_post_greet(self, name: str = "Person") -> InvocableResponse[str]:
+        return InvocableResponse(string=f"Hello, {name}!")
+
+    @get("public_get_greet", public=True)
+    def public_get_greet(self, name: str = "Person") -> InvocableResponse[str]:
+        return InvocableResponse(string=f"Hello, {name}!")
+
     @post("future_greet")
     def future_greet(self, name: str = "Person") -> InvocableResponse[Task]:
         task_1 = self.invoke_later("greet", arguments={"name": name})
         return InvocableResponse(json=task_1)
 
     @post("future_greet_then_greet_again")
     def future_greet_then_greet_again(self, name: str = "Person") -> InvocableResponse[Task]:
@@ -113,15 +121,15 @@
     def get_config(self) -> InvocableResponse[dict]:
         """This is called get_config because there's already `.config` object on the class."""
         return InvocableResponse(
             json={
                 "workspaceId": self.client.config.workspace_id,
                 "appBase": self.client.config.app_base,
                 "apiBase": self.client.config.api_base,
-                "apiKey": self.client.config.api_key,
+                "apiKey": self.client.config.api_key.get_secret_value(),
             }
         )
 
     @post("learn")
     def learn(self, fact: str = None) -> InvocableResponse[dict]:
         """Learns a new fact."""
         if fact is None:
```

### Comparing `steamship-2.3.9/tests/assets/packages/fancy_types.py` & `steamship-2.7.17/tests/assets/packages/fancy_types.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/packages/hello_world.py` & `steamship-2.7.17/tests/assets/packages/hello_world.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from steamship.invocable import Invocable, InvocableResponse, get, post
+from steamship.invocable import InvocableResponse, PackageService, get, post
 from steamship.invocable.lambda_handler import create_safe_handler
 
 
-class HelloWorld(Invocable):
+class HelloWorld(PackageService):
     @post("greet")
     def greet(self, name: str = "Person") -> InvocableResponse:
         return InvocableResponse(string=f"Hello, {name}")
 
     @get("workspace")
     def workspace(self) -> InvocableResponse:
         return InvocableResponse(string=self.client.config.workspace_id)
```

### Comparing `steamship-2.3.9/tests/assets/packages/safe_loaded_bad_import.pyignore` & `steamship-2.7.17/tests/assets/packages/safe_loaded_bad_import.pyignore`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/packages/signed_url_package.py` & `steamship-2.7.17/tests/assets/packages/signed_url_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/palm_tree.png` & `steamship-2.7.17/tests/assets/palm_tree.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/blockifiers/async_blockifier.py` & `steamship-2.7.17/tests/assets/plugins/blockifiers/async_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/blockifiers/blockifier.py` & `steamship-2.7.17/tests/assets/plugins/blockifiers/blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/blockifiers/csv_blockifier.py` & `steamship-2.7.17/tests/assets/plugins/blockifiers/csv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/blockifiers/tsv_blockifier.py` & `steamship-2.7.17/tests/assets/plugins/blockifiers/tsv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer.py` & `steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_by_url.py` & `steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_by_url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_python_error.py` & `steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_python_error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py` & `steamship-2.7.17/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_configurable_tagger.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_configurable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_embedder.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_logging_tagger.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_logging_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_parser.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_prompt_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,32 @@
-import logging
-import re
-
-from steamship import Block, DocTag, Tag
-from steamship.data import TagKind
-from steamship.invocable import InvocableResponse
+from steamship import Block, File, Tag
+from steamship.data import GenerationTag, TagKind, TagValueKey
+from steamship.invocable import InvocableResponse, create_handler
 from steamship.invocable.plugin_service import PluginRequest
 from steamship.plugin.inputs.block_and_tag_plugin_input import BlockAndTagPluginInput
 from steamship.plugin.outputs.block_and_tag_plugin_output import BlockAndTagPluginOutput
 from steamship.plugin.tagger import Tagger
 
-# If this isn't present, Localstack won't show logs
-logging.getLogger().setLevel(logging.INFO)
-
-
-def tag_sentences(block: Block):
-    """Splits the document into sentences by assuming a period is a sentence divider."""
-    # Add the period back
-    tags = []
-    for m in re.finditer(r"[^.]+", block.text):
-        tags.append(
-            Tag(
-                kind=TagKind.DOCUMENT,
-                name=DocTag.SENTENCE,
-                start_idx=m.start(),
-                end_idx=m.end() + 1,
-            )
-        )
-    if block.tags:
-        block.tags.extend(tags)
-    else:
-        block.tags = tags
-
-
-class TestParserPlugin(Tagger):
-    # TODO: WARNING! We will need to implement some logic that prevents
-    # a distributed endless loop. E.g., a parser plugin returning the results
-    # of using the Steamship client to call parse.. via itself!
 
+class TestPromptGeneratorPlugin(Tagger):
     def run(
         self, request: PluginRequest[BlockAndTagPluginInput]
     ) -> InvocableResponse[BlockAndTagPluginOutput]:
-        logging.info(f"Inside parser: {type(request)}")
-        file = request.data.file
-        for block in file.blocks:
-            tag_sentences(block)
-        if request.data is not None:
-            ret = InvocableResponse(data=BlockAndTagPluginOutput(file=file))
-            logging.info(f"Ret: {ret}")
-            return ret
+        """Merely returns the prompt."""
+        request_file = request.data.file
+        output = BlockAndTagPluginOutput(file=File(id=request_file.id), tags=[])
+        for block in request.data.file.blocks:
+            text = block.text
+            tags = [
+                Tag(
+                    kind=TagKind.GENERATION,
+                    name=GenerationTag.PROMPT_COMPLETION,
+                    value={TagValueKey.STRING_VALUE: text},
+                )
+            ]
+            output_block = Block(id=block.id, tags=tags)
+            output.file.blocks.append(output_block)
+
+        return InvocableResponse(data=output)
+
+
+handler = create_handler(TestPromptGeneratorPlugin)
```

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_prompt_generator.py` & `steamship-2.7.17/tests/assets/plugins/generators/test_image_to_text_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from steamship import Block, File, Tag
-from steamship.data import GenerationTag, TagKind, TagValueKey
-from steamship.invocable import InvocableResponse, create_handler
-from steamship.invocable.plugin_service import PluginRequest
-from steamship.plugin.inputs.block_and_tag_plugin_input import BlockAndTagPluginInput
-from steamship.plugin.outputs.block_and_tag_plugin_output import BlockAndTagPluginOutput
-from steamship.plugin.tagger import Tagger
+from steamship import Block, MimeTypes
+from steamship.invocable import InvocableResponse
+from steamship.plugin.generator import Generator
+from steamship.plugin.inputs.raw_block_and_tag_plugin_input import RawBlockAndTagPluginInput
+from steamship.plugin.outputs.plugin_output import UsageReport
+from steamship.plugin.outputs.raw_block_and_tag_plugin_output import RawBlockAndTagPluginOutput
+from steamship.plugin.request import PluginRequest
 
 
-class TestPromptGeneratorPlugin(Tagger):
+class TestGenerator(Generator):
     def run(
-        self, request: PluginRequest[BlockAndTagPluginInput]
-    ) -> InvocableResponse[BlockAndTagPluginOutput]:
-        """Merely returns the prompt."""
-        request_file = request.data.file
-        output = BlockAndTagPluginOutput(file=File(id=request_file.id), tags=[])
-        for block in request.data.file.blocks:
-            text = block.text
-            tags = [
-                Tag(
-                    kind=TagKind.GENERATION,
-                    name=GenerationTag.PROMPT_COMPLETION,
-                    value={TagValueKey.STRING_VALUE: text},
-                )
-            ]
-            output_block = Block(id=block.id, tags=tags)
-            output.file.blocks.append(output_block)
+        self, request: PluginRequest[RawBlockAndTagPluginInput]
+    ) -> InvocableResponse[RawBlockAndTagPluginOutput]:
+        image_blocks = 0
+        fetched_raw = 0
+        for block in request.data.blocks:
+            if block.mime_type == MimeTypes.PNG:
+                image_blocks += 1
+                _ = block.raw()
+                fetched_raw += 1
 
-        return InvocableResponse(data=output)
-
-
-handler = create_handler(TestPromptGeneratorPlugin)
+        output_text = f"Found {image_blocks} image blocks and fetched data from {fetched_raw}"
+        return InvocableResponse(
+            data=RawBlockAndTagPluginOutput(
+                blocks=[Block(text=output_text)], usage=[UsageReport.run_units(1)]
+            )
+        )
```

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py` & `steamship-2.7.17/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_configurable_package_instance.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_configurable_package_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+import pytest
 from steamship_tests import PACKAGES_PATH
 from steamship_tests.utils.deployables import deploy_package
-from steamship_tests.utils.fixtures import get_steamship_client
 
-from steamship import PackageInstance
+from steamship import PackageInstance, Steamship
 
 
-def test_configurable_instance_invoke():
+@pytest.mark.usefixtures("client")
+def test_configurable_instance_invoke(client: Steamship):
     greeting1 = "Hola"
     config_template = {
         "greeting": {"type": "string"},
         "snake_case_config": {"type": "string"},
         "camelCaseConfig": {"type": "string"},
         "defaultConfig": {"type": "string", "default": "defaulted"},
     }
     instance_config = {
         "greeting": greeting1,
         "snake_case_config": "hisss",
         "camelCaseConfig": "spit!",
     }
-    client = get_steamship_client()
     hello_world_path = PACKAGES_PATH / "configurable_hello_world.py"
 
     with deploy_package(
         client,
         hello_world_path,
         version_config_template=config_template,
         instance_config=instance_config,
@@ -46,14 +46,15 @@
             "greeting": greeting2,
             "snake_case_config": "hisss",
             "camelCaseConfig": "spit!",
         }
         instance2 = PackageInstance.create(
             client, package_id=package.id, package_version_id=version.id, config=instance_config2
         )
+        instance2.wait_for_init()
 
         res2 = instance2.invoke("greet")
         assert res2 == f"{greeting2}, Person"
 
         # Test with quick-create
         greeting3 = "Howdy"
         instance_config3 = {
@@ -75,7 +76,18 @@
             "greeting": greeting4,
             "snake_case_config": "hisss",
             "camelCaseConfig": "spit!",
         }
         instance4 = client.use(package.handle, config=instance_config4)
         assert instance4.invoke("greet") == f"{greeting4}, Person"
         assert instance4.id != instance3.id
+
+        # Test instance with configuration in Chinese characters
+        greeting5 = "你好"
+        instance_config5 = {
+            "greeting": greeting5,
+            "snake_case_config": "hisss",
+            "camelCaseConfig": "spit!",
+        }
+        instance5 = client.use(package.handle, config=instance_config5)
+        assert instance5.invoke("greet") == f"{greeting5}, Person"
+        assert instance5.id != ""  # instance4.id
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_package_error_visibility.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_package_error_visibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from assets.packages.demo_package import TestPackage
 
-ERROR_NO_METHOD = "No handler for POST /method_doesnt_exist available."
+ERROR_NO_METHOD = "No handler for POST method_doesnt_exist available."
 ERROR_STEAMSHIP_ERROR = "[ERROR - POST raise_steamship_error] raise_steamship_error"
 ERROR_PYTHON_ERROR = "[ERROR - POST raise_python_error] raise_python_error"
 
 
 @pytest.mark.parametrize("invocable_handler", [TestPackage], indirect=True)
 def test_instance_invoke_unit(invocable_handler):
     """Test that the handler returns the proper errors"""
```

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_package_instance.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_package_instance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 import json
 import re
 
 import pytest
 import requests
+from assets.packages.demo_package import TestPackage
+from requests import ConnectTimeout
 from steamship_tests import PACKAGES_PATH, TEST_ASSETS_PATH
 from steamship_tests.utils.deployables import deploy_package
 from steamship_tests.utils.fixtures import get_steamship_client
 
 from steamship import PackageInstance, SteamshipError, Task, Workspace
 from steamship.base import TaskState
 from steamship.base.mime_types import MimeTypes
@@ -38,42 +40,55 @@
     with deploy_package(client, demo_package_path) as (package, version, instance):
         # Now let's invoke it!
         # Note: we're invoking the data at demo_package.py in the tests/assets/packages folder
 
         def get_raw(path: str):
             return requests.get(
                 instance.full_url_for(path),
-                headers={"authorization": f"Bearer {client.config.api_key}"},
+                headers={"authorization": f"Bearer {client.config.api_key.get_secret_value()}"},
             )
 
         res = instance.invoke("greet", verb=Verb.GET)
         assert res == "Hello, Person!"
 
         resp = get_raw("greet")
         assert resp.text == "Hello, Person!"
 
         res = instance.invoke("greet", verb=Verb.GET, name="Ted")
         assert res == "Hello, Ted!"
         url = instance.full_url_for("greet?name=Ted")
-        resp = requests.get(url, headers={"authorization": f"Bearer {client.config.api_key}"})
+        resp = requests.get(
+            url, headers={"authorization": f"Bearer {client.config.api_key.get_secret_value()}"}
+        )
         assert resp.text == "Hello, Ted!"
 
+        # res = instance.invoke("greet", verb=Verb.GET, name="Ted with spaces")
+        # assert res == "Hello, Ted!"
+        # url = instance.full_url_for("greet?name=Ted")
+        # resp = requests.get(
+        #     url, headers={"authorization": f"Bearer {client.config.api_key.get_secret_value()}"}
+        # )
+        # assert resp.text == "Hello, Ted with spaces!"
+        # Actually returns: 'Hello, Ted+with+spaces!'
+
         res = instance.invoke("greet", verb=Verb.POST)
         assert res == "Hello, Person!"
         url = instance.full_url_for("greet")
-        resp = requests.post(url, headers={"authorization": f"Bearer {client.config.api_key}"})
+        resp = requests.post(
+            url, headers={"authorization": f"Bearer {client.config.api_key.get_secret_value()}"}
+        )
         assert resp.text == "Hello, Person!"
 
         res = instance.invoke("greet", verb=Verb.POST, name="Ted")
         assert res == "Hello, Ted!"
         url = instance.full_url_for("greet")
         resp = requests.post(
             url,
             json={"name": "Ted"},
-            headers={"authorization": f"Bearer {client.config.api_key}"},
+            headers={"authorization": f"Bearer {client.config.api_key.get_secret_value()}"},
         )
         assert resp.text == "Hello, Ted!"
 
         # Now we test different return types
         resp_string = get_raw("resp_string")
         assert resp_string.text == "A String"
 
@@ -117,15 +132,15 @@
         my_api_base = _fix_url(client.config.api_base)
         remote_api_base = _fix_url(configuration_within_lambda["apiBase"])
 
         assert my_app_base == remote_app_base
         assert my_api_base == remote_api_base
 
         # API key should NOT be the same as the original, because the invocable should be given a workspace-scoped key
-        assert configuration_within_lambda["apiKey"] != client.config.api_key
+        assert configuration_within_lambda["apiKey"] != client.config.api_key.get_secret_value()
 
         # WorkspaceId is an exception. Rather than being the WorkspaceId of the client, it should be the WorkspaceId
         # of the App Instance.
         assert configuration_within_lambda["workspaceId"] == instance.workspace_id  # WorkspaceID
 
         # The test invocable should NOT be able to fetch the User's account info.
         with pytest.raises(SteamshipError) as excinfo:
@@ -219,19 +234,36 @@
 
     workspace = Workspace.create(steamship)
     steamship.switch_workspace(workspace_id=workspace.id)
 
     assert workspace.handle != "default"
 
     with deploy_package(steamship, demo_package_path) as (package, version, instance):
-
         assert instance.package_handle == package.handle
         assert instance.package_version_handle == version.handle
 
         got_instance = PackageInstance.get(steamship, instance.handle)
 
         assert got_instance.package_handle == package.handle
         assert got_instance.package_version_handle == version.handle
 
         use_instance = steamship.use(package_handle=package.handle, version=version.handle)
         assert use_instance.package_handle == package.handle
         assert use_instance.package_version_handle == version.handle
+
+
+def test_package_invoke_timeout():
+    client = get_steamship_client()
+    demo_package_path = PACKAGES_PATH / "demo_package.py"
+
+    with client.temporary_workspace() as client:
+        with deploy_package(client, demo_package_path) as (_, _, instance):
+            with pytest.raises(ConnectTimeout):
+                _ = instance.invoke("greet", verb=Verb.GET, timeout_s=0.001)
+            with pytest.raises(ConnectTimeout):
+                _ = instance.invoke("greet", verb=Verb.POST, timeout_s=0.001)
+
+
+def test_package_spec_sdk_version():
+    test_package = TestPackage()
+    spec = test_package.__steamship_dir__()
+    assert spec["sdkVersion"] is not None
```

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_returns_list.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_returns_list.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_signed_url_package.py` & `steamship-2.7.17/tests/steamship_tests/app/integration/test_signed_url_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/app/integration/test_use_package.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_use_plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 import pytest
-from steamship_tests import PACKAGES_PATH
-from steamship_tests.utils.client import steamship_use
-from steamship_tests.utils.deployables import deploy_package
+from steamship_tests import PLUGINS_PATH
+from steamship_tests.utils.client import steamship_use_plugin
+from steamship_tests.utils.deployables import deploy_plugin
 from steamship_tests.utils.fixtures import get_steamship_client
 from steamship_tests.utils.random import random_name
 
 from steamship import SteamshipError
 
 
-def test_use_package():
+def test_use_plugin():
     client = get_steamship_client()
-    demo_package_path = PACKAGES_PATH / "demo_package.py"
 
-    with deploy_package(client, demo_package_path) as (package, version, instance):
-        # Test for infinite recursion bug
-        assert package.__repr__()
-
-        # Now let's invoke it!
-        # Note: we're invoking the data at demo_package.py in the tests/assets/packages folder
-        package_handle_1 = random_name()
-        package_handle_2 = random_name()
+    plugin_handle_1 = random_name()
+    plugin_handle_2 = random_name()
+
+    blockifier_path = PLUGINS_PATH / "blockifiers" / "blockifier.py"
+    with deploy_plugin(client, blockifier_path, "blockifier") as (
+        plugin,
+        version,
+        instance,
+    ):
+        plugin_handle = plugin.handle
 
         # Test that without specifying an instance handle, the user is delivered into a workspace called
-        # packageHandle-default and delivered an instance called workspaceHandle-default
+        # pluginHandle-default and delivered an instance called pluginHandle-default
         #
         # These are the same semantics as workspaces: if you don't specify, you get taken to a `default` space,
         # but in this case we need to prefix with the type to avoid namespace collision within the space.
-        with steamship_use(package.handle) as static_use_instance1:
-            with steamship_use(package.handle, delete_workspace=False) as static_use_instance2:
+        with steamship_use_plugin(plugin_handle) as static_use_instance1:
+            with steamship_use_plugin(
+                plugin_handle, delete_workspace=False
+            ) as static_use_instance2:
                 assert (
                     static_use_instance1.client.config.workspace_handle
                     == static_use_instance2.client.config.workspace_handle
                 )
                 assert static_use_instance1.handle == static_use_instance2.handle
-                assert static_use_instance1.client.config.workspace_handle == package.handle
-                assert static_use_instance1.handle == package.handle
+                assert static_use_instance1.client.config.workspace_handle == plugin.handle
+                assert static_use_instance1.handle == plugin.handle
 
-        with steamship_use(package.handle, package_handle_1) as static_use_instance1:
-            with steamship_use(package.handle, package_handle_2) as static_use_instance2:
+        with steamship_use_plugin(plugin_handle, plugin_handle_1) as static_use_instance1:
+            with steamship_use_plugin(plugin_handle, plugin_handle_2) as static_use_instance2:
                 # Instance 1 and 2 have handles equal to their workspace handles
                 assert (
                     static_use_instance1.client.config.workspace_handle
                     == static_use_instance1.handle
                 )
                 assert (
                     static_use_instance1.client.config.workspace_id
@@ -63,20 +66,20 @@
                 # And neither one of these is the default workspace
                 assert static_use_instance1.workspace_id != client.config.workspace_id
                 assert static_use_instance2.workspace_id != client.config.workspace_id
                 assert static_use_instance1.client.config.workspace_handle != "default"
                 assert static_use_instance2.client.config.workspace_handle != "default"
 
                 # And they are in the requested workspaces
-                assert static_use_instance1.client.config.workspace_handle == package_handle_1
-                assert static_use_instance2.client.config.workspace_handle == package_handle_2
+                assert static_use_instance1.client.config.workspace_handle == plugin_handle_1
+                assert static_use_instance2.client.config.workspace_handle == plugin_handle_2
 
             # We can also bring up a second instance of the same invocable
-            with steamship_use(
-                package.handle, package_handle_1, delete_workspace=False
+            with steamship_use_plugin(
+                plugin_handle, plugin_handle_1, delete_workspace=False
             ) as static_use_instance1a:
                 assert (
                     static_use_instance1a.client.config.workspace_handle
                     == static_use_instance1a.handle
                 )
                 assert (
                     static_use_instance1a.client.config.workspace_id
@@ -87,21 +90,21 @@
                 assert (
                     static_use_instance1a.handle == static_use_instance1.handle
                 )  # It's the same instance (handle)
                 assert (
                     static_use_instance1a.id == static_use_instance1.id
                 )  # It's the same instance (id)
 
-            # Or we could have (1) created a client anchored to the Workspace `package_handle_1` and then
+            # Or we could have (1) created a client anchored to the Workspace `plugin_handle_1` and then
             # (2) Loaded that handle from within the client.
-            client2 = get_steamship_client(workspace_handle=package_handle_1)
-            assert client2.config.workspace_handle == package_handle_1
+            client2 = get_steamship_client(workspace_handle=plugin_handle_1)
+            assert client2.config.workspace_handle == plugin_handle_1
             assert client2.config.workspace_id == static_use_instance1.workspace_id
 
-            static_use_instance1a = client2.use(package.handle, package_handle_1)
+            static_use_instance1a = client2.use_plugin(plugin_handle, plugin_handle_1)
             assert (
                 static_use_instance1a.client.config.workspace_handle == static_use_instance1a.handle
             )  # The client is in the same workspace (handle)!
             assert (
                 static_use_instance1a.client.config.workspace_id
                 == static_use_instance1a.workspace_id
             )  # The client is in the same workspace (id)!
@@ -119,36 +122,88 @@
             # And here's the potentially hazardous thing that's possible:
             # You can use a client's member function `use` to create a second instance of that package that shares the
             # same workspace as the first, meaning it implicitly shares data.
             #
             # This is potentially useful, so it's not clear we want to forbid it (e.g. package1 could tag data, and
             # package2 could query data). But we want to encourage `Steamship.use` over `client.use` for basic use
             # due to the easier to understand scope semantics.
-            package_handle_1b = random_name()
-            static_use_instance1b = client2.use(package.handle, package_handle_1b)
+            plugin_handle_1b = random_name()
+            static_use_instance1b = client2.use_plugin(plugin_handle, plugin_handle_1b)
             assert (
                 static_use_instance1b.client.config.workspace_handle == static_use_instance1.handle
             )
             assert (
                 static_use_instance1b.client.config.workspace_id
                 == static_use_instance1.workspace_id
             )
             assert static_use_instance1b.workspace_id == static_use_instance1.workspace_id
             # But the handle isn't the same
             assert static_use_instance1b.handle != static_use_instance1.handle
             assert static_use_instance1b.id != static_use_instance1.id
 
 
-def test_use_package_fails_with_same_instance_name_but_different_package_name():
+def test_use_plugin_fails_with_same_instance_name_but_different_plugin_name():
     client = get_steamship_client()
 
     instance_handle = random_name()
 
-    demo_package_path = PACKAGES_PATH / "demo_package.py"
-
-    with deploy_package(client, demo_package_path) as (app, version, instance):
-        with deploy_package(client, demo_package_path) as (app2, version2, instance2):
-            client.use(app.handle, instance_handle)
+    blockifier_path = PLUGINS_PATH / "blockifiers" / "blockifier.py"
+    with deploy_plugin(client, blockifier_path, "blockifier") as (
+        plugin,
+        version,
+        instance,
+    ):
+        with deploy_plugin(client, blockifier_path, "blockifier") as (
+            plugin2,
+            version2,
+            instance2,
+        ):
+            client.use_plugin(plugin.handle, instance_handle)
 
             # Should fail because we're using the shortcut `import_plugin` method with the same instance
             with pytest.raises(SteamshipError):
-                client.use(app2.handle, instance_handle)
+                client.use_plugin(plugin2.handle, instance_handle)
+
+
+def test_use_plugin_fails_with_same_instance_name_but_different_config_unless_anon():
+    client = get_steamship_client()
+    csv_blockifier_plugin_path = PLUGINS_PATH / "blockifiers" / "csv_blockifier.py"
+
+    version_config_template = {
+        "text_column": {"type": "string"},
+        "tag_columns": {"type": "string"},
+        "tag_kind": {"type": "string"},
+    }
+    instance_config = {  # Has to match up
+        "text_column": "Message",
+        "tag_columns": "Category",
+        "tag_kind": "Intent",
+    }
+    instance_config_2 = {  # Has to match up
+        "text_column": "Message",
+        "tag_columns": "Category",
+        "tag_kind": "Other Thing",
+    }
+
+    with deploy_plugin(
+        client,
+        csv_blockifier_plugin_path,
+        "blockifier",
+        version_config_template=version_config_template,
+        instance_config=instance_config,
+    ) as (plugin, version, instance):
+        # This should work
+        instance_2 = client.use_plugin(plugin.handle, instance.handle, config=instance_config)
+        assert instance_2.handle == instance.handle
+
+        # This should fail because config changed
+        with pytest.raises(SteamshipError):
+            client.use_plugin(plugin.handle, instance.handle, config=instance_config_2)
+
+        # This succeeds because the name includes the hash of the config
+        instance_3 = client.use_plugin(plugin.handle, config=instance_config)
+        assert instance_3.handle != plugin.handle
+
+        # This succeeds because the name includes the hash of the config
+        instance_4 = client.use_plugin(plugin.handle, config=instance_config_2)
+        assert instance_4.handle != plugin.handle
+        assert instance_4.handle != instance_3.handle
```

### Comparing `steamship-2.3.9/tests/steamship_tests/app/unit/test_config_template_extraction.py` & `steamship-2.7.17/tests/steamship_tests/app/unit/test_config_template_extraction.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/app/unit/test_demo_app_spec.py` & `steamship-2.7.17/tests/steamship_tests/app/unit/test_demo_app_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,40 +10,43 @@
 @pytest.mark.parametrize("invocable_handler", [TestPackage], indirect=True)
 def test_package_spec(invocable_handler: Callable[[str, str, Optional[dict]], dict]):
     """Test that the handler returns the proper directory information"""
     rd = invocable_handler("GET", "/__dir__", {}).get("data")
 
     assert rd.get("doc") is None
     assert rd.get("methods") is not None
-    assert len(rd.get("methods")) == 18
+    assert len(rd.get("methods")) == 23
 
     saw_public = False
 
     for method in rd.get("methods"):
         if method.get("path") == "/greet" and method.get("verb") == "GET":
             assert method.get("config") is not None
             assert method.get("config").get("public") is True
             assert method.get("config").get("timeout") == 10
             assert method.get("config").get("identifier") == "foo"
             assert method.get("config").get("body") == 98.6
             assert method.get("config").get("not_there") is None
 
             saw_public = True
+        elif "public" in method.get("path"):
+            assert method.get("config") is not None
+            assert method.get("config").get("public") is True
         else:
-            assert method.get("config") == {}
+            assert (method.get("config") == {}) or (method.get("config") is None)
 
     assert saw_public
 
 
 @pytest.mark.parametrize("invocable_handler", [FancyTypes], indirect=True)
 def test_package_spec_fancy_types(invocable_handler: Callable[[str, str, Optional[dict]], dict]):
     """Test that the handler returns the proper directory information"""
     rd = invocable_handler("GET", "/__dir__", {}).get("data")
 
-    assert len(rd.get("methods")) == 2
+    assert len(rd.get("methods")) == 5
     for method in rd.get("methods"):
         if method.get("path") == "/enum_route":
             values = method.get("args")[0].get("values")
             assert values is not None
             assert len(values) == 2
             assert values[0] == "value1"
             assert values[1] == "value2"
@@ -60,24 +63,32 @@
     invocable_handler: Callable[[str, str, Optional[dict]], dict]
 ):
     """Test that the handler returns the proper directory information, even for a configuration-required invocable."""
     rd = invocable_handler("GET", "/__dir__", {}).get("data")
 
     assert rd.get("doc") is None
     assert rd.get("methods") is not None
-    assert len(rd.get("methods")) == 4
+    assert len(rd.get("methods")) == 7
 
 
 @pytest.mark.parametrize("invocable_handler", [OptionalParams], indirect=True)
 def test_package_spec_optional_params(
     invocable_handler: Callable[[str, str, Optional[dict]], dict]
 ):
     """Test that the handler returns the proper directory information"""
     rd = invocable_handler("GET", "/__dir__", {}).get("data")
 
-    assert len(rd.get("methods")) == 1
-    method = rd.get("methods")[0]
+    assert len(rd.get("methods")) == 4
+    method = None
+    for a_method in rd.get("methods"):
+        if a_method.get("path") not in ["/__dir__", "/__instance_init__"]:
+            method = a_method
+            break
+
+    assert method is not None
+    assert len(method.get("args")) > 0
+
     values = method.get("args")[0].get("values")
     assert values is not None
     assert len(values) == 2
     assert values[0] == "value1"
     assert values[1] == "value2"
```

### Comparing `steamship-2.3.9/tests/steamship_tests/app/unit/test_response.py` & `steamship-2.7.17/tests/steamship_tests/app/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/base/test_binary_utils.py` & `steamship-2.7.17/tests/steamship_tests/base/test_binary_utils.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/base/test_configuration.py` & `steamship-2.7.17/tests/steamship_tests/base/test_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import webbrowser
 from unittest import mock
 
 import pytest
 from pydantic import ValidationError
 
 from steamship import Configuration, SteamshipError
 from steamship.base.configuration import DEFAULT_API_BASE, DEFAULT_APP_BASE, DEFAULT_WEB_BASE
@@ -47,10 +48,15 @@
     assert configuration.web_base is not None
     assert configuration.app_base is not None
     assert configuration.api_base is not None
 
 
 @mock.patch.dict(os.environ, {"STEAMSHIP_API_KEY": ""})
 def test_empty_api_key() -> None:
-    with pytest.raises(SteamshipError):
-        # Note: We're referencing a non existing profile to make sure the api key is not loaded from the default profile in steamship.json
-        Configuration(api_key=None, profile="non-existing-profile")
+
+    # Only run this test on non-local (i.e., CI/CD) otherwise will attempt browser login
+    try:
+        _ = webbrowser.get()
+    except webbrowser.Error:
+        with pytest.raises(SteamshipError):
+            # Note: We're referencing a non existing profile to make sure the api key is not loaded from the default profile in steamship.json
+            Configuration(api_key=None, profile="non-existing-profile")
```

### Comparing `steamship-2.3.9/tests/steamship_tests/base/test_serialization.py` & `steamship-2.7.17/tests/steamship_tests/base/test_serialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 def test_serialize_client_to_json_works(client: Steamship):
     assert "use" not in client.dict().keys()
     assert "use_plugin" not in client.dict().keys()
 
     j = json.dumps(client.dict())  # this will fail if `use` or `use_plugin` are output by dict()
     assert j is not None
 
+    j = json.dumps(
+        client.dict(exclude={"foo"})
+    )  # this will fail if `use` or `use_plugin` are output by dict()
+    assert j is not None
+
+    j = json.dumps(
+        client.dict(exclude={"foo": True})
+    )  # this will fail if `use` or `use_plugin` are output by dict()
+    assert j is not None
+
 
 @pytest.mark.usefixtures("client")
 def test_serialize_many_models(client: Steamship):
     json.dumps(Block(client=client).dict())
     json.dumps(Block(client=client, tags=[Tag(client=client)]).dict())
     json.dumps(Tag(client=client).dict())
     json.dumps(File(client=client).dict())
```

### Comparing `steamship-2.3.9/tests/steamship_tests/base/test_steamship_error_serializable.py` & `steamship-2.7.17/tests/steamship_tests/base/test_steamship_error_serializable.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/base/test_task.py` & `steamship-2.7.17/tests/steamship_tests/base/test_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+import pytest
 from steamship_tests.utils.fixtures import get_steamship_client
 
+from steamship import SteamshipError
 from steamship.base.model import CamelModel
 from steamship.base.tasks import TaskState
 
 
 class NoOpResult(CamelModel):
     pass
 
@@ -26,14 +28,40 @@
     assert result_2_task is not None
     assert result_2_task.state == TaskState.waiting
 
     result_2_task.wait()
 
     # And now it has completed
     assert result_2_task.state == TaskState.succeeded
+    assert result_2_task.output is not None
+    assert type(result_2_task.output) == NoOpResult
+
+
+def test_task_wait_milliseconds():
+    client = get_steamship_client()
+
+    # Can't wait a negative amount
+    with pytest.raises(SteamshipError):
+        result_task_1 = client.post("task/noop", expect=NoOpResult, task_delay_ms=-43)
+
+    # No wait is no wait
+    result_task_1 = client.post("task/noop", expect=NoOpResult, task_delay_ms=0)
+
+    assert result_task_1 is not None
+    assert type(result_task_1) == NoOpResult
+
+    # When we background it, we get a task back instead
+    result_2_task = client.post("task/noop", expect=NoOpResult, task_delay_ms=1000)
+    assert result_2_task is not None
+    assert result_2_task.state == TaskState.waiting
+
+    result_2_task.wait()
+
+    # And now it has completed
+    assert result_2_task.state == TaskState.succeeded
     assert result_2_task.output is not None
     assert type(result_2_task.output) == NoOpResult
 
 
 def test_task_update():
     client = get_steamship_client()
```

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_blockify.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_blockify.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_classify.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_classify.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_convert_ocr.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_convert_ocr.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_embed.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_embed.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_embed_file.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_embed_file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_tag.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_tag.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/operations/test_tag_file.py` & `steamship-2.7.17/tests/steamship_tests/client/operations/test_tag_file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/test_client.py` & `steamship-2.7.17/tests/steamship_tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/client/test_task_dependencies.py` & `steamship-2.7.17/tests/steamship_tests/client/test_task_dependencies.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,36 @@
     )
     assert response is not None
     assert response.state == TaskState.waiting
     assert response.task_id is not None
     return response
 
 
+def test_task_wait_callback():
+    """Test basic connection"""
+    client = get_steamship_client()
+
+    task1 = schedule_task(client)
+
+    retries_checked = 0
+
+    def on_task_check(retry_number, total_sec, task):
+        nonlocal retries_checked
+        retries_checked = retries_checked + 1
+        assert retry_number
+        assert retry_number > 0
+        assert total_sec
+        assert total_sec > 0
+        assert task.task_id == task1.task_id
+
+    task1.wait(on_each_refresh=on_task_check)
+    assert retries_checked > 0
+    assert task1.state == TaskState.succeeded
+
+
 def test_task_dependencies_parallel_success():
     """Test basic connection"""
     client = get_steamship_client()
 
     task1 = schedule_task(client)
     task2 = schedule_task(client)
     task3 = schedule_task(client, dependencies=[task1, task2])
@@ -41,17 +63,25 @@
 
 def test_task_dependencies_parallel_failure():
     """Test basic connection"""
     client = get_steamship_client()
 
     task1 = schedule_task(client)
     task2 = schedule_task(client, please_fail=True)
-    task3 = schedule_task(client, dependencies=[task1, task2])
+
+    because_of_engine_timing_task2_already_failed = False
+
+    try:
+        task3 = schedule_task(client, dependencies=[task1, task2])
+    except SteamshipError as e:
+        assert "At least one dependent already failed" in e.message  # noqa: PT017
+        because_of_engine_timing_task2_already_failed = True
 
     task1.wait()
     assert task1.state == TaskState.succeeded
 
     with pytest.raises(SteamshipError):
         task2.wait()  # It failed!
 
-    with pytest.raises(SteamshipError):
-        task3.wait()  # It failed too -- because of the rollup!
+    if not because_of_engine_timing_task2_already_failed:
+        with pytest.raises(SteamshipError):
+            task3.wait()  # It failed too -- because of the rollup!
```

### Comparing `steamship-2.3.9/tests/steamship_tests/data/tags/test_file_tags.py` & `steamship-2.7.17/tests/steamship_tests/data/tags/test_file_tags.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/data/test_file.py` & `steamship-2.7.17/tests/steamship_tests/data/test_block.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,224 +1,241 @@
-import json
-
 import pytest
-from steamship_tests import PLUGINS_PATH
-from steamship_tests.utils.deployables import deploy_plugin
+import requests
+from steamship_tests import TEST_ASSETS_PATH
 
-from steamship import MimeTypes, SteamshipError
+from steamship import MimeTypes
 from steamship.client import Steamship
+from steamship.data import TagKind
 from steamship.data.block import Block
 from steamship.data.file import File
 from steamship.data.tags.tag import Tag
 
 
 @pytest.mark.usefixtures("client")
-def test_file_upload(client: Steamship):
-    a = File.create(client=client, handle="foo", content="A", mime_type=MimeTypes.MKD)
+def test_query(client: Steamship):
+    a = File.create(
+        client=client,
+        blocks=[
+            Block(text="A", tags=[Tag(kind="BlockTag")]),
+            Block(text="B"),
+        ],
+    )
     assert a.id is not None
-    assert a.mime_type == MimeTypes.MKD
-    assert a.handle == "foo"
-
-    b = File.create(client=client, content="B", mime_type=MimeTypes.TXT)
+    a = a.refresh()
+    b = File.create(
+        client=client,
+        blocks=[
+            Block(text="A"),
+            Block(text="B", tags=[Tag(kind="Test")]),
+        ],
+        tags=[Tag(kind="FileTag")],
+    )
     assert b.id is not None
-    assert b.mime_type == MimeTypes.TXT
+    b = b.refresh()
 
-    assert a.id != b.id
+    blocks = Block.query(client=client, tag_filter_query='blocktag and kind "BlockTag"').blocks
+    assert len(blocks) == 1
+    assert blocks[0].id == a.blocks[0].id
+
+    blocks = Block.query(client=client, tag_filter_query='blocktag and kind "Test"').blocks
+    assert len(blocks) == 1
+    assert blocks[0].id == b.blocks[1].id
 
-    assert a.raw().decode("utf-8") == "A"
     a.delete()
     b.delete()
 
 
 @pytest.mark.usefixtures("client")
-def test_only_blocks_or_content(client: Steamship):
-    with pytest.raises(SteamshipError):
-        _ = File.create(client=client, content="A", blocks=[], mime_type=MimeTypes.MKD)
+def test_append_indices(client: Steamship):
+    file = File.create(client, blocks=[Block(text="first")])
+    assert len(file.blocks) == 1
+    assert file.blocks[0].index_in_file == 0
+
+    appended_block = Block.create(client, file_id=file.id, text="second")
+    assert appended_block.index_in_file == 1
+
+    file.refresh()
+    assert len(file.blocks) == 2
+    assert file.blocks[0].index_in_file == 0
+    assert file.blocks[0].text == "first"
+    assert file.blocks[1].index_in_file == 1
+    assert file.blocks[1].text == "second"
 
 
 @pytest.mark.usefixtures("client")
-def test_file_upload_with_content_and_tags(client: Steamship):
-    a = File.create(
-        client=client,
-        content="ABC",
-        mime_type=MimeTypes.MKD,
-        tags=[Tag(kind="SomeKind")],
+def test_append_block_url(client: Steamship):
+    file = File.create(client, blocks=[])
+
+    appended_block = Block.create(
+        client, file_id=file.id, url="https://docs.steamship.com/_static/Steamship-symbol-dark.png"
     )
-    assert a.id is not None
-    assert a.mime_type == MimeTypes.MKD
-    assert len(a.tags) == 1
-    assert a.tags[0].file_id == a.id
-    assert a.tags[0].kind == "SomeKind"
-    assert a.raw().decode("utf-8") == "ABC"
-
-
-def test_file_import_response_dict():
-    resp = File.CreateResponse(_bytes=b"some bytes", mime_type=MimeTypes.BINARY)
-    to_dict = resp.dict(include={"data_", "mime_type"})
-    file_create_response = File.CreateResponse.parse_obj(to_dict)
-    assert resp.data_ == file_create_response.data_
-    assert resp.mime_type == file_create_response.mime_type
-
-
-def test_file_import_response_bytes_serialization():
-    file_resp = File.CreateResponse(_bytes=b"some bytes", mime_type=MimeTypes.BINARY)
-    to_dict = file_resp.dict()
-    as_json_string = json.dumps(to_dict)
-    as_dict_again = json.loads(as_json_string)
-    assert as_dict_again == to_dict
 
+    assert appended_block.text == ""
+    file.refresh()
+    assert len(file.blocks) == 1
+    assert file.blocks[0].mime_type == MimeTypes.PNG
 
-def test_file_upload_with_blocks(client: Steamship):
-    a = File.create(
-        client=client,
-        blocks=[
-            Block(text="A", tags=[Tag(kind="BlockTag")]),
-            Block(text="B", tags=[Tag(kind="BlockTag")]),
-        ],
-    )
-    assert a.id is not None
+    block_content = file.blocks[0].raw()
+    assert len(block_content) == 20693
+    assert not file.blocks[0].is_text()
 
-    query_result = Block.query(client, f'file_id "{a.id}"')
 
-    def check_blocks(block_list):
-        assert len(block_list) == 2
-        assert block_list[0].tags is not None
-        assert len(block_list[0].tags) == 1
-        assert block_list[0].tags[0].kind == "BlockTag"
-        assert block_list[0].text == "A"
-
-    assert query_result.blocks is not None
-    check_blocks(query_result.blocks)
-
-    # Let's get the file fresh
-    aa = File.get(client, _id=a.id)
-    check_blocks(aa.blocks)
-    a.delete()
+@pytest.mark.usefixtures("client")
+def test_text_mime_type(client: Steamship):
+    file = File.create(client, blocks=[Block(text="first")])
+    _ = Block.create(client, file_id=file.id, text="second")
+    file.refresh()
+    assert len(file.blocks) == 2
+    for block in file.blocks:
+        assert block.mime_type == MimeTypes.TXT
+        assert block.is_text()
 
 
-def test_file_upload_with_blocks_and_tags(client: Steamship):
-    a = File.create(
-        client=client,
-        blocks=[
-            Block(text="A", tags=[Tag(kind="BlockTag")]),
-            Block(text="B", tags=[Tag(kind="BlockTag")]),
-        ],
-        tags=[Tag(kind="FileTag")],
-    )
-    assert a.id is not None
+@pytest.mark.usefixtures("client")
+def test_append_block_content_text(client: Steamship):
+    file = File.create(client, blocks=[])
 
-    blocks = Block.query(client, f'file_id "{a.id}"')
+    appended_block = Block.create(client, file_id=file.id, content=bytes("This is a test", "utf-8"))
 
-    def check_blocks(block_list):
-        assert len(block_list) == 2
-        assert block_list[0].tags is not None
-        assert len(block_list[0].tags) == 1
-        assert block_list[0].tags[0].kind == "BlockTag"
-        assert block_list[0].text == "A"
-
-    assert blocks.blocks is not None
-    check_blocks(blocks.blocks)
-
-    # Let's get the file fresh
-    aa = File.get(client, _id=a.id)
-    check_blocks(aa.blocks)
-    assert aa.tags is not None
-    assert len(aa.tags) == 1
-    assert aa.tags[0].kind == "FileTag"
+    assert appended_block.text == "This is a test"
+    file.refresh()
+    assert len(file.blocks) == 1
+    assert file.blocks[0].mime_type == MimeTypes.TXT
 
-    a.delete()
+    assert file.blocks[0].is_text()
 
 
-def test_file_upload_with_tags(client: Steamship):
-    a = File.create(
-        client=client,
-        tags=[Tag(kind="FileTag")],
+@pytest.mark.usefixtures("client")
+def test_append_block_content_image(client: Steamship):
+    file = File.create(client, blocks=[])
+
+    palm_tree_path = TEST_ASSETS_PATH / "palm_tree.png"
+    with palm_tree_path.open("rb") as f:
+        palm_bytes = f.read()
+
+    appended_block = Block.create(
+        client, file_id=file.id, content=palm_bytes, mime_type=MimeTypes.PNG
     )
-    assert a.id is not None
 
-    query_result = Tag.query(client, f'filetag and file_id "{a.id}"')
+    assert appended_block.text == ""
+    file.refresh()
+    assert len(file.blocks) == 1
+    assert file.blocks[0].mime_type == MimeTypes.PNG
 
-    def check_tags(file_tag_list):
-        assert len(file_tag_list) == 1
-        assert file_tag_list[0] is not None
-        assert file_tag_list[0].kind == "FileTag"
-
-    assert query_result.tags is not None
-    check_tags(query_result.tags)
-
-    # Let's get the file fresh
-    aa = File.get(client, _id=a.id)
-    check_tags(aa.tags)
+    assert not file.blocks[0].is_text()
 
-    a.delete()
+    raw_content = file.blocks[0].raw()
+    assert raw_content == palm_bytes
 
 
-def test_query(client: Steamship):
-    a = File.create(
-        client=client,
-        blocks=[
-            Block(text="A", tags=[Tag(kind="BlockTag")]),
-            Block(text="B"),
-        ],
-    )
-    assert a.id is not None
-    b = File.create(
-        client=client,
-        blocks=[Block(text="A"), Block(text="B")],
-        tags=[Tag(kind="FileTag")],
+@pytest.mark.usefixtures("client")
+def test_append_with_tag(client: Steamship):
+    file = File.create(client, blocks=[Block(text="first", tags=[Tag(kind=TagKind.DOCUMENT)])])
+    assert len(file.blocks) == 1
+    assert file.blocks[0].index_in_file == 0
+
+    appended_block = Block.create(
+        client, file_id=file.id, text="second", tags=[Tag(kind=TagKind.DOCUMENT)]
+    )
+    assert appended_block.index_in_file == 1
+
+    file.refresh()
+    assert len(file.blocks) == 2
+    assert file.blocks[0].index_in_file == 0
+    assert file.blocks[0].text == "first"
+    assert file.blocks[1].index_in_file == 1
+    assert file.blocks[1].text == "second"
+
+    assert len(file.blocks[1].tags) == 1
+    assert file.blocks[1].tags[0].kind == TagKind.DOCUMENT
+
+
+@pytest.mark.usefixtures("client")
+def test_create_with_tags(client: Steamship):
+    file = File.create(client, content="empty")
+    new_block = Block.create(
+        client,
+        file_id=file.id,
+        text="foo",
+        tags=[Tag(kind="bar", name="foo"), Tag(kind="baz", name="foo")],
     )
-    assert b.id is not None
+    assert len(new_block.tags) == 2
 
-    files = File.query(client=client, tag_filter_query='blocktag and kind "BlockTag"').files
-    assert len(files) == 1
-    assert files[0].id == a.id
-
-    files = File.query(client=client, tag_filter_query='filetag and kind "FileTag"').files
-    assert len(files) == 1
-    assert files[0].id == b.id
-
-    # Test serialization; This shouldn't throw
-    out_file = File.get(client, _id=b.id)
-    json.dumps(out_file.dict())
 
-    a.delete()
-    b.delete()
+@pytest.mark.usefixtures("client")
+def test_append_is_present(client: Steamship):
+    file = File.create(client, blocks=[Block(text="first")])
+    assert len(file.blocks) == 1
+
+    file.append_block(text="second")
+    assert len(file.blocks) == 2
+
+    file.refresh()
+    assert len(file.blocks) == 2
+
+    my_file = File.create(client, handle="my_file", content="")
+    assert len(my_file.blocks) == 0
+    my_file.append_block(text="first")
+    assert len(my_file.blocks) == 1
 
 
-def test_file_list(client: Steamship):
-    a = File.create(
-        client=client,
-        tags=[Tag(kind="FileTag")],
-    )
-    b = File.create(
-        client=client,
-        tags=[Tag(kind="FileTag")],
-    )
-    c = File.create(
-        client=client,
-        tags=[Tag(kind="FileTag")],
+@pytest.mark.usefixtures("client")
+def test_append_block_public_data(client: Steamship):
+    file = File.create(client, blocks=[])
+
+    appended_block = Block.create(
+        client, file_id=file.id, content=bytes("This is a test", "utf-8"), public_data=True
     )
+    assert appended_block.public_data
 
-    files = File.list(client=client).files
-    assert len(files) == 3
-    assert a in files
-    assert b in files
-    assert c in files
+    # Intentionally no API key
+    response = requests.get(appended_block.raw_data_url)
 
-    a.delete()
-    b.delete()
-    c.delete()
+    assert response.text == "This is a test"
+    assert response.headers["content-type"] == MimeTypes.TXT
+
+
+@pytest.mark.usefixtures("client")
+def test_append_block_private_data(client: Steamship):
+    file = File.create(client, blocks=[])
+
+    appended_block = Block.create(client, file_id=file.id, content=bytes("This is a test", "utf-8"))
+    assert not appended_block.public_data
 
+    # Intentionally no API key
+    failed_response = requests.get(appended_block.raw_data_url)
+    assert not failed_response.ok
 
-def test_file_refresh(client: Steamship):
-    blockifier_path = PLUGINS_PATH / "blockifiers" / "blockifier.py"
-    with deploy_plugin(client, blockifier_path, "blockifier") as (
-        plugin,
-        version,
-        instance,
-    ):
-        file = File.create(client=client, content="This is a test.")
-        assert len(file.blocks) == 0
-        file.blockify(plugin_instance=instance.handle).wait()
-        file.refresh()  # don't reassign file
-        assert len(file.blocks) == 4
-        file.delete()
+    # Should still be able to get with API key
+    response = requests.get(
+        appended_block.raw_data_url,
+        headers={"Authorization": f"Bearer {client.config.api_key.get_secret_value()}"},
+    )
+
+    assert response.text == "This is a test"
+    assert response.headers["content-type"] == MimeTypes.TXT
+
+
+@pytest.mark.usefixtures("client")
+def test_set_public_data(client: Steamship):
+    file = File.create(client, blocks=[])
+    block = Block.create(client, file_id=file.id, content=bytes("This is a test", "utf-8"))
+
+    assert not block.public_data
+
+    # With public data false, call should fail
+    # Intentionally no API key
+    failed_response = requests.get(block.raw_data_url)
+    assert not failed_response.ok
+
+    # With public data true, call should succeed
+    block.set_public_data(True)
+    # Intentionally no API key
+    response = requests.get(block.raw_data_url)
+    assert response.text == "This is a test"
+    assert response.headers["content-type"] == MimeTypes.TXT
+
+    # Setting back to false, should fail again
+    block.set_public_data(False)
+    # Intentionally no API key
+    failed_response = requests.get(block.raw_data_url)
+    assert not failed_response.ok
```

### Comparing `steamship-2.3.9/tests/steamship_tests/data/test_img.png` & `steamship-2.7.17/tests/steamship_tests/data/test_img.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/data/test_package_version.py` & `steamship-2.7.17/tests/steamship_tests/data/test_package_version.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/data/test_plugins.py` & `steamship-2.7.17/tests/steamship_tests/data/test_plugins.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import uuid
 
 import pytest
 from steamship_tests.utils.fixtures import get_steamship_client
 
 from steamship import PluginInstance, SteamshipError, Workspace
 from steamship.data.plugin import Plugin, PluginAdapterType, PluginType
+from steamship.data.user import User
 
 
 def test_plugin_create():
     steamship = get_steamship_client()
 
-    my_plugins = Plugin.list(steamship)
-    orig_count = len(my_plugins.plugins)
+    resp = Plugin.list(steamship)
+    prior_plugin_ids = [plugin.id for plugin in resp.plugins]
 
     plugin_args = {
         "client": steamship,
         "description": "This is just for test",
         "type_": PluginType.tagger,
         "transport": PluginAdapterType.steamship_docker,
         "is_public": True,
@@ -24,46 +25,44 @@
 
     required_fields = {"description", "type_"}
     for required_field in required_fields:
         del plugin_args[required_field]
         with pytest.raises(TypeError):
             Plugin.create(**plugin_args)
 
-    my_plugins = Plugin.list(steamship)
-    assert len(my_plugins.plugins) == orig_count
-
     plugin = Plugin.create(
         client=steamship,
         description="This is just for test",
         type_=PluginType.tagger,
         transport=PluginAdapterType.steamship_docker,
         is_public=False,
     )
-    my_plugins = Plugin.list(steamship)
-    assert len(my_plugins.plugins) == orig_count + 1
+
+    assert plugin.id not in prior_plugin_ids
+
+    resp = Plugin.list(steamship)
+    assert plugin.id in [
+        plugin.id for plugin in resp.plugins
+    ]  # newly-created plugin should be top of list
+    assert plugin.description in [plugin.description for plugin in resp.plugins]
+
+    user_id = User.current(steamship).id
+    assert plugin.user_id == user_id
 
     # No fetch_if_exists doesn't work
     with pytest.raises(SteamshipError):
         _ = Plugin.create(
             client=steamship,
             handle=plugin.handle,
             description="This is just for test",
             type_=PluginType.tagger,
             transport=PluginAdapterType.steamship_docker,
             is_public=False,
         )
 
-    my_plugins = Plugin.list(steamship)
-    assert len(my_plugins.plugins) == orig_count + 1
-
-    assert plugin.id in [plugin.id for plugin in my_plugins.plugins]
-    assert plugin.description in [plugin.description for plugin in my_plugins.plugins]
-
-    # assert(my_plugins.plugins[0].description != plugin.description)
-
 
 def test_plugin_public():
     steamship = get_steamship_client()
 
     resp = Plugin.list(steamship)
     assert resp.plugins is not None
     plugins = resp.plugins
@@ -85,14 +84,55 @@
     instance = PluginInstance.create(steamship, plugin_handle="test-tagger", handle=handle)
     assert instance.id is not None
 
     other_instance = PluginInstance.get(steamship, handle=handle)
     assert instance.id == other_instance.id
 
 
+def test_plugin_update():
+    steamship = get_steamship_client()
+
+    plugin = Plugin.create(
+        client=steamship,
+        description="This is just for test",
+        type_=PluginType.tagger,
+        transport=PluginAdapterType.steamship_docker,
+        is_public=False,
+    )
+
+    new_description = "f"
+    plugin.description = new_description
+
+    plugin = plugin.update(steamship)
+    assert plugin.description == new_description
+
+    got_plugin = Plugin.get(steamship, handle=plugin.handle)
+    assert got_plugin.description == new_description
+
+
+def test_plugin_delete():
+    steamship = get_steamship_client()
+
+    plugin = Plugin.create(
+        client=steamship,
+        description="This is just for test",
+        type_=PluginType.tagger,
+        transport=PluginAdapterType.steamship_docker,
+        is_public=False,
+    )
+
+    assert plugin is not None
+
+    plugin.delete()
+
+    # Validate plugin is gone
+    with pytest.raises(SteamshipError):
+        _ = Plugin.get(steamship, handle=plugin.handle)
+
+
 def test_plugin_instance_quick_create():
     steamship = get_steamship_client()
 
     handle = f"test_tagger_test_handle{uuid.uuid4()}"
     handle2 = f"test_tagger_test_handle{uuid.uuid4()}"
 
     p1 = steamship.use_plugin("test-tagger", handle)
```

### Comparing `steamship-2.3.9/tests/steamship_tests/data/test_task_comments.py` & `steamship-2.7.17/tests/steamship_tests/data/test_task_comments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import pytest
 from steamship_tests.utils.fixtures import get_steamship_client
 from steamship_tests.utils.random import random_index, random_name
 
-from steamship import Tag
+from steamship import SteamshipError, Tag
+from steamship.base.request import SortOrder
 from steamship.base.tasks import TaskComment
 from steamship.data.embeddings import EmbeddedItem
 
 _TEST_EMBEDDER = "test-embedder"
 
 
 def _list_equal(actual, expected):
@@ -49,15 +51,15 @@
         comments = TaskComment.list(client=steamship, task_id=res.task_id)
         assert len(comments.comments) == 0
 
         # Now let's add one
         res.add_comment(external_id="Foo1", external_type="Bar1", metadata=[1, 2, 3])
         res.add_comment(external_id="Foo2", external_type="Bar2", metadata=[1, 2, 3, 4])
 
-        comments = TaskComment.list(client=steamship, task_id=res.task_id)
+        comments = TaskComment.list(client=steamship, task_id=res.task_id, sort_order=SortOrder.ASC)
         assert len(comments.comments) == 2
         comment = comments.comments[0]
         assert comment.external_id == "Foo1"
         assert comment.external_type == "Bar1"
         _list_equal(comment.metadata, [1, 2, 3])
 
         comment = comments.comments[1]
@@ -79,14 +81,41 @@
         assert comment.external_type == "Bar"
         _list_equal(comment.metadata, {"value": [1, 2]})
         comments.comments[0].delete()
         comments = TaskComment.list(client=steamship, task_id=res.task_id)
         assert len(comments.comments) == 0
 
 
+def test_task_comment_list_paging():
+    steamship = get_steamship_client()
+    with random_index(steamship, _TEST_EMBEDDER) as index:
+        item1 = Tag(text="Pizza", name="pizza", kind="food", value={"value": [1, 2, 3]})
+        index.insert(item1)
+
+        res = index.search(item1.text, k=1)
+        res.wait()
+
+        res.add_comment(external_id="Foo1", external_type="Bar1", metadata=[1, 2, 3])
+        res.add_comment(external_id="Foo2", external_type="Bar2", metadata=[1, 2, 3, 4])
+        res.add_comment(external_id="Foo3", external_type="Bar3", metadata=[1, 2, 3, 4])
+
+        resp = TaskComment.list(client=steamship, task_id=res.task_id, page_size=2)
+        assert len(resp.comments) == 2
+        assert resp.next_page_token is not None
+
+        resp = TaskComment.list(
+            client=steamship, task_id=res.task_id, page_size=2, page_token=resp.next_page_token
+        )
+        assert len(resp.comments) == 1
+        assert resp.next_page_token is None
+
+        with pytest.raises(SteamshipError):
+            TaskComment.list(steamship, page_size=-1)
+
+
 def test_task_comment_feedback_reporting():
     """
     We want to be able to generate reports like this:
 
     Select Across Gorup    -- externalGroup
     Inputs Seen: XXX       -- Distinct externalId
     Inputs Suggested: YYY  -- Add to metadata
```

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
         instance2 = PluginInstance.create(
             client,
             plugin_id=plugin.id,
             plugin_version_id=version.id,
             config=instance_config2,
         )
+        instance2.wait_for_init()
         assert instance2 is not None
 
         res = instance2.tag(doc=test_doc)
         res.wait()
         assert res.output is not None
         assert len(res.output.file.blocks) == 1
         assert res.output.file.blocks[0].text == test_doc
```

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_embedder.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_skill.py` & `steamship-2.7.17/tests/steamship_tests/plugin/integration/test_use_skill.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_blockifier.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_config_block.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_config_block.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_file_importer.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_response_post_update.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_response_post_update.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_service.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/util.py` & `steamship-2.7.17/tests/steamship_tests/plugin/unit/trainable/util.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/server/test_package_local.py` & `steamship-2.7.17/tests/steamship_tests/server/test_package_local.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/server/test_task_timeout.py` & `steamship-2.7.17/tests/steamship_tests/server/test_task_timeout.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/deployables.py` & `steamship-2.7.17/tests/steamship_tests/utils/deployables.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,24 @@
 import contextlib
 import io
-import logging
 import os
-import subprocess  # noqa: S404
-import tempfile
-import time
 import zipfile
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from steamship_tests import ROOT_PATH, SRC_PATH, TEST_ASSETS_PATH
 
 from steamship import Package, PackageInstance, PackageVersion, Steamship
 from steamship.data.plugin import HostingType, Plugin
 from steamship.data.plugin.plugin_instance import PluginInstance
 from steamship.data.plugin.plugin_version import PluginVersion
 from steamship.data.user import User
 
 
-def install_dependencies(folder: str, requirements_path: Path):
-    subprocess.run(  # noqa: S607,S603
-        ["pip", "install", "--target", folder, "-r", str(requirements_path.resolve())],
-        stdout=subprocess.PIPE,
-    )
-    # Write an empty requirements.txt to the test deployment.
-    # Note that this is INTENTIONALLY different than the behavior of a deployable
-    # deployed with the CLI, so that you can use the steamship version that you're currently editing
-    with open(Path(folder) / "requirements.txt", "w") as requirements_file:
-        requirements_file.write("")
-
-
-def zip_deployable(file_path: Path) -> bytes:
+def zip_deployable(file_path: Path, additional_requirements: Optional[List[str]] = None) -> bytes:
     """Prepare and zip a Steamship plugin."""
 
     package_paths = [
         SRC_PATH / "steamship",
     ]
 
     zip_buffer = io.BytesIO()
@@ -45,26 +29,21 @@
 
         # Copy in the package paths from source
         for package_path in package_paths:
             for root, _, files in os.walk(package_path):
                 for file in files:
                     pypi_file = Path(root) / file
                     zip_file.write(pypi_file, pypi_file.relative_to(package_path.parent))
-
-        # Copy in package paths from pip
-        with tempfile.TemporaryDirectory() as package_dir:
-            logging.info(f"Created tempdir for pip installs: {package_dir}")
-            install_dependencies(
-                folder=package_dir, requirements_path=ROOT_PATH / "requirements.txt"
-            )
-            # Now write that whole folder
-            for root, _, files in os.walk(package_dir):
-                for file in files:
-                    pypi_file = Path(root) / file
-                    zip_file.write(pypi_file, pypi_file.relative_to(package_dir))
+        if additional_requirements is None:
+            zip_file.write(ROOT_PATH / "requirements.txt", "requirements.txt")
+        else:
+            with open(ROOT_PATH / "requirements.txt", "r") as file:
+                requirements_string = file.read()
+            requirements_string += "\n" + "\n".join(additional_requirements)
+            zip_file.writestr("requirements.txt", requirements_string)
 
         # Now we'll copy in the whole assets directory so that our test files can access things there..
         for root, _, files in os.walk(TEST_ASSETS_PATH):
             for file in files:
                 the_file = Path(root) / file
                 relative_path = the_file.relative_to(TEST_ASSETS_PATH.parent)
                 zip_file.write(the_file, relative_path)
@@ -79,14 +58,15 @@
     client: Steamship,
     py_path: Path,
     plugin_type: str,
     training_platform: Optional[HostingType] = None,
     version_config_template: Dict[str, Any] = None,
     instance_config: Dict[str, Any] = None,
     safe_load_handler: bool = False,
+    wait_for_init: bool = True,
 ):
     plugin = Plugin.create(
         client,
         training_platform=training_platform,
         type_=plugin_type,
         transport="jsonOverHttp",
         description="A Plugin (python client steamship_tests)",
@@ -115,26 +95,30 @@
     )
 
     assert plugin_instance.plugin_id == plugin.id
     assert plugin_instance.plugin_version_id == plugin_version.id
 
     _check_user(client, plugin_instance)
 
+    if wait_for_init:
+        plugin_instance.wait_for_init()
+
     yield plugin, plugin_version, plugin_instance
 
     _delete_deployable(plugin_instance, plugin_version, plugin)
 
 
 @contextlib.contextmanager
 def deploy_package(
     client: Steamship,
     py_path: Path,
     version_config_template: Dict[str, Any] = None,
     instance_config: Dict[str, Any] = None,
     safe_load_handler: bool = False,
+    wait_for_init: bool = True,
 ):
     package = Package.create(client)
 
     zip_bytes = zip_deployable(py_path)
     hosting_handler = "steamship.invocable.entrypoint.safe_handler" if safe_load_handler else None
     version = PackageVersion.create(
         client,
@@ -153,24 +137,28 @@
     )
 
     assert package_instance.package_id == package.id
     assert package_instance.package_version_id == version.id
 
     _check_user(client, package_instance)
 
+    if wait_for_init:
+        package_instance.wait_for_init()
+
     yield package, version, package_instance
 
     _delete_deployable(package_instance, version, package)
 
 
 def _check_user(client, instance):
     user = User.current(client)
     assert instance.user_id == user.id
 
 
 def _delete_deployable(instance, version, deployable):
     instance.delete()
+    version.delete()
+    deployable.delete()
 
 
 def _wait_for_version(version: [PackageVersion, PluginVersion]):
-    time.sleep(15)
     assert version is not None
```

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/fixtures.py` & `steamship-2.7.17/tests/steamship_tests/utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/random.py` & `steamship-2.7.17/tests/steamship_tests/utils/random.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_camel_model.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_camel_model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_client.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_enums.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_enums.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_kv_store.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_kv_store.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_signed_urls.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_signed_urls.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_static_instance_methods.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_static_instance_methods.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.9/tests/steamship_tests/utils/test_zip_archives.py` & `steamship-2.7.17/tests/steamship_tests/utils/test_zip_archives.py`

 * *Files identical despite different names*

