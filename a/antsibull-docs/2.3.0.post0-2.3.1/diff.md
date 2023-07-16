# Comparing `tmp/antsibull_docs-2.3.0.post0.tar.gz` & `tmp/antsibull_docs-2.3.1.tar.gz`

## Comparing `antsibull_docs-2.3.0.post0.tar` & `antsibull_docs-2.3.1.tar`

### file list

```diff
@@ -1,618 +1,618 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.flake8
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.pylintrc.automated
--rw-r--r--   0        0        0    29161 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/LICENSE
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/antsibull-docs.cfg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/codecov.yml
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/noxfile.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.github/patchback.yml
--rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.github/workflows/build-css.yml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.reuse/dep5
--rw-r--r--   0        0        0    35365 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/changelogs/fragments/.keep
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/docs/schemas.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/app_context.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/augment_docs.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/collection_config.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/collection_links.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/constants.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/env_variables.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/extra_docs.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_extra_docs.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_helpers.py
--rw-r--r--   0        0        0    33046 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_plugin_docs.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/plugin_docs.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/process_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/py.typed
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/rstcheck.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/__init__.py
--rw-r--r--   0        0        0    29884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/antsibull_docs.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/__init__.py
--rw-r--r--   0        0        0    13667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/_build.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/collection.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/collection_plugins.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/current.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/devel.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/lint_docs.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/plugin.py
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/stable.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/__init__.py
--rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/ansible_2_10_routing.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/__init__.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
--rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    13316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/build_sh.j2
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/conf_py.j2
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/__init__.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/ansible_doc.py
--rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/fqcn.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/parsing.py
--rw-r--r--   0        0        0    19449 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/routing.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/__init__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/environment.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/filters.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/tests.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/__init__.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/_counter.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/htmlify.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/rstify.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/semantic_helper.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/ansible_doc.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/app_context.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/collection_config.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/collection_links.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/ansible_doc.py
--rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/base.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/callback.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/module.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/plugin.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/positional.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/role.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/collection_name_transformer.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/get_pkg_data.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/rst.py
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/vendored/ansible.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/__init__.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/collections.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/hierarchy.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/indexes.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/plugin_stubs.py
--rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/plugins.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/__init__.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/antsibull-minimal.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/assets.py
--rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/roles.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/sphinx_helper.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/browserslistrc
--rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/build.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/cssnano.config.js
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/argcomplete.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/rstcheck.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/__init__.pyi
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/constants.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/release.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/cli/__init__.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/cli/arguments.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/collections/list.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/galaxy/collection.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/module_utils/_text.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/module_utils/common/json.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/plugins/loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/utils/collection_loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/ansible/utils/plugin_docs.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/jinja2/utils.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/rstcheck_core/__init__.pyi
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/rstcheck_core/checker.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/rstcheck_core/config.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/stubs/rstcheck_core/types.pyi
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/validate-html.py
--rw-r--r--   0        0        0  1043185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all-others.json.license
--rw-r--r--   0        0        0  1041339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all.json.license
--rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col1.json.license
--rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col2.json.license
--rw-r--r--   0        0        0    41105 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.col.json.license
--rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-all-others.json.license
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-all.json.license
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns.col1.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-version.output
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible-version.output.license
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/ansible_doc_caching.py
--rwxr-xr-x   0        0        0     3401 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/build-docs-baseline.sh
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/build-sphinx-init-baseline.sh
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/sanitize-ansible-doc-dump.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/sanitize-ansible-galaxy-list.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/test.rst
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/test_docs_baseline.py
--rw-r--r--   0        0        0   101030 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/test_docs_linting.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/test_sphinx_init_baseline.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/environment_variables.rst
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_become.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_cache.rst
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_callback.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_cliconf.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_connection.rst
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_filter.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_inventory.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_lookup.rst
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_module.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_role.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_shell.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_strategy.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_test.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_vars.rst
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/index.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/index.rst
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_become.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_cache.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_callback.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_cliconf.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_connection.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_filter.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_inventory.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_lookup.rst
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_module.rst
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_role.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_shell.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_strategy.rst
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_test.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_vars.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/index.rst
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col1/index.rst
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/index.rst
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_redirect_module.rst
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/.gitignore
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/build.sh
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/conf.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/requirements.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/build.sh
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/test_schema.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become.json.license
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become_results.json.license
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache.json.license
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache_results.json.license
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback.json.license
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback_results.json.license
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf.json.license
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf_results.json.license
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection.json.license
--rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection_results.json.license
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter.json.license
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter_results.json.license
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi.json.license
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi_results.json.license
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory.json.license
--rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory_results.json.license
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup.json.license
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup_results.json.license
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module.json.license
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf.json.license
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf_results.json.license
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role.json.license
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role_results.json.license
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell.json.license
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy.json.license
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy_results.json.license
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test.json.license
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test_results.json.license
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars.json.license
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars_results.json.license
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection.json.license
--rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection_results.json.license
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/units/test_jinja2.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/units/markup/test_counter.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/units/markup/test_markup.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/tests/units/markup/test_semantic_helper.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/.gitignore
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/README.md
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0    10045 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.flake8
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.pylintrc.automated
+-rw-r--r--   0        0        0    29161 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/antsibull-docs.cfg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/codecov.yml
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.github/patchback.yml
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.github/workflows/build-css.yml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.reuse/dep5
+-rw-r--r--   0        0        0    35365 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/changelogs/fragments/.keep
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/docs/schemas.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/app_context.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/augment_docs.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/collection_config.py
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/collection_links.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/constants.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/env_variables.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/extra_docs.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/lint_extra_docs.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/lint_helpers.py
+-rw-r--r--   0        0        0    33046 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/lint_plugin_docs.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/plugin_docs.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/process_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/py.typed
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/rstcheck.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/__init__.py
+-rw-r--r--   0        0        0    29884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/antsibull_docs.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/__init__.py
+-rw-r--r--   0        0        0    13667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/_build.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/collection.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/collection_plugins.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/current.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/devel.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/lint_docs.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/plugin.py
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/sphinx_init.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/stable.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/__init__.py
+-rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/ansible_2_10_routing.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    13316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/_gitignore.j2
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/build_sh.j2
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/conf_py.j2
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/__init__.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/ansible_doc.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/fqcn.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/parsing.py
+-rw-r--r--   0        0        0    19449 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/routing.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/jinja2/__init__.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/jinja2/environment.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/jinja2/filters.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/jinja2/tests.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/markup/__init__.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/markup/_counter.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/markup/htmlify.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/markup/rstify.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/markup/semantic_helper.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/ansible_doc.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/app_context.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/collection_config.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/collection_links.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/ansible_doc.py
+-rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/base.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/callback.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/module.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/plugin.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/positional.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/role.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/utils/collection_name_transformer.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/utils/get_pkg_data.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/utils/rst.py
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/vendored/ansible.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/__init__.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/collections.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/hierarchy.py
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/indexes.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/plugin_stubs.py
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/antsibull_docs/write_docs/plugins.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/__init__.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/antsibull-minimal.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/antsibull-minimal.css.license
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/assets.py
+-rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/roles.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/sphinx_helper.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/browserslistrc
+-rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/build.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/cssnano.config.js
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/argcomplete.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/rstcheck.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/__init__.pyi
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/constants.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/release.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/cli/__init__.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/cli/arguments.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/collections/list.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/galaxy/collection.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/module_utils/_text.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/module_utils/common/json.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/plugins/loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/utils/collection_loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/ansible/utils/plugin_docs.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/jinja2/utils.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/rstcheck_core/__init__.pyi
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/rstcheck_core/checker.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/rstcheck_core/config.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/stubs/rstcheck_core/types.pyi
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/validate-html.py
+-rw-r--r--   0        0        0  1043185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all-others.json.license
+-rw-r--r--   0        0        0  1041339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all.json.license
+-rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col1.json.license
+-rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col2.json.license
+-rw-r--r--   0        0        0    41105 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.col.json.license
+-rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-all-others.json.license
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-all.json.license
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns.col1.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns.col2.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns2.col.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-version.output
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible-version.output.license
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/ansible_doc_caching.py
+-rwxr-xr-x   0        0        0     3401 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/build-docs-baseline.sh
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/build-sphinx-init-baseline.sh
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/sanitize-ansible-doc-dump.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/sanitize-ansible-galaxy-list.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/test.rst
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/test_docs_baseline.py
+-rw-r--r--   0        0        0   101030 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/test_docs_linting.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/test_sphinx_init_baseline.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/environment_variables.rst
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_lookup.rst
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_module.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_vars.rst
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/index.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/environment_variables.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_become.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_cache.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_callback.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_connection.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_filter.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_inventory.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_lookup.rst
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_module.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_role.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_shell.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_strategy.rst
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_test.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_vars.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/index.rst
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/index.rst
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/.gitignore
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/build.sh
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/conf.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/requirements.txt
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/build.sh
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/rst/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/environment_variables.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_module.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/test_schema.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become.json.license
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become_results.json.license
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache.json.license
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache_results.json.license
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback.json.license
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback_results.json.license
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf.json.license
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf_results.json.license
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection.json.license
+-rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection_results.json.license
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter.json.license
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter_results.json.license
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi.json.license
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi_results.json.license
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory.json.license
+-rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory_results.json.license
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup.json.license
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup_results.json.license
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module.json.license
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf.json.license
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf_results.json.license
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role.json.license
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role_results.json.license
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell.json.license
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy.json.license
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy_results.json.license
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test.json.license
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test_results.json.license
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars.json.license
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars_results.json.license
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection.json.license
+-rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection_results.json.license
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/units/test_jinja2.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/units/markup/test_counter.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/units/markup/test_markup.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/tests/units/markup/test_semantic_helper.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/.gitignore
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/README.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 antsibull_docs-2.3.1/PKG-INFO
```

### Comparing `antsibull_docs-2.3.0.post0/.pylintrc.automated` & `antsibull_docs-2.3.1/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/CHANGELOG.rst` & `antsibull_docs-2.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/LICENSE` & `antsibull_docs-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/antsibull-docs.cfg` & `antsibull_docs-2.3.1/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/noxfile.py` & `antsibull_docs-2.3.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/.github/workflows/antsibull-docs.yml` & `antsibull_docs-2.3.1/.github/workflows/antsibull-docs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/.github/workflows/build-css.yml` & `antsibull_docs-2.3.1/.github/workflows/build-css.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/.github/workflows/nox.yml` & `antsibull_docs-2.3.1/.github/workflows/nox.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/changelogs/changelog.yaml` & `antsibull_docs-2.3.1/changelogs/changelog.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/changelogs/config.yaml` & `antsibull_docs-2.3.1/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/docs/schemas.rst` & `antsibull_docs-2.3.1/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/app_context.py` & `antsibull_docs-2.3.1/src/antsibull_docs/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/augment_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/augment_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/collection_config.py` & `antsibull_docs-2.3.1/src/antsibull_docs/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/collection_links.py` & `antsibull_docs-2.3.1/src/antsibull_docs/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/constants.py` & `antsibull_docs-2.3.1/src/antsibull_docs/constants.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/env_variables.py` & `antsibull_docs-2.3.1/src/antsibull_docs/env_variables.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/extra_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_extra_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/lint_extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_helpers.py` & `antsibull_docs-2.3.1/src/antsibull_docs/lint_helpers.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/lint_plugin_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/lint_plugin_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/plugin_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/plugin_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/process_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/process_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/rstcheck.py` & `antsibull_docs-2.3.1/src/antsibull_docs/rstcheck.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/antsibull_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/antsibull_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/_build.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/_build.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/collection.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/collection.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/collection_plugins.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/collection_plugins.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/current.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/current.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/devel.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/devel.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/lint_docs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/lint_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/plugin.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/sphinx_init.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/sphinx_init.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/cli/doc_commands/stable.py` & `antsibull_docs-2.3.1/src/antsibull_docs/cli/doc_commands/stable.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/ansible_2_10_routing.yml` & `antsibull_docs-2.3.1/src/antsibull_docs/data/ansible_2_10_routing.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/build_sh.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/build_sh.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/conf_py.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/conf_py.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2` & `antsibull_docs-2.3.1/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/__init__.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/ansible_doc.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/fqcn.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/fqcn.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/parsing.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/parsing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/docs_parsing/routing.py` & `antsibull_docs-2.3.1/src/antsibull_docs/docs_parsing/routing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/__init__.py` & `antsibull_docs-2.3.1/src/antsibull_docs/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/environment.py` & `antsibull_docs-2.3.1/src/antsibull_docs/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/filters.py` & `antsibull_docs-2.3.1/src/antsibull_docs/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/jinja2/tests.py` & `antsibull_docs-2.3.1/src/antsibull_docs/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/_counter.py` & `antsibull_docs-2.3.1/src/antsibull_docs/markup/_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/htmlify.py` & `antsibull_docs-2.3.1/src/antsibull_docs/markup/htmlify.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/rstify.py` & `antsibull_docs-2.3.1/src/antsibull_docs/markup/rstify.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/markup/semantic_helper.py` & `antsibull_docs-2.3.1/src/antsibull_docs/markup/semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/ansible_doc.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/app_context.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/collection_config.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/collection_links.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/__init__.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/ansible_doc.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/base.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/base.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/callback.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/callback.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/module.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/module.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/plugin.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/positional.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/positional.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/schemas/docs/role.py` & `antsibull_docs-2.3.1/src/antsibull_docs/schemas/docs/role.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/collection_name_transformer.py` & `antsibull_docs-2.3.1/src/antsibull_docs/utils/collection_name_transformer.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/utils/get_pkg_data.py` & `antsibull_docs-2.3.1/src/antsibull_docs/utils/get_pkg_data.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/vendored/ansible.py` & `antsibull_docs-2.3.1/src/antsibull_docs/vendored/ansible.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/__init__.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/collections.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/hierarchy.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/hierarchy.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/indexes.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/indexes.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/plugin_stubs.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/plugin_stubs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/antsibull_docs/write_docs/plugins.py` & `antsibull_docs-2.3.1/src/antsibull_docs/write_docs/plugins.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/__init__.py` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/antsibull-minimal.css` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/antsibull-minimal.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/assets.py` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/assets.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/roles.py` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/roles.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/sphinx_helper.py` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/sphinx_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/antsibull-minimal.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/src/sphinx_antsibull_ext/css/build.sh` & `antsibull_docs-2.3.1/src/sphinx_antsibull_ext/css/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/stubs/rstcheck.pyi` & `antsibull_docs-2.3.1/stubs/rstcheck.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/stubs/rstcheck_core/config.pyi` & `antsibull_docs-2.3.1/stubs/rstcheck_core/config.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/validate-html.py` & `antsibull_docs-2.3.1/tests/validate-html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all-others.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all-others.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-all.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-all.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col1.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col1.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns.col2.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns.col2.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.col.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.col.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-doc-cache-ns2.flatcol.json` & `antsibull_docs-2.3.1/tests/functional/ansible-doc-cache-ns2.flatcol.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible-version.output` & `antsibull_docs-2.3.1/tests/functional/ansible-version.output`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/ansible_doc_caching.py` & `antsibull_docs-2.3.1/tests/functional/ansible_doc_caching.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/build-docs-baseline.sh` & `antsibull_docs-2.3.1/tests/functional/build-docs-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/build-sphinx-init-baseline.sh` & `antsibull_docs-2.3.1/tests/functional/build-sphinx-init-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/sanitize-ansible-doc-dump.py` & `antsibull_docs-2.3.1/tests/functional/sanitize-ansible-doc-dump.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/sanitize-ansible-galaxy-list.py` & `antsibull_docs-2.3.1/tests/functional/sanitize-ansible-galaxy-list.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/test_docs_baseline.py` & `antsibull_docs-2.3.1/tests/functional/test_docs_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/test_docs_linting.py` & `antsibull_docs-2.3.1/tests/functional/test_docs_linting.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/test_sphinx_init_baseline.py` & `antsibull_docs-2.3.1/tests/functional/test_sphinx_init_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/environment_variables.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/index_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns/col2/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-default/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/environment_variables.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/index_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/build.sh` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-collections/conf.py` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-collections/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/build.sh` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-config/conf.py` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-config/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/build.sh` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-current/conf.py` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-current/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/build.sh` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-sphinx-init-extra/conf.py` & `antsibull_docs-2.3.1/tests/functional/baseline-sphinx-init-extra/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/environment_variables.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py` & `antsibull_docs-2.3.1/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py` & `antsibull_docs-2.3.1/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py` & `antsibull_docs-2.3.1/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/test_schema.py` & `antsibull_docs-2.3.1/tests/functional/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_become_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_become_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cache_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cache_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_callback_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_callback_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_cliconf_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_cliconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_connection_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_filter_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_filter_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_httpapi_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_httpapi_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_inventory_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_inventory_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_lookup_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_lookup_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_module_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_module_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_netconf_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_netconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_role_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_role_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_shell_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_shell_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_strategy_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_strategy_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_test_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_test_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/one_vars_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/one_vars_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/functional/schema/good_data/ssh_connection_results.json` & `antsibull_docs-2.3.1/tests/functional/schema/good_data/ssh_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/units/test_jinja2.py` & `antsibull_docs-2.3.1/tests/units/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/units/markup/test_counter.py` & `antsibull_docs-2.3.1/tests/units/markup/test_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/units/markup/test_markup.py` & `antsibull_docs-2.3.1/tests/units/markup/test_markup.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/tests/units/markup/test_semantic_helper.py` & `antsibull_docs-2.3.1/tests/units/markup/test_semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/.gitignore` & `antsibull_docs-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/README.md` & `antsibull_docs-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/pyproject.toml` & `antsibull_docs-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs"
-version = "2.3.0.post0"
+version = "2.3.1"
 description = "Tools for building Ansible documentation"
 license = "GPL-3.0-or-later"
 license-files = {globs=["LICENSES/*.txt"]}
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Ansible",
```

### Comparing `antsibull_docs-2.3.0.post0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs-2.3.1/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.3.0.post0/PKG-INFO` & `antsibull_docs-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs
-Version: 2.3.0.post0
+Version: 2.3.1
 Summary: Tools for building Ansible documentation
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-docs/issues
 Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later
```

