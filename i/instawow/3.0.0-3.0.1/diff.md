# Comparing `tmp/instawow-3.0.0.tar.gz` & `tmp/instawow-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instawow-3.0.0.tar", max compression
+gzip compressed data, was "instawow-3.0.1.tar", max compression
```

## Comparing `instawow-3.0.0.tar` & `instawow-3.0.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     2110 2023-06-15 21:30:50.086022 instawow-3.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-3.0.0/COPYING
--rw-r--r--   0        0        0     7860 2023-05-29 18:39:16.917316 instawow-3.0.0/README.rst
--rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-3.0.0/gui-webview/src/instawow_gui/__init__.py
--rw-r--r--   0        0        0     4374 2023-06-15 21:30:50.086871 instawow-3.0.0/gui-webview/src/instawow_gui/app.py
--rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-3.0.0/gui-webview/src/instawow_gui/frontend/.gitignore
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-3.0.0/gui-webview/src/instawow_gui/frontend/__init__.py
--rw-r--r--   0        0        0      415 2023-06-15 21:47:45.678440 instawow-3.0.0/gui-webview/src/instawow_gui/frontend/index.html
--rw-r--r--   0        0        0    19643 2023-06-15 21:48:01.233901 instawow-3.0.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
--rw-r--r--   0        0        0   514792 2023-06-15 21:48:01.237424 instawow-3.0.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
--rw-r--r--   0        0        0    28364 2023-06-15 08:47:57.174236 instawow-3.0.0/gui-webview/src/instawow_gui/json_rpc_server.py
--rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-3.0.0/gui-webview/src/instawow_gui/py.typed
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-3.0.0/gui-webview/src/instawow_gui/resources/__init__.py
--rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns
--rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico
--rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.png
--rw-r--r--   0        0        0     3677 2023-06-15 21:48:32.484777 instawow-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      213 2023-04-13 13:01:04.746899 instawow-3.0.0/src/instawow/__init__.py
--rw-r--r--   0        0        0      480 2023-02-10 14:46:48.188526 instawow-3.0.0/src/instawow/__main__.py
--rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-3.0.0/src/instawow/_addon_hashing.py
--rw-r--r--   0        0        0    10049 2023-06-08 14:48:29.524925 instawow-3.0.0/src/instawow/_cli_prompts.py
--rw-r--r--   0        0        0     7760 2023-02-01 10:07:51.063301 instawow-3.0.0/src/instawow/_custom_slpp.py
--rw-r--r--   0        0        0     3429 2023-06-07 20:33:05.900705 instawow-3.0.0/src/instawow/_http_cache_db.py
--rw-r--r--   0        0        0      842 2023-04-17 17:43:24.869397 instawow-3.0.0/src/instawow/_import_wrapper.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-3.0.0/src/instawow/_migrations/__init__.py
--rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-3.0.0/src/instawow/_migrations/alembic.ini
--rw-r--r--   0        0        0     1265 2023-05-29 18:35:35.600953 instawow-3.0.0/src/instawow/_migrations/env.py
--rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-3.0.0/src/instawow/_migrations/script.py.mako
--rw-r--r--   0        0        0      567 2023-04-26 09:53:54.276530 instawow-3.0.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
--rw-r--r--   0        0        0      615 2023-02-10 14:46:48.148613 instawow-3.0.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
--rw-r--r--   0        0        0      771 2023-02-10 14:46:48.142255 instawow-3.0.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
--rw-r--r--   0        0        0     1330 2023-02-10 14:46:48.148806 instawow-3.0.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
--rw-r--r--   0        0        0      752 2023-02-10 14:46:48.137514 instawow-3.0.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
--rw-r--r--   0        0        0      769 2023-02-10 14:46:48.139872 instawow-3.0.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
--rw-r--r--   0        0        0      858 2023-02-10 14:46:48.133648 instawow-3.0.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
--rw-r--r--   0        0        0     3242 2023-02-10 14:46:48.157600 instawow-3.0.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
--rw-r--r--   0        0        0     2601 2023-02-10 14:46:48.153141 instawow-3.0.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
--rw-r--r--   0        0        0      814 2023-02-10 14:46:48.145012 instawow-3.0.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-3.0.0/src/instawow/_migrations/versions/__init__.py
--rw-r--r--   0        0        0      784 2023-02-10 14:46:48.139232 instawow-3.0.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
--rw-r--r--   0        0        0     3847 2023-02-10 14:46:48.143020 instawow-3.0.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py
--rw-r--r--   0        0        0     1266 2023-02-10 14:46:48.135782 instawow-3.0.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
--rw-r--r--   0        0        0     1231 2023-02-10 14:46:48.147304 instawow-3.0.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
--rw-r--r--   0        0        0      556 2023-02-10 14:46:48.146303 instawow-3.0.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
--rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-3.0.0/src/instawow/_sources/__init__.py
--rw-r--r--   0        0        0    14356 2023-06-10 11:12:09.538866 instawow-3.0.0/src/instawow/_sources/cfcore.py
--rw-r--r--   0        0        0    16378 2023-05-29 18:35:35.601774 instawow-3.0.0/src/instawow/_sources/github.py
--rw-r--r--   0        0        0     2339 2023-05-29 18:35:35.556230 instawow-3.0.0/src/instawow/_sources/instawow.py
--rw-r--r--   0        0        0     3764 2023-06-06 15:31:10.708481 instawow-3.0.0/src/instawow/_sources/tukui.py
--rw-r--r--   0        0        0     6837 2023-05-29 18:35:35.556331 instawow-3.0.0/src/instawow/_sources/wago.py
--rw-r--r--   0        0        0     8715 2023-06-15 21:30:50.087839 instawow-3.0.0/src/instawow/_sources/wowi.py
--rw-r--r--   0        0        0     1317 2023-06-15 21:48:32.488617 instawow-3.0.0/src/instawow/_version.py
--rw-r--r--   0        0        0      120 2022-12-15 17:34:52.403485 instawow-3.0.0/src/instawow/_wa_templates/CHANGELOG.md
--rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-3.0.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
--rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-3.0.0/src/instawow/_wa_templates/README
--rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-3.0.0/src/instawow/_wa_templates/WeakAurasCompanion.toc
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-3.0.0/src/instawow/_wa_templates/__init__.py
--rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-3.0.0/src/instawow/_wa_templates/data.lua
--rw-r--r--   0        0        0     1059 2023-04-22 08:30:05.257712 instawow-3.0.0/src/instawow/_wa_templates/init.lua
--rw-r--r--   0        0        0     3772 2023-05-29 18:31:15.588569 instawow-3.0.0/src/instawow/cataloguer.py
--rw-r--r--   0        0        0    45077 2023-06-10 11:17:32.726471 instawow-3.0.0/src/instawow/cli.py
--rw-r--r--   0        0        0     5442 2023-05-28 08:27:31.429396 instawow-3.0.0/src/instawow/common.py
--rw-r--r--   0        0        0    13193 2023-06-10 17:54:07.035884 instawow-3.0.0/src/instawow/config.py
--rw-r--r--   0        0        0     1657 2023-05-13 09:07:15.761326 instawow-3.0.0/src/instawow/github_auth.py
--rw-r--r--   0        0        0     3180 2023-06-07 20:31:59.197436 instawow-3.0.0/src/instawow/http.py
--rw-r--r--   0        0        0    30152 2023-05-29 18:36:34.266735 instawow-3.0.0/src/instawow/manager.py
--rw-r--r--   0        0        0     6686 2023-05-29 18:35:35.601602 instawow-3.0.0/src/instawow/matchers.py
--rw-r--r--   0        0        0     4973 2023-05-26 14:23:06.080614 instawow-3.0.0/src/instawow/pkg_db.py
--rw-r--r--   0        0        0     3915 2023-06-10 07:25:09.673724 instawow-3.0.0/src/instawow/pkg_models.py
--rw-r--r--   0        0        0     1204 2023-04-30 09:14:55.435397 instawow-3.0.0/src/instawow/plugins.py
--rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-3.0.0/src/instawow/py.typed
--rw-r--r--   0        0        0     5324 2023-06-10 14:54:02.738499 instawow-3.0.0/src/instawow/resolvers.py
--rw-r--r--   0        0        0     4845 2023-05-29 18:36:33.688476 instawow-3.0.0/src/instawow/results.py
--rw-r--r--   0        0        0     8941 2023-05-17 07:03:57.941218 instawow-3.0.0/src/instawow/utils.py
--rw-r--r--   0        0        0    12525 2023-05-13 22:09:38.962298 instawow-3.0.0/src/instawow/wa_updater.py
--rw-r--r--   0        0        0     1628 2023-05-25 07:07:09.513115 instawow-3.0.0/src/instawow/wow_installations.py
--rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4091 2023-06-10 11:13:27.968210 instawow-3.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-3.0.0/tests/fixtures/FakeAddon/FakeAddon.lua
--rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-3.0.0/tests/fixtures/FakeAddon/FakeAddon.toc
--rw-r--r--   0        0        0     7661 2023-06-06 20:48:00.489989 instawow-3.0.0/tests/fixtures/http/__init__.py
--rw-r--r--   0        0        0  6104393 2023-06-06 20:49:12.044214 instawow-3.0.0/tests/fixtures/http/base-catalogue-v7.compact.json
--rw-r--r--   0        0        0   232321 2023-06-06 20:48:41.590803 instawow-3.0.0/tests/fixtures/http/curse-addon--all.json
--rw-r--r--   0        0        0      113 2023-06-06 20:48:45.250746 instawow-3.0.0/tests/fixtures/http/curse-addon-changelog.json
--rw-r--r--   0        0        0    91509 2023-06-06 20:48:42.461796 instawow-3.0.0/tests/fixtures/http/curse-addon-files.json
--rw-r--r--   0        0        0      115 2023-06-06 20:49:12.208158 instawow-3.0.0/tests/fixtures/http/github-oauth-login-access-token.json
--rw-r--r--   0        0        0      187 2023-06-06 20:49:12.132502 instawow-3.0.0/tests/fixtures/http/github-oauth-login-device-code.json
--rw-r--r--   0        0        0      446 2023-06-06 20:49:01.616742 instawow-3.0.0/tests/fixtures/http/github-release-molinari-release-json.json
--rw-r--r--   0        0        0     6139 2023-06-06 20:48:59.919739 instawow-3.0.0/tests/fixtures/http/github-release-molinari.json
--rw-r--r--   0        0        0     1895 2023-06-06 20:49:09.317621 instawow-3.0.0/tests/fixtures/http/github-release-no-assets.json
--rw-r--r--   0        0        0     8022 2023-06-06 20:49:05.521565 instawow-3.0.0/tests/fixtures/http/github-release-no-release-json.json
--rw-r--r--   0        0        0      398 2023-06-06 20:48:56.927056 instawow-3.0.0/tests/fixtures/http/github-release-release-json-release-json.json
--rw-r--r--   0        0        0     8128 2023-06-06 20:48:54.924791 instawow-3.0.0/tests/fixtures/http/github-release-release-json.json
--rw-r--r--   0        0        0     6742 2023-06-06 20:48:58.033753 instawow-3.0.0/tests/fixtures/http/github-repo-molinari.json
--rw-r--r--   0        0        0     5632 2023-06-06 20:49:03.327014 instawow-3.0.0/tests/fixtures/http/github-repo-no-release-json.json
--rw-r--r--   0        0        0     6803 2023-06-06 20:49:07.571590 instawow-3.0.0/tests/fixtures/http/github-repo-no-releases.json
--rw-r--r--   0        0        0     5536 2023-06-06 20:48:53.504470 instawow-3.0.0/tests/fixtures/http/github-repo-release-json.json
--rwxr-xr-x   0        0        0     4183 2023-06-06 20:48:22.101303 instawow-3.0.0/tests/fixtures/http/regen.sh
--rw-r--r--   0        0        0      769 2023-06-06 23:19:53.522108 instawow-3.0.0/tests/fixtures/http/tukui-ui--elvui.json
--rw-r--r--   0        0        0      676 2023-06-06 23:20:04.298176 instawow-3.0.0/tests/fixtures/http/tukui-ui--tukui.json
--rw-r--r--   0        0        0      938 2023-06-06 20:49:12.279530 instawow-3.0.0/tests/fixtures/http/wago-match-addons.json
--rw-r--r--   0        0        0     3072 2023-06-06 20:48:49.124687 instawow-3.0.0/tests/fixtures/http/wowi-filedetails.json
--rw-r--r--   0        0        0      930 2023-06-06 20:48:47.677451 instawow-3.0.0/tests/fixtures/http/wowi-filelist.json
--rw-r--r--   0        0        0     1328 2023-05-29 18:35:35.550835 instawow-3.0.0/tests/plugin/instawow_test_plugin.py
--rw-r--r--   0        0        0      276 2023-04-30 09:12:16.610136 instawow-3.0.0/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0     5553 2023-05-25 15:00:57.258425 instawow-3.0.0/tests/test__slpp.py
--rw-r--r--   0        0        0     8500 2023-06-06 15:51:10.450525 instawow-3.0.0/tests/test__sources.py
--rw-r--r--   0        0        0     3125 2023-06-10 11:16:29.545570 instawow-3.0.0/tests/test__version.py
--rw-r--r--   0        0        0    17897 2023-06-06 20:51:58.192542 instawow-3.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     1350 2023-05-19 22:19:41.380750 instawow-3.0.0/tests/test_common.py
--rw-r--r--   0        0        0     3770 2023-06-10 11:20:20.064181 instawow-3.0.0/tests/test_config.py
--rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-3.0.0/tests/test_github_oauth_flow.py
--rw-r--r--   0        0        0     3033 2023-06-06 23:13:59.658917 instawow-3.0.0/tests/test_github_zip_parsing.py
--rw-r--r--   0        0        0     4473 2023-06-08 14:41:42.827899 instawow-3.0.0/tests/test_json_rpc_api.py
--rw-r--r--   0        0        0    13424 2023-06-06 20:53:39.204136 instawow-3.0.0/tests/test_manager.py
--rw-r--r--   0        0        0     3935 2023-06-06 23:17:04.310471 instawow-3.0.0/tests/test_matchers.py
--rw-r--r--   0        0        0     4491 2023-01-04 01:37:53.376282 instawow-3.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     3487 2023-05-29 18:36:14.611876 instawow-3.0.0/tests/test_wa_updater.py
--rw-r--r--   0        0        0     2029 2023-05-25 14:00:11.531683 instawow-3.0.0/tests/test_wow_installations.py
--rw-r--r--   0        0        0     9568 1970-01-01 00:00:00.000000 instawow-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2110 2023-06-15 21:30:50.086022 instawow-3.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-3.0.1/COPYING
+-rw-r--r--   0        0        0     7860 2023-05-29 18:39:16.917316 instawow-3.0.1/README.rst
+-rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-3.0.1/gui-webview/src/instawow_gui/__init__.py
+-rw-r--r--   0        0        0     4374 2023-06-15 21:30:50.086871 instawow-3.0.1/gui-webview/src/instawow_gui/app.py
+-rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-3.0.1/gui-webview/src/instawow_gui/frontend/.gitignore
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-3.0.1/gui-webview/src/instawow_gui/frontend/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-16 08:09:30.799367 instawow-3.0.1/gui-webview/src/instawow_gui/frontend/index.html
+-rw-r--r--   0        0        0    19643 2023-07-16 08:09:40.519062 instawow-3.0.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
+-rw-r--r--   0        0        0   515006 2023-07-16 08:09:40.518958 instawow-3.0.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
+-rw-r--r--   0        0        0    28235 2023-07-16 06:53:54.839021 instawow-3.0.1/gui-webview/src/instawow_gui/json_rpc_server.py
+-rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-3.0.1/gui-webview/src/instawow_gui/py.typed
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-3.0.1/gui-webview/src/instawow_gui/resources/__init__.py
+-rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.icns
+-rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.ico
+-rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.png
+-rw-r--r--   0        0        0     3628 2023-07-16 08:11:04.366249 instawow-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-04-13 13:01:04.746899 instawow-3.0.1/src/instawow/__init__.py
+-rw-r--r--   0        0        0      480 2023-02-10 14:46:48.188526 instawow-3.0.1/src/instawow/__main__.py
+-rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-3.0.1/src/instawow/_addon_hashing.py
+-rw-r--r--   0        0        0    10049 2023-06-08 14:48:29.524925 instawow-3.0.1/src/instawow/_cli_prompts.py
+-rw-r--r--   0        0        0     7760 2023-02-01 10:07:51.063301 instawow-3.0.1/src/instawow/_custom_slpp.py
+-rw-r--r--   0        0        0     3429 2023-06-07 20:33:05.900705 instawow-3.0.1/src/instawow/_http_cache_db.py
+-rw-r--r--   0        0        0      842 2023-04-17 17:43:24.869397 instawow-3.0.1/src/instawow/_import_wrapper.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-3.0.1/src/instawow/_migrations/__init__.py
+-rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-3.0.1/src/instawow/_migrations/alembic.ini
+-rw-r--r--   0        0        0     1265 2023-05-29 18:35:35.600953 instawow-3.0.1/src/instawow/_migrations/env.py
+-rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-3.0.1/src/instawow/_migrations/script.py.mako
+-rw-r--r--   0        0        0      567 2023-04-26 09:53:54.276530 instawow-3.0.1/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
+-rw-r--r--   0        0        0      615 2023-02-10 14:46:48.148613 instawow-3.0.1/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
+-rw-r--r--   0        0        0      771 2023-02-10 14:46:48.142255 instawow-3.0.1/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
+-rw-r--r--   0        0        0     1330 2023-02-10 14:46:48.148806 instawow-3.0.1/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
+-rw-r--r--   0        0        0      752 2023-02-10 14:46:48.137514 instawow-3.0.1/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
+-rw-r--r--   0        0        0      769 2023-02-10 14:46:48.139872 instawow-3.0.1/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
+-rw-r--r--   0        0        0      858 2023-02-10 14:46:48.133648 instawow-3.0.1/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
+-rw-r--r--   0        0        0     3242 2023-02-10 14:46:48.157600 instawow-3.0.1/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
+-rw-r--r--   0        0        0     2601 2023-02-10 14:46:48.153141 instawow-3.0.1/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
+-rw-r--r--   0        0        0      814 2023-02-10 14:46:48.145012 instawow-3.0.1/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-3.0.1/src/instawow/_migrations/versions/__init__.py
+-rw-r--r--   0        0        0      784 2023-02-10 14:46:48.139232 instawow-3.0.1/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
+-rw-r--r--   0        0        0     3847 2023-02-10 14:46:48.143020 instawow-3.0.1/src/instawow/_migrations/versions/e13430219249_add_cascade.py
+-rw-r--r--   0        0        0     1266 2023-02-10 14:46:48.135782 instawow-3.0.1/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
+-rw-r--r--   0        0        0     1231 2023-02-10 14:46:48.147304 instawow-3.0.1/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
+-rw-r--r--   0        0        0      556 2023-02-10 14:46:48.146303 instawow-3.0.1/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
+-rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-3.0.1/src/instawow/_sources/__init__.py
+-rw-r--r--   0        0        0    14356 2023-06-10 11:12:09.538866 instawow-3.0.1/src/instawow/_sources/cfcore.py
+-rw-r--r--   0        0        0    16632 2023-07-16 07:27:28.821240 instawow-3.0.1/src/instawow/_sources/github.py
+-rw-r--r--   0        0        0     2318 2023-06-24 13:57:24.797957 instawow-3.0.1/src/instawow/_sources/instawow.py
+-rw-r--r--   0        0        0     3764 2023-06-17 15:44:51.513169 instawow-3.0.1/src/instawow/_sources/tukui.py
+-rw-r--r--   0        0        0     6837 2023-05-29 18:35:35.556331 instawow-3.0.1/src/instawow/_sources/wago.py
+-rw-r--r--   0        0        0     8715 2023-06-15 21:30:50.087839 instawow-3.0.1/src/instawow/_sources/wowi.py
+-rw-r--r--   0        0        0     1317 2023-07-16 08:11:04.369754 instawow-3.0.1/src/instawow/_version.py
+-rw-r--r--   0        0        0      120 2022-12-15 17:34:52.403485 instawow-3.0.1/src/instawow/_wa_templates/CHANGELOG.md
+-rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-3.0.1/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
+-rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-3.0.1/src/instawow/_wa_templates/README
+-rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-3.0.1/src/instawow/_wa_templates/WeakAurasCompanion.toc
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-3.0.1/src/instawow/_wa_templates/__init__.py
+-rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-3.0.1/src/instawow/_wa_templates/data.lua
+-rw-r--r--   0        0        0     1059 2023-04-22 08:30:05.257712 instawow-3.0.1/src/instawow/_wa_templates/init.lua
+-rw-r--r--   0        0        0     3813 2023-06-24 14:19:16.240393 instawow-3.0.1/src/instawow/cataloguer.py
+-rw-r--r--   0        0        0    45612 2023-07-16 08:02:36.471735 instawow-3.0.1/src/instawow/cli.py
+-rw-r--r--   0        0        0     5442 2023-05-28 08:27:31.429396 instawow-3.0.1/src/instawow/common.py
+-rw-r--r--   0        0        0    13193 2023-06-10 17:54:07.035884 instawow-3.0.1/src/instawow/config.py
+-rw-r--r--   0        0        0     1657 2023-05-13 09:07:15.761326 instawow-3.0.1/src/instawow/github_auth.py
+-rw-r--r--   0        0        0     3180 2023-06-07 20:31:59.197436 instawow-3.0.1/src/instawow/http.py
+-rw-r--r--   0        0        0    29985 2023-06-24 15:19:54.142645 instawow-3.0.1/src/instawow/manager.py
+-rw-r--r--   0        0        0     6686 2023-05-29 18:35:35.601602 instawow-3.0.1/src/instawow/matchers.py
+-rw-r--r--   0        0        0     4973 2023-05-26 14:23:06.080614 instawow-3.0.1/src/instawow/pkg_db.py
+-rw-r--r--   0        0        0     3973 2023-06-24 14:00:21.171451 instawow-3.0.1/src/instawow/pkg_models.py
+-rw-r--r--   0        0        0     1204 2023-07-08 15:12:55.198028 instawow-3.0.1/src/instawow/plugins.py
+-rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-3.0.1/src/instawow/py.typed
+-rw-r--r--   0        0        0     5324 2023-07-08 15:13:13.325191 instawow-3.0.1/src/instawow/resolvers.py
+-rw-r--r--   0        0        0     4932 2023-06-24 14:18:39.633647 instawow-3.0.1/src/instawow/results.py
+-rw-r--r--   0        0        0     8928 2023-06-24 13:30:10.904313 instawow-3.0.1/src/instawow/utils.py
+-rw-r--r--   0        0        0    12525 2023-05-13 22:09:38.962298 instawow-3.0.1/src/instawow/wa_updater.py
+-rw-r--r--   0        0        0     1628 2023-05-25 07:07:09.513115 instawow-3.0.1/src/instawow/wow_installations.py
+-rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-3.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     4091 2023-06-10 11:13:27.968210 instawow-3.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-3.0.1/tests/fixtures/FakeAddon/FakeAddon.lua
+-rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-3.0.1/tests/fixtures/FakeAddon/FakeAddon.toc
+-rw-r--r--   0        0        0     7821 2023-07-16 07:36:58.505899 instawow-3.0.1/tests/fixtures/http/__init__.py
+-rw-r--r--   0        0        0  6104393 2023-06-06 20:49:12.044214 instawow-3.0.1/tests/fixtures/http/base-catalogue-v7.compact.json
+-rw-r--r--   0        0        0   232321 2023-06-06 20:48:41.590803 instawow-3.0.1/tests/fixtures/http/curse-addon--all.json
+-rw-r--r--   0        0        0      113 2023-06-06 20:48:45.250746 instawow-3.0.1/tests/fixtures/http/curse-addon-changelog.json
+-rw-r--r--   0        0        0    91509 2023-06-06 20:48:42.461796 instawow-3.0.1/tests/fixtures/http/curse-addon-files.json
+-rw-r--r--   0        0        0      115 2023-06-06 20:49:12.208158 instawow-3.0.1/tests/fixtures/http/github-oauth-login-access-token.json
+-rw-r--r--   0        0        0      187 2023-06-06 20:49:12.132502 instawow-3.0.1/tests/fixtures/http/github-oauth-login-device-code.json
+-rw-r--r--   0        0        0      446 2023-06-06 20:49:01.616742 instawow-3.0.1/tests/fixtures/http/github-release-molinari-release-json.json
+-rw-r--r--   0        0        0     6139 2023-06-06 20:48:59.919739 instawow-3.0.1/tests/fixtures/http/github-release-molinari.json
+-rw-r--r--   0        0        0     1895 2023-06-06 20:49:09.317621 instawow-3.0.1/tests/fixtures/http/github-release-no-assets.json
+-rw-r--r--   0        0        0     8022 2023-06-06 20:49:05.521565 instawow-3.0.1/tests/fixtures/http/github-release-no-release-json.json
+-rw-r--r--   0        0        0      398 2023-06-06 20:48:56.927056 instawow-3.0.1/tests/fixtures/http/github-release-release-json-release-json.json
+-rw-r--r--   0        0        0     8128 2023-06-06 20:48:54.924791 instawow-3.0.1/tests/fixtures/http/github-release-release-json.json
+-rw-r--r--   0        0        0     6742 2023-06-06 20:48:58.033753 instawow-3.0.1/tests/fixtures/http/github-repo-molinari.json
+-rw-r--r--   0        0        0     5632 2023-06-06 20:49:03.327014 instawow-3.0.1/tests/fixtures/http/github-repo-no-release-json.json
+-rw-r--r--   0        0        0     6803 2023-06-06 20:49:07.571590 instawow-3.0.1/tests/fixtures/http/github-repo-no-releases.json
+-rw-r--r--   0        0        0     5536 2023-06-06 20:48:53.504470 instawow-3.0.1/tests/fixtures/http/github-repo-release-json.json
+-rwxr-xr-x   0        0        0     4183 2023-06-06 20:48:22.101303 instawow-3.0.1/tests/fixtures/http/regen.sh
+-rw-r--r--   0        0        0      769 2023-06-06 23:19:53.522108 instawow-3.0.1/tests/fixtures/http/tukui-ui--elvui.json
+-rw-r--r--   0        0        0      676 2023-06-06 23:20:04.298176 instawow-3.0.1/tests/fixtures/http/tukui-ui--tukui.json
+-rw-r--r--   0        0        0      938 2023-06-06 20:49:12.279530 instawow-3.0.1/tests/fixtures/http/wago-match-addons.json
+-rw-r--r--   0        0        0     3072 2023-06-06 20:48:49.124687 instawow-3.0.1/tests/fixtures/http/wowi-filedetails.json
+-rw-r--r--   0        0        0      930 2023-06-06 20:48:47.677451 instawow-3.0.1/tests/fixtures/http/wowi-filelist.json
+-rw-r--r--   0        0        0     1328 2023-05-29 18:35:35.550835 instawow-3.0.1/tests/plugin/instawow_test_plugin.py
+-rw-r--r--   0        0        0      276 2023-04-30 09:12:16.610136 instawow-3.0.1/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0     5553 2023-05-25 15:00:57.258425 instawow-3.0.1/tests/test__slpp.py
+-rw-r--r--   0        0        0     8500 2023-06-06 15:51:10.450525 instawow-3.0.1/tests/test__sources.py
+-rw-r--r--   0        0        0     3125 2023-06-10 11:16:29.545570 instawow-3.0.1/tests/test__version.py
+-rw-r--r--   0        0        0    17897 2023-06-06 20:51:58.192542 instawow-3.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1350 2023-05-19 22:19:41.380750 instawow-3.0.1/tests/test_common.py
+-rw-r--r--   0        0        0     3770 2023-06-10 11:20:20.064181 instawow-3.0.1/tests/test_config.py
+-rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-3.0.1/tests/test_github_oauth_flow.py
+-rw-r--r--   0        0        0     3033 2023-06-06 23:13:59.658917 instawow-3.0.1/tests/test_github_zip_parsing.py
+-rw-r--r--   0        0        0     4473 2023-06-08 14:41:42.827899 instawow-3.0.1/tests/test_json_rpc_api.py
+-rw-r--r--   0        0        0    13424 2023-06-06 20:53:39.204136 instawow-3.0.1/tests/test_manager.py
+-rw-r--r--   0        0        0     3935 2023-06-06 23:17:04.310471 instawow-3.0.1/tests/test_matchers.py
+-rw-r--r--   0        0        0     4491 2023-01-04 01:37:53.376282 instawow-3.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0     3487 2023-05-29 18:36:14.611876 instawow-3.0.1/tests/test_wa_updater.py
+-rw-r--r--   0        0        0     2029 2023-05-25 14:00:11.531683 instawow-3.0.1/tests/test_wow_installations.py
+-rw-r--r--   0        0        0     9568 1970-01-01 00:00:00.000000 instawow-3.0.1/PKG-INFO
```

### Comparing `instawow-3.0.0/CHANGELOG.rst` & `instawow-3.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/COPYING` & `instawow-3.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/README.rst` & `instawow-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/app.py` & `instawow-3.0.1/gui-webview/src/instawow_gui/app.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css` & `instawow-3.0.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.css`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js` & `instawow-3.0.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -30,15 +30,18 @@
     }
 
     function l(e, t) {
         return e != e ? t == t : e !== t
     }
 
     function u(t, ...r) {
-        if (null == t) return e;
+        if (null == t) {
+            for (const e of r) e(void 0);
+            return e
+        }
         const n = t.subscribe(...r);
         return n.unsubscribe ? () => n.unsubscribe() : n
     }
 
     function c(e, t, r) {
         e.$$.on_destroy.push(u(t, r))
     }
@@ -117,196 +120,201 @@
                 })
             })),
             abort() {
                 _.delete(t)
             }
         }
     }
-    const A = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
+    var A = "undefined" != typeof global ? global : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {};
+    const q = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : A;
 
-    function q(e, t) {
+    function E(e, t) {
         e.appendChild(t)
     }
 
-    function E(e) {
+    function T(e) {
         if (!e) return document;
         const t = e.getRootNode ? e.getRootNode() : e.ownerDocument;
         return t && t.host ? t : e.ownerDocument
     }
 
-    function T(e) {
-        const t = D("style");
-        return function(e, t) {
-            q(e.head || e, t), t.sheet
-        }(E(e), t), t.sheet
+    function $(e) {
+        const t = C("style");
+        return t.textContent = "/* empty */",
+            function(e, t) {
+                E(e.head || e, t), t.sheet
+            }(T(e), t), t.sheet
     }
 
-    function $(e, t, r) {
+    function O(e, t, r) {
         e.insertBefore(t, r || null)
     }
 
-    function O(e) {
+    function S(e) {
         e.parentNode && e.parentNode.removeChild(e)
     }
 
-    function S(e, t) {
+    function D(e, t) {
         for (let r = 0; r < e.length; r += 1) e[r] && e[r].d(t)
     }
 
-    function D(e) {
+    function C(e) {
         return document.createElement(e)
     }
 
-    function C(e) {
+    function R(e) {
         return document.createElementNS("http://www.w3.org/2000/svg", e)
     }
 
-    function R(e) {
+    function L(e) {
         return document.createTextNode(e)
     }
 
-    function L() {
-        return R(" ")
+    function N() {
+        return L(" ")
     }
 
-    function N() {
-        return R("")
+    function I() {
+        return L("")
     }
 
-    function I(e, t, r, n) {
+    function F(e, t, r, n) {
         return e.addEventListener(t, r, n), () => e.removeEventListener(t, r, n)
     }
 
-    function F(e) {
+    function M(e) {
         return function(t) {
             return t.preventDefault(), e.call(this, t)
         }
     }
 
-    function M(e) {
+    function P(e) {
         return function(t) {
             return t.stopPropagation(), e.call(this, t)
         }
     }
 
-    function P(e, t, r) {
+    function j(e, t, r) {
         null == r ? e.removeAttribute(t) : e.getAttribute(t) !== r && e.setAttribute(t, r)
     }
 
-    function j(e, t) {
-        for (const r in t) P(e, r, t[r])
+    function B(e, t) {
+        for (const r in t) j(e, r, t[r])
     }
 
-    function B(e) {
+    function U(e) {
         let t;
         return {
             p(...r) {
                 t = r, t.forEach((t => e.push(t)))
             },
             r() {
                 t.forEach((t => e.splice(e.indexOf(t), 1)))
             }
         }
     }
 
-    function U(e, t) {
+    function V(e, t) {
         t = "" + t, e.data !== t && (e.data = t)
     }
 
-    function V(e, t) {
+    function z(e, t) {
         e.value = null == t ? "" : t
     }
 
-    function z(e, t, r) {
+    function H(e, t, r) {
         for (let r = 0; r < e.options.length; r += 1) {
             const n = e.options[r];
             if (n.__value === t) return void(n.selected = !0)
         }
         r && void 0 === t || (e.selectedIndex = -1)
     }
 
-    function H(e, t) {
+    function W(e, t) {
         for (let r = 0; r < e.options.length; r += 1) {
             const n = e.options[r];
             n.selected = ~t.indexOf(n.__value)
         }
     }
 
-    function W(e) {
+    function G(e) {
         const t = e.querySelector(":checked");
         return t && t.__value
     }
-    let G;
+    let Z;
 
-    function Z() {
-        if (void 0 === G) {
-            G = !1;
+    function J() {
+        if (void 0 === Z) {
+            Z = !1;
             try {
                 "undefined" != typeof window && window.parent && window.parent.document
             } catch (e) {
-                G = !0
+                Z = !0
             }
         }
-        return G
+        return Z
     }
 
-    function J(e, t, r) {
-        e.classList[r ? "add" : "remove"](t)
+    function Y(e, t, r) {
+        e.classList.toggle(t, !!r)
     }
 
-    function Y(e, t, {
+    function K(e, t, {
         bubbles: r = !1,
         cancelable: n = !1
     } = {}) {
-        const i = document.createEvent("CustomEvent");
-        return i.initCustomEvent(e, r, n, t), i
+        return new CustomEvent(e, {
+            detail: t,
+            bubbles: r,
+            cancelable: n
+        })
     }
-    const K = new Map;
-    let X, Q = 0;
+    const X = new Map;
+    let Q, ee = 0;
 
-    function ee(e, t, r, n, i, o, s, a = 0) {
+    function te(e, t, r, n, i, o, s, a = 0) {
         const l = 16.666 / n;
         let u = "{\n";
         for (let e = 0; e <= 1; e += l) {
             const n = t + (r - t) * o(e);
             u += 100 * e + `%{${s(n,1-n)}}\n`
         }
         const c = u + `100% {${s(r,1-r)}}\n}`,
             f = `__svelte_${function(e){let t=5381,r=e.length;for(;r--;)t=(t<<5)-t^e.charCodeAt(r);return t>>>0}(c)}_${a}`,
-            h = E(e),
+            h = T(e),
             {
                 stylesheet: p,
                 rules: d
-            } = K.get(h) || function(e, t) {
+            } = X.get(h) || function(e, t) {
                 const r = {
-                    stylesheet: T(t),
+                    stylesheet: $(t),
                     rules: {}
                 };
-                return K.set(e, r), r
+                return X.set(e, r), r
             }(h, e);
         d[f] || (d[f] = !0, p.insertRule(`@keyframes ${f} ${c}`, p.cssRules.length));
         const m = e.style.animation || "";
-        return e.style.animation = `${m?`${m}, `:""}${f} ${n}ms linear ${i}ms 1 both`, Q += 1, f
+        return e.style.animation = `${m?`${m}, `:""}${f} ${n}ms linear ${i}ms 1 both`, ee += 1, f
     }
 
-    function te(e, t) {
+    function re(e, t) {
         const r = (e.style.animation || "").split(", "),
             n = r.filter(t ? e => e.indexOf(t) < 0 : e => -1 === e.indexOf("__svelte")),
             i = r.length - n.length;
-        i && (e.style.animation = n.join(", "), Q -= i, Q || w((() => {
-            Q || (K.forEach((e => {
+        i && (e.style.animation = n.join(", "), ee -= i, ee || w((() => {
+            ee || (X.forEach((e => {
                 const {
                     ownerNode: t
                 } = e.stylesheet;
-                t && O(t)
-            })), K.clear())
+                t && S(t)
+            })), X.clear())
         })))
     }
 
-    function re(e) {
+    function ne(e) {
         const t = getComputedStyle(e);
         if ("absolute" !== t.position && "fixed" !== t.position) {
             const {
                 width: r,
                 height: n
             } = t, i = e.getBoundingClientRect();
             e.style.position = "absolute", e.style.width = r, e.style.height = n,
@@ -317,205 +325,204 @@
                             i = "none" === n.transform ? "" : n.transform;
                         e.style.transform = `${i} translate(${t.left-r.left}px, ${t.top-r.top}px)`
                     }
                 }(e, i)
         }
     }
 
-    function ne(e) {
-        X = e
+    function ie(e) {
+        Q = e
     }
 
-    function ie() {
-        if (!X) throw new Error("Function called outside component initialization");
-        return X
+    function oe() {
+        if (!Q) throw new Error("Function called outside component initialization");
+        return Q
     }
 
-    function oe(e) {
-        ie().$$.on_mount.push(e)
+    function se(e) {
+        oe().$$.on_mount.push(e)
     }
 
-    function se() {
-        const e = ie();
+    function ae() {
+        const e = oe();
         return (t, r, {
             cancelable: n = !1
         } = {}) => {
             const i = e.$$.callbacks[t];
             if (i) {
-                const o = Y(t, r, {
+                const o = K(t, r, {
                     cancelable: n
                 });
                 return i.slice().forEach((t => {
                     t.call(e, o)
                 })), !o.defaultPrevented
             }
             return !0
         }
     }
 
-    function ae(e, t) {
-        return ie().$$.context.set(e, t), t
+    function le(e, t) {
+        return oe().$$.context.set(e, t), t
     }
 
-    function le(e) {
-        return ie().$$.context.get(e)
+    function ue(e) {
+        return oe().$$.context.get(e)
     }
 
-    function ue(e, t) {
+    function ce(e, t) {
         const r = e.$$.callbacks[t.type];
         r && r.slice().forEach((e => e.call(this, t)))
     }
-    const ce = [],
-        fe = [];
-    let he = [];
-    const pe = [],
-        de = Promise.resolve();
-    let me = !1;
-
-    function ge(e) {
-        he.push(e)
-    }
+    const fe = [],
+        he = [];
+    let pe = [];
+    const de = [],
+        me = Promise.resolve();
+    let ge = !1;
 
     function ve(e) {
         pe.push(e)
     }
-    const ye = new Set;
-    let be, we = 0;
 
-    function _e() {
-        if (0 !== we) return;
-        const e = X;
+    function ye(e) {
+        de.push(e)
+    }
+    const be = new Set;
+    let we, _e = 0;
+
+    function ke() {
+        if (0 !== _e) return;
+        const e = Q;
         do {
             try {
-                for (; we < ce.length;) {
-                    const e = ce[we];
-                    we++, ne(e), ke(e.$$)
+                for (; _e < fe.length;) {
+                    const e = fe[_e];
+                    _e++, ie(e), xe(e.$$)
                 }
             } catch (e) {
-                throw ce.length = 0, we = 0, e
+                throw fe.length = 0, _e = 0, e
             }
-            for (ne(null), ce.length = 0, we = 0; fe.length;) fe.pop()();
-            for (let e = 0; e < he.length; e += 1) {
-                const t = he[e];
-                ye.has(t) || (ye.add(t), t())
+            for (ie(null), fe.length = 0, _e = 0; he.length;) he.pop()();
+            for (let e = 0; e < pe.length; e += 1) {
+                const t = pe[e];
+                be.has(t) || (be.add(t), t())
             }
-            he.length = 0
-        } while (ce.length);
-        for (; pe.length;) pe.pop()();
-        me = !1, ye.clear(), ne(e)
+            pe.length = 0
+        } while (fe.length);
+        for (; de.length;) de.pop()();
+        ge = !1, be.clear(), ie(e)
     }
 
-    function ke(e) {
+    function xe(e) {
         if (null !== e.fragment) {
             e.update(), o(e.before_update);
             const t = e.dirty;
-            e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(ge)
+            e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(ve)
         }
     }
 
-    function xe() {
-        return be || (be = Promise.resolve(), be.then((() => {
-            be = null
-        }))), be
+    function Ae() {
+        return we || (we = Promise.resolve(), we.then((() => {
+            we = null
+        }))), we
     }
 
-    function Ae(e, t, r) {
-        e.dispatchEvent(Y(`${t?"intro":"outro"}${r}`))
+    function qe(e, t, r) {
+        e.dispatchEvent(K(`${t?"intro":"outro"}${r}`))
     }
-    const qe = new Set;
-    let Ee;
+    const Ee = new Set;
+    let Te;
 
-    function Te() {
-        Ee = {
+    function $e() {
+        Te = {
             r: 0,
             c: [],
-            p: Ee
+            p: Te
         }
     }
 
-    function $e() {
-        Ee.r || o(Ee.c), Ee = Ee.p
+    function Oe() {
+        Te.r || o(Te.c), Te = Te.p
     }
 
-    function Oe(e, t) {
-        e && e.i && (qe.delete(e), e.i(t))
+    function Se(e, t) {
+        e && e.i && (Ee.delete(e), e.i(t))
     }
 
-    function Se(e, t, r, n) {
+    function De(e, t, r, n) {
         if (e && e.o) {
-            if (qe.has(e)) return;
-            qe.add(e), Ee.c.push((() => {
-                qe.delete(e), n && (r && e.d(1), n())
+            if (Ee.has(e)) return;
+            Ee.add(e), Te.c.push((() => {
+                Ee.delete(e), n && (r && e.d(1), n())
             })), e.o(t)
         } else n && n()
     }
-    const De = {
+    const Ce = {
         duration: 0
     };
 
-    function Ce(r, n, i) {
+    function Re(r, n, i) {
         const o = {
             direction: "in"
         };
         let a, l, u = n(r, i, o),
             c = !1,
             f = 0;
 
         function h() {
-            a && te(r, a)
+            a && re(r, a)
         }
 
         function p() {
             const {
                 delay: n = 0,
                 duration: i = 300,
                 easing: o = t,
                 tick: s = e,
                 css: p
-            } = u || De;
-            p && (a = ee(r, 0, 1, i, n, o, p, f++)), s(0, 1);
+            } = u || Ce;
+            p && (a = te(r, 0, 1, i, n, o, p, f++)), s(0, 1);
             const d = b() + n,
                 m = d + i;
-            l && l.abort(), c = !0, ge((() => Ae(r, !0, "start"))), l = x((e => {
+            l && l.abort(), c = !0, ve((() => qe(r, !0, "start"))), l = x((e => {
                 if (c) {
-                    if (e >= m) return s(1, 0), Ae(r, !0, "end"), h(), c = !1;
+                    if (e >= m) return s(1, 0), qe(r, !0, "end"), h(), c = !1;
                     if (e >= d) {
                         const t = o((e - d) / i);
                         s(t, 1 - t)
                     }
                 }
                 return c
             }))
         }
         let d = !1;
         return {
             start() {
-                d || (d = !0, te(r), s(u) ? (u = u(o), xe().then(p)) : p())
+                d || (d = !0, re(r), s(u) ? (u = u(o), Ae().then(p)) : p())
             },
             invalidate() {
                 d = !1
             },
             end() {
                 c && (h(), c = !1)
             }
         }
     }
 
-    function Re(r, n, i, a) {
-        const l = {
-            direction: "both"
-        };
-        let u = n(r, i, l),
+    function Le(r, n, i, a) {
+        let l, u = n(r, i, {
+                direction: "both"
+            }),
             c = a ? 0 : 1,
             f = null,
             h = null,
             p = null;
 
         function d() {
-            p && te(r, p)
+            p && re(r, p)
         }
 
         function m(e, t) {
             const r = e.b - c;
             return t *= Math.abs(r), {
                 a: c,
                 b: e.b,
@@ -528,95 +535,101 @@
         }
 
         function g(n) {
             const {
                 delay: i = 0,
                 duration: s = 300,
                 easing: a = t,
-                tick: l = e,
-                css: g
-            } = u || De, v = {
+                tick: g = e,
+                css: v
+            } = u || Ce, y = {
                 start: b() + i,
                 b: n
             };
-            n || (v.group = Ee, Ee.r += 1), f || h ? h = v : (g && (d(), p = ee(r, c, n, s, i, a, g)), n && l(0, 1), f = m(v, s), ge((() => Ae(r, n, "start"))), x((e => {
-                if (h && e > h.start && (f = m(h, s), h = null, Ae(r, f.b, "start"), g && (d(), p = ee(r, c, f.b, f.duration, 0, a, u.css))), f)
-                    if (e >= f.end) l(c = f.b, 1 - c), Ae(r, f.b, "end"), h || (f.b ? d() : --f.group.r || o(f.group.c)), f = null;
+            n || (y.group = Te, Te.r += 1), "inert" in r && (n ? void 0 !== l && (r.inert = l) : (l = r.inert, r.inert = !0)), f || h ? h = y : (v && (d(), p = te(r, c, n, s, i, a, v)), n && g(0, 1), f = m(y, s), ve((() => qe(r, n, "start"))), x((e => {
+                if (h && e > h.start && (f = m(h, s), h = null, qe(r, f.b, "start"), v && (d(), p = te(r, c, f.b, f.duration, 0, a, u.css))), f)
+                    if (e >= f.end) g(c = f.b, 1 - c), qe(r, f.b, "end"), h || (f.b ? d() : --f.group.r || o(f.group.c)), f = null;
                     else if (e >= f.start) {
                     const t = e - f.start;
-                    c = f.a + f.d * a(t / f.duration), l(c, 1 - c)
+                    c = f.a + f.d * a(t / f.duration), g(c, 1 - c)
                 }
                 return !(!f && !h)
             })))
         }
         return {
             run(e) {
-                s(u) ? xe().then((() => {
-                    u = u(l), g(e)
+                s(u) ? Ae().then((() => {
+                    u = u({
+                        direction: e ? "in" : "out"
+                    }), g(e)
                 })) : g(e)
             },
             end() {
                 d(), f = h = null
             }
         }
     }
 
-    function Le(e, t) {
+    function Ne(e, t) {
         const r = t.token = {};
 
         function n(e, n, i, o) {
             if (t.token !== r) return;
             t.resolved = o;
             let s = t.ctx;
             void 0 !== i && (s = s.slice(), s[i] = o);
             const a = e && (t.current = e)(s);
             let l = !1;
             t.block && (t.blocks ? t.blocks.forEach(((e, r) => {
-                r !== n && e && (Te(), Se(e, 1, 1, (() => {
+                r !== n && e && ($e(), De(e, 1, 1, (() => {
                     t.blocks[r] === e && (t.blocks[r] = null)
-                })), $e())
-            })) : t.block.d(1), a.c(), Oe(a, 1), a.m(t.mount(), t.anchor), l = !0), t.block = a, t.blocks && (t.blocks[n] = a), l && _e()
+                })), Oe())
+            })) : t.block.d(1), a.c(), Se(a, 1), a.m(t.mount(), t.anchor), l = !0), t.block = a, t.blocks && (t.blocks[n] = a), l && ke()
         }
         if (!(i = e) || "object" != typeof i && "function" != typeof i || "function" != typeof i.then) {
             if (t.current !== t.then) return n(t.then, 1, t.value, e), !0;
             t.resolved = e
         } else {
-            const r = ie();
+            const r = oe();
             if (e.then((e => {
-                    ne(r), n(t.then, 1, t.value, e), ne(null)
+                    ie(r), n(t.then, 1, t.value, e), ie(null)
                 }), (e => {
-                    if (ne(r), n(t.catch, 2, t.error, e), ne(null), !t.hasCatch) throw e
+                    if (ie(r), n(t.catch, 2, t.error, e), ie(null), !t.hasCatch) throw e
                 })), t.current !== t.pending) return n(t.pending, 0), !0
         }
         var i
     }
 
-    function Ne(e, t, r) {
+    function Ie(e, t, r) {
         const n = t.slice(),
             {
                 resolved: i
             } = e;
         e.current === e.then && (n[e.value] = i), e.current === e.catch && (n[e.error] = i), e.block.p(n, r)
     }
 
-    function Ie(e, t) {
+    function Fe(e) {
+        return void 0 !== e?.length ? e : Array.from(e)
+    }
+
+    function Me(e, t) {
         e.d(1), t.delete(e.key)
     }
 
-    function Fe(e, t) {
-        Se(e, 1, 1, (() => {
+    function Pe(e, t) {
+        De(e, 1, 1, (() => {
             t.delete(e.key)
         }))
     }
 
-    function Me(e, t) {
-        e.f(), Fe(e, t)
+    function je(e, t) {
+        e.f(), Pe(e, t)
     }
 
-    function Pe(e, t, r, n, i, s, a, l, u, c, f, h) {
+    function Be(e, t, r, n, i, s, a, l, u, c, f, h) {
         let p = e.length,
             d = s.length,
             m = p;
         const g = {};
         for (; m--;) g[e[m].key] = m;
         const v = [],
             y = new Map,
@@ -628,15 +641,15 @@
             let l = a.get(o);
             l ? n && w.push((() => l.p(e, t))) : (l = c(o, e), l.c()), y.set(o, v[m] = l), o in g && b.set(o, Math.abs(m - g[o]))
         }
         const _ = new Set,
             k = new Set;
 
         function x(e) {
-            Oe(e, 1), e.m(l, f), a.set(e.key, e), f = e.first, d--
+            Se(e, 1), e.m(l, f), a.set(e.key, e), f = e.first, d--
         }
         for (; p && d;) {
             const t = v[d - 1],
                 r = e[p - 1],
                 n = t.key,
                 i = r.key;
             t === r ? (f = t.first, p--, d--) : y.has(i) ? !a.has(n) || _.has(n) ? x(t) : k.has(i) ? p-- : b.get(n) > b.get(i) ? (k.add(n), x(t)) : (_.add(i), p--) : (u(r, a), p--)
@@ -645,15 +658,15 @@
             const t = e[p];
             y.has(t.key) || u(t, a)
         }
         for (; d;) x(v[d - 1]);
         return o(w), v
     }
 
-    function je(e, t) {
+    function Ue(e, t) {
         const r = {},
             n = {},
             i = {
                 $$scope: 1
             };
         let o = e.length;
         for (; o--;) {
@@ -666,54 +679,54 @@
             } else
                 for (const e in s) i[e] = 1
         }
         for (const e in n) e in r || (r[e] = void 0);
         return r
     }
 
-    function Be(e) {
+    function Ve(e) {
         return "object" == typeof e && null !== e ? e : {}
     }
 
-    function Ue(e, t, r) {
+    function ze(e, t, r) {
         const n = e.$$.props[t];
         void 0 !== n && (e.$$.bound[n] = r, r(e.$$.ctx[n]))
     }
 
-    function Ve(e) {
+    function He(e) {
         e && e.c()
     }
 
-    function ze(e, t, r, i) {
+    function We(e, t, r) {
         const {
-            fragment: a,
-            after_update: l
+            fragment: i,
+            after_update: a
         } = e.$$;
-        a && a.m(t, r), i || ge((() => {
+        i && i.m(t, r), ve((() => {
             const t = e.$$.on_mount.map(n).filter(s);
             e.$$.on_destroy ? e.$$.on_destroy.push(...t) : o(t), e.$$.on_mount = []
-        })), l.forEach(ge)
+        })), a.forEach(ve)
     }
 
-    function He(e, t) {
+    function Ge(e, t) {
         const r = e.$$;
         null !== r.fragment && (! function(e) {
             const t = [],
                 r = [];
-            he.forEach((n => -1 === e.indexOf(n) ? t.push(n) : r.push(n))), r.forEach((e => e())), he = t
+            pe.forEach((n => -1 === e.indexOf(n) ? t.push(n) : r.push(n))), r.forEach((e => e())), pe = t
         }(r.after_update), o(r.on_destroy), r.fragment && r.fragment.d(t), r.on_destroy = r.fragment = null, r.ctx = [])
     }
 
-    function We(e, t) {
-        -1 === e.$$.dirty[0] && (ce.push(e), me || (me = !0, de.then(_e)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
+    function Ze(e, t) {
+        -1 === e.$$.dirty[0] && (fe.push(e), ge || (ge = !0, me.then(ke)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
     }
 
-    function Ge(t, r, n, s, a, l, u, c = [-1]) {
-        const f = X;
-        ne(t);
+    function Je(t, r, n, s, a, l, u, c = [-1]) {
+        const f = Q;
+        ie(t);
         const h = t.$$ = {
             fragment: null,
             ctx: [],
             props: l,
             update: e,
             not_equal: a,
             bound: i(),
@@ -728,66 +741,68 @@
             skip_bound: !1,
             root: r.target || f.$$.root
         };
         u && u(h.root);
         let p = !1;
         if (h.ctx = n ? n(t, r.props || {}, ((e, r, ...n) => {
                 const i = n.length ? n[0] : r;
-                return h.ctx && a(h.ctx[e], h.ctx[e] = i) && (!h.skip_bound && h.bound[e] && h.bound[e](i), p && We(t, e)), r
+                return h.ctx && a(h.ctx[e], h.ctx[e] = i) && (!h.skip_bound && h.bound[e] && h.bound[e](i), p && Ze(t, e)), r
             })) : [], h.update(), p = !0, o(h.before_update), h.fragment = !!s && s(h.ctx), r.target) {
             if (r.hydrate) {
                 const e = function(e) {
                     return Array.from(e.childNodes)
                 }(r.target);
-                h.fragment && h.fragment.l(e), e.forEach(O)
+                h.fragment && h.fragment.l(e), e.forEach(S)
             } else h.fragment && h.fragment.c();
-            r.intro && Oe(t.$$.fragment), ze(t, r.target, r.anchor, r.customElement), _e()
+            r.intro && Se(t.$$.fragment), We(t, r.target, r.anchor), ke()
         }
-        ne(f)
+        ie(f)
     }
-    class Ze {
+    class Ye {
+        $$ = void 0;
+        $$set = void 0;
         $destroy() {
-            He(this, 1), this.$destroy = e
+            Ge(this, 1), this.$destroy = e
         }
         $on(t, r) {
             if (!s(r)) return e;
             const n = this.$$.callbacks[t] || (this.$$.callbacks[t] = []);
             return n.push(r), () => {
                 const e = n.indexOf(r); - 1 !== e && n.splice(e, 1)
             }
         }
         $set(e) {
             var t;
             this.$$set && (t = e, 0 !== Object.keys(t).length) && (this.$$.skip_bound = !0, this.$$set(e), this.$$.skip_bound = !1)
         }
     }
 
-    function Je(e) {
+    function Ke(e) {
         const t = e - 1;
         return t * t * t + 1
     }
 
-    function Ye(e, {
+    function Xe(e, {
         delay: r = 0,
         duration: n = 400,
         easing: i = t
     } = {}) {
         const o = +getComputedStyle(e).opacity;
         return {
             delay: r,
             duration: n,
             easing: i,
             css: e => "opacity: " + e * o
         }
     }
 
-    function Ke(e, {
+    function Qe(e, {
         delay: t = 0,
         duration: r = 400,
-        easing: n = Je,
+        easing: n = Ke,
         axis: i = "y"
     } = {}) {
         const o = getComputedStyle(e),
             s = +o.opacity,
             a = "y" === i ? "height" : "width",
             l = parseFloat(o[a]),
             u = "y" === i ? ["top", "bottom"] : ["left", "right"],
@@ -802,18 +817,18 @@
             delay: t,
             duration: r,
             easing: n,
             css: e => `overflow: hidden;opacity: ${Math.min(20*e,1)*s};${a}: ${e*l}px;padding-${u[0]}: ${e*f}px;padding-${u[1]}: ${e*h}px;margin-${u[0]}: ${e*p}px;margin-${u[1]}: ${e*d}px;border-${u[0]}-width: ${e*m}px;border-${u[1]}-width: ${e*g}px;`
         }
     }
 
-    function Xe(e, {
+    function et(e, {
         delay: t = 0,
         duration: r = 400,
-        easing: n = Je,
+        easing: n = Ke,
         start: i = 0,
         opacity: o = 0
     } = {}) {
         const s = getComputedStyle(e),
             a = +s.opacity,
             l = "none" === s.transform ? "" : s.transform,
             u = 1 - i,
@@ -821,57 +836,63 @@
         return {
             delay: t,
             duration: r,
             easing: n,
             css: (e, t) => `\n\t\t\ttransform: ${l} scale(${1-u*t});\n\t\t\topacity: ${a-c*t}\n\t\t`
         }
     }
-    const Qe = [];
+    "undefined" != typeof window && (window.__svelte || (window.__svelte = {
+        v: new Set
+    })).v.add("4");
+    const tt = [];
 
-    function et(t, r = e) {
+    function rt(t, r = e) {
         let n;
         const i = new Set;
 
         function o(e) {
             if (a(t, e) && (t = e, n)) {
-                const e = !Qe.length;
-                for (const e of i) e[1](), Qe.push(e, t);
+                const e = !tt.length;
+                for (const e of i) e[1](), tt.push(e, t);
                 if (e) {
-                    for (let e = 0; e < Qe.length; e += 2) Qe[e][0](Qe[e + 1]);
-                    Qe.length = 0
+                    for (let e = 0; e < tt.length; e += 2) tt[e][0](tt[e + 1]);
+                    tt.length = 0
                 }
             }
         }
+
+        function s(e) {
+            o(e(t))
+        }
         return {
             set: o,
-            update: function(e) {
-                o(e(t))
-            },
-            subscribe: function(s, a = e) {
-                const l = [s, a];
-                return i.add(l), 1 === i.size && (n = r(o) || e), s(t), () => {
-                    i.delete(l), 0 === i.size && n && (n(), n = null)
+            update: s,
+            subscribe: function(a, l = e) {
+                const u = [a, l];
+                return i.add(u), 1 === i.size && (n = r(o, s) || e), a(t), () => {
+                    i.delete(u), 0 === i.size && n && (n(), n = null)
                 }
             }
         }
     }
-    const tt = et({});
+    const nt = rt({});
 
-    function rt(e, t, r, n) {
+    function it(e, t, r, n) {
         if ("a" === r && !n) throw new TypeError("Private accessor was defined without a getter");
         if ("function" == typeof t ? e !== t || !n : !t.has(e)) throw new TypeError("Cannot read private member from an object whose class did not declare it");
         return "m" === r ? n : "a" === r ? n.call(e) : n ? n.value : t.get(e)
     }
-    var nt = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
+    "function" == typeof SuppressedError && SuppressedError;
+    var ot = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
 
-    function it(e) {
+    function st(e) {
         return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e
     }
 
-    function ot(e) {
+    function at(e) {
         if (e.__esModule) return e;
         var t = e.default;
         if ("function" == typeof t) {
             var r = function e() {
                 if (this instanceof e) {
                     var r = [null];
                     return r.push.apply(r, arguments), new(Function.bind.apply(t, r))
@@ -888,71 +909,71 @@
                 enumerable: !0,
                 get: function() {
                     return e[t]
                 }
             })
         })), r
     }
-    var st = {},
-        at = {};
+    var lt = {},
+        ut = {};
 
-    function lt() {}
+    function ct() {}
 
-    function ut() {
-        ut.init.call(this)
+    function ft() {
+        ft.init.call(this)
     }
 
-    function ct(e) {
-        return void 0 === e._maxListeners ? ut.defaultMaxListeners : e._maxListeners
+    function ht(e) {
+        return void 0 === e._maxListeners ? ft.defaultMaxListeners : e._maxListeners
     }
 
-    function ft(e, t, r, n) {
+    function pt(e, t, r, n) {
         var i, o, s, a;
         if ("function" != typeof r) throw new TypeError('"listener" argument must be a function');
-        if ((o = e._events) ? (o.newListener && (e.emit("newListener", t, r.listener ? r.listener : r), o = e._events), s = o[t]) : (o = e._events = new lt, e._eventsCount = 0), s) {
-            if ("function" == typeof s ? s = o[t] = n ? [r, s] : [s, r] : n ? s.unshift(r) : s.push(r), !s.warned && (i = ct(e)) && i > 0 && s.length > i) {
+        if ((o = e._events) ? (o.newListener && (e.emit("newListener", t, r.listener ? r.listener : r), o = e._events), s = o[t]) : (o = e._events = new ct, e._eventsCount = 0), s) {
+            if ("function" == typeof s ? s = o[t] = n ? [r, s] : [s, r] : n ? s.unshift(r) : s.push(r), !s.warned && (i = ht(e)) && i > 0 && s.length > i) {
                 s.warned = !0;
                 var l = new Error("Possible EventEmitter memory leak detected. " + s.length + " " + t + " listeners added. Use emitter.setMaxListeners() to increase limit");
                 l.name = "MaxListenersExceededWarning", l.emitter = e, l.type = t, l.count = s.length, a = l, "function" == typeof console.warn ? console.warn(a) : console.log(a)
             }
         } else s = o[t] = r, ++e._eventsCount;
         return e
     }
 
-    function ht(e, t, r) {
+    function dt(e, t, r) {
         var n = !1;
 
         function i() {
             e.removeListener(t, i), n || (n = !0, r.apply(e, arguments))
         }
         return i.listener = r, i
     }
 
-    function pt(e) {
+    function mt(e) {
         var t = this._events;
         if (t) {
             var r = t[e];
             if ("function" == typeof r) return 1;
             if (r) return r.length
         }
         return 0
     }
 
-    function dt(e, t) {
+    function gt(e, t) {
         for (var r = new Array(t); t--;) r[t] = e[t];
         return r
     }
-    lt.prototype = Object.create(null), ut.EventEmitter = ut, ut.usingDomains = !1, ut.prototype.domain = void 0, ut.prototype._events = void 0, ut.prototype._maxListeners = void 0, ut.defaultMaxListeners = 10, ut.init = function() {
-        this.domain = null, ut.usingDomains && undefined.active, this._events && this._events !== Object.getPrototypeOf(this)._events || (this._events = new lt, this._eventsCount = 0), this._maxListeners = this._maxListeners || void 0
-    }, ut.prototype.setMaxListeners = function(e) {
+    ct.prototype = Object.create(null), ft.EventEmitter = ft, ft.usingDomains = !1, ft.prototype.domain = void 0, ft.prototype._events = void 0, ft.prototype._maxListeners = void 0, ft.defaultMaxListeners = 10, ft.init = function() {
+        this.domain = null, ft.usingDomains && undefined.active, this._events && this._events !== Object.getPrototypeOf(this)._events || (this._events = new ct, this._eventsCount = 0), this._maxListeners = this._maxListeners || void 0
+    }, ft.prototype.setMaxListeners = function(e) {
         if ("number" != typeof e || e < 0 || isNaN(e)) throw new TypeError('"n" argument must be a positive number');
         return this._maxListeners = e, this
-    }, ut.prototype.getMaxListeners = function() {
-        return ct(this)
-    }, ut.prototype.emit = function(e) {
+    }, ft.prototype.getMaxListeners = function() {
+        return ht(this)
+    }, ft.prototype.emit = function(e) {
         var t, r, n, i, o, s, a, l = "error" === e;
         if (s = this._events) l = l && null == s.error;
         else if (!l) return !1;
         if (a = this.domain, l) {
             if (t = arguments[1], !a) {
                 if (t instanceof Error) throw t;
                 var u = new Error('Uncaught, unspecified "error" event. (' + t + ")");
@@ -963,113 +984,113 @@
         if (!(r = s[e])) return !1;
         var c = "function" == typeof r;
         switch (n = arguments.length) {
             case 1:
                 ! function(e, t, r) {
                     if (t) e.call(r);
                     else
-                        for (var n = e.length, i = dt(e, n), o = 0; o < n; ++o) i[o].call(r)
+                        for (var n = e.length, i = gt(e, n), o = 0; o < n; ++o) i[o].call(r)
                 }(r, c, this);
                 break;
             case 2:
                 ! function(e, t, r, n) {
                     if (t) e.call(r, n);
                     else
-                        for (var i = e.length, o = dt(e, i), s = 0; s < i; ++s) o[s].call(r, n)
+                        for (var i = e.length, o = gt(e, i), s = 0; s < i; ++s) o[s].call(r, n)
                 }(r, c, this, arguments[1]);
                 break;
             case 3:
                 ! function(e, t, r, n, i) {
                     if (t) e.call(r, n, i);
                     else
-                        for (var o = e.length, s = dt(e, o), a = 0; a < o; ++a) s[a].call(r, n, i)
+                        for (var o = e.length, s = gt(e, o), a = 0; a < o; ++a) s[a].call(r, n, i)
                 }(r, c, this, arguments[1], arguments[2]);
                 break;
             case 4:
                 ! function(e, t, r, n, i, o) {
                     if (t) e.call(r, n, i, o);
                     else
-                        for (var s = e.length, a = dt(e, s), l = 0; l < s; ++l) a[l].call(r, n, i, o)
+                        for (var s = e.length, a = gt(e, s), l = 0; l < s; ++l) a[l].call(r, n, i, o)
                 }(r, c, this, arguments[1], arguments[2], arguments[3]);
                 break;
             default:
                 for (i = new Array(n - 1), o = 1; o < n; o++) i[o - 1] = arguments[o];
                 ! function(e, t, r, n) {
                     if (t) e.apply(r, n);
                     else
-                        for (var i = e.length, o = dt(e, i), s = 0; s < i; ++s) o[s].apply(r, n)
+                        for (var i = e.length, o = gt(e, i), s = 0; s < i; ++s) o[s].apply(r, n)
                 }(r, c, this, i)
         }
         return !0
-    }, ut.prototype.addListener = function(e, t) {
-        return ft(this, e, t, !1)
-    }, ut.prototype.on = ut.prototype.addListener, ut.prototype.prependListener = function(e, t) {
-        return ft(this, e, t, !0)
-    }, ut.prototype.once = function(e, t) {
+    }, ft.prototype.addListener = function(e, t) {
+        return pt(this, e, t, !1)
+    }, ft.prototype.on = ft.prototype.addListener, ft.prototype.prependListener = function(e, t) {
+        return pt(this, e, t, !0)
+    }, ft.prototype.once = function(e, t) {
         if ("function" != typeof t) throw new TypeError('"listener" argument must be a function');
-        return this.on(e, ht(this, e, t)), this
-    }, ut.prototype.prependOnceListener = function(e, t) {
+        return this.on(e, dt(this, e, t)), this
+    }, ft.prototype.prependOnceListener = function(e, t) {
         if ("function" != typeof t) throw new TypeError('"listener" argument must be a function');
-        return this.prependListener(e, ht(this, e, t)), this
-    }, ut.prototype.removeListener = function(e, t) {
+        return this.prependListener(e, dt(this, e, t)), this
+    }, ft.prototype.removeListener = function(e, t) {
         var r, n, i, o, s;
         if ("function" != typeof t) throw new TypeError('"listener" argument must be a function');
         if (!(n = this._events)) return this;
         if (!(r = n[e])) return this;
-        if (r === t || r.listener && r.listener === t) 0 == --this._eventsCount ? this._events = new lt : (delete n[e], n.removeListener && this.emit("removeListener", e, r.listener || t));
+        if (r === t || r.listener && r.listener === t) 0 == --this._eventsCount ? this._events = new ct : (delete n[e], n.removeListener && this.emit("removeListener", e, r.listener || t));
         else if ("function" != typeof r) {
             for (i = -1, o = r.length; o-- > 0;)
                 if (r[o] === t || r[o].listener && r[o].listener === t) {
                     s = r[o].listener, i = o;
                     break
                 } if (i < 0) return this;
             if (1 === r.length) {
-                if (r[0] = void 0, 0 == --this._eventsCount) return this._events = new lt, this;
+                if (r[0] = void 0, 0 == --this._eventsCount) return this._events = new ct, this;
                 delete n[e]
             } else ! function(e, t) {
                 for (var r = t, n = r + 1, i = e.length; n < i; r += 1, n += 1) e[r] = e[n];
                 e.pop()
             }(r, i);
             n.removeListener && this.emit("removeListener", e, s || t)
         }
         return this
-    }, ut.prototype.off = function(e, t) {
+    }, ft.prototype.off = function(e, t) {
         return this.removeListener(e, t)
-    }, ut.prototype.removeAllListeners = function(e) {
+    }, ft.prototype.removeAllListeners = function(e) {
         var t, r;
         if (!(r = this._events)) return this;
-        if (!r.removeListener) return 0 === arguments.length ? (this._events = new lt, this._eventsCount = 0) : r[e] && (0 == --this._eventsCount ? this._events = new lt : delete r[e]), this;
+        if (!r.removeListener) return 0 === arguments.length ? (this._events = new ct, this._eventsCount = 0) : r[e] && (0 == --this._eventsCount ? this._events = new ct : delete r[e]), this;
         if (0 === arguments.length) {
             for (var n, i = Object.keys(r), o = 0; o < i.length; ++o) "removeListener" !== (n = i[o]) && this.removeAllListeners(n);
-            return this.removeAllListeners("removeListener"), this._events = new lt, this._eventsCount = 0, this
+            return this.removeAllListeners("removeListener"), this._events = new ct, this._eventsCount = 0, this
         }
         if ("function" == typeof(t = r[e])) this.removeListener(e, t);
         else if (t)
             do {
                 this.removeListener(e, t[t.length - 1])
             } while (t[0]);
         return this
-    }, ut.prototype.listeners = function(e) {
+    }, ft.prototype.listeners = function(e) {
         var t, r = this._events;
         return r && (t = r[e]) ? "function" == typeof t ? [t.listener || t] : function(e) {
             for (var t = new Array(e.length), r = 0; r < t.length; ++r) t[r] = e[r].listener || e[r];
             return t
         }(t) : []
-    }, ut.listenerCount = function(e, t) {
-        return "function" == typeof e.listenerCount ? e.listenerCount(t) : pt.call(e, t)
-    }, ut.prototype.listenerCount = pt, ut.prototype.eventNames = function() {
+    }, ft.listenerCount = function(e, t) {
+        return "function" == typeof e.listenerCount ? e.listenerCount(t) : mt.call(e, t)
+    }, ft.prototype.listenerCount = mt, ft.prototype.eventNames = function() {
         return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : []
     };
-    var mt = ot(Object.freeze({
+    var vt = at(Object.freeze({
         __proto__: null,
-        EventEmitter: ut,
-        default: ut
+        EventEmitter: ft,
+        default: ft
     }));
     ! function(e) {
-        var t = nt && nt.__awaiter || function(e, t, r, n) {
+        var t = ot && ot.__awaiter || function(e, t, r, n) {
                 return new(r || (r = Promise))((function(i, o) {
                     function s(e) {
                         try {
                             l(n.next(e))
                         } catch (e) {
                             o(e)
                         }
@@ -1088,15 +1109,15 @@
                         e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                             e(t)
                         }))).then(s, a)
                     }
                     l((n = n.apply(e, t || [])).next())
                 }))
             },
-            r = nt && nt.__generator || function(e, t) {
+            r = ot && ot.__generator || function(e, t) {
                 var r, n, i, o, s = {
                     label: 0,
                     sent: function() {
                         if (1 & i[0]) throw i[1];
                         return i[1]
                     },
                     trys: [],
@@ -1166,15 +1187,15 @@
                         }([o, a])
                     }
                 }
             };
         Object.defineProperty(e, "__esModule", {
             value: !0
         }), e.defaultNextRequest = void 0;
-        var n = mt;
+        var n = vt;
         e.defaultNextRequest = function() {
             var e = -1;
             return function() {
                 return ++e
             }
         };
         var i = function() {
@@ -1236,21 +1257,21 @@
             }, i.prototype.handleError = function(e) {
                 this.requestChannel.emit("error", e)
             }, i.prototype.handleNotification = function(e) {
                 this.requestChannel.emit("notification", e)
             }, i
         }();
         e.default = i
-    }(at);
-    var gt = {},
-        vt = {},
-        yt = {},
-        bt = {};
+    }(ut);
+    var yt = {},
+        bt = {},
+        wt = {},
+        _t = {};
     ! function(e) {
-        var t, r = nt && nt.__extends || (t = function(e, r) {
+        var t, r = ot && ot.__extends || (t = function(e, r) {
             return t = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var r in t) t.hasOwnProperty(r) && (e[r] = t[r])
@@ -1278,22 +1299,22 @@
                     i = r.message,
                     o = r.code,
                     s = r.data;
                 return new n(i, o, s)
             }
             return new n("Unknown error", e.ERR_UNKNOWN, t)
         }
-    }(bt), Object.defineProperty(yt, "__esModule", {
+    }(_t), Object.defineProperty(wt, "__esModule", {
         value: !0
-    }), yt.TransportRequestManager = void 0;
-    var wt = mt,
-        _t = bt,
-        kt = function() {
+    }), wt.TransportRequestManager = void 0;
+    var kt = vt,
+        xt = _t,
+        At = function() {
             function e() {
-                this.pendingRequest = {}, this.pendingBatchRequest = {}, this.transportEventChannel = new wt.EventEmitter
+                this.pendingRequest = {}, this.pendingBatchRequest = {}, this.transportEventChannel = new kt.EventEmitter
             }
             return e.prototype.addRequest = function(e, t) {
                 return this.transportEventChannel.emit("pending", e), e instanceof Array ? (this.addBatchReq(e, t), Promise.resolve()) : this.addReq(e.internalID, t)
             }, e.prototype.settlePendingRequest = function(e, t) {
                 var r = this;
                 e.forEach((function(e) {
                     var n = r.pendingRequest[e.internalID];
@@ -1304,15 +1325,15 @@
             }, e.prototype.resolveResponse = function(e, t) {
                 void 0 === t && (t = !0);
                 var r = e;
                 try {
                     if (r = JSON.parse(e), !1 === this.checkJSONRPC(r)) return;
                     return r instanceof Array ? this.resolveBatch(r, t) : this.resolveRes(r, t)
                 } catch (r) {
-                    var n = new _t.JSONRPCError("Bad response format", _t.ERR_UNKNOWN, e);
+                    var n = new xt.JSONRPCError("Bad response format", xt.ERR_UNKNOWN, e);
                     return t && this.transportEventChannel.emit("error", n), n
                 }
             }, e.prototype.addBatchReq = function(e, t) {
                 var r = this;
                 return e.forEach((function(e) {
                     var t = e.resolve,
                         n = e.reject,
@@ -1333,401 +1354,401 @@
             }, e.prototype.checkJSONRPC = function(e) {
                 var t = [e];
                 return e instanceof Array && (t = e), t.every((function(e) {
                     return void 0 !== e.result || void 0 !== e.error || void 0 !== e.method
                 }))
             }, e.prototype.processResult = function(e, t) {
                 if (e.error) {
-                    var r = _t.convertJSONToRPCError(e);
+                    var r = xt.convertJSONToRPCError(e);
                     t.reject(r)
                 } else t.resolve(e.result)
             }, e.prototype.resolveBatch = function(e, t) {
                 var r = this,
                     n = e.map((function(e) {
                         return r.resolveRes(e, t)
                     })).filter((function(e) {
                         return e
                     }));
                 if (n.length > 0) return n[0]
             }, e.prototype.resolveRes = function(e, t) {
                 var r, n = e.id,
                     i = e.error,
                     o = this.pendingRequest[n];
-                return o ? (delete this.pendingRequest[n], this.processResult(e, o), void this.transportEventChannel.emit("response", e)) : void 0 !== n || void 0 !== i ? (i && (r = _t.convertJSONToRPCError(e)), t && i && r && this.transportEventChannel.emit("error", r), r) : void this.transportEventChannel.emit("notification", e)
+                return o ? (delete this.pendingRequest[n], this.processResult(e, o), void this.transportEventChannel.emit("response", e)) : void 0 !== n || void 0 !== i ? (i && (r = xt.convertJSONToRPCError(e)), t && i && r && this.transportEventChannel.emit("error", r), r) : void this.transportEventChannel.emit("notification", e)
             }, e.prototype.setRequestTimeout = function(e, t, r) {
                 var n = this;
                 setTimeout((function() {
-                    delete n.pendingRequest[e], r(new _t.JSONRPCError("Request timeout request took longer than " + t + " ms to resolve", _t.ERR_TIMEOUT))
+                    delete n.pendingRequest[e], r(new xt.JSONRPCError("Request timeout request took longer than " + t + " ms to resolve", xt.ERR_TIMEOUT))
                 }), t)
             }, e
         }();
-    yt.TransportRequestManager = kt, Object.defineProperty(vt, "__esModule", {
+    wt.TransportRequestManager = At, Object.defineProperty(bt, "__esModule", {
         value: !0
-    }), vt.Transport = void 0;
-    var xt = yt,
-        At = function() {
+    }), bt.Transport = void 0;
+    var qt = wt,
+        Et = function() {
             function e() {
-                this.transportRequestManager = new xt.TransportRequestManager, this.transportRequestManager.transportEventChannel.on("error", (function() {}))
+                this.transportRequestManager = new qt.TransportRequestManager, this.transportRequestManager.transportEventChannel.on("error", (function() {}))
             }
             return e.prototype.subscribe = function(e, t) {
                 this.transportRequestManager.transportEventChannel.addListener(e, t)
             }, e.prototype.unsubscribe = function(e, t) {
                 if (!e) return this.transportRequestManager.transportEventChannel.removeAllListeners();
                 e && t && this.transportRequestManager.transportEventChannel.removeListener(e, t)
             }, e.prototype.parseData = function(e) {
                 return e instanceof Array ? e.map((function(e) {
                     return e.request.request
                 })) : e.request
             }, e
         }();
-    vt.Transport = At;
-    var qt, Et = {};
-    qt = Et, Object.defineProperty(qt, "__esModule", {
+    bt.Transport = Et;
+    var Tt, $t = {};
+    Tt = $t, Object.defineProperty(Tt, "__esModule", {
         value: !0
-    }), qt.getNotifications = qt.getBatchRequests = qt.isNotification = void 0, qt.isNotification = function(e) {
+    }), Tt.getNotifications = Tt.getBatchRequests = Tt.isNotification = void 0, Tt.isNotification = function(e) {
         return void 0 === e.request.id || null === e.request.id
-    }, qt.getBatchRequests = function(e) {
+    }, Tt.getBatchRequests = function(e) {
         return e instanceof Array ? e.filter((function(e) {
             var t = e.request.request.id;
             return null != t
         })).map((function(e) {
             return e.request
         })) : []
-    }, qt.getNotifications = function(e) {
+    }, Tt.getNotifications = function(e) {
         return e instanceof Array ? e.filter((function(e) {
-            return qt.isNotification(e.request)
+            return Tt.isNotification(e.request)
         })).map((function(e) {
             return e.request
-        })) : qt.isNotification(e) ? [e] : []
+        })) : Tt.isNotification(e) ? [e] : []
     };
-    var Tt, $t = nt && nt.__extends || (Tt = function(e, t) {
-        return Tt = Object.setPrototypeOf || {
+    var Ot, St = ot && ot.__extends || (Ot = function(e, t) {
+        return Ot = Object.setPrototypeOf || {
             __proto__: []
         }
         instanceof Array && function(e, t) {
             e.__proto__ = t
         } || function(e, t) {
             for (var r in t) t.hasOwnProperty(r) && (e[r] = t[r])
-        }, Tt(e, t)
+        }, Ot(e, t)
     }, function(e, t) {
         function r() {
             this.constructor = e
         }
-        Tt(e, t), e.prototype = null === t ? Object.create(t) : (r.prototype = t.prototype, new r)
+        Ot(e, t), e.prototype = null === t ? Object.create(t) : (r.prototype = t.prototype, new r)
     });
-    Object.defineProperty(gt, "__esModule", {
+    Object.defineProperty(yt, "__esModule", {
         value: !0
     });
-    var Ot = Et,
-        St = bt,
-        Dt = function(e) {
+    var Dt = $t,
+        Ct = _t,
+        Rt = function(e) {
             function t(t, r, n) {
                 var i = e.call(this) || this;
                 return i.connection = t, i.reqUri = r, i.resUri = n, i
             }
-            return $t(t, e), t.prototype.connect = function() {
+            return St(t, e), t.prototype.connect = function() {
                 var e = this;
                 return this.connection.on(this.resUri, (function(t) {
                     e.transportRequestManager.resolveResponse(t)
                 })), Promise.resolve()
             }, t.prototype.sendData = function(e, t) {
                 void 0 === t && (t = null);
                 var r = this.transportRequestManager.addRequest(e, t),
-                    n = Ot.getNotifications(e),
+                    n = Dt.getNotifications(e),
                     i = this.parseData(e);
                 try {
                     return this.connection.emit(this.reqUri, i), this.transportRequestManager.settlePendingRequest(n), r
                 } catch (e) {
-                    var o = new St.JSONRPCError(e.message, St.ERR_UNKNOWN, e);
+                    var o = new Ct.JSONRPCError(e.message, Ct.ERR_UNKNOWN, e);
                     return this.transportRequestManager.settlePendingRequest(n, o), Promise.reject(o)
                 }
             }, t.prototype.close = function() {
                 this.connection.removeAllListeners()
             }, t
-        }(vt.Transport);
-    gt.default = Dt;
-    var Ct = {},
-        Rt = "undefined" != typeof globalThis && globalThis || "undefined" != typeof self && self || void 0 !== Rt && Rt,
-        Lt = "URLSearchParams" in Rt,
-        Nt = "Symbol" in Rt && "iterator" in Symbol,
-        It = "FileReader" in Rt && "Blob" in Rt && function() {
+        }(bt.Transport);
+    yt.default = Rt;
+    var Lt = {},
+        Nt = "undefined" != typeof globalThis && globalThis || "undefined" != typeof self && self || void 0 !== Nt && Nt,
+        It = "URLSearchParams" in Nt,
+        Ft = "Symbol" in Nt && "iterator" in Symbol,
+        Mt = "FileReader" in Nt && "Blob" in Nt && function() {
             try {
                 return new Blob, !0
             } catch (e) {
                 return !1
             }
         }(),
-        Ft = "FormData" in Rt,
-        Mt = "ArrayBuffer" in Rt;
-    if (Mt) var Pt = ["[object Int8Array]", "[object Uint8Array]", "[object Uint8ClampedArray]", "[object Int16Array]", "[object Uint16Array]", "[object Int32Array]", "[object Uint32Array]", "[object Float32Array]", "[object Float64Array]"],
-        jt = ArrayBuffer.isView || function(e) {
-            return e && Pt.indexOf(Object.prototype.toString.call(e)) > -1
+        Pt = "FormData" in Nt,
+        jt = "ArrayBuffer" in Nt;
+    if (jt) var Bt = ["[object Int8Array]", "[object Uint8Array]", "[object Uint8ClampedArray]", "[object Int16Array]", "[object Uint16Array]", "[object Int32Array]", "[object Uint32Array]", "[object Float32Array]", "[object Float64Array]"],
+        Ut = ArrayBuffer.isView || function(e) {
+            return e && Bt.indexOf(Object.prototype.toString.call(e)) > -1
         };
 
-    function Bt(e) {
+    function Vt(e) {
         if ("string" != typeof e && (e = String(e)), /[^a-z0-9\-#$%&'*+.^_`|~!]/i.test(e) || "" === e) throw new TypeError('Invalid character in header field name: "' + e + '"');
         return e.toLowerCase()
     }
 
-    function Ut(e) {
+    function zt(e) {
         return "string" != typeof e && (e = String(e)), e
     }
 
-    function Vt(e) {
+    function Ht(e) {
         var t = {
             next: function() {
                 var t = e.shift();
                 return {
                     done: void 0 === t,
                     value: t
                 }
             }
         };
-        return Nt && (t[Symbol.iterator] = function() {
+        return Ft && (t[Symbol.iterator] = function() {
             return t
         }), t
     }
 
-    function zt(e) {
-        this.map = {}, e instanceof zt ? e.forEach((function(e, t) {
+    function Wt(e) {
+        this.map = {}, e instanceof Wt ? e.forEach((function(e, t) {
             this.append(t, e)
         }), this) : Array.isArray(e) ? e.forEach((function(e) {
             this.append(e[0], e[1])
         }), this) : e && Object.getOwnPropertyNames(e).forEach((function(t) {
             this.append(t, e[t])
         }), this)
     }
 
-    function Ht(e) {
+    function Gt(e) {
         if (e.bodyUsed) return Promise.reject(new TypeError("Already read"));
         e.bodyUsed = !0
     }
 
-    function Wt(e) {
+    function Zt(e) {
         return new Promise((function(t, r) {
             e.onload = function() {
                 t(e.result)
             }, e.onerror = function() {
                 r(e.error)
             }
         }))
     }
 
-    function Gt(e) {
+    function Jt(e) {
         var t = new FileReader,
-            r = Wt(t);
+            r = Zt(t);
         return t.readAsArrayBuffer(e), r
     }
 
-    function Zt(e) {
+    function Yt(e) {
         if (e.slice) return e.slice(0);
         var t = new Uint8Array(e.byteLength);
         return t.set(new Uint8Array(e)), t.buffer
     }
 
-    function Jt() {
+    function Kt() {
         return this.bodyUsed = !1, this._initBody = function(e) {
             var t;
-            this.bodyUsed = this.bodyUsed, this._bodyInit = e, e ? "string" == typeof e ? this._bodyText = e : It && Blob.prototype.isPrototypeOf(e) ? this._bodyBlob = e : Ft && FormData.prototype.isPrototypeOf(e) ? this._bodyFormData = e : Lt && URLSearchParams.prototype.isPrototypeOf(e) ? this._bodyText = e.toString() : Mt && It && ((t = e) && DataView.prototype.isPrototypeOf(t)) ? (this._bodyArrayBuffer = Zt(e.buffer), this._bodyInit = new Blob([this._bodyArrayBuffer])) : Mt && (ArrayBuffer.prototype.isPrototypeOf(e) || jt(e)) ? this._bodyArrayBuffer = Zt(e) : this._bodyText = e = Object.prototype.toString.call(e) : this._bodyText = "", this.headers.get("content-type") || ("string" == typeof e ? this.headers.set("content-type", "text/plain;charset=UTF-8") : this._bodyBlob && this._bodyBlob.type ? this.headers.set("content-type", this._bodyBlob.type) : Lt && URLSearchParams.prototype.isPrototypeOf(e) && this.headers.set("content-type", "application/x-www-form-urlencoded;charset=UTF-8"))
-        }, It && (this.blob = function() {
-            var e = Ht(this);
+            this.bodyUsed = this.bodyUsed, this._bodyInit = e, e ? "string" == typeof e ? this._bodyText = e : Mt && Blob.prototype.isPrototypeOf(e) ? this._bodyBlob = e : Pt && FormData.prototype.isPrototypeOf(e) ? this._bodyFormData = e : It && URLSearchParams.prototype.isPrototypeOf(e) ? this._bodyText = e.toString() : jt && Mt && ((t = e) && DataView.prototype.isPrototypeOf(t)) ? (this._bodyArrayBuffer = Yt(e.buffer), this._bodyInit = new Blob([this._bodyArrayBuffer])) : jt && (ArrayBuffer.prototype.isPrototypeOf(e) || Ut(e)) ? this._bodyArrayBuffer = Yt(e) : this._bodyText = e = Object.prototype.toString.call(e) : this._bodyText = "", this.headers.get("content-type") || ("string" == typeof e ? this.headers.set("content-type", "text/plain;charset=UTF-8") : this._bodyBlob && this._bodyBlob.type ? this.headers.set("content-type", this._bodyBlob.type) : It && URLSearchParams.prototype.isPrototypeOf(e) && this.headers.set("content-type", "application/x-www-form-urlencoded;charset=UTF-8"))
+        }, Mt && (this.blob = function() {
+            var e = Gt(this);
             if (e) return e;
             if (this._bodyBlob) return Promise.resolve(this._bodyBlob);
             if (this._bodyArrayBuffer) return Promise.resolve(new Blob([this._bodyArrayBuffer]));
             if (this._bodyFormData) throw new Error("could not read FormData body as blob");
             return Promise.resolve(new Blob([this._bodyText]))
         }, this.arrayBuffer = function() {
             if (this._bodyArrayBuffer) {
-                var e = Ht(this);
+                var e = Gt(this);
                 return e || (ArrayBuffer.isView(this._bodyArrayBuffer) ? Promise.resolve(this._bodyArrayBuffer.buffer.slice(this._bodyArrayBuffer.byteOffset, this._bodyArrayBuffer.byteOffset + this._bodyArrayBuffer.byteLength)) : Promise.resolve(this._bodyArrayBuffer))
             }
-            return this.blob().then(Gt)
+            return this.blob().then(Jt)
         }), this.text = function() {
-            var e = Ht(this);
+            var e = Gt(this);
             if (e) return e;
             if (this._bodyBlob) return function(e) {
                 var t = new FileReader,
-                    r = Wt(t);
+                    r = Zt(t);
                 return t.readAsText(e), r
             }(this._bodyBlob);
             if (this._bodyArrayBuffer) return Promise.resolve(function(e) {
                 for (var t = new Uint8Array(e), r = new Array(t.length), n = 0; n < t.length; n++) r[n] = String.fromCharCode(t[n]);
                 return r.join("")
             }(this._bodyArrayBuffer));
             if (this._bodyFormData) throw new Error("could not read FormData body as text");
             return Promise.resolve(this._bodyText)
-        }, Ft && (this.formData = function() {
-            return this.text().then(Xt)
+        }, Pt && (this.formData = function() {
+            return this.text().then(er)
         }), this.json = function() {
             return this.text().then(JSON.parse)
         }, this
     }
-    zt.prototype.append = function(e, t) {
-        e = Bt(e), t = Ut(t);
+    Wt.prototype.append = function(e, t) {
+        e = Vt(e), t = zt(t);
         var r = this.map[e];
         this.map[e] = r ? r + ", " + t : t
-    }, zt.prototype.delete = function(e) {
-        delete this.map[Bt(e)]
-    }, zt.prototype.get = function(e) {
-        return e = Bt(e), this.has(e) ? this.map[e] : null
-    }, zt.prototype.has = function(e) {
-        return this.map.hasOwnProperty(Bt(e))
-    }, zt.prototype.set = function(e, t) {
-        this.map[Bt(e)] = Ut(t)
-    }, zt.prototype.forEach = function(e, t) {
+    }, Wt.prototype.delete = function(e) {
+        delete this.map[Vt(e)]
+    }, Wt.prototype.get = function(e) {
+        return e = Vt(e), this.has(e) ? this.map[e] : null
+    }, Wt.prototype.has = function(e) {
+        return this.map.hasOwnProperty(Vt(e))
+    }, Wt.prototype.set = function(e, t) {
+        this.map[Vt(e)] = zt(t)
+    }, Wt.prototype.forEach = function(e, t) {
         for (var r in this.map) this.map.hasOwnProperty(r) && e.call(t, this.map[r], r, this)
-    }, zt.prototype.keys = function() {
+    }, Wt.prototype.keys = function() {
         var e = [];
         return this.forEach((function(t, r) {
             e.push(r)
-        })), Vt(e)
-    }, zt.prototype.values = function() {
+        })), Ht(e)
+    }, Wt.prototype.values = function() {
         var e = [];
         return this.forEach((function(t) {
             e.push(t)
-        })), Vt(e)
-    }, zt.prototype.entries = function() {
+        })), Ht(e)
+    }, Wt.prototype.entries = function() {
         var e = [];
         return this.forEach((function(t, r) {
             e.push([r, t])
-        })), Vt(e)
-    }, Nt && (zt.prototype[Symbol.iterator] = zt.prototype.entries);
-    var Yt = ["DELETE", "GET", "HEAD", "OPTIONS", "POST", "PUT"];
+        })), Ht(e)
+    }, Ft && (Wt.prototype[Symbol.iterator] = Wt.prototype.entries);
+    var Xt = ["DELETE", "GET", "HEAD", "OPTIONS", "POST", "PUT"];
 
-    function Kt(e, t) {
-        if (!(this instanceof Kt)) throw new TypeError('Please use the "new" operator, this DOM object constructor cannot be called as a function.');
+    function Qt(e, t) {
+        if (!(this instanceof Qt)) throw new TypeError('Please use the "new" operator, this DOM object constructor cannot be called as a function.');
         var r, n, i = (t = t || {}).body;
-        if (e instanceof Kt) {
+        if (e instanceof Qt) {
             if (e.bodyUsed) throw new TypeError("Already read");
-            this.url = e.url, this.credentials = e.credentials, t.headers || (this.headers = new zt(e.headers)), this.method = e.method, this.mode = e.mode, this.signal = e.signal, i || null == e._bodyInit || (i = e._bodyInit, e.bodyUsed = !0)
+            this.url = e.url, this.credentials = e.credentials, t.headers || (this.headers = new Wt(e.headers)), this.method = e.method, this.mode = e.mode, this.signal = e.signal, i || null == e._bodyInit || (i = e._bodyInit, e.bodyUsed = !0)
         } else this.url = String(e);
-        if (this.credentials = t.credentials || this.credentials || "same-origin", !t.headers && this.headers || (this.headers = new zt(t.headers)), this.method = (r = t.method || this.method || "GET", n = r.toUpperCase(), Yt.indexOf(n) > -1 ? n : r), this.mode = t.mode || this.mode || null, this.signal = t.signal || this.signal, this.referrer = null, ("GET" === this.method || "HEAD" === this.method) && i) throw new TypeError("Body not allowed for GET or HEAD requests");
+        if (this.credentials = t.credentials || this.credentials || "same-origin", !t.headers && this.headers || (this.headers = new Wt(t.headers)), this.method = (r = t.method || this.method || "GET", n = r.toUpperCase(), Xt.indexOf(n) > -1 ? n : r), this.mode = t.mode || this.mode || null, this.signal = t.signal || this.signal, this.referrer = null, ("GET" === this.method || "HEAD" === this.method) && i) throw new TypeError("Body not allowed for GET or HEAD requests");
         if (this._initBody(i), !("GET" !== this.method && "HEAD" !== this.method || "no-store" !== t.cache && "no-cache" !== t.cache)) {
             var o = /([?&])_=[^&]*/;
             if (o.test(this.url)) this.url = this.url.replace(o, "$1_=" + (new Date).getTime());
             else {
                 this.url += (/\?/.test(this.url) ? "&" : "?") + "_=" + (new Date).getTime()
             }
         }
     }
 
-    function Xt(e) {
+    function er(e) {
         var t = new FormData;
         return e.trim().split("&").forEach((function(e) {
             if (e) {
                 var r = e.split("="),
                     n = r.shift().replace(/\+/g, " "),
                     i = r.join("=").replace(/\+/g, " ");
                 t.append(decodeURIComponent(n), decodeURIComponent(i))
             }
         })), t
     }
 
-    function Qt(e, t) {
-        if (!(this instanceof Qt)) throw new TypeError('Please use the "new" operator, this DOM object constructor cannot be called as a function.');
-        t || (t = {}), this.type = "default", this.status = void 0 === t.status ? 200 : t.status, this.ok = this.status >= 200 && this.status < 300, this.statusText = void 0 === t.statusText ? "" : "" + t.statusText, this.headers = new zt(t.headers), this.url = t.url || "", this._initBody(e)
+    function tr(e, t) {
+        if (!(this instanceof tr)) throw new TypeError('Please use the "new" operator, this DOM object constructor cannot be called as a function.');
+        t || (t = {}), this.type = "default", this.status = void 0 === t.status ? 200 : t.status, this.ok = this.status >= 200 && this.status < 300, this.statusText = void 0 === t.statusText ? "" : "" + t.statusText, this.headers = new Wt(t.headers), this.url = t.url || "", this._initBody(e)
     }
-    Kt.prototype.clone = function() {
-        return new Kt(this, {
+    Qt.prototype.clone = function() {
+        return new Qt(this, {
             body: this._bodyInit
         })
-    }, Jt.call(Kt.prototype), Jt.call(Qt.prototype), Qt.prototype.clone = function() {
-        return new Qt(this._bodyInit, {
+    }, Kt.call(Qt.prototype), Kt.call(tr.prototype), tr.prototype.clone = function() {
+        return new tr(this._bodyInit, {
             status: this.status,
             statusText: this.statusText,
-            headers: new zt(this.headers),
+            headers: new Wt(this.headers),
             url: this.url
         })
-    }, Qt.error = function() {
-        var e = new Qt(null, {
+    }, tr.error = function() {
+        var e = new tr(null, {
             status: 0,
             statusText: ""
         });
         return e.type = "error", e
     };
-    var er = [301, 302, 303, 307, 308];
-    Qt.redirect = function(e, t) {
-        if (-1 === er.indexOf(t)) throw new RangeError("Invalid status code");
-        return new Qt(null, {
+    var rr = [301, 302, 303, 307, 308];
+    tr.redirect = function(e, t) {
+        if (-1 === rr.indexOf(t)) throw new RangeError("Invalid status code");
+        return new tr(null, {
             status: t,
             headers: {
                 location: e
             }
         })
     };
-    var tr = Rt.DOMException;
+    var nr = Nt.DOMException;
     try {
-        new tr
+        new nr
     } catch (e) {
-        (tr = function(e, t) {
+        (nr = function(e, t) {
             this.message = e, this.name = t;
             var r = Error(e);
             this.stack = r.stack
-        }).prototype = Object.create(Error.prototype), tr.prototype.constructor = tr
+        }).prototype = Object.create(Error.prototype), nr.prototype.constructor = nr
     }
 
-    function rr(e, t) {
+    function ir(e, t) {
         return new Promise((function(r, n) {
-            var i = new Kt(e, t);
-            if (i.signal && i.signal.aborted) return n(new tr("Aborted", "AbortError"));
+            var i = new Qt(e, t);
+            if (i.signal && i.signal.aborted) return n(new nr("Aborted", "AbortError"));
             var o = new XMLHttpRequest;
 
             function s() {
                 o.abort()
             }
             o.onload = function() {
                 var e, t, n = {
                     status: o.status,
                     statusText: o.statusText,
-                    headers: (e = o.getAllResponseHeaders() || "", t = new zt, e.replace(/\r?\n[\t ]+/g, " ").split("\r").map((function(e) {
+                    headers: (e = o.getAllResponseHeaders() || "", t = new Wt, e.replace(/\r?\n[\t ]+/g, " ").split("\r").map((function(e) {
                         return 0 === e.indexOf("\n") ? e.substr(1, e.length) : e
                     })).forEach((function(e) {
                         var r = e.split(":"),
                             n = r.shift().trim();
                         if (n) {
                             var i = r.join(":").trim();
                             t.append(n, i)
                         }
                     })), t)
                 };
                 n.url = "responseURL" in o ? o.responseURL : n.headers.get("X-Request-URL");
                 var i = "response" in o ? o.response : o.responseText;
                 setTimeout((function() {
-                    r(new Qt(i, n))
+                    r(new tr(i, n))
                 }), 0)
             }, o.onerror = function() {
                 setTimeout((function() {
                     n(new TypeError("Network request failed"))
                 }), 0)
             }, o.ontimeout = function() {
                 setTimeout((function() {
                     n(new TypeError("Network request failed"))
                 }), 0)
             }, o.onabort = function() {
                 setTimeout((function() {
-                    n(new tr("Aborted", "AbortError"))
+                    n(new nr("Aborted", "AbortError"))
                 }), 0)
             }, o.open(i.method, function(e) {
                 try {
-                    return "" === e && Rt.location.href ? Rt.location.href : e
+                    return "" === e && Nt.location.href ? Nt.location.href : e
                 } catch (t) {
                     return e
                 }
-            }(i.url), !0), "include" === i.credentials ? o.withCredentials = !0 : "omit" === i.credentials && (o.withCredentials = !1), "responseType" in o && (It ? o.responseType = "blob" : Mt && i.headers.get("Content-Type") && -1 !== i.headers.get("Content-Type").indexOf("application/octet-stream") && (o.responseType = "arraybuffer")), !t || "object" != typeof t.headers || t.headers instanceof zt ? i.headers.forEach((function(e, t) {
+            }(i.url), !0), "include" === i.credentials ? o.withCredentials = !0 : "omit" === i.credentials && (o.withCredentials = !1), "responseType" in o && (Mt ? o.responseType = "blob" : jt && i.headers.get("Content-Type") && -1 !== i.headers.get("Content-Type").indexOf("application/octet-stream") && (o.responseType = "arraybuffer")), !t || "object" != typeof t.headers || t.headers instanceof Wt ? i.headers.forEach((function(e, t) {
                 o.setRequestHeader(t, e)
             })) : Object.getOwnPropertyNames(t.headers).forEach((function(e) {
-                o.setRequestHeader(e, Ut(t.headers[e]))
+                o.setRequestHeader(e, zt(t.headers[e]))
             })), i.signal && (i.signal.addEventListener("abort", s), o.onreadystatechange = function() {
                 4 === o.readyState && i.signal.removeEventListener("abort", s)
             }), o.send(void 0 === i._bodyInit ? null : i._bodyInit)
         }))
     }
-    rr.polyfill = !0, Rt.fetch || (Rt.fetch = rr, Rt.Headers = zt, Rt.Request = Kt, Rt.Response = Qt);
-    var nr = self.fetch.bind(self),
-        ir = nt && nt.__extends || function() {
+    ir.polyfill = !0, Nt.fetch || (Nt.fetch = ir, Nt.Headers = Wt, Nt.Request = Qt, Nt.Response = tr);
+    var or = self.fetch.bind(self),
+        sr = ot && ot.__extends || function() {
             var e = function(t, r) {
                 return e = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
@@ -1737,15 +1758,15 @@
             return function(t, r) {
                 function n() {
                     this.constructor = t
                 }
                 e(t, r), t.prototype = null === r ? Object.create(r) : (n.prototype = r.prototype, new n)
             }
         }(),
-        or = nt && nt.__awaiter || function(e, t, r, n) {
+        ar = ot && ot.__awaiter || function(e, t, r, n) {
             return new(r || (r = Promise))((function(i, o) {
                 function s(e) {
                     try {
                         l(n.next(e))
                     } catch (e) {
                         o(e)
                     }
@@ -1764,15 +1785,15 @@
                     e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                         e(t)
                     }))).then(s, a)
                 }
                 l((n = n.apply(e, t || [])).next())
             }))
         },
-        sr = nt && nt.__generator || function(e, t) {
+        lr = ot && ot.__generator || function(e, t) {
             var r, n, i, o, s = {
                 label: 0,
                 sent: function() {
                     if (1 & i[0]) throw i[1];
                     return i[1]
                 },
                 trys: [],
@@ -1839,77 +1860,76 @@
                             value: o[0] ? o[1] : void 0,
                             done: !0
                         }
                     }([o, a])
                 }
             }
         },
-        ar = nt && nt.__importDefault || function(e) {
+        ur = ot && ot.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
-    Object.defineProperty(Ct, "__esModule", {
+    Object.defineProperty(Lt, "__esModule", {
         value: !0
-    }), Ct.HTTPTransport = void 0;
-    var lr = ar(nr),
-        ur = Et,
-        cr = bt,
-        fr = function(e) {
+    }), Lt.HTTPTransport = void 0;
+    var cr = ur(or),
+        fr = $t,
+        hr = _t,
+        pr = function(e) {
             function t(r, n) {
                 var i = e.call(this) || this;
                 return i.onlyNotifications = function(e) {
                     return e instanceof Array ? e.every((function(e) {
                         return null === e.request.request.id || void 0 === e.request.request.id
                     })) : null === e.request.id || void 0 === e.request.id
                 }, i.uri = r, i.credentials = n && n.credentials, i.headers = t.setupHeaders(n && n.headers), i.injectedFetcher = null == n ? void 0 : n.fetcher, i
             }
-            return ir(t, e), t.prototype.connect = function() {
+            return sr(t, e), t.prototype.connect = function() {
                 return Promise.resolve()
             }, t.prototype.sendData = function(e, t) {
-                return void 0 === t && (t = null), or(this, void 0, void 0, (function() {
+                return void 0 === t && (t = null), ar(this, void 0, void 0, (function() {
                     var r, n, i, o, s, a, l, u;
-                    return sr(this, (function(c) {
+                    return lr(this, (function(c) {
                         switch (c.label) {
                             case 0:
-                                r = this.transportRequestManager.addRequest(e, t), n = ur.getNotifications(e), i = ur.getBatchRequests(e), o = this.injectedFetcher || lr.default, c.label = 1;
+                                r = this.transportRequestManager.addRequest(e, t), n = fr.getNotifications(e), i = fr.getBatchRequests(e), o = this.injectedFetcher || cr.default, c.label = 1;
                             case 1:
                                 return c.trys.push([1, 4, , 5]), [4, o(this.uri, {
                                     method: "POST",
                                     headers: this.headers,
                                     body: JSON.stringify(this.parseData(e)),
                                     credentials: this.credentials
                                 })];
                             case 2:
                                 return s = c.sent(), this.transportRequestManager.settlePendingRequest(n), this.onlyNotifications(e) ? [2, Promise.resolve()] : [4, s.text()];
                             case 3:
                                 return a = c.sent(), (u = this.transportRequestManager.resolveResponse(a)) ? (this.transportRequestManager.settlePendingRequest(i, u), [2, Promise.reject(u)]) : [3, 5];
                             case 4:
-                                return l = c.sent(), u = new cr.JSONRPCError(l.message, cr.ERR_UNKNOWN, l), this.transportRequestManager.settlePendingRequest(n, u), this.transportRequestManager.settlePendingRequest(ur.getBatchRequests(e), u), [2, Promise.reject(u)];
+                                return l = c.sent(), u = new hr.JSONRPCError(l.message, hr.ERR_UNKNOWN, l), this.transportRequestManager.settlePendingRequest(n, u), this.transportRequestManager.settlePendingRequest(fr.getBatchRequests(e), u), [2, Promise.reject(u)];
                             case 5:
                                 return [2, r]
                         }
                     }))
                 }))
             }, t.prototype.close = function() {}, t.setupHeaders = function(e) {
                 var t = new Headers(e);
                 return t.set("Content-Type", "application/json"), t
             }, t
-        }(vt.Transport);
-    Ct.HTTPTransport = fr, Ct.default = fr;
-    var hr = {},
-        pr = "undefined" != typeof global ? global : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {},
-        dr = null;
-    "undefined" != typeof WebSocket ? dr = WebSocket : "undefined" != typeof MozWebSocket ? dr = MozWebSocket : void 0 !== pr ? dr = pr.WebSocket || pr.MozWebSocket : "undefined" != typeof window ? dr = window.WebSocket || window.MozWebSocket : "undefined" != typeof self && (dr = self.WebSocket || self.MozWebSocket);
-    var mr = dr,
-        gr = ot(Object.freeze({
+        }(bt.Transport);
+    Lt.HTTPTransport = pr, Lt.default = pr;
+    var dr = {},
+        mr = null;
+    "undefined" != typeof WebSocket ? mr = WebSocket : "undefined" != typeof MozWebSocket ? mr = MozWebSocket : void 0 !== A ? mr = A.WebSocket || A.MozWebSocket : "undefined" != typeof window ? mr = window.WebSocket || window.MozWebSocket : "undefined" != typeof self && (mr = self.WebSocket || self.MozWebSocket);
+    var gr = mr,
+        vr = at(Object.freeze({
             __proto__: null,
-            default: mr
+            default: gr
         })),
-        vr = nt && nt.__extends || function() {
+        yr = ot && ot.__extends || function() {
             var e = function(t, r) {
                 return e = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
@@ -1919,15 +1939,15 @@
             return function(t, r) {
                 function n() {
                     this.constructor = t
                 }
                 e(t, r), t.prototype = null === r ? Object.create(r) : (n.prototype = r.prototype, new n)
             }
         }(),
-        yr = nt && nt.__awaiter || function(e, t, r, n) {
+        br = ot && ot.__awaiter || function(e, t, r, n) {
             return new(r || (r = Promise))((function(i, o) {
                 function s(e) {
                     try {
                         l(n.next(e))
                     } catch (e) {
                         o(e)
                     }
@@ -1946,15 +1966,15 @@
                     e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                         e(t)
                     }))).then(s, a)
                 }
                 l((n = n.apply(e, t || [])).next())
             }))
         },
-        br = nt && nt.__generator || function(e, t) {
+        wr = ot && ot.__generator || function(e, t) {
             var r, n, i, o, s = {
                 label: 0,
                 sent: function() {
                     if (1 & i[0]) throw i[1];
                     return i[1]
                 },
                 trys: [],
@@ -2021,61 +2041,61 @@
                             value: o[0] ? o[1] : void 0,
                             done: !0
                         }
                     }([o, a])
                 }
             }
         },
-        wr = nt && nt.__importDefault || function(e) {
+        _r = ot && ot.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
-    Object.defineProperty(hr, "__esModule", {
+    Object.defineProperty(dr, "__esModule", {
         value: !0
     });
-    var _r = wr(gr),
-        kr = Et,
-        xr = bt,
-        Ar = function(e) {
+    var kr = _r(vr),
+        xr = $t,
+        Ar = _t,
+        qr = function(e) {
             function t(t) {
                 var r = e.call(this) || this;
-                return r.uri = t, r.connection = new _r.default(t), r
+                return r.uri = t, r.connection = new kr.default(t), r
             }
-            return vr(t, e), t.prototype.connect = function() {
+            return yr(t, e), t.prototype.connect = function() {
                 var e = this;
                 return new Promise((function(t, r) {
                     var n = function() {
                         e.connection.removeEventListener("open", n), t()
                     };
                     e.connection.addEventListener("open", n), e.connection.addEventListener("message", (function(t) {
                         var r = t.data;
                         e.transportRequestManager.resolveResponse(r)
                     }))
                 }))
             }, t.prototype.sendData = function(e, t) {
-                return void 0 === t && (t = 5e3), yr(this, void 0, void 0, (function() {
+                return void 0 === t && (t = 5e3), br(this, void 0, void 0, (function() {
                     var r, n, i;
-                    return br(this, (function(o) {
-                        r = this.transportRequestManager.addRequest(e, t), n = kr.getNotifications(e);
+                    return wr(this, (function(o) {
+                        r = this.transportRequestManager.addRequest(e, t), n = xr.getNotifications(e);
                         try {
                             this.connection.send(JSON.stringify(this.parseData(e))), this.transportRequestManager.settlePendingRequest(n)
                         } catch (t) {
-                            i = new xr.JSONRPCError(t.message, xr.ERR_UNKNOWN, t), this.transportRequestManager.settlePendingRequest(n, i), this.transportRequestManager.settlePendingRequest(kr.getBatchRequests(e), i), r = Promise.reject(i)
+                            i = new Ar.JSONRPCError(t.message, Ar.ERR_UNKNOWN, t), this.transportRequestManager.settlePendingRequest(n, i), this.transportRequestManager.settlePendingRequest(xr.getBatchRequests(e), i), r = Promise.reject(i)
                         }
                         return [2, r]
                     }))
                 }))
             }, t.prototype.close = function() {
                 this.connection.close()
             }, t
-        }(vt.Transport);
-    hr.default = Ar;
-    var qr = {},
-        Er = nt && nt.__extends || function() {
+        }(bt.Transport);
+    dr.default = qr;
+    var Er = {},
+        Tr = ot && ot.__extends || function() {
             var e = function(t, r) {
                 return e = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
@@ -2085,15 +2105,15 @@
             return function(t, r) {
                 function n() {
                     this.constructor = t
                 }
                 e(t, r), t.prototype = null === r ? Object.create(r) : (n.prototype = r.prototype, new n)
             }
         }(),
-        Tr = nt && nt.__awaiter || function(e, t, r, n) {
+        $r = ot && ot.__awaiter || function(e, t, r, n) {
             return new(r || (r = Promise))((function(i, o) {
                 function s(e) {
                     try {
                         l(n.next(e))
                     } catch (e) {
                         o(e)
                     }
@@ -2112,15 +2132,15 @@
                     e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                         e(t)
                     }))).then(s, a)
                 }
                 l((n = n.apply(e, t || [])).next())
             }))
         },
-        $r = nt && nt.__generator || function(e, t) {
+        Or = ot && ot.__generator || function(e, t) {
             var r, n, i, o, s = {
                 label: 0,
                 sent: function() {
                     if (1 & i[0]) throw i[1];
                     return i[1]
                 },
                 trys: [],
@@ -2187,62 +2207,62 @@
                             value: o[0] ? o[1] : void 0,
                             done: !0
                         }
                     }([o, a])
                 }
             }
         };
-    Object.defineProperty(qr, "__esModule", {
+    Object.defineProperty(Er, "__esModule", {
         value: !0
     });
-    var Or = Et,
-        Sr = function(e) {
+    var Sr = $t,
+        Dr = function(e) {
             function t(t) {
                 var r = e.call(this) || this;
                 return r.messageHandler = function(e) {
                     r.transportRequestManager.resolveResponse(JSON.stringify(e.data))
                 }, r.uri = t, r.postMessageID = "post-message-transport-" + Math.random(), r
             }
-            return Er(t, e), t.prototype.createWindow = function(e) {
+            return Tr(t, e), t.prototype.createWindow = function(e) {
                 return new Promise((function(t, r) {
                     var n, i, o;
                     i = e, o = window.screen.height, n = window.open(i, "inspector:popup", "left=0,top=0,width=400,height=" + o + ",resizable,scrollbars=yes,status=1"), setTimeout((function() {
                         t(n)
                     }), 3e3)
                 }))
             }, t.prototype.connect = function() {
                 var e = this,
                     t = /^(http|https):\/\/.*$/;
                 return new Promise((function(r, n) {
-                    return Tr(e, void 0, void 0, (function() {
+                    return $r(e, void 0, void 0, (function() {
                         var e;
-                        return $r(this, (function(i) {
+                        return Or(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return t.test(this.uri) || n(new Error("Bad URI")), e = this, [4, this.createWindow(this.uri)];
                                 case 1:
                                     return e.frame = i.sent(), window.addEventListener("message", this.messageHandler), r(), [2]
                             }
                         }))
                     }))
                 }))
             }, t.prototype.sendData = function(e, t) {
-                return Tr(this, void 0, void 0, (function() {
+                return $r(this, void 0, void 0, (function() {
                     var t, r;
-                    return $r(this, (function(n) {
-                        return t = this.transportRequestManager.addRequest(e, null), r = Or.getNotifications(e), this.frame && (this.frame.postMessage(e.request, this.uri), this.transportRequestManager.settlePendingRequest(r)), [2, t]
+                    return Or(this, (function(n) {
+                        return t = this.transportRequestManager.addRequest(e, null), r = Sr.getNotifications(e), this.frame && (this.frame.postMessage(e.request, this.uri), this.transportRequestManager.settlePendingRequest(r)), [2, t]
                     }))
                 }))
             }, t.prototype.close = function() {
                 this.frame && (window.removeEventListener("message", this.messageHandler), this.frame.close())
             }, t
-        }(vt.Transport);
-    qr.default = Sr;
-    var Dr = {},
-        Cr = nt && nt.__extends || function() {
+        }(bt.Transport);
+    Er.default = Dr;
+    var Cr = {},
+        Rr = ot && ot.__extends || function() {
             var e = function(t, r) {
                 return e = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
@@ -2252,15 +2272,15 @@
             return function(t, r) {
                 function n() {
                     this.constructor = t
                 }
                 e(t, r), t.prototype = null === r ? Object.create(r) : (n.prototype = r.prototype, new n)
             }
         }(),
-        Rr = nt && nt.__awaiter || function(e, t, r, n) {
+        Lr = ot && ot.__awaiter || function(e, t, r, n) {
             return new(r || (r = Promise))((function(i, o) {
                 function s(e) {
                     try {
                         l(n.next(e))
                     } catch (e) {
                         o(e)
                     }
@@ -2279,15 +2299,15 @@
                     e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                         e(t)
                     }))).then(s, a)
                 }
                 l((n = n.apply(e, t || [])).next())
             }))
         },
-        Lr = nt && nt.__generator || function(e, t) {
+        Nr = ot && ot.__generator || function(e, t) {
             var r, n, i, o, s = {
                 label: 0,
                 sent: function() {
                     if (1 & i[0]) throw i[1];
                     return i[1]
                 },
                 trys: [],
@@ -2354,64 +2374,64 @@
                             value: o[0] ? o[1] : void 0,
                             done: !0
                         }
                     }([o, a])
                 }
             }
         };
-    Object.defineProperty(Dr, "__esModule", {
+    Object.defineProperty(Cr, "__esModule", {
         value: !0
     });
-    var Nr = Et,
-        Ir = function(e) {
+    var Ir = $t,
+        Fr = function(e) {
             function t(t) {
                 var r = e.call(this) || this;
                 return r.messageHandler = function(e) {
                     r.transportRequestManager.resolveResponse(JSON.stringify(e.data))
                 }, r.uri = t, r.postMessageID = "post-message-transport-" + Math.random(), r
             }
-            return Cr(t, e), t.prototype.createWindow = function(e) {
+            return Rr(t, e), t.prototype.createWindow = function(e) {
                 var t = this;
                 return new Promise((function(r, n) {
                     var i, o = document.createElement("iframe");
                     o.setAttribute("id", t.postMessageID), o.setAttribute("width", "0px"), o.setAttribute("height", "0px"), o.setAttribute("style", "visiblity:hidden;border:none;outline:none;"), o.addEventListener("load", (function() {
                         r(i)
                     })), o.setAttribute("src", e), window.document.body.appendChild(o), i = o.contentWindow
                 }))
             }, t.prototype.connect = function() {
                 var e = this,
                     t = /^(http|https):\/\/.*$/;
                 return new Promise((function(r, n) {
-                    return Rr(e, void 0, void 0, (function() {
+                    return Lr(e, void 0, void 0, (function() {
                         var e;
-                        return Lr(this, (function(i) {
+                        return Nr(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return t.test(this.uri) || n(new Error("Bad URI")), e = this, [4, this.createWindow(this.uri)];
                                 case 1:
                                     return e.frame = i.sent(), window.addEventListener("message", this.messageHandler), r(), [2]
                             }
                         }))
                     }))
                 }))
             }, t.prototype.sendData = function(e, t) {
-                return Rr(this, void 0, void 0, (function() {
+                return Lr(this, void 0, void 0, (function() {
                     var t, r;
-                    return Lr(this, (function(n) {
-                        return t = this.transportRequestManager.addRequest(e, null), r = Nr.getNotifications(e), this.frame && (this.frame.postMessage(e.request, "*"), this.transportRequestManager.settlePendingRequest(r)), [2, t]
+                    return Nr(this, (function(n) {
+                        return t = this.transportRequestManager.addRequest(e, null), r = Ir.getNotifications(e), this.frame && (this.frame.postMessage(e.request, "*"), this.transportRequestManager.settlePendingRequest(r)), [2, t]
                     }))
                 }))
             }, t.prototype.close = function() {
                 var e = document.getElementById(this.postMessageID);
                 null == e || e.remove(), window.removeEventListener("message", this.messageHandler)
             }, t
-        }(vt.Transport);
-    Dr.default = Ir;
-    var Fr = {},
-        Mr = nt && nt.__awaiter || function(e, t, r, n) {
+        }(bt.Transport);
+    Cr.default = Fr;
+    var Mr = {},
+        Pr = ot && ot.__awaiter || function(e, t, r, n) {
             return new(r || (r = Promise))((function(i, o) {
                 function s(e) {
                     try {
                         l(n.next(e))
                     } catch (e) {
                         o(e)
                     }
@@ -2430,15 +2450,15 @@
                     e.done ? i(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
                         e(t)
                     }))).then(s, a)
                 }
                 l((n = n.apply(e, t || [])).next())
             }))
         },
-        Pr = nt && nt.__generator || function(e, t) {
+        jr = ot && ot.__generator || function(e, t) {
             var r, n, i, o, s = {
                 label: 0,
                 sent: function() {
                     if (1 & i[0]) throw i[1];
                     return i[1]
                 },
                 trys: [],
@@ -2505,41 +2525,41 @@
                             value: o[0] ? o[1] : void 0,
                             done: !0
                         }
                     }([o, a])
                 }
             }
         };
-    Object.defineProperty(Fr, "__esModule", {
+    Object.defineProperty(Mr, "__esModule", {
         value: !0
     });
-    var jr, Br, Ur, Vr, zr = function() {
+    var Br, Ur, Vr, zr, Hr = function() {
         function e(e) {
             this.requestManager = e
         }
         return e.prototype.startBatch = function() {
             return this.requestManager.startBatch()
         }, e.prototype.stopBatch = function() {
             return this.requestManager.stopBatch()
         }, e.prototype.request = function(e, t) {
-            return Mr(this, void 0, void 0, (function() {
-                return Pr(this, (function(r) {
+            return Pr(this, void 0, void 0, (function() {
+                return jr(this, (function(r) {
                     switch (r.label) {
                         case 0:
                             return this.requestManager.connectPromise ? [4, this.requestManager.connectPromise] : [3, 2];
                         case 1:
                             r.sent(), r.label = 2;
                         case 2:
                             return [2, this.requestManager.request(e, !1, t)]
                     }
                 }))
             }))
         }, e.prototype.notify = function(e) {
-            return Mr(this, void 0, void 0, (function() {
-                return Pr(this, (function(t) {
+            return Pr(this, void 0, void 0, (function() {
+                return jr(this, (function(t) {
                     switch (t.label) {
                         case 0:
                             return this.requestManager.connectPromise ? [4, this.requestManager.connectPromise] : [3, 2];
                         case 1:
                             t.sent(), t.label = 2;
                         case 2:
                             return [2, this.requestManager.request(e, !0, null)]
@@ -2550,64 +2570,64 @@
             this.requestManager.requestChannel.addListener("notification", e)
         }, e.prototype.onError = function(e) {
             this.requestManager.requestChannel.addListener("error", e)
         }, e.prototype.close = function() {
             this.requestManager.close()
         }, e
     }();
-    Fr.default = zr,
+    Mr.default = Hr,
         function(e) {
-            var t = nt && nt.__importDefault || function(e) {
+            var t = ot && ot.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.PostMessageIframeTransport = e.PostMessageWindowTransport = e.JSONRPCError = e.WebSocketTransport = e.EventEmitterTransport = e.HTTPTransport = e.RequestManager = e.Client = void 0;
-            var r = t(at);
+            var r = t(ut);
             e.RequestManager = r.default;
-            var n = t(gt);
+            var n = t(yt);
             e.EventEmitterTransport = n.default;
-            var i = t(Ct);
+            var i = t(Lt);
             e.HTTPTransport = i.default;
-            var o = t(hr);
+            var o = t(dr);
             e.WebSocketTransport = o.default;
-            var s = t(qr);
+            var s = t(Er);
             e.PostMessageWindowTransport = s.default;
-            var a = t(Dr);
+            var a = t(Cr);
             e.PostMessageIframeTransport = a.default;
-            var l = bt;
+            var l = _t;
             Object.defineProperty(e, "JSONRPCError", {
                 enumerable: !0,
                 get: function() {
                     return l.JSONRPCError
                 }
             });
-            var u = t(Fr);
+            var u = t(Mr);
             e.Client = u.default, e.default = u.default
-        }(st),
+        }(lt),
         function(e) {
             e.Retail = "retail", e.VanillaClassic = "vanilla_classic", e.Classic = "classic"
-        }(jr || (jr = {})),
+        }(Br || (Br = {})),
         function(e) {
             e.AnyFlavour = "any_flavour", e.AnyReleaseType = "any_release_type", e.VersionEq = "version_eq"
-        }(Br || (Br = {})),
+        }(Ur || (Ur = {})),
         function(e) {
             e.Html = "html", e.Markdown = "markdown", e.Raw = "raw"
-        }(Ur || (Ur = {})),
+        }(Vr || (Vr = {})),
         function(e) {
             e.toc_source_ids = "toc_source_ids", e.folder_hashes = "folder_hashes", e.folder_name_subsets = "folder_name_subsets", e.addon_names_with_folder_names = "addon_names_with_folder_names"
-        }(Vr || (Vr = {}));
-    class Hr {
+        }(zr || (zr = {}));
+    class Wr {
         constructor(e, t) {
             this._clientWrapper = e, this.profile = t
         }
         withProfile(e) {
-            return new Hr(this._clientWrapper, e)
+            return new Wr(this._clientWrapper, e)
         }
         async request(e) {
             const t = await this._clientWrapper.client;
             return await t.request(e, 0)
         }
         async readProfile(e) {
             return await this.request({
@@ -2787,24 +2807,24 @@
                 params: {
                     title: e,
                     message: t
                 }
             })
         }
     }
-    const Wr = e => ({
+    const Gr = e => ({
         source: e.source,
         alias: e.slug,
         id: e.id,
-        strategies: Object.fromEntries(Object.entries(e.options).map((([t, r]) => [t, r ? t === Br.VersionEq ? e.version : r : null])))
+        strategies: Object.fromEntries(Object.entries(e.options).map((([t, r]) => [t, r ? t === Ur.VersionEq ? e.version : r : null])))
     });
-    var Gr = {},
-        Zr = {};
+    var Zr = {},
+        Jr = {};
     ! function(e) {
-        var t = nt && nt.__awaiter || function(e, t, r, n) {
+        var t = ot && ot.__awaiter || function(e, t, r, n) {
                 return new(r || (r = Promise))((function(i, o) {
                     function s(e) {
                         try {
                             l(n.next(e))
                         } catch (e) {
                             o(e)
                         }
@@ -2822,15 +2842,15 @@
                         e.done ? i(e.value) : new r((function(t) {
                             t(e.value)
                         })).then(s, a)
                     }
                     l((n = n.apply(e, t || [])).next())
                 }))
             },
-            r = nt && nt.__generator || function(e, t) {
+            r = ot && ot.__generator || function(e, t) {
                 var r, n, i, o = {
                     label: 0,
                     sent: function() {
                         if (1 & i[0]) throw i[1];
                         return i[1]
                     },
                     trys: [],
@@ -2967,17 +2987,17 @@
                                 return [2]
                         }
                     }))
                 }))
             }, e
         }();
         e.default = n
-    }(Zr);
-    var Jr = {},
-        Yr = nt && nt.__extends || function() {
+    }(Jr);
+    var Yr = {},
+        Kr = ot && ot.__extends || function() {
             var e = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var r in t) t.hasOwnProperty(r) && (e[r] = t[r])
@@ -2985,533 +3005,533 @@
             return function(t, r) {
                 function n() {
                     this.constructor = t
                 }
                 e(t, r), t.prototype = null === r ? Object.create(r) : (n.prototype = r.prototype, new n)
             }
         }();
-    Jr.__esModule = !0;
-    var Kr, Xr, Qr, en, tn, rn = function(e) {
+    Yr.__esModule = !0;
+    var Xr, Qr, en, tn, rn, nn = function(e) {
         function t() {
             return e.call(this, 1) || this
         }
-        return Yr(t, e), t
-    }(Zr.default);
-    Jr.Lock = rn,
+        return Kr(t, e), t
+    }(Jr.default);
+    Yr.Lock = nn,
         function(e) {
             e.__esModule = !0;
-            var t = Zr;
+            var t = Jr;
             e.default = t.default,
                 function(t) {
                     for (var r in t) e.hasOwnProperty(r) || (e[r] = t[r])
-                }(Jr)
-        }(Gr);
-    Kr = new WeakMap, Xr = new WeakMap;
-    Qr = new WeakSet, en = function(e) {
+                }(Yr)
+        }(Zr);
+    Xr = new WeakMap, Qr = new WeakMap;
+    en = new WeakSet, tn = function(e) {
         return !!e && "object" == typeof e && "traceback_exception" in e
-    }, tn = function(e) {
-        if (e instanceof st.JSONRPCError && rt(this, Qr, "m", en).call(this, e.data)) {
+    }, rn = function(e) {
+        if (e instanceof lt.JSONRPCError && it(this, en, "m", tn).call(this, e.data)) {
             const t = function(e) {
                     let t;
                     return u(e, (e => t = e))(), t
-                }(ln) ?? "*",
+                }(un) ?? "*",
                 r = e.data.traceback_exception.filter(Boolean).slice(-1).join("");
-            tt.update((n => ({
+            nt.update((n => ({
                 ...n,
                 [t]: [{
                     heading: e.message,
                     message: r
                 }, ...n[t] ?? []]
             })))
         }
     };
-    const nn = (on = new class extends Hr {
+    const on = (sn = new class extends Wr {
         constructor() {
-            super(...arguments), Qr.add(this)
+            super(...arguments), en.add(this)
         }
         async request(e) {
             try {
                 return await super.request(e)
             } catch (e) {
-                throw rt(this, Qr, "m", tn).call(this, e), e
+                throw it(this, en, "m", rn).call(this, e), e
             }
         }
     }(new class {
         constructor() {
-            Kr.set(this, new Gr.Lock), Xr.set(this, void 0)
+            Xr.set(this, new Zr.Lock), Qr.set(this, void 0)
         }
         get client() {
-            return rt(this, Kr, "f").execute((() => {
+            return it(this, Xr, "f").execute((() => {
                 let e;
-                if (rt(this, Xr, "f")) {
-                    const [t, r] = rt(this, Xr, "f");
+                if (it(this, Qr, "f")) {
+                    const [t, r] = it(this, Qr, "f");
                     [WebSocket.CLOSING, WebSocket.CLOSED].includes(r.connection.readyState) || (e = t)
                 }
                 if (!e) {
-                    const t = new st.WebSocketTransport(`ws://${location.host}/api`),
-                        r = new st.RequestManager([t]);
-                    e = new st.Client(r),
+                    const t = new lt.WebSocketTransport(`ws://${location.host}/api`),
+                        r = new lt.RequestManager([t]);
+                    e = new lt.Client(r),
                         function(e, t, r, n, i) {
                             if ("m" === n) throw new TypeError("Private method is not writable");
                             if ("a" === n && !i) throw new TypeError("Private accessor was defined without a setter");
                             if ("function" == typeof t ? e !== t || !i : !t.has(e)) throw new TypeError("Cannot write private member to an object whose class did not declare it");
                             "a" === n ? i.call(e, r) : i ? i.value = r : t.set(e, r)
-                        }(this, Xr, [e, t], "f")
+                        }(this, Qr, [e, t], "f")
                 }
                 return e
             }))
         }
     }), {
-        subscribe: et(on, sn).subscribe
+        subscribe: rt(sn, an).subscribe
     });
-    var on, sn;
-    const an = et({}),
-        ln = et();
-    var un = {
+    var sn, an;
+    const ln = rt({}),
+        un = rt();
+    var cn = {
             prefix: "fas",
             iconName: "trash-can",
             icon: [448, 512, [61460, "trash-alt"], "f2ed", "M135.2 17.7C140.6 6.8 151.7 0 163.8 0H284.2c12.1 0 23.2 6.8 28.6 17.7L320 32h96c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 96 0 81.7 0 64S14.3 32 32 32h96l7.2-14.3zM32 128H416V448c0 35.3-28.7 64-64 64H96c-35.3 0-64-28.7-64-64V128zm96 64c-8.8 0-16 7.2-16 16V432c0 8.8 7.2 16 16 16s16-7.2 16-16V208c0-8.8-7.2-16-16-16zm96 0c-8.8 0-16 7.2-16 16V432c0 8.8 7.2 16 16 16s16-7.2 16-16V208c0-8.8-7.2-16-16-16zm96 0c-8.8 0-16 7.2-16 16V432c0 8.8 7.2 16 16 16s16-7.2 16-16V208c0-8.8-7.2-16-16-16z"]
         },
-        cn = {
+        fn = {
             prefix: "fas",
             iconName: "square-up-right",
             icon: [448, 512, [8599, "external-link-square-alt"], "f360", "M384 32c35.3 0 64 28.7 64 64V416c0 35.3-28.7 64-64 64H64c-35.3 0-64-28.7-64-64V96C0 60.7 28.7 32 64 32H384zM320 313.4V176c0-8.8-7.2-16-16-16H166.6c-12.5 0-22.6 10.1-22.6 22.6c0 6 2.4 11.8 6.6 16L184 232l-66.3 66.3C114 302 112 306.9 112 312s2 10 5.7 13.7l36.7 36.7c3.6 3.6 8.5 5.7 13.7 5.7s10-2 13.7-5.7L248 296l33.4 33.4c4.2 4.2 10 6.6 16 6.6c12.5 0 22.6-10.1 22.6-22.6z"]
         },
-        fn = {
+        hn = {
             prefix: "fas",
             iconName: "circle-chevron-down",
             icon: [512, 512, ["chevron-circle-down"], "f13a", "M256 0a256 256 0 1 0 0 512A256 256 0 1 0 256 0zM135 241c-9.4-9.4-9.4-24.6 0-33.9s24.6-9.4 33.9 0l87 87 87-87c9.4-9.4 24.6-9.4 33.9 0s9.4 24.6 0 33.9L273 345c-9.4 9.4-24.6 9.4-33.9 0L135 241z"]
         },
-        hn = {
+        pn = {
             prefix: "fas",
             iconName: "folder-open",
             icon: [576, 512, [128194, 128449, 61717], "f07c", "M88.7 223.8L0 375.8V96C0 60.7 28.7 32 64 32H181.5c17 0 33.3 6.7 45.3 18.7l26.5 26.5c12 12 28.3 18.7 45.3 18.7H416c35.3 0 64 28.7 64 64v32H144c-22.8 0-43.8 12.1-55.3 31.8zm27.6 16.1C122.1 230 132.6 224 144 224H544c11.5 0 22 6.1 27.7 16.1s5.7 22.2-.1 32.1l-112 192C453.9 474 443.4 480 432 480H32c-11.5 0-22-6.1-27.7-16.1s-5.7-22.2 .1-32.1l112-192z"]
         },
-        pn = {
+        dn = {
             prefix: "fas",
             iconName: "circle-chevron-up",
             icon: [512, 512, ["chevron-circle-up"], "f139", "M256 512A256 256 0 1 0 256 0a256 256 0 1 0 0 512zM377 271c9.4 9.4 9.4 24.6 0 33.9s-24.6 9.4-33.9 0l-87-87-87 87c-9.4 9.4-24.6 9.4-33.9 0s-9.4-24.6 0-33.9L239 167c9.4-9.4 24.6-9.4 33.9 0L377 271z"]
         },
-        dn = {
+        mn = {
             prefix: "fas",
             iconName: "filter",
             icon: [512, 512, [], "f0b0", "M3.9 54.9C10.5 40.9 24.5 32 40 32H472c15.5 0 29.5 8.9 36.1 22.9s4.6 30.5-5.2 42.5L320 320.9V448c0 12.1-6.8 23.2-17.7 28.6s-23.8 4.3-33.5-3l-64-48c-8.1-6-12.8-15.5-12.8-25.6V320.9L9 97.3C-.7 85.4-2.8 68.8 3.9 54.9z"]
         },
-        mn = {
+        gn = {
             prefix: "fas",
             iconName: "question",
             icon: [320, 512, [10067, 10068, 61736], "3f", "M80 160c0-35.3 28.7-64 64-64h32c35.3 0 64 28.7 64 64v3.6c0 21.8-11.1 42.1-29.4 53.8l-42.2 27.1c-25.2 16.2-40.4 44.1-40.4 74V320c0 17.7 14.3 32 32 32s32-14.3 32-32v-1.4c0-8.2 4.2-15.8 11-20.2l42.2-27.1c36.6-23.6 58.8-64.1 58.8-107.7V160c0-70.7-57.3-128-128-128H144C73.3 32 16 89.3 16 160c0 17.7 14.3 32 32 32s32-14.3 32-32zm80 320a40 40 0 1 0 0-80 40 40 0 1 0 0 80z"]
         },
-        gn = {
+        vn = {
             prefix: "fas",
             iconName: "circle-right",
             icon: [512, 512, [61838, "arrow-alt-circle-right"], "f35a", "M0 256a256 256 0 1 0 512 0A256 256 0 1 0 0 256zM294.6 135.1l99.9 107.1c3.5 3.8 5.5 8.7 5.5 13.8s-2 10.1-5.5 13.8L294.6 376.9c-4.2 4.5-10.1 7.1-16.3 7.1C266 384 256 374 256 361.7l0-57.7-96 0c-17.7 0-32-14.3-32-32l0-32c0-17.7 14.3-32 32-32l96 0 0-57.7c0-12.3 10-22.3 22.3-22.3c6.2 0 12.1 2.6 16.3 7.1z"]
         },
-        vn = {
+        yn = {
             prefix: "fas",
             iconName: "circle-left",
             icon: [512, 512, [61840, "arrow-alt-circle-left"], "f359", "M512 256A256 256 0 1 0 0 256a256 256 0 1 0 512 0zM217.4 376.9L117.5 269.8c-3.5-3.8-5.5-8.7-5.5-13.8s2-10.1 5.5-13.8l99.9-107.1c4.2-4.5 10.1-7.1 16.3-7.1c12.3 0 22.3 10 22.3 22.3l0 57.7 96 0c17.7 0 32 14.3 32 32l0 32c0 17.7-14.3 32-32 32l-96 0 0 57.7c0 12.3-10 22.3-22.3 22.3c-6.2 0-12.1-2.6-16.3-7.1z"]
         },
-        yn = {
+        bn = {
             prefix: "fas",
             iconName: "gear",
             icon: [512, 512, [9881, "cog"], "f013", "M495.9 166.6c3.2 8.7 .5 18.4-6.4 24.6l-43.3 39.4c1.1 8.3 1.7 16.8 1.7 25.4s-.6 17.1-1.7 25.4l43.3 39.4c6.9 6.2 9.6 15.9 6.4 24.6c-4.4 11.9-9.7 23.3-15.8 34.3l-4.7 8.1c-6.6 11-14 21.4-22.1 31.2c-5.9 7.2-15.7 9.6-24.5 6.8l-55.7-17.7c-13.4 10.3-28.2 18.9-44 25.4l-12.5 57.1c-2 9.1-9 16.3-18.2 17.8c-13.8 2.3-28 3.5-42.5 3.5s-28.7-1.2-42.5-3.5c-9.2-1.5-16.2-8.7-18.2-17.8l-12.5-57.1c-15.8-6.5-30.6-15.1-44-25.4L83.1 425.9c-8.8 2.8-18.6 .3-24.5-6.8c-8.1-9.8-15.5-20.2-22.1-31.2l-4.7-8.1c-6.1-11-11.4-22.4-15.8-34.3c-3.2-8.7-.5-18.4 6.4-24.6l43.3-39.4C64.6 273.1 64 264.6 64 256s.6-17.1 1.7-25.4L22.4 191.2c-6.9-6.2-9.6-15.9-6.4-24.6c4.4-11.9 9.7-23.3 15.8-34.3l4.7-8.1c6.6-11 14-21.4 22.1-31.2c5.9-7.2 15.7-9.6 24.5-6.8l55.7 17.7c13.4-10.3 28.2-18.9 44-25.4l12.5-57.1c2-9.1 9-16.3 18.2-17.8C227.3 1.2 241.5 0 256 0s28.7 1.2 42.5 3.5c9.2 1.5 16.2 8.7 18.2 17.8l12.5 57.1c15.8 6.5 30.6 15.1 44 25.4l55.7-17.7c8.8-2.8 18.6-.3 24.5 6.8c8.1 9.8 15.5 20.2 22.1 31.2l4.7 8.1c6.1 11 11.4 22.4 15.8 34.3zM256 336a80 80 0 1 0 0-160 80 80 0 1 0 0 160z"]
         },
-        bn = {
+        wn = {
             prefix: "fas",
             iconName: "sliders",
             icon: [512, 512, ["sliders-h"], "f1de", "M0 416c0 17.7 14.3 32 32 32l54.7 0c12.3 28.3 40.5 48 73.3 48s61-19.7 73.3-48L480 448c17.7 0 32-14.3 32-32s-14.3-32-32-32l-246.7 0c-12.3-28.3-40.5-48-73.3-48s-61 19.7-73.3 48L32 384c-17.7 0-32 14.3-32 32zm128 0a32 32 0 1 1 64 0 32 32 0 1 1 -64 0zM320 256a32 32 0 1 1 64 0 32 32 0 1 1 -64 0zm32-80c-32.8 0-61 19.7-73.3 48L32 224c-17.7 0-32 14.3-32 32s14.3 32 32 32l246.7 0c12.3 28.3 40.5 48 73.3 48s61-19.7 73.3-48l54.7 0c17.7 0 32-14.3 32-32s-14.3-32-32-32l-54.7 0c-12.3-28.3-40.5-48-73.3-48zM192 128a32 32 0 1 1 0-64 32 32 0 1 1 0 64zm73.3-64C253 35.7 224.8 16 192 16s-61 19.7-73.3 48L32 64C14.3 64 0 78.3 0 96s14.3 32 32 32l86.7 0c12.3 28.3 40.5 48 73.3 48s61-19.7 73.3-48L480 128c17.7 0 32-14.3 32-32s-14.3-32-32-32L265.3 64z"]
         },
-        wn = {
+        _n = {
             prefix: "fas",
             iconName: "arrow-right-arrow-left",
             icon: [448, 512, [8644, "exchange"], "f0ec", "M438.6 150.6c12.5-12.5 12.5-32.8 0-45.3l-96-96c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3L338.7 96 32 96C14.3 96 0 110.3 0 128s14.3 32 32 32l306.7 0-41.4 41.4c-12.5 12.5-12.5 32.8 0 45.3s32.8 12.5 45.3 0l96-96zm-333.3 352c12.5 12.5 32.8 12.5 45.3 0s12.5-32.8 0-45.3L109.3 416 416 416c17.7 0 32-14.3 32-32s-14.3-32-32-32l-306.7 0 41.4-41.4c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0l-96 96c-12.5 12.5-12.5 32.8 0 45.3l96 96z"]
         },
-        _n = {
+        kn = {
             prefix: "fas",
             iconName: "ellipsis",
             icon: [448, 512, ["ellipsis-h"], "f141", "M8 256a56 56 0 1 1 112 0A56 56 0 1 1 8 256zm160 0a56 56 0 1 1 112 0 56 56 0 1 1 -112 0zm216-56a56 56 0 1 1 0 112 56 56 0 1 1 0-112z"]
         },
-        kn = {
+        xn = {
             prefix: "fas",
             iconName: "table-list",
             icon: [512, 512, ["th-list"], "f00b", "M0 96C0 60.7 28.7 32 64 32H448c35.3 0 64 28.7 64 64V416c0 35.3-28.7 64-64 64H64c-35.3 0-64-28.7-64-64V96zm64 0v64h64V96H64zm384 0H192v64H448V96zM64 224v64h64V224H64zm384 0H192v64H448V224zM64 352v64h64V352H64zm384 0H192v64H448V352z"]
         },
-        xn = {
+        An = {
             prefix: "fas",
             iconName: "circle-xmark",
             icon: [512, 512, [61532, "times-circle", "xmark-circle"], "f057", "M256 512A256 256 0 1 0 256 0a256 256 0 1 0 0 512zM175 175c9.4-9.4 24.6-9.4 33.9 0l47 47 47-47c9.4-9.4 24.6-9.4 33.9 0s9.4 24.6 0 33.9l-47 47 47 47c9.4 9.4 9.4 24.6 0 33.9s-24.6 9.4-33.9 0l-47-47-47 47c-9.4 9.4-24.6 9.4-33.9 0s-9.4-24.6 0-33.9l47-47-47-47c-9.4-9.4-9.4-24.6 0-33.9z"]
         };
 
-    function An(e) {
+    function qn(e) {
         e[16] = e[17].access_tokens
     }
 
-    function qn(e) {
+    function En(e) {
         e[18] = e[17].verification_uri, e[19] = e[17].user_code
     }
 
-    function En(t) {
+    function Tn(t) {
         return {
             c: e,
             m: e,
             p: e,
             d: e
         }
     }
 
-    function Tn(e) {
+    function $n(e) {
         let t, r, n, i, s, a, l;
-        An(e);
-        let u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, E, T, S, C, N, j, B, V, z, H, W, G, Z, J, Y, K, X, Q, ee, te = null === e[16].github ? "generate" : "regenerate";
+        qn(e);
+        let u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, q, T, $, D, R, I, B, U, z, H, W, G, Z, J, Y, K, X, Q, ee, te = null === e[16].github ? "generate" : "regenerate";
 
         function re(e, t) {
-            return e[0] ? On : $n
+            return e[0] ? Sn : On
         }
         let ne = re(e),
             ie = ne(e);
         return {
             c() {
-                t = D("div"), t.textContent = "access tokens", r = L(), n = D("div"), i = D("div"), i.textContent = "GitHub:", s = L(), a = D("div"), l = D("button"), u = R(te), c = L(), f = D("div"), ie.c(), h = L(), p = D("label"), p.textContent = "CFCore:", d = L(), m = D("div"), g = D("input"), y = L(), b = D("button"), w = R("update"), k = L(), x = D("div"), A = R("A CFCore access token is required to use CurseForge. Log in to\n          "), E = D("button"), E.textContent = "CFCore", T = R(" to generate an access token."), S = L(), C = D("label"), C.textContent = "Wago:", N = L(), j = D("div"), B = D("input"), z = L(), H = D("button"), W = R("update"), Z = L(), J = D("div"), Y = R("An access token is required to use Wago Addons. Wago issues tokens to some\n          "), K = D("button"), K.textContent = "Patreon", X = R(" subscribers."), P(t, "class", "section-header svelte-vgp2pk"), P(i, "class", "label-like svelte-vgp2pk"), P(l, "class", "form-control"), l.disabled = e[0], P(f, "class", "description svelte-vgp2pk"), P(a, "class", "value-rows svelte-vgp2pk"), P(p, "for", "__cfcore-input-box"), P(p, "class", "svelte-vgp2pk"), P(g, "id", "__cfcore-input-box"), P(g, "class", "form-control"), P(g, "type", "password"), g.value = v = e[16].cfcore, P(b, "class", "form-control primary"), b.disabled = _ = void 0 === e[1], P(E, "role", "link"), P(x, "class", "description svelte-vgp2pk"), P(m, "class", "value-rows svelte-vgp2pk"), P(C, "for", "__wago-input-box"), P(C, "class", "svelte-vgp2pk"), P(B, "id", "__wago-input-box"), P(B, "class", "form-control"), P(B, "type", "password"), B.value = V = e[16].wago_addons, P(H, "class", "form-control primary"), H.disabled = G = void 0 === e[2], P(K, "role", "link"), P(J, "class", "description svelte-vgp2pk"), P(j, "class", "value-rows svelte-vgp2pk"), P(n, "class", "row form-grid svelte-vgp2pk")
+                t = C("div"), t.textContent = "access tokens", r = N(), n = C("div"), i = C("div"), i.textContent = "GitHub:", s = N(), a = C("div"), l = C("button"), u = L(te), c = N(), f = C("div"), ie.c(), h = N(), p = C("label"), p.textContent = "CFCore:", d = N(), m = C("div"), g = C("input"), y = N(), b = C("button"), w = L("update"), k = N(), x = C("div"), A = L("A CFCore access token is required to use CurseForge. Log in to\n          "), q = C("button"), q.textContent = "CFCore", T = L(" to generate an access token."), $ = N(), D = C("label"), D.textContent = "Wago:", R = N(), I = C("div"), B = C("input"), z = N(), H = C("button"), W = L("update"), Z = N(), J = C("div"), Y = L("An access token is required to use Wago Addons. Wago issues tokens to some\n          "), K = C("button"), K.textContent = "Patreon", X = L(" subscribers."), j(t, "class", "section-header svelte-vgp2pk"), j(i, "class", "label-like svelte-vgp2pk"), j(l, "class", "form-control"), l.disabled = e[0], j(f, "class", "description svelte-vgp2pk"), j(a, "class", "value-rows svelte-vgp2pk"), j(p, "for", "__cfcore-input-box"), j(p, "class", "svelte-vgp2pk"), j(g, "id", "__cfcore-input-box"), j(g, "class", "form-control"), j(g, "type", "password"), g.value = v = e[16].cfcore, j(b, "class", "form-control primary"), b.disabled = _ = void 0 === e[1], j(q, "role", "link"), j(x, "class", "description svelte-vgp2pk"), j(m, "class", "value-rows svelte-vgp2pk"), j(D, "for", "__wago-input-box"), j(D, "class", "svelte-vgp2pk"), j(B, "id", "__wago-input-box"), j(B, "class", "form-control"), j(B, "type", "password"), B.value = U = e[16].wago_addons, j(H, "class", "form-control primary"), H.disabled = G = void 0 === e[2], j(K, "role", "link"), j(J, "class", "description svelte-vgp2pk"), j(I, "class", "value-rows svelte-vgp2pk"), j(n, "class", "row form-grid svelte-vgp2pk")
             },
             m(o, v) {
-                $(o, t, v), $(o, r, v), $(o, n, v), q(n, i), q(n, s), q(n, a), q(a, l), q(l, u), q(a, c), q(a, f), ie.m(f, null), q(n, h), q(n, p), q(n, d), q(n, m), q(m, g), q(m, y), q(m, b), q(b, w), q(m, k), q(m, x), q(x, A), q(x, E), q(x, T), q(n, S), q(n, C), q(n, N), q(n, j), q(j, B), q(j, z), q(j, H), q(H, W), q(j, Z), q(j, J), q(J, Y), q(J, K), q(J, X), Q || (ee = [I(l, "click", e[8]), I(g, "input", e[10]), I(b, "click", e[11]), I(E, "click", M(F(e[12]))), I(B, "input", e[13]), I(H, "click", e[14]), I(K, "click", M(F(e[15])))], Q = !0)
+                O(o, t, v), O(o, r, v), O(o, n, v), E(n, i), E(n, s), E(n, a), E(a, l), E(l, u), E(a, c), E(a, f), ie.m(f, null), E(n, h), E(n, p), E(n, d), E(n, m), E(m, g), E(m, y), E(m, b), E(b, w), E(m, k), E(m, x), E(x, A), E(x, q), E(x, T), E(n, $), E(n, D), E(n, R), E(n, I), E(I, B), E(I, z), E(I, H), E(H, W), E(I, Z), E(I, J), E(J, Y), E(J, K), E(J, X), Q || (ee = [F(l, "click", e[8]), F(g, "input", e[10]), F(b, "click", e[11]), F(q, "click", P(M(e[12]))), F(B, "input", e[13]), F(H, "click", e[14]), F(K, "click", P(M(e[15])))], Q = !0)
             },
             p(e, t) {
-                An(e), 8 & t && te !== (te = null === e[16].github ? "generate" : "regenerate") && U(u, te), 1 & t && (l.disabled = e[0]), ne === (ne = re(e)) && ie ? ie.p(e, t) : (ie.d(1), ie = ne(e), ie && (ie.c(), ie.m(f, null))), 8 & t && v !== (v = e[16].cfcore) && g.value !== v && (g.value = v), 2 & t && _ !== (_ = void 0 === e[1]) && (b.disabled = _), 8 & t && V !== (V = e[16].wago_addons) && B.value !== V && (B.value = V), 4 & t && G !== (G = void 0 === e[2]) && (H.disabled = G)
+                qn(e), 8 & t && te !== (te = null === e[16].github ? "generate" : "regenerate") && V(u, te), 1 & t && (l.disabled = e[0]), ne === (ne = re(e)) && ie ? ie.p(e, t) : (ie.d(1), ie = ne(e), ie && (ie.c(), ie.m(f, null))), 8 & t && v !== (v = e[16].cfcore) && g.value !== v && (g.value = v), 2 & t && _ !== (_ = void 0 === e[1]) && (b.disabled = _), 8 & t && U !== (U = e[16].wago_addons) && B.value !== U && (B.value = U), 4 & t && G !== (G = void 0 === e[2]) && (H.disabled = G)
             },
             d(e) {
-                e && O(t), e && O(r), e && O(n), ie.d(), Q = !1, o(ee)
+                e && (S(t), S(r), S(n)), ie.d(), Q = !1, o(ee)
             }
         }
     }
 
-    function $n(t) {
+    function On(t) {
         let r;
         return {
             c() {
-                r = R("Generate a GitHub access token to increase your hourly limit from 60 to 5,000 requests.")
+                r = L("Generate a GitHub access token to increase your hourly limit from 60 to 5,000 requests.")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function On(e) {
+    function Sn(e) {
         let t, r, n = {
             ctx: e,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: Fn,
-            then: Dn,
-            catch: Sn,
+            pending: Mn,
+            then: Cn,
+            catch: Dn,
             value: 17
         };
-        return Le(r = e[3].initiateGithubAuthFlow(), n), {
+        return Ne(r = e[3].initiateGithubAuthFlow(), n), {
             c() {
-                t = N(), n.block.c()
+                t = I(), n.block.c()
             },
             m(e, r) {
-                $(e, t, r), n.block.m(e, n.anchor = r), n.mount = () => t.parentNode, n.anchor = t
+                O(e, t, r), n.block.m(e, n.anchor = r), n.mount = () => t.parentNode, n.anchor = t
             },
             p(t, i) {
-                e = t, n.ctx = e, 8 & i && r !== (r = e[3].initiateGithubAuthFlow()) && Le(r, n) || Ne(n, e, i)
+                e = t, n.ctx = e, 8 & i && r !== (r = e[3].initiateGithubAuthFlow()) && Ne(r, n) || Ie(n, e, i)
             },
             d(e) {
-                e && O(t), n.block.d(e), n.token = null, n = null
+                e && S(t), n.block.d(e), n.token = null, n = null
             }
         }
     }
 
-    function Sn(t) {
+    function Dn(t) {
         return {
             c: e,
             m: e,
             p: e,
             d: e
         }
     }
 
-    function Dn(e) {
+    function Cn(e) {
         let t;
-        qn(e);
+        En(e);
         let r = {
             ctx: e,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: In,
-            then: Rn,
-            catch: Cn,
+            pending: Fn,
+            then: Ln,
+            catch: Rn,
             value: 20
         };
-        return Le(e[6](), r), {
+        return Ne(e[6](), r), {
             c() {
-                t = N(), r.block.c()
+                t = I(), r.block.c()
             },
             m(e, n) {
-                $(e, t, n), r.block.m(e, r.anchor = n), r.mount = () => t.parentNode, r.anchor = t
+                O(e, t, n), r.block.m(e, r.anchor = n), r.mount = () => t.parentNode, r.anchor = t
             },
             p(t, n) {
-                qn(e = t), Ne(r, e, n)
+                En(e = t), Ie(r, e, n)
             },
             d(e) {
-                e && O(t), r.block.d(e), r.token = null, r = null
+                e && S(t), r.block.d(e), r.token = null, r = null
             }
         }
     }
 
-    function Cn(t) {
+    function Rn(t) {
         return {
             c: e,
             m: e,
             p: e,
             d: e
         }
     }
 
-    function Rn(t) {
+    function Ln(t) {
         let r;
         let n = function(e, t) {
-                return "success" === e[20] ? Nn : "failure" === e[20] ? Ln : void 0
+                return "success" === e[20] ? In : "failure" === e[20] ? Nn : void 0
             }(t),
             i = n && n(t);
         return {
             c() {
-                i && i.c(), r = N()
+                i && i.c(), r = I()
             },
             m(e, t) {
-                i && i.m(e, t), $(e, r, t)
+                i && i.m(e, t), O(e, r, t)
             },
             p: e,
             d(e) {
-                i && i.d(e), e && O(r)
+                e && S(r), i && i.d(e)
             }
         }
     }
 
-    function Ln(e) {
+    function Nn(e) {
         let t;
         return {
             c() {
-                t = R("Authentication failed.")
+                t = L("Authentication failed.")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function Nn(e) {
+    function In(e) {
         let t;
         return {
             c() {
-                t = R("Authenticated.")
+                t = L("Authenticated.")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function In(e) {
+    function Fn(e) {
         let t, r, n, i, o, s, a, l, u, c = e[18] + "",
             f = e[19] + "";
 
         function h() {
             return e[9](e[18])
         }
         return {
             c() {
-                t = R("Navigate to\n                "), r = D("button"), n = R(c), i = R('\n                and insert the following code to authenticate with instawow: "'), o = D("code"), s = R(f), a = R('".'), P(r, "role", "link")
+                t = L("Navigate to\n                "), r = C("button"), n = L(c), i = L('\n                and insert the following code to authenticate with instawow: "'), o = C("code"), s = L(f), a = L('".'), j(r, "role", "link")
             },
             m(e, c) {
-                $(e, t, c), $(e, r, c), q(r, n), $(e, i, c), $(e, o, c), q(o, s), $(e, a, c), l || (u = I(r, "click", M(F(h))), l = !0)
+                O(e, t, c), O(e, r, c), E(r, n), O(e, i, c), O(e, o, c), E(o, s), O(e, a, c), l || (u = F(r, "click", P(M(h))), l = !0)
             },
             p(t, r) {
-                e = t, 8 & r && c !== (c = e[18] + "") && U(n, c), 8 & r && f !== (f = e[19] + "") && U(s, f)
+                e = t, 8 & r && c !== (c = e[18] + "") && V(n, c), 8 & r && f !== (f = e[19] + "") && V(s, f)
             },
             d(e) {
-                e && O(t), e && O(r), e && O(i), e && O(o), e && O(a), l = !1, u()
+                e && (S(t), S(r), S(i), S(o), S(a)), l = !1, u()
             }
         }
     }
 
-    function Fn(t) {
+    function Mn(t) {
         let r;
         return {
             c() {
-                r = R("Initiating authorisation flow...")
+                r = L("Initiating authorisation flow...")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Mn(t) {
+    function Pn(t) {
         let r;
         return {
             c() {
-                r = D("div"), r.textContent = "Loading...", P(r, "class", "row")
+                r = C("div"), r.textContent = "Loading...", j(r, "class", "row")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Pn(t) {
+    function jn(t) {
         let r, n, i, o, s, a, l = {
             ctx: t,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: Mn,
-            then: Tn,
-            catch: En,
+            pending: Pn,
+            then: $n,
+            catch: Tn,
             value: 17
         };
-        return Le(o = t[3].readGlobalConfig(), l), {
+        return Ne(o = t[3].readGlobalConfig(), l), {
             c() {
-                r = D("div"), r.textContent = "config", n = L(), i = D("form"), l.block.c(), P(r, "class", "title-bar"), P(i, "class", "content svelte-vgp2pk")
+                r = C("div"), r.textContent = "config", n = N(), i = C("form"), l.block.c(), j(r, "class", "title-bar"), j(i, "class", "content svelte-vgp2pk")
             },
             m(e, o) {
-                $(e, r, o), $(e, n, o), $(e, i, o), l.block.m(i, l.anchor = null), l.mount = () => i, l.anchor = null, s || (a = I(i, "submit", F(t[7])), s = !0)
+                O(e, r, o), O(e, n, o), O(e, i, o), l.block.m(i, l.anchor = null), l.mount = () => i, l.anchor = null, s || (a = F(i, "submit", M(t[7])), s = !0)
             },
             p(e, [r]) {
-                t = e, l.ctx = t, 8 & r && o !== (o = t[3].readGlobalConfig()) && Le(o, l) || Ne(l, t, r)
+                t = e, l.ctx = t, 8 & r && o !== (o = t[3].readGlobalConfig()) && Ne(o, l) || Ie(l, t, r)
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(n), e && O(i), l.block.d(), l.token = null, l = null, s = !1, a()
+                e && (S(r), S(n), S(i)), l.block.d(), l.token = null, l = null, s = !1, a()
             }
         }
     }
 
-    function jn(e, t, r) {
+    function Bn(e, t, r) {
         let n;
-        c(e, nn, (e => r(3, n = e)));
+        c(e, on, (e => r(3, n = e)));
         let i, o, s = !1;
         const a = async () => {
             await n.updateGlobalConfig({
                 cfcore: i
             })
         }, l = async () => {
             await n.updateGlobalConfig({
                 wago_addons: o
             })
         };
         var u;
         u = () => {
             n.cancelGithubAuthFlow()
-        }, ie().$$.on_destroy.push(u);
+        }, oe().$$.on_destroy.push(u);
         return [s, i, o, n, a, l, async () => {
                 const {
                     status: e
                 } = await n.queryGithubAuthFlowStatus();
                 return r(0, s = !1), e
             },
             function(t) {
-                ue.call(this, e, t)
+                ce.call(this, e, t)
             }, () => r(0, s = !0), e => n.openUrl(e), e => r(1, i = e.currentTarget.value || null), () => a(), () => n.openUrl("https://console.curseforge.com/"), e => r(2, o = e.currentTarget.value || null), () => l(), () => n.openUrl("https://addons.wago.io/patreon")]
     }
-    class Bn extends Ze {
+    class Un extends Ye {
         constructor(e) {
-            super(), Ge(this, e, jn, Pn, a, {})
+            super(), Je(this, e, Bn, jn, a, {})
         }
     }
 
-    function Un(e) {
+    function Vn(e) {
         let t, r, n, i, s, a, l;
         const u = e[3].default,
             c = f(u, e, e[2], null);
         return {
             c() {
-                t = D("div"), r = D("dialog"), c && c.c(), r.open = !0, P(r, "class", "modal svelte-jd3rlo"), P(r, "aria-modal", "true"), P(t, "class", "modal-wrapper svelte-jd3rlo")
+                t = C("div"), r = C("dialog"), c && c.c(), r.open = !0, j(r, "class", "modal svelte-jd3rlo"), j(r, "aria-modal", "true"), j(t, "class", "modal-wrapper svelte-jd3rlo")
             },
             m(n, i) {
-                $(n, t, i), q(t, r), c && c.m(r, null), s = !0, a || (l = [I(window, "keydown", e[1]), I(r, "click", M(e[4])), I(t, "click", e[0])], a = !0)
+                O(n, t, i), E(t, r), c && c.m(r, null), s = !0, a || (l = [F(window, "keydown", e[1]), F(r, "click", P(e[4])), F(t, "click", e[0])], a = !0)
             },
             p(e, [t]) {
                 c && c.p && (!s || 4 & t) && d(c, u, e, e[2], s ? p(u, e[2], t, null) : m(e[2]), null)
             },
             i(e) {
-                s || (Oe(c, e), n || ge((() => {
-                    n = Ce(r, Xe, {
+                s || (Se(c, e), e && (n || ve((() => {
+                    n = Re(r, et, {
                         duration: 200
                     }), n.start()
-                })), ge((() => {
-                    s && (i || (i = Re(t, Ye, {
+                }))), e && ve((() => {
+                    s && (i || (i = Le(t, Xe, {
                         duration: 200
                     }, !0)), i.run(1))
                 })), s = !0)
             },
             o(e) {
-                Se(c, e), i || (i = Re(t, Ye, {
+                De(c, e), e && (i || (i = Le(t, Xe, {
                     duration: 200
-                }, !1)), i.run(0), s = !1
+                }, !1)), i.run(0)), s = !1
             },
             d(e) {
-                e && O(t), c && c.d(e), e && i && i.end(), a = !1, o(l)
+                e && S(t), c && c.d(e), e && i && i.end(), a = !1, o(l)
             }
         }
     }
 
-    function Vn(e, t, r) {
+    function zn(e, t, r) {
         let {
             $$slots: n = {},
             $$scope: i
         } = t;
-        const o = se(),
+        const o = ae(),
             s = () => {
                 o("dismiss")
             };
-        return ae("modal", {
+        return le("modal", {
             dismiss: s
         }), e.$$set = e => {
             "$$scope" in e && r(2, i = e.$$scope)
         }, [s, e => {
             "Escape" === e.key && (s(), e.preventDefault())
         }, i, n, function(t) {
-            ue.call(this, e, t)
+            ce.call(this, e, t)
         }]
     }
-    class zn extends Ze {
+    class Hn extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Vn, Un, a, {
+            super(), Je(this, e, zn, Vn, a, {
                 dismiss: 0
             })
         }
         get dismiss() {
             return this.$$.ctx[0]
         }
     }
-    var Hn = {
+    var Wn = {
         exports: {}
     };
     /**
      * @license
      * Lodash <https://lodash.com/>
      * Copyright OpenJS Foundation and other contributors <https://openjsf.org/>
      * Released under MIT license <https://lodash.com/license>
@@ -3634,16 +3654,16 @@
                 Ye = "(?:" + [Le, Pe, je].join("|") + ")" + Je,
                 Ke = "(?:" + [Me + Ce + "?", Ce, Pe, je, Se].join("|") + ")",
                 Xe = RegExp(Oe, "g"),
                 Qe = RegExp(Ce, "g"),
                 et = RegExp(Fe + "(?=" + Fe + ")|" + Ke + Je, "g"),
                 tt = RegExp([Be + "?" + Ne + "+" + He + "(?=" + [De, Be, "$"].join("|") + ")", ze + "+" + We + "(?=" + [De, Be + Ve, "$"].join("|") + ")", Be + "?" + Ve + "+" + He, Be + "+" + We, "\\d*(?:1ST|2ND|3RD|(?![123])\\dTH)(?=\\b|[a-z_])", "\\d*(?:1st|2nd|3rd|(?![123])\\dth)(?=\\b|[A-Z_])", Re, Ye].join("|"), "g"),
                 rt = RegExp("[" + Ue + ke + xe + Te + "]"),
-                it = /[a-z][A-Z]|[A-Z]{2}[a-z]|[0-9][a-zA-Z]|[a-zA-Z][0-9]|[^a-zA-Z0-9 ]/,
-                ot = ["Array", "Buffer", "DataView", "Date", "Error", "Float32Array", "Float64Array", "Function", "Int8Array", "Int16Array", "Int32Array", "Map", "Math", "Object", "Promise", "RegExp", "Set", "String", "Symbol", "TypeError", "Uint8Array", "Uint8ClampedArray", "Uint16Array", "Uint32Array", "WeakMap", "_", "clearTimeout", "isFinite", "parseInt", "setTimeout"],
+                nt = /[a-z][A-Z]|[A-Z]{2}[a-z]|[0-9][a-zA-Z]|[a-zA-Z][0-9]|[^a-zA-Z0-9 ]/,
+                it = ["Array", "Buffer", "DataView", "Date", "Error", "Float32Array", "Float64Array", "Function", "Int8Array", "Int16Array", "Int32Array", "Map", "Math", "Object", "Promise", "RegExp", "Set", "String", "Symbol", "TypeError", "Uint8Array", "Uint8ClampedArray", "Uint16Array", "Uint32Array", "WeakMap", "_", "clearTimeout", "isFinite", "parseInt", "setTimeout"],
                 st = -1,
                 at = {};
             at[L] = at[N] = at[I] = at[F] = at[M] = at[P] = at[j] = at[B] = at[U] = !0, at[g] = at[v] = at[C] = at[y] = at[R] = at[b] = at[w] = at[_] = at[x] = at[A] = at[q] = at[T] = at[$] = at[O] = at[D] = !1;
             var lt = {};
             lt[g] = lt[v] = lt[C] = lt[R] = lt[y] = lt[b] = lt[L] = lt[N] = lt[I] = lt[F] = lt[M] = lt[x] = lt[A] = lt[q] = lt[T] = lt[$] = lt[O] = lt[S] = lt[P] = lt[j] = lt[B] = lt[U] = !0, lt[w] = lt[_] = lt[D] = !1;
             var ut = {
                     "\\": "\\",
@@ -3651,15 +3671,15 @@
                     "\n": "n",
                     "\r": "r",
                     "\u2028": "u2028",
                     "\u2029": "u2029"
                 },
                 ct = parseFloat,
                 ft = parseInt,
-                ht = "object" == typeof nt && nt && nt.Object === Object && nt,
+                ht = "object" == typeof ot && ot && ot.Object === Object && ot,
                 pt = "object" == typeof self && self && self.Object === Object && self,
                 dt = ht || pt || Function("return this")(),
                 mt = t && !t.nodeType && t,
                 gt = mt && e && !e.nodeType && e,
                 vt = gt && gt.exports === mt,
                 yt = vt && ht.process,
                 bt = function() {
@@ -4129,15 +4149,15 @@
                 "&amp;": "&",
                 "&lt;": "<",
                 "&gt;": ">",
                 "&quot;": '"',
                 "&#39;": "'"
             });
             var gr = function e(t) {
-                var oe, ke = (t = null == t ? dt : gr.defaults(dt.Object(), t, gr.pick(dt, ot))).Array,
+                var oe, ke = (t = null == t ? dt : gr.defaults(dt.Object(), t, gr.pick(dt, it))).Array,
                     xe = t.Date,
                     Ae = t.Error,
                     qe = t.Function,
                     Ee = t.Math,
                     Te = t.Object,
                     $e = t.RegExp,
                     Oe = t.String,
@@ -4161,15 +4181,15 @@
                     Ge = lr(Te.getPrototypeOf, Te),
                     Ze = Te.create,
                     Je = Re.propertyIsEnumerable,
                     Ye = De.splice,
                     Ke = ze ? ze.isConcatSpreadable : r,
                     et = ze ? ze.iterator : r,
                     rt = ze ? ze.toStringTag : r,
-                    nt = function() {
+                    ot = function() {
                         try {
                             var e = ho(Te, "defineProperty");
                             return e({}, "", {}), e
                         } catch (e) {}
                     }(),
                     ut = t.clearTimeout !== dt.clearTimeout && t.clearTimeout,
                     ht = xe && xe.now !== dt.Date.now && xe.now,
@@ -4317,15 +4337,15 @@
                 }
 
                 function on(e, t) {
                     return e && Di(t, Ca(t), e)
                 }
 
                 function sn(e, t, r) {
-                    "__proto__" == t && nt ? nt(e, t, {
+                    "__proto__" == t && ot ? ot(e, t, {
                         configurable: !0,
                         enumerable: !0,
                         value: r,
                         writable: !0
                     }) : e[t] = r
                 }
 
@@ -4976,16 +4996,16 @@
                         tn(l, u, c), l = l[u]
                     }
                     return e
                 }
                 var ti = Sr ? function(e, t) {
                         return Sr.set(e, t), e
                     } : il,
-                    ri = nt ? function(e, t) {
-                        return nt(e, "toString", {
+                    ri = ot ? function(e, t) {
+                        return ot(e, "toString", {
                             configurable: !0,
                             enumerable: !1,
                             value: tl(t),
                             writable: !0
                         })
                     } : il;
 
@@ -6386,15 +6406,15 @@
                 var Ya = Fi((function(e, t, r) {
                         return e + (r ? " " : "") + t.toUpperCase()
                     })),
                     Ka = Ii("toUpperCase");
 
                 function Xa(e, t, n) {
                     return e = ba(e), (t = n ? r : t) === r ? function(e) {
-                        return it.test(e)
+                        return nt.test(e)
                     }(e) ? function(e) {
                         return e.match(tt) || []
                     }(e) : function(e) {
                         return e.match(ue) || []
                     }(e) : e.match(t) || []
                 }
                 var Qa = Kn((function(e, t) {
@@ -7234,58 +7254,58 @@
                 }, jr.prototype.toJSON = jr.prototype.valueOf = jr.prototype.value = function() {
                     return mi(this.__wrapped__, this.__actions__)
                 }, jr.prototype.first = jr.prototype.head, et && (jr.prototype[et] = function() {
                     return this
                 }), jr
             }();
             gt ? ((gt.exports = gr)._ = gr, mt._ = gr) : dt._ = gr
-        }).call(nt)
-    }(Hn, Hn.exports);
-    var Wn = Hn.exports,
-        Gn = it(Wn);
+        }).call(ot)
+    }(Wn, Wn.exports);
+    var Gn = Wn.exports,
+        Zn = st(Gn);
 
-    function Zn(t) {
+    function Jn(t) {
         let n, i, o, s, a = [{
                 width: t[0]
             }, {
                 height: t[1]
             }, {
                 viewBox: o = "0 0 " + t[0] + " " + t[1]
             }, {
                 class: s = "icon " + t[3] + "-" + t[2]
             }, t[5]],
             l = {};
         for (let e = 0; e < a.length; e += 1) l = r(l, a[e]);
         return {
             c() {
-                n = C("svg"), i = C("path"), P(i, "d", t[4]), j(n, l)
+                n = R("svg"), i = R("path"), j(i, "d", t[4]), B(n, l)
             },
             m(e, t) {
-                $(e, n, t), q(n, i)
+                O(e, n, t), E(n, i)
             },
             p(e, [t]) {
-                j(n, l = je(a, [{
+                B(n, l = Ue(a, [{
                     width: e[0]
                 }, {
                     height: e[1]
                 }, {
                     viewBox: o
                 }, {
                     class: s
                 }, 32 & t && e[5]]))
             },
             i: e,
             o: e,
             d(e) {
-                e && O(n)
+                e && S(n)
             }
         }
     }
 
-    function Jn(e, t, n) {
+    function Yn(e, t, n) {
         const i = ["icon"];
         let o = g(t, i),
             {
                 icon: s
             } = t;
         const {
             icon: [a, l, , , u],
@@ -7296,220 +7316,220 @@
             t = r(r({}, t), function(e) {
                 const t = {};
                 for (const r in e) "$" !== r[0] && (t[r] = e[r]);
                 return t
             }(e)), n(5, o = g(t, i)), "icon" in e && n(6, s = e.icon)
         }, [a, l, c, f, h, o, s]
     }
-    class Yn extends Ze {
+    class Kn extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Jn, Zn, l, {
+            super(), Je(this, e, Yn, Jn, l, {
                 icon: 6
             })
         }
     }
 
-    function Kn(e, t, r) {
+    function Xn(e, t, r) {
         const n = e.slice();
         return n[18] = t[r], n
     }
 
-    function Xn(e) {
+    function Qn(e) {
         let t, r, n = e[3].get("profile") + "";
         return {
             c() {
-                t = D("div"), r = R(n), P(t, "class", "row error-text")
+                t = C("div"), r = L(n), j(t, "class", "row error-text")
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, t) {
-                8 & t && n !== (n = e[3].get("profile") + "") && U(r, n)
+                8 & t && n !== (n = e[3].get("profile") + "") && V(r, n)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function Qn(e) {
+    function ei(e) {
         let t, r, n = e[3].get("addon_dir") + "";
         return {
             c() {
-                t = D("div"), r = R(n), P(t, "class", "row error-text")
+                t = C("div"), r = L(n), j(t, "class", "row error-text")
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, t) {
-                8 & t && n !== (n = e[3].get("addon_dir") + "") && U(r, n)
+                8 & t && n !== (n = e[3].get("addon_dir") + "") && V(r, n)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function ei(e) {
+    function ti(e) {
         let t, r, n = e[3].get("game_flavour") + "";
         return {
             c() {
-                t = D("div"), r = R(n), P(t, "class", "row error-text")
+                t = C("div"), r = L(n), j(t, "class", "row error-text")
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, t) {
-                8 & t && n !== (n = e[3].get("game_flavour") + "") && U(r, n)
+                8 & t && n !== (n = e[3].get("game_flavour") + "") && V(r, n)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function ti(t) {
+    function ri(t) {
         let r, n, i = t[18] + "";
         return {
             c() {
-                r = D("option"), n = R(i), r.__value = t[18], r.value = r.__value
+                r = C("option"), n = L(i), r.__value = t[18], z(r, r.__value)
             },
             m(e, t) {
-                $(e, r, t), q(r, n)
+                O(e, r, t), E(r, n)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function ri(t) {
+    function ni(t) {
         let r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x = t[3].has("profile"),
             A = t[3].has("addon_dir"),
-            E = x && Xn(t),
+            q = x && Qn(t),
             T = t[4] && function(e) {
                 let t, r, n;
                 return {
                     c() {
-                        t = D("input"), P(t, "aria-label", "profile"), P(t, "class", "row form-control"), P(t, "type", "text"), P(t, "placeholder", "profile"), J(t, "error", e[3].has("profile"))
+                        t = C("input"), j(t, "aria-label", "profile"), j(t, "class", "row form-control"), j(t, "type", "text"), j(t, "placeholder", "profile"), Y(t, "error", e[3].has("profile"))
                     },
                     m(i, o) {
-                        $(i, t, o), V(t, e[0]), r || (n = I(t, "input", e[10]), r = !0)
+                        O(i, t, o), z(t, e[0]), r || (n = F(t, "input", e[10]), r = !0)
                     },
                     p(e, r) {
-                        1 & r && t.value !== e[0] && V(t, e[0]), 8 & r && J(t, "error", e[3].has("profile"))
+                        1 & r && t.value !== e[0] && z(t, e[0]), 8 & r && Y(t, "error", e[3].has("profile"))
                     },
                     d(e) {
-                        e && O(t), r = !1, n()
+                        e && S(t), r = !1, n()
                     }
                 }
             }(t),
-            C = A && Qn(t);
-        p = new Yn({
+            $ = A && ei(t);
+        p = new Kn({
             props: {
-                icon: hn
+                icon: pn
             }
         });
         let R = !t[4] && function(e) {
                 let t, r, n, i, o = e[3].has("game_flavour"),
-                    s = o && ei(e),
-                    a = Object.values(jr),
+                    s = o && ti(e),
+                    a = Fe(Object.values(Br)),
                     l = [];
-                for (let t = 0; t < a.length; t += 1) l[t] = ti(Kn(e, a, t));
+                for (let t = 0; t < a.length; t += 1) l[t] = ri(Xn(e, a, t));
                 return {
                     c() {
-                        s && s.c(), t = L(), r = D("select");
+                        s && s.c(), t = N(), r = C("select");
                         for (let e = 0; e < l.length; e += 1) l[e].c();
-                        P(r, "aria-label", "game flavour"), P(r, "class", "row form-control"), void 0 === e[2] && ge((() => e[12].call(r))), J(r, "error", e[3].has("game_flavour"))
+                        j(r, "aria-label", "game flavour"), j(r, "class", "row form-control"), void 0 === e[2] && ve((() => e[12].call(r))), Y(r, "error", e[3].has("game_flavour"))
                     },
                     m(o, a) {
-                        s && s.m(o, a), $(o, t, a), $(o, r, a);
+                        s && s.m(o, a), O(o, t, a), O(o, r, a);
                         for (let e = 0; e < l.length; e += 1) l[e] && l[e].m(r, null);
-                        z(r, e[2], !0), n || (i = I(r, "change", e[12]), n = !0)
+                        H(r, e[2], !0), n || (i = F(r, "change", e[12]), n = !0)
                     },
                     p(e, n) {
-                        if (8 & n && (o = e[3].has("game_flavour")), o ? s ? s.p(e, n) : (s = ei(e), s.c(), s.m(t.parentNode, t)) : s && (s.d(1), s = null), 0 & n) {
+                        if (8 & n && (o = e[3].has("game_flavour")), o ? s ? s.p(e, n) : (s = ti(e), s.c(), s.m(t.parentNode, t)) : s && (s.d(1), s = null), 0 & n) {
                             let t;
-                            for (a = Object.values(jr), t = 0; t < a.length; t += 1) {
-                                const i = Kn(e, a, t);
-                                l[t] ? l[t].p(i, n) : (l[t] = ti(i), l[t].c(), l[t].m(r, null))
+                            for (a = Fe(Object.values(Br)), t = 0; t < a.length; t += 1) {
+                                const i = Xn(e, a, t);
+                                l[t] ? l[t].p(i, n) : (l[t] = ri(i), l[t].c(), l[t].m(r, null))
                             }
                             for (; t < l.length; t += 1) l[t].d(1);
                             l.length = a.length
                         }
-                        4 & n && z(r, e[2]), 8 & n && J(r, "error", e[3].has("game_flavour"))
+                        4 & n && H(r, e[2]), 8 & n && Y(r, "error", e[3].has("game_flavour"))
                     },
                     d(e) {
-                        s && s.d(e), e && O(t), e && O(r), S(l, e), n = !1, i()
+                        e && (S(t), S(r)), s && s.d(e), D(l, e), n = !1, i()
                     }
                 }
             }(t),
-            N = !t[4] && function(t) {
+            L = !t[4] && function(t) {
                 let r, n, i, o, s;
-                return n = new Yn({
+                return n = new Kn({
                     props: {
-                        icon: un
+                        icon: cn
                     }
                 }), {
                     c() {
-                        r = D("button"), Ve(n.$$.fragment), P(r, "class", "form-control"), P(r, "aria-label", "delete profile"), P(r, "title", "delete profile"), P(r, "type", "button")
+                        r = C("button"), He(n.$$.fragment), j(r, "class", "form-control"), j(r, "aria-label", "delete profile"), j(r, "title", "delete profile"), j(r, "type", "button")
                     },
                     m(e, a) {
-                        $(e, r, a), ze(n, r, null), i = !0, o || (s = I(r, "click", F(t[13])), o = !0)
+                        O(e, r, a), We(n, r, null), i = !0, o || (s = F(r, "click", M(t[13])), o = !0)
                     },
                     p: e,
                     i(e) {
-                        i || (Oe(n.$$.fragment, e), i = !0)
+                        i || (Se(n.$$.fragment, e), i = !0)
                     },
                     o(e) {
-                        Se(n.$$.fragment, e), i = !1
+                        De(n.$$.fragment, e), i = !1
                     },
                     d(e) {
-                        e && O(r), He(n), o = !1, s()
+                        e && S(r), Ge(n), o = !1, s()
                     }
                 }
             }(t);
         return {
             c() {
-                r = D("dialog"), n = D("form"), E && E.c(), i = L(), T && T.c(), s = L(), C && C.c(), a = L(), l = D("div"), u = D("input"), f = L(), h = D("button"), Ve(p.$$.fragment), d = L(), R && R.c(), m = L(), g = D("div"), v = D("button"), v.textContent = "save", y = L(), N && N.c(), P(u, "aria-label", "add-on folder"), P(u, "class", "form-control"), P(u, "type", "text"), u.disabled = !0, P(u, "placeholder", "add-on folder"), u.value = c = t[1] || "", J(u, "error", t[3].has("addon_dir")), P(h, "aria-label", "select folder"), P(h, "class", "form-control"), P(h, "type", "button"), P(l, "class", "row input-array"), P(v, "class", "form-control"), P(v, "type", "submit"), P(g, "class", "row input-array"), P(n, "class", "content"), r.open = !0, P(r, "class", "modal svelte-1lyvqkk")
+                r = C("dialog"), n = C("form"), q && q.c(), i = N(), T && T.c(), s = N(), $ && $.c(), a = N(), l = C("div"), u = C("input"), f = N(), h = C("button"), He(p.$$.fragment), d = N(), R && R.c(), m = N(), g = C("div"), v = C("button"), v.textContent = "save", y = N(), L && L.c(), j(u, "aria-label", "add-on folder"), j(u, "class", "form-control"), j(u, "type", "text"), u.disabled = !0, j(u, "placeholder", "add-on folder"), u.value = c = t[1] || "", Y(u, "error", t[3].has("addon_dir")), j(h, "aria-label", "select folder"), j(h, "class", "form-control"), j(h, "type", "button"), j(l, "class", "row input-array"), j(v, "class", "form-control"), j(v, "type", "submit"), j(g, "class", "row input-array"), j(n, "class", "content"), r.open = !0, j(r, "class", "modal svelte-1lyvqkk")
             },
             m(e, o) {
-                $(e, r, o), q(r, n), E && E.m(n, null), q(n, i), T && T.m(n, null), q(n, s), C && C.m(n, null), q(n, a), q(n, l), q(l, u), q(l, f), q(l, h), ze(p, h, null), q(n, d), R && R.m(n, null), q(n, m), q(n, g), q(g, v), q(g, y), N && N.m(g, null), w = !0, _ || (k = [I(window, "keydown", t[8]), I(h, "click", F(t[11])), I(n, "submit", F(t[14]))], _ = !0)
+                O(e, r, o), E(r, n), q && q.m(n, null), E(n, i), T && T.m(n, null), E(n, s), $ && $.m(n, null), E(n, a), E(n, l), E(l, u), E(l, f), E(l, h), We(p, h, null), E(n, d), R && R.m(n, null), E(n, m), E(n, g), E(g, v), E(g, y), L && L.m(g, null), w = !0, _ || (k = [F(window, "keydown", t[8]), F(h, "click", M(t[11])), F(n, "submit", M(t[14]))], _ = !0)
             },
             p(e, [t]) {
-                8 & t && (x = e[3].has("profile")), x ? E ? E.p(e, t) : (E = Xn(e), E.c(), E.m(n, i)) : E && (E.d(1), E = null), e[4] && T.p(e, t), 8 & t && (A = e[3].has("addon_dir")), A ? C ? C.p(e, t) : (C = Qn(e), C.c(), C.m(n, a)) : C && (C.d(1), C = null), (!w || 2 & t && c !== (c = e[1] || "") && u.value !== c) && (u.value = c), (!w || 8 & t) && J(u, "error", e[3].has("addon_dir")), e[4] || R.p(e, t), e[4] || N.p(e, t)
+                8 & t && (x = e[3].has("profile")), x ? q ? q.p(e, t) : (q = Qn(e), q.c(), q.m(n, i)) : q && (q.d(1), q = null), e[4] && T.p(e, t), 8 & t && (A = e[3].has("addon_dir")), A ? $ ? $.p(e, t) : ($ = ei(e), $.c(), $.m(n, a)) : $ && ($.d(1), $ = null), (!w || 2 & t && c !== (c = e[1] || "") && u.value !== c) && (u.value = c), (!w || 8 & t) && Y(u, "error", e[3].has("addon_dir")), e[4] || R.p(e, t), e[4] || L.p(e, t)
             },
             i(e) {
-                w || (Oe(p.$$.fragment, e), Oe(N), ge((() => {
-                    w && (b || (b = Re(r, Ye, {
+                w || (Se(p.$$.fragment, e), Se(L), e && ve((() => {
+                    w && (b || (b = Le(r, Xe, {
                         duration: 200
                     }, !0)), b.run(1))
                 })), w = !0)
             },
             o(e) {
-                Se(p.$$.fragment, e), Se(N), b || (b = Re(r, Ye, {
+                De(p.$$.fragment, e), De(L), e && (b || (b = Le(r, Xe, {
                     duration: 200
-                }, !1)), b.run(0), w = !1
+                }, !1)), b.run(0)), w = !1
             },
             d(e) {
-                e && O(r), E && E.d(), T && T.d(), C && C.d(), He(p), R && R.d(), N && N.d(), e && b && b.end(), _ = !1, o(k)
+                e && S(r), q && q.d(), T && T.d(), $ && $.d(), Ge(p), R && R.d(), L && L.d(), e && b && b.end(), _ = !1, o(k)
             }
         }
     }
 
-    function ni(e, t, r) {
+    function ii(e, t, r) {
         let n, i, o;
-        c(e, an, (e => r(15, n = e))), c(e, ln, (e => r(16, i = e))), c(e, nn, (e => r(17, o = e)));
+        c(e, ln, (e => r(15, n = e))), c(e, un, (e => r(16, i = e))), c(e, on, (e => r(17, o = e)));
         let {
             editing: s
         } = t;
         const a = "new" === s;
         let l, u, f, h = new Map;
-        a ? f = jr.Retail : ({
+        a ? f = Br.Retail : ({
             profile: l,
             addon_dir: u,
             game_flavour: f
         } = n[i]);
         const p = async () => {
             const {
                 selection: e
@@ -7517,525 +7537,525 @@
             null !== e && r(1, u = e)
         }, d = async () => {
             if (a && l in n || !l && "__default__" in n) return h.set("profile", l ? "a profile with that name already exists" : "a default profile already exists"), void r(3, h);
             let e;
             try {
                 e = await o.writeProfile(l, u, f, a)
             } catch (e) {
-                if (e instanceof st.JSONRPCError) return console.log(e), void r(3, h = new Map(e.data.map((({
+                if (e instanceof lt.JSONRPCError) return console.log(e), void r(3, h = new Map(e.data.map((({
                     path: [e],
                     message: t
                 }) => [String(e), t]))));
                 throw e
             }
-            v(an, n = {
+            v(ln, n = {
                 ...n,
                 [e.profile]: e
-            }, n), a && v(ln, i = e.profile, i), r(9, s = !1)
+            }, n), a && v(un, i = e.profile, i), r(9, s = !1)
         }, m = async () => {
             const {
                 ok: e
             } = await o.confirm("Delete profile", "Do you really want to delete this profile?\n\nDeleting a profile does not delete your add-ons; it simply dissociates the add-on folder from instawow.  However, you will have to reconcile your add-ons again if you create a new profile for this folder and your rollback history will be lost.");
-            e && (await o.deleteProfile(l), v(an, n = Wn.omit(n, l), n), v(ln, [i] = Object.keys(n), i), r(9, s = !1))
+            e && (await o.deleteProfile(l), v(ln, n = Gn.omit(n, l), n), v(un, [i] = Object.keys(n), i), r(9, s = !1))
         };
         return e.$$set = e => {
             "editing" in e && r(9, s = e.editing)
         }, [l, u, f, h, a, p, d, m, e => {
             "Escape" === e.key && s && (r(9, s = !1), e.preventDefault())
         }, s, function() {
             l = this.value, r(0, l)
         }, () => p(), function() {
-            f = W(this), r(2, f)
+            f = G(this), r(2, f)
         }, () => m(), () => d()]
     }
-    class ii extends Ze {
+    class oi extends Ye {
         constructor(e) {
-            super(), Ge(this, e, ni, ri, a, {
+            super(), Je(this, e, ii, ni, a, {
                 editing: 9
             })
         }
     }
 
-    function oi(e, t, r) {
+    function si(e, t, r) {
         const n = e.slice();
         return n[10] = t[r], n
     }
 
-    function si(e, t) {
+    function ai(e, t) {
         let r, n, i, o = t[10] + "";
         return {
             key: e,
             first: null,
             c() {
-                r = D("option"), n = R(o), r.__value = i = t[10], r.value = r.__value, P(r, "class", "svelte-ys6f4f"), this.first = r
+                r = C("option"), n = L(o), r.__value = i = t[10], z(r, r.__value), j(r, "class", "svelte-ys6f4f"), this.first = r
             },
             m(e, t) {
-                $(e, r, t), q(r, n)
+                O(e, r, t), E(r, n)
             },
             p(e, s) {
-                t = e, 4 & s && o !== (o = t[10] + "") && U(n, o), 4 & s && i !== (i = t[10]) && (r.__value = i, r.value = r.__value)
+                t = e, 4 & s && o !== (o = t[10] + "") && V(n, o), 4 & s && i !== (i = t[10]) && (r.__value = i, z(r, r.__value))
             },
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function ai(e) {
+    function li(e) {
         let t, r;
-        return t = new zn({
+        return t = new Hn({
             props: {
                 $$slots: {
-                    default: [ci]
+                    default: [fi]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("dismiss", e[9]), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(e, r) {
                 const n = {};
                 8192 & r && (n.$$scope = {
                     dirty: r,
                     ctx: e
                 }), t.$set(n)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function li(e) {
+    function ui(e) {
         let t, r, n;
 
         function i(t) {
             e[8](t)
         }
         let o = {};
-        return void 0 !== e[0] && (o.editing = e[0]), t = new ii({
+        return void 0 !== e[0] && (o.editing = e[0]), t = new oi({
             props: o
-        }), fe.push((() => Ue(t, "editing", i))), {
+        }), he.push((() => ze(t, "editing", i))), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, r) {
-                ze(t, e, r), n = !0
+                We(t, e, r), n = !0
             },
             p(e, n) {
                 const i = {};
-                !r && 1 & n && (r = !0, i.editing = e[0], ve((() => r = !1))), t.$set(i)
+                !r && 1 & n && (r = !0, i.editing = e[0], ye((() => r = !1))), t.$set(i)
             },
             i(e) {
-                n || (Oe(t.$$.fragment, e), n = !0)
+                n || (Se(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), n = !1
+                De(t.$$.fragment, e), n = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function ui(e) {
+    function ci(e) {
         let t, r, n;
 
         function i(t) {
             e[7](t)
         }
         let o = {};
-        return void 0 !== e[0] && (o.editing = e[0]), t = new ii({
+        return void 0 !== e[0] && (o.editing = e[0]), t = new oi({
             props: o
-        }), fe.push((() => Ue(t, "editing", i))), {
+        }), he.push((() => ze(t, "editing", i))), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, r) {
-                ze(t, e, r), n = !0
+                We(t, e, r), n = !0
             },
             p(e, n) {
                 const i = {};
-                !r && 1 & n && (r = !0, i.editing = e[0], ve((() => r = !1))), t.$set(i)
+                !r && 1 & n && (r = !0, i.editing = e[0], ye((() => r = !1))), t.$set(i)
             },
             i(e) {
-                n || (Oe(t.$$.fragment, e), n = !0)
+                n || (Se(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), n = !1
+                De(t.$$.fragment, e), n = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function ci(e) {
+    function fi(e) {
         let t, r;
-        return t = new Bn({}), {
+        return t = new Un({}), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function fi(e) {
+    function hi(e) {
         let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _ = [],
             k = new Map;
-        i = new Yn({
+        i = new Kn({
             props: {
-                icon: yn
+                icon: bn
             }
         });
-        let x = Object.keys(e[2]);
+        let x = Fe(Object.keys(e[2]));
         const A = e => e[10];
         for (let t = 0; t < x.length; t += 1) {
-            let r = oi(e, x, t),
+            let r = si(e, x, t),
                 n = A(r);
-            k.set(n, _[t] = si(n, r))
+            k.set(n, _[t] = ai(n, r))
         }
-        const E = [ui, li, ai],
+        const q = [ci, ui, li],
             T = [];
 
-        function S(e, t) {
+        function $(e, t) {
             return "new" === e[0] ? 0 : "existing" === e[0] ? 1 : "auth" === e[0] ? 2 : -1
         }
-        return ~(g = S(e)) && (v = T[g] = E[g](e)), {
+        return ~(g = $(e)) && (v = T[g] = q[g](e)), {
             c() {
-                t = D("div"), r = D("div"), n = D("button"), Ve(i.$$.fragment), s = L(), a = D("select");
+                t = C("div"), r = C("div"), n = C("button"), He(i.$$.fragment), s = N(), a = C("select");
                 for (let e = 0; e < _.length; e += 1) _[e].c();
-                u = L(), c = D("button"), f = R("edit"), p = L(), d = D("button"), d.textContent = "add", m = L(), v && v.c(), P(n, "aria-label", "configure access tokens"), P(n, "class", "svelte-ys6f4f"), P(a, "aria-label", "profile"), a.disabled = l = !!e[0], P(a, "class", "svelte-ys6f4f"), void 0 === e[1] && ge((() => e[4].call(a))), P(c, "aria-label", "edit profile"), c.disabled = h = !e[1], P(c, "class", "svelte-ys6f4f"), P(d, "aria-label", "add profile"), P(d, "class", "svelte-ys6f4f"), P(r, "class", "profile-switcher svelte-ys6f4f"), P(t, "class", "profile-switcher-wrapper svelte-ys6f4f")
+                u = N(), c = C("button"), f = L("edit"), p = N(), d = C("button"), d.textContent = "add", m = N(), v && v.c(), j(n, "aria-label", "configure access tokens"), j(n, "class", "svelte-ys6f4f"), j(a, "aria-label", "profile"), a.disabled = l = !!e[0], j(a, "class", "svelte-ys6f4f"), void 0 === e[1] && ve((() => e[4].call(a))), j(c, "aria-label", "edit profile"), c.disabled = h = !e[1], j(c, "class", "svelte-ys6f4f"), j(d, "aria-label", "add profile"), j(d, "class", "svelte-ys6f4f"), j(r, "class", "profile-switcher svelte-ys6f4f"), j(t, "class", "profile-switcher-wrapper svelte-ys6f4f")
             },
             m(o, l) {
-                $(o, t, l), q(t, r), q(r, n), ze(i, n, null), q(r, s), q(r, a);
+                O(o, t, l), E(t, r), E(r, n), We(i, n, null), E(r, s), E(r, a);
                 for (let e = 0; e < _.length; e += 1) _[e] && _[e].m(a, null);
-                z(a, e[1], !0), q(r, u), q(r, c), q(c, f), q(r, p), q(r, d), q(t, m), ~g && T[g].m(t, null), y = !0, b || (w = [I(n, "click", e[3]), I(a, "change", e[4]), I(c, "click", e[5]), I(d, "click", e[6])], b = !0)
+                H(a, e[1], !0), E(r, u), E(r, c), E(c, f), E(r, p), E(r, d), E(t, m), ~g && T[g].m(t, null), y = !0, b || (w = [F(n, "click", e[3]), F(a, "change", e[4]), F(c, "click", e[5]), F(d, "click", e[6])], b = !0)
             },
             p(e, [r]) {
-                4 & r && (x = Object.keys(e[2]), _ = Pe(_, r, A, 1, e, x, k, a, Ie, si, null, oi)), (!y || 1 & r && l !== (l = !!e[0])) && (a.disabled = l), 6 & r && z(a, e[1]), (!y || 6 & r && h !== (h = !e[1])) && (c.disabled = h);
+                4 & r && (x = Fe(Object.keys(e[2])), _ = Be(_, r, A, 1, e, x, k, a, Me, ai, null, si)), (!y || 1 & r && l !== (l = !!e[0])) && (a.disabled = l), 6 & r && H(a, e[1]), (!y || 6 & r && h !== (h = !e[1])) && (c.disabled = h);
                 let n = g;
-                g = S(e), g === n ? ~g && T[g].p(e, r) : (v && (Te(), Se(T[n], 1, 1, (() => {
+                g = $(e), g === n ? ~g && T[g].p(e, r) : (v && ($e(), De(T[n], 1, 1, (() => {
                     T[n] = null
-                })), $e()), ~g ? (v = T[g], v ? v.p(e, r) : (v = T[g] = E[g](e), v.c()), Oe(v, 1), v.m(t, null)) : v = null)
+                })), Oe()), ~g ? (v = T[g], v ? v.p(e, r) : (v = T[g] = q[g](e), v.c()), Se(v, 1), v.m(t, null)) : v = null)
             },
             i(e) {
-                y || (Oe(i.$$.fragment, e), Oe(v), y = !0)
+                y || (Se(i.$$.fragment, e), Se(v), y = !0)
             },
             o(e) {
-                Se(i.$$.fragment, e), Se(v), y = !1
+                De(i.$$.fragment, e), De(v), y = !1
             },
             d(e) {
-                e && O(t), He(i);
+                e && S(t), Ge(i);
                 for (let e = 0; e < _.length; e += 1) _[e].d();
                 ~g && T[g].d(), b = !1, o(w)
             }
         }
     }
 
-    function hi(e, t, r) {
+    function pi(e, t, r) {
         let n, i;
-        c(e, ln, (e => r(1, n = e))), c(e, an, (e => r(2, i = e)));
+        c(e, un, (e => r(1, n = e))), c(e, ln, (e => r(2, i = e)));
         let o = !1;
-        oe((() => {
+        se((() => {
             n || r(0, o = "new")
         }));
         return [o, n, i, () => r(0, o = "auth" !== o && "auth"), function() {
-            n = W(this), ln.set(n)
+            n = G(this), un.set(n)
         }, () => r(0, o = "existing" !== o && "existing"), () => r(0, o = "new" !== o && "new"), function(e) {
             o = e, r(0, o)
         }, function(e) {
             o = e, r(0, o)
         }, () => r(0, o = !1)]
     }
-    class pi extends Ze {
+    class di extends Ye {
         constructor(e) {
-            super(), Ge(this, e, hi, fi, a, {})
+            super(), Je(this, e, pi, hi, a, {})
         }
     }
-    class di extends Error {}
-    class mi extends di {
+    class mi extends Error {}
+    class gi extends mi {
         constructor(e) {
             super(`Invalid DateTime: ${e.toMessage()}`)
         }
     }
-    class gi extends di {
+    class vi extends mi {
         constructor(e) {
             super(`Invalid Interval: ${e.toMessage()}`)
         }
     }
-    class vi extends di {
+    class yi extends mi {
         constructor(e) {
             super(`Invalid Duration: ${e.toMessage()}`)
         }
     }
-    class yi extends di {}
-    class bi extends di {
+    class bi extends mi {}
+    class wi extends mi {
         constructor(e) {
             super(`Invalid unit ${e}`)
         }
     }
-    class wi extends di {}
-    class _i extends di {
+    class _i extends mi {}
+    class ki extends mi {
         constructor() {
             super("Zone is an abstract class")
         }
     }
-    const ki = "numeric",
-        xi = "short",
-        Ai = "long",
-        qi = {
-            year: ki,
-            month: ki,
-            day: ki
-        },
+    const xi = "numeric",
+        Ai = "short",
+        qi = "long",
         Ei = {
-            year: ki,
+            year: xi,
             month: xi,
-            day: ki
+            day: xi
         },
         Ti = {
-            year: ki,
-            month: xi,
-            day: ki,
-            weekday: xi
+            year: xi,
+            month: Ai,
+            day: xi
         },
         $i = {
-            year: ki,
+            year: xi,
             month: Ai,
-            day: ki
+            day: xi,
+            weekday: Ai
         },
         Oi = {
-            year: ki,
-            month: Ai,
-            day: ki,
-            weekday: Ai
+            year: xi,
+            month: qi,
+            day: xi
         },
         Si = {
-            hour: ki,
-            minute: ki
+            year: xi,
+            month: qi,
+            day: xi,
+            weekday: qi
         },
         Di = {
-            hour: ki,
-            minute: ki,
-            second: ki
+            hour: xi,
+            minute: xi
         },
         Ci = {
-            hour: ki,
-            minute: ki,
-            second: ki,
-            timeZoneName: xi
+            hour: xi,
+            minute: xi,
+            second: xi
         },
         Ri = {
-            hour: ki,
-            minute: ki,
-            second: ki,
+            hour: xi,
+            minute: xi,
+            second: xi,
             timeZoneName: Ai
         },
         Li = {
-            hour: ki,
-            minute: ki,
-            hourCycle: "h23"
+            hour: xi,
+            minute: xi,
+            second: xi,
+            timeZoneName: qi
         },
         Ni = {
-            hour: ki,
-            minute: ki,
-            second: ki,
+            hour: xi,
+            minute: xi,
             hourCycle: "h23"
         },
         Ii = {
-            hour: ki,
-            minute: ki,
-            second: ki,
-            hourCycle: "h23",
-            timeZoneName: xi
+            hour: xi,
+            minute: xi,
+            second: xi,
+            hourCycle: "h23"
         },
         Fi = {
-            hour: ki,
-            minute: ki,
-            second: ki,
+            hour: xi,
+            minute: xi,
+            second: xi,
             hourCycle: "h23",
             timeZoneName: Ai
         },
         Mi = {
-            year: ki,
-            month: ki,
-            day: ki,
-            hour: ki,
-            minute: ki
+            hour: xi,
+            minute: xi,
+            second: xi,
+            hourCycle: "h23",
+            timeZoneName: qi
         },
         Pi = {
-            year: ki,
-            month: ki,
-            day: ki,
-            hour: ki,
-            minute: ki,
-            second: ki
+            year: xi,
+            month: xi,
+            day: xi,
+            hour: xi,
+            minute: xi
         },
         ji = {
-            year: ki,
+            year: xi,
             month: xi,
-            day: ki,
-            hour: ki,
-            minute: ki
+            day: xi,
+            hour: xi,
+            minute: xi,
+            second: xi
         },
         Bi = {
-            year: ki,
-            month: xi,
-            day: ki,
-            hour: ki,
-            minute: ki,
-            second: ki
+            year: xi,
+            month: Ai,
+            day: xi,
+            hour: xi,
+            minute: xi
         },
         Ui = {
-            year: ki,
-            month: xi,
-            day: ki,
-            weekday: xi,
-            hour: ki,
-            minute: ki
+            year: xi,
+            month: Ai,
+            day: xi,
+            hour: xi,
+            minute: xi,
+            second: xi
         },
         Vi = {
-            year: ki,
+            year: xi,
             month: Ai,
-            day: ki,
-            hour: ki,
-            minute: ki,
-            timeZoneName: xi
+            day: xi,
+            weekday: Ai,
+            hour: xi,
+            minute: xi
         },
         zi = {
-            year: ki,
-            month: Ai,
-            day: ki,
-            hour: ki,
-            minute: ki,
-            second: ki,
-            timeZoneName: xi
+            year: xi,
+            month: qi,
+            day: xi,
+            hour: xi,
+            minute: xi,
+            timeZoneName: Ai
         },
         Hi = {
-            year: ki,
-            month: Ai,
-            day: ki,
-            weekday: Ai,
-            hour: ki,
-            minute: ki,
+            year: xi,
+            month: qi,
+            day: xi,
+            hour: xi,
+            minute: xi,
+            second: xi,
             timeZoneName: Ai
         },
         Wi = {
-            year: ki,
-            month: Ai,
-            day: ki,
-            weekday: Ai,
-            hour: ki,
-            minute: ki,
-            second: ki,
-            timeZoneName: Ai
+            year: xi,
+            month: qi,
+            day: xi,
+            weekday: qi,
+            hour: xi,
+            minute: xi,
+            timeZoneName: qi
+        },
+        Gi = {
+            year: xi,
+            month: qi,
+            day: xi,
+            weekday: qi,
+            hour: xi,
+            minute: xi,
+            second: xi,
+            timeZoneName: qi
         };
-    class Gi {
+    class Zi {
         get type() {
-            throw new _i
+            throw new ki
         }
         get name() {
-            throw new _i
+            throw new ki
         }
         get ianaName() {
             return this.name
         }
         get isUniversal() {
-            throw new _i
+            throw new ki
         }
         offsetName(e, t) {
-            throw new _i
+            throw new ki
         }
         formatOffset(e, t) {
-            throw new _i
+            throw new ki
         }
         offset(e) {
-            throw new _i
+            throw new ki
         }
         equals(e) {
-            throw new _i
+            throw new ki
         }
         get isValid() {
-            throw new _i
+            throw new ki
         }
     }
-    let Zi = null;
-    class Ji extends Gi {
+    let Ji = null;
+    class Yi extends Zi {
         static get instance() {
-            return null === Zi && (Zi = new Ji), Zi
+            return null === Ji && (Ji = new Yi), Ji
         }
         get type() {
             return "system"
         }
         get name() {
             return (new Intl.DateTimeFormat).resolvedOptions().timeZone
         }
         get isUniversal() {
             return !1
         }
         offsetName(e, {
             format: t,
             locale: r
         }) {
-            return Uo(e, t, r)
+            return Vo(e, t, r)
         }
         formatOffset(e, t) {
-            return Wo(this.offset(e), t)
+            return Go(this.offset(e), t)
         }
         offset(e) {
             return -new Date(e).getTimezoneOffset()
         }
         equals(e) {
             return "system" === e.type
         }
         get isValid() {
             return !0
         }
     }
-    let Yi = {};
-    const Ki = {
+    let Ki = {};
+    const Xi = {
         year: 0,
         month: 1,
         day: 2,
         era: 3,
         hour: 4,
         minute: 5,
         second: 6
     };
-    let Xi = {};
-    class Qi extends Gi {
+    let Qi = {};
+    class eo extends Zi {
         static create(e) {
-            return Xi[e] || (Xi[e] = new Qi(e)), Xi[e]
+            return Qi[e] || (Qi[e] = new eo(e)), Qi[e]
         }
         static resetCache() {
-            Xi = {}, Yi = {}
+            Qi = {}, Ki = {}
         }
         static isValidSpecifier(e) {
             return this.isValidZone(e)
         }
         static isValidZone(e) {
             if (!e) return !1;
             try {
@@ -8043,70 +8063,70 @@
                     timeZone: e
                 }).format(), !0
             } catch (e) {
                 return !1
             }
         }
         constructor(e) {
-            super(), this.zoneName = e, this.valid = Qi.isValidZone(e)
+            super(), this.zoneName = e, this.valid = eo.isValidZone(e)
         }
         get type() {
             return "iana"
         }
         get name() {
             return this.zoneName
         }
         get isUniversal() {
             return !1
         }
         offsetName(e, {
             format: t,
             locale: r
         }) {
-            return Uo(e, t, r, this.name)
+            return Vo(e, t, r, this.name)
         }
         formatOffset(e, t) {
-            return Wo(this.offset(e), t)
+            return Go(this.offset(e), t)
         }
         offset(e) {
             const t = new Date(e);
             if (isNaN(t)) return NaN;
-            const r = (n = this.name, Yi[n] || (Yi[n] = new Intl.DateTimeFormat("en-US", {
+            const r = (n = this.name, Ki[n] || (Ki[n] = new Intl.DateTimeFormat("en-US", {
                 hour12: !1,
                 timeZone: n,
                 year: "numeric",
                 month: "2-digit",
                 day: "2-digit",
                 hour: "2-digit",
                 minute: "2-digit",
                 second: "2-digit",
                 era: "short"
-            })), Yi[n]);
+            })), Ki[n]);
             var n;
             let [i, o, s, a, l, u, c] = r.formatToParts ? function(e, t) {
                 const r = e.formatToParts(t),
                     n = [];
                 for (let e = 0; e < r.length; e++) {
                     const {
                         type: t,
                         value: i
-                    } = r[e], o = Ki[t];
-                    "era" === t ? n[o] = i : Ao(o) || (n[o] = parseInt(i, 10))
+                    } = r[e], o = Xi[t];
+                    "era" === t ? n[o] = i : qo(o) || (n[o] = parseInt(i, 10))
                 }
                 return n
             }(r, t) : function(e, t) {
                 const r = e.format(t).replace(/\u200E/g, ""),
                     n = /(\d+)\/(\d+)\/(\d+) (AD|BC),? (\d+):(\d+):(\d+)/.exec(r),
                     [, i, o, s, a, l, u, c] = n;
                 return [s, i, o, a, l, u, c]
             }(r, t);
             "BC" === a && (i = 1 - Math.abs(i));
             let f = +t;
             const h = f % 1e3;
-            return f -= h >= 0 ? h : 1e3 + h, (Po({
+            return f -= h >= 0 ? h : 1e3 + h, (jo({
                 year: i,
                 month: o,
                 day: s,
                 hour: 24 === l ? 0 : l,
                 minute: u,
                 second: c,
                 millisecond: 0
@@ -8115,75 +8135,75 @@
         equals(e) {
             return "iana" === e.type && e.name === this.name
         }
         get isValid() {
             return this.valid
         }
     }
-    let eo = {};
     let to = {};
+    let ro = {};
 
-    function ro(e, t = {}) {
+    function no(e, t = {}) {
         const r = JSON.stringify([e, t]);
-        let n = to[r];
-        return n || (n = new Intl.DateTimeFormat(e, t), to[r] = n), n
+        let n = ro[r];
+        return n || (n = new Intl.DateTimeFormat(e, t), ro[r] = n), n
     }
-    let no = {};
     let io = {};
-    let oo = null;
+    let oo = {};
+    let so = null;
 
-    function so(e, t, r, n, i) {
+    function ao(e, t, r, n, i) {
         const o = e.listingMode(r);
         return "error" === o ? null : "en" === o ? n(t) : i(t)
     }
-    class ao {
+    class lo {
         constructor(e, t, r) {
             this.padTo = r.padTo || 0, this.floor = r.floor || !1;
             const {
                 padTo: n,
                 floor: i,
                 ...o
             } = r;
             if (!t || Object.keys(o).length > 0) {
                 const t = {
                     useGrouping: !1,
                     ...r
                 };
                 r.padTo > 0 && (t.minimumIntegerDigits = r.padTo), this.inf = function(e, t = {}) {
                     const r = JSON.stringify([e, t]);
-                    let n = no[r];
-                    return n || (n = new Intl.NumberFormat(e, t), no[r] = n), n
+                    let n = io[r];
+                    return n || (n = new Intl.NumberFormat(e, t), io[r] = n), n
                 }(e, t)
             }
         }
         format(e) {
             if (this.inf) {
                 const t = this.floor ? Math.floor(e) : e;
                 return this.inf.format(t)
             }
-            return Do(this.floor ? Math.floor(e) : No(e, 3), this.padTo)
+            return Co(this.floor ? Math.floor(e) : Io(e, 3), this.padTo)
         }
     }
-    class lo {
+    class uo {
         constructor(e, t, r) {
             let n;
             if (this.opts = r, this.originalZone = void 0, this.opts.timeZone) this.dt = e;
             else if ("fixed" === e.zone.type) {
                 const t = e.offset / 60 * -1,
                     r = t >= 0 ? `Etc/GMT+${t}` : `Etc/GMT${t}`;
-                0 !== e.offset && Qi.create(r).valid ? (n = r, this.dt = e) : (n = "UTC", this.dt = 0 === e.offset ? e : e.setZone("UTC").plus({
+                0 !== e.offset && eo.create(r).valid ? (n = r, this.dt = e) : (n = "UTC", this.dt = 0 === e.offset ? e : e.setZone("UTC").plus({
                     minutes: e.offset
                 }), this.originalZone = e.zone)
             } else "system" === e.zone.type ? this.dt = e : "iana" === e.zone.type ? (this.dt = e, n = e.zone.name) : (n = "UTC", this.dt = e.setZone("UTC").plus({
                 minutes: e.offset
             }), this.originalZone = e.zone);
             const i = {
                 ...this.opts
             };
-            i.timeZone = i.timeZone || n, this.dtf = ro(t, i)
+            i.timeZone = i.timeZone || n, this.dtf = no(t, i)
         }
         format() {
             return this.originalZone ? this.formatToParts().map((({
                 value: e
             }) => e)).join("") : this.dtf.format(this.dt.toJSDate())
         }
         formatToParts() {
@@ -8202,26 +8222,26 @@
                 return e
             })) : e
         }
         resolvedOptions() {
             return this.dtf.resolvedOptions()
         }
     }
-    class uo {
+    class co {
         constructor(e, t, r) {
             this.opts = {
                 style: "long",
                 ...r
-            }, !t && To() && (this.rtf = function(e, t = {}) {
+            }, !t && $o() && (this.rtf = function(e, t = {}) {
                 const {
                     base: r,
                     ...n
                 } = t, i = JSON.stringify([e, n]);
-                let o = io[i];
-                return o || (o = new Intl.RelativeTimeFormat(e, t), io[i] = o), o
+                let o = oo[i];
+                return o || (o = new Intl.RelativeTimeFormat(e, t), oo[i] = o), o
             }(e, r))
         }
         format(e, t) {
             return this.rtf ? this.rtf.format(e, t) : function(e, t, r = "always", n = !1) {
                 const i = {
                         years: ["year", "yr."],
                         quarters: ["quarter", "qtr."],
@@ -8252,46 +8272,46 @@
                 return s ? `${a} ${c} ago` : `in ${a} ${c}`
             }(t, e, this.opts.numeric, "long" !== this.opts.style)
         }
         formatToParts(e, t) {
             return this.rtf ? this.rtf.formatToParts(e, t) : []
         }
     }
-    class co {
+    class fo {
         static fromOpts(e) {
-            return co.create(e.locale, e.numberingSystem, e.outputCalendar, e.defaultToEN)
+            return fo.create(e.locale, e.numberingSystem, e.outputCalendar, e.defaultToEN)
         }
         static create(e, t, r, n = !1) {
-            const i = e || xo.defaultLocale,
-                o = i || (n ? "en-US" : oo || (oo = (new Intl.DateTimeFormat).resolvedOptions().locale, oo)),
-                s = t || xo.defaultNumberingSystem,
-                a = r || xo.defaultOutputCalendar;
-            return new co(o, s, a, i)
+            const i = e || Ao.defaultLocale,
+                o = i || (n ? "en-US" : so || (so = (new Intl.DateTimeFormat).resolvedOptions().locale, so)),
+                s = t || Ao.defaultNumberingSystem,
+                a = r || Ao.defaultOutputCalendar;
+            return new fo(o, s, a, i)
         }
         static resetCache() {
-            oo = null, to = {}, no = {}, io = {}
+            so = null, ro = {}, io = {}, oo = {}
         }
         static fromObject({
             locale: e,
             numberingSystem: t,
             outputCalendar: r
         } = {}) {
-            return co.create(e, t, r)
+            return fo.create(e, t, r)
         }
         constructor(e, t, r, n) {
             const [i, o, s] = function(e) {
                 const t = e.indexOf("-x-"); - 1 !== t && (e = e.substring(0, t));
                 const r = e.indexOf("-u-");
                 if (-1 === r) return [e]; {
                     let t, n;
                     try {
-                        t = ro(e).resolvedOptions(), n = e
+                        t = no(e).resolvedOptions(), n = e
                     } catch (i) {
                         const o = e.substring(0, r);
-                        t = ro(o).resolvedOptions(), n = o
+                        t = no(o).resolvedOptions(), n = o
                     }
                     const {
                         numberingSystem: i,
                         calendar: o
                     } = t;
                     return [n, i, o]
                 }
@@ -8312,162 +8332,162 @@
         }
         listingMode() {
             const e = this.isEnglish(),
                 t = !(null !== this.numberingSystem && "latn" !== this.numberingSystem || null !== this.outputCalendar && "gregory" !== this.outputCalendar);
             return e && t ? "en" : "intl"
         }
         clone(e) {
-            return e && 0 !== Object.getOwnPropertyNames(e).length ? co.create(e.locale || this.specifiedLocale, e.numberingSystem || this.numberingSystem, e.outputCalendar || this.outputCalendar, e.defaultToEN || !1) : this
+            return e && 0 !== Object.getOwnPropertyNames(e).length ? fo.create(e.locale || this.specifiedLocale, e.numberingSystem || this.numberingSystem, e.outputCalendar || this.outputCalendar, e.defaultToEN || !1) : this
         }
         redefaultToEN(e = {}) {
             return this.clone({
                 ...e,
                 defaultToEN: !0
             })
         }
         redefaultToSystem(e = {}) {
             return this.clone({
                 ...e,
                 defaultToEN: !1
             })
         }
         months(e, t = !1, r = !0) {
-            return so(this, e, r, Ko, (() => {
+            return ao(this, e, r, Xo, (() => {
                 const r = t ? {
                         month: e,
                         day: "numeric"
                     } : {
                         month: e
                     },
                     n = t ? "format" : "standalone";
                 return this.monthsCache[n][e] || (this.monthsCache[n][e] = function(e) {
                     const t = [];
                     for (let r = 1; r <= 12; r++) {
-                        const n = pl.utc(2016, r, 1);
+                        const n = dl.utc(2016, r, 1);
                         t.push(e(n))
                     }
                     return t
                 }((e => this.extract(e, r, "month")))), this.monthsCache[n][e]
             }))
         }
         weekdays(e, t = !1, r = !0) {
-            return so(this, e, r, ts, (() => {
+            return ao(this, e, r, rs, (() => {
                 const r = t ? {
                         weekday: e,
                         year: "numeric",
                         month: "long",
                         day: "numeric"
                     } : {
                         weekday: e
                     },
                     n = t ? "format" : "standalone";
                 return this.weekdaysCache[n][e] || (this.weekdaysCache[n][e] = function(e) {
                     const t = [];
                     for (let r = 1; r <= 7; r++) {
-                        const n = pl.utc(2016, 11, 13 + r);
+                        const n = dl.utc(2016, 11, 13 + r);
                         t.push(e(n))
                     }
                     return t
                 }((e => this.extract(e, r, "weekday")))), this.weekdaysCache[n][e]
             }))
         }
         meridiems(e = !0) {
-            return so(this, void 0, e, (() => rs), (() => {
+            return ao(this, void 0, e, (() => ns), (() => {
                 if (!this.meridiemCache) {
                     const e = {
                         hour: "numeric",
                         hourCycle: "h12"
                     };
-                    this.meridiemCache = [pl.utc(2016, 11, 13, 9), pl.utc(2016, 11, 13, 19)].map((t => this.extract(t, e, "dayperiod")))
+                    this.meridiemCache = [dl.utc(2016, 11, 13, 9), dl.utc(2016, 11, 13, 19)].map((t => this.extract(t, e, "dayperiod")))
                 }
                 return this.meridiemCache
             }))
         }
         eras(e, t = !0) {
-            return so(this, e, t, ss, (() => {
+            return ao(this, e, t, as, (() => {
                 const t = {
                     era: e
                 };
-                return this.eraCache[e] || (this.eraCache[e] = [pl.utc(-40, 1, 1), pl.utc(2017, 1, 1)].map((e => this.extract(e, t, "era")))), this.eraCache[e]
+                return this.eraCache[e] || (this.eraCache[e] = [dl.utc(-40, 1, 1), dl.utc(2017, 1, 1)].map((e => this.extract(e, t, "era")))), this.eraCache[e]
             }))
         }
         extract(e, t, r) {
             const n = this.dtFormatter(e, t).formatToParts().find((e => e.type.toLowerCase() === r));
             return n ? n.value : null
         }
         numberFormatter(e = {}) {
-            return new ao(this.intl, e.forceSimple || this.fastNumbers, e)
+            return new lo(this.intl, e.forceSimple || this.fastNumbers, e)
         }
         dtFormatter(e, t = {}) {
-            return new lo(e, this.intl, t)
+            return new uo(e, this.intl, t)
         }
         relFormatter(e = {}) {
-            return new uo(this.intl, this.isEnglish(), e)
+            return new co(this.intl, this.isEnglish(), e)
         }
         listFormatter(e = {}) {
             return function(e, t = {}) {
                 const r = JSON.stringify([e, t]);
-                let n = eo[r];
-                return n || (n = new Intl.ListFormat(e, t), eo[r] = n), n
+                let n = to[r];
+                return n || (n = new Intl.ListFormat(e, t), to[r] = n), n
             }(this.intl, e)
         }
         isEnglish() {
             return "en" === this.locale || "en-us" === this.locale.toLowerCase() || new Intl.DateTimeFormat(this.intl).resolvedOptions().locale.startsWith("en-us")
         }
         equals(e) {
             return this.locale === e.locale && this.numberingSystem === e.numberingSystem && this.outputCalendar === e.outputCalendar
         }
     }
-    let fo = null;
-    class ho extends Gi {
+    let ho = null;
+    class po extends Zi {
         static get utcInstance() {
-            return null === fo && (fo = new ho(0)), fo
+            return null === ho && (ho = new po(0)), ho
         }
         static instance(e) {
-            return 0 === e ? ho.utcInstance : new ho(e)
+            return 0 === e ? po.utcInstance : new po(e)
         }
         static parseSpecifier(e) {
             if (e) {
                 const t = e.match(/^utc(?:([+-]\d{1,2})(?::(\d{2}))?)?$/i);
-                if (t) return new ho(Vo(t[1], t[2]))
+                if (t) return new po(zo(t[1], t[2]))
             }
             return null
         }
         constructor(e) {
             super(), this.fixed = e
         }
         get type() {
             return "fixed"
         }
         get name() {
-            return 0 === this.fixed ? "UTC" : `UTC${Wo(this.fixed,"narrow")}`
+            return 0 === this.fixed ? "UTC" : `UTC${Go(this.fixed,"narrow")}`
         }
         get ianaName() {
-            return 0 === this.fixed ? "Etc/UTC" : `Etc/GMT${Wo(-this.fixed,"narrow")}`
+            return 0 === this.fixed ? "Etc/UTC" : `Etc/GMT${Go(-this.fixed,"narrow")}`
         }
         offsetName() {
             return this.name
         }
         formatOffset(e, t) {
-            return Wo(this.fixed, t)
+            return Go(this.fixed, t)
         }
         get isUniversal() {
             return !0
         }
         offset() {
             return this.fixed
         }
         equals(e) {
             return "fixed" === e.type && e.fixed === this.fixed
         }
         get isValid() {
             return !0
         }
     }
-    class po extends Gi {
+    class mo extends Zi {
         constructor(e) {
             super(), this.zoneName = e
         }
         get type() {
             return "invalid"
         }
         get name() {
@@ -8489,169 +8509,169 @@
             return !1
         }
         get isValid() {
             return !1
         }
     }
 
-    function mo(e, t) {
-        if (Ao(e) || null === e) return t;
-        if (e instanceof Gi) return e;
+    function go(e, t) {
+        if (qo(e) || null === e) return t;
+        if (e instanceof Zi) return e;
         if ("string" == typeof e) {
             const r = e.toLowerCase();
-            return "default" === r ? t : "local" === r || "system" === r ? Ji.instance : "utc" === r || "gmt" === r ? ho.utcInstance : ho.parseSpecifier(r) || Qi.create(e)
+            return "default" === r ? t : "local" === r || "system" === r ? Yi.instance : "utc" === r || "gmt" === r ? po.utcInstance : po.parseSpecifier(r) || eo.create(e)
         }
-        return qo(e) ? ho.instance(e) : "object" == typeof e && e.offset && "number" == typeof e.offset ? e : new po(e)
+        return Eo(e) ? po.instance(e) : "object" == typeof e && e.offset && "number" == typeof e.offset ? e : new mo(e)
     }
-    let go, vo = () => Date.now(),
-        yo = "system",
-        bo = null,
+    let vo, yo = () => Date.now(),
+        bo = "system",
         wo = null,
         _o = null,
-        ko = 60;
-    class xo {
+        ko = null,
+        xo = 60;
+    class Ao {
         static get now() {
-            return vo
+            return yo
         }
         static set now(e) {
-            vo = e
+            yo = e
         }
         static set defaultZone(e) {
-            yo = e
+            bo = e
         }
         static get defaultZone() {
-            return mo(yo, Ji.instance)
+            return go(bo, Yi.instance)
         }
         static get defaultLocale() {
-            return bo
+            return wo
         }
         static set defaultLocale(e) {
-            bo = e
+            wo = e
         }
         static get defaultNumberingSystem() {
-            return wo
+            return _o
         }
         static set defaultNumberingSystem(e) {
-            wo = e
+            _o = e
         }
         static get defaultOutputCalendar() {
-            return _o
+            return ko
         }
         static set defaultOutputCalendar(e) {
-            _o = e
+            ko = e
         }
         static get twoDigitCutoffYear() {
-            return ko
+            return xo
         }
         static set twoDigitCutoffYear(e) {
-            ko = e % 100
+            xo = e % 100
         }
         static get throwOnInvalid() {
-            return go
+            return vo
         }
         static set throwOnInvalid(e) {
-            go = e
+            vo = e
         }
         static resetCaches() {
-            co.resetCache(), Qi.resetCache()
+            fo.resetCache(), eo.resetCache()
         }
     }
 
-    function Ao(e) {
+    function qo(e) {
         return void 0 === e
     }
 
-    function qo(e) {
+    function Eo(e) {
         return "number" == typeof e
     }
 
-    function Eo(e) {
+    function To(e) {
         return "number" == typeof e && e % 1 == 0
     }
 
-    function To() {
+    function $o() {
         try {
             return "undefined" != typeof Intl && !!Intl.RelativeTimeFormat
         } catch (e) {
             return !1
         }
     }
 
-    function $o(e, t, r) {
+    function Oo(e, t, r) {
         if (0 !== e.length) return e.reduce(((e, n) => {
             const i = [t(n), n];
             return e && r(e[0], i[0]) === e[0] ? e : i
         }), null)[1]
     }
 
-    function Oo(e, t) {
+    function So(e, t) {
         return Object.prototype.hasOwnProperty.call(e, t)
     }
 
-    function So(e, t, r) {
-        return Eo(e) && e >= t && e <= r
+    function Do(e, t, r) {
+        return To(e) && e >= t && e <= r
     }
 
-    function Do(e, t = 2) {
+    function Co(e, t = 2) {
         let r;
         return r = e < 0 ? "-" + ("" + -e).padStart(t, "0") : ("" + e).padStart(t, "0"), r
     }
 
-    function Co(e) {
-        return Ao(e) || null === e || "" === e ? void 0 : parseInt(e, 10)
-    }
-
     function Ro(e) {
-        return Ao(e) || null === e || "" === e ? void 0 : parseFloat(e)
+        return qo(e) || null === e || "" === e ? void 0 : parseInt(e, 10)
     }
 
     function Lo(e) {
-        if (!Ao(e) && null !== e && "" !== e) {
+        return qo(e) || null === e || "" === e ? void 0 : parseFloat(e)
+    }
+
+    function No(e) {
+        if (!qo(e) && null !== e && "" !== e) {
             const t = 1e3 * parseFloat("0." + e);
             return Math.floor(t)
         }
     }
 
-    function No(e, t, r = !1) {
+    function Io(e, t, r = !1) {
         const n = 10 ** t;
         return (r ? Math.trunc : Math.round)(e * n) / n
     }
 
-    function Io(e) {
+    function Fo(e) {
         return e % 4 == 0 && (e % 100 != 0 || e % 400 == 0)
     }
 
-    function Fo(e) {
-        return Io(e) ? 366 : 365
+    function Mo(e) {
+        return Fo(e) ? 366 : 365
     }
 
-    function Mo(e, t) {
+    function Po(e, t) {
         const r = function(e, t) {
             return e - t * Math.floor(e / t)
         }(t - 1, 12) + 1;
-        return 2 === r ? Io(e + (t - r) / 12) ? 29 : 28 : [31, null, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31][r - 1]
+        return 2 === r ? Fo(e + (t - r) / 12) ? 29 : 28 : [31, null, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31][r - 1]
     }
 
-    function Po(e) {
+    function jo(e) {
         let t = Date.UTC(e.year, e.month - 1, e.day, e.hour, e.minute, e.second, e.millisecond);
         return e.year < 100 && e.year >= 0 && (t = new Date(t), t.setUTCFullYear(e.year, e.month - 1, e.day)), +t
     }
 
-    function jo(e) {
+    function Bo(e) {
         const t = (e + Math.floor(e / 4) - Math.floor(e / 100) + Math.floor(e / 400)) % 7,
             r = e - 1,
             n = (r + Math.floor(r / 4) - Math.floor(r / 100) + Math.floor(r / 400)) % 7;
         return 4 === t || 3 === n ? 53 : 52
     }
 
-    function Bo(e) {
-        return e > 99 ? e : e > xo.twoDigitCutoffYear ? 1900 + e : 2e3 + e
+    function Uo(e) {
+        return e > 99 ? e : e > Ao.twoDigitCutoffYear ? 1900 + e : 2e3 + e
     }
 
-    function Uo(e, t, r, n = null) {
+    function Vo(e, t, r, n = null) {
         const i = new Date(e),
             o = {
                 hourCycle: "h23",
                 year: "numeric",
                 month: "2-digit",
                 day: "2-digit",
                 hour: "2-digit",
@@ -8662,144 +8682,144 @@
                 timeZoneName: t,
                 ...o
             },
             a = new Intl.DateTimeFormat(r, s).formatToParts(i).find((e => "timezonename" === e.type.toLowerCase()));
         return a ? a.value : null
     }
 
-    function Vo(e, t) {
+    function zo(e, t) {
         let r = parseInt(e, 10);
         Number.isNaN(r) && (r = 0);
         const n = parseInt(t, 10) || 0;
         return 60 * r + (r < 0 || Object.is(r, -0) ? -n : n)
     }
 
-    function zo(e) {
+    function Ho(e) {
         const t = Number(e);
-        if ("boolean" == typeof e || "" === e || Number.isNaN(t)) throw new wi(`Invalid unit value ${e}`);
+        if ("boolean" == typeof e || "" === e || Number.isNaN(t)) throw new _i(`Invalid unit value ${e}`);
         return t
     }
 
-    function Ho(e, t) {
+    function Wo(e, t) {
         const r = {};
         for (const n in e)
-            if (Oo(e, n)) {
+            if (So(e, n)) {
                 const i = e[n];
                 if (null == i) continue;
-                r[t(n)] = zo(i)
+                r[t(n)] = Ho(i)
             } return r
     }
 
-    function Wo(e, t) {
+    function Go(e, t) {
         const r = Math.trunc(Math.abs(e / 60)),
             n = Math.trunc(Math.abs(e % 60)),
             i = e >= 0 ? "+" : "-";
         switch (t) {
             case "short":
-                return `${i}${Do(r,2)}:${Do(n,2)}`;
+                return `${i}${Co(r,2)}:${Co(n,2)}`;
             case "narrow":
                 return `${i}${r}${n>0?`:${n}`:""}`;
             case "techie":
-                return `${i}${Do(r,2)}${Do(n,2)}`;
+                return `${i}${Co(r,2)}${Co(n,2)}`;
             default:
                 throw new RangeError(`Value format ${t} is out of range for property format`)
         }
     }
 
-    function Go(e) {
+    function Zo(e) {
         return function(e, t) {
             return t.reduce(((t, r) => (t[r] = e[r], t)), {})
         }(e, ["hour", "minute", "second", "millisecond"])
     }
-    const Zo = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"],
-        Jo = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-        Yo = ["J", "F", "M", "A", "M", "J", "J", "A", "S", "O", "N", "D"];
+    const Jo = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"],
+        Yo = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+        Ko = ["J", "F", "M", "A", "M", "J", "J", "A", "S", "O", "N", "D"];
 
-    function Ko(e) {
+    function Xo(e) {
         switch (e) {
             case "narrow":
-                return [...Yo];
+                return [...Ko];
             case "short":
-                return [...Jo];
+                return [...Yo];
             case "long":
-                return [...Zo];
+                return [...Jo];
             case "numeric":
                 return ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"];
             case "2-digit":
                 return ["01", "02", "03", "04", "05", "06", "07", "08", "09", "10", "11", "12"];
             default:
                 return null
         }
     }
-    const Xo = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
-        Qo = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
-        es = ["M", "T", "W", "T", "F", "S", "S"];
+    const Qo = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
+        es = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
+        ts = ["M", "T", "W", "T", "F", "S", "S"];
 
-    function ts(e) {
+    function rs(e) {
         switch (e) {
             case "narrow":
-                return [...es];
+                return [...ts];
             case "short":
-                return [...Qo];
+                return [...es];
             case "long":
-                return [...Xo];
+                return [...Qo];
             case "numeric":
                 return ["1", "2", "3", "4", "5", "6", "7"];
             default:
                 return null
         }
     }
-    const rs = ["AM", "PM"],
-        ns = ["Before Christ", "Anno Domini"],
-        is = ["BC", "AD"],
-        os = ["B", "A"];
+    const ns = ["AM", "PM"],
+        is = ["Before Christ", "Anno Domini"],
+        os = ["BC", "AD"],
+        ss = ["B", "A"];
 
-    function ss(e) {
+    function as(e) {
         switch (e) {
             case "narrow":
-                return [...os];
+                return [...ss];
             case "short":
-                return [...is];
+                return [...os];
             case "long":
-                return [...ns];
+                return [...is];
             default:
                 return null
         }
     }
 
-    function as(e, t) {
+    function ls(e, t) {
         let r = "";
         for (const n of e) n.literal ? r += n.val : r += t(n.val);
         return r
     }
-    const ls = {
-        D: qi,
-        DD: Ei,
-        DDD: $i,
-        DDDD: Oi,
-        t: Si,
-        tt: Di,
-        ttt: Ci,
-        tttt: Ri,
-        T: Li,
-        TT: Ni,
-        TTT: Ii,
-        TTTT: Fi,
-        f: Mi,
-        ff: ji,
-        fff: Vi,
-        ffff: Hi,
-        F: Pi,
-        FF: Bi,
-        FFF: zi,
-        FFFF: Wi
+    const us = {
+        D: Ei,
+        DD: Ti,
+        DDD: Oi,
+        DDDD: Si,
+        t: Di,
+        tt: Ci,
+        ttt: Ri,
+        tttt: Li,
+        T: Ni,
+        TT: Ii,
+        TTT: Fi,
+        TTTT: Mi,
+        f: Pi,
+        ff: Bi,
+        fff: zi,
+        ffff: Wi,
+        F: ji,
+        FF: Ui,
+        FFF: Hi,
+        FFFF: Gi
     };
-    class us {
+    class cs {
         static create(e, t = {}) {
-            return new us(e, t)
+            return new cs(e, t)
         }
         static parseFormat(e) {
             let t = null,
                 r = "",
                 n = !1;
             const i = [];
             for (let o = 0; o < e.length; o++) {
@@ -8814,15 +8834,15 @@
             }
             return r.length > 0 && i.push({
                 literal: n || /^\s+$/.test(r),
                 val: r
             }), i
         }
         static macroTokenToFormatOpts(e) {
-            return ls[e]
+            return us[e]
         }
         constructor(e, t) {
             this.opts = t, this.loc = e, this.systemLoc = null
         }
         formatWithSystemDefault(e, t) {
             null === this.systemLoc && (this.systemLoc = this.loc.redefaultToSystem());
             return this.systemLoc.dtFormatter(e, {
@@ -8851,58 +8871,58 @@
         resolvedOptions(e, t = {}) {
             return this.loc.dtFormatter(e, {
                 ...this.opts,
                 ...t
             }).resolvedOptions()
         }
         num(e, t = 0) {
-            if (this.opts.forceSimple) return Do(e, t);
+            if (this.opts.forceSimple) return Co(e, t);
             const r = {
                 ...this.opts
             };
             return t > 0 && (r.padTo = t), this.loc.numberFormatter(r).format(e)
         }
         formatDateTimeFromString(e, t) {
             const r = "en" === this.loc.listingMode(),
                 n = this.loc.outputCalendar && "gregory" !== this.loc.outputCalendar,
                 i = (t, r) => this.loc.extract(e, t, r),
                 o = t => e.isOffsetFixed && 0 === e.offset && t.allowZ ? "Z" : e.isValid ? e.zone.formatOffset(e.ts, t.format) : "",
                 s = () => r ? function(e) {
-                    return rs[e.hour < 12 ? 0 : 1]
+                    return ns[e.hour < 12 ? 0 : 1]
                 }(e) : i({
                     hour: "numeric",
                     hourCycle: "h12"
                 }, "dayperiod"),
                 a = (t, n) => r ? function(e, t) {
-                    return Ko(t)[e.month - 1]
+                    return Xo(t)[e.month - 1]
                 }(e, t) : i(n ? {
                     month: t
                 } : {
                     month: t,
                     day: "numeric"
                 }, "month"),
                 l = (t, n) => r ? function(e, t) {
-                    return ts(t)[e.weekday - 1]
+                    return rs(t)[e.weekday - 1]
                 }(e, t) : i(n ? {
                     weekday: t
                 } : {
                     weekday: t,
                     month: "long",
                     day: "numeric"
                 }, "weekday"),
                 u = t => {
-                    const r = us.macroTokenToFormatOpts(t);
+                    const r = cs.macroTokenToFormatOpts(t);
                     return r ? this.formatWithSystemDefault(e, r) : t
                 },
                 c = t => r ? function(e, t) {
-                    return ss(t)[e.year < 0 ? 0 : 1]
+                    return as(t)[e.year < 0 ? 0 : 1]
                 }(e, t) : i({
                     era: t
                 }, "era");
-            return as(us.parseFormat(t), (t => {
+            return ls(cs.parseFormat(t), (t => {
                 switch (t) {
                     case "S":
                         return this.num(e.millisecond);
                     case "u":
                     case "SSS":
                         return this.num(e.millisecond, 3);
                     case "s":
@@ -9073,176 +9093,176 @@
                             return "month";
                         case "y":
                             return "year";
                         default:
                             return null
                     }
                 },
-                n = us.parseFormat(t),
+                n = cs.parseFormat(t),
                 i = n.reduce(((e, {
                     literal: t,
                     val: r
                 }) => t ? e : e.concat(r)), []);
-            return as(n, (e => t => {
+            return ls(n, (e => t => {
                 const n = r(t);
                 return n ? this.num(e.get(n), t.length) : t
             })(e.shiftTo(...i.map(r).filter((e => e)))))
         }
     }
-    class cs {
+    class fs {
         constructor(e, t) {
             this.reason = e, this.explanation = t
         }
         toMessage() {
             return this.explanation ? `${this.reason}: ${this.explanation}` : this.reason
         }
     }
-    const fs = /[A-Za-z_+-]{1,256}(?::?\/[A-Za-z0-9_+-]{1,256}(?:\/[A-Za-z0-9_+-]{1,256})?)?/;
+    const hs = /[A-Za-z_+-]{1,256}(?::?\/[A-Za-z0-9_+-]{1,256}(?:\/[A-Za-z0-9_+-]{1,256})?)?/;
 
-    function hs(...e) {
+    function ps(...e) {
         const t = e.reduce(((e, t) => e + t.source), "");
         return RegExp(`^${t}$`)
     }
 
-    function ps(...e) {
+    function ds(...e) {
         return t => e.reduce((([e, r, n], i) => {
             const [o, s, a] = i(t, n);
             return [{
                 ...e,
                 ...o
             }, s || r, a]
         }), [{}, null, 1]).slice(0, 2)
     }
 
-    function ds(e, ...t) {
+    function ms(e, ...t) {
         if (null == e) return [null, null];
         for (const [r, n] of t) {
             const t = r.exec(e);
             if (t) return n(t)
         }
         return [null, null]
     }
 
-    function ms(...e) {
+    function gs(...e) {
         return (t, r) => {
             const n = {};
             let i;
-            for (i = 0; i < e.length; i++) n[e[i]] = Co(t[r + i]);
+            for (i = 0; i < e.length; i++) n[e[i]] = Ro(t[r + i]);
             return [n, null, r + i]
         }
     }
-    const gs = /(?:(Z)|([+-]\d\d)(?::?(\d\d))?)/,
-        vs = /(\d\d)(?::?(\d\d)(?::?(\d\d)(?:[.,](\d{1,30}))?)?)?/,
-        ys = RegExp(`${vs.source}${`(?:${gs.source}?(?:\\[(${fs.source})\\])?)?`}`),
-        bs = RegExp(`(?:T${ys.source})?`),
-        ws = ms("weekYear", "weekNumber", "weekDay"),
-        _s = ms("year", "ordinal"),
-        ks = RegExp(`${vs.source} ?(?:${gs.source}|(${fs.source}))?`),
-        xs = RegExp(`(?: ${ks.source})?`);
+    const vs = /(?:(Z)|([+-]\d\d)(?::?(\d\d))?)/,
+        ys = /(\d\d)(?::?(\d\d)(?::?(\d\d)(?:[.,](\d{1,30}))?)?)?/,
+        bs = RegExp(`${ys.source}${`(?:${vs.source}?(?:\\[(${hs.source})\\])?)?`}`),
+        ws = RegExp(`(?:T${bs.source})?`),
+        _s = gs("weekYear", "weekNumber", "weekDay"),
+        ks = gs("year", "ordinal"),
+        xs = RegExp(`${ys.source} ?(?:${vs.source}|(${hs.source}))?`),
+        As = RegExp(`(?: ${xs.source})?`);
 
-    function As(e, t, r) {
+    function qs(e, t, r) {
         const n = e[t];
-        return Ao(n) ? r : Co(n)
+        return qo(n) ? r : Ro(n)
     }
 
-    function qs(e, t) {
+    function Es(e, t) {
         return [{
-            hours: As(e, t, 0),
-            minutes: As(e, t + 1, 0),
-            seconds: As(e, t + 2, 0),
-            milliseconds: Lo(e[t + 3])
+            hours: qs(e, t, 0),
+            minutes: qs(e, t + 1, 0),
+            seconds: qs(e, t + 2, 0),
+            milliseconds: No(e[t + 3])
         }, null, t + 4]
     }
 
-    function Es(e, t) {
+    function Ts(e, t) {
         const r = !e[t] && !e[t + 1],
-            n = Vo(e[t + 1], e[t + 2]);
-        return [{}, r ? null : ho.instance(n), t + 3]
+            n = zo(e[t + 1], e[t + 2]);
+        return [{}, r ? null : po.instance(n), t + 3]
     }
 
-    function Ts(e, t) {
-        return [{}, e[t] ? Qi.create(e[t]) : null, t + 1]
+    function $s(e, t) {
+        return [{}, e[t] ? eo.create(e[t]) : null, t + 1]
     }
-    const $s = RegExp(`^T?${vs.source}$`),
-        Os = /^-?P(?:(?:(-?\d{1,20}(?:\.\d{1,20})?)Y)?(?:(-?\d{1,20}(?:\.\d{1,20})?)M)?(?:(-?\d{1,20}(?:\.\d{1,20})?)W)?(?:(-?\d{1,20}(?:\.\d{1,20})?)D)?(?:T(?:(-?\d{1,20}(?:\.\d{1,20})?)H)?(?:(-?\d{1,20}(?:\.\d{1,20})?)M)?(?:(-?\d{1,20})(?:[.,](-?\d{1,20}))?S)?)?)$/;
+    const Os = RegExp(`^T?${ys.source}$`),
+        Ss = /^-?P(?:(?:(-?\d{1,20}(?:\.\d{1,20})?)Y)?(?:(-?\d{1,20}(?:\.\d{1,20})?)M)?(?:(-?\d{1,20}(?:\.\d{1,20})?)W)?(?:(-?\d{1,20}(?:\.\d{1,20})?)D)?(?:T(?:(-?\d{1,20}(?:\.\d{1,20})?)H)?(?:(-?\d{1,20}(?:\.\d{1,20})?)M)?(?:(-?\d{1,20})(?:[.,](-?\d{1,20}))?S)?)?)$/;
 
-    function Ss(e) {
+    function Ds(e) {
         const [t, r, n, i, o, s, a, l, u] = e, c = "-" === t[0], f = l && "-" === l[0], h = (e, t = !1) => void 0 !== e && (t || e && c) ? -e : e;
         return [{
-            years: h(Ro(r)),
-            months: h(Ro(n)),
-            weeks: h(Ro(i)),
-            days: h(Ro(o)),
-            hours: h(Ro(s)),
-            minutes: h(Ro(a)),
-            seconds: h(Ro(l), "-0" === l),
-            milliseconds: h(Lo(u), f)
+            years: h(Lo(r)),
+            months: h(Lo(n)),
+            weeks: h(Lo(i)),
+            days: h(Lo(o)),
+            hours: h(Lo(s)),
+            minutes: h(Lo(a)),
+            seconds: h(Lo(l), "-0" === l),
+            milliseconds: h(No(u), f)
         }]
     }
-    const Ds = {
+    const Cs = {
         GMT: 0,
         EDT: -240,
         EST: -300,
         CDT: -300,
         CST: -360,
         MDT: -360,
         MST: -420,
         PDT: -420,
         PST: -480
     };
 
-    function Cs(e, t, r, n, i, o, s) {
+    function Rs(e, t, r, n, i, o, s) {
         const a = {
-            year: 2 === t.length ? Bo(Co(t)) : Co(t),
-            month: Jo.indexOf(r) + 1,
-            day: Co(n),
-            hour: Co(i),
-            minute: Co(o)
+            year: 2 === t.length ? Uo(Ro(t)) : Ro(t),
+            month: Yo.indexOf(r) + 1,
+            day: Ro(n),
+            hour: Ro(i),
+            minute: Ro(o)
         };
-        return s && (a.second = Co(s)), e && (a.weekday = e.length > 3 ? Xo.indexOf(e) + 1 : Qo.indexOf(e) + 1), a
+        return s && (a.second = Ro(s)), e && (a.weekday = e.length > 3 ? Qo.indexOf(e) + 1 : es.indexOf(e) + 1), a
     }
-    const Rs = /^(?:(Mon|Tue|Wed|Thu|Fri|Sat|Sun),\s)?(\d{1,2})\s(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s(\d{2,4})\s(\d\d):(\d\d)(?::(\d\d))?\s(?:(UT|GMT|[ECMP][SD]T)|([Zz])|(?:([+-]\d\d)(\d\d)))$/;
+    const Ls = /^(?:(Mon|Tue|Wed|Thu|Fri|Sat|Sun),\s)?(\d{1,2})\s(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s(\d{2,4})\s(\d\d):(\d\d)(?::(\d\d))?\s(?:(UT|GMT|[ECMP][SD]T)|([Zz])|(?:([+-]\d\d)(\d\d)))$/;
 
-    function Ls(e) {
-        const [, t, r, n, i, o, s, a, l, u, c, f] = e, h = Cs(t, i, n, r, o, s, a);
+    function Ns(e) {
+        const [, t, r, n, i, o, s, a, l, u, c, f] = e, h = Rs(t, i, n, r, o, s, a);
         let p;
-        return p = l ? Ds[l] : u ? 0 : Vo(c, f), [h, new ho(p)]
+        return p = l ? Cs[l] : u ? 0 : zo(c, f), [h, new po(p)]
     }
-    const Ns = /^(Mon|Tue|Wed|Thu|Fri|Sat|Sun), (\d\d) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) (\d{4}) (\d\d):(\d\d):(\d\d) GMT$/,
-        Is = /^(Monday|Tuesday|Wednesday|Thursday|Friday|Saturday|Sunday), (\d\d)-(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)-(\d\d) (\d\d):(\d\d):(\d\d) GMT$/,
-        Fs = /^(Mon|Tue|Wed|Thu|Fri|Sat|Sun) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) ( \d|\d\d) (\d\d):(\d\d):(\d\d) (\d{4})$/;
+    const Is = /^(Mon|Tue|Wed|Thu|Fri|Sat|Sun), (\d\d) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) (\d{4}) (\d\d):(\d\d):(\d\d) GMT$/,
+        Fs = /^(Monday|Tuesday|Wednesday|Thursday|Friday|Saturday|Sunday), (\d\d)-(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)-(\d\d) (\d\d):(\d\d):(\d\d) GMT$/,
+        Ms = /^(Mon|Tue|Wed|Thu|Fri|Sat|Sun) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) ( \d|\d\d) (\d\d):(\d\d):(\d\d) (\d{4})$/;
 
-    function Ms(e) {
+    function Ps(e) {
         const [, t, r, n, i, o, s, a] = e;
-        return [Cs(t, i, n, r, o, s, a), ho.utcInstance]
+        return [Rs(t, i, n, r, o, s, a), po.utcInstance]
     }
 
-    function Ps(e) {
+    function js(e) {
         const [, t, r, n, i, o, s, a] = e;
-        return [Cs(t, a, r, n, i, o, s), ho.utcInstance]
+        return [Rs(t, a, r, n, i, o, s), po.utcInstance]
     }
-    const js = hs(/([+-]\d{6}|\d{4})(?:-?(\d\d)(?:-?(\d\d))?)?/, bs),
-        Bs = hs(/(\d{4})-?W(\d\d)(?:-?(\d))?/, bs),
-        Us = hs(/(\d{4})-?(\d{3})/, bs),
-        Vs = hs(ys),
-        zs = ps((function(e, t) {
+    const Bs = ps(/([+-]\d{6}|\d{4})(?:-?(\d\d)(?:-?(\d\d))?)?/, ws),
+        Us = ps(/(\d{4})-?W(\d\d)(?:-?(\d))?/, ws),
+        Vs = ps(/(\d{4})-?(\d{3})/, ws),
+        zs = ps(bs),
+        Hs = ds((function(e, t) {
             return [{
-                year: As(e, t),
-                month: As(e, t + 1, 1),
-                day: As(e, t + 2, 1)
+                year: qs(e, t),
+                month: qs(e, t + 1, 1),
+                day: qs(e, t + 2, 1)
             }, null, t + 3]
-        }), qs, Es, Ts),
-        Hs = ps(ws, qs, Es, Ts),
-        Ws = ps(_s, qs, Es, Ts),
-        Gs = ps(qs, Es, Ts);
-    const Zs = ps(qs);
-    const Js = hs(/(\d{4})-(\d\d)-(\d\d)/, xs),
-        Ys = hs(ks),
-        Ks = ps(qs, Es, Ts);
-    const Xs = {
+        }), Es, Ts, $s),
+        Ws = ds(_s, Es, Ts, $s),
+        Gs = ds(ks, Es, Ts, $s),
+        Zs = ds(Es, Ts, $s);
+    const Js = ds(Es);
+    const Ys = ps(/(\d{4})-(\d\d)-(\d\d)/, As),
+        Ks = ps(xs),
+        Xs = ds(Es, Ts, $s);
+    const Qs = {
             weeks: {
                 days: 7,
                 hours: 168,
                 minutes: 10080,
                 seconds: 604800,
                 milliseconds: 6048e5
             },
@@ -9261,15 +9281,15 @@
                 seconds: 60,
                 milliseconds: 6e4
             },
             seconds: {
                 milliseconds: 1e3
             }
         },
-        Qs = {
+        ea = {
             years: {
                 quarters: 4,
                 months: 12,
                 weeks: 52,
                 days: 365,
                 hours: 8760,
                 minutes: 525600,
@@ -9289,24 +9309,24 @@
                 weeks: 4,
                 days: 30,
                 hours: 720,
                 minutes: 43200,
                 seconds: 2592e3,
                 milliseconds: 2592e6
             },
-            ...Xs
+            ...Qs
         },
-        ea = 365.2425,
-        ta = 30.436875,
-        ra = {
+        ta = 365.2425,
+        ra = 30.436875,
+        na = {
             years: {
                 quarters: 4,
                 months: 12,
                 weeks: 52.1775,
-                days: ea,
+                days: ta,
                 hours: 8765.82,
                 minutes: 525949.2,
                 seconds: 525949.2 * 60,
                 milliseconds: 525949.2 * 60 * 1e3
             },
             quarters: {
                 months: 3,
@@ -9315,89 +9335,89 @@
                 hours: 2191.455,
                 minutes: 131487.3,
                 seconds: 525949.2 * 60 / 4,
                 milliseconds: 7889237999.999999
             },
             months: {
                 weeks: 4.3481250000000005,
-                days: ta,
+                days: ra,
                 hours: 730.485,
                 minutes: 43829.1,
                 seconds: 2629746,
                 milliseconds: 2629746e3
             },
-            ...Xs
+            ...Qs
         },
-        na = ["years", "quarters", "months", "weeks", "days", "hours", "minutes", "seconds", "milliseconds"],
-        ia = na.slice(0).reverse();
+        ia = ["years", "quarters", "months", "weeks", "days", "hours", "minutes", "seconds", "milliseconds"],
+        oa = ia.slice(0).reverse();
 
-    function oa(e, t, r = !1) {
+    function sa(e, t, r = !1) {
         const n = {
             values: r ? t.values : {
                 ...e.values,
                 ...t.values || {}
             },
             loc: e.loc.clone(t.loc),
             conversionAccuracy: t.conversionAccuracy || e.conversionAccuracy,
             matrix: t.matrix || e.matrix
         };
-        return new aa(n)
+        return new la(n)
     }
 
-    function sa(e, t, r, n, i) {
+    function aa(e, t, r, n, i) {
         const o = e[i][r],
             s = t[r] / o,
             a = !(Math.sign(s) === Math.sign(n[i])) && 0 !== n[i] && Math.abs(s) <= 1 ? function(e) {
                 return e < 0 ? Math.floor(e) : Math.ceil(e)
             }(s) : Math.trunc(s);
         n[i] += a, t[r] -= a * o
     }
-    class aa {
+    class la {
         constructor(e) {
             const t = "longterm" === e.conversionAccuracy || !1;
-            let r = t ? ra : Qs;
-            e.matrix && (r = e.matrix), this.values = e.values, this.loc = e.loc || co.create(), this.conversionAccuracy = t ? "longterm" : "casual", this.invalid = e.invalid || null, this.matrix = r, this.isLuxonDuration = !0
+            let r = t ? na : ea;
+            e.matrix && (r = e.matrix), this.values = e.values, this.loc = e.loc || fo.create(), this.conversionAccuracy = t ? "longterm" : "casual", this.invalid = e.invalid || null, this.matrix = r, this.isLuxonDuration = !0
         }
         static fromMillis(e, t) {
-            return aa.fromObject({
+            return la.fromObject({
                 milliseconds: e
             }, t)
         }
         static fromObject(e, t = {}) {
-            if (null == e || "object" != typeof e) throw new wi("Duration.fromObject: argument expected to be an object, got " + (null === e ? "null" : typeof e));
-            return new aa({
-                values: Ho(e, aa.normalizeUnit),
-                loc: co.fromObject(t),
+            if (null == e || "object" != typeof e) throw new _i("Duration.fromObject: argument expected to be an object, got " + (null === e ? "null" : typeof e));
+            return new la({
+                values: Wo(e, la.normalizeUnit),
+                loc: fo.fromObject(t),
                 conversionAccuracy: t.conversionAccuracy,
                 matrix: t.matrix
             })
         }
         static fromDurationLike(e) {
-            if (qo(e)) return aa.fromMillis(e);
-            if (aa.isDuration(e)) return e;
-            if ("object" == typeof e) return aa.fromObject(e);
-            throw new wi(`Unknown duration argument ${e} of type ${typeof e}`)
+            if (Eo(e)) return la.fromMillis(e);
+            if (la.isDuration(e)) return e;
+            if ("object" == typeof e) return la.fromObject(e);
+            throw new _i(`Unknown duration argument ${e} of type ${typeof e}`)
         }
         static fromISO(e, t) {
             const [r] = function(e) {
-                return ds(e, [Os, Ss])
+                return ms(e, [Ss, Ds])
             }(e);
-            return r ? aa.fromObject(r, t) : aa.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
+            return r ? la.fromObject(r, t) : la.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
         }
         static fromISOTime(e, t) {
             const [r] = function(e) {
-                return ds(e, [$s, Zs])
+                return ms(e, [Os, Js])
             }(e);
-            return r ? aa.fromObject(r, t) : aa.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
+            return r ? la.fromObject(r, t) : la.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
         }
         static invalid(e, t = null) {
-            if (!e) throw new wi("need to specify a reason the Duration is invalid");
-            const r = e instanceof cs ? e : new cs(e, t);
-            if (xo.throwOnInvalid) throw new vi(r);
-            return new aa({
+            if (!e) throw new _i("need to specify a reason the Duration is invalid");
+            const r = e instanceof fs ? e : new fs(e, t);
+            if (Ao.throwOnInvalid) throw new yi(r);
+            return new la({
                 invalid: r
             })
         }
         static normalizeUnit(e) {
             const t = {
                 year: "years",
                 years: "years",
@@ -9414,15 +9434,15 @@
                 minute: "minutes",
                 minutes: "minutes",
                 second: "seconds",
                 seconds: "seconds",
                 millisecond: "milliseconds",
                 milliseconds: "milliseconds"
             } [e ? e.toLowerCase() : e];
-            if (!t) throw new bi(e);
+            if (!t) throw new wi(e);
             return t
         }
         static isDuration(e) {
             return e && e.isLuxonDuration || !1
         }
         get locale() {
             return this.isValid ? this.loc.locale : null
@@ -9431,20 +9451,20 @@
             return this.isValid ? this.loc.numberingSystem : null
         }
         toFormat(e, t = {}) {
             const r = {
                 ...t,
                 floor: !1 !== t.round && !1 !== t.floor
             };
-            return this.isValid ? us.create(this.loc, r).formatDurationFromString(this, e) : "Invalid Duration"
+            return this.isValid ? cs.create(this.loc, r).formatDurationFromString(this, e) : "Invalid Duration"
         }
         toHuman(e = {}) {
-            const t = na.map((t => {
+            const t = ia.map((t => {
                 const r = this.values[t];
-                return Ao(r) ? null : this.loc.numberFormatter({
+                return qo(r) ? null : this.loc.numberFormatter({
                     style: "unit",
                     unitDisplay: "long",
                     ...e,
                     unit: t.slice(0, -1)
                 }).format(r)
             })).filter((e => e));
             return this.loc.listFormatter({
@@ -9457,15 +9477,15 @@
             return this.isValid ? {
                 ...this.values
             } : {}
         }
         toISO() {
             if (!this.isValid) return null;
             let e = "P";
-            return 0 !== this.years && (e += this.years + "Y"), 0 === this.months && 0 === this.quarters || (e += this.months + 3 * this.quarters + "M"), 0 !== this.weeks && (e += this.weeks + "W"), 0 !== this.days && (e += this.days + "D"), 0 === this.hours && 0 === this.minutes && 0 === this.seconds && 0 === this.milliseconds || (e += "T"), 0 !== this.hours && (e += this.hours + "H"), 0 !== this.minutes && (e += this.minutes + "M"), 0 === this.seconds && 0 === this.milliseconds || (e += No(this.seconds + this.milliseconds / 1e3, 3) + "S"), "P" === e && (e += "T0S"), e
+            return 0 !== this.years && (e += this.years + "Y"), 0 === this.months && 0 === this.quarters || (e += this.months + 3 * this.quarters + "M"), 0 !== this.weeks && (e += this.weeks + "W"), 0 !== this.days && (e += this.days + "D"), 0 === this.hours && 0 === this.minutes && 0 === this.seconds && 0 === this.milliseconds || (e += "T"), 0 !== this.hours && (e += this.hours + "H"), 0 !== this.minutes && (e += this.minutes + "M"), 0 === this.seconds && 0 === this.milliseconds || (e += Io(this.seconds + this.milliseconds / 1e3, 3) + "S"), "P" === e && (e += "T0S"), e
         }
         toISOTime(e = {}) {
             if (!this.isValid) return null;
             const t = this.toMillis();
             if (t < 0 || t >= 864e5) return null;
             e = {
                 suppressMilliseconds: !1,
@@ -9490,53 +9510,53 @@
             return this.as("milliseconds")
         }
         valueOf() {
             return this.toMillis()
         }
         plus(e) {
             if (!this.isValid) return this;
-            const t = aa.fromDurationLike(e),
+            const t = la.fromDurationLike(e),
                 r = {};
-            for (const e of na)(Oo(t.values, e) || Oo(this.values, e)) && (r[e] = t.get(e) + this.get(e));
-            return oa(this, {
+            for (const e of ia)(So(t.values, e) || So(this.values, e)) && (r[e] = t.get(e) + this.get(e));
+            return sa(this, {
                 values: r
             }, !0)
         }
         minus(e) {
             if (!this.isValid) return this;
-            const t = aa.fromDurationLike(e);
+            const t = la.fromDurationLike(e);
             return this.plus(t.negate())
         }
         mapUnits(e) {
             if (!this.isValid) return this;
             const t = {};
-            for (const r of Object.keys(this.values)) t[r] = zo(e(this.values[r], r));
-            return oa(this, {
+            for (const r of Object.keys(this.values)) t[r] = Ho(e(this.values[r], r));
+            return sa(this, {
                 values: t
             }, !0)
         }
         get(e) {
-            return this[aa.normalizeUnit(e)]
+            return this[la.normalizeUnit(e)]
         }
         set(e) {
             if (!this.isValid) return this;
-            return oa(this, {
+            return sa(this, {
                 values: {
                     ...this.values,
-                    ...Ho(e, aa.normalizeUnit)
+                    ...Wo(e, la.normalizeUnit)
                 }
             })
         }
         reconfigure({
             locale: e,
             numberingSystem: t,
             conversionAccuracy: r,
             matrix: n
         } = {}) {
-            return oa(this, {
+            return sa(this, {
                 loc: this.loc.clone({
                     locale: e,
                     numberingSystem: t
                 }),
                 matrix: n,
                 conversionAccuracy: r
             })
@@ -9544,61 +9564,61 @@
         as(e) {
             return this.isValid ? this.shiftTo(e).get(e) : NaN
         }
         normalize() {
             if (!this.isValid) return this;
             const e = this.toObject();
             return function(e, t) {
-                ia.reduce(((r, n) => Ao(t[n]) ? r : (r && sa(e, t, r, t, n), n)), null)
-            }(this.matrix, e), oa(this, {
+                oa.reduce(((r, n) => qo(t[n]) ? r : (r && aa(e, t, r, t, n), n)), null)
+            }(this.matrix, e), sa(this, {
                 values: e
             }, !0)
         }
         rescale() {
             if (!this.isValid) return this;
             const e = function(e) {
                 const t = {};
                 for (const [r, n] of Object.entries(e)) 0 !== n && (t[r] = n);
                 return t
             }(this.normalize().shiftToAll().toObject());
-            return oa(this, {
+            return sa(this, {
                 values: e
             }, !0)
         }
         shiftTo(...e) {
             if (!this.isValid) return this;
             if (0 === e.length) return this;
-            e = e.map((e => aa.normalizeUnit(e)));
+            e = e.map((e => la.normalizeUnit(e)));
             const t = {},
                 r = {},
                 n = this.toObject();
             let i;
-            for (const o of na)
+            for (const o of ia)
                 if (e.indexOf(o) >= 0) {
                     i = o;
                     let e = 0;
                     for (const t in r) e += this.matrix[t][o] * r[t], r[t] = 0;
-                    qo(n[o]) && (e += n[o]);
+                    Eo(n[o]) && (e += n[o]);
                     const s = Math.trunc(e);
                     t[o] = s, r[o] = (1e3 * e - 1e3 * s) / 1e3;
-                    for (const e in n) na.indexOf(e) > na.indexOf(o) && sa(this.matrix, n, e, t, o)
-                } else qo(n[o]) && (r[o] = n[o]);
+                    for (const e in n) ia.indexOf(e) > ia.indexOf(o) && aa(this.matrix, n, e, t, o)
+                } else Eo(n[o]) && (r[o] = n[o]);
             for (const e in r) 0 !== r[e] && (t[i] += e === i ? r[e] : r[e] / this.matrix[i][e]);
-            return oa(this, {
+            return sa(this, {
                 values: t
             }, !0).normalize()
         }
         shiftToAll() {
             return this.isValid ? this.shiftTo("years", "months", "weeks", "days", "hours", "minutes", "seconds", "milliseconds") : this
         }
         negate() {
             if (!this.isValid) return this;
             const e = {};
             for (const t of Object.keys(this.values)) e[t] = 0 === this.values[t] ? 0 : -this.values[t];
-            return oa(this, {
+            return sa(this, {
                 values: e
             }, !0)
         }
         get years() {
             return this.isValid ? this.values.years || 0 : NaN
         }
         get quarters() {
@@ -9633,78 +9653,78 @@
         }
         get invalidExplanation() {
             return this.invalid ? this.invalid.explanation : null
         }
         equals(e) {
             if (!this.isValid || !e.isValid) return !1;
             if (!this.loc.equals(e.loc)) return !1;
-            for (const n of na)
+            for (const n of ia)
                 if (t = this.values[n], r = e.values[n], !(void 0 === t || 0 === t ? void 0 === r || 0 === r : t === r)) return !1;
             var t, r;
             return !0
         }
     }
-    const la = "Invalid Interval";
-    class ua {
+    const ua = "Invalid Interval";
+    class ca {
         constructor(e) {
             this.s = e.start, this.e = e.end, this.invalid = e.invalid || null, this.isLuxonInterval = !0
         }
         static invalid(e, t = null) {
-            if (!e) throw new wi("need to specify a reason the Interval is invalid");
-            const r = e instanceof cs ? e : new cs(e, t);
-            if (xo.throwOnInvalid) throw new gi(r);
-            return new ua({
+            if (!e) throw new _i("need to specify a reason the Interval is invalid");
+            const r = e instanceof fs ? e : new fs(e, t);
+            if (Ao.throwOnInvalid) throw new vi(r);
+            return new ca({
                 invalid: r
             })
         }
         static fromDateTimes(e, t) {
-            const r = dl(e),
-                n = dl(t),
+            const r = ml(e),
+                n = ml(t),
                 i = function(e, t) {
-                    return e && e.isValid ? t && t.isValid ? t < e ? ua.invalid("end before start", `The end of an interval must be after its start, but you had start=${e.toISO()} and end=${t.toISO()}`) : null : ua.invalid("missing or invalid end") : ua.invalid("missing or invalid start")
+                    return e && e.isValid ? t && t.isValid ? t < e ? ca.invalid("end before start", `The end of an interval must be after its start, but you had start=${e.toISO()} and end=${t.toISO()}`) : null : ca.invalid("missing or invalid end") : ca.invalid("missing or invalid start")
                 }(r, n);
-            return null == i ? new ua({
+            return null == i ? new ca({
                 start: r,
                 end: n
             }) : i
         }
         static after(e, t) {
-            const r = aa.fromDurationLike(t),
-                n = dl(e);
-            return ua.fromDateTimes(n, n.plus(r))
+            const r = la.fromDurationLike(t),
+                n = ml(e);
+            return ca.fromDateTimes(n, n.plus(r))
         }
         static before(e, t) {
-            const r = aa.fromDurationLike(t),
-                n = dl(e);
-            return ua.fromDateTimes(n.minus(r), n)
+            const r = la.fromDurationLike(t),
+                n = ml(e);
+            return ca.fromDateTimes(n.minus(r), n)
         }
         static fromISO(e, t) {
             const [r, n] = (e || "").split("/", 2);
             if (r && n) {
                 let e, i, o, s;
                 try {
-                    e = pl.fromISO(r, t), i = e.isValid
+                    e = dl.fromISO(r, t), i = e.isValid
                 } catch (n) {
                     i = !1
                 }
                 try {
-                    o = pl.fromISO(n, t), s = o.isValid
+                    o = dl.fromISO(n, t), s = o.isValid
                 } catch (n) {
                     s = !1
                 }
-                if (i && s) return ua.fromDateTimes(e, o);
+                if (i && s) return ca.fromDateTimes(e, o);
                 if (i) {
-                    const r = aa.fromISO(n, t);
-                    if (r.isValid) return ua.after(e, r)
+                    const r = la.fromISO(n, t);
+                    if (r.isValid) return ca.after(e, r)
                 } else if (s) {
-                    const e = aa.fromISO(r, t);
-                    if (e.isValid) return ua.before(o, e)
+                    const e = la.fromISO(r, t);
+                    if (e.isValid) return ca.before(o, e)
                 }
             }
-            return ua.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
+            return ca.invalid("unparsable", `the input "${e}" can't be parsed as ISO 8601`)
         }
         static isInterval(e) {
             return e && e.isLuxonInterval || !1
         }
         get start() {
             return this.isValid ? this.s : null
         }
@@ -9744,41 +9764,41 @@
         contains(e) {
             return !!this.isValid && (this.s <= e && this.e > e)
         }
         set({
             start: e,
             end: t
         } = {}) {
-            return this.isValid ? ua.fromDateTimes(e || this.s, t || this.e) : this
+            return this.isValid ? ca.fromDateTimes(e || this.s, t || this.e) : this
         }
         splitAt(...e) {
             if (!this.isValid) return [];
-            const t = e.map(dl).filter((e => this.contains(e))).sort(),
+            const t = e.map(ml).filter((e => this.contains(e))).sort(),
                 r = [];
             let {
                 s: n
             } = this, i = 0;
             for (; n < this.e;) {
                 const e = t[i] || this.e,
                     o = +e > +this.e ? this.e : e;
-                r.push(ua.fromDateTimes(n, o)), n = o, i += 1
+                r.push(ca.fromDateTimes(n, o)), n = o, i += 1
             }
             return r
         }
         splitBy(e) {
-            const t = aa.fromDurationLike(e);
+            const t = la.fromDurationLike(e);
             if (!this.isValid || !t.isValid || 0 === t.as("milliseconds")) return [];
             let r, {
                     s: n
                 } = this,
                 i = 1;
             const o = [];
             for (; n < this.e;) {
                 const e = this.start.plus(t.mapUnits((e => e * i)));
-                r = +e > +this.e ? this.e : e, o.push(ua.fromDateTimes(n, r)), n = r, i += 1
+                r = +e > +this.e ? this.e : e, o.push(ca.fromDateTimes(n, r)), n = r, i += 1
             }
             return o
         }
         divideEqually(e) {
             return this.isValid ? this.splitBy(this.length() / e).slice(0, e) : []
         }
         overlaps(e) {
@@ -9796,21 +9816,21 @@
         equals(e) {
             return !(!this.isValid || !e.isValid) && (this.s.equals(e.s) && this.e.equals(e.e))
         }
         intersection(e) {
             if (!this.isValid) return this;
             const t = this.s > e.s ? this.s : e.s,
                 r = this.e < e.e ? this.e : e.e;
-            return t >= r ? null : ua.fromDateTimes(t, r)
+            return t >= r ? null : ca.fromDateTimes(t, r)
         }
         union(e) {
             if (!this.isValid) return this;
             const t = this.s < e.s ? this.s : e.s,
                 r = this.e > e.e ? this.e : e.e;
-            return ua.fromDateTimes(t, r)
+            return ca.fromDateTimes(t, r)
         }
         static merge(e) {
             const [t, r] = e.sort(((e, t) => e.s - t.s)).reduce((([e, t], r) => t ? t.overlaps(r) || t.abutsStart(r) ? [e, t.union(r)] : [e.concat([t]), r] : [e, r]), [
                 [], null
             ]);
             return r && t.push(r), t
         }
@@ -9822,144 +9842,144 @@
                     time: e.s,
                     type: "s"
                 }, {
                     time: e.e,
                     type: "e"
                 }])),
                 o = Array.prototype.concat(...i).sort(((e, t) => e.time - t.time));
-            for (const e of o) r += "s" === e.type ? 1 : -1, 1 === r ? t = e.time : (t && +t != +e.time && n.push(ua.fromDateTimes(t, e.time)), t = null);
-            return ua.merge(n)
+            for (const e of o) r += "s" === e.type ? 1 : -1, 1 === r ? t = e.time : (t && +t != +e.time && n.push(ca.fromDateTimes(t, e.time)), t = null);
+            return ca.merge(n)
         }
         difference(...e) {
-            return ua.xor([this].concat(e)).map((e => this.intersection(e))).filter((e => e && !e.isEmpty()))
+            return ca.xor([this].concat(e)).map((e => this.intersection(e))).filter((e => e && !e.isEmpty()))
         }
         toString() {
-            return this.isValid ? `[${this.s.toISO()} – ${this.e.toISO()})` : la
+            return this.isValid ? `[${this.s.toISO()} – ${this.e.toISO()})` : ua
         }
-        toLocaleString(e = qi, t = {}) {
-            return this.isValid ? us.create(this.s.loc.clone(t), e).formatInterval(this) : la
+        toLocaleString(e = Ei, t = {}) {
+            return this.isValid ? cs.create(this.s.loc.clone(t), e).formatInterval(this) : ua
         }
         toISO(e) {
-            return this.isValid ? `${this.s.toISO(e)}/${this.e.toISO(e)}` : la
+            return this.isValid ? `${this.s.toISO(e)}/${this.e.toISO(e)}` : ua
         }
         toISODate() {
-            return this.isValid ? `${this.s.toISODate()}/${this.e.toISODate()}` : la
+            return this.isValid ? `${this.s.toISODate()}/${this.e.toISODate()}` : ua
         }
         toISOTime(e) {
-            return this.isValid ? `${this.s.toISOTime(e)}/${this.e.toISOTime(e)}` : la
+            return this.isValid ? `${this.s.toISOTime(e)}/${this.e.toISOTime(e)}` : ua
         }
         toFormat(e, {
             separator: t = " – "
         } = {}) {
-            return this.isValid ? `${this.s.toFormat(e)}${t}${this.e.toFormat(e)}` : la
+            return this.isValid ? `${this.s.toFormat(e)}${t}${this.e.toFormat(e)}` : ua
         }
         toDuration(e, t) {
-            return this.isValid ? this.e.diff(this.s, e, t) : aa.invalid(this.invalidReason)
+            return this.isValid ? this.e.diff(this.s, e, t) : la.invalid(this.invalidReason)
         }
         mapEndpoints(e) {
-            return ua.fromDateTimes(e(this.s), e(this.e))
+            return ca.fromDateTimes(e(this.s), e(this.e))
         }
     }
-    class ca {
-        static hasDST(e = xo.defaultZone) {
-            const t = pl.now().setZone(e).set({
+    class fa {
+        static hasDST(e = Ao.defaultZone) {
+            const t = dl.now().setZone(e).set({
                 month: 12
             });
             return !e.isUniversal && t.offset !== t.set({
                 month: 6
             }).offset
         }
         static isValidIANAZone(e) {
-            return Qi.isValidZone(e)
+            return eo.isValidZone(e)
         }
         static normalizeZone(e) {
-            return mo(e, xo.defaultZone)
+            return go(e, Ao.defaultZone)
         }
         static months(e = "long", {
             locale: t = null,
             numberingSystem: r = null,
             locObj: n = null,
             outputCalendar: i = "gregory"
         } = {}) {
-            return (n || co.create(t, r, i)).months(e)
+            return (n || fo.create(t, r, i)).months(e)
         }
         static monthsFormat(e = "long", {
             locale: t = null,
             numberingSystem: r = null,
             locObj: n = null,
             outputCalendar: i = "gregory"
         } = {}) {
-            return (n || co.create(t, r, i)).months(e, !0)
+            return (n || fo.create(t, r, i)).months(e, !0)
         }
         static weekdays(e = "long", {
             locale: t = null,
             numberingSystem: r = null,
             locObj: n = null
         } = {}) {
-            return (n || co.create(t, r, null)).weekdays(e)
+            return (n || fo.create(t, r, null)).weekdays(e)
         }
         static weekdaysFormat(e = "long", {
             locale: t = null,
             numberingSystem: r = null,
             locObj: n = null
         } = {}) {
-            return (n || co.create(t, r, null)).weekdays(e, !0)
+            return (n || fo.create(t, r, null)).weekdays(e, !0)
         }
         static meridiems({
             locale: e = null
         } = {}) {
-            return co.create(e).meridiems()
+            return fo.create(e).meridiems()
         }
         static eras(e = "short", {
             locale: t = null
         } = {}) {
-            return co.create(t, null, "gregory").eras(e)
+            return fo.create(t, null, "gregory").eras(e)
         }
         static features() {
             return {
-                relative: To()
+                relative: $o()
             }
         }
     }
 
-    function fa(e, t) {
+    function ha(e, t) {
         const r = e => e.toUTC(0, {
                 keepLocalTime: !0
             }).startOf("day").valueOf(),
             n = r(t) - r(e);
-        return Math.floor(aa.fromMillis(n).as("days"))
+        return Math.floor(la.fromMillis(n).as("days"))
     }
 
-    function ha(e, t, r, n) {
+    function pa(e, t, r, n) {
         let [i, o, s, a] = function(e, t, r) {
             const n = [
                     ["years", (e, t) => t.year - e.year],
                     ["quarters", (e, t) => t.quarter - e.quarter + 4 * (t.year - e.year)],
                     ["months", (e, t) => t.month - e.month + 12 * (t.year - e.year)],
                     ["weeks", (e, t) => {
-                        const r = fa(e, t);
+                        const r = ha(e, t);
                         return (r - r % 7) / 7
                     }],
-                    ["days", fa]
+                    ["days", ha]
                 ],
                 i = {},
                 o = e;
             let s, a;
             for (const [l, u] of n) r.indexOf(l) >= 0 && (s = l, i[l] = u(e, t), a = o.plus(i), a > t ? (i[l]--, e = o.plus(i)) : e = a);
             return [e, i, a, s]
         }(e, t, r);
         const l = t - i,
             u = r.filter((e => ["hours", "minutes", "seconds", "milliseconds"].indexOf(e) >= 0));
         0 === u.length && (s < t && (s = i.plus({
             [a]: 1
         })), s !== i && (o[a] = (o[a] || 0) + l / (s - i)));
-        const c = aa.fromObject(o, n);
-        return u.length > 0 ? aa.fromMillis(l, n).shiftTo(...u).plus(c) : c
+        const c = la.fromObject(o, n);
+        return u.length > 0 ? la.fromMillis(l, n).shiftTo(...u).plus(c) : c
     }
-    const pa = {
+    const da = {
             arab: "[٠-٩]",
             arabext: "[۰-۹]",
             bali: "[᭐-᭙]",
             beng: "[০-৯]",
             deva: "[०-९]",
             fullwide: "[０-９]",
             gujr: "[૦-૯]",
@@ -9974,15 +9994,15 @@
             orya: "[୦-୯]",
             tamldec: "[௦-௯]",
             telu: "[౦-౯]",
             thai: "[๐-๙]",
             tibt: "[༠-༩]",
             latn: "\\d"
         },
-        da = {
+        ma = {
             arab: [1632, 1641],
             arabext: [1776, 1785],
             bali: [6992, 7001],
             beng: [2534, 2543],
             deva: [2406, 2415],
             fullwide: [65296, 65303],
             gujr: [2790, 2799],
@@ -9995,82 +10015,82 @@
             mymr: [4160, 4169],
             orya: [2918, 2927],
             tamldec: [3046, 3055],
             telu: [3174, 3183],
             thai: [3664, 3673],
             tibt: [3872, 3881]
         },
-        ma = pa.hanidec.replace(/[\[|\]]/g, "").split("");
+        ga = da.hanidec.replace(/[\[|\]]/g, "").split("");
 
-    function ga({
+    function va({
         numberingSystem: e
     }, t = "") {
-        return new RegExp(`${pa[e||"latn"]}${t}`)
+        return new RegExp(`${da[e||"latn"]}${t}`)
     }
-    const va = "missing Intl.DateTimeFormat.formatToParts support";
+    const ya = "missing Intl.DateTimeFormat.formatToParts support";
 
-    function ya(e, t = (e => e)) {
+    function ba(e, t = (e => e)) {
         return {
             regex: e,
             deser: ([e]) => t(function(e) {
                 let t = parseInt(e, 10);
                 if (isNaN(t)) {
                     t = "";
                     for (let r = 0; r < e.length; r++) {
                         const n = e.charCodeAt(r);
-                        if (-1 !== e[r].search(pa.hanidec)) t += ma.indexOf(e[r]);
+                        if (-1 !== e[r].search(da.hanidec)) t += ga.indexOf(e[r]);
                         else
-                            for (const e in da) {
-                                const [r, i] = da[e];
+                            for (const e in ma) {
+                                const [r, i] = ma[e];
                                 n >= r && n <= i && (t += n - r)
                             }
                     }
                     return parseInt(t, 10)
                 }
                 return t
             }(e))
         }
     }
-    const ba = `[ ${String.fromCharCode(160)}]`,
-        wa = new RegExp(ba, "g");
+    const wa = `[ ${String.fromCharCode(160)}]`,
+        _a = new RegExp(wa, "g");
 
-    function _a(e) {
-        return e.replace(/\./g, "\\.?").replace(wa, ba)
+    function ka(e) {
+        return e.replace(/\./g, "\\.?").replace(_a, wa)
     }
 
-    function ka(e) {
-        return e.replace(/\./g, "").replace(wa, " ").toLowerCase()
+    function xa(e) {
+        return e.replace(/\./g, "").replace(_a, " ").toLowerCase()
     }
 
-    function xa(e, t) {
+    function Aa(e, t) {
         return null === e ? null : {
-            regex: RegExp(e.map(_a).join("|")),
-            deser: ([r]) => e.findIndex((e => ka(r) === ka(e))) + t
+            regex: RegExp(e.map(ka).join("|")),
+            deser: ([r]) => e.findIndex((e => xa(r) === xa(e))) + t
         }
     }
 
-    function Aa(e, t) {
+    function qa(e, t) {
         return {
             regex: e,
-            deser: ([, e, t]) => Vo(e, t),
+            deser: ([, e, t]) => zo(e, t),
             groups: t
         }
     }
 
-    function qa(e) {
+    function Ea(e) {
         return {
             regex: e,
             deser: ([e]) => e
         }
     }
 
-    function Ea(e) {
+    function Ta(e) {
         return e.replace(/[\-\[\]{}()*+?.,\\\^$|#\s]/g, "\\$&")
     }
-    const Ta = {
+    const $a = {
         year: {
             "2-digit": "yy",
             numeric: "yyyyy"
         },
         month: {
             numeric: "M",
             "2-digit": "MM",
@@ -10100,128 +10120,128 @@
             "2-digit": "ss"
         },
         timeZoneName: {
             long: "ZZZZZ",
             short: "ZZZ"
         }
     };
-    let $a = null;
+    let Oa = null;
 
-    function Oa(e, t) {
+    function Sa(e, t) {
         return Array.prototype.concat(...e.map((e => function(e, t) {
             if (e.literal) return e;
-            const r = Da(us.macroTokenToFormatOpts(e.val), t);
+            const r = Ca(cs.macroTokenToFormatOpts(e.val), t);
             return null == r || r.includes(void 0) ? e : r
         }(e, t))))
     }
 
-    function Sa(e, t, r) {
-        const n = Oa(us.parseFormat(r), e),
+    function Da(e, t, r) {
+        const n = Sa(cs.parseFormat(r), e),
             i = n.map((t => function(e, t) {
-                const r = ga(t),
-                    n = ga(t, "{2}"),
-                    i = ga(t, "{3}"),
-                    o = ga(t, "{4}"),
-                    s = ga(t, "{6}"),
-                    a = ga(t, "{1,2}"),
-                    l = ga(t, "{1,3}"),
-                    u = ga(t, "{1,6}"),
-                    c = ga(t, "{1,9}"),
-                    f = ga(t, "{2,4}"),
-                    h = ga(t, "{4,6}"),
+                const r = va(t),
+                    n = va(t, "{2}"),
+                    i = va(t, "{3}"),
+                    o = va(t, "{4}"),
+                    s = va(t, "{6}"),
+                    a = va(t, "{1,2}"),
+                    l = va(t, "{1,3}"),
+                    u = va(t, "{1,6}"),
+                    c = va(t, "{1,9}"),
+                    f = va(t, "{2,4}"),
+                    h = va(t, "{4,6}"),
                     p = e => ({
-                        regex: RegExp(Ea(e.val)),
+                        regex: RegExp(Ta(e.val)),
                         deser: ([e]) => e,
                         literal: !0
                     }),
                     d = (d => {
                         if (e.literal) return p(d);
                         switch (d.val) {
                             case "G":
-                                return xa(t.eras("short", !1), 0);
+                                return Aa(t.eras("short", !1), 0);
                             case "GG":
-                                return xa(t.eras("long", !1), 0);
+                                return Aa(t.eras("long", !1), 0);
                             case "y":
-                                return ya(u);
+                                return ba(u);
                             case "yy":
                             case "kk":
-                                return ya(f, Bo);
+                                return ba(f, Uo);
                             case "yyyy":
                             case "kkkk":
-                                return ya(o);
+                                return ba(o);
                             case "yyyyy":
-                                return ya(h);
+                                return ba(h);
                             case "yyyyyy":
-                                return ya(s);
+                                return ba(s);
                             case "M":
                             case "L":
                             case "d":
                             case "H":
                             case "h":
                             case "m":
                             case "q":
                             case "s":
                             case "W":
-                                return ya(a);
+                                return ba(a);
                             case "MM":
                             case "LL":
                             case "dd":
                             case "HH":
                             case "hh":
                             case "mm":
                             case "qq":
                             case "ss":
                             case "WW":
-                                return ya(n);
+                                return ba(n);
                             case "MMM":
-                                return xa(t.months("short", !0, !1), 1);
+                                return Aa(t.months("short", !0, !1), 1);
                             case "MMMM":
-                                return xa(t.months("long", !0, !1), 1);
+                                return Aa(t.months("long", !0, !1), 1);
                             case "LLL":
-                                return xa(t.months("short", !1, !1), 1);
+                                return Aa(t.months("short", !1, !1), 1);
                             case "LLLL":
-                                return xa(t.months("long", !1, !1), 1);
+                                return Aa(t.months("long", !1, !1), 1);
                             case "o":
                             case "S":
-                                return ya(l);
+                                return ba(l);
                             case "ooo":
                             case "SSS":
-                                return ya(i);
+                                return ba(i);
                             case "u":
-                                return qa(c);
+                                return Ea(c);
                             case "uu":
-                                return qa(a);
+                                return Ea(a);
                             case "uuu":
                             case "E":
                             case "c":
-                                return ya(r);
+                                return ba(r);
                             case "a":
-                                return xa(t.meridiems(), 0);
+                                return Aa(t.meridiems(), 0);
                             case "EEE":
-                                return xa(t.weekdays("short", !1, !1), 1);
+                                return Aa(t.weekdays("short", !1, !1), 1);
                             case "EEEE":
-                                return xa(t.weekdays("long", !1, !1), 1);
+                                return Aa(t.weekdays("long", !1, !1), 1);
                             case "ccc":
-                                return xa(t.weekdays("short", !0, !1), 1);
+                                return Aa(t.weekdays("short", !0, !1), 1);
                             case "cccc":
-                                return xa(t.weekdays("long", !0, !1), 1);
+                                return Aa(t.weekdays("long", !0, !1), 1);
                             case "Z":
                             case "ZZ":
-                                return Aa(new RegExp(`([+-]${a.source})(?::(${n.source}))?`), 2);
+                                return qa(new RegExp(`([+-]${a.source})(?::(${n.source}))?`), 2);
                             case "ZZZ":
-                                return Aa(new RegExp(`([+-]${a.source})(${n.source})?`), 2);
+                                return qa(new RegExp(`([+-]${a.source})(${n.source})?`), 2);
                             case "z":
-                                return qa(/[a-z_+-/]{1,256}?/i);
+                                return Ea(/[a-z_+-/]{1,256}?/i);
                             case " ":
-                                return qa(/[^\S\n\r]/);
+                                return Ea(/[^\S\n\r]/);
                             default:
                                 return p(d)
                         }
                     })(e) || {
-                        invalidReason: va
+                        invalidReason: ya
                     };
                 return d.token = e, d
             }(t, e))),
             o = i.find((e => e.invalidReason));
         if (o) return {
             input: t,
             tokens: n,
@@ -10232,24 +10252,24 @@
                 return [`^${t}$`, e]
             }(i), o = RegExp(e, "i"), [s, a] = function(e, t, r) {
                 const n = e.match(t);
                 if (n) {
                     const e = {};
                     let t = 1;
                     for (const i in r)
-                        if (Oo(r, i)) {
+                        if (So(r, i)) {
                             const o = r[i],
                                 s = o.groups ? o.groups + 1 : 1;
                             !o.literal && o.token && (e[o.token.val[0]] = o.deser(n.slice(t, t + s))), t += s
                         } return [n, e]
                 }
                 return [n, {}]
             }(t, o, r), [l, u, c] = a ? function(e) {
                 let t, r = null;
-                Ao(e.z) || (r = Qi.create(e.z)), Ao(e.Z) || (r || (r = new ho(e.Z)), t = e.Z), Ao(e.q) || (e.M = 3 * (e.q - 1) + 1), Ao(e.h) || (e.h < 12 && 1 === e.a ? e.h += 12 : 12 === e.h && 0 === e.a && (e.h = 0)), 0 === e.G && e.y && (e.y = -e.y), Ao(e.u) || (e.S = Lo(e.u));
+                qo(e.z) || (r = eo.create(e.z)), qo(e.Z) || (r || (r = new po(e.Z)), t = e.Z), qo(e.q) || (e.M = 3 * (e.q - 1) + 1), qo(e.h) || (e.h < 12 && 1 === e.a ? e.h += 12 : 12 === e.h && 0 === e.a && (e.h = 0)), 0 === e.G && e.y && (e.y = -e.y), qo(e.u) || (e.S = No(e.u));
                 const n = Object.keys(e).reduce(((t, r) => {
                     const n = (e => {
                         switch (e) {
                             case "S":
                                 return "millisecond";
                             case "s":
                                 return "second";
@@ -10280,301 +10300,301 @@
                                 return null
                         }
                     })(r);
                     return n && (t[n] = e[r]), t
                 }), {});
                 return [n, r, t]
             }(a) : [null, null, void 0];
-            if (Oo(a, "a") && Oo(a, "H")) throw new yi("Can't include meridiem when specifying 24-hour format");
+            if (So(a, "a") && So(a, "H")) throw new bi("Can't include meridiem when specifying 24-hour format");
             return {
                 input: t,
                 tokens: n,
                 regex: o,
                 rawMatches: s,
                 matches: a,
                 result: l,
                 zone: u,
                 specificOffset: c
             }
         }
     }
 
-    function Da(e, t) {
+    function Ca(e, t) {
         if (!e) return null;
-        return us.create(t, e).formatDateTimeParts(($a || ($a = pl.fromMillis(1555555555555)), $a)).map((t => function(e, t) {
+        return cs.create(t, e).formatDateTimeParts((Oa || (Oa = dl.fromMillis(1555555555555)), Oa)).map((t => function(e, t) {
             const {
                 type: r,
                 value: n
             } = e;
             if ("literal" === r) {
                 const e = /^\s+$/.test(n);
                 return {
                     literal: !e,
                     val: e ? " " : n
                 }
             }
             const i = t[r];
-            let o = Ta[r];
+            let o = $a[r];
             if ("object" == typeof o && (o = o[i]), o) return {
                 literal: !1,
                 val: o
             }
         }(t, e)))
     }
-    const Ca = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334],
-        Ra = [0, 31, 60, 91, 121, 152, 182, 213, 244, 274, 305, 335];
+    const Ra = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334],
+        La = [0, 31, 60, 91, 121, 152, 182, 213, 244, 274, 305, 335];
 
-    function La(e, t) {
-        return new cs("unit out of range", `you specified ${t} (of type ${typeof t}) as a ${e}, which is invalid`)
+    function Na(e, t) {
+        return new fs("unit out of range", `you specified ${t} (of type ${typeof t}) as a ${e}, which is invalid`)
     }
 
-    function Na(e, t, r) {
+    function Ia(e, t, r) {
         const n = new Date(Date.UTC(e, t - 1, r));
         e < 100 && e >= 0 && n.setUTCFullYear(n.getUTCFullYear() - 1900);
         const i = n.getUTCDay();
         return 0 === i ? 7 : i
     }
 
-    function Ia(e, t, r) {
-        return r + (Io(e) ? Ra : Ca)[t - 1]
+    function Fa(e, t, r) {
+        return r + (Fo(e) ? La : Ra)[t - 1]
     }
 
-    function Fa(e, t) {
-        const r = Io(e) ? Ra : Ca,
+    function Ma(e, t) {
+        const r = Fo(e) ? La : Ra,
             n = r.findIndex((e => e < t));
         return {
             month: n + 1,
             day: t - r[n]
         }
     }
 
-    function Ma(e) {
+    function Pa(e) {
         const {
             year: t,
             month: r,
             day: n
-        } = e, i = Ia(t, r, n), o = Na(t, r, n);
+        } = e, i = Fa(t, r, n), o = Ia(t, r, n);
         let s, a = Math.floor((i - o + 10) / 7);
-        return a < 1 ? (s = t - 1, a = jo(s)) : a > jo(t) ? (s = t + 1, a = 1) : s = t, {
+        return a < 1 ? (s = t - 1, a = Bo(s)) : a > Bo(t) ? (s = t + 1, a = 1) : s = t, {
             weekYear: s,
             weekNumber: a,
             weekday: o,
-            ...Go(e)
+            ...Zo(e)
         }
     }
 
-    function Pa(e) {
+    function ja(e) {
         const {
             weekYear: t,
             weekNumber: r,
             weekday: n
-        } = e, i = Na(t, 1, 4), o = Fo(t);
+        } = e, i = Ia(t, 1, 4), o = Mo(t);
         let s, a = 7 * r + n - i - 3;
-        a < 1 ? (s = t - 1, a += Fo(s)) : a > o ? (s = t + 1, a -= Fo(t)) : s = t;
+        a < 1 ? (s = t - 1, a += Mo(s)) : a > o ? (s = t + 1, a -= Mo(t)) : s = t;
         const {
             month: l,
             day: u
-        } = Fa(s, a);
+        } = Ma(s, a);
         return {
             year: s,
             month: l,
             day: u,
-            ...Go(e)
+            ...Zo(e)
         }
     }
 
-    function ja(e) {
+    function Ba(e) {
         const {
             year: t,
             month: r,
             day: n
         } = e;
         return {
             year: t,
-            ordinal: Ia(t, r, n),
-            ...Go(e)
+            ordinal: Fa(t, r, n),
+            ...Zo(e)
         }
     }
 
-    function Ba(e) {
+    function Ua(e) {
         const {
             year: t,
             ordinal: r
         } = e, {
             month: n,
             day: i
-        } = Fa(t, r);
+        } = Ma(t, r);
         return {
             year: t,
             month: n,
             day: i,
-            ...Go(e)
+            ...Zo(e)
         }
     }
 
-    function Ua(e) {
-        const t = Eo(e.year),
-            r = So(e.month, 1, 12),
-            n = So(e.day, 1, Mo(e.year, e.month));
-        return t ? r ? !n && La("day", e.day) : La("month", e.month) : La("year", e.year)
+    function Va(e) {
+        const t = To(e.year),
+            r = Do(e.month, 1, 12),
+            n = Do(e.day, 1, Po(e.year, e.month));
+        return t ? r ? !n && Na("day", e.day) : Na("month", e.month) : Na("year", e.year)
     }
 
-    function Va(e) {
+    function za(e) {
         const {
             hour: t,
             minute: r,
             second: n,
             millisecond: i
-        } = e, o = So(t, 0, 23) || 24 === t && 0 === r && 0 === n && 0 === i, s = So(r, 0, 59), a = So(n, 0, 59), l = So(i, 0, 999);
-        return o ? s ? a ? !l && La("millisecond", i) : La("second", n) : La("minute", r) : La("hour", t)
+        } = e, o = Do(t, 0, 23) || 24 === t && 0 === r && 0 === n && 0 === i, s = Do(r, 0, 59), a = Do(n, 0, 59), l = Do(i, 0, 999);
+        return o ? s ? a ? !l && Na("millisecond", i) : Na("second", n) : Na("minute", r) : Na("hour", t)
     }
-    const za = "Invalid DateTime",
-        Ha = 864e13;
+    const Ha = "Invalid DateTime",
+        Wa = 864e13;
 
-    function Wa(e) {
-        return new cs("unsupported zone", `the zone "${e.name}" is not supported`)
+    function Ga(e) {
+        return new fs("unsupported zone", `the zone "${e.name}" is not supported`)
     }
 
-    function Ga(e) {
-        return null === e.weekData && (e.weekData = Ma(e.c)), e.weekData
+    function Za(e) {
+        return null === e.weekData && (e.weekData = Pa(e.c)), e.weekData
     }
 
-    function Za(e, t) {
+    function Ja(e, t) {
         const r = {
             ts: e.ts,
             zone: e.zone,
             c: e.c,
             o: e.o,
             loc: e.loc,
             invalid: e.invalid
         };
-        return new pl({
+        return new dl({
             ...r,
             ...t,
             old: r
         })
     }
 
-    function Ja(e, t, r) {
+    function Ya(e, t, r) {
         let n = e - 60 * t * 1e3;
         const i = r.offset(n);
         if (t === i) return [n, t];
         n -= 60 * (i - t) * 1e3;
         const o = r.offset(n);
         return i === o ? [n, i] : [e - 60 * Math.min(i, o) * 1e3, Math.max(i, o)]
     }
 
-    function Ya(e, t) {
+    function Ka(e, t) {
         const r = new Date(e += 60 * t * 1e3);
         return {
             year: r.getUTCFullYear(),
             month: r.getUTCMonth() + 1,
             day: r.getUTCDate(),
             hour: r.getUTCHours(),
             minute: r.getUTCMinutes(),
             second: r.getUTCSeconds(),
             millisecond: r.getUTCMilliseconds()
         }
     }
 
-    function Ka(e, t, r) {
-        return Ja(Po(e), t, r)
+    function Xa(e, t, r) {
+        return Ya(jo(e), t, r)
     }
 
-    function Xa(e, t) {
+    function Qa(e, t) {
         const r = e.o,
             n = e.c.year + Math.trunc(t.years),
             i = e.c.month + Math.trunc(t.months) + 3 * Math.trunc(t.quarters),
             o = {
                 ...e.c,
                 year: n,
                 month: i,
-                day: Math.min(e.c.day, Mo(n, i)) + Math.trunc(t.days) + 7 * Math.trunc(t.weeks)
+                day: Math.min(e.c.day, Po(n, i)) + Math.trunc(t.days) + 7 * Math.trunc(t.weeks)
             },
-            s = aa.fromObject({
+            s = la.fromObject({
                 years: t.years - Math.trunc(t.years),
                 quarters: t.quarters - Math.trunc(t.quarters),
                 months: t.months - Math.trunc(t.months),
                 weeks: t.weeks - Math.trunc(t.weeks),
                 days: t.days - Math.trunc(t.days),
                 hours: t.hours,
                 minutes: t.minutes,
                 seconds: t.seconds,
                 milliseconds: t.milliseconds
             }).as("milliseconds"),
-            a = Po(o);
-        let [l, u] = Ja(a, r, e.zone);
+            a = jo(o);
+        let [l, u] = Ya(a, r, e.zone);
         return 0 !== s && (l += s, u = e.zone.offset(l)), {
             ts: l,
             o: u
         }
     }
 
-    function Qa(e, t, r, n, i, o) {
+    function el(e, t, r, n, i, o) {
         const {
             setZone: s,
             zone: a
         } = r;
         if (e && 0 !== Object.keys(e).length || t) {
             const n = t || a,
-                i = pl.fromObject(e, {
+                i = dl.fromObject(e, {
                     ...r,
                     zone: n,
                     specificOffset: o
                 });
             return s ? i : i.setZone(a)
         }
-        return pl.invalid(new cs("unparsable", `the input "${i}" can't be parsed as ${n}`))
+        return dl.invalid(new fs("unparsable", `the input "${i}" can't be parsed as ${n}`))
     }
 
-    function el(e, t, r = !0) {
-        return e.isValid ? us.create(co.create("en-US"), {
+    function tl(e, t, r = !0) {
+        return e.isValid ? cs.create(fo.create("en-US"), {
             allowZ: r,
             forceSimple: !0
         }).formatDateTimeFromString(e, t) : null
     }
 
-    function tl(e, t) {
+    function rl(e, t) {
         const r = e.c.year > 9999 || e.c.year < 0;
         let n = "";
-        return r && e.c.year >= 0 && (n += "+"), n += Do(e.c.year, r ? 6 : 4), t ? (n += "-", n += Do(e.c.month), n += "-", n += Do(e.c.day)) : (n += Do(e.c.month), n += Do(e.c.day)), n
+        return r && e.c.year >= 0 && (n += "+"), n += Co(e.c.year, r ? 6 : 4), t ? (n += "-", n += Co(e.c.month), n += "-", n += Co(e.c.day)) : (n += Co(e.c.month), n += Co(e.c.day)), n
     }
 
-    function rl(e, t, r, n, i, o) {
-        let s = Do(e.c.hour);
-        return t ? (s += ":", s += Do(e.c.minute), 0 === e.c.second && r || (s += ":")) : s += Do(e.c.minute), 0 === e.c.second && r || (s += Do(e.c.second), 0 === e.c.millisecond && n || (s += ".", s += Do(e.c.millisecond, 3))), i && (e.isOffsetFixed && 0 === e.offset && !o ? s += "Z" : e.o < 0 ? (s += "-", s += Do(Math.trunc(-e.o / 60)), s += ":", s += Do(Math.trunc(-e.o % 60))) : (s += "+", s += Do(Math.trunc(e.o / 60)), s += ":", s += Do(Math.trunc(e.o % 60)))), o && (s += "[" + e.zone.ianaName + "]"), s
+    function nl(e, t, r, n, i, o) {
+        let s = Co(e.c.hour);
+        return t ? (s += ":", s += Co(e.c.minute), 0 === e.c.second && r || (s += ":")) : s += Co(e.c.minute), 0 === e.c.second && r || (s += Co(e.c.second), 0 === e.c.millisecond && n || (s += ".", s += Co(e.c.millisecond, 3))), i && (e.isOffsetFixed && 0 === e.offset && !o ? s += "Z" : e.o < 0 ? (s += "-", s += Co(Math.trunc(-e.o / 60)), s += ":", s += Co(Math.trunc(-e.o % 60))) : (s += "+", s += Co(Math.trunc(e.o / 60)), s += ":", s += Co(Math.trunc(e.o % 60)))), o && (s += "[" + e.zone.ianaName + "]"), s
     }
-    const nl = {
+    const il = {
             month: 1,
             day: 1,
             hour: 0,
             minute: 0,
             second: 0,
             millisecond: 0
         },
-        il = {
+        ol = {
             weekNumber: 1,
             weekday: 1,
             hour: 0,
             minute: 0,
             second: 0,
             millisecond: 0
         },
-        ol = {
+        sl = {
             ordinal: 1,
             hour: 0,
             minute: 0,
             second: 0,
             millisecond: 0
         },
-        sl = ["year", "month", "day", "hour", "minute", "second", "millisecond"],
-        al = ["weekYear", "weekNumber", "weekday", "hour", "minute", "second", "millisecond"],
-        ll = ["year", "ordinal", "hour", "minute", "second", "millisecond"];
+        al = ["year", "month", "day", "hour", "minute", "second", "millisecond"],
+        ll = ["weekYear", "weekNumber", "weekday", "hour", "minute", "second", "millisecond"],
+        ul = ["year", "ordinal", "hour", "minute", "second", "millisecond"];
 
-    function ul(e) {
+    function cl(e) {
         const t = {
             year: "year",
             years: "year",
             month: "month",
             months: "month",
             day: "day",
             days: "day",
@@ -10593,238 +10613,238 @@
             weeknumber: "weekNumber",
             weeksnumber: "weekNumber",
             weeknumbers: "weekNumber",
             weekyear: "weekYear",
             weekyears: "weekYear",
             ordinal: "ordinal"
         } [e.toLowerCase()];
-        if (!t) throw new bi(e);
+        if (!t) throw new wi(e);
         return t
     }
 
-    function cl(e, t) {
-        const r = mo(t.zone, xo.defaultZone),
-            n = co.fromObject(t),
-            i = xo.now();
+    function fl(e, t) {
+        const r = go(t.zone, Ao.defaultZone),
+            n = fo.fromObject(t),
+            i = Ao.now();
         let o, s;
-        if (Ao(e.year)) o = i;
+        if (qo(e.year)) o = i;
         else {
-            for (const t of sl) Ao(e[t]) && (e[t] = nl[t]);
-            const t = Ua(e) || Va(e);
-            if (t) return pl.invalid(t);
+            for (const t of al) qo(e[t]) && (e[t] = il[t]);
+            const t = Va(e) || za(e);
+            if (t) return dl.invalid(t);
             const n = r.offset(i);
-            [o, s] = Ka(e, n, r)
+            [o, s] = Xa(e, n, r)
         }
-        return new pl({
+        return new dl({
             ts: o,
             zone: r,
             loc: n,
             o: s
         })
     }
 
-    function fl(e, t, r) {
-        const n = !!Ao(r.round) || r.round,
+    function hl(e, t, r) {
+        const n = !!qo(r.round) || r.round,
             i = (e, i) => {
-                e = No(e, n || r.calendary ? 0 : 2, !0);
+                e = Io(e, n || r.calendary ? 0 : 2, !0);
                 return t.loc.clone(r).relFormatter(r).format(e, i)
             },
             o = n => r.calendary ? t.hasSame(e, n) ? 0 : t.startOf(n).diff(e.startOf(n), n).get(n) : t.diff(e, n).get(n);
         if (r.unit) return i(o(r.unit), r.unit);
         for (const e of r.units) {
             const t = o(e);
             if (Math.abs(t) >= 1) return i(t, e)
         }
         return i(e > t ? -0 : 0, r.units[r.units.length - 1])
     }
 
-    function hl(e) {
+    function pl(e) {
         let t, r = {};
         return e.length > 0 && "object" == typeof e[e.length - 1] ? (r = e[e.length - 1], t = Array.from(e).slice(0, e.length - 1)) : t = Array.from(e), [r, t]
     }
-    class pl {
+    class dl {
         constructor(e) {
-            const t = e.zone || xo.defaultZone;
-            let r = e.invalid || (Number.isNaN(e.ts) ? new cs("invalid input") : null) || (t.isValid ? null : Wa(t));
-            this.ts = Ao(e.ts) ? xo.now() : e.ts;
+            const t = e.zone || Ao.defaultZone;
+            let r = e.invalid || (Number.isNaN(e.ts) ? new fs("invalid input") : null) || (t.isValid ? null : Ga(t));
+            this.ts = qo(e.ts) ? Ao.now() : e.ts;
             let n = null,
                 i = null;
             if (!r) {
                 if (e.old && e.old.ts === this.ts && e.old.zone.equals(t))[n, i] = [e.old.c, e.old.o];
                 else {
                     const e = t.offset(this.ts);
-                    n = Ya(this.ts, e), r = Number.isNaN(n.year) ? new cs("invalid input") : null, n = r ? null : n, i = r ? null : e
+                    n = Ka(this.ts, e), r = Number.isNaN(n.year) ? new fs("invalid input") : null, n = r ? null : n, i = r ? null : e
                 }
             }
-            this._zone = t, this.loc = e.loc || co.create(), this.invalid = r, this.weekData = null, this.c = n, this.o = i, this.isLuxonDateTime = !0
+            this._zone = t, this.loc = e.loc || fo.create(), this.invalid = r, this.weekData = null, this.c = n, this.o = i, this.isLuxonDateTime = !0
         }
         static now() {
-            return new pl({})
+            return new dl({})
         }
         static local() {
-            const [e, t] = hl(arguments), [r, n, i, o, s, a, l] = t;
-            return cl({
+            const [e, t] = pl(arguments), [r, n, i, o, s, a, l] = t;
+            return fl({
                 year: r,
                 month: n,
                 day: i,
                 hour: o,
                 minute: s,
                 second: a,
                 millisecond: l
             }, e)
         }
         static utc() {
-            const [e, t] = hl(arguments), [r, n, i, o, s, a, l] = t;
-            return e.zone = ho.utcInstance, cl({
+            const [e, t] = pl(arguments), [r, n, i, o, s, a, l] = t;
+            return e.zone = po.utcInstance, fl({
                 year: r,
                 month: n,
                 day: i,
                 hour: o,
                 minute: s,
                 second: a,
                 millisecond: l
             }, e)
         }
         static fromJSDate(e, t = {}) {
             const r = (n = e, "[object Date]" === Object.prototype.toString.call(n) ? e.valueOf() : NaN);
             var n;
-            if (Number.isNaN(r)) return pl.invalid("invalid input");
-            const i = mo(t.zone, xo.defaultZone);
-            return i.isValid ? new pl({
+            if (Number.isNaN(r)) return dl.invalid("invalid input");
+            const i = go(t.zone, Ao.defaultZone);
+            return i.isValid ? new dl({
                 ts: r,
                 zone: i,
-                loc: co.fromObject(t)
-            }) : pl.invalid(Wa(i))
+                loc: fo.fromObject(t)
+            }) : dl.invalid(Ga(i))
         }
         static fromMillis(e, t = {}) {
-            if (qo(e)) return e < -Ha || e > Ha ? pl.invalid("Timestamp out of range") : new pl({
+            if (Eo(e)) return e < -Wa || e > Wa ? dl.invalid("Timestamp out of range") : new dl({
                 ts: e,
-                zone: mo(t.zone, xo.defaultZone),
-                loc: co.fromObject(t)
+                zone: go(t.zone, Ao.defaultZone),
+                loc: fo.fromObject(t)
             });
-            throw new wi(`fromMillis requires a numerical input, but received a ${typeof e} with value ${e}`)
+            throw new _i(`fromMillis requires a numerical input, but received a ${typeof e} with value ${e}`)
         }
         static fromSeconds(e, t = {}) {
-            if (qo(e)) return new pl({
+            if (Eo(e)) return new dl({
                 ts: 1e3 * e,
-                zone: mo(t.zone, xo.defaultZone),
-                loc: co.fromObject(t)
+                zone: go(t.zone, Ao.defaultZone),
+                loc: fo.fromObject(t)
             });
-            throw new wi("fromSeconds requires a numerical input")
+            throw new _i("fromSeconds requires a numerical input")
         }
         static fromObject(e, t = {}) {
             e = e || {};
-            const r = mo(t.zone, xo.defaultZone);
-            if (!r.isValid) return pl.invalid(Wa(r));
-            const n = xo.now(),
-                i = Ao(t.specificOffset) ? r.offset(n) : t.specificOffset,
-                o = Ho(e, ul),
-                s = !Ao(o.ordinal),
-                a = !Ao(o.year),
-                l = !Ao(o.month) || !Ao(o.day),
+            const r = go(t.zone, Ao.defaultZone);
+            if (!r.isValid) return dl.invalid(Ga(r));
+            const n = Ao.now(),
+                i = qo(t.specificOffset) ? r.offset(n) : t.specificOffset,
+                o = Wo(e, cl),
+                s = !qo(o.ordinal),
+                a = !qo(o.year),
+                l = !qo(o.month) || !qo(o.day),
                 u = a || l,
                 c = o.weekYear || o.weekNumber,
-                f = co.fromObject(t);
-            if ((u || s) && c) throw new yi("Can't mix weekYear/weekNumber units with year/month/day or ordinals");
-            if (l && s) throw new yi("Can't mix ordinal dates with month/day");
+                f = fo.fromObject(t);
+            if ((u || s) && c) throw new bi("Can't mix weekYear/weekNumber units with year/month/day or ordinals");
+            if (l && s) throw new bi("Can't mix ordinal dates with month/day");
             const h = c || o.weekday && !u;
-            let p, d, m = Ya(n, i);
-            h ? (p = al, d = il, m = Ma(m)) : s ? (p = ll, d = ol, m = ja(m)) : (p = sl, d = nl);
+            let p, d, m = Ka(n, i);
+            h ? (p = ll, d = ol, m = Pa(m)) : s ? (p = ul, d = sl, m = Ba(m)) : (p = al, d = il);
             let g = !1;
             for (const e of p) {
-                Ao(o[e]) ? o[e] = g ? d[e] : m[e] : g = !0
+                qo(o[e]) ? o[e] = g ? d[e] : m[e] : g = !0
             }
             const v = h ? function(e) {
-                    const t = Eo(e.weekYear),
-                        r = So(e.weekNumber, 1, jo(e.weekYear)),
-                        n = So(e.weekday, 1, 7);
-                    return t ? r ? !n && La("weekday", e.weekday) : La("week", e.week) : La("weekYear", e.weekYear)
+                    const t = To(e.weekYear),
+                        r = Do(e.weekNumber, 1, Bo(e.weekYear)),
+                        n = Do(e.weekday, 1, 7);
+                    return t ? r ? !n && Na("weekday", e.weekday) : Na("week", e.week) : Na("weekYear", e.weekYear)
                 }(o) : s ? function(e) {
-                    const t = Eo(e.year),
-                        r = So(e.ordinal, 1, Fo(e.year));
-                    return t ? !r && La("ordinal", e.ordinal) : La("year", e.year)
-                }(o) : Ua(o),
-                y = v || Va(o);
-            if (y) return pl.invalid(y);
-            const b = h ? Pa(o) : s ? Ba(o) : o,
-                [w, _] = Ka(b, i, r),
-                k = new pl({
+                    const t = To(e.year),
+                        r = Do(e.ordinal, 1, Mo(e.year));
+                    return t ? !r && Na("ordinal", e.ordinal) : Na("year", e.year)
+                }(o) : Va(o),
+                y = v || za(o);
+            if (y) return dl.invalid(y);
+            const b = h ? ja(o) : s ? Ua(o) : o,
+                [w, _] = Xa(b, i, r),
+                k = new dl({
                     ts: w,
                     zone: r,
                     o: _,
                     loc: f
                 });
-            return o.weekday && u && e.weekday !== k.weekday ? pl.invalid("mismatched weekday", `you can't specify both a weekday of ${o.weekday} and a date of ${k.toISO()}`) : k
+            return o.weekday && u && e.weekday !== k.weekday ? dl.invalid("mismatched weekday", `you can't specify both a weekday of ${o.weekday} and a date of ${k.toISO()}`) : k
         }
         static fromISO(e, t = {}) {
             const [r, n] = function(e) {
-                return ds(e, [js, zs], [Bs, Hs], [Us, Ws], [Vs, Gs])
+                return ms(e, [Bs, Hs], [Us, Ws], [Vs, Gs], [zs, Zs])
             }(e);
-            return Qa(r, n, t, "ISO 8601", e)
+            return el(r, n, t, "ISO 8601", e)
         }
         static fromRFC2822(e, t = {}) {
             const [r, n] = function(e) {
-                return ds(function(e) {
+                return ms(function(e) {
                     return e.replace(/\([^()]*\)|[\n\t]/g, " ").replace(/(\s\s+)/g, " ").trim()
-                }(e), [Rs, Ls])
+                }(e), [Ls, Ns])
             }(e);
-            return Qa(r, n, t, "RFC 2822", e)
+            return el(r, n, t, "RFC 2822", e)
         }
         static fromHTTP(e, t = {}) {
             const [r, n] = function(e) {
-                return ds(e, [Ns, Ms], [Is, Ms], [Fs, Ps])
+                return ms(e, [Is, Ps], [Fs, Ps], [Ms, js])
             }(e);
-            return Qa(r, n, t, "HTTP", t)
+            return el(r, n, t, "HTTP", t)
         }
         static fromFormat(e, t, r = {}) {
-            if (Ao(e) || Ao(t)) throw new wi("fromFormat requires an input string and a format");
+            if (qo(e) || qo(t)) throw new _i("fromFormat requires an input string and a format");
             const {
                 locale: n = null,
                 numberingSystem: i = null
-            } = r, o = co.fromOpts({
+            } = r, o = fo.fromOpts({
                 locale: n,
                 numberingSystem: i,
                 defaultToEN: !0
             }), [s, a, l, u] = function(e, t, r) {
                 const {
                     result: n,
                     zone: i,
                     specificOffset: o,
                     invalidReason: s
-                } = Sa(e, t, r);
+                } = Da(e, t, r);
                 return [n, i, o, s]
             }(o, e, t);
-            return u ? pl.invalid(u) : Qa(s, a, r, `format ${t}`, e, l)
+            return u ? dl.invalid(u) : el(s, a, r, `format ${t}`, e, l)
         }
         static fromString(e, t, r = {}) {
-            return pl.fromFormat(e, t, r)
+            return dl.fromFormat(e, t, r)
         }
         static fromSQL(e, t = {}) {
             const [r, n] = function(e) {
-                return ds(e, [Js, zs], [Ys, Ks])
+                return ms(e, [Ys, Hs], [Ks, Xs])
             }(e);
-            return Qa(r, n, t, "SQL", e)
+            return el(r, n, t, "SQL", e)
         }
         static invalid(e, t = null) {
-            if (!e) throw new wi("need to specify a reason the DateTime is invalid");
-            const r = e instanceof cs ? e : new cs(e, t);
-            if (xo.throwOnInvalid) throw new mi(r);
-            return new pl({
+            if (!e) throw new _i("need to specify a reason the DateTime is invalid");
+            const r = e instanceof fs ? e : new fs(e, t);
+            if (Ao.throwOnInvalid) throw new gi(r);
+            return new dl({
                 invalid: r
             })
         }
         static isDateTime(e) {
             return e && e.isLuxonDateTime || !1
         }
         static parseFormatForOpts(e, t = {}) {
-            const r = Da(e, co.fromObject(t));
+            const r = Ca(e, fo.fromObject(t));
             return r ? r.map((e => e ? e.val : null)).join("") : null
         }
         static expandFormat(e, t = {}) {
-            return Oa(us.parseFormat(e), co.fromObject(t)).map((e => e.val)).join("")
+            return Sa(cs.parseFormat(e), fo.fromObject(t)).map((e => e.val)).join("")
         }
         get(e) {
             return this[e]
         }
         get isValid() {
             return null === this.invalid
         }
@@ -10870,42 +10890,42 @@
         get second() {
             return this.isValid ? this.c.second : NaN
         }
         get millisecond() {
             return this.isValid ? this.c.millisecond : NaN
         }
         get weekYear() {
-            return this.isValid ? Ga(this).weekYear : NaN
+            return this.isValid ? Za(this).weekYear : NaN
         }
         get weekNumber() {
-            return this.isValid ? Ga(this).weekNumber : NaN
+            return this.isValid ? Za(this).weekNumber : NaN
         }
         get weekday() {
-            return this.isValid ? Ga(this).weekday : NaN
+            return this.isValid ? Za(this).weekday : NaN
         }
         get ordinal() {
-            return this.isValid ? ja(this.c).ordinal : NaN
+            return this.isValid ? Ba(this.c).ordinal : NaN
         }
         get monthShort() {
-            return this.isValid ? ca.months("short", {
+            return this.isValid ? fa.months("short", {
                 locObj: this.loc
             })[this.month - 1] : null
         }
         get monthLong() {
-            return this.isValid ? ca.months("long", {
+            return this.isValid ? fa.months("long", {
                 locObj: this.loc
             })[this.month - 1] : null
         }
         get weekdayShort() {
-            return this.isValid ? ca.weekdays("short", {
+            return this.isValid ? fa.weekdays("short", {
                 locObj: this.loc
             })[this.weekday - 1] : null
         }
         get weekdayLong() {
-            return this.isValid ? ca.weekdays("long", {
+            return this.isValid ? fa.weekdays("long", {
                 locObj: this.loc
             })[this.weekday - 1] : null
         }
         get offset() {
             return this.isValid ? +this.o : NaN
         }
         get offsetNameShort() {
@@ -10928,120 +10948,120 @@
                 month: 1,
                 day: 1
             }).offset || this.offset > this.set({
                 month: 5
             }).offset)
         }
         get isInLeapYear() {
-            return Io(this.year)
+            return Fo(this.year)
         }
         get daysInMonth() {
-            return Mo(this.year, this.month)
+            return Po(this.year, this.month)
         }
         get daysInYear() {
-            return this.isValid ? Fo(this.year) : NaN
+            return this.isValid ? Mo(this.year) : NaN
         }
         get weeksInWeekYear() {
-            return this.isValid ? jo(this.weekYear) : NaN
+            return this.isValid ? Bo(this.weekYear) : NaN
         }
         resolvedLocaleOptions(e = {}) {
             const {
                 locale: t,
                 numberingSystem: r,
                 calendar: n
-            } = us.create(this.loc.clone(e), e).resolvedOptions(this);
+            } = cs.create(this.loc.clone(e), e).resolvedOptions(this);
             return {
                 locale: t,
                 numberingSystem: r,
                 outputCalendar: n
             }
         }
         toUTC(e = 0, t = {}) {
-            return this.setZone(ho.instance(e), t)
+            return this.setZone(po.instance(e), t)
         }
         toLocal() {
-            return this.setZone(xo.defaultZone)
+            return this.setZone(Ao.defaultZone)
         }
         setZone(e, {
             keepLocalTime: t = !1,
             keepCalendarTime: r = !1
         } = {}) {
-            if ((e = mo(e, xo.defaultZone)).equals(this.zone)) return this;
+            if ((e = go(e, Ao.defaultZone)).equals(this.zone)) return this;
             if (e.isValid) {
                 let n = this.ts;
                 if (t || r) {
                     const t = e.offset(this.ts),
                         r = this.toObject();
-                    [n] = Ka(r, t, e)
+                    [n] = Xa(r, t, e)
                 }
-                return Za(this, {
+                return Ja(this, {
                     ts: n,
                     zone: e
                 })
             }
-            return pl.invalid(Wa(e))
+            return dl.invalid(Ga(e))
         }
         reconfigure({
             locale: e,
             numberingSystem: t,
             outputCalendar: r
         } = {}) {
-            return Za(this, {
+            return Ja(this, {
                 loc: this.loc.clone({
                     locale: e,
                     numberingSystem: t,
                     outputCalendar: r
                 })
             })
         }
         setLocale(e) {
             return this.reconfigure({
                 locale: e
             })
         }
         set(e) {
             if (!this.isValid) return this;
-            const t = Ho(e, ul),
-                r = !Ao(t.weekYear) || !Ao(t.weekNumber) || !Ao(t.weekday),
-                n = !Ao(t.ordinal),
-                i = !Ao(t.year),
-                o = !Ao(t.month) || !Ao(t.day),
+            const t = Wo(e, cl),
+                r = !qo(t.weekYear) || !qo(t.weekNumber) || !qo(t.weekday),
+                n = !qo(t.ordinal),
+                i = !qo(t.year),
+                o = !qo(t.month) || !qo(t.day),
                 s = i || o,
                 a = t.weekYear || t.weekNumber;
-            if ((s || n) && a) throw new yi("Can't mix weekYear/weekNumber units with year/month/day or ordinals");
-            if (o && n) throw new yi("Can't mix ordinal dates with month/day");
+            if ((s || n) && a) throw new bi("Can't mix weekYear/weekNumber units with year/month/day or ordinals");
+            if (o && n) throw new bi("Can't mix ordinal dates with month/day");
             let l;
-            r ? l = Pa({
-                ...Ma(this.c),
+            r ? l = ja({
+                ...Pa(this.c),
                 ...t
-            }) : Ao(t.ordinal) ? (l = {
+            }) : qo(t.ordinal) ? (l = {
                 ...this.toObject(),
                 ...t
-            }, Ao(t.day) && (l.day = Math.min(Mo(l.year, l.month), l.day))) : l = Ba({
-                ...ja(this.c),
+            }, qo(t.day) && (l.day = Math.min(Po(l.year, l.month), l.day))) : l = Ua({
+                ...Ba(this.c),
                 ...t
             });
-            const [u, c] = Ka(l, this.o, this.zone);
-            return Za(this, {
+            const [u, c] = Xa(l, this.o, this.zone);
+            return Ja(this, {
                 ts: u,
                 o: c
             })
         }
         plus(e) {
             if (!this.isValid) return this;
-            return Za(this, Xa(this, aa.fromDurationLike(e)))
+            return Ja(this, Qa(this, la.fromDurationLike(e)))
         }
         minus(e) {
             if (!this.isValid) return this;
-            return Za(this, Xa(this, aa.fromDurationLike(e).negate()))
+            return Ja(this, Qa(this, la.fromDurationLike(e).negate()))
         }
         startOf(e) {
             if (!this.isValid) return this;
             const t = {},
-                r = aa.normalizeUnit(e);
+                r = la.normalizeUnit(e);
             switch (r) {
                 case "years":
                     t.month = 1;
                 case "quarters":
                 case "months":
                     t.day = 1;
                 case "weeks":
@@ -11062,75 +11082,75 @@
         }
         endOf(e) {
             return this.isValid ? this.plus({
                 [e]: 1
             }).startOf(e).minus(1) : this
         }
         toFormat(e, t = {}) {
-            return this.isValid ? us.create(this.loc.redefaultToEN(t)).formatDateTimeFromString(this, e) : za
+            return this.isValid ? cs.create(this.loc.redefaultToEN(t)).formatDateTimeFromString(this, e) : Ha
         }
-        toLocaleString(e = qi, t = {}) {
-            return this.isValid ? us.create(this.loc.clone(t), e).formatDateTime(this) : za
+        toLocaleString(e = Ei, t = {}) {
+            return this.isValid ? cs.create(this.loc.clone(t), e).formatDateTime(this) : Ha
         }
         toLocaleParts(e = {}) {
-            return this.isValid ? us.create(this.loc.clone(e), e).formatDateTimeParts(this) : []
+            return this.isValid ? cs.create(this.loc.clone(e), e).formatDateTimeParts(this) : []
         }
         toISO({
             format: e = "extended",
             suppressSeconds: t = !1,
             suppressMilliseconds: r = !1,
             includeOffset: n = !0,
             extendedZone: i = !1
         } = {}) {
             if (!this.isValid) return null;
             const o = "extended" === e;
-            let s = tl(this, o);
-            return s += "T", s += rl(this, o, t, r, n, i), s
+            let s = rl(this, o);
+            return s += "T", s += nl(this, o, t, r, n, i), s
         }
         toISODate({
             format: e = "extended"
         } = {}) {
-            return this.isValid ? tl(this, "extended" === e) : null
+            return this.isValid ? rl(this, "extended" === e) : null
         }
         toISOWeekDate() {
-            return el(this, "kkkk-'W'WW-c")
+            return tl(this, "kkkk-'W'WW-c")
         }
         toISOTime({
             suppressMilliseconds: e = !1,
             suppressSeconds: t = !1,
             includeOffset: r = !0,
             includePrefix: n = !1,
             extendedZone: i = !1,
             format: o = "extended"
         } = {}) {
             if (!this.isValid) return null;
-            return (n ? "T" : "") + rl(this, "extended" === o, t, e, r, i)
+            return (n ? "T" : "") + nl(this, "extended" === o, t, e, r, i)
         }
         toRFC2822() {
-            return el(this, "EEE, dd LLL yyyy HH:mm:ss ZZZ", !1)
+            return tl(this, "EEE, dd LLL yyyy HH:mm:ss ZZZ", !1)
         }
         toHTTP() {
-            return el(this.toUTC(), "EEE, dd LLL yyyy HH:mm:ss 'GMT'")
+            return tl(this.toUTC(), "EEE, dd LLL yyyy HH:mm:ss 'GMT'")
         }
         toSQLDate() {
-            return this.isValid ? tl(this, !0) : null
+            return this.isValid ? rl(this, !0) : null
         }
         toSQLTime({
             includeOffset: e = !0,
             includeZone: t = !1,
             includeOffsetSpace: r = !0
         } = {}) {
             let n = "HH:mm:ss.SSS";
-            return (t || e) && (r && (n += " "), t ? n += "z" : e && (n += "ZZ")), el(this, n, !0)
+            return (t || e) && (r && (n += " "), t ? n += "z" : e && (n += "ZZ")), tl(this, n, !0)
         }
         toSQL(e = {}) {
             return this.isValid ? `${this.toSQLDate()} ${this.toSQLTime(e)}` : null
         }
         toString() {
-            return this.isValid ? this.toISO() : za
+            return this.isValid ? this.toISO() : Ha
         }
         valueOf() {
             return this.toMillis()
         }
         toMillis() {
             return this.isValid ? this.ts : NaN
         }
@@ -11153,505 +11173,505 @@
             };
             return e.includeConfig && (t.outputCalendar = this.outputCalendar, t.numberingSystem = this.loc.numberingSystem, t.locale = this.loc.locale), t
         }
         toJSDate() {
             return new Date(this.isValid ? this.ts : NaN)
         }
         diff(e, t = "milliseconds", r = {}) {
-            if (!this.isValid || !e.isValid) return aa.invalid("created by diffing an invalid DateTime");
+            if (!this.isValid || !e.isValid) return la.invalid("created by diffing an invalid DateTime");
             const n = {
                     locale: this.locale,
                     numberingSystem: this.numberingSystem,
                     ...r
                 },
-                i = (a = t, Array.isArray(a) ? a : [a]).map(aa.normalizeUnit),
+                i = (a = t, Array.isArray(a) ? a : [a]).map(la.normalizeUnit),
                 o = e.valueOf() > this.valueOf(),
-                s = ha(o ? this : e, o ? e : this, i, n);
+                s = pa(o ? this : e, o ? e : this, i, n);
             var a;
             return o ? s.negate() : s
         }
         diffNow(e = "milliseconds", t = {}) {
-            return this.diff(pl.now(), e, t)
+            return this.diff(dl.now(), e, t)
         }
         until(e) {
-            return this.isValid ? ua.fromDateTimes(this, e) : this
+            return this.isValid ? ca.fromDateTimes(this, e) : this
         }
         hasSame(e, t) {
             if (!this.isValid) return !1;
             const r = e.valueOf(),
                 n = this.setZone(e.zone, {
                     keepLocalTime: !0
                 });
             return n.startOf(t) <= r && r <= n.endOf(t)
         }
         equals(e) {
             return this.isValid && e.isValid && this.valueOf() === e.valueOf() && this.zone.equals(e.zone) && this.loc.equals(e.loc)
         }
         toRelative(e = {}) {
             if (!this.isValid) return null;
-            const t = e.base || pl.fromObject({}, {
+            const t = e.base || dl.fromObject({}, {
                     zone: this.zone
                 }),
                 r = e.padding ? this < t ? -e.padding : e.padding : 0;
             let n = ["years", "months", "days", "hours", "minutes", "seconds"],
                 i = e.unit;
-            return Array.isArray(e.unit) && (n = e.unit, i = void 0), fl(t, this.plus(r), {
+            return Array.isArray(e.unit) && (n = e.unit, i = void 0), hl(t, this.plus(r), {
                 ...e,
                 numeric: "always",
                 units: n,
                 unit: i
             })
         }
         toRelativeCalendar(e = {}) {
-            return this.isValid ? fl(e.base || pl.fromObject({}, {
+            return this.isValid ? hl(e.base || dl.fromObject({}, {
                 zone: this.zone
             }), this, {
                 ...e,
                 numeric: "auto",
                 units: ["years", "months", "days"],
                 calendary: !0
             }) : null
         }
         static min(...e) {
-            if (!e.every(pl.isDateTime)) throw new wi("min requires all arguments be DateTimes");
-            return $o(e, (e => e.valueOf()), Math.min)
+            if (!e.every(dl.isDateTime)) throw new _i("min requires all arguments be DateTimes");
+            return Oo(e, (e => e.valueOf()), Math.min)
         }
         static max(...e) {
-            if (!e.every(pl.isDateTime)) throw new wi("max requires all arguments be DateTimes");
-            return $o(e, (e => e.valueOf()), Math.max)
+            if (!e.every(dl.isDateTime)) throw new _i("max requires all arguments be DateTimes");
+            return Oo(e, (e => e.valueOf()), Math.max)
         }
         static fromFormatExplain(e, t, r = {}) {
             const {
                 locale: n = null,
                 numberingSystem: i = null
             } = r;
-            return Sa(co.fromOpts({
+            return Da(fo.fromOpts({
                 locale: n,
                 numberingSystem: i,
                 defaultToEN: !0
             }), e, t)
         }
         static fromStringExplain(e, t, r = {}) {
-            return pl.fromFormatExplain(e, t, r)
+            return dl.fromFormatExplain(e, t, r)
         }
         static get DATE_SHORT() {
-            return qi
+            return Ei
         }
         static get DATE_MED() {
-            return Ei
+            return Ti
         }
         static get DATE_MED_WITH_WEEKDAY() {
-            return Ti
+            return $i
         }
         static get DATE_FULL() {
-            return $i
+            return Oi
         }
         static get DATE_HUGE() {
-            return Oi
+            return Si
         }
         static get TIME_SIMPLE() {
-            return Si
+            return Di
         }
         static get TIME_WITH_SECONDS() {
-            return Di
+            return Ci
         }
         static get TIME_WITH_SHORT_OFFSET() {
-            return Ci
+            return Ri
         }
         static get TIME_WITH_LONG_OFFSET() {
-            return Ri
+            return Li
         }
         static get TIME_24_SIMPLE() {
-            return Li
+            return Ni
         }
         static get TIME_24_WITH_SECONDS() {
-            return Ni
+            return Ii
         }
         static get TIME_24_WITH_SHORT_OFFSET() {
-            return Ii
+            return Fi
         }
         static get TIME_24_WITH_LONG_OFFSET() {
-            return Fi
+            return Mi
         }
         static get DATETIME_SHORT() {
-            return Mi
+            return Pi
         }
         static get DATETIME_SHORT_WITH_SECONDS() {
-            return Pi
+            return ji
         }
         static get DATETIME_MED() {
-            return ji
+            return Bi
         }
         static get DATETIME_MED_WITH_SECONDS() {
-            return Bi
+            return Ui
         }
         static get DATETIME_MED_WITH_WEEKDAY() {
-            return Ui
+            return Vi
         }
         static get DATETIME_FULL() {
-            return Vi
+            return zi
         }
         static get DATETIME_FULL_WITH_SECONDS() {
-            return zi
+            return Hi
         }
         static get DATETIME_HUGE() {
-            return Hi
+            return Wi
         }
         static get DATETIME_HUGE_WITH_SECONDS() {
-            return Wi
+            return Gi
         }
     }
 
-    function dl(e) {
-        if (pl.isDateTime(e)) return e;
-        if (e && e.valueOf && qo(e.valueOf())) return pl.fromJSDate(e);
-        if (e && "object" == typeof e) return pl.fromObject(e);
-        throw new wi(`Unknown datetime argument: ${e}, of type ${typeof e}`)
+    function ml(e) {
+        if (dl.isDateTime(e)) return e;
+        if (e && e.valueOf && Eo(e.valueOf())) return dl.fromJSDate(e);
+        if (e && "object" == typeof e) return dl.fromObject(e);
+        throw new _i(`Unknown datetime argument: ${e}, of type ${typeof e}`)
     }
 
-    function ml(e, t, r) {
+    function gl(e, t, r) {
         const n = e.slice();
         return n[17] = t[r][0], n[18] = t[r][1], n[19] = t, n[20] = r, n
     }
 
-    function gl(e, t, r) {
+    function vl(e, t, r) {
         const n = e.slice();
         return n[21] = t[r].date, n[18] = t[r].label, n[22] = t[r].flavour, n
     }
 
-    function vl(e, t, r) {
+    function yl(e, t, r) {
         const n = e.slice();
         return n[25] = t[r][0], n[26] = t[r][1].name, n
     }
 
-    function yl(e) {
+    function bl(e) {
         let t, r, n, i = e[26] + "";
         return {
             c() {
-                t = D("option"), r = R(i), t.__value = n = e[25], t.value = t.__value
+                t = C("option"), r = L(i), t.__value = n = e[25], z(t, t.__value)
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, o) {
-                4 & o && i !== (i = e[26] + "") && U(r, i), 4 & o && n !== (n = e[25]) && (t.__value = n, t.value = t.__value)
+                4 & o && i !== (i = e[26] + "") && V(r, i), 4 & o && n !== (n = e[25]) && (t.__value = n, z(t, t.__value))
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function bl(e) {
-        let t, r, n, i, o, s, a = e[18] + "";
+    function wl(e) {
+        let t, r, n, i, o;
 
-        function l() {
+        function s() {
             return e[11](e[21])
         }
         return {
             c() {
-                t = D("li"), r = D("button"), n = R(a), i = L(), P(r, "type", "button"), P(r, "class", "svelte-1074j9"), J(t, "disabled", e[0].fromAlias)
+                t = C("li"), r = C("button"), r.textContent = `${e[18]}`, n = N(), j(r, "type", "button"), j(r, "class", "svelte-1074j9"), Y(t, "disabled", e[0].fromAlias)
             },
             m(e, a) {
-                $(e, t, a), q(t, r), q(r, n), q(t, i), o || (s = I(r, "click", l), o = !0)
+                O(e, t, a), E(t, r), E(t, n), i || (o = F(r, "click", s), i = !0)
             },
             p(r, n) {
-                e = r, 1 & n && J(t, "disabled", e[0].fromAlias)
+                e = r, 1 & n && Y(t, "disabled", e[0].fromAlias)
             },
             d(e) {
-                e && O(t), o = !1, s()
+                e && S(t), i = !1, o()
             }
         }
     }
 
-    function wl(e) {
-        let t, r = (!e[22] || e[1] === e[22]) && bl(e);
+    function _l(e) {
+        let t, r = (!e[22] || e[1] === e[22]) && wl(e);
         return {
             c() {
-                r && r.c(), t = N()
+                r && r.c(), t = I()
             },
             m(e, n) {
-                r && r.m(e, n), $(e, t, n)
+                r && r.m(e, n), O(e, t, n)
             },
             p(e, n) {
-                e[22] && e[1] !== e[22] ? r && (r.d(1), r = null) : r ? r.p(e, n) : (r = bl(e), r.c(), r.m(t.parentNode, t))
+                e[22] && e[1] !== e[22] ? r && (r.d(1), r = null) : r ? r.p(e, n) : (r = wl(e), r.c(), r.m(t.parentNode, t))
             },
             d(e) {
-                r && r.d(e), e && O(t)
+                e && S(t), r && r.d(e)
             }
         }
     }
 
-    function _l(e) {
+    function kl(e) {
         let t, r, n, i, o, s, a, l, u = e[18] + "";
 
         function c() {
             e[12].call(s, e[17])
         }
         return {
             c() {
-                t = D("label"), r = R(u), n = R(":"), i = L(), o = D("div"), s = D("input"), P(t, "class", "control svelte-1074j9"), P(t, "for", "__" + e[17] + "-control"), P(s, "id", "__" + e[17] + "-control"), P(s, "type", "checkbox"), s.disabled = e[3], P(o, "class", "form-control checkbox-container svelte-1074j9")
+                t = C("label"), r = L(u), n = L(":"), i = N(), o = C("div"), s = C("input"), j(t, "class", "control svelte-1074j9"), j(t, "for", "__" + e[17] + "-control"), j(s, "id", "__" + e[17] + "-control"), j(s, "type", "checkbox"), s.disabled = e[3], j(o, "class", "form-control checkbox-container svelte-1074j9")
             },
             m(u, f) {
-                $(u, t, f), q(t, r), q(t, n), $(u, i, f), $(u, o, f), q(o, s), s.checked = e[0].strategies[e[17]], a || (l = I(s, "change", c), a = !0)
+                O(u, t, f), E(t, r), E(t, n), O(u, i, f), O(u, o, f), E(o, s), s.checked = e[0].strategies[e[17]], a || (l = F(s, "change", c), a = !0)
             },
             p(t, r) {
                 e = t, 8 & r && (s.disabled = e[3]), 17 & r && (s.checked = e[0].strategies[e[17]])
             },
             d(e) {
-                e && O(t), e && O(i), e && O(o), a = !1, l()
+                e && (S(t), S(i), S(o)), a = !1, l()
             }
         }
     }
 
-    function kl(t) {
-        let r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, E, T, C, R, N, M, j, B, U = Object.entries(t[2]),
-            W = [];
-        for (let e = 0; e < U.length; e += 1) W[e] = yl(vl(t, U, e));
-        let G = t[5],
+    function xl(t) {
+        let r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, q, T, $, R, L, I, P, B, U = Fe(Object.entries(t[2])),
+            V = [];
+        for (let e = 0; e < U.length; e += 1) V[e] = bl(yl(t, U, e));
+        let G = Fe(t[5]),
             Z = [];
-        for (let e = 0; e < G.length; e += 1) Z[e] = wl(gl(t, G, e));
-        let J = t[4],
+        for (let e = 0; e < G.length; e += 1) Z[e] = _l(vl(t, G, e));
+        let J = Fe(t[4]),
             Y = [];
-        for (let e = 0; e < J.length; e += 1) Y[e] = _l(ml(t, J, e));
+        for (let e = 0; e < J.length; e += 1) Y[e] = kl(gl(t, J, e));
         return {
             c() {
-                r = D("form"), n = D("div"), i = D("label"), i.textContent = "results:", s = L(), a = D("select"), l = D("option"), l.textContent = "20", u = D("option"), u.textContent = "50", c = D("option"), c.textContent = "100", h = L(), p = D("label"), p.textContent = "sources:", d = L(), m = D("select");
-                for (let e = 0; e < W.length; e += 1) W[e].c();
-                v = L(), y = D("label"), y.textContent = "updated on/after:", b = L(), w = D("input"), k = L(), x = D("ul");
+                r = C("form"), n = C("div"), i = C("label"), i.textContent = "results:", s = N(), a = C("select"), l = C("option"), l.textContent = "20", u = C("option"), u.textContent = "50", c = C("option"), c.textContent = "100", h = N(), p = C("label"), p.textContent = "sources:", d = N(), m = C("select");
+                for (let e = 0; e < V.length; e += 1) V[e].c();
+                v = N(), y = C("label"), y.textContent = "updated on/after:", b = N(), w = C("input"), k = N(), x = C("ul");
                 for (let e = 0; e < Z.length; e += 1) Z[e].c();
-                A = L();
+                A = N();
                 for (let e = 0; e < Y.length; e += 1) Y[e].c();
-                E = L(), T = D("label"), T.textContent = "version:", C = L(), R = D("input"), N = L(), M = D("div"), M.innerHTML = '<button class="form-control svelte-1074j9" type="submit">search</button> \n    <button class="form-control svelte-1074j9" type="reset">reset</button>', P(i, "for", "__search-limit"), P(i, "class", "svelte-1074j9"), l.__value = 20, l.value = l.__value, u.__value = 50, u.value = u.__value, c.__value = 100, c.value = c.__value, P(a, "id", "__search-limit"), P(a, "class", "form-control"), a.disabled = f = t[0].fromAlias, void 0 === t[0].limit && ge((() => t[8].call(a))), P(p, "for", "__search-source"), P(p, "class", "svelte-1074j9"), P(m, "id", "__search-source"), P(m, "class", "form-control"), m.multiple = !0, m.disabled = g = t[0].fromAlias, void 0 === t[0].sources && ge((() => t[9].call(m))), P(y, "for", "__search-start-date"), P(y, "class", "svelte-1074j9"), P(w, "type", "text"), P(w, "id", "__search-start-date"), P(w, "class", "form-control"), P(w, "placeholder", "YYYY-MM-DD"), w.disabled = _ = t[0].fromAlias, P(x, "class", "start-date-suggestions svelte-1074j9"), P(T, "class", "control svelte-1074j9"), P(T, "for", "__version-control"), P(R, "id", "__version-control"), P(R, "type", "text"), P(R, "class", "form-control"), P(R, "placeholder", "version"), P(R, "aria-label", "version"), R.disabled = t[3], P(n, "class", "row form-grid svelte-1074j9"), P(M, "class", "row input-array"), P(r, "class", "content svelte-1074j9")
+                q = N(), T = C("label"), T.textContent = "version:", $ = N(), R = C("input"), L = N(), I = C("div"), I.innerHTML = '<button class="form-control svelte-1074j9" type="submit">search</button> <button class="form-control svelte-1074j9" type="reset">reset</button>', j(i, "for", "__search-limit"), j(i, "class", "svelte-1074j9"), l.__value = 20, z(l, l.__value), u.__value = 50, z(u, u.__value), c.__value = 100, z(c, c.__value), j(a, "id", "__search-limit"), j(a, "class", "form-control"), a.disabled = f = t[0].fromAlias, void 0 === t[0].limit && ve((() => t[8].call(a))), j(p, "for", "__search-source"), j(p, "class", "svelte-1074j9"), j(m, "id", "__search-source"), j(m, "class", "form-control"), m.multiple = !0, m.disabled = g = t[0].fromAlias, void 0 === t[0].sources && ve((() => t[9].call(m))), j(y, "for", "__search-start-date"), j(y, "class", "svelte-1074j9"), j(w, "type", "text"), j(w, "id", "__search-start-date"), j(w, "class", "form-control"), j(w, "placeholder", "YYYY-MM-DD"), w.disabled = _ = t[0].fromAlias, j(x, "class", "start-date-suggestions svelte-1074j9"), j(T, "class", "control svelte-1074j9"), j(T, "for", "__version-control"), j(R, "id", "__version-control"), j(R, "type", "text"), j(R, "class", "form-control"), j(R, "placeholder", "version"), j(R, "aria-label", "version"), R.disabled = t[3], j(n, "class", "row form-grid svelte-1074j9"), j(I, "class", "row input-array"), j(r, "class", "content svelte-1074j9")
             },
             m(e, o) {
-                $(e, r, o), q(r, n), q(n, i), q(n, s), q(n, a), q(a, l), q(a, u), q(a, c), z(a, t[0].limit, !0), q(n, h), q(n, p), q(n, d), q(n, m);
-                for (let e = 0; e < W.length; e += 1) W[e] && W[e].m(m, null);
-                H(m, t[0].sources), q(n, v), q(n, y), q(n, b), q(n, w), V(w, t[0].startDate), q(n, k), q(n, x);
+                O(e, r, o), E(r, n), E(n, i), E(n, s), E(n, a), E(a, l), E(a, u), E(a, c), H(a, t[0].limit, !0), E(n, h), E(n, p), E(n, d), E(n, m);
+                for (let e = 0; e < V.length; e += 1) V[e] && V[e].m(m, null);
+                W(m, t[0].sources), E(n, v), E(n, y), E(n, b), E(n, w), z(w, t[0].startDate), E(n, k), E(n, x);
                 for (let e = 0; e < Z.length; e += 1) Z[e] && Z[e].m(x, null);
-                q(n, A);
+                E(n, A);
                 for (let e = 0; e < Y.length; e += 1) Y[e] && Y[e].m(n, null);
-                q(n, E), q(n, T), q(n, C), q(n, R), V(R, t[0].strategies[Br.VersionEq]), q(r, N), q(r, M), j || (B = [I(a, "change", t[8]), I(m, "change", t[9]), I(w, "input", t[10]), I(R, "input", t[13]), I(r, "submit", F(t[14])), I(r, "reset", t[15])], j = !0)
+                E(n, q), E(n, T), E(n, $), E(n, R), z(R, t[0].strategies[Ur.VersionEq]), E(r, L), E(r, I), P || (B = [F(a, "change", t[8]), F(m, "change", t[9]), F(w, "input", t[10]), F(R, "input", t[13]), F(r, "submit", M(t[14])), F(r, "reset", t[15])], P = !0)
             },
             p(e, [t]) {
-                if (1 & t && f !== (f = e[0].fromAlias) && (a.disabled = f), 1 & t && z(a, e[0].limit), 4 & t) {
+                if (1 & t && f !== (f = e[0].fromAlias) && (a.disabled = f), 1 & t && H(a, e[0].limit), 4 & t) {
                     let r;
-                    for (U = Object.entries(e[2]), r = 0; r < U.length; r += 1) {
-                        const n = vl(e, U, r);
-                        W[r] ? W[r].p(n, t) : (W[r] = yl(n), W[r].c(), W[r].m(m, null))
+                    for (U = Fe(Object.entries(e[2])), r = 0; r < U.length; r += 1) {
+                        const n = yl(e, U, r);
+                        V[r] ? V[r].p(n, t) : (V[r] = bl(n), V[r].c(), V[r].m(m, null))
                     }
-                    for (; r < W.length; r += 1) W[r].d(1);
-                    W.length = U.length
+                    for (; r < V.length; r += 1) V[r].d(1);
+                    V.length = U.length
                 }
-                if (1 & t && g !== (g = e[0].fromAlias) && (m.disabled = g), 1 & t && H(m, e[0].sources), 1 & t && _ !== (_ = e[0].fromAlias) && (w.disabled = _), 1 & t && w.value !== e[0].startDate && V(w, e[0].startDate), 35 & t) {
+                if (1 & t && g !== (g = e[0].fromAlias) && (m.disabled = g), 1 & t && W(m, e[0].sources), 1 & t && _ !== (_ = e[0].fromAlias) && (w.disabled = _), 1 & t && w.value !== e[0].startDate && z(w, e[0].startDate), 35 & t) {
                     let r;
-                    for (G = e[5], r = 0; r < G.length; r += 1) {
-                        const n = gl(e, G, r);
-                        Z[r] ? Z[r].p(n, t) : (Z[r] = wl(n), Z[r].c(), Z[r].m(x, null))
+                    for (G = Fe(e[5]), r = 0; r < G.length; r += 1) {
+                        const n = vl(e, G, r);
+                        Z[r] ? Z[r].p(n, t) : (Z[r] = _l(n), Z[r].c(), Z[r].m(x, null))
                     }
                     for (; r < Z.length; r += 1) Z[r].d(1);
                     Z.length = G.length
                 }
                 if (25 & t) {
                     let r;
-                    for (J = e[4], r = 0; r < J.length; r += 1) {
-                        const i = ml(e, J, r);
-                        Y[r] ? Y[r].p(i, t) : (Y[r] = _l(i), Y[r].c(), Y[r].m(n, E))
+                    for (J = Fe(e[4]), r = 0; r < J.length; r += 1) {
+                        const i = gl(e, J, r);
+                        Y[r] ? Y[r].p(i, t) : (Y[r] = kl(i), Y[r].c(), Y[r].m(n, q))
                     }
                     for (; r < Y.length; r += 1) Y[r].d(1);
                     Y.length = J.length
                 }
-                8 & t && (R.disabled = e[3]), 1 & t && R.value !== e[0].strategies[Br.VersionEq] && V(R, e[0].strategies[Br.VersionEq])
+                8 & t && (R.disabled = e[3]), 1 & t && R.value !== e[0].strategies[Ur.VersionEq] && z(R, e[0].strategies[Ur.VersionEq])
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), S(W, e), S(Z, e), S(Y, e), j = !1, o(B)
+                e && S(r), D(V, e), D(Z, e), D(Y, e), P = !1, o(B)
             }
         }
     }
 
-    function xl(e, t, r) {
+    function Al(e, t, r) {
         let {
             flavour: n,
             sources: i,
             searchFilterInstalled: o,
             searchOptions: s
         } = t;
         const a = [
-                [Br.AnyFlavour, "any flavour"],
-                [Br.AnyReleaseType, "any release type"]
+                [Ur.AnyFlavour, "any flavour"],
+                [Ur.AnyReleaseType, "any release type"]
             ],
             l = [{
                 date: "2022-11-15",
                 label: "10.0.2",
-                flavour: jr.Retail
+                flavour: Br.Retail
             }, {
-                date: pl.now().minus({
+                date: dl.now().minus({
                     days: 1
                 }).toISODate(),
                 label: "yesterday",
                 flavour: null
             }],
-            u = se(),
+            u = ae(),
             {
                 dismiss: c
-            } = le("modal"),
+            } = ue("modal"),
             f = () => {
                 u("requestSearch"), c()
             };
         return e.$$set = e => {
             "flavour" in e && r(1, n = e.flavour), "sources" in e && r(2, i = e.sources), "searchFilterInstalled" in e && r(3, o = e.searchFilterInstalled), "searchOptions" in e && r(0, s = e.searchOptions)
         }, e.$$.update = () => {
             1 & e.$$.dirty && "" === s.startDate && r(0, s.startDate = null, s)
         }, [s, n, i, o, a, l, u, f, function() {
-            s.limit = W(this), r(0, s)
+            s.limit = G(this), r(0, s)
         }, function() {
             var e;
             s.sources = (e = this, [].map.call(e.querySelectorAll(":checked"), (e => e.__value))), r(0, s)
         }, function() {
             s.startDate = this.value, r(0, s)
         }, e => {
             s.fromAlias || r(0, s.startDate = e, s)
         }, function(e) {
             s.strategies[e] = this.checked, r(0, s)
         }, function() {
-            s.strategies[Br.VersionEq] = this.value, r(0, s)
+            s.strategies[Ur.VersionEq] = this.value, r(0, s)
         }, () => f(), () => u("requestReset")]
     }
-    class Al extends Ze {
+    class ql extends Ye {
         constructor(e) {
-            super(), Ge(this, e, xl, kl, a, {
+            super(), Je(this, e, Al, xl, a, {
                 flavour: 1,
                 sources: 2,
                 searchFilterInstalled: 3,
                 searchOptions: 0
             })
         }
     }
 
-    function ql(e, t, r) {
+    function El(e, t, r) {
         const n = e.slice();
         return n[1] = t[r], n
     }
 
-    function El(e) {
+    function Tl(e) {
         let t, r, n, i, o, s, a, l = e[1].version + "",
-            u = pl.fromISO(e[1].install_time).toRelative() + "";
+            u = dl.fromISO(e[1].install_time).toRelative() + "";
         return {
             c() {
-                t = D("option"), r = R(l), n = R("\n        (installed\n        "), i = R(u), o = R(")\n      "), t.__value = s = e[1].version, t.value = t.__value, t.disabled = a = e[0].version === e[1].version
+                t = C("option"), r = L(l), n = L("\n        (installed\n        "), i = L(u), o = L(")\n      "), t.__value = s = e[1].version, z(t, t.__value), t.disabled = a = e[0].version === e[1].version
             },
             m(e, s) {
-                $(e, t, s), q(t, r), q(t, n), q(t, i), q(t, o)
+                O(e, t, s), E(t, r), E(t, n), E(t, i), E(t, o)
             },
             p(e, n) {
-                1 & n && l !== (l = e[1].version + "") && U(r, l), 1 & n && u !== (u = pl.fromISO(e[1].install_time).toRelative() + "") && U(i, u), 1 & n && s !== (s = e[1].version) && (t.__value = s, t.value = t.__value), 1 & n && a !== (a = e[0].version === e[1].version) && (t.disabled = a)
+                1 & n && l !== (l = e[1].version + "") && V(r, l), 1 & n && u !== (u = dl.fromISO(e[1].install_time).toRelative() + "") && V(i, u), 1 & n && s !== (s = e[1].version) && (t.__value = s, z(t, t.__value)), 1 & n && a !== (a = e[0].version === e[1].version) && (t.disabled = a)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function Tl(t) {
-        let r, n, i, s, a, l, u, c, f = t[0].logged_versions,
+    function $l(t) {
+        let r, n, i, s, a, l, u, c, f = Fe(t[0].logged_versions),
             h = [];
-        for (let e = 0; e < f.length; e += 1) h[e] = El(ql(t, f, e));
+        for (let e = 0; e < f.length; e += 1) h[e] = Tl(El(t, f, e));
         return {
             c() {
-                r = D("div"), r.textContent = "rollback", n = L(), i = D("form"), s = D("select");
+                r = C("div"), r.textContent = "rollback", n = N(), i = C("form"), s = C("select");
                 for (let e = 0; e < h.length; e += 1) h[e].c();
-                a = L(), l = D("button"), l.textContent = "rollback", P(r, "class", "title-bar"), P(s, "class", "row form-control"), P(s, "aria-label", "strategy"), void 0 === t[1] && ge((() => t[3].call(s))), P(l, "class", "row form-control"), P(l, "type", "submit"), P(i, "class", "content")
+                a = N(), l = C("button"), l.textContent = "rollback", j(r, "class", "title-bar"), j(s, "class", "row form-control"), j(s, "aria-label", "strategy"), void 0 === t[1] && ve((() => t[3].call(s))), j(l, "class", "row form-control"), j(l, "type", "submit"), j(i, "class", "content")
             },
             m(e, o) {
-                $(e, r, o), $(e, n, o), $(e, i, o), q(i, s);
+                O(e, r, o), O(e, n, o), O(e, i, o), E(i, s);
                 for (let e = 0; e < h.length; e += 1) h[e] && h[e].m(s, null);
-                z(s, t[1], !0), q(i, a), q(i, l), u || (c = [I(s, "change", t[3]), I(i, "submit", F(t[4]))], u = !0)
+                H(s, t[1], !0), E(i, a), E(i, l), u || (c = [F(s, "change", t[3]), F(i, "submit", M(t[4]))], u = !0)
             },
             p(e, [t]) {
                 if (1 & t) {
                     let r;
-                    for (f = e[0].logged_versions, r = 0; r < f.length; r += 1) {
-                        const n = ql(e, f, r);
-                        h[r] ? h[r].p(n, t) : (h[r] = El(n), h[r].c(), h[r].m(s, null))
+                    for (f = Fe(e[0].logged_versions), r = 0; r < f.length; r += 1) {
+                        const n = El(e, f, r);
+                        h[r] ? h[r].p(n, t) : (h[r] = Tl(n), h[r].c(), h[r].m(s, null))
                     }
                     for (; r < h.length; r += 1) h[r].d(1);
                     h.length = f.length
                 }
-                3 & t && z(s, e[1])
+                3 & t && H(s, e[1])
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(n), e && O(i), S(h, e), u = !1, o(c)
+                e && (S(r), S(n), S(i)), D(h, e), u = !1, o(c)
             }
         }
     }
 
-    function $l(e, t, r) {
+    function Ol(e, t, r) {
         let {
             addon: n
         } = t;
-        const i = se(),
+        const i = ae(),
             {
                 dismiss: o
-            } = le("modal");
+            } = ue("modal");
         let s;
         const a = () => {
             i("requestRollback", {
                 ...n,
                 version: s,
                 options: {
                     ...n.options,
                     version_eq: !0
                 }
             }), o()
         };
         return e.$$set = e => {
             "addon" in e && r(0, n = e.addon)
         }, [n, s, a, function() {
-            s = W(this), r(1, s), r(0, n)
+            s = G(this), r(1, s), r(0, n)
         }, () => a()]
     }
-    class Ol extends Ze {
+    class Sl extends Ye {
         constructor(e) {
-            super(), Ge(this, e, $l, Tl, a, {
+            super(), Je(this, e, Ol, $l, a, {
                 addon: 0
             })
         }
     }
-    var Sl = [],
-        Dl = [],
-        Cl = "undefined" != typeof Uint8Array ? Uint8Array : Array,
-        Rl = !1;
+    var Dl = [],
+        Cl = [],
+        Rl = "undefined" != typeof Uint8Array ? Uint8Array : Array,
+        Ll = !1;
 
-    function Ll() {
-        Rl = !0;
-        for (var e = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", t = 0; t < 64; ++t) Sl[t] = e[t], Dl[e.charCodeAt(t)] = t;
-        Dl["-".charCodeAt(0)] = 62, Dl["_".charCodeAt(0)] = 63
+    function Nl() {
+        Ll = !0;
+        for (var e = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", t = 0; t < 64; ++t) Dl[t] = e[t], Cl[e.charCodeAt(t)] = t;
+        Cl["-".charCodeAt(0)] = 62, Cl["_".charCodeAt(0)] = 63
     }
 
-    function Nl(e) {
-        return Sl[e >> 18 & 63] + Sl[e >> 12 & 63] + Sl[e >> 6 & 63] + Sl[63 & e]
+    function Il(e) {
+        return Dl[e >> 18 & 63] + Dl[e >> 12 & 63] + Dl[e >> 6 & 63] + Dl[63 & e]
     }
 
-    function Il(e, t, r) {
-        for (var n, i = [], o = t; o < r; o += 3) n = (e[o] << 16) + (e[o + 1] << 8) + e[o + 2], i.push(Nl(n));
+    function Fl(e, t, r) {
+        for (var n, i = [], o = t; o < r; o += 3) n = (e[o] << 16) + (e[o + 1] << 8) + e[o + 2], i.push(Il(n));
         return i.join("")
     }
 
-    function Fl(e) {
+    function Ml(e) {
         var t;
-        Rl || Ll();
-        for (var r = e.length, n = r % 3, i = "", o = [], s = 16383, a = 0, l = r - n; a < l; a += s) o.push(Il(e, a, a + s > l ? l : a + s));
-        return 1 === n ? (t = e[r - 1], i += Sl[t >> 2], i += Sl[t << 4 & 63], i += "==") : 2 === n && (t = (e[r - 2] << 8) + e[r - 1], i += Sl[t >> 10], i += Sl[t >> 4 & 63], i += Sl[t << 2 & 63], i += "="), o.push(i), o.join("")
+        Ll || Nl();
+        for (var r = e.length, n = r % 3, i = "", o = [], s = 16383, a = 0, l = r - n; a < l; a += s) o.push(Fl(e, a, a + s > l ? l : a + s));
+        return 1 === n ? (t = e[r - 1], i += Dl[t >> 2], i += Dl[t << 4 & 63], i += "==") : 2 === n && (t = (e[r - 2] << 8) + e[r - 1], i += Dl[t >> 10], i += Dl[t >> 4 & 63], i += Dl[t << 2 & 63], i += "="), o.push(i), o.join("")
     }
 
-    function Ml(e, t, r, n, i) {
+    function Pl(e, t, r, n, i) {
         var o, s, a = 8 * i - n - 1,
             l = (1 << a) - 1,
             u = l >> 1,
             c = -7,
             f = r ? i - 1 : 0,
             h = r ? -1 : 1,
             p = e[t + f];
@@ -11661,185 +11681,185 @@
         else {
             if (o === l) return s ? NaN : 1 / 0 * (p ? -1 : 1);
             s += Math.pow(2, n), o -= u
         }
         return (p ? -1 : 1) * s * Math.pow(2, o - n)
     }
 
-    function Pl(e, t, r, n, i, o) {
+    function jl(e, t, r, n, i, o) {
         var s, a, l, u = 8 * o - i - 1,
             c = (1 << u) - 1,
             f = c >> 1,
             h = 23 === i ? Math.pow(2, -24) - Math.pow(2, -77) : 0,
             p = n ? 0 : o - 1,
             d = n ? 1 : -1,
             m = t < 0 || 0 === t && 1 / t < 0 ? 1 : 0;
         for (t = Math.abs(t), isNaN(t) || t === 1 / 0 ? (a = isNaN(t) ? 1 : 0, s = c) : (s = Math.floor(Math.log(t) / Math.LN2), t * (l = Math.pow(2, -s)) < 1 && (s--, l *= 2), (t += s + f >= 1 ? h / l : h * Math.pow(2, 1 - f)) * l >= 2 && (s++, l /= 2), s + f >= c ? (a = 0, s = c) : s + f >= 1 ? (a = (t * l - 1) * Math.pow(2, i), s += f) : (a = t * Math.pow(2, f - 1) * Math.pow(2, i), s = 0)); i >= 8; e[r + p] = 255 & a, p += d, a /= 256, i -= 8);
         for (s = s << i | a, u += i; u > 0; e[r + p] = 255 & s, p += d, s /= 256, u -= 8);
         e[r + p - d] |= 128 * m
     }
-    var jl = {}.toString,
-        Bl = Array.isArray || function(e) {
-            return "[object Array]" == jl.call(e)
+    var Bl = {}.toString,
+        Ul = Array.isArray || function(e) {
+            return "[object Array]" == Bl.call(e)
         };
 
-    function Ul() {
-        return zl.TYPED_ARRAY_SUPPORT ? 2147483647 : 1073741823
+    function Vl() {
+        return Hl.TYPED_ARRAY_SUPPORT ? 2147483647 : 1073741823
     }
 
-    function Vl(e, t) {
-        if (Ul() < t) throw new RangeError("Invalid typed array length");
-        return zl.TYPED_ARRAY_SUPPORT ? (e = new Uint8Array(t)).__proto__ = zl.prototype : (null === e && (e = new zl(t)), e.length = t), e
+    function zl(e, t) {
+        if (Vl() < t) throw new RangeError("Invalid typed array length");
+        return Hl.TYPED_ARRAY_SUPPORT ? (e = new Uint8Array(t)).__proto__ = Hl.prototype : (null === e && (e = new Hl(t)), e.length = t), e
     }
 
-    function zl(e, t, r) {
-        if (!(zl.TYPED_ARRAY_SUPPORT || this instanceof zl)) return new zl(e, t, r);
+    function Hl(e, t, r) {
+        if (!(Hl.TYPED_ARRAY_SUPPORT || this instanceof Hl)) return new Hl(e, t, r);
         if ("number" == typeof e) {
             if ("string" == typeof t) throw new Error("If encoding is specified then the first argument must be a string");
-            return Gl(this, e)
+            return Zl(this, e)
         }
-        return Hl(this, e, t, r)
+        return Wl(this, e, t, r)
     }
 
-    function Hl(e, t, r, n) {
+    function Wl(e, t, r, n) {
         if ("number" == typeof t) throw new TypeError('"value" argument must not be a number');
         return "undefined" != typeof ArrayBuffer && t instanceof ArrayBuffer ? function(e, t, r, n) {
             if (t.byteLength, r < 0 || t.byteLength < r) throw new RangeError("'offset' is out of bounds");
             if (t.byteLength < r + (n || 0)) throw new RangeError("'length' is out of bounds");
             t = void 0 === r && void 0 === n ? new Uint8Array(t) : void 0 === n ? new Uint8Array(t, r) : new Uint8Array(t, r, n);
-            zl.TYPED_ARRAY_SUPPORT ? (e = t).__proto__ = zl.prototype : e = Zl(e, t);
+            Hl.TYPED_ARRAY_SUPPORT ? (e = t).__proto__ = Hl.prototype : e = Jl(e, t);
             return e
         }(e, t, r, n) : "string" == typeof t ? function(e, t, r) {
             "string" == typeof r && "" !== r || (r = "utf8");
-            if (!zl.isEncoding(r)) throw new TypeError('"encoding" must be a valid string encoding');
-            var n = 0 | Kl(t, r);
-            e = Vl(e, n);
+            if (!Hl.isEncoding(r)) throw new TypeError('"encoding" must be a valid string encoding');
+            var n = 0 | Xl(t, r);
+            e = zl(e, n);
             var i = e.write(t, r);
             i !== n && (e = e.slice(0, i));
             return e
         }(e, t, r) : function(e, t) {
-            if (Yl(t)) {
-                var r = 0 | Jl(t.length);
-                return 0 === (e = Vl(e, r)).length || t.copy(e, 0, 0, r), e
+            if (Kl(t)) {
+                var r = 0 | Yl(t.length);
+                return 0 === (e = zl(e, r)).length || t.copy(e, 0, 0, r), e
             }
             if (t) {
-                if ("undefined" != typeof ArrayBuffer && t.buffer instanceof ArrayBuffer || "length" in t) return "number" != typeof t.length || (n = t.length) != n ? Vl(e, 0) : Zl(e, t);
-                if ("Buffer" === t.type && Bl(t.data)) return Zl(e, t.data)
+                if ("undefined" != typeof ArrayBuffer && t.buffer instanceof ArrayBuffer || "length" in t) return "number" != typeof t.length || (n = t.length) != n ? zl(e, 0) : Jl(e, t);
+                if ("Buffer" === t.type && Ul(t.data)) return Jl(e, t.data)
             }
             var n;
             throw new TypeError("First argument must be a string, Buffer, ArrayBuffer, Array, or array-like object.")
         }(e, t)
     }
 
-    function Wl(e) {
+    function Gl(e) {
         if ("number" != typeof e) throw new TypeError('"size" argument must be a number');
         if (e < 0) throw new RangeError('"size" argument must not be negative')
     }
 
-    function Gl(e, t) {
-        if (Wl(t), e = Vl(e, t < 0 ? 0 : 0 | Jl(t)), !zl.TYPED_ARRAY_SUPPORT)
+    function Zl(e, t) {
+        if (Gl(t), e = zl(e, t < 0 ? 0 : 0 | Yl(t)), !Hl.TYPED_ARRAY_SUPPORT)
             for (var r = 0; r < t; ++r) e[r] = 0;
         return e
     }
 
-    function Zl(e, t) {
-        var r = t.length < 0 ? 0 : 0 | Jl(t.length);
-        e = Vl(e, r);
+    function Jl(e, t) {
+        var r = t.length < 0 ? 0 : 0 | Yl(t.length);
+        e = zl(e, r);
         for (var n = 0; n < r; n += 1) e[n] = 255 & t[n];
         return e
     }
 
-    function Jl(e) {
-        if (e >= Ul()) throw new RangeError("Attempt to allocate Buffer larger than maximum size: 0x" + Ul().toString(16) + " bytes");
+    function Yl(e) {
+        if (e >= Vl()) throw new RangeError("Attempt to allocate Buffer larger than maximum size: 0x" + Vl().toString(16) + " bytes");
         return 0 | e
     }
 
-    function Yl(e) {
+    function Kl(e) {
         return !(null == e || !e._isBuffer)
     }
 
-    function Kl(e, t) {
-        if (Yl(e)) return e.length;
+    function Xl(e, t) {
+        if (Kl(e)) return e.length;
         if ("undefined" != typeof ArrayBuffer && "function" == typeof ArrayBuffer.isView && (ArrayBuffer.isView(e) || e instanceof ArrayBuffer)) return e.byteLength;
         "string" != typeof e && (e = "" + e);
         var r = e.length;
         if (0 === r) return 0;
         for (var n = !1;;) switch (t) {
             case "ascii":
             case "latin1":
             case "binary":
                 return r;
             case "utf8":
             case "utf-8":
             case void 0:
-                return Au(e).length;
+                return qu(e).length;
             case "ucs2":
             case "ucs-2":
             case "utf16le":
             case "utf-16le":
                 return 2 * r;
             case "hex":
                 return r >>> 1;
             case "base64":
-                return qu(e).length;
+                return Eu(e).length;
             default:
-                if (n) return Au(e).length;
+                if (n) return qu(e).length;
                 t = ("" + t).toLowerCase(), n = !0
         }
     }
 
-    function Xl(e, t, r) {
+    function Ql(e, t, r) {
         var n = !1;
         if ((void 0 === t || t < 0) && (t = 0), t > this.length) return "";
         if ((void 0 === r || r > this.length) && (r = this.length), r <= 0) return "";
         if ((r >>>= 0) <= (t >>>= 0)) return "";
         for (e || (e = "utf8");;) switch (e) {
             case "hex":
-                return pu(this, t, r);
+                return du(this, t, r);
             case "utf8":
             case "utf-8":
-                return uu(this, t, r);
+                return cu(this, t, r);
             case "ascii":
-                return fu(this, t, r);
+                return hu(this, t, r);
             case "latin1":
             case "binary":
-                return hu(this, t, r);
+                return pu(this, t, r);
             case "base64":
-                return lu(this, t, r);
+                return uu(this, t, r);
             case "ucs2":
             case "ucs-2":
             case "utf16le":
             case "utf-16le":
-                return du(this, t, r);
+                return mu(this, t, r);
             default:
                 if (n) throw new TypeError("Unknown encoding: " + e);
                 e = (e + "").toLowerCase(), n = !0
         }
     }
 
-    function Ql(e, t, r) {
+    function eu(e, t, r) {
         var n = e[t];
         e[t] = e[r], e[r] = n
     }
 
-    function eu(e, t, r, n, i) {
+    function tu(e, t, r, n, i) {
         if (0 === e.length) return -1;
         if ("string" == typeof r ? (n = r, r = 0) : r > 2147483647 ? r = 2147483647 : r < -2147483648 && (r = -2147483648), r = +r, isNaN(r) && (r = i ? 0 : e.length - 1), r < 0 && (r = e.length + r), r >= e.length) {
             if (i) return -1;
             r = e.length - 1
         } else if (r < 0) {
             if (!i) return -1;
             r = 0
         }
-        if ("string" == typeof t && (t = zl.from(t, n)), Yl(t)) return 0 === t.length ? -1 : tu(e, t, r, n, i);
-        if ("number" == typeof t) return t &= 255, zl.TYPED_ARRAY_SUPPORT && "function" == typeof Uint8Array.prototype.indexOf ? i ? Uint8Array.prototype.indexOf.call(e, t, r) : Uint8Array.prototype.lastIndexOf.call(e, t, r) : tu(e, [t], r, n, i);
+        if ("string" == typeof t && (t = Hl.from(t, n)), Kl(t)) return 0 === t.length ? -1 : ru(e, t, r, n, i);
+        if ("number" == typeof t) return t &= 255, Hl.TYPED_ARRAY_SUPPORT && "function" == typeof Uint8Array.prototype.indexOf ? i ? Uint8Array.prototype.indexOf.call(e, t, r) : Uint8Array.prototype.lastIndexOf.call(e, t, r) : ru(e, [t], r, n, i);
         throw new TypeError("val must be string, number or Buffer")
     }
 
-    function tu(e, t, r, n, i) {
+    function ru(e, t, r, n, i) {
         var o, s = 1,
             a = e.length,
             l = t.length;
         if (void 0 !== n && ("ucs2" === (n = String(n).toLowerCase()) || "ucs-2" === n || "utf16le" === n || "utf-16le" === n)) {
             if (e.length < 2 || t.length < 2) return -1;
             s = 2, a /= 2, l /= 2, r /= 2
         }
@@ -11860,60 +11880,60 @@
                         f = !1;
                         break
                     } if (f) return o
             }
         return -1
     }
 
-    function ru(e, t, r, n) {
+    function nu(e, t, r, n) {
         r = Number(r) || 0;
         var i = e.length - r;
         n ? (n = Number(n)) > i && (n = i) : n = i;
         var o = t.length;
         if (o % 2 != 0) throw new TypeError("Invalid hex string");
         n > o / 2 && (n = o / 2);
         for (var s = 0; s < n; ++s) {
             var a = parseInt(t.substr(2 * s, 2), 16);
             if (isNaN(a)) return s;
             e[r + s] = a
         }
         return s
     }
 
-    function nu(e, t, r, n) {
-        return Eu(Au(t, e.length - r), e, r, n)
+    function iu(e, t, r, n) {
+        return Tu(qu(t, e.length - r), e, r, n)
     }
 
-    function iu(e, t, r, n) {
-        return Eu(function(e) {
+    function ou(e, t, r, n) {
+        return Tu(function(e) {
             for (var t = [], r = 0; r < e.length; ++r) t.push(255 & e.charCodeAt(r));
             return t
         }(t), e, r, n)
     }
 
-    function ou(e, t, r, n) {
-        return iu(e, t, r, n)
-    }
-
     function su(e, t, r, n) {
-        return Eu(qu(t), e, r, n)
+        return ou(e, t, r, n)
     }
 
     function au(e, t, r, n) {
-        return Eu(function(e, t) {
+        return Tu(Eu(t), e, r, n)
+    }
+
+    function lu(e, t, r, n) {
+        return Tu(function(e, t) {
             for (var r, n, i, o = [], s = 0; s < e.length && !((t -= 2) < 0); ++s) n = (r = e.charCodeAt(s)) >> 8, i = r % 256, o.push(i), o.push(n);
             return o
         }(t, e.length - r), e, r, n)
     }
 
-    function lu(e, t, r) {
-        return 0 === t && r === e.length ? Fl(e) : Fl(e.slice(t, r))
+    function uu(e, t, r) {
+        return 0 === t && r === e.length ? Ml(e) : Ml(e.slice(t, r))
     }
 
-    function uu(e, t, r) {
+    function cu(e, t, r) {
         r = Math.min(e.length, r);
         for (var n = [], i = t; i < r;) {
             var o, s, a, l, u = e[i],
                 c = null,
                 f = u > 239 ? 4 : u > 223 ? 3 : u > 191 ? 2 : 1;
             if (i + f <= r) switch (f) {
                 case 1:
@@ -11928,46 +11948,46 @@
                 case 4:
                     o = e[i + 1], s = e[i + 2], a = e[i + 3], 128 == (192 & o) && 128 == (192 & s) && 128 == (192 & a) && (l = (15 & u) << 18 | (63 & o) << 12 | (63 & s) << 6 | 63 & a) > 65535 && l < 1114112 && (c = l)
             }
             null === c ? (c = 65533, f = 1) : c > 65535 && (c -= 65536, n.push(c >>> 10 & 1023 | 55296), c = 56320 | 1023 & c), n.push(c), i += f
         }
         return function(e) {
             var t = e.length;
-            if (t <= cu) return String.fromCharCode.apply(String, e);
+            if (t <= fu) return String.fromCharCode.apply(String, e);
             var r = "",
                 n = 0;
-            for (; n < t;) r += String.fromCharCode.apply(String, e.slice(n, n += cu));
+            for (; n < t;) r += String.fromCharCode.apply(String, e.slice(n, n += fu));
             return r
         }(n)
     }
-    zl.TYPED_ARRAY_SUPPORT = void 0 === pr.TYPED_ARRAY_SUPPORT || pr.TYPED_ARRAY_SUPPORT, Ul(), zl.poolSize = 8192, zl._augment = function(e) {
-        return e.__proto__ = zl.prototype, e
-    }, zl.from = function(e, t, r) {
-        return Hl(null, e, t, r)
-    }, zl.TYPED_ARRAY_SUPPORT && (zl.prototype.__proto__ = Uint8Array.prototype, zl.__proto__ = Uint8Array, "undefined" != typeof Symbol && Symbol.species && zl[Symbol.species]), zl.alloc = function(e, t, r) {
+    Hl.TYPED_ARRAY_SUPPORT = void 0 === A.TYPED_ARRAY_SUPPORT || A.TYPED_ARRAY_SUPPORT, Vl(), Hl.poolSize = 8192, Hl._augment = function(e) {
+        return e.__proto__ = Hl.prototype, e
+    }, Hl.from = function(e, t, r) {
+        return Wl(null, e, t, r)
+    }, Hl.TYPED_ARRAY_SUPPORT && (Hl.prototype.__proto__ = Uint8Array.prototype, Hl.__proto__ = Uint8Array, "undefined" != typeof Symbol && Symbol.species && Hl[Symbol.species]), Hl.alloc = function(e, t, r) {
         return function(e, t, r, n) {
-            return Wl(t), t <= 0 ? Vl(e, t) : void 0 !== r ? "string" == typeof n ? Vl(e, t).fill(r, n) : Vl(e, t).fill(r) : Vl(e, t)
+            return Gl(t), t <= 0 ? zl(e, t) : void 0 !== r ? "string" == typeof n ? zl(e, t).fill(r, n) : zl(e, t).fill(r) : zl(e, t)
         }(null, e, t, r)
-    }, zl.allocUnsafe = function(e) {
-        return Gl(null, e)
-    }, zl.allocUnsafeSlow = function(e) {
-        return Gl(null, e)
-    }, zl.isBuffer = function(e) {
-        return null != e && (!!e._isBuffer || Tu(e) || function(e) {
-            return "function" == typeof e.readFloatLE && "function" == typeof e.slice && Tu(e.slice(0, 0))
+    }, Hl.allocUnsafe = function(e) {
+        return Zl(null, e)
+    }, Hl.allocUnsafeSlow = function(e) {
+        return Zl(null, e)
+    }, Hl.isBuffer = function(e) {
+        return null != e && (!!e._isBuffer || $u(e) || function(e) {
+            return "function" == typeof e.readFloatLE && "function" == typeof e.slice && $u(e.slice(0, 0))
         }(e))
-    }, zl.compare = function(e, t) {
-        if (!Yl(e) || !Yl(t)) throw new TypeError("Arguments must be Buffers");
+    }, Hl.compare = function(e, t) {
+        if (!Kl(e) || !Kl(t)) throw new TypeError("Arguments must be Buffers");
         if (e === t) return 0;
         for (var r = e.length, n = t.length, i = 0, o = Math.min(r, n); i < o; ++i)
             if (e[i] !== t[i]) {
                 r = e[i], n = t[i];
                 break
             } return r < n ? -1 : n < r ? 1 : 0
-    }, zl.isEncoding = function(e) {
+    }, Hl.isEncoding = function(e) {
         switch (String(e).toLowerCase()) {
             case "hex":
             case "utf8":
             case "utf-8":
             case "ascii":
             case "latin1":
             case "binary":
@@ -11976,328 +11996,328 @@
             case "ucs-2":
             case "utf16le":
             case "utf-16le":
                 return !0;
             default:
                 return !1
         }
-    }, zl.concat = function(e, t) {
-        if (!Bl(e)) throw new TypeError('"list" argument must be an Array of Buffers');
-        if (0 === e.length) return zl.alloc(0);
+    }, Hl.concat = function(e, t) {
+        if (!Ul(e)) throw new TypeError('"list" argument must be an Array of Buffers');
+        if (0 === e.length) return Hl.alloc(0);
         var r;
         if (void 0 === t)
             for (t = 0, r = 0; r < e.length; ++r) t += e[r].length;
-        var n = zl.allocUnsafe(t),
+        var n = Hl.allocUnsafe(t),
             i = 0;
         for (r = 0; r < e.length; ++r) {
             var o = e[r];
-            if (!Yl(o)) throw new TypeError('"list" argument must be an Array of Buffers');
+            if (!Kl(o)) throw new TypeError('"list" argument must be an Array of Buffers');
             o.copy(n, i), i += o.length
         }
         return n
-    }, zl.byteLength = Kl, zl.prototype._isBuffer = !0, zl.prototype.swap16 = function() {
+    }, Hl.byteLength = Xl, Hl.prototype._isBuffer = !0, Hl.prototype.swap16 = function() {
         var e = this.length;
         if (e % 2 != 0) throw new RangeError("Buffer size must be a multiple of 16-bits");
-        for (var t = 0; t < e; t += 2) Ql(this, t, t + 1);
+        for (var t = 0; t < e; t += 2) eu(this, t, t + 1);
         return this
-    }, zl.prototype.swap32 = function() {
+    }, Hl.prototype.swap32 = function() {
         var e = this.length;
         if (e % 4 != 0) throw new RangeError("Buffer size must be a multiple of 32-bits");
-        for (var t = 0; t < e; t += 4) Ql(this, t, t + 3), Ql(this, t + 1, t + 2);
+        for (var t = 0; t < e; t += 4) eu(this, t, t + 3), eu(this, t + 1, t + 2);
         return this
-    }, zl.prototype.swap64 = function() {
+    }, Hl.prototype.swap64 = function() {
         var e = this.length;
         if (e % 8 != 0) throw new RangeError("Buffer size must be a multiple of 64-bits");
-        for (var t = 0; t < e; t += 8) Ql(this, t, t + 7), Ql(this, t + 1, t + 6), Ql(this, t + 2, t + 5), Ql(this, t + 3, t + 4);
+        for (var t = 0; t < e; t += 8) eu(this, t, t + 7), eu(this, t + 1, t + 6), eu(this, t + 2, t + 5), eu(this, t + 3, t + 4);
         return this
-    }, zl.prototype.toString = function() {
+    }, Hl.prototype.toString = function() {
         var e = 0 | this.length;
-        return 0 === e ? "" : 0 === arguments.length ? uu(this, 0, e) : Xl.apply(this, arguments)
-    }, zl.prototype.equals = function(e) {
-        if (!Yl(e)) throw new TypeError("Argument must be a Buffer");
-        return this === e || 0 === zl.compare(this, e)
-    }, zl.prototype.inspect = function() {
+        return 0 === e ? "" : 0 === arguments.length ? cu(this, 0, e) : Ql.apply(this, arguments)
+    }, Hl.prototype.equals = function(e) {
+        if (!Kl(e)) throw new TypeError("Argument must be a Buffer");
+        return this === e || 0 === Hl.compare(this, e)
+    }, Hl.prototype.inspect = function() {
         var e = "";
         return this.length > 0 && (e = this.toString("hex", 0, 50).match(/.{2}/g).join(" "), this.length > 50 && (e += " ... ")), "<Buffer " + e + ">"
-    }, zl.prototype.compare = function(e, t, r, n, i) {
-        if (!Yl(e)) throw new TypeError("Argument must be a Buffer");
+    }, Hl.prototype.compare = function(e, t, r, n, i) {
+        if (!Kl(e)) throw new TypeError("Argument must be a Buffer");
         if (void 0 === t && (t = 0), void 0 === r && (r = e ? e.length : 0), void 0 === n && (n = 0), void 0 === i && (i = this.length), t < 0 || r > e.length || n < 0 || i > this.length) throw new RangeError("out of range index");
         if (n >= i && t >= r) return 0;
         if (n >= i) return -1;
         if (t >= r) return 1;
         if (this === e) return 0;
         for (var o = (i >>>= 0) - (n >>>= 0), s = (r >>>= 0) - (t >>>= 0), a = Math.min(o, s), l = this.slice(n, i), u = e.slice(t, r), c = 0; c < a; ++c)
             if (l[c] !== u[c]) {
                 o = l[c], s = u[c];
                 break
             } return o < s ? -1 : s < o ? 1 : 0
-    }, zl.prototype.includes = function(e, t, r) {
+    }, Hl.prototype.includes = function(e, t, r) {
         return -1 !== this.indexOf(e, t, r)
-    }, zl.prototype.indexOf = function(e, t, r) {
-        return eu(this, e, t, r, !0)
-    }, zl.prototype.lastIndexOf = function(e, t, r) {
-        return eu(this, e, t, r, !1)
-    }, zl.prototype.write = function(e, t, r, n) {
+    }, Hl.prototype.indexOf = function(e, t, r) {
+        return tu(this, e, t, r, !0)
+    }, Hl.prototype.lastIndexOf = function(e, t, r) {
+        return tu(this, e, t, r, !1)
+    }, Hl.prototype.write = function(e, t, r, n) {
         if (void 0 === t) n = "utf8", r = this.length, t = 0;
         else if (void 0 === r && "string" == typeof t) n = t, r = this.length, t = 0;
         else {
             if (!isFinite(t)) throw new Error("Buffer.write(string, encoding, offset[, length]) is no longer supported");
             t |= 0, isFinite(r) ? (r |= 0, void 0 === n && (n = "utf8")) : (n = r, r = void 0)
         }
         var i = this.length - t;
         if ((void 0 === r || r > i) && (r = i), e.length > 0 && (r < 0 || t < 0) || t > this.length) throw new RangeError("Attempt to write outside buffer bounds");
         n || (n = "utf8");
         for (var o = !1;;) switch (n) {
             case "hex":
-                return ru(this, e, t, r);
+                return nu(this, e, t, r);
             case "utf8":
             case "utf-8":
-                return nu(this, e, t, r);
-            case "ascii":
                 return iu(this, e, t, r);
+            case "ascii":
+                return ou(this, e, t, r);
             case "latin1":
             case "binary":
-                return ou(this, e, t, r);
-            case "base64":
                 return su(this, e, t, r);
+            case "base64":
+                return au(this, e, t, r);
             case "ucs2":
             case "ucs-2":
             case "utf16le":
             case "utf-16le":
-                return au(this, e, t, r);
+                return lu(this, e, t, r);
             default:
                 if (o) throw new TypeError("Unknown encoding: " + n);
                 n = ("" + n).toLowerCase(), o = !0
         }
-    }, zl.prototype.toJSON = function() {
+    }, Hl.prototype.toJSON = function() {
         return {
             type: "Buffer",
             data: Array.prototype.slice.call(this._arr || this, 0)
         }
     };
-    var cu = 4096;
+    var fu = 4096;
 
-    function fu(e, t, r) {
+    function hu(e, t, r) {
         var n = "";
         r = Math.min(e.length, r);
         for (var i = t; i < r; ++i) n += String.fromCharCode(127 & e[i]);
         return n
     }
 
-    function hu(e, t, r) {
+    function pu(e, t, r) {
         var n = "";
         r = Math.min(e.length, r);
         for (var i = t; i < r; ++i) n += String.fromCharCode(e[i]);
         return n
     }
 
-    function pu(e, t, r) {
+    function du(e, t, r) {
         var n = e.length;
         (!t || t < 0) && (t = 0), (!r || r < 0 || r > n) && (r = n);
-        for (var i = "", o = t; o < r; ++o) i += xu(e[o]);
+        for (var i = "", o = t; o < r; ++o) i += Au(e[o]);
         return i
     }
 
-    function du(e, t, r) {
+    function mu(e, t, r) {
         for (var n = e.slice(t, r), i = "", o = 0; o < n.length; o += 2) i += String.fromCharCode(n[o] + 256 * n[o + 1]);
         return i
     }
 
-    function mu(e, t, r) {
+    function gu(e, t, r) {
         if (e % 1 != 0 || e < 0) throw new RangeError("offset is not uint");
         if (e + t > r) throw new RangeError("Trying to access beyond buffer length")
     }
 
-    function gu(e, t, r, n, i, o) {
-        if (!Yl(e)) throw new TypeError('"buffer" argument must be a Buffer instance');
+    function vu(e, t, r, n, i, o) {
+        if (!Kl(e)) throw new TypeError('"buffer" argument must be a Buffer instance');
         if (t > i || t < o) throw new RangeError('"value" argument is out of bounds');
         if (r + n > e.length) throw new RangeError("Index out of range")
     }
 
-    function vu(e, t, r, n) {
+    function yu(e, t, r, n) {
         t < 0 && (t = 65535 + t + 1);
         for (var i = 0, o = Math.min(e.length - r, 2); i < o; ++i) e[r + i] = (t & 255 << 8 * (n ? i : 1 - i)) >>> 8 * (n ? i : 1 - i)
     }
 
-    function yu(e, t, r, n) {
+    function bu(e, t, r, n) {
         t < 0 && (t = 4294967295 + t + 1);
         for (var i = 0, o = Math.min(e.length - r, 4); i < o; ++i) e[r + i] = t >>> 8 * (n ? i : 3 - i) & 255
     }
 
-    function bu(e, t, r, n, i, o) {
+    function wu(e, t, r, n, i, o) {
         if (r + n > e.length) throw new RangeError("Index out of range");
         if (r < 0) throw new RangeError("Index out of range")
     }
 
-    function wu(e, t, r, n, i) {
-        return i || bu(e, 0, r, 4), Pl(e, t, r, n, 23, 4), r + 4
+    function _u(e, t, r, n, i) {
+        return i || wu(e, 0, r, 4), jl(e, t, r, n, 23, 4), r + 4
     }
 
-    function _u(e, t, r, n, i) {
-        return i || bu(e, 0, r, 8), Pl(e, t, r, n, 52, 8), r + 8
+    function ku(e, t, r, n, i) {
+        return i || wu(e, 0, r, 8), jl(e, t, r, n, 52, 8), r + 8
     }
-    zl.prototype.slice = function(e, t) {
+    Hl.prototype.slice = function(e, t) {
         var r, n = this.length;
-        if ((e = ~~e) < 0 ? (e += n) < 0 && (e = 0) : e > n && (e = n), (t = void 0 === t ? n : ~~t) < 0 ? (t += n) < 0 && (t = 0) : t > n && (t = n), t < e && (t = e), zl.TYPED_ARRAY_SUPPORT)(r = this.subarray(e, t)).__proto__ = zl.prototype;
+        if ((e = ~~e) < 0 ? (e += n) < 0 && (e = 0) : e > n && (e = n), (t = void 0 === t ? n : ~~t) < 0 ? (t += n) < 0 && (t = 0) : t > n && (t = n), t < e && (t = e), Hl.TYPED_ARRAY_SUPPORT)(r = this.subarray(e, t)).__proto__ = Hl.prototype;
         else {
             var i = t - e;
-            r = new zl(i, void 0);
+            r = new Hl(i, void 0);
             for (var o = 0; o < i; ++o) r[o] = this[o + e]
         }
         return r
-    }, zl.prototype.readUIntLE = function(e, t, r) {
-        e |= 0, t |= 0, r || mu(e, t, this.length);
+    }, Hl.prototype.readUIntLE = function(e, t, r) {
+        e |= 0, t |= 0, r || gu(e, t, this.length);
         for (var n = this[e], i = 1, o = 0; ++o < t && (i *= 256);) n += this[e + o] * i;
         return n
-    }, zl.prototype.readUIntBE = function(e, t, r) {
-        e |= 0, t |= 0, r || mu(e, t, this.length);
+    }, Hl.prototype.readUIntBE = function(e, t, r) {
+        e |= 0, t |= 0, r || gu(e, t, this.length);
         for (var n = this[e + --t], i = 1; t > 0 && (i *= 256);) n += this[e + --t] * i;
         return n
-    }, zl.prototype.readUInt8 = function(e, t) {
-        return t || mu(e, 1, this.length), this[e]
-    }, zl.prototype.readUInt16LE = function(e, t) {
-        return t || mu(e, 2, this.length), this[e] | this[e + 1] << 8
-    }, zl.prototype.readUInt16BE = function(e, t) {
-        return t || mu(e, 2, this.length), this[e] << 8 | this[e + 1]
-    }, zl.prototype.readUInt32LE = function(e, t) {
-        return t || mu(e, 4, this.length), (this[e] | this[e + 1] << 8 | this[e + 2] << 16) + 16777216 * this[e + 3]
-    }, zl.prototype.readUInt32BE = function(e, t) {
-        return t || mu(e, 4, this.length), 16777216 * this[e] + (this[e + 1] << 16 | this[e + 2] << 8 | this[e + 3])
-    }, zl.prototype.readIntLE = function(e, t, r) {
-        e |= 0, t |= 0, r || mu(e, t, this.length);
+    }, Hl.prototype.readUInt8 = function(e, t) {
+        return t || gu(e, 1, this.length), this[e]
+    }, Hl.prototype.readUInt16LE = function(e, t) {
+        return t || gu(e, 2, this.length), this[e] | this[e + 1] << 8
+    }, Hl.prototype.readUInt16BE = function(e, t) {
+        return t || gu(e, 2, this.length), this[e] << 8 | this[e + 1]
+    }, Hl.prototype.readUInt32LE = function(e, t) {
+        return t || gu(e, 4, this.length), (this[e] | this[e + 1] << 8 | this[e + 2] << 16) + 16777216 * this[e + 3]
+    }, Hl.prototype.readUInt32BE = function(e, t) {
+        return t || gu(e, 4, this.length), 16777216 * this[e] + (this[e + 1] << 16 | this[e + 2] << 8 | this[e + 3])
+    }, Hl.prototype.readIntLE = function(e, t, r) {
+        e |= 0, t |= 0, r || gu(e, t, this.length);
         for (var n = this[e], i = 1, o = 0; ++o < t && (i *= 256);) n += this[e + o] * i;
         return n >= (i *= 128) && (n -= Math.pow(2, 8 * t)), n
-    }, zl.prototype.readIntBE = function(e, t, r) {
-        e |= 0, t |= 0, r || mu(e, t, this.length);
+    }, Hl.prototype.readIntBE = function(e, t, r) {
+        e |= 0, t |= 0, r || gu(e, t, this.length);
         for (var n = t, i = 1, o = this[e + --n]; n > 0 && (i *= 256);) o += this[e + --n] * i;
         return o >= (i *= 128) && (o -= Math.pow(2, 8 * t)), o
-    }, zl.prototype.readInt8 = function(e, t) {
-        return t || mu(e, 1, this.length), 128 & this[e] ? -1 * (255 - this[e] + 1) : this[e]
-    }, zl.prototype.readInt16LE = function(e, t) {
-        t || mu(e, 2, this.length);
+    }, Hl.prototype.readInt8 = function(e, t) {
+        return t || gu(e, 1, this.length), 128 & this[e] ? -1 * (255 - this[e] + 1) : this[e]
+    }, Hl.prototype.readInt16LE = function(e, t) {
+        t || gu(e, 2, this.length);
         var r = this[e] | this[e + 1] << 8;
         return 32768 & r ? 4294901760 | r : r
-    }, zl.prototype.readInt16BE = function(e, t) {
-        t || mu(e, 2, this.length);
+    }, Hl.prototype.readInt16BE = function(e, t) {
+        t || gu(e, 2, this.length);
         var r = this[e + 1] | this[e] << 8;
         return 32768 & r ? 4294901760 | r : r
-    }, zl.prototype.readInt32LE = function(e, t) {
-        return t || mu(e, 4, this.length), this[e] | this[e + 1] << 8 | this[e + 2] << 16 | this[e + 3] << 24
-    }, zl.prototype.readInt32BE = function(e, t) {
-        return t || mu(e, 4, this.length), this[e] << 24 | this[e + 1] << 16 | this[e + 2] << 8 | this[e + 3]
-    }, zl.prototype.readFloatLE = function(e, t) {
-        return t || mu(e, 4, this.length), Ml(this, e, !0, 23, 4)
-    }, zl.prototype.readFloatBE = function(e, t) {
-        return t || mu(e, 4, this.length), Ml(this, e, !1, 23, 4)
-    }, zl.prototype.readDoubleLE = function(e, t) {
-        return t || mu(e, 8, this.length), Ml(this, e, !0, 52, 8)
-    }, zl.prototype.readDoubleBE = function(e, t) {
-        return t || mu(e, 8, this.length), Ml(this, e, !1, 52, 8)
-    }, zl.prototype.writeUIntLE = function(e, t, r, n) {
-        (e = +e, t |= 0, r |= 0, n) || gu(this, e, t, r, Math.pow(2, 8 * r) - 1, 0);
+    }, Hl.prototype.readInt32LE = function(e, t) {
+        return t || gu(e, 4, this.length), this[e] | this[e + 1] << 8 | this[e + 2] << 16 | this[e + 3] << 24
+    }, Hl.prototype.readInt32BE = function(e, t) {
+        return t || gu(e, 4, this.length), this[e] << 24 | this[e + 1] << 16 | this[e + 2] << 8 | this[e + 3]
+    }, Hl.prototype.readFloatLE = function(e, t) {
+        return t || gu(e, 4, this.length), Pl(this, e, !0, 23, 4)
+    }, Hl.prototype.readFloatBE = function(e, t) {
+        return t || gu(e, 4, this.length), Pl(this, e, !1, 23, 4)
+    }, Hl.prototype.readDoubleLE = function(e, t) {
+        return t || gu(e, 8, this.length), Pl(this, e, !0, 52, 8)
+    }, Hl.prototype.readDoubleBE = function(e, t) {
+        return t || gu(e, 8, this.length), Pl(this, e, !1, 52, 8)
+    }, Hl.prototype.writeUIntLE = function(e, t, r, n) {
+        (e = +e, t |= 0, r |= 0, n) || vu(this, e, t, r, Math.pow(2, 8 * r) - 1, 0);
         var i = 1,
             o = 0;
         for (this[t] = 255 & e; ++o < r && (i *= 256);) this[t + o] = e / i & 255;
         return t + r
-    }, zl.prototype.writeUIntBE = function(e, t, r, n) {
-        (e = +e, t |= 0, r |= 0, n) || gu(this, e, t, r, Math.pow(2, 8 * r) - 1, 0);
+    }, Hl.prototype.writeUIntBE = function(e, t, r, n) {
+        (e = +e, t |= 0, r |= 0, n) || vu(this, e, t, r, Math.pow(2, 8 * r) - 1, 0);
         var i = r - 1,
             o = 1;
         for (this[t + i] = 255 & e; --i >= 0 && (o *= 256);) this[t + i] = e / o & 255;
         return t + r
-    }, zl.prototype.writeUInt8 = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 1, 255, 0), zl.TYPED_ARRAY_SUPPORT || (e = Math.floor(e)), this[t] = 255 & e, t + 1
-    }, zl.prototype.writeUInt16LE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 2, 65535, 0), zl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8) : vu(this, e, t, !0), t + 2
-    }, zl.prototype.writeUInt16BE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 2, 65535, 0), zl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 8, this[t + 1] = 255 & e) : vu(this, e, t, !1), t + 2
-    }, zl.prototype.writeUInt32LE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 4, 4294967295, 0), zl.TYPED_ARRAY_SUPPORT ? (this[t + 3] = e >>> 24, this[t + 2] = e >>> 16, this[t + 1] = e >>> 8, this[t] = 255 & e) : yu(this, e, t, !0), t + 4
-    }, zl.prototype.writeUInt32BE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 4, 4294967295, 0), zl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e) : yu(this, e, t, !1), t + 4
-    }, zl.prototype.writeIntLE = function(e, t, r, n) {
+    }, Hl.prototype.writeUInt8 = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 1, 255, 0), Hl.TYPED_ARRAY_SUPPORT || (e = Math.floor(e)), this[t] = 255 & e, t + 1
+    }, Hl.prototype.writeUInt16LE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 2, 65535, 0), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8) : yu(this, e, t, !0), t + 2
+    }, Hl.prototype.writeUInt16BE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 2, 65535, 0), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 8, this[t + 1] = 255 & e) : yu(this, e, t, !1), t + 2
+    }, Hl.prototype.writeUInt32LE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 4, 4294967295, 0), Hl.TYPED_ARRAY_SUPPORT ? (this[t + 3] = e >>> 24, this[t + 2] = e >>> 16, this[t + 1] = e >>> 8, this[t] = 255 & e) : bu(this, e, t, !0), t + 4
+    }, Hl.prototype.writeUInt32BE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 4, 4294967295, 0), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e) : bu(this, e, t, !1), t + 4
+    }, Hl.prototype.writeIntLE = function(e, t, r, n) {
         if (e = +e, t |= 0, !n) {
             var i = Math.pow(2, 8 * r - 1);
-            gu(this, e, t, r, i - 1, -i)
+            vu(this, e, t, r, i - 1, -i)
         }
         var o = 0,
             s = 1,
             a = 0;
         for (this[t] = 255 & e; ++o < r && (s *= 256);) e < 0 && 0 === a && 0 !== this[t + o - 1] && (a = 1), this[t + o] = (e / s >> 0) - a & 255;
         return t + r
-    }, zl.prototype.writeIntBE = function(e, t, r, n) {
+    }, Hl.prototype.writeIntBE = function(e, t, r, n) {
         if (e = +e, t |= 0, !n) {
             var i = Math.pow(2, 8 * r - 1);
-            gu(this, e, t, r, i - 1, -i)
+            vu(this, e, t, r, i - 1, -i)
         }
         var o = r - 1,
             s = 1,
             a = 0;
         for (this[t + o] = 255 & e; --o >= 0 && (s *= 256);) e < 0 && 0 === a && 0 !== this[t + o + 1] && (a = 1), this[t + o] = (e / s >> 0) - a & 255;
         return t + r
-    }, zl.prototype.writeInt8 = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 1, 127, -128), zl.TYPED_ARRAY_SUPPORT || (e = Math.floor(e)), e < 0 && (e = 255 + e + 1), this[t] = 255 & e, t + 1
-    }, zl.prototype.writeInt16LE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 2, 32767, -32768), zl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8) : vu(this, e, t, !0), t + 2
-    }, zl.prototype.writeInt16BE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 2, 32767, -32768), zl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 8, this[t + 1] = 255 & e) : vu(this, e, t, !1), t + 2
-    }, zl.prototype.writeInt32LE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 4, 2147483647, -2147483648), zl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8, this[t + 2] = e >>> 16, this[t + 3] = e >>> 24) : yu(this, e, t, !0), t + 4
-    }, zl.prototype.writeInt32BE = function(e, t, r) {
-        return e = +e, t |= 0, r || gu(this, e, t, 4, 2147483647, -2147483648), e < 0 && (e = 4294967295 + e + 1), zl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e) : yu(this, e, t, !1), t + 4
-    }, zl.prototype.writeFloatLE = function(e, t, r) {
-        return wu(this, e, t, !0, r)
-    }, zl.prototype.writeFloatBE = function(e, t, r) {
-        return wu(this, e, t, !1, r)
-    }, zl.prototype.writeDoubleLE = function(e, t, r) {
+    }, Hl.prototype.writeInt8 = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 1, 127, -128), Hl.TYPED_ARRAY_SUPPORT || (e = Math.floor(e)), e < 0 && (e = 255 + e + 1), this[t] = 255 & e, t + 1
+    }, Hl.prototype.writeInt16LE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 2, 32767, -32768), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8) : yu(this, e, t, !0), t + 2
+    }, Hl.prototype.writeInt16BE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 2, 32767, -32768), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 8, this[t + 1] = 255 & e) : yu(this, e, t, !1), t + 2
+    }, Hl.prototype.writeInt32LE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 4, 2147483647, -2147483648), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = 255 & e, this[t + 1] = e >>> 8, this[t + 2] = e >>> 16, this[t + 3] = e >>> 24) : bu(this, e, t, !0), t + 4
+    }, Hl.prototype.writeInt32BE = function(e, t, r) {
+        return e = +e, t |= 0, r || vu(this, e, t, 4, 2147483647, -2147483648), e < 0 && (e = 4294967295 + e + 1), Hl.TYPED_ARRAY_SUPPORT ? (this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e) : bu(this, e, t, !1), t + 4
+    }, Hl.prototype.writeFloatLE = function(e, t, r) {
         return _u(this, e, t, !0, r)
-    }, zl.prototype.writeDoubleBE = function(e, t, r) {
+    }, Hl.prototype.writeFloatBE = function(e, t, r) {
         return _u(this, e, t, !1, r)
-    }, zl.prototype.copy = function(e, t, r, n) {
+    }, Hl.prototype.writeDoubleLE = function(e, t, r) {
+        return ku(this, e, t, !0, r)
+    }, Hl.prototype.writeDoubleBE = function(e, t, r) {
+        return ku(this, e, t, !1, r)
+    }, Hl.prototype.copy = function(e, t, r, n) {
         if (r || (r = 0), n || 0 === n || (n = this.length), t >= e.length && (t = e.length), t || (t = 0), n > 0 && n < r && (n = r), n === r) return 0;
         if (0 === e.length || 0 === this.length) return 0;
         if (t < 0) throw new RangeError("targetStart out of bounds");
         if (r < 0 || r >= this.length) throw new RangeError("sourceStart out of bounds");
         if (n < 0) throw new RangeError("sourceEnd out of bounds");
         n > this.length && (n = this.length), e.length - t < n - r && (n = e.length - t + r);
         var i, o = n - r;
         if (this === e && r < t && t < n)
             for (i = o - 1; i >= 0; --i) e[i + t] = this[i + r];
-        else if (o < 1e3 || !zl.TYPED_ARRAY_SUPPORT)
+        else if (o < 1e3 || !Hl.TYPED_ARRAY_SUPPORT)
             for (i = 0; i < o; ++i) e[i + t] = this[i + r];
         else Uint8Array.prototype.set.call(e, this.subarray(r, r + o), t);
         return o
-    }, zl.prototype.fill = function(e, t, r, n) {
+    }, Hl.prototype.fill = function(e, t, r, n) {
         if ("string" == typeof e) {
             if ("string" == typeof t ? (n = t, t = 0, r = this.length) : "string" == typeof r && (n = r, r = this.length), 1 === e.length) {
                 var i = e.charCodeAt(0);
                 i < 256 && (e = i)
             }
             if (void 0 !== n && "string" != typeof n) throw new TypeError("encoding must be a string");
-            if ("string" == typeof n && !zl.isEncoding(n)) throw new TypeError("Unknown encoding: " + n)
+            if ("string" == typeof n && !Hl.isEncoding(n)) throw new TypeError("Unknown encoding: " + n)
         } else "number" == typeof e && (e &= 255);
         if (t < 0 || this.length < t || this.length < r) throw new RangeError("Out of range index");
         if (r <= t) return this;
         var o;
         if (t >>>= 0, r = void 0 === r ? this.length : r >>> 0, e || (e = 0), "number" == typeof e)
             for (o = t; o < r; ++o) this[o] = e;
         else {
-            var s = Yl(e) ? e : Au(new zl(e, n).toString()),
+            var s = Kl(e) ? e : qu(new Hl(e, n).toString()),
                 a = s.length;
             for (o = 0; o < r - t; ++o) this[o + t] = s[o % a]
         }
         return this
     };
-    var ku = /[^+\/0-9A-Za-z-_]/g;
+    var xu = /[^+\/0-9A-Za-z-_]/g;
 
-    function xu(e) {
+    function Au(e) {
         return e < 16 ? "0" + e.toString(16) : e.toString(16)
     }
 
-    function Au(e, t) {
+    function qu(e, t) {
         var r;
         t = t || 1 / 0;
         for (var n = e.length, i = null, o = [], s = 0; s < n; ++s) {
             if ((r = e.charCodeAt(s)) > 55295 && r < 57344) {
                 if (!i) {
                     if (r > 56319) {
                         (t -= 3) > -1 && o.push(239, 191, 189);
@@ -12330,42 +12350,42 @@
                 if ((t -= 4) < 0) break;
                 o.push(r >> 18 | 240, r >> 12 & 63 | 128, r >> 6 & 63 | 128, 63 & r | 128)
             }
         }
         return o
     }
 
-    function qu(e) {
+    function Eu(e) {
         return function(e) {
             var t, r, n, i, o, s;
-            Rl || Ll();
+            Ll || Nl();
             var a = e.length;
             if (a % 4 > 0) throw new Error("Invalid string. Length must be a multiple of 4");
-            o = "=" === e[a - 2] ? 2 : "=" === e[a - 1] ? 1 : 0, s = new Cl(3 * a / 4 - o), n = o > 0 ? a - 4 : a;
+            o = "=" === e[a - 2] ? 2 : "=" === e[a - 1] ? 1 : 0, s = new Rl(3 * a / 4 - o), n = o > 0 ? a - 4 : a;
             var l = 0;
-            for (t = 0, r = 0; t < n; t += 4, r += 3) i = Dl[e.charCodeAt(t)] << 18 | Dl[e.charCodeAt(t + 1)] << 12 | Dl[e.charCodeAt(t + 2)] << 6 | Dl[e.charCodeAt(t + 3)], s[l++] = i >> 16 & 255, s[l++] = i >> 8 & 255, s[l++] = 255 & i;
-            return 2 === o ? (i = Dl[e.charCodeAt(t)] << 2 | Dl[e.charCodeAt(t + 1)] >> 4, s[l++] = 255 & i) : 1 === o && (i = Dl[e.charCodeAt(t)] << 10 | Dl[e.charCodeAt(t + 1)] << 4 | Dl[e.charCodeAt(t + 2)] >> 2, s[l++] = i >> 8 & 255, s[l++] = 255 & i), s
+            for (t = 0, r = 0; t < n; t += 4, r += 3) i = Cl[e.charCodeAt(t)] << 18 | Cl[e.charCodeAt(t + 1)] << 12 | Cl[e.charCodeAt(t + 2)] << 6 | Cl[e.charCodeAt(t + 3)], s[l++] = i >> 16 & 255, s[l++] = i >> 8 & 255, s[l++] = 255 & i;
+            return 2 === o ? (i = Cl[e.charCodeAt(t)] << 2 | Cl[e.charCodeAt(t + 1)] >> 4, s[l++] = 255 & i) : 1 === o && (i = Cl[e.charCodeAt(t)] << 10 | Cl[e.charCodeAt(t + 1)] << 4 | Cl[e.charCodeAt(t + 2)] >> 2, s[l++] = i >> 8 & 255, s[l++] = 255 & i), s
         }(function(e) {
             if ((e = function(e) {
                     return e.trim ? e.trim() : e.replace(/^\s+|\s+$/g, "")
-                }(e).replace(ku, "")).length < 2) return "";
+                }(e).replace(xu, "")).length < 2) return "";
             for (; e.length % 4 != 0;) e += "=";
             return e
         }(e))
     }
 
-    function Eu(e, t, r, n) {
+    function Tu(e, t, r, n) {
         for (var i = 0; i < n && !(i + r >= t.length || i >= e.length); ++i) t[i + r] = e[i];
         return i
     }
 
-    function Tu(e) {
+    function $u(e) {
         return !!e.constructor && "function" == typeof e.constructor.isBuffer && e.constructor.isBuffer(e)
     }
-    var $u = function(e) {
+    var Ou = function(e) {
         return (e = e || {}).circles ? function(e) {
             var t = [],
                 r = [];
             return e.proto ? function e(i) {
                 if ("object" != typeof i || null === i) return i;
                 if (i instanceof Date) return new Date(i);
                 if (Array.isArray(i)) return n(i, e);
@@ -12374,15 +12394,15 @@
                 var o = {};
                 for (var s in t.push(i), r.push(o), i) {
                     var a = i[s];
                     if ("object" != typeof a || null === a) o[s] = a;
                     else if (a instanceof Date) o[s] = new Date(a);
                     else if (a instanceof Map) o[s] = new Map(n(Array.from(a), e));
                     else if (a instanceof Set) o[s] = new Set(n(Array.from(a), e));
-                    else if (ArrayBuffer.isView(a)) o[s] = Ou(a);
+                    else if (ArrayBuffer.isView(a)) o[s] = Su(a);
                     else {
                         var l = t.indexOf(a);
                         o[s] = -1 !== l ? r[l] : e(a)
                     }
                 }
                 return t.pop(), r.pop(), o
             } : function e(i) {
@@ -12395,29 +12415,29 @@
                 for (var s in t.push(i), r.push(o), i)
                     if (!1 !== Object.hasOwnProperty.call(i, s)) {
                         var a = i[s];
                         if ("object" != typeof a || null === a) o[s] = a;
                         else if (a instanceof Date) o[s] = new Date(a);
                         else if (a instanceof Map) o[s] = new Map(n(Array.from(a), e));
                         else if (a instanceof Set) o[s] = new Set(n(Array.from(a), e));
-                        else if (ArrayBuffer.isView(a)) o[s] = Ou(a);
+                        else if (ArrayBuffer.isView(a)) o[s] = Su(a);
                         else {
                             var l = t.indexOf(a);
                             o[s] = -1 !== l ? r[l] : e(a)
                         }
                     } return t.pop(), r.pop(), o
             };
 
             function n(e, n) {
                 for (var i = Object.keys(e), o = new Array(i.length), s = 0; s < i.length; s++) {
                     var a = i[s],
                         l = e[a];
                     if ("object" != typeof l || null === l) o[a] = l;
                     else if (l instanceof Date) o[a] = new Date(l);
-                    else if (ArrayBuffer.isView(l)) o[a] = Ou(l);
+                    else if (ArrayBuffer.isView(l)) o[a] = Su(l);
                     else {
                         var u = t.indexOf(l);
                         o[a] = -1 !== u ? r[u] : n(l)
                     }
                 }
                 return o
             }
@@ -12426,433 +12446,433 @@
             if (r instanceof Date) return new Date(r);
             if (Array.isArray(r)) return t(r, e);
             if (r instanceof Map) return new Map(t(Array.from(r), e));
             if (r instanceof Set) return new Set(t(Array.from(r), e));
             var n = {};
             for (var i in r) {
                 var o = r[i];
-                "object" != typeof o || null === o ? n[i] = o : o instanceof Date ? n[i] = new Date(o) : o instanceof Map ? n[i] = new Map(t(Array.from(o), e)) : o instanceof Set ? n[i] = new Set(t(Array.from(o), e)) : ArrayBuffer.isView(o) ? n[i] = Ou(o) : n[i] = e(o)
+                "object" != typeof o || null === o ? n[i] = o : o instanceof Date ? n[i] = new Date(o) : o instanceof Map ? n[i] = new Map(t(Array.from(o), e)) : o instanceof Set ? n[i] = new Set(t(Array.from(o), e)) : ArrayBuffer.isView(o) ? n[i] = Su(o) : n[i] = e(o)
             }
             return n
         } : r;
 
         function t(e, t) {
             for (var r = Object.keys(e), n = new Array(r.length), i = 0; i < r.length; i++) {
                 var o = r[i],
                     s = e[o];
-                "object" != typeof s || null === s ? n[o] = s : s instanceof Date ? n[o] = new Date(s) : ArrayBuffer.isView(s) ? n[o] = Ou(s) : n[o] = t(s)
+                "object" != typeof s || null === s ? n[o] = s : s instanceof Date ? n[o] = new Date(s) : ArrayBuffer.isView(s) ? n[o] = Su(s) : n[o] = t(s)
             }
             return n
         }
 
         function r(e) {
             if ("object" != typeof e || null === e) return e;
             if (e instanceof Date) return new Date(e);
             if (Array.isArray(e)) return t(e, r);
             if (e instanceof Map) return new Map(t(Array.from(e), r));
             if (e instanceof Set) return new Set(t(Array.from(e), r));
             var n = {};
             for (var i in e)
                 if (!1 !== Object.hasOwnProperty.call(e, i)) {
                     var o = e[i];
-                    "object" != typeof o || null === o ? n[i] = o : o instanceof Date ? n[i] = new Date(o) : o instanceof Map ? n[i] = new Map(t(Array.from(o), r)) : o instanceof Set ? n[i] = new Set(t(Array.from(o), r)) : ArrayBuffer.isView(o) ? n[i] = Ou(o) : n[i] = r(o)
+                    "object" != typeof o || null === o ? n[i] = o : o instanceof Date ? n[i] = new Date(o) : o instanceof Map ? n[i] = new Map(t(Array.from(o), r)) : o instanceof Set ? n[i] = new Set(t(Array.from(o), r)) : ArrayBuffer.isView(o) ? n[i] = Su(o) : n[i] = r(o)
                 } return n
         }
     };
 
-    function Ou(e) {
-        return e instanceof zl ? zl.from(e) : new e.constructor(e.buffer.slice(), e.byteOffset, e.length)
+    function Su(e) {
+        return e instanceof Hl ? Hl.from(e) : new e.constructor(e.buffer.slice(), e.byteOffset, e.length)
     }
-    var Su = it($u);
+    var Du = st(Ou);
     /**
      * @name codsen-utils
      * @fileoverview Various utility functions
      * @version 1.6.0
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/codsen-utils/}
      */
-    function Du(e) {
+    function Cu(e) {
         if (null == e || "object" != typeof e) return !1;
         let t = Object.getPrototypeOf(e);
         return (null === t || t === Object.prototype || null === Object.getPrototypeOf(t)) && (!(Symbol.iterator in e) && !(Symbol.toStringTag in e))
     }
 
-    function Cu(e) {
+    function Ru(e) {
         return "string" == typeof e
     }
 
-    function Ru(e) {
+    function Lu(e) {
         return Number.isSafeInteger(e) && e >= 0
     }
 
-    function Lu(e) {
+    function Nu(e) {
         return null != e
     }
 
-    function Nu(e, t) {
-        return Du(e) && Cu(t) && t in e
+    function Iu(e, t) {
+        return Cu(e) && Ru(t) && t in e
     }
-    Su();
-    var Iu = "object" == typeof pr && pr && pr.Object === Object && pr,
-        Fu = "object" == typeof self && self && self.Object === Object && self,
-        Mu = Iu || Fu || Function("return this")(),
-        Pu = Mu.Symbol,
-        ju = Object.prototype,
-        Bu = ju.hasOwnProperty,
-        Uu = ju.toString,
-        Vu = Pu ? Pu.toStringTag : void 0;
-    var zu = Object.prototype.toString;
-    var Hu = "[object Null]",
-        Wu = "[object Undefined]",
-        Gu = Pu ? Pu.toStringTag : void 0;
-
-    function Zu(e) {
-        return null == e ? void 0 === e ? Wu : Hu : Gu && Gu in Object(e) ? function(e) {
-            var t = Bu.call(e, Vu),
-                r = e[Vu];
+    Du();
+    var Fu = "object" == typeof A && A && A.Object === Object && A,
+        Mu = "object" == typeof self && self && self.Object === Object && self,
+        Pu = Fu || Mu || Function("return this")(),
+        ju = Pu.Symbol,
+        Bu = Object.prototype,
+        Uu = Bu.hasOwnProperty,
+        Vu = Bu.toString,
+        zu = ju ? ju.toStringTag : void 0;
+    var Hu = Object.prototype.toString;
+    var Wu = "[object Null]",
+        Gu = "[object Undefined]",
+        Zu = ju ? ju.toStringTag : void 0;
+
+    function Ju(e) {
+        return null == e ? void 0 === e ? Gu : Wu : Zu && Zu in Object(e) ? function(e) {
+            var t = Uu.call(e, zu),
+                r = e[zu];
             try {
-                e[Vu] = void 0;
+                e[zu] = void 0;
                 var n = !0
             } catch (e) {}
-            var i = Uu.call(e);
-            return n && (t ? e[Vu] = r : delete e[Vu]), i
+            var i = Vu.call(e);
+            return n && (t ? e[zu] = r : delete e[zu]), i
         }(e) : function(e) {
-            return zu.call(e)
+            return Hu.call(e)
         }(e)
     }
 
-    function Ju(e) {
+    function Yu(e) {
         return null != e && "object" == typeof e
     }
-    var Yu = "[object Symbol]";
+    var Ku = "[object Symbol]";
 
-    function Ku(e, t) {
+    function Xu(e, t) {
         for (var r = -1, n = null == e ? 0 : e.length, i = Array(n); ++r < n;) i[r] = t(e[r], r, e);
         return i
     }
-    var Xu = Array.isArray,
-        Qu = 1 / 0,
-        ec = Pu ? Pu.prototype : void 0,
-        tc = ec ? ec.toString : void 0;
+    var Qu = Array.isArray,
+        ec = 1 / 0,
+        tc = ju ? ju.prototype : void 0,
+        rc = tc ? tc.toString : void 0;
 
-    function rc(e) {
+    function nc(e) {
         if ("string" == typeof e) return e;
-        if (Xu(e)) return Ku(e, rc) + "";
+        if (Qu(e)) return Xu(e, nc) + "";
         if (function(e) {
-                return "symbol" == typeof e || Ju(e) && Zu(e) == Yu
-            }(e)) return tc ? tc.call(e) : "";
+                return "symbol" == typeof e || Yu(e) && Ju(e) == Ku
+            }(e)) return rc ? rc.call(e) : "";
         var t = e + "";
-        return "0" == t && 1 / e == -Qu ? "-0" : t
+        return "0" == t && 1 / e == -ec ? "-0" : t
     }
-    var nc = /\s/;
-    var ic = /^\s+/;
+    var ic = /\s/;
+    var oc = /^\s+/;
 
-    function oc(e) {
+    function sc(e) {
         return e ? e.slice(0, function(e) {
-            for (var t = e.length; t-- && nc.test(e.charAt(t)););
+            for (var t = e.length; t-- && ic.test(e.charAt(t)););
             return t
-        }(e) + 1).replace(ic, "") : e
+        }(e) + 1).replace(oc, "") : e
     }
 
-    function sc(e) {
+    function ac(e) {
         var t = typeof e;
         return null != e && ("object" == t || "function" == t)
     }
 
-    function ac(e) {
+    function lc(e) {
         return e
     }
-    var lc = "[object AsyncFunction]",
-        uc = "[object Function]",
-        cc = "[object GeneratorFunction]",
-        fc = "[object Proxy]";
-
-    function hc(e) {
-        if (!sc(e)) return !1;
-        var t = Zu(e);
-        return t == uc || t == cc || t == lc || t == fc
-    }
-    var pc, dc = Mu["__core-js_shared__"],
-        mc = (pc = /[^.]+$/.exec(dc && dc.keys && dc.keys.IE_PROTO || "")) ? "Symbol(src)_1." + pc : "";
-    var gc = Function.prototype.toString;
-    var vc = /^\[object .+?Constructor\]$/,
-        yc = Function.prototype,
-        bc = Object.prototype,
-        wc = yc.toString,
-        _c = bc.hasOwnProperty,
-        kc = RegExp("^" + wc.call(_c).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
-
-    function xc(e) {
-        return !(!sc(e) || function(e) {
-            return !!mc && mc in e
-        }(e)) && (hc(e) ? kc : vc).test(function(e) {
+    var uc = "[object AsyncFunction]",
+        cc = "[object Function]",
+        fc = "[object GeneratorFunction]",
+        hc = "[object Proxy]";
+
+    function pc(e) {
+        if (!ac(e)) return !1;
+        var t = Ju(e);
+        return t == cc || t == fc || t == uc || t == hc
+    }
+    var dc, mc = Pu["__core-js_shared__"],
+        gc = (dc = /[^.]+$/.exec(mc && mc.keys && mc.keys.IE_PROTO || "")) ? "Symbol(src)_1." + dc : "";
+    var vc = Function.prototype.toString;
+    var yc = /^\[object .+?Constructor\]$/,
+        bc = Function.prototype,
+        wc = Object.prototype,
+        _c = bc.toString,
+        kc = wc.hasOwnProperty,
+        xc = RegExp("^" + _c.call(kc).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
+
+    function Ac(e) {
+        return !(!ac(e) || function(e) {
+            return !!gc && gc in e
+        }(e)) && (pc(e) ? xc : yc).test(function(e) {
             if (null != e) {
                 try {
-                    return gc.call(e)
+                    return vc.call(e)
                 } catch (e) {}
                 try {
                     return e + ""
                 } catch (e) {}
             }
             return ""
         }(e))
     }
 
-    function Ac(e, t) {
+    function qc(e, t) {
         var r = function(e, t) {
             return null == e ? void 0 : e[t]
         }(e, t);
-        return xc(r) ? r : void 0
+        return Ac(r) ? r : void 0
     }
-    var qc = Date.now;
+    var Ec = Date.now;
 
-    function Ec(e) {
+    function Tc(e) {
         return function() {
             return e
         }
     }
-    var Tc = function() {
+    var $c = function() {
             try {
-                var e = Ac(Object, "defineProperty");
+                var e = qc(Object, "defineProperty");
                 return e({}, "", {}), e
             } catch (e) {}
         }(),
-        $c = Tc,
-        Oc = $c ? function(e, t) {
-            return $c(e, "toString", {
+        Oc = $c,
+        Sc = Oc ? function(e, t) {
+            return Oc(e, "toString", {
                 configurable: !0,
                 enumerable: !1,
-                value: Ec(t),
+                value: Tc(t),
                 writable: !0
             })
-        } : ac,
-        Sc = function(e) {
+        } : lc,
+        Dc = function(e) {
             var t = 0,
                 r = 0;
             return function() {
-                var n = qc(),
+                var n = Ec(),
                     i = 16 - (n - r);
                 if (r = n, i > 0) {
                     if (++t >= 800) return arguments[0]
                 } else t = 0;
                 return e.apply(void 0, arguments)
             }
-        }(Oc),
-        Dc = Sc;
+        }(Sc),
+        Cc = Dc;
 
-    function Cc(e) {
+    function Rc(e) {
         return e != e
     }
 
-    function Rc(e, t, r) {
+    function Lc(e, t, r) {
         return t == t ? function(e, t, r) {
             for (var n = r - 1, i = e.length; ++n < i;)
                 if (e[n] === t) return n;
             return -1
         }(e, t, r) : function(e, t, r, n) {
             for (var i = e.length, o = r + (n ? 1 : -1); n ? o-- : ++o < i;)
                 if (t(e[o], o, e)) return o;
             return -1
-        }(e, Cc, r)
+        }(e, Rc, r)
     }
 
-    function Lc(e, t) {
-        return !!(null == e ? 0 : e.length) && Rc(e, t, 0) > -1
+    function Nc(e, t) {
+        return !!(null == e ? 0 : e.length) && Lc(e, t, 0) > -1
     }
 
-    function Nc(e, t) {
+    function Ic(e, t) {
         return e === t || e != e && t != t
     }
-    var Ic = Math.max;
-    var Fc = 9007199254740991;
+    var Fc = Math.max;
+    var Mc = 9007199254740991;
 
-    function Mc(e) {
+    function Pc(e) {
         return null != e && function(e) {
-            return "number" == typeof e && e > -1 && e % 1 == 0 && e <= Fc
-        }(e.length) && !hc(e)
+            return "number" == typeof e && e > -1 && e % 1 == 0 && e <= Mc
+        }(e.length) && !pc(e)
     }
-    var Pc = Ac(Object, "create");
-    var jc = Object.prototype.hasOwnProperty;
+    var jc = qc(Object, "create");
     var Bc = Object.prototype.hasOwnProperty;
+    var Uc = Object.prototype.hasOwnProperty;
 
-    function Uc(e) {
+    function Vc(e) {
         var t = -1,
             r = null == e ? 0 : e.length;
         for (this.clear(); ++t < r;) {
             var n = e[t];
             this.set(n[0], n[1])
         }
     }
 
-    function Vc(e, t) {
+    function zc(e, t) {
         for (var r = e.length; r--;)
-            if (Nc(e[r][0], t)) return r;
+            if (Ic(e[r][0], t)) return r;
         return -1
     }
-    Uc.prototype.clear = function() {
-        this.__data__ = Pc ? Pc(null) : {}, this.size = 0
-    }, Uc.prototype.delete = function(e) {
+    Vc.prototype.clear = function() {
+        this.__data__ = jc ? jc(null) : {}, this.size = 0
+    }, Vc.prototype.delete = function(e) {
         var t = this.has(e) && delete this.__data__[e];
         return this.size -= t ? 1 : 0, t
-    }, Uc.prototype.get = function(e) {
+    }, Vc.prototype.get = function(e) {
         var t = this.__data__;
-        if (Pc) {
+        if (jc) {
             var r = t[e];
             return "__lodash_hash_undefined__" === r ? void 0 : r
         }
-        return jc.call(t, e) ? t[e] : void 0
-    }, Uc.prototype.has = function(e) {
+        return Bc.call(t, e) ? t[e] : void 0
+    }, Vc.prototype.has = function(e) {
         var t = this.__data__;
-        return Pc ? void 0 !== t[e] : Bc.call(t, e)
-    }, Uc.prototype.set = function(e, t) {
+        return jc ? void 0 !== t[e] : Uc.call(t, e)
+    }, Vc.prototype.set = function(e, t) {
         var r = this.__data__;
-        return this.size += this.has(e) ? 0 : 1, r[e] = Pc && void 0 === t ? "__lodash_hash_undefined__" : t, this
+        return this.size += this.has(e) ? 0 : 1, r[e] = jc && void 0 === t ? "__lodash_hash_undefined__" : t, this
     };
-    var zc = Array.prototype.splice;
+    var Hc = Array.prototype.splice;
 
-    function Hc(e) {
+    function Wc(e) {
         var t = -1,
             r = null == e ? 0 : e.length;
         for (this.clear(); ++t < r;) {
             var n = e[t];
             this.set(n[0], n[1])
         }
     }
-    Hc.prototype.clear = function() {
+    Wc.prototype.clear = function() {
         this.__data__ = [], this.size = 0
-    }, Hc.prototype.delete = function(e) {
+    }, Wc.prototype.delete = function(e) {
         var t = this.__data__,
-            r = Vc(t, e);
-        return !(r < 0) && (r == t.length - 1 ? t.pop() : zc.call(t, r, 1), --this.size, !0)
-    }, Hc.prototype.get = function(e) {
+            r = zc(t, e);
+        return !(r < 0) && (r == t.length - 1 ? t.pop() : Hc.call(t, r, 1), --this.size, !0)
+    }, Wc.prototype.get = function(e) {
         var t = this.__data__,
-            r = Vc(t, e);
+            r = zc(t, e);
         return r < 0 ? void 0 : t[r][1]
-    }, Hc.prototype.has = function(e) {
-        return Vc(this.__data__, e) > -1
-    }, Hc.prototype.set = function(e, t) {
+    }, Wc.prototype.has = function(e) {
+        return zc(this.__data__, e) > -1
+    }, Wc.prototype.set = function(e, t) {
         var r = this.__data__,
-            n = Vc(r, e);
+            n = zc(r, e);
         return n < 0 ? (++this.size, r.push([e, t])) : r[n][1] = t, this
     };
-    var Wc = Ac(Mu, "Map");
+    var Gc = qc(Pu, "Map");
 
-    function Gc(e, t) {
+    function Zc(e, t) {
         var r = e.__data__;
         return function(e) {
             var t = typeof e;
             return "string" == t || "number" == t || "symbol" == t || "boolean" == t ? "__proto__" !== e : null === e
         }(t) ? r["string" == typeof t ? "string" : "hash"] : r.map
     }
 
-    function Zc(e) {
+    function Jc(e) {
         var t = -1,
             r = null == e ? 0 : e.length;
         for (this.clear(); ++t < r;) {
             var n = e[t];
             this.set(n[0], n[1])
         }
     }
 
-    function Jc(e, t, r) {
+    function Yc(e, t, r) {
         var n = e.length;
         return r = void 0 === r ? n : r, !t && r >= n ? e : function(e, t, r) {
             var n = -1,
                 i = e.length;
             t < 0 && (t = -t > i ? 0 : i + t), (r = r > i ? i : r) < 0 && (r += i), i = t > r ? 0 : r - t >>> 0, t >>>= 0;
             for (var o = Array(i); ++n < i;) o[n] = e[n + t];
             return o
         }(e, t, r)
     }
-    Zc.prototype.clear = function() {
+    Jc.prototype.clear = function() {
         this.size = 0, this.__data__ = {
-            hash: new Uc,
-            map: new(Wc || Hc),
-            string: new Uc
+            hash: new Vc,
+            map: new(Gc || Wc),
+            string: new Vc
         }
-    }, Zc.prototype.delete = function(e) {
-        var t = Gc(this, e).delete(e);
+    }, Jc.prototype.delete = function(e) {
+        var t = Zc(this, e).delete(e);
         return this.size -= t ? 1 : 0, t
-    }, Zc.prototype.get = function(e) {
-        return Gc(this, e).get(e)
-    }, Zc.prototype.has = function(e) {
-        return Gc(this, e).has(e)
-    }, Zc.prototype.set = function(e, t) {
-        var r = Gc(this, e),
+    }, Jc.prototype.get = function(e) {
+        return Zc(this, e).get(e)
+    }, Jc.prototype.has = function(e) {
+        return Zc(this, e).has(e)
+    }, Jc.prototype.set = function(e, t) {
+        var r = Zc(this, e),
             n = r.size;
         return r.set(e, t), this.size += r.size == n ? 0 : 1, this
     };
-    var Yc = RegExp("[\\u200d\\ud800-\\udfff\\u0300-\\u036f\\ufe20-\\ufe2f\\u20d0-\\u20ff\\ufe0e\\ufe0f]");
-    var Kc = "\\ud800-\\udfff",
-        Xc = "[" + Kc + "]",
-        Qc = "[\\u0300-\\u036f\\ufe20-\\ufe2f\\u20d0-\\u20ff]",
-        ef = "\\ud83c[\\udffb-\\udfff]",
-        tf = "[^" + Kc + "]",
-        rf = "(?:\\ud83c[\\udde6-\\uddff]){2}",
-        nf = "[\\ud800-\\udbff][\\udc00-\\udfff]",
-        of = "(?:" + Qc + "|" + ef + ")" + "?",
-        sf = "[\\ufe0e\\ufe0f]?",
-        af = sf + of + ("(?:\\u200d(?:" + [tf, rf, nf].join("|") + ")" + sf + of + ")*"),
-        lf = "(?:" + [tf + Qc + "?", Qc, rf, nf, Xc].join("|") + ")",
-        uf = RegExp(ef + "(?=" + ef + ")|" + lf + af, "g");
+    var Kc = RegExp("[\\u200d\\ud800-\\udfff\\u0300-\\u036f\\ufe20-\\ufe2f\\u20d0-\\u20ff\\ufe0e\\ufe0f]");
+    var Xc = "\\ud800-\\udfff",
+        Qc = "[" + Xc + "]",
+        ef = "[\\u0300-\\u036f\\ufe20-\\ufe2f\\u20d0-\\u20ff]",
+        tf = "\\ud83c[\\udffb-\\udfff]",
+        rf = "[^" + Xc + "]",
+        nf = "(?:\\ud83c[\\udde6-\\uddff]){2}",
+        of = "[\\ud800-\\udbff][\\udc00-\\udfff]",
+        sf = "(?:" + ef + "|" + tf + ")" + "?",
+        af = "[\\ufe0e\\ufe0f]?",
+        lf = af + sf + ("(?:\\u200d(?:" + [rf, nf, of].join("|") + ")" + af + sf + ")*"),
+        uf = "(?:" + [rf + ef + "?", ef, nf, of, Qc].join("|") + ")",
+        cf = RegExp(tf + "(?=" + tf + ")|" + uf + lf, "g");
 
-    function cf(e) {
+    function ff(e) {
         return function(e) {
-            return Yc.test(e)
+            return Kc.test(e)
         }(e) ? function(e) {
-            return e.match(uf) || []
+            return e.match(cf) || []
         }(e) : function(e) {
             return e.split("")
         }(e)
     }
 
-    function ff(e) {
+    function hf(e) {
         var t = -1,
             r = null == e ? 0 : e.length;
-        for (this.__data__ = new Zc; ++t < r;) this.add(e[t])
+        for (this.__data__ = new Jc; ++t < r;) this.add(e[t])
     }
 
-    function hf(e, t) {
+    function pf(e, t) {
         return e.has(t)
     }
 
-    function pf(e, t, r) {
+    function df(e, t, r) {
         for (var n = -1, i = null == e ? 0 : e.length; ++n < i;)
             if (r(t, e[n])) return !0;
         return !1
     }
-    ff.prototype.add = ff.prototype.push = function(e) {
+    hf.prototype.add = hf.prototype.push = function(e) {
         return this.__data__.set(e, "__lodash_hash_undefined__"), this
-    }, ff.prototype.has = function(e) {
+    }, hf.prototype.has = function(e) {
         return this.__data__.has(e)
     };
 
-    function df(e, t, r) {
+    function mf(e, t, r) {
         if (e = function(e) {
-                return null == e ? "" : rc(e)
-            }(e), e && (r || void 0 === t)) return oc(e);
-        if (!e || !(t = rc(t))) return e;
-        var n = cf(e),
-            i = cf(t),
+                return null == e ? "" : nc(e)
+            }(e), e && (r || void 0 === t)) return sc(e);
+        if (!e || !(t = nc(t))) return e;
+        var n = ff(e),
+            i = ff(t),
             o = function(e, t) {
-                for (var r = -1, n = e.length; ++r < n && Rc(t, e[r], 0) > -1;);
+                for (var r = -1, n = e.length; ++r < n && Lc(t, e[r], 0) > -1;);
                 return r
             }(n, i),
             s = function(e, t) {
-                for (var r = e.length; r-- && Rc(t, e[r], 0) > -1;);
+                for (var r = e.length; r-- && Lc(t, e[r], 0) > -1;);
                 return r
             }(n, i) + 1;
-        return Jc(n, o, s).join("")
+        return Yc(n, o, s).join("")
     }
-    var mf = function(e, t) {
-            return Dc(function(e, t, r) {
-                return t = Ic(void 0 === t ? e.length - 1 : t, 0),
+    var gf = function(e, t) {
+            return Cc(function(e, t, r) {
+                return t = Fc(void 0 === t ? e.length - 1 : t, 0),
                     function() {
-                        for (var n = arguments, i = -1, o = Ic(n.length - t, 0), s = Array(o); ++i < o;) s[i] = n[t + i];
+                        for (var n = arguments, i = -1, o = Fc(n.length - t, 0), s = Array(o); ++i < o;) s[i] = n[t + i];
                         i = -1;
                         for (var a = Array(t + 1); ++i < t;) a[i] = n[i];
                         return a[t] = r(s),
                             function(e, t, r) {
                                 switch (r.length) {
                                     case 0:
                                         return e.call(t);
@@ -12862,53 +12882,53 @@
                                         return e.call(t, r[0], r[1]);
                                     case 3:
                                         return e.call(t, r[0], r[1], r[2])
                                 }
                                 return e.apply(t, r)
                             }(e, this, a)
                     }
-            }(e, t, ac), e + "")
+            }(e, t, lc), e + "")
         }((function(e, t) {
             return function(e) {
-                return Ju(e) && Mc(e)
+                return Yu(e) && Pc(e)
             }(e) ? function(e, t, r, n) {
                 var i = -1,
-                    o = Lc,
+                    o = Nc,
                     s = !0,
                     a = e.length,
                     l = [],
                     u = t.length;
                 if (!a) return l;
-                r && (t = Ku(t, function(e) {
+                r && (t = Xu(t, function(e) {
                     return function(t) {
                         return e(t)
                     }
-                }(r))), n ? (o = pf, s = !1) : t.length >= 200 && (o = hf, s = !1, t = new ff(t));
+                }(r))), n ? (o = df, s = !1) : t.length >= 200 && (o = pf, s = !1, t = new hf(t));
                 e: for (; ++i < a;) {
                     var c = e[i],
                         f = null == r ? c : r(c);
                     if (c = n || 0 !== c ? c : 0, s && f == f) {
                         for (var h = u; h--;)
                             if (t[h] === f) continue e;
                         l.push(c)
                     } else o(t, f, n) || l.push(c)
                 }
                 return l
             }(e, t) : []
         })),
-        gf = mf,
-        vf = {},
-        yf = {};
-    Object.defineProperty(yf, "__esModule", {
+        vf = gf,
+        yf = {},
+        bf = {};
+    Object.defineProperty(bf, "__esModule", {
         value: !0
-    }), yf.bodyRegExps = {
+    }), bf.bodyRegExps = {
         xml: /&(?:#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+);?/g,
         html4: /&(?:nbsp|iexcl|cent|pound|curren|yen|brvbar|sect|uml|copy|ordf|laquo|not|shy|reg|macr|deg|plusmn|sup2|sup3|acute|micro|para|middot|cedil|sup1|ordm|raquo|frac14|frac12|frac34|iquest|Agrave|Aacute|Acirc|Atilde|Auml|Aring|AElig|Ccedil|Egrave|Eacute|Ecirc|Euml|Igrave|Iacute|Icirc|Iuml|ETH|Ntilde|Ograve|Oacute|Ocirc|Otilde|Ouml|times|Oslash|Ugrave|Uacute|Ucirc|Uuml|Yacute|THORN|szlig|agrave|aacute|acirc|atilde|auml|aring|aelig|ccedil|egrave|eacute|ecirc|euml|igrave|iacute|icirc|iuml|eth|ntilde|ograve|oacute|ocirc|otilde|ouml|divide|oslash|ugrave|uacute|ucirc|uuml|yacute|thorn|yuml|quot|amp|lt|gt|#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+);?/g,
         html5: /&(?:AElig|AMP|Aacute|Acirc|Agrave|Aring|Atilde|Auml|COPY|Ccedil|ETH|Eacute|Ecirc|Egrave|Euml|GT|Iacute|Icirc|Igrave|Iuml|LT|Ntilde|Oacute|Ocirc|Ograve|Oslash|Otilde|Ouml|QUOT|REG|THORN|Uacute|Ucirc|Ugrave|Uuml|Yacute|aacute|acirc|acute|aelig|agrave|amp|aring|atilde|auml|brvbar|ccedil|cedil|cent|copy|curren|deg|divide|eacute|ecirc|egrave|eth|euml|frac12|frac14|frac34|gt|iacute|icirc|iexcl|igrave|iquest|iuml|laquo|lt|macr|micro|middot|nbsp|not|ntilde|oacute|ocirc|ograve|ordf|ordm|oslash|otilde|ouml|para|plusmn|pound|quot|raquo|reg|sect|shy|sup1|sup2|sup3|szlig|thorn|times|uacute|ucirc|ugrave|uml|uuml|yacute|yen|yuml|#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+);?/g
-    }, yf.namedReferences = {
+    }, bf.namedReferences = {
         xml: {
             entities: {
                 "&lt;": "<",
                 "&gt;": ">",
                 "&quot;": '"',
                 "&apos;": "'",
                 "&amp;": "&"
@@ -17278,18 +17298,18 @@
                 "𝕫": "&zopf;",
                 "𝓏": "&zscr;",
                 "‍": "&zwj;",
                 "‌": "&zwnj;"
             }
         }
     };
-    var bf = {};
-    Object.defineProperty(bf, "__esModule", {
+    var wf = {};
+    Object.defineProperty(wf, "__esModule", {
         value: !0
-    }), bf.numericUnicodeMap = {
+    }), wf.numericUnicodeMap = {
         0: 65533,
         128: 8364,
         130: 8218,
         131: 402,
         132: 8222,
         133: 8230,
         134: 8224,
@@ -17311,129 +17331,129 @@
         153: 8482,
         154: 353,
         155: 8250,
         156: 339,
         158: 382,
         159: 376
     };
-    var wf = {};
-    Object.defineProperty(wf, "__esModule", {
+    var _f = {};
+    Object.defineProperty(_f, "__esModule", {
         value: !0
-    }), wf.fromCodePoint = String.fromCodePoint || function(e) {
+    }), _f.fromCodePoint = String.fromCodePoint || function(e) {
         return String.fromCharCode(Math.floor((e - 65536) / 1024) + 55296, (e - 65536) % 1024 + 56320)
-    }, wf.getCodePoint = String.prototype.codePointAt ? function(e, t) {
+    }, _f.getCodePoint = String.prototype.codePointAt ? function(e, t) {
         return e.codePointAt(t)
     } : function(e, t) {
         return 1024 * (e.charCodeAt(t) - 55296) + e.charCodeAt(t + 1) - 56320 + 65536
-    }, wf.highSurrogateFrom = 55296, wf.highSurrogateTo = 56319;
-    var _f = nt && nt.__assign || function() {
-        return _f = Object.assign || function(e) {
+    }, _f.highSurrogateFrom = 55296, _f.highSurrogateTo = 56319;
+    var kf = ot && ot.__assign || function() {
+        return kf = Object.assign || function(e) {
             for (var t, r = 1, n = arguments.length; r < n; r++)
                 for (var i in t = arguments[r]) Object.prototype.hasOwnProperty.call(t, i) && (e[i] = t[i]);
             return e
-        }, _f.apply(this, arguments)
+        }, kf.apply(this, arguments)
     };
-    Object.defineProperty(vf, "__esModule", {
+    Object.defineProperty(yf, "__esModule", {
         value: !0
     });
-    var kf = yf,
-        xf = bf,
+    var xf = bf,
         Af = wf,
-        qf = _f(_f({}, kf.namedReferences), {
-            all: kf.namedReferences.html5
+        qf = _f,
+        Ef = kf(kf({}, xf.namedReferences), {
+            all: xf.namedReferences.html5
         }),
-        Ef = {
+        Tf = {
             specialChars: /[<>'"&]/g,
             nonAscii: /(?:[<>'"&\u0080-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])/g,
             nonAsciiPrintable: /(?:[<>'"&\x01-\x08\x11-\x15\x17-\x1F\x7f-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])/g,
             extensive: /(?:[\x01-\x0c\x0e-\x1f\x21-\x2c\x2e-\x2f\x3a-\x40\x5b-\x60\x7b-\x7d\x7f-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])/g
         },
-        Tf = {
+        $f = {
             mode: "specialChars",
             level: "all",
             numeric: "decimal"
         };
-    vf.encode = function(e, t) {
-        var r = void 0 === (s = (o = void 0 === t ? Tf : t).mode) ? "specialChars" : s,
+    yf.encode = function(e, t) {
+        var r = void 0 === (s = (o = void 0 === t ? $f : t).mode) ? "specialChars" : s,
             n = void 0 === (c = o.numeric) ? "decimal" : c,
             i = o.level;
         if (!e) return "";
-        var o, s, a = Ef[r],
-            l = qf[void 0 === i ? "all" : i].characters,
+        var o, s, a = Tf[r],
+            l = Ef[void 0 === i ? "all" : i].characters,
             u = "hexadecimal" === n;
         if (a.lastIndex = 0, o = a.exec(e)) {
             s = "";
             var c = 0;
             do {
                 c !== o.index && (s += e.substring(c, o.index));
                 var f = l[i = o[0]];
                 if (!f) {
-                    var h = i.length > 1 ? Af.getCodePoint(i, 0) : i.charCodeAt(0);
+                    var h = i.length > 1 ? qf.getCodePoint(i, 0) : i.charCodeAt(0);
                     f = (u ? "&#x" + h.toString(16) : "&#" + h) + ";"
                 }
                 s += f, c = o.index + i.length
             } while (o = a.exec(e));
             c !== e.length && (s += e.substring(c))
         } else s = e;
         return s
     };
-    var $f = {
+    var Of = {
             scope: "body",
             level: "all"
         },
-        Of = /&(?:#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+);/g,
-        Sf = /&(?:#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+)[;=]?/g,
-        Df = {
+        Sf = /&(?:#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+);/g,
+        Df = /&(?:#\d+|#[xX][\da-fA-F]+|[0-9a-zA-Z]+)[;=]?/g,
+        Cf = {
             xml: {
-                strict: Of,
-                attribute: Sf,
-                body: kf.bodyRegExps.xml
+                strict: Sf,
+                attribute: Df,
+                body: xf.bodyRegExps.xml
             },
             html4: {
-                strict: Of,
-                attribute: Sf,
-                body: kf.bodyRegExps.html4
+                strict: Sf,
+                attribute: Df,
+                body: xf.bodyRegExps.html4
             },
             html5: {
-                strict: Of,
-                attribute: Sf,
-                body: kf.bodyRegExps.html5
+                strict: Sf,
+                attribute: Df,
+                body: xf.bodyRegExps.html5
             }
         },
-        Cf = _f(_f({}, Df), {
-            all: Df.html5
+        Rf = kf(kf({}, Cf), {
+            all: Cf.html5
         }),
-        Rf = String.fromCharCode,
-        Lf = Rf(65533),
-        Nf = {
+        Lf = String.fromCharCode,
+        Nf = Lf(65533),
+        If = {
             level: "all"
         };
-    vf.decodeEntity = function(e, t) {
-        var r = void 0 === (n = (void 0 === t ? Nf : t).level) ? "all" : n;
+    yf.decodeEntity = function(e, t) {
+        var r = void 0 === (n = (void 0 === t ? If : t).level) ? "all" : n;
         if (!e) return "";
         var n = e;
         e[e.length - 1];
-        var i = qf[r].entities[e];
+        var i = Ef[r].entities[e];
         if (i) n = i;
         else if ("&" === e[0] && "#" === e[1]) {
             var o = e[2],
                 s = "x" == o || "X" == o ? parseInt(e.substr(3), 16) : parseInt(e.substr(2));
-            n = s >= 1114111 ? Lf : s > 65535 ? Af.fromCodePoint(s) : Rf(xf.numericUnicodeMap[s] || s)
+            n = s >= 1114111 ? Nf : s > 65535 ? qf.fromCodePoint(s) : Lf(Af.numericUnicodeMap[s] || s)
         }
         return n
     };
-    var If = vf.decode = function(e, t) {
-            var r = void 0 === t ? $f : t,
+    var Ff = yf.decode = function(e, t) {
+            var r = void 0 === t ? Of : t,
                 n = r.level,
                 i = void 0 === n ? "all" : n,
                 o = r.scope,
                 s = void 0 === o ? "xml" === i ? "strict" : "body" : o;
             if (!e) return "";
-            var a = Cf[i][s],
-                l = qf[i].entities,
+            var a = Rf[i][s],
+                l = Ef[i].entities,
                 u = "attribute" === s,
                 c = "strict" === s;
             a.lastIndex = 0;
             var f, h = a.exec(e);
             if (h) {
                 f = "";
                 var p = 0;
@@ -17446,39 +17466,39 @@
                     else if (c && ";" !== g) m = d;
                     else {
                         var v = l[d];
                         if (v) m = v;
                         else if ("&" === d[0] && "#" === d[1]) {
                             var y = d[2],
                                 b = "x" == y || "X" == y ? parseInt(d.substr(3), 16) : parseInt(d.substr(2));
-                            m = b >= 1114111 ? Lf : b > 65535 ? Af.fromCodePoint(b) : Rf(xf.numericUnicodeMap[b] || b)
+                            m = b >= 1114111 ? Nf : b > 65535 ? qf.fromCodePoint(b) : Lf(Af.numericUnicodeMap[b] || b)
                         }
                     }
                     f += m, p = h.index + d.length
                 } while (h = a.exec(e));
                 p !== e.length && (f += e.substring(p))
             } else f = e;
             return f
         },
-        Ff = {
+        Mf = {
             strictlyTwoElementsInRangeArrays: !1,
             progressFn: null
         };
     /**
      * @name ranges-sort
      * @fileoverview Sort string index ranges
      * @version 6.0.8
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/ranges-sort/}
      */
-    function Mf(e, t) {
+    function Pf(e, t) {
         if (!Array.isArray(e) || !e.length) return e;
         let r, n, i = {
-            ...Ff,
+            ...Mf,
             ...t
         };
         if (i.strictlyTwoElementsInRangeArrays && !e.every(((e, t) => !(!Array.isArray(e) || 2 !== e.length) || (r = t, n = e.length, !1)))) throw new TypeError(`ranges-sort: [THROW_ID_03] The first argument should be an array and must consist of arrays which are natural number indexes representing TWO string index ranges. However, ${r}th range (${JSON.stringify(e[r],null,4)}) has not two but ${n} elements!`);
         if (!e.every(((e, t) => !(!Array.isArray(e) || !Number.isInteger(e[0]) || e[0] < 0 || !Number.isInteger(e[1]) || e[1] < 0) || (r = t, !1)))) throw new TypeError(`ranges-sort: [THROW_ID_04] The first argument should be an array and must consist of arrays which are natural number indexes representing string index ranges. However, ${r}th range (${JSON.stringify(e[r],null,4)}) does not consist of only natural numbers!`);
         let o = e.length ** 2,
             s = 0;
         return Array.from(e).sort(((e, t) => (i.progressFn && (s += 1, i.progressFn(Math.floor(100 * s / o))), e[0] === t[0] ? e[1] < t[1] ? -1 : e[1] > t[1] ? 1 : 0 : e[0] < t[0] ? -1 : 1)))
@@ -17487,30 +17507,30 @@
      * @name ranges-merge
      * @fileoverview Merge and sort string index ranges
      * @version 9.0.10
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/ranges-merge/}
      */
-    var Pf = {
+    var jf = {
         mergeType: 1,
         progressFn: null,
         joinRangesThatTouchEdges: !0
     };
-    var jf = !0,
-        Bf = "Invariant failed";
+    var Bf = !0,
+        Uf = "Invariant failed";
     /**
      * @name ranges-apply
      * @fileoverview Take an array of string index ranges, delete/replace the string according to them
      * @version 7.0.10
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/ranges-apply/}
      */
-    function Uf(e, t, r) {
+    function Vf(e, t, r) {
         let n, i = 0,
             o = 0;
         if (0 === arguments.length) throw new Error("ranges-apply: [THROW_ID_01] inputs missing!");
         if ("string" != typeof e) throw new TypeError(`ranges-apply: [THROW_ID_02] first input argument must be a string! Currently it's: ${typeof e}, equal to: ${JSON.stringify(e,null,4)}`);
         if (t && !Array.isArray(t)) throw new TypeError(`ranges-apply: [THROW_ID_03] second input argument must be an array (or null)! Currently it's: ${typeof t}, equal to: ${JSON.stringify(t,null,4)}`);
         if (r && "function" != typeof r) throw new TypeError(`ranges-apply: [THROW_ID_04] the third input argument must be a function (or falsey)! Currently it's: ${typeof r}, equal to: ${JSON.stringify(r,null,4)}`);
         if (!t?.filter((e => e)).length) return e;
@@ -17534,42 +17554,42 @@
                 return !!e && "object" == typeof e && !Array.isArray(e)
             }
             if (!Array.isArray(e) || !e.length) return null;
             let n;
             if (t) {
                 if (!r(t)) throw new Error(`emlint: [THROW_ID_03] the second input argument must be a plain object. It was given as:\n${JSON.stringify(t,null,4)} (type ${typeof t})`);
                 if (n = {
-                        ...Pf,
+                        ...jf,
                         ...t
                     }, n.progressFn && r(n.progressFn) && !Object.keys(n.progressFn).length) n.progressFn = null;
                 else if (n.progressFn && "function" != typeof n.progressFn) throw new Error(`ranges-merge: [THROW_ID_01] opts.progressFn must be a function! It was given of a type: "${typeof n.progressFn}", equal to ${JSON.stringify(n.progressFn,null,4)}`);
                 if (![1, 2, "1", "2"].includes(n.mergeType)) throw new Error(`ranges-merge: [THROW_ID_02] opts.mergeType was customised to a wrong thing! It was given of a type: "${typeof n.mergeType}", equal to ${JSON.stringify(n.mergeType,null,4)}`);
                 if ("boolean" != typeof n.joinRangesThatTouchEdges) throw new Error(`ranges-merge: [THROW_ID_04] opts.joinRangesThatTouchEdges was customised to a wrong thing! It was given of a type: "${typeof n.joinRangesThatTouchEdges}", equal to ${JSON.stringify(n.joinRangesThatTouchEdges,null,4)}`)
             } else n = {
-                ...Pf
+                ...jf
             };
             let i, o, s, a = e.filter((e => Array.isArray(e))).map((e => [...e])).filter((e => void 0 !== e[2] || e[0] !== e[1]));
-            i = n.progressFn ? Mf(a, {
+            i = n.progressFn ? Pf(a, {
                 progressFn: e => {
                     s = Math.floor(e / 5), s !== o && (o = s, n.progressFn(s))
                 }
-            }) : Mf(a);
+            }) : Pf(a);
             let l = i.length - 1;
             for (let e = l; e > 0; e--) n.progressFn && (s = Math.floor(78 * (1 - e / l)) + 21, s !== o && s > o && (o = s, n.progressFn(s))), (i[e][0] <= i[e - 1][0] || !n.joinRangesThatTouchEdges && i[e][0] < i[e - 1][1] || n.joinRangesThatTouchEdges && i[e][0] <= i[e - 1][1]) && (i[e - 1][0] = Math.min(i[e][0], i[e - 1][0]), i[e - 1][1] = Math.max(i[e][1], i[e - 1][1]), void 0 !== i[e][2] && (i[e - 1][0] >= i[e][0] || i[e - 1][1] <= i[e][1]) && null !== i[e - 1][2] && (null === i[e][2] && null !== i[e - 1][2] ? i[e - 1][2] = null : null != i[e - 1][2] ? 2 == +n.mergeType && i[e - 1][0] === i[e][0] ? i[e - 1][2] = i[e][2] : i[e - 1][2] += i[e][2] : i[e - 1][2] = i[e][2]), i.splice(e, 1), e = i.length);
             return i.length ? i : null
         }(n, {
             progressFn: e => {
                 r && (i = 10 + Math.floor(e / 10), i !== o && (o = i, r(i)))
             }
         });
         ! function(e, t) {
             if (!e) {
-                if (jf) throw new Error(Bf);
+                if (Bf) throw new Error(Uf);
                 var r = "function" == typeof t ? t() : t,
-                    n = r ? "".concat(Bf, ": ").concat(r) : Bf;
+                    n = r ? "".concat(Uf, ": ").concat(r) : Uf;
                 throw new Error(n)
             }
         }(l);
         let u = l.length;
         if (u > 0) {
             let t = e.slice(l[u - 1][1]);
             e = l.reduce(((t, n, s, a) => {
@@ -17585,15 +17605,15 @@
      * @name string-collapse-leading-whitespace
      * @fileoverview Collapse the leading and trailing whitespace of a string
      * @version 7.0.5
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/string-collapse-leading-whitespace/}
      */
-    function Vf(e, t = 1) {
+    function zf(e, t = 1) {
         function r(e) {
             return Array.from(e).reverse().join("")
         }
 
         function n(e, t, r) {
             let n = r ? "\n" : "\r",
                 i = r ? "\r" : "\n";
@@ -17629,66 +17649,66 @@
      * @name ranges-push
      * @fileoverview Gather string index ranges
      * @version 7.0.10
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/ranges-push/}
      */
-    var zf = {
+    var Hf = {
         mergeType: 1,
         progressFn: null,
         joinRangesThatTouchEdges: !0
     };
-    var Hf = {
+    var Wf = {
             limitToBeAddedWhitespace: !1,
             limitLinebreaksCount: 1,
             mergeType: 1
         },
-        Wf = class {
+        Gf = class {
             constructor(e) {
                 let t = {
-                    ...Hf,
+                    ...Wf,
                     ...e
                 };
                 if (t.mergeType && 1 !== t.mergeType && 2 !== t.mergeType)
-                    if (Cu(t.mergeType) && "1" === t.mergeType.trim()) t.mergeType = 1;
+                    if (Ru(t.mergeType) && "1" === t.mergeType.trim()) t.mergeType = 1;
                     else {
-                        if (!Cu(t.mergeType) || "2" !== t.mergeType.trim()) throw new Error(`ranges-push: [THROW_ID_02] opts.mergeType was customised to a wrong thing! It was given of a type: "${typeof t.mergeType}", equal to ${JSON.stringify(t.mergeType,null,4)}`);
+                        if (!Ru(t.mergeType) || "2" !== t.mergeType.trim()) throw new Error(`ranges-push: [THROW_ID_02] opts.mergeType was customised to a wrong thing! It was given of a type: "${typeof t.mergeType}", equal to ${JSON.stringify(t.mergeType,null,4)}`);
                         t.mergeType = 2
                     } this.opts = t, this.ranges = []
             }
             ranges;
             opts;
             add(e, t, r) {
                 if (null == e && null == t) return;
-                if (Lu(e) && !Lu(t)) {
+                if (Nu(e) && !Nu(t)) {
                     if (Array.isArray(e)) {
                         if (e.length) {
                             if (e.some((e => Array.isArray(e)))) return void e.forEach((e => {
                                 Array.isArray(e) && this.add(...e)
                             }));
-                            e.length && Ru(+e[0]) && Ru(+e[1]) && this.add(...e)
+                            e.length && Lu(+e[0]) && Lu(+e[1]) && this.add(...e)
                         }
                         return
                     }
                     throw new TypeError(`ranges-push/Ranges/add(): [THROW_ID_12] the first input argument, "from" is set (${JSON.stringify(e,null,0)}) but second-one, "to" is not (${JSON.stringify(t,null,0)})`)
                 }
-                if (!Lu(e) && Lu(t)) throw new TypeError(`ranges-push/Ranges/add(): [THROW_ID_13] the second input argument, "to" is set (${JSON.stringify(t,null,0)}) but first-one, "from" is not (${JSON.stringify(e,null,0)})`);
+                if (!Nu(e) && Nu(t)) throw new TypeError(`ranges-push/Ranges/add(): [THROW_ID_13] the second input argument, "to" is set (${JSON.stringify(t,null,0)}) but first-one, "from" is not (${JSON.stringify(e,null,0)})`);
                 let n = +e,
                     i = +t;
-                if (Ru(r) && (r = String(r)), !Ru(n) || !Ru(i)) throw Ru(n) && n >= 0 ? new TypeError(`ranges-push/Ranges/add(): [THROW_ID_10] "to" value, the second input argument, must be a natural number or zero! Currently it's of a type "${typeof i}" equal to: ${JSON.stringify(i,null,4)}`) : new TypeError(`ranges-push/Ranges/add(): [THROW_ID_09] "from" value, the first input argument, must be a natural number or zero! Currently it's of a type "${typeof n}" equal to: ${JSON.stringify(n,null,4)}`);
-                if (Lu(r) && !Cu(r) && !Ru(r)) throw new TypeError(`ranges-push/Ranges/add(): [THROW_ID_08] The third argument, the value to add, was given not as string but ${typeof r}, equal to:\n${JSON.stringify(r,null,4)}`);
-                if (Lu(this.ranges) && Array.isArray(this.last()) && n === this.last()[1]) {
-                    if (this.last()[1] = i, this.last()[2], null !== this.last()[2] && Lu(r)) {
+                if (Lu(r) && (r = String(r)), !Lu(n) || !Lu(i)) throw Lu(n) && n >= 0 ? new TypeError(`ranges-push/Ranges/add(): [THROW_ID_10] "to" value, the second input argument, must be a natural number or zero! Currently it's of a type "${typeof i}" equal to: ${JSON.stringify(i,null,4)}`) : new TypeError(`ranges-push/Ranges/add(): [THROW_ID_09] "from" value, the first input argument, must be a natural number or zero! Currently it's of a type "${typeof n}" equal to: ${JSON.stringify(n,null,4)}`);
+                if (Nu(r) && !Ru(r) && !Lu(r)) throw new TypeError(`ranges-push/Ranges/add(): [THROW_ID_08] The third argument, the value to add, was given not as string but ${typeof r}, equal to:\n${JSON.stringify(r,null,4)}`);
+                if (Nu(this.ranges) && Array.isArray(this.last()) && n === this.last()[1]) {
+                    if (this.last()[1] = i, this.last()[2], null !== this.last()[2] && Nu(r)) {
                         let e = !this.last()[2] || !this.last()[2].length || this.opts?.mergeType && 1 !== this.opts.mergeType ? r : `${this.last()[2]}${r}`;
-                        this.opts.limitToBeAddedWhitespace && (e = Vf(e, this.opts.limitLinebreaksCount)), Cu(e) && !e.length || (this.last()[2] = e)
+                        this.opts.limitToBeAddedWhitespace && (e = zf(e, this.opts.limitLinebreaksCount)), Ru(e) && !e.length || (this.last()[2] = e)
                     }
                 } else {
                     this.ranges || (this.ranges = []);
-                    let e = void 0 === r || Cu(r) && !r.length ? [n, i] : [n, i, r && this.opts.limitToBeAddedWhitespace ? Vf(r, this.opts.limitLinebreaksCount) : r];
+                    let e = void 0 === r || Ru(r) && !r.length ? [n, i] : [n, i, r && this.opts.limitToBeAddedWhitespace ? zf(r, this.opts.limitLinebreaksCount) : r];
                     this.ranges.push(e)
                 }
             }
             push(e, t, r) {
                 this.add(e, t, r)
             }
             current() {
@@ -17697,42 +17717,42 @@
                         return !!e && "object" == typeof e && !Array.isArray(e)
                     }
                     if (!Array.isArray(e) || !e.length) return null;
                     let n;
                     if (t) {
                         if (!r(t)) throw new Error(`emlint: [THROW_ID_03] the second input argument must be a plain object. It was given as:\n${JSON.stringify(t,null,4)} (type ${typeof t})`);
                         if (n = {
-                                ...zf,
+                                ...Hf,
                                 ...t
                             }, n.progressFn && r(n.progressFn) && !Object.keys(n.progressFn).length) n.progressFn = null;
                         else if (n.progressFn && "function" != typeof n.progressFn) throw new Error(`ranges-merge: [THROW_ID_01] resolvedOpts.progressFn must be a function! It was given of a type: "${typeof n.progressFn}", equal to ${JSON.stringify(n.progressFn,null,4)}`);
                         if (![1, 2, "1", "2"].includes(n.mergeType)) throw new Error(`ranges-merge: [THROW_ID_02] resolvedOpts.mergeType was customised to a wrong thing! It was given of a type: "${typeof n.mergeType}", equal to ${JSON.stringify(n.mergeType,null,4)}`);
                         if ("boolean" != typeof n.joinRangesThatTouchEdges) throw new Error(`ranges-merge: [THROW_ID_04] resolvedOpts.joinRangesThatTouchEdges was customised to a wrong thing! It was given of a type: "${typeof n.joinRangesThatTouchEdges}", equal to ${JSON.stringify(n.joinRangesThatTouchEdges,null,4)}`)
                     } else n = {
-                        ...zf
+                        ...Hf
                     };
                     let i, o, s, a = e.filter((e => Array.isArray(e))).map((e => [...e])).filter((e => void 0 !== e[2] || e[0] !== e[1]));
-                    i = n.progressFn ? Mf(a, {
+                    i = n.progressFn ? Pf(a, {
                         progressFn: e => {
                             s = Math.floor(e / 5), s !== o && (o = s, n.progressFn(s))
                         }
-                    }) : Mf(a);
+                    }) : Pf(a);
                     let l = i.length - 1;
                     for (let e = l; e > 0; e--) n.progressFn && (s = Math.floor(78 * (1 - e / l)) + 21, s !== o && s > o && (o = s, n.progressFn(s))), (i[e][0] <= i[e - 1][0] || !n.joinRangesThatTouchEdges && i[e][0] < i[e - 1][1] || n.joinRangesThatTouchEdges && i[e][0] <= i[e - 1][1]) && (i[e - 1][0] = Math.min(i[e][0], i[e - 1][0]), i[e - 1][1] = Math.max(i[e][1], i[e - 1][1]), void 0 !== i[e][2] && (i[e - 1][0] >= i[e][0] || i[e - 1][1] <= i[e][1]) && null !== i[e - 1][2] && (null === i[e][2] && null !== i[e - 1][2] ? i[e - 1][2] = null : null != i[e - 1][2] ? 2 == +n.mergeType && i[e - 1][0] === i[e][0] ? i[e - 1][2] = i[e][2] : i[e - 1][2] += i[e][2] : i[e - 1][2] = i[e][2]), i.splice(e, 1), e = i.length);
                     return i.length ? i : null
                 }(this.ranges, {
                     mergeType: this.opts.mergeType
-                }), this.ranges && this.opts.limitToBeAddedWhitespace ? this.ranges.map((e => Lu(e[2]) ? [e[0], e[1], Vf(e[2], this.opts.limitLinebreaksCount)] : e)) : this.ranges) : null
+                }), this.ranges && this.opts.limitToBeAddedWhitespace ? this.ranges.map((e => Nu(e[2]) ? [e[0], e[1], zf(e[2], this.opts.limitLinebreaksCount)] : e)) : this.ranges) : null
             }
             wipe() {
                 this.ranges = []
             }
             replace(e) {
                 if (Array.isArray(e) && e.length) {
-                    if (!Array.isArray(e[0]) || !Ru(e[0][0])) throw new Error(`ranges-push/Ranges/replace(): [THROW_ID_11] Single range was given but we expected array of arrays! The first element, ${JSON.stringify(e[0],null,4)} should be an array and its first element should be an integer, a string index.`);
+                    if (!Array.isArray(e[0]) || !Lu(e[0][0])) throw new Error(`ranges-push/Ranges/replace(): [THROW_ID_11] Single range was given but we expected array of arrays! The first element, ${JSON.stringify(e[0],null,4)} should be an array and its first element should be an integer, a string index.`);
                     this.ranges = Array.from(e)
                 } else this.ranges = []
             }
             last() {
                 return Array.isArray(this.ranges) && this.ranges.length ? this.ranges[this.ranges.length - 1] : null
             }
         };
@@ -17740,29 +17760,29 @@
      * @name string-left-right
      * @fileoverview Looks up the first non-whitespace character to the left/right of a given index
      * @version 6.0.13
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/string-left-right/}
      */
-    Su();
-    var Gf = " ";
+    Du();
+    var Zf = " ";
 
-    function Zf(e, t = 0) {
+    function Jf(e, t = 0) {
         return function({
             str: e,
             idx: t = 0,
             stopAtNewlines: r = !1,
             stopAtRawNbsp: n = !1
         }) {
             if ("string" != typeof e || !e.length || ((!t || "number" != typeof t) && (t = 0), !e[t + 1])) return null;
-            if (e[t + 1] && (e[t + 1].trim() || r && "\n\r".includes(e[t + 1]) || n && e[t + 1] === Gf)) return t + 1;
-            if (e[t + 2] && (e[t + 2].trim() || r && "\n\r".includes(e[t + 2]) || n && e[t + 2] === Gf)) return t + 2;
+            if (e[t + 1] && (e[t + 1].trim() || r && "\n\r".includes(e[t + 1]) || n && e[t + 1] === Zf)) return t + 1;
+            if (e[t + 2] && (e[t + 2].trim() || r && "\n\r".includes(e[t + 2]) || n && e[t + 2] === Zf)) return t + 2;
             for (let i = t + 1, o = e.length; i < o; i++)
-                if (e[i].trim() || r && "\n\r".includes(e[i]) || n && e[i] === Gf) return i;
+                if (e[i].trim() || r && "\n\r".includes(e[i]) || n && e[i] === Zf) return i;
             return null
         }({
             str: e,
             idx: t,
             stopAtNewlines: !1,
             stopAtRawNbsp: !1
         })
@@ -17771,46 +17791,46 @@
      * @name string-strip-html
      * @fileoverview Strip HTML tags from strings. No parser, accepts mixed sources.
      * @version 13.4.1
      * @author Roy Revelt, Codsen Ltd
      * @license MIT
      * {@link https://codsen.com/os/string-strip-html/}
      */
-    function Jf(e) {
+    function Yf(e) {
         return /[-_A-Za-z0-9]/.test(e)
     }
 
-    function Yf(e, t) {
+    function Kf(e, t) {
         if (!e) return [];
         if (Array.isArray(e)) return e.filter((e => "string" == typeof e && e.trim()));
         if ("string" == typeof e) return e.trim() ? [e] : [];
         throw new TypeError(`string-strip-html/stripHtml(): [THROW_ID_05] ${t} must be array containing zero or more strings or something falsey. Currently it's equal to: ${e}, that a type of ${typeof e}.`)
     }
 
-    function Kf(e, t, r, n) {
+    function Xf(e, t, r, n) {
         for (let i = t, o = e.length; i < o; i++) {
             if (e.startsWith(r, i)) return !0;
             if (e.startsWith(n, i)) return !1
         }
         return !1
     }
 
-    function Xf(e, t, r) {
-        return e?.quotes, e?.quotes?.value && Kf(t, r + 1, e.quotes.value, ">"), e?.quotes?.next, Kf(t, e?.quotes?.next - 1, e?.quotes?.value, ">"), !e?.quotes || !Kf(t, r + 1, e.quotes.value, ">") && -1 !== e?.quotes?.next && Kf(t, e?.quotes?.next - 1, e?.quotes?.value, ">")
+    function Qf(e, t, r) {
+        return e?.quotes, e?.quotes?.value && Xf(t, r + 1, e.quotes.value, ">"), e?.quotes?.next, Xf(t, e?.quotes?.next - 1, e?.quotes?.value, ">"), !e?.quotes || !Xf(t, r + 1, e.quotes.value, ">") && -1 !== e?.quotes?.next && Xf(t, e?.quotes?.next - 1, e?.quotes?.value, ">")
     }
 
-    function Qf(e, t) {
+    function eh(e, t) {
         return (t.match(new RegExp(e, "g")) || []).length
     }
-    var eh = new Set(["!doctype", "abbr", "address", "area", "article", "aside", "audio", "base", "bdi", "bdo", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "doctype", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "math", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "param", "picture", "pre", "progress", "rb", "rp", "rt", "rtc", "ruby", "samp", "script", "section", "select", "slot", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "svg", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "ul", "var", "video", "wbr", "xml"]),
-        th = new Set(["a", "b", "i", "p", "q", "s", "u"]),
-        rh = new Set([".", ",", ";", "!", "?"]),
-        nh = new Set([".", ",", "?", ";", ")", "…", '"', "»"]),
-        ih = new Set(["a", "abbr", "acronym", "audio", "b", "bdi", "bdo", "big", "button", "canvas", "cite", "code", "data", "datalist", "del", "dfn", "em", "embed", "i", "iframe", "input", "ins", "kbd", "label", "map", "mark", "meter", "noscript", "object", "output", "picture", "progress", "q", "ruby", "s", "samp", "select", "slot", "small", "span", "strong", "sub", "sup", "svg", "template", "textarea", "time", "u", "tt", "var", "video", "wbr"]),
-        oh = {
+    var th = new Set(["!doctype", "abbr", "address", "area", "article", "aside", "audio", "base", "bdi", "bdo", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "doctype", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "math", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "param", "picture", "pre", "progress", "rb", "rp", "rt", "rtc", "ruby", "samp", "script", "section", "select", "slot", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "svg", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "ul", "var", "video", "wbr", "xml"]),
+        rh = new Set(["a", "b", "i", "p", "q", "s", "u"]),
+        nh = new Set([".", ",", ";", "!", "?"]),
+        ih = new Set([".", ",", "?", ";", ")", "…", '"', "»"]),
+        oh = new Set(["a", "abbr", "acronym", "audio", "b", "bdi", "bdo", "big", "button", "canvas", "cite", "code", "data", "datalist", "del", "dfn", "em", "embed", "i", "iframe", "input", "ins", "kbd", "label", "map", "mark", "meter", "noscript", "object", "output", "picture", "progress", "q", "ruby", "s", "samp", "select", "slot", "small", "span", "strong", "sub", "sup", "svg", "template", "textarea", "time", "u", "tt", "var", "video", "wbr"]),
+        sh = {
             ignoreTags: [],
             ignoreTagsWithTheirContents: [],
             onlyStripTags: [],
             stripTogetherWithTheirContents: ["script", "style", "xml"],
             skipHtmlDecoding: !1,
             trimOnlySpaces: !1,
             stripRecognisedHTMLOnly: !1,
@@ -17823,15 +17843,15 @@
             ignoreIndentations: !1,
             cb: null,
             reportProgressFunc: null,
             reportProgressFuncFrom: 0,
             reportProgressFuncTo: 100
         };
 
-    function sh(e, t) {
+    function ah(e, t) {
         let r = Date.now(),
             n = [],
             i = [],
             o = [],
             s = [],
             a = {};
         a = {
@@ -17855,15 +17875,15 @@
         function y(t, r, i) {
             if (Array.isArray(r.stripTogetherWithTheirContents) && (r.stripTogetherWithTheirContents.includes(a.name) || r.stripTogetherWithTheirContents.includes("*")))
                 if (a.slashPresent && Array.isArray(n) && n.some((e => e.name === a.name))) {
                     for (let o = n.length; o--;)
                         if (n[o].name === a.name) {
                             s = s.filter((([e, r]) => (e < n[o].lastOpeningBracketAt || e >= t + 1) && (r <= n[o].lastOpeningBracketAt || r > t + 1)));
                             let l = t + 1;
-                            a.lastClosingBracketAt && (l = a.lastClosingBracketAt + 1), s.push([n[o].lastOpeningBracketAt, l]), nh.has(e[t]) && r.cb ? r.cb({
+                            a.lastClosingBracketAt && (l = a.lastClosingBracketAt + 1), s.push([n[o].lastOpeningBracketAt, l]), ih.has(e[t]) && r.cb ? r.cb({
                                 tag: a,
                                 deleteFrom: n[o].lastOpeningBracketAt,
                                 deleteTo: t + 1,
                                 insert: null,
                                 rangesArr: i,
                                 proposedReturn: [n[o].lastOpeningBracketAt, t, null]
                             }) : r.cb && r.cb({
@@ -17882,31 +17902,31 @@
 
         function b(t, r, n, i, o, s) {
             if (Array.isArray($.current()) && "number" == typeof n && 0 === $.current()[0][0] && $.current()[0][1] >= n) return "";
             if (e.length === i && s && !q?.dumpLinkHrefsNearby?.enabled) return null;
             let l = "";
             if (Number.isInteger(n) && n < o && (l += t.slice(n, o)), Number.isInteger(i) && i > s + 1) {
                 let r = t.slice(s + 1, i);
-                i && !Zf(e, i - 1) && (r = r.trimEnd()), r.includes("\n") && _(i, t) ? l += " " : l += r
+                i && !Jf(e, i - 1) && (r = r.trimEnd()), r.includes("\n") && _(i, t) ? l += " " : l += r
             }
-            let u = !nh.has(t[r]),
+            let u = !ih.has(t[r]),
                 c = ">" !== t[i - 1] || !t[n].trim(),
                 f = !['"', "("].includes(t[o - 1]),
                 h = ![";", ".", ":", "!"].includes(t[r]);
-            if ((u || c && f && h) && (c || f) && "!" !== t[r] && (!ih.has(a.name) || "number" == typeof n && n < o || "number" == typeof i && i > s + 1)) {
+            if ((u || c && f && h) && (c || f) && "!" !== t[r] && (!oh.has(a.name) || "number" == typeof n && n < o || "number" == typeof i && i > s + 1)) {
                 let e = l.match(/\n/g);
                 return Array.isArray(e) && e.length ? 1 === e.length ? "\n" : 2 === e.length ? "\n\n" : "\n\n\n" : " "
             }
             return ""
         }
 
         function w(t, r) {
             if (t.dumpLinkHrefsNearby?.enabled && p.tagName && p.tagName === a.name && a.lastOpeningBracketAt && (p.openingTagEnds && a.lastOpeningBracketAt > p.openingTagEnds || !p.openingTagEnds) && (m = !0), m) {
                 let n = t.dumpLinkHrefsNearby?.putOnNewLine ? "\n\n" : "";
-                d = `${n}${p.hrefValue}`, ("number" != typeof r || Zf(e, r - 1)) && (d += n)
+                d = `${n}${p.hrefValue}`, ("number" != typeof r || Jf(e, r - 1)) && (d += n)
             }
         }
 
         function _(t, r) {
             return r ? "<" === r[t] && "%" !== r[t + 1] : "<" === e[t] && "%" !== e[t + 1]
         }
 
@@ -17918,55 +17938,55 @@
             if (r.ignoreTagsWithTheirContents.includes("*")) return !0;
             let o = e.indexOf(`<${n.name}`, t),
                 s = e.indexOf(`</${n.name}`, t);
             return !(!n.slashPresent && -1 === s || n.slashPresent && !i.some((e => e.name === n.name)) || s > -1 && o > -1 && o < s) && r.ignoreTagsWithTheirContents.includes(n.name)
         }
         if ("string" != typeof e) throw new TypeError(`string-strip-html/stripHtml(): [THROW_ID_01] Input must be string! Currently it's: ${(typeof e).toLowerCase()}, equal to:\n${JSON.stringify(e,null,4)}`);
         if (t) {
-            if (!Du(t)) throw new TypeError(`string-strip-html/stripHtml(): [THROW_ID_02] Optional Options Object must be a plain object! Currently it's: ${(typeof t).toLowerCase()}, equal to:\n${JSON.stringify(t,null,4)}`);
+            if (!Cu(t)) throw new TypeError(`string-strip-html/stripHtml(): [THROW_ID_02] Optional Options Object must be a plain object! Currently it's: ${(typeof t).toLowerCase()}, equal to:\n${JSON.stringify(t,null,4)}`);
             if (t.reportProgressFunc && "function" != typeof t.reportProgressFunc) throw new Error(`string-strip-html/stripHtml(): [THROW_ID_03] The Optional Options Object's key reportProgressFunc, callback function, should be a function but it was given as type ${typeof t.reportProgressFunc}, equal to ${JSON.stringify(t.reportProgressFunc,null,4)}`);
             if ("boolean" == typeof t.dumpLinkHrefsNearby && null != t.dumpLinkHrefsNearby) throw new Error(`string-strip-html/stripHtml(): [THROW_ID_04] The Optional Options Object's key should be a plain object but it was given as type ${typeof t.dumpLinkHrefsNearby}, equal to ${JSON.stringify(t.dumpLinkHrefsNearby,null,4)}`)
         }
 
         function A() {
             m && (p = {
                 tagName: "",
                 hrefValue: "",
                 openingTagEnds: void 0
             }, m = !1)
         }
         let q = {
-            ...oh,
+            ...sh,
             ...t,
-            dumpLinkHrefsNearby: Object.assign({}, oh.dumpLinkHrefsNearby, t?.dumpLinkHrefsNearby)
+            dumpLinkHrefsNearby: Object.assign({}, sh.dumpLinkHrefsNearby, t?.dumpLinkHrefsNearby)
         };
-        if (Nu(q, "returnRangesOnly")) throw new TypeError("string-strip-html/stripHtml(): [THROW_ID_05] The Optional Options Object's key returnRangesOnly has been removed from the API since v.5 release.");
+        if (Iu(q, "returnRangesOnly")) throw new TypeError("string-strip-html/stripHtml(): [THROW_ID_05] The Optional Options Object's key returnRangesOnly has been removed from the API since v.5 release.");
         if (q.reportProgressFunc) {
             if ("number" != typeof q.reportProgressFuncFrom) throw new Error(`string-strip-html/stripHtml(): [THROW_ID_06] The Optional Options Object's key reportProgressFuncFrom, callback function's "from" range, should be a number but it was given as type ${typeof q.reportProgressFuncFrom}, equal to ${JSON.stringify(q.reportProgressFuncFrom,null,4)}`);
             if ("number" != typeof q.reportProgressFuncTo) throw new Error(`string-strip-html/stripHtml(): [THROW_ID_07] The Optional Options Object's key reportProgressFuncTo, callback function's "to" range, should be a number but it was given as type ${typeof q.reportProgressFuncTo}, equal to ${JSON.stringify(q.reportProgressFuncTo,null,4)}`)
         }
-        q.ignoreTags = Yf(q.ignoreTags, "resolvedOpts.ignoreTags"), q.onlyStripTags = Yf(q.onlyStripTags, "resolvedOpts.onlyStripTags");
+        q.ignoreTags = Kf(q.ignoreTags, "resolvedOpts.ignoreTags"), q.onlyStripTags = Kf(q.onlyStripTags, "resolvedOpts.onlyStripTags");
         let E = !!q.onlyStripTags.length;
-        q.onlyStripTags.length && q.ignoreTags.length && (q.onlyStripTags = gf(q.onlyStripTags, ...q.ignoreTags)), q.stripTogetherWithTheirContents ? "string" == typeof q.stripTogetherWithTheirContents && q.stripTogetherWithTheirContents.length && (q.stripTogetherWithTheirContents = [q.stripTogetherWithTheirContents]) : q.stripTogetherWithTheirContents = [];
+        q.onlyStripTags.length && q.ignoreTags.length && (q.onlyStripTags = vf(q.onlyStripTags, ...q.ignoreTags)), q.stripTogetherWithTheirContents ? "string" == typeof q.stripTogetherWithTheirContents && q.stripTogetherWithTheirContents.length && (q.stripTogetherWithTheirContents = [q.stripTogetherWithTheirContents]) : q.stripTogetherWithTheirContents = [];
         let T = {};
         if (q.stripTogetherWithTheirContents && Array.isArray(q.stripTogetherWithTheirContents) && q.stripTogetherWithTheirContents.length && !q.stripTogetherWithTheirContents.every(((e, t) => "string" == typeof e || (T.el = e, T.i = t, !1)))) throw new TypeError(`string-strip-html/stripHtml(): [THROW_ID_08] Optional Options Object's key stripTogetherWithTheirContents was set to contain not just string elements! For example, element at index ${T.i} has a value ${T.el} which is not string but ${(typeof T.el).toLowerCase()}.`);
         q.cb || (q.cb = ({
             rangesArr: e,
             proposedReturn: t
         }) => {
             t && e.push(...t)
         });
-        let $ = new Wf({
+        let $ = new Gf({
             limitToBeAddedWhitespace: !0,
             limitLinebreaksCount: 2
         });
         if (!q.skipHtmlDecoding)
-            for (; e !== If(e, {
+            for (; e !== Ff(e, {
                     scope: "strict"
-                });) e = If(e, {
+                });) e = Ff(e, {
                 scope: "strict"
             });
         let O = !1,
             S = !1,
             D = 0,
             C = 0,
             R = e.length,
@@ -17981,15 +18001,15 @@
                 }
             }
             if (!O && k(t) && (!a || Object.keys(a).length < 2) && t > 1)
                 for (let r = t; r--;)
                     if (void 0 === e[r - 1] || k(r)) {
                         let n = void 0 === e[r - 1] ? r : r + 1,
                             i = e.slice(n, t + 1) || "";
-                        if ((i.includes("/>") || i.includes("/ >") || i.includes('="') || i.includes("='")) && e !== `<${df(i.trim(),"/>")}>` && [...eh].some((e => df(i.trim().split(/\s+/).filter((e => e.trim())).filter(((e, t) => 0 === t)), "/>").toLowerCase() === e)) && "" === sh(`<${i.trim()}>`, q).result) {
+                        if ((i.includes("/>") || i.includes("/ >") || i.includes('="') || i.includes("='")) && e !== `<${mf(i.trim(),"/>")}>` && [...th].some((e => mf(i.trim().split(/\s+/).filter((e => e.trim())).filter(((e, t) => 0 === t)), "/>").toLowerCase() === e)) && "" === ah(`<${i.trim()}>`, q).result) {
                             (!o.length || o[o.length - 1][0] !== a.lastOpeningBracketAt) && o.push([n, t + 1]), (!s.length || s[s.length - 1][0] !== a.lastOpeningBracketAt) && s.push([n, t + 1]);
                             let r = b(e, t, n, t + 1, n, t + 1),
                                 i = t + 1;
                             if (e[i] && !e[i].trim())
                                 for (let t = i; t < R; t++)
                                     if (e[t].trim()) {
                                         i = t;
@@ -18011,15 +18031,15 @@
                         if ("string" == typeof e.name && "href" === e.name.toLowerCase()) return r = `${q.dumpLinkHrefsNearby?.wrapHeads||""}${e.value}${q.dumpLinkHrefsNearby?.wrapTails||""}`, !0
                     })) && (p = {
                         tagName: a.name,
                         hrefValue: r,
                         openingTagEnds: void 0
                     })
                 } else !S && !a.quotes && a.nameStarts && (a.quotes = {}, a.quotes.value = e[t], a.quotes.start = t, a.quotes.next = e.indexOf(e[t], t + 1), h.nameStarts && h.nameEnds && h.nameEnds < t && h.nameStarts < t && !h.valueStarts && (h.name = e.slice(h.nameStarts, h.nameEnds)));
-            if (!(void 0 === a.nameStarts || void 0 !== a.nameEnds || e[t].trim() && Jf(e[t]))) {
+            if (!(void 0 === a.nameStarts || void 0 !== a.nameEnds || e[t].trim() && Yf(e[t]))) {
                 if (a.nameEnds = t, a.name = e.slice(a.nameStarts, a.nameEnds + (k(t) || "/" === e[t] || void 0 !== e[t + 1] ? 0 : 1)), "!" !== e[a.nameStarts - 1] && !a.name.replace(/-/g, "").length || /^\d+$/.test(a.name[0])) {
                     a = {};
                     continue
                 }
                 if ("string" == typeof a.name && "doctype" === a.name.toLowerCase() && (S = !0), _(t)) {
                     w(q);
                     let r = b(e, t, a.leftOuterWhitespace, t, a.lastOpeningBracketAt, t);
@@ -18029,22 +18049,22 @@
                         deleteTo: t,
                         insert: `${r}${d}${r}`,
                         rangesArr: $,
                         proposedReturn: [a.leftOuterWhitespace, t, `${r}${d}${r}`]
                     }), A(), y(t, q, $)
                 }
             }
-            if (a.quotes?.start && a.quotes.start < t && !a.quotes.end && h.nameEnds && h.equalsAt && !h.valueStarts && (h.valueStarts = t), !a.quotes && h.nameEnds && "=" === e[t] && !h.valueStarts && !h.equalsAt && (h.equalsAt = t), !a.quotes && h.nameStarts && h.nameEnds && !h.valueStarts && e[t].trim() && "=" !== e[t] && (a.attributes.push(h), h = {}), !a.quotes && h.nameStarts && !h.nameEnds && (S && "'\"".includes(e[h.nameStarts]) ? h.nameStarts < t && e[t] === e[h.nameStarts] && (h.nameEnds = t + 1, h.name = e.slice(h.nameStarts, h.nameEnds)) : e[t].trim() ? "=" === e[t] ? h.equalsAt || (h.nameEnds = t, h.equalsAt = t, h.name = e.slice(h.nameStarts, h.nameEnds)) : ("/" === e[t] || k(t) || _(t)) && (h.nameEnds = t, h.name = e.slice(h.nameStarts, h.nameEnds), a.attributes.push(h), h = {}) : (h.nameEnds = t, h.name = e.slice(h.nameStarts, h.nameEnds))), !a.quotes && a.nameEnds < t && !e[t - 1].trim() && e[t].trim() && !"<>/!".includes(e[t]) && !h.nameStarts && !a.lastClosingBracketAt && (h.nameStarts = t), null !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && "/" === e[t] && a.onlyPlausible && (a.onlyPlausible = !1), null !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && "/" !== e[t] && (void 0 === a.onlyPlausible && (e[t].trim() && !_(t) || a.slashPresent ? a.onlyPlausible = !1 : a.onlyPlausible = !0), e[t].trim() && void 0 === a.nameStarts && !_(t) && "/" !== e[t] && !k(t) && "!" !== e[t] && (a.nameStarts = t, a.nameContainsLetters = !1)), a.nameStarts && !a.quotes && "string" == typeof e[t] && e[t].toLowerCase() !== e[t].toUpperCase() && (a.nameContainsLetters = !0), k(t) && (Xf(a, e, t) || a.quotes.value && "number" == typeof a.lastOpeningBracketAt && Qf(a.quotes.value, e.slice(a.lastOpeningBracketAt, t)) % 2 == 1 && !e.slice(a.lastOpeningBracketAt + 1, t).includes("<") && !e.slice(a.lastOpeningBracketAt + 1, t).includes(">")) && void 0 !== a.lastOpeningBracketAt && (a.lastClosingBracketAt = t, g = null, Object.keys(h).length && (a.attributes.push(h), h = {}), q.dumpLinkHrefsNearby?.enabled && p.tagName && !p.openingTagEnds && (p.openingTagEnds = t)), (!S || ">" === e[t]) && void 0 !== a.lastOpeningBracketAt) {
+            if (a.quotes?.start && a.quotes.start < t && !a.quotes.end && h.nameEnds && h.equalsAt && !h.valueStarts && (h.valueStarts = t), !a.quotes && h.nameEnds && "=" === e[t] && !h.valueStarts && !h.equalsAt && (h.equalsAt = t), !a.quotes && h.nameStarts && h.nameEnds && !h.valueStarts && e[t].trim() && "=" !== e[t] && (a.attributes.push(h), h = {}), !a.quotes && h.nameStarts && !h.nameEnds && (S && "'\"".includes(e[h.nameStarts]) ? h.nameStarts < t && e[t] === e[h.nameStarts] && (h.nameEnds = t + 1, h.name = e.slice(h.nameStarts, h.nameEnds)) : e[t].trim() ? "=" === e[t] ? h.equalsAt || (h.nameEnds = t, h.equalsAt = t, h.name = e.slice(h.nameStarts, h.nameEnds)) : ("/" === e[t] || k(t) || _(t)) && (h.nameEnds = t, h.name = e.slice(h.nameStarts, h.nameEnds), a.attributes.push(h), h = {}) : (h.nameEnds = t, h.name = e.slice(h.nameStarts, h.nameEnds))), !a.quotes && a.nameEnds < t && !e[t - 1].trim() && e[t].trim() && !"<>/!".includes(e[t]) && !h.nameStarts && !a.lastClosingBracketAt && (h.nameStarts = t), null !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && "/" === e[t] && a.onlyPlausible && (a.onlyPlausible = !1), null !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && "/" !== e[t] && (void 0 === a.onlyPlausible && (e[t].trim() && !_(t) || a.slashPresent ? a.onlyPlausible = !1 : a.onlyPlausible = !0), e[t].trim() && void 0 === a.nameStarts && !_(t) && "/" !== e[t] && !k(t) && "!" !== e[t] && (a.nameStarts = t, a.nameContainsLetters = !1)), a.nameStarts && !a.quotes && "string" == typeof e[t] && e[t].toLowerCase() !== e[t].toUpperCase() && (a.nameContainsLetters = !0), k(t) && (Qf(a, e, t) || a.quotes.value && "number" == typeof a.lastOpeningBracketAt && eh(a.quotes.value, e.slice(a.lastOpeningBracketAt, t)) % 2 == 1 && !e.slice(a.lastOpeningBracketAt + 1, t).includes("<") && !e.slice(a.lastOpeningBracketAt + 1, t).includes(">")) && void 0 !== a.lastOpeningBracketAt && (a.lastClosingBracketAt = t, g = null, Object.keys(h).length && (a.attributes.push(h), h = {}), q.dumpLinkHrefsNearby?.enabled && p.tagName && !p.openingTagEnds && (p.openingTagEnds = t)), (!S || ">" === e[t]) && void 0 !== a.lastOpeningBracketAt) {
                 if (void 0 === a.lastClosingBracketAt) {
                     if (a.lastOpeningBracketAt < t && !_(t) && (void 0 === e[t + 1] || _(t + 1) && !a?.quotes?.value) && a.nameContainsLetters && "number" == typeof a.nameStarts) {
-                        if (a.name = e.slice(a.nameStarts, a.nameEnds || t + 1).toLowerCase(), (!o.length || o[o.length - 1][0] !== a.lastOpeningBracketAt) && o.push([a.lastOpeningBracketAt, t + 1]), q.ignoreTags.includes(a.name) || x(t, q, a) || !eh.has(a.name) && (a.onlyPlausible || q.stripRecognisedHTMLOnly)) {
+                        if (a.name = e.slice(a.nameStarts, a.nameEnds || t + 1).toLowerCase(), (!o.length || o[o.length - 1][0] !== a.lastOpeningBracketAt) && o.push([a.lastOpeningBracketAt, t + 1]), q.ignoreTags.includes(a.name) || x(t, q, a) || !th.has(a.name) && (a.onlyPlausible || q.stripRecognisedHTMLOnly)) {
                             a = {}, h = {};
                             continue
                         }
-                        if ((eh.has(a.name) || th.has(a.name)) && (!1 === a.onlyPlausible || !0 === a.onlyPlausible && a.attributes.length) || void 0 === e[t + 1]) {
+                        if ((th.has(a.name) || rh.has(a.name)) && (!1 === a.onlyPlausible || !0 === a.onlyPlausible && a.attributes.length) || void 0 === e[t + 1]) {
                             w(q);
                             let r, n = b(e, t, a.leftOuterWhitespace, t + 1, a.lastOpeningBracketAt, a.lastClosingBracketAt);
                             O && "script" === a.name && a.slashPresent && (O = !1), r = null === n || null === d ? null : `${n}${d}${n}`, q.cb({
                                 tag: a,
                                 deleteFrom: a.leftOuterWhitespace,
                                 deleteTo: t + 1,
                                 insert: r,
@@ -18060,15 +18080,15 @@
                             } else s.push([a.lastOpeningBracketAt, t + 1])
                     }
                 } else if (t > a.lastClosingBracketAt && e[t].trim() || void 0 === e[t + 1] || q.ignoreIndentations && "\r\n".includes(e[t])) {
                     let r = a.lastClosingBracketAt === t ? t + 1 : t;
                     q.trimOnlySpaces && r === R - 1 && null !== g && g < t && (r = g), (!o.length || o[o.length - 1][0] !== a.lastOpeningBracketAt) && o.push([a.lastOpeningBracketAt, a.lastClosingBracketAt + 1]);
                     let n = q.ignoreTags.includes(a.name),
                         l = x(t, q, a);
-                    if (!v || q.stripRecognisedHTMLOnly && "string" == typeof a.name && !eh.has(a.name.toLowerCase()) && !th.has(a.name.toLowerCase()) || !E && (n || l) || E && !q.onlyStripTags.includes(a.name) || q.ignoreTagsWithTheirContents.includes(a.name)) {
+                    if (!v || q.stripRecognisedHTMLOnly && "string" == typeof a.name && !th.has(a.name.toLowerCase()) && !rh.has(a.name.toLowerCase()) || !E && (n || l) || E && !q.onlyStripTags.includes(a.name) || q.ignoreTagsWithTheirContents.includes(a.name)) {
                         if (l)
                             if (a.slashPresent) {
                                 for (let e = i.length; e--;)
                                     if (i[e].name === a.name) {
                                         i.splice(e, 1);
                                         break
                                     } i.length || (v = !0)
@@ -18077,22 +18097,22 @@
                             tag: a,
                             deleteFrom: null,
                             deleteTo: null,
                             insert: null,
                             rangesArr: $,
                             proposedReturn: null
                         }), a = {}, h = {}
-                    } else if (!a.onlyPlausible || 0 === a.attributes.length && a.name && (eh.has(a.name.toLowerCase()) || th.has(a.name.toLowerCase())) || a.attributes?.some((e => e.equalsAt))) {
+                    } else if (!a.onlyPlausible || 0 === a.attributes.length && a.name && (th.has(a.name.toLowerCase()) || rh.has(a.name.toLowerCase())) || a.attributes?.some((e => e.equalsAt))) {
                         (!s.length || s[s.length - 1][0] !== a.lastOpeningBracketAt) && s.push([a.lastOpeningBracketAt, a.lastClosingBracketAt + 1]);
                         let n, i = b(e, t, a.leftOuterWhitespace, r, a.lastOpeningBracketAt, a.lastClosingBracketAt);
-                        d = "", m = !1, w(q, r), "string" == typeof d && d.length ? (n = `${i}${d}${"\n\n"===i?"\n":i}`, r === a.lastClosingBracketAt + 1 && (!e[r] || !rh.has(e[r])) && (n += " "), a.leftOuterWhitespace === a.lastOpeningBracketAt && $.last() && $.last()[1] < a.lastOpeningBracketAt && (!q?.dumpLinkHrefsNearby?.putOnNewLine || !rh.has(e[r])) && (n = " " + n)) : n = i, null !== n && (0 === a.leftOuterWhitespace || !Zf(e, r - 1)) && (!q.dumpLinkHrefsNearby?.enabled || "a" !== a.name) && (n = void 0);
+                        d = "", m = !1, w(q, r), "string" == typeof d && d.length ? (n = `${i}${d}${"\n\n"===i?"\n":i}`, r === a.lastClosingBracketAt + 1 && (!e[r] || !nh.has(e[r])) && (n += " "), a.leftOuterWhitespace === a.lastOpeningBracketAt && $.last() && $.last()[1] < a.lastOpeningBracketAt && (!q?.dumpLinkHrefsNearby?.putOnNewLine || !nh.has(e[r])) && (n = " " + n)) : n = i, null !== n && (0 === a.leftOuterWhitespace || !Jf(e, r - 1)) && (!q.dumpLinkHrefsNearby?.enabled || "a" !== a.name) && (n = void 0);
                         let o = 0;
-                        if (m && rh.has(e[r])) {
+                        if (m && nh.has(e[r])) {
                             q.dumpLinkHrefsNearby?.putOnNewLine && (n = `${e[r]}${n||""}`);
-                            let i = Zf(e, r);
+                            let i = Jf(e, r);
                             i && n?.endsWith("\n") ? o += i - t : (!i || i > t) && o++
                         }
                         q.cb({
                             tag: a,
                             deleteFrom: a.leftOuterWhitespace,
                             deleteTo: r + o,
                             insert: n,
@@ -18100,16 +18120,16 @@
                             proposedReturn: [a.leftOuterWhitespace, r + o, n]
                         }), A(), y(t, q, $)
                     } else a = {};
                     k(t) || (a = {})
                 }
                 S && (S = !1)
             }
-            if ((!O || "<" === e[t] && Zf(e, Zf(e, t)) && "/" === e[Zf(e, t)] && e.startsWith("script", Zf(e, Zf(e, t)))) && _(t) && !_(t - 1) && !"'\"".includes(e[t + 1]) && (!"'\"".includes(e[t + 2]) || /\w/.test(e[t + 1])) && ("c" !== e[t + 1] || ":" !== e[t + 2]) && ("f" !== e[t + 1] || "m" !== e[t + 2] || "t" !== e[t + 3] || ":" !== e[t + 4]) && ("s" !== e[t + 1] || "q" !== e[t + 2] || "l" !== e[t + 3] || ":" !== e[t + 4]) && ("x" !== e[t + 1] || ":" !== e[t + 2]) && ("f" !== e[t + 1] || "n" !== e[t + 2] || ":" !== e[t + 3]) && Xf(a, e, t)) {
-                if (k(Zf(e, t))) continue;
+            if ((!O || "<" === e[t] && Jf(e, Jf(e, t)) && "/" === e[Jf(e, t)] && e.startsWith("script", Jf(e, Jf(e, t)))) && _(t) && !_(t - 1) && !"'\"".includes(e[t + 1]) && (!"'\"".includes(e[t + 2]) || /\w/.test(e[t + 1])) && ("c" !== e[t + 1] || ":" !== e[t + 2]) && ("f" !== e[t + 1] || "m" !== e[t + 2] || "t" !== e[t + 3] || ":" !== e[t + 4]) && ("s" !== e[t + 1] || "q" !== e[t + 2] || "l" !== e[t + 3] || ":" !== e[t + 4]) && ("x" !== e[t + 1] || ":" !== e[t + 2]) && ("f" !== e[t + 1] || "n" !== e[t + 2] || ":" !== e[t + 3]) && Qf(a, e, t)) {
+                if (k(Jf(e, t))) continue;
                 if (a.nameEnds && a.nameEnds < t && !a.lastClosingBracketAt && (!0 === a.onlyPlausible && a.attributes && a.attributes.length || !1 === a.onlyPlausible)) {
                     let r = b(e, t, a.leftOuterWhitespace, t, a.lastOpeningBracketAt, t);
                     q.cb({
                         tag: a,
                         deleteFrom: a.leftOuterWhitespace,
                         deleteTo: t,
                         insert: r,
@@ -18133,15 +18153,15 @@
                                 rangesArr: $,
                                 proposedReturn: [a.leftOuterWhitespace, n, l]
                             }), t = i - 1, ">" === e[i] && (t = i), a = {}, h = {};
                             break
                         }
                 }
             }
-            e[t].trim() && 847 !== e[t].charCodeAt(0) ? (null !== l && (!a.quotes && h.equalsAt > l - 1 && h.nameEnds && h.equalsAt > h.nameEnds && '"' !== e[t] && "'" !== e[t] && (Du(h) && a.attributes.push(h), h = {}, a.equalsSpottedAt = void 0), l = null), f || (f = !0, v && !O && "number" == typeof c && t && c < t - 1 && (e.slice(c + 1, t).trim() ? c = null : q.ignoreIndentations || $.push([c + 1, t])))) : (null === l && (l = t, void 0 !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && a.nameStarts && a.nameStarts < a.lastOpeningBracketAt && t === a.lastOpeningBracketAt + 1 && !n.some((e => e.name === a.name)) && (a.onlyPlausible = !0, a.name = void 0, a.nameStarts = void 0)), ("\n" === e[t] || "\r" === e[t]) && (c = t, f && (f = !1))), " " === e[t] ? null === u && (u = t) : null !== u && (u = null), "script" === a.name && (O = !a.slashPresent)
+            e[t].trim() && 847 !== e[t].charCodeAt(0) ? (null !== l && (!a.quotes && h.equalsAt > l - 1 && h.nameEnds && h.equalsAt > h.nameEnds && '"' !== e[t] && "'" !== e[t] && (Cu(h) && a.attributes.push(h), h = {}, a.equalsSpottedAt = void 0), l = null), f || (f = !0, v && !O && "number" == typeof c && t && c < t - 1 && (e.slice(c + 1, t).trim() ? c = null : q.ignoreIndentations || $.push([c + 1, t])))) : (null === l && (l = t, void 0 !== a.lastOpeningBracketAt && a.lastOpeningBracketAt < t && a.nameStarts && a.nameStarts < a.lastOpeningBracketAt && t === a.lastOpeningBracketAt + 1 && !n.some((e => e.name === a.name)) && (a.onlyPlausible = !0, a.name = void 0, a.nameStarts = void 0)), ("\n" === e[t] || "\r" === e[t]) && (c = t, f && (f = !1))), " " === e[t] ? null === u && (u = t) : null !== u && (u = null), "script" === a.name && (O = !a.slashPresent)
         }
         if (e && !q.ignoreIndentations && (q.trimOnlySpaces && " " === e[0] || !q.trimOnlySpaces && !e[0].trim()))
             for (let t = 0; t < R; t++) {
                 if (q.trimOnlySpaces && " " !== e[t] || !q.trimOnlySpaces && e[t].trim()) {
                     $.push([0, t]);
                     break
                 }
@@ -18159,304 +18179,304 @@
             let r = $.ranges[$.ranges.length - 1][2];
             $.ranges[$.ranges.length - 1] = [t, $.ranges[$.ranges.length - 1][1]], r?.trim() && $.ranges[$.ranges.length - 1].push(r.trimEnd())
         }
         return {
             log: {
                 timeTakenInMilliseconds: Date.now() - r
             },
-            result: Uf(e, $.current()),
+            result: Vf(e, $.current()),
             ranges: $.current(),
             allTagLocations: o,
             filteredTagLocations: s
         }
     }
 
-    function ah(e) {
+    function lh(e) {
         let t, r, n, i;
         return {
             c() {
-                t = D("pre"), r = R("        "), n = R(e[0]), i = R("\n      ")
+                t = C("pre"), r = L("        "), n = L(e[0]), i = L("\n      ")
             },
             m(e, o) {
-                $(e, t, o), q(t, r), q(t, n), q(t, i)
+                O(e, t, o), E(t, r), E(t, n), E(t, i)
             },
             p(e, t) {
-                1 & t && U(n, e[0])
+                1 & t && V(n, e[0])
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function lh(e) {
-        let t, r = sh(e[0], {
+    function uh(e) {
+        let t, r = ah(e[0], {
             ignoreTags: e[2],
             dumpLinkHrefsNearby: {
                 enabled: !0,
                 putOnNewLine: !1,
                 wrapHeads: '<span class="link">&lt;',
                 wrapTails: "&gt;</span>"
             }
         }).result + "";
         return {
             c() {
-                t = D("blockquote")
+                t = C("blockquote")
             },
             m(e, n) {
-                $(e, t, n), t.innerHTML = r
+                O(e, t, n), t.innerHTML = r
             },
             p(e, n) {
-                1 & n && r !== (r = sh(e[0], {
+                1 & n && r !== (r = ah(e[0], {
                     ignoreTags: e[2],
                     dumpLinkHrefsNearby: {
                         enabled: !0,
                         putOnNewLine: !1,
                         wrapHeads: '<span class="link">&lt;',
                         wrapTails: "&gt;</span>"
                     }
                 }).result + "") && (t.innerHTML = r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function uh(t) {
+    function ch(t) {
         let r, n, i;
 
         function o(e, t) {
-            return e[1] ? lh : ah
+            return e[1] ? uh : lh
         }
         let s = o(t),
             a = s(t);
         return {
             c() {
-                r = D("div"), r.textContent = "changelog", n = L(), i = D("div"), a.c(), P(r, "class", "title-bar"), P(i, "class", "content svelte-n5l6oa")
+                r = C("div"), r.textContent = "changelog", n = N(), i = C("div"), a.c(), j(r, "class", "title-bar"), j(i, "class", "content svelte-n5l6oa")
             },
             m(e, t) {
-                $(e, r, t), $(e, n, t), $(e, i, t), a.m(i, null)
+                O(e, r, t), O(e, n, t), O(e, i, t), a.m(i, null)
             },
             p(e, [t]) {
                 s === (s = o(e)) && a ? a.p(e, t) : (a.d(1), a = s(e), a && (a.c(), a.m(i, null)))
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(n), e && O(i), a.d()
+                e && (S(r), S(n), S(i)), a.d()
             }
         }
     }
 
-    function ch(e, t, r) {
+    function fh(e, t, r) {
         let {
             changelog: n,
             renderAsHtml: i
         } = t;
         return e.$$set = e => {
             "changelog" in e && r(0, n = e.changelog), "renderAsHtml" in e && r(1, i = e.renderAsHtml)
         }, [n, i, ["b", "br", "code", "h1", "h2", "h3", "h4", "h5", "h6", "i", "li", "p", "pre", "ul"]]
     }
-    class fh extends Ze {
+    class hh extends Ye {
         constructor(e) {
-            super(), Ge(this, e, ch, uh, a, {
+            super(), Je(this, e, fh, ch, a, {
                 changelog: 0,
                 renderAsHtml: 1
             })
         }
     }
 
-    function hh(e, t, r) {
+    function ph(e, t, r) {
         const n = e.slice();
         return n[13] = t[r], n[15] = r, n
     }
 
-    function ph(e) {
-        let t, r, n = e[0].slice(1).map(wh).join(", ") + "";
+    function dh(e) {
+        let t, r, n = e[0].slice(1).map(_h).join(", ") + "";
         return {
             c() {
-                t = D("span"), r = R(n), P(t, "class", "remaining-folders svelte-1xsfw74")
+                t = C("span"), r = L(n), j(t, "class", "remaining-folders svelte-1xsfw74")
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, t) {
-                1 & t && n !== (n = e[0].slice(1).map(wh).join(", ") + "") && U(r, n)
+                1 & t && n !== (n = e[0].slice(1).map(_h).join(", ") + "") && V(r, n)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function dh(e) {
+    function mh(e) {
         let t;
         return {
             c() {
-                t = D("p"), t.textContent = "no matches found", P(t, "class", "unreconciled-message svelte-1xsfw74")
+                t = C("p"), t.textContent = "no matches found", j(t, "class", "unreconciled-message svelte-1xsfw74")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function mh(e) {
-        let t, r, n, i, o, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, E, T, C, N, F = e[1].length + "";
+    function gh(e) {
+        let t, r, n, i, o, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, q, T, $, R, I = e[1].length + "";
 
         function M(e, t) {
-            return e[5] ? vh : gh
+            return e[5] ? yh : vh
         }
-        let j = M(e),
-            V = j(e);
-        h = new Yn({
+        let P = M(e),
+            B = P(e);
+        h = new Kn({
             props: {
                 class: "icon icon-collapsed",
-                icon: fn
+                icon: hn
             }
-        }), d = new Yn({
+        }), d = new Kn({
             props: {
                 class: "icon icon-expanded",
-                icon: pn
+                icon: dn
             }
         });
-        let z = e[1],
-            H = [];
-        for (let t = 0; t < z.length; t += 1) H[t] = yh(hh(e, z, t));
-        return T = B(e[10][0]), {
-            c() {
-                t = D("details"), r = D("summary"), n = D("div"), i = D("div"), i.textContent = `${e[7]()}`, o = L(), s = D("div"), a = R("("), l = R(F), u = R(")\n            "), V.c(), c = L(), f = D("div"), Ve(h.$$.fragment), p = L(), Ve(d.$$.fragment), m = L(), g = D("ul");
-                for (let e = 0; e < H.length; e += 1) H[e].c();
-                v = L(), y = D("li"), b = D("input"), _ = L(), k = D("label"), x = D("span"), x.textContent = "skip", P(i, "aria-label", "installed version"), P(i, "class", "defn-or-version svelte-1xsfw74"), P(s, "aria-label", "selection"), P(s, "class", "defn-or-version svelte-1xsfw74"), P(f, "class", "svelte-1xsfw74"), P(n, "class", "selection-grid svelte-1xsfw74"), P(r, "class", "svelte-1xsfw74"), P(b, "type", "radio"), P(b, "id", w = "addon-selection-" + e[2] + "-skip"), b.__value = -1, b.value = b.__value, P(b, "class", "svelte-1xsfw74"), P(x, "class", "defn-or-version svelte-1xsfw74"), P(k, "for", A = "addon-selection-" + e[2] + "-skip"), P(k, "class", "svelte-1xsfw74"), P(y, "class", "svelte-1xsfw74"), P(g, "class", "selection-grid choices svelte-1xsfw74"), P(t, "class", "selection-controls svelte-1xsfw74"), t.open = e[3], T.p(b)
+        let H = Fe(e[1]),
+            W = [];
+        for (let t = 0; t < H.length; t += 1) W[t] = bh(ph(e, H, t));
+        return T = U(e[10][0]), {
+            c() {
+                t = C("details"), r = C("summary"), n = C("div"), i = C("div"), i.textContent = `${e[7]()}`, o = N(), s = C("div"), a = L("("), l = L(I), u = L(")\n            "), B.c(), c = N(), f = C("div"), He(h.$$.fragment), p = N(), He(d.$$.fragment), m = N(), g = C("ul");
+                for (let e = 0; e < W.length; e += 1) W[e].c();
+                v = N(), y = C("li"), b = C("input"), _ = N(), k = C("label"), x = C("span"), x.textContent = "skip", j(i, "aria-label", "installed version"), j(i, "class", "defn-or-version svelte-1xsfw74"), j(s, "aria-label", "selection"), j(s, "class", "defn-or-version svelte-1xsfw74"), j(f, "class", "svelte-1xsfw74"), j(n, "class", "selection-grid svelte-1xsfw74"), j(r, "class", "svelte-1xsfw74"), j(b, "type", "radio"), j(b, "id", w = "addon-selection-" + e[2] + "-skip"), b.__value = -1, z(b, b.__value), j(b, "class", "svelte-1xsfw74"), j(x, "class", "defn-or-version svelte-1xsfw74"), j(k, "for", A = "addon-selection-" + e[2] + "-skip"), j(k, "class", "svelte-1xsfw74"), j(y, "class", "svelte-1xsfw74"), j(g, "class", "selection-grid choices svelte-1xsfw74"), j(t, "class", "selection-controls svelte-1xsfw74"), t.open = e[3], T.p(b)
             },
             m(w, A) {
-                $(w, t, A), q(t, r), q(r, n), q(n, i), q(n, o), q(n, s), q(s, a), q(s, l), q(s, u), V.m(s, null), q(n, c), q(n, f), ze(h, f, null), q(f, p), ze(d, f, null), q(t, m), q(t, g);
-                for (let e = 0; e < H.length; e += 1) H[e] && H[e].m(g, null);
-                q(g, v), q(g, y), q(y, b), b.checked = b.__value === e[4], q(y, _), q(y, k), q(k, x), E = !0, C || (N = I(b, "change", e[12]), C = !0)
+                O(w, t, A), E(t, r), E(r, n), E(n, i), E(n, o), E(n, s), E(s, a), E(s, l), E(s, u), B.m(s, null), E(n, c), E(n, f), We(h, f, null), E(f, p), We(d, f, null), E(t, m), E(t, g);
+                for (let e = 0; e < W.length; e += 1) W[e] && W[e].m(g, null);
+                E(g, v), E(g, y), E(y, b), b.checked = b.__value === e[4], E(y, _), E(y, k), E(k, x), q = !0, $ || (R = F(b, "change", e[12]), $ = !0)
             },
             p(e, r) {
-                if ((!E || 2 & r) && F !== (F = e[1].length + "") && U(l, F), j === (j = M(e)) && V ? V.p(e, r) : (V.d(1), V = j(e), V && (V.c(), V.m(s, null))), 86 & r) {
+                if ((!q || 2 & r) && I !== (I = e[1].length + "") && V(l, I), P === (P = M(e)) && B ? B.p(e, r) : (B.d(1), B = P(e), B && (B.c(), B.m(s, null))), 86 & r) {
                     let t;
-                    for (z = e[1], t = 0; t < z.length; t += 1) {
-                        const n = hh(e, z, t);
-                        H[t] ? H[t].p(n, r) : (H[t] = yh(n), H[t].c(), H[t].m(g, v))
-                    }
-                    for (; t < H.length; t += 1) H[t].d(1);
-                    H.length = z.length
-                }(!E || 4 & r && w !== (w = "addon-selection-" + e[2] + "-skip")) && P(b, "id", w), 16 & r && (b.checked = b.__value === e[4]), (!E || 4 & r && A !== (A = "addon-selection-" + e[2] + "-skip")) && P(k, "for", A), (!E || 8 & r) && (t.open = e[3])
+                    for (H = Fe(e[1]), t = 0; t < H.length; t += 1) {
+                        const n = ph(e, H, t);
+                        W[t] ? W[t].p(n, r) : (W[t] = bh(n), W[t].c(), W[t].m(g, v))
+                    }
+                    for (; t < W.length; t += 1) W[t].d(1);
+                    W.length = H.length
+                }(!q || 4 & r && w !== (w = "addon-selection-" + e[2] + "-skip")) && j(b, "id", w), 16 & r && (b.checked = b.__value === e[4]), (!q || 4 & r && A !== (A = "addon-selection-" + e[2] + "-skip")) && j(k, "for", A), (!q || 8 & r) && (t.open = e[3])
             },
             i(e) {
-                E || (Oe(h.$$.fragment, e), Oe(d.$$.fragment, e), E = !0)
+                q || (Se(h.$$.fragment, e), Se(d.$$.fragment, e), q = !0)
             },
             o(e) {
-                Se(h.$$.fragment, e), Se(d.$$.fragment, e), E = !1
+                De(h.$$.fragment, e), De(d.$$.fragment, e), q = !1
             },
             d(e) {
-                e && O(t), V.d(), He(h), He(d), S(H, e), T.r(), C = !1, N()
+                e && S(t), B.d(), Ge(h), Ge(d), D(W, e), T.r(), $ = !1, R()
             }
         }
     }
 
-    function gh(t) {
+    function vh(t) {
         let r;
         return {
             c() {
-                r = R("skip")
+                r = L("skip")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function vh(e) {
+    function yh(e) {
         let t, r, n, i, o, s, a, l = e[5].source + "",
             u = e[5].slug + "",
             c = e[5].version + "";
         return {
             c() {
-                t = R(l), r = R(":"), n = R(u), i = R("=="), o = D("span"), s = R(c), P(o, "title", a = e[5].date_published), P(o, "class", "svelte-1xsfw74")
+                t = L(l), r = L(":"), n = L(u), i = L("=="), o = C("span"), s = L(c), j(o, "title", a = e[5].date_published), j(o, "class", "svelte-1xsfw74")
             },
             m(e, a) {
-                $(e, t, a), $(e, r, a), $(e, n, a), $(e, i, a), $(e, o, a), q(o, s)
+                O(e, t, a), O(e, r, a), O(e, n, a), O(e, i, a), O(e, o, a), E(o, s)
             },
             p(e, r) {
-                32 & r && l !== (l = e[5].source + "") && U(t, l), 32 & r && u !== (u = e[5].slug + "") && U(n, u), 32 & r && c !== (c = e[5].version + "") && U(s, c), 32 & r && a !== (a = e[5].date_published) && P(o, "title", a)
+                32 & r && l !== (l = e[5].source + "") && V(t, l), 32 & r && u !== (u = e[5].slug + "") && V(n, u), 32 & r && c !== (c = e[5].version + "") && V(s, c), 32 & r && a !== (a = e[5].date_published) && j(o, "title", a)
             },
             d(e) {
-                e && O(t), e && O(r), e && O(n), e && O(i), e && O(o)
+                e && (S(t), S(r), S(n), S(i), S(o))
             }
         }
     }
 
-    function yh(e) {
+    function bh(e) {
         let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b = e[13].source + "",
             w = e[13].slug + "",
             _ = e[13].version + "";
 
         function k() {
             return e[11](e[13])
         }
-        return g = B(e[10][0]), {
+        return g = U(e[10][0]), {
             c() {
-                t = D("li"), r = D("input"), i = L(), s = D("label"), a = D("span"), l = R(b), u = R(":"), c = R(w), f = R("=="), h = R(_), p = L(), d = D("button"), d.textContent = "[↗]", P(r, "type", "radio"), P(r, "id", n = "addon-selection-" + e[2] + "-" + e[15]), r.__value = e[15], r.value = r.__value, P(r, "class", "svelte-1xsfw74"), P(a, "class", "defn-or-version svelte-1xsfw74"), P(d, "role", "link"), P(d, "class", "svelte-1xsfw74"), P(s, "for", m = "addon-selection-" + e[2] + "-" + e[15]), P(s, "class", "svelte-1xsfw74"), P(t, "class", "svelte-1xsfw74"), g.p(r)
+                t = C("li"), r = C("input"), i = N(), s = C("label"), a = C("span"), l = L(b), u = L(":"), c = L(w), f = L("=="), h = L(_), p = N(), d = C("button"), d.textContent = "[↗]", j(r, "type", "radio"), j(r, "id", n = "addon-selection-" + e[2] + "-" + e[15]), r.__value = e[15], z(r, r.__value), j(r, "class", "svelte-1xsfw74"), j(a, "class", "defn-or-version svelte-1xsfw74"), j(d, "role", "link"), j(d, "class", "svelte-1xsfw74"), j(s, "for", m = "addon-selection-" + e[2] + "-" + e[15]), j(s, "class", "svelte-1xsfw74"), j(t, "class", "svelte-1xsfw74"), g.p(r)
             },
             m(n, o) {
-                $(n, t, o), q(t, r), r.checked = r.__value === e[4], q(t, i), q(t, s), q(s, a), q(a, l), q(a, u), q(a, c), q(a, f), q(a, h), q(s, p), q(s, d), v || (y = [I(r, "change", e[9]), I(d, "click", M(F(k)))], v = !0)
+                O(n, t, o), E(t, r), r.checked = r.__value === e[4], E(t, i), E(t, s), E(s, a), E(a, l), E(a, u), E(a, c), E(a, f), E(a, h), E(s, p), E(s, d), v || (y = [F(r, "change", e[9]), F(d, "click", P(M(k)))], v = !0)
             },
             p(t, i) {
-                e = t, 4 & i && n !== (n = "addon-selection-" + e[2] + "-" + e[15]) && P(r, "id", n), 16 & i && (r.checked = r.__value === e[4]), 2 & i && b !== (b = e[13].source + "") && U(l, b), 2 & i && w !== (w = e[13].slug + "") && U(c, w), 2 & i && _ !== (_ = e[13].version + "") && U(h, _), 4 & i && m !== (m = "addon-selection-" + e[2] + "-" + e[15]) && P(s, "for", m)
+                e = t, 4 & i && n !== (n = "addon-selection-" + e[2] + "-" + e[15]) && j(r, "id", n), 16 & i && (r.checked = r.__value === e[4]), 2 & i && b !== (b = e[13].source + "") && V(l, b), 2 & i && w !== (w = e[13].slug + "") && V(c, w), 2 & i && _ !== (_ = e[13].version + "") && V(h, _), 4 & i && m !== (m = "addon-selection-" + e[2] + "-" + e[15]) && j(s, "for", m)
             },
             d(e) {
-                e && O(t), g.r(), v = !1, o(y)
+                e && S(t), g.r(), v = !1, o(y)
             }
         }
     }
 
-    function bh(e) {
+    function wh(e) {
         let t, r, n, i, o, s, a, l, u, c = e[0][0].name + "",
-            f = e[0].length > 1 && ph(e),
-            h = !e[1].length && dh(),
-            p = e[1].length && mh(e);
+            f = e[0].length > 1 && dh(e),
+            h = !e[1].length && mh(),
+            p = e[1].length && gh(e);
         return {
             c() {
-                t = D("div"), r = D("div"), n = D("div"), i = D("span"), o = R(c), s = L(), f && f.c(), a = L(), h && h.c(), l = L(), p && p.c(), P(i, "class", "main-folder"), P(n, "class", "folders svelte-1xsfw74"), P(r, "class", "header svelte-1xsfw74"), P(t, "class", "addon-stub svelte-1xsfw74")
+                t = C("div"), r = C("div"), n = C("div"), i = C("span"), o = L(c), s = N(), f && f.c(), a = N(), h && h.c(), l = N(), p && p.c(), j(i, "class", "main-folder"), j(n, "class", "folders svelte-1xsfw74"), j(r, "class", "header svelte-1xsfw74"), j(t, "class", "addon-stub svelte-1xsfw74")
             },
             m(e, c) {
-                $(e, t, c), q(t, r), q(r, n), q(n, i), q(i, o), q(n, s), f && f.m(n, null), q(r, a), h && h.m(r, null), q(t, l), p && p.m(t, null), u = !0
+                O(e, t, c), E(t, r), E(r, n), E(n, i), E(i, o), E(n, s), f && f.m(n, null), E(r, a), h && h.m(r, null), E(t, l), p && p.m(t, null), u = !0
             },
             p(e, [i]) {
-                (!u || 1 & i) && c !== (c = e[0][0].name + "") && U(o, c), e[0].length > 1 ? f ? f.p(e, i) : (f = ph(e), f.c(), f.m(n, null)) : f && (f.d(1), f = null), e[1].length ? h && (h.d(1), h = null) : h || (h = dh(), h.c(), h.m(r, null)), e[1].length ? p ? (p.p(e, i), 2 & i && Oe(p, 1)) : (p = mh(e), p.c(), Oe(p, 1), p.m(t, null)) : p && (Te(), Se(p, 1, 1, (() => {
+                (!u || 1 & i) && c !== (c = e[0][0].name + "") && V(o, c), e[0].length > 1 ? f ? f.p(e, i) : (f = dh(e), f.c(), f.m(n, null)) : f && (f.d(1), f = null), e[1].length ? h && (h.d(1), h = null) : h || (h = mh(), h.c(), h.m(r, null)), e[1].length ? p ? (p.p(e, i), 2 & i && Se(p, 1)) : (p = gh(e), p.c(), Se(p, 1), p.m(t, null)) : p && ($e(), De(p, 1, 1, (() => {
                     p = null
-                })), $e())
+                })), Oe())
             },
             i(e) {
-                u || (Oe(p), u = !0)
+                u || (Se(p), u = !0)
             },
             o(e) {
-                Se(p), u = !1
+                De(p), u = !1
             },
             d(e) {
-                e && O(t), f && f.d(), h && h.d(), p && p.d()
+                e && S(t), f && f.d(), h && h.d(), p && p.d()
             }
         }
     }
-    const wh = e => e.name;
+    const _h = e => e.name;
 
-    function _h(e, t, r) {
+    function kh(e, t, r) {
         let n;
-        c(e, nn, (e => r(6, n = e)));
+        c(e, on, (e => r(6, n = e)));
         let i, {
                 selections: o,
                 folders: s,
                 choices: a,
                 idx: l,
                 expanded: u = !1
             } = t,
@@ -18472,466 +18492,466 @@
                 []
             ], e => n.openUrl(e.url),
             function() {
                 f = this.__value, r(4, f)
             }
         ]
     }
-    class kh extends Ze {
+    class xh extends Ye {
         constructor(e) {
-            super(), Ge(this, e, _h, bh, a, {
+            super(), Je(this, e, kh, wh, a, {
                 selections: 8,
                 folders: 0,
                 choices: 1,
                 idx: 2,
                 expanded: 3
             })
         }
     }
-    var xh, Ah, qh;
+    var Ah, qh, Eh;
 
-    function Eh(t) {
+    function Th(t) {
         let r, n, i, o, s, a;
         return {
             c() {
-                r = D("div"), n = C("svg"), i = C("circle"), P(i, "r", t[4] - Th), P(i, "cx", t[4]), P(i, "cy", t[4]), P(i, "style", o = `\n        stroke-dasharray: ${t[5]} ${t[5]};\n        stroke-dashoffset: ${t[3]};\n        stroke-width: ${Th};\n      `), P(i, "class", "svelte-1iz2oiq"), J(i, "indeterminate", t[2]), P(n, "height", t[0]), P(n, "width", t[0]), P(n, "viewBox", s = "0 0 " + t[0] + " " + t[0]), P(n, "class", "svelte-1iz2oiq"), P(r, "role", "progressbar"), P(r, "aria-valuemin", 0), P(r, "aria-valuemax", 1), P(r, "aria-valuenow", a = t[2] ? void 0 : t[1])
+                r = C("div"), n = R("svg"), i = R("circle"), j(i, "r", t[4] - $h), j(i, "cx", t[4]), j(i, "cy", t[4]), j(i, "style", o = `\n        stroke-dasharray: ${t[5]} ${t[5]};\n        stroke-dashoffset: ${t[3]};\n        stroke-width: ${$h};\n      `), j(i, "class", "svelte-1iz2oiq"), Y(i, "indeterminate", t[2]), j(n, "height", t[0]), j(n, "width", t[0]), j(n, "viewBox", s = "0 0 " + t[0] + " " + t[0]), j(n, "class", "svelte-1iz2oiq"), j(r, "role", "progressbar"), j(r, "aria-valuemin", 0), j(r, "aria-valuemax", 1), j(r, "aria-valuenow", a = t[2] ? void 0 : t[1])
             },
             m(e, t) {
-                $(e, r, t), q(r, n), q(n, i)
+                O(e, r, t), E(r, n), E(n, i)
             },
             p(e, [t]) {
-                8 & t && o !== (o = `\n        stroke-dasharray: ${e[5]} ${e[5]};\n        stroke-dashoffset: ${e[3]};\n        stroke-width: ${Th};\n      `) && P(i, "style", o), 4 & t && J(i, "indeterminate", e[2]), 1 & t && P(n, "height", e[0]), 1 & t && P(n, "width", e[0]), 1 & t && s !== (s = "0 0 " + e[0] + " " + e[0]) && P(n, "viewBox", s), 6 & t && a !== (a = e[2] ? void 0 : e[1]) && P(r, "aria-valuenow", a)
+                8 & t && o !== (o = `\n        stroke-dasharray: ${e[5]} ${e[5]};\n        stroke-dashoffset: ${e[3]};\n        stroke-width: ${$h};\n      `) && j(i, "style", o), 4 & t && Y(i, "indeterminate", e[2]), 1 & t && j(n, "height", e[0]), 1 & t && j(n, "width", e[0]), 1 & t && s !== (s = "0 0 " + e[0] + " " + e[0]) && j(n, "viewBox", s), 6 & t && a !== (a = e[2] ? void 0 : e[1]) && j(r, "aria-valuenow", a)
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }! function(e) {
         e[e.Installed = 0] = "Installed", e[e.FilterInstalled = 1] = "FilterInstalled", e[e.ReconcileInstalled = 2] = "ReconcileInstalled", e[e.Search = 3] = "Search", e[e.Reconcile = 4] = "Reconcile"
-    }(xh || (xh = {})),
+    }(Ah || (Ah = {})),
     function(e) {
         e[e.Dense = 0] = "Dense", e[e.Compact = 1] = "Compact", e[e.Expanded = 2] = "Expanded"
-    }(Ah || (Ah = {})),
+    }(qh || (qh = {})),
     function(e) {
         e[e.VisitHomepage = 0] = "VisitHomepage", e[e.ViewChangelog = 1] = "ViewChangelog", e[e.RevealFolder = 2] = "RevealFolder", e[e.Resolve = 3] = "Resolve", e[e.Rollback = 4] = "Rollback", e[e.Pin = 5] = "Pin", e[e.Unpin = 6] = "Unpin", e[e.Unreconcile = 7] = "Unreconcile", e[e.InstallAndReplace = 8] = "InstallAndReplace"
-    }(qh || (qh = {}));
-    const Th = 2;
+    }(Eh || (Eh = {}));
+    const $h = 2;
 
-    function $h(e, t, r) {
+    function Oh(e, t, r) {
         let n, i, {
             diameter: o,
             progress: s
         } = t;
         const a = o / 2,
-            l = 2 * (a - Th) * Math.PI;
+            l = 2 * (a - $h) * Math.PI;
         return e.$$set = e => {
             "diameter" in e && r(0, o = e.diameter), "progress" in e && r(1, s = e.progress)
         }, e.$$.update = () => {
             2 & e.$$.dirty && r(2, n = 0 === s), 6 & e.$$.dirty && r(3, i = l - (n ? .75 : s) * l)
         }, [o, s, n, i, a, l]
     }
-    class Oh extends Ze {
+    class Sh extends Ye {
         constructor(e) {
-            super(), Ge(this, e, $h, Eh, a, {
+            super(), Je(this, e, Oh, Th, a, {
                 diameter: 0,
                 progress: 1
             })
         }
     }
 
-    function Sh(e, t, r) {
+    function Dh(e, t, r) {
         const n = e.slice();
         return n[30] = t[r], n
     }
 
-    function Dh(e) {
+    function Ch(e) {
         let t, r, n, i, o, s, a, l, u;
-        return o = new Yn({
+        return o = new Kn({
             props: {
-                icon: wn
+                icon: _n
             }
-        }), a = B(e[15][0]), {
+        }), a = U(e[15][0]), {
             c() {
-                t = D("li"), r = D("input"), n = L(), i = D("label"), Ve(o.$$.fragment), P(r, "class", "control svelte-nmk0ob"), P(r, "id", "__radio-reconcile-installed"), P(r, "type", "radio"), r.__value = xh.ReconcileInstalled, r.value = r.__value, P(i, "class", "control svelte-nmk0ob"), P(i, "for", "__radio-reconcile-installed"), P(i, "aria-label", "change add-on sources"), P(i, "title", "change add-on sources"), P(t, "class", "svelte-nmk0ob"), a.p(r)
+                t = C("li"), r = C("input"), n = N(), i = C("label"), He(o.$$.fragment), j(r, "class", "control svelte-nmk0ob"), j(r, "id", "__radio-reconcile-installed"), j(r, "type", "radio"), r.__value = Ah.ReconcileInstalled, z(r, r.__value), j(i, "class", "control svelte-nmk0ob"), j(i, "for", "__radio-reconcile-installed"), j(i, "aria-label", "change add-on sources"), j(i, "title", "change add-on sources"), j(t, "class", "svelte-nmk0ob"), a.p(r)
             },
             m(a, c) {
-                $(a, t, c), q(t, r), r.checked = r.__value === e[0], q(t, n), q(t, i), ze(o, i, null), s = !0, l || (u = I(r, "change", e[17]), l = !0)
+                O(a, t, c), E(t, r), r.checked = r.__value === e[0], E(t, n), E(t, i), We(o, i, null), s = !0, l || (u = F(r, "change", e[17]), l = !0)
             },
             p(e, t) {
                 1 & t[0] && (r.checked = r.__value === e[0])
             },
             i(e) {
-                s || (Oe(o.$$.fragment, e), s = !0)
+                s || (Se(o.$$.fragment, e), s = !0)
             },
             o(e) {
-                Se(o.$$.fragment, e), s = !1
+                De(o.$$.fragment, e), s = !1
             },
             d(e) {
-                e && O(t), He(o), a.r(), l = !1, u()
+                e && S(t), Ge(o), a.r(), l = !1, u()
             }
         }
     }
 
-    function Ch(t) {
+    function Rh(t) {
         let r, n, i, o, s, a;
-        return i = new Yn({
+        return i = new Kn({
             props: {
-                icon: kn
+                icon: xn
             }
         }), {
             c() {
-                r = D("li"), n = D("button"), Ve(i.$$.fragment), P(n, "class", "control svelte-nmk0ob"), P(n, "aria-label", "condense/expand add-on cells"), P(n, "title", "condense/expand add-on cells"), P(r, "class", "svelte-nmk0ob")
+                r = C("li"), n = C("button"), He(i.$$.fragment), j(n, "class", "control svelte-nmk0ob"), j(n, "aria-label", "condense/expand add-on cells"), j(n, "title", "condense/expand add-on cells"), j(r, "class", "svelte-nmk0ob")
             },
             m(e, l) {
-                $(e, r, l), q(r, n), ze(i, n, null), o = !0, s || (a = I(n, "click", t[18]), s = !0)
+                O(e, r, l), E(r, n), We(i, n, null), o = !0, s || (a = F(n, "click", t[18]), s = !0)
             },
             p: e,
             i(e) {
-                o || (Oe(i.$$.fragment, e), o = !0)
+                o || (Se(i.$$.fragment, e), o = !0)
             },
             o(e) {
-                Se(i.$$.fragment, e), o = !1
+                De(i.$$.fragment, e), o = !1
             },
             d(e) {
-                e && O(r), He(i), s = !1, a()
+                e && S(r), Ge(i), s = !1, a()
             }
         }
     }
 
-    function Rh(e) {
+    function Lh(e) {
         let t, r, n, i, s, a, l, u, c, f, h;
-        return s = new Yn({
+        return s = new Kn({
             props: {
-                icon: dn
+                icon: mn
             }
         }), {
             c() {
-                t = D("li"), r = D("input"), n = L(), i = D("label"), Ve(s.$$.fragment), a = L(), l = D("li"), u = D("input"), P(r, "class", "control svelte-nmk0ob"), P(r, "id", "__search-installed"), P(r, "type", "checkbox"), P(i, "class", "control svelte-nmk0ob"), P(i, "for", "__search-installed"), P(i, "aria-label", "search installed add-ons"), P(i, "title", "search installed add-ons"), P(t, "class", "svelte-nmk0ob"), P(u, "class", "control search-control svelte-nmk0ob"), P(u, "type", "text"), P(u, "placeholder", "search"), P(l, "class", "svelte-nmk0ob")
+                t = C("li"), r = C("input"), n = N(), i = C("label"), He(s.$$.fragment), a = N(), l = C("li"), u = C("input"), j(r, "class", "control svelte-nmk0ob"), j(r, "id", "__search-installed"), j(r, "type", "checkbox"), j(i, "class", "control svelte-nmk0ob"), j(i, "for", "__search-installed"), j(i, "aria-label", "search installed add-ons"), j(i, "title", "search installed add-ons"), j(t, "class", "svelte-nmk0ob"), j(u, "class", "control search-control svelte-nmk0ob"), j(u, "type", "text"), j(u, "placeholder", "search"), j(l, "class", "svelte-nmk0ob")
             },
             m(o, p) {
-                $(o, t, p), q(t, r), r.checked = e[2], q(t, n), q(t, i), ze(s, i, null), $(o, a, p), $(o, l, p), q(l, u), e[21](u), V(u, e[1]), c = !0, f || (h = [I(r, "change", e[20]), I(u, "input", e[22]), I(u, "keydown", e[23])], f = !0)
+                O(o, t, p), E(t, r), r.checked = e[2], E(t, n), E(t, i), We(s, i, null), O(o, a, p), O(o, l, p), E(l, u), e[21](u), z(u, e[1]), c = !0, f || (h = [F(r, "change", e[20]), F(u, "input", e[22]), F(u, "keydown", e[23])], f = !0)
             },
             p(e, t) {
-                4 & t[0] && (r.checked = e[2]), 2 & t[0] && u.value !== e[1] && V(u, e[1])
+                4 & t[0] && (r.checked = e[2]), 2 & t[0] && u.value !== e[1] && z(u, e[1])
             },
             i(e) {
-                c || (Oe(s.$$.fragment, e), c = !0)
+                c || (Se(s.$$.fragment, e), c = !0)
             },
             o(e) {
-                Se(s.$$.fragment, e), c = !1
+                De(s.$$.fragment, e), c = !1
             },
             d(r) {
-                r && O(t), He(s), r && O(a), r && O(l), e[21](null), f = !1, o(h)
+                r && (S(t), S(a), S(l)), Ge(s), e[21](null), f = !1, o(h)
             }
         }
     }
 
-    function Lh(t) {
-        let r, n, i, o, s = Object.values(Vr),
+    function Nh(t) {
+        let r, n, i, o, s = Fe(Object.values(zr)),
             a = [];
-        for (let e = 0; e < s.length; e += 1) a[e] = Nh(Sh(t, s, e));
+        for (let e = 0; e < s.length; e += 1) a[e] = Ih(Dh(t, s, e));
         return {
             c() {
-                r = D("li"), n = D("select");
+                r = C("li"), n = C("select");
                 for (let e = 0; e < a.length; e += 1) a[e].c();
-                P(n, "class", "control reconciliation-stage-control svelte-nmk0ob"), P(n, "aria-label", "reconciliation stage"), n.disabled = t[9], void 0 === t[3] && ge((() => t[19].call(n))), P(r, "class", "svelte-nmk0ob")
+                j(n, "class", "control reconciliation-stage-control svelte-nmk0ob"), j(n, "aria-label", "reconciliation stage"), n.disabled = t[9], void 0 === t[3] && ve((() => t[19].call(n))), j(r, "class", "svelte-nmk0ob")
             },
             m(e, s) {
-                $(e, r, s), q(r, n);
+                O(e, r, s), E(r, n);
                 for (let e = 0; e < a.length; e += 1) a[e] && a[e].m(n, null);
-                z(n, t[3], !0), i || (o = I(n, "change", t[19]), i = !0)
+                H(n, t[3], !0), i || (o = F(n, "change", t[19]), i = !0)
             },
             p(e, t) {
                 if (0 & t) {
                     let r;
-                    for (s = Object.values(Vr), r = 0; r < s.length; r += 1) {
-                        const i = Sh(e, s, r);
-                        a[r] ? a[r].p(i, t) : (a[r] = Nh(i), a[r].c(), a[r].m(n, null))
+                    for (s = Fe(Object.values(zr)), r = 0; r < s.length; r += 1) {
+                        const i = Dh(e, s, r);
+                        a[r] ? a[r].p(i, t) : (a[r] = Ih(i), a[r].c(), a[r].m(n, null))
                     }
                     for (; r < a.length; r += 1) a[r].d(1);
                     a.length = s.length
                 }
-                512 & t[0] && (n.disabled = e[9]), 8 & t[0] && z(n, e[3])
+                512 & t[0] && (n.disabled = e[9]), 8 & t[0] && H(n, e[3])
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), S(a, e), i = !1, o()
+                e && S(r), D(a, e), i = !1, o()
             }
         }
     }
 
-    function Nh(t) {
+    function Ih(t) {
         let r, n, i = t[30] + "";
         return {
             c() {
-                r = D("option"), n = R(i), r.__value = t[30], r.value = r.__value, P(r, "class", "svelte-nmk0ob")
+                r = C("option"), n = L(i), r.__value = t[30], z(r, r.__value), j(r, "class", "svelte-nmk0ob")
             },
             m(e, t) {
-                $(e, r, t), q(r, n)
+                O(e, r, t), E(r, n)
             },
             p: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Ih(e) {
+    function Fh(e) {
         let t, r, n;
-        return r = new Oh({
+        return r = new Sh({
             props: {
                 diameter: 18,
                 progress: 0
             }
         }), {
             c() {
-                t = D("div"), Ve(r.$$.fragment), P(t, "class", "progress-indicator svelte-nmk0ob")
+                t = C("div"), He(r.$$.fragment), j(t, "class", "progress-indicator svelte-nmk0ob")
             },
             m(e, i) {
-                $(e, t, i), ze(r, t, null), n = !0
+                O(e, t, i), We(r, t, null), n = !0
             },
             i(e) {
-                n || (Oe(r.$$.fragment, e), n = !0)
+                n || (Se(r.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(r.$$.fragment, e), n = !1
+                De(r.$$.fragment, e), n = !1
             },
             d(e) {
-                e && O(t), He(r)
+                e && S(t), Ge(r)
             }
         }
     }
 
-    function Fh(e) {
+    function Mh(e) {
         let t, r, n;
-        return r = new Oh({
+        return r = new Sh({
             props: {
                 diameter: 18,
                 progress: 0
             }
         }), {
             c() {
-                t = D("div"), Ve(r.$$.fragment), P(t, "class", "progress-indicator svelte-nmk0ob")
+                t = C("div"), He(r.$$.fragment), j(t, "class", "progress-indicator svelte-nmk0ob")
             },
             m(e, i) {
-                $(e, t, i), ze(r, t, null), n = !0
+                O(e, t, i), We(r, t, null), n = !0
             },
             i(e) {
-                n || (Oe(r.$$.fragment, e), n = !0)
+                n || (Se(r.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(r.$$.fragment, e), n = !1
+                De(r.$$.fragment, e), n = !1
             },
             d(e) {
-                e && O(t), He(r)
+                e && S(t), Ge(r)
             }
         }
     }
 
-    function Mh(t) {
+    function Ph(t) {
         let r, n, i, o, s;
         return {
             c() {
-                r = D("li"), n = D("button"), i = R("switch sources"), P(n, "class", "control svelte-nmk0ob"), n.disabled = t[9], P(r, "class", "svelte-nmk0ob")
+                r = C("li"), n = C("button"), i = L("switch sources"), j(n, "class", "control svelte-nmk0ob"), n.disabled = t[9], j(r, "class", "svelte-nmk0ob")
             },
             m(e, a) {
-                $(e, r, a), q(r, n), q(n, i), o || (s = I(n, "click", t[29]), o = !0)
+                O(e, r, a), E(r, n), E(n, i), o || (s = F(n, "click", t[29]), o = !0)
             },
             p(e, t) {
                 512 & t[0] && (n.disabled = e[9])
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), o = !1, s()
+                e && S(r), o = !1, s()
             }
         }
     }
 
-    function Ph(t) {
+    function jh(t) {
         let r, n, i, s, a, l, u, c, f, h;
         return {
             c() {
-                r = D("li"), n = D("button"), i = R("install"), a = L(), l = D("li"), u = D("button"), c = R("automate"), P(n, "class", "control svelte-nmk0ob"), n.disabled = s = !t[10] || t[9], P(r, "class", "svelte-nmk0ob"), P(u, "class", "control svelte-nmk0ob"), u.disabled = t[9], P(l, "class", "svelte-nmk0ob")
+                r = C("li"), n = C("button"), i = L("install"), a = N(), l = C("li"), u = C("button"), c = L("automate"), j(n, "class", "control svelte-nmk0ob"), n.disabled = s = !t[10] || t[9], j(r, "class", "svelte-nmk0ob"), j(u, "class", "control svelte-nmk0ob"), u.disabled = t[9], j(l, "class", "svelte-nmk0ob")
             },
             m(e, o) {
-                $(e, r, o), q(r, n), q(n, i), $(e, a, o), $(e, l, o), q(l, u), q(u, c), f || (h = [I(n, "click", t[27]), I(u, "click", t[28])], f = !0)
+                O(e, r, o), E(r, n), E(n, i), O(e, a, o), O(e, l, o), E(l, u), E(u, c), f || (h = [F(n, "click", t[27]), F(u, "click", t[28])], f = !0)
             },
             p(e, t) {
                 1536 & t[0] && s !== (s = !e[10] || e[9]) && (n.disabled = s), 512 & t[0] && (u.disabled = e[9])
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(a), e && O(l), f = !1, o(h)
+                e && (S(r), S(a), S(l)), f = !1, o(h)
             }
         }
     }
 
-    function jh(e) {
+    function Bh(e) {
         let t, r, n, i, o, s;
-        return n = new Yn({
+        return n = new Kn({
             props: {
-                icon: bn
+                icon: wn
             }
         }), {
             c() {
-                t = D("li"), r = D("button"), Ve(n.$$.fragment), P(r, "class", "control svelte-nmk0ob"), P(r, "aria-label", "show search options"), J(r, "dirty", e[4]), P(t, "class", "svelte-nmk0ob")
+                t = C("li"), r = C("button"), He(n.$$.fragment), j(r, "class", "control svelte-nmk0ob"), j(r, "aria-label", "show search options"), Y(r, "dirty", e[4]), j(t, "class", "svelte-nmk0ob")
             },
             m(a, l) {
-                $(a, t, l), q(t, r), ze(n, r, null), i = !0, o || (s = I(r, "click", e[26]), o = !0)
+                O(a, t, l), E(t, r), We(n, r, null), i = !0, o || (s = F(r, "click", e[26]), o = !0)
             },
             p(e, t) {
-                (!i || 16 & t[0]) && J(r, "dirty", e[4])
+                (!i || 16 & t[0]) && Y(r, "dirty", e[4])
             },
             i(e) {
-                i || (Oe(n.$$.fragment, e), i = !0)
+                i || (Se(n.$$.fragment, e), i = !0)
             },
             o(e) {
-                Se(n.$$.fragment, e), i = !1
+                De(n.$$.fragment, e), i = !1
             },
             d(e) {
-                e && O(t), He(n), o = !1, s()
+                e && S(t), Ge(n), o = !1, s()
             }
         }
     }
 
-    function Bh(t) {
+    function Uh(t) {
         let r, n, i, s, a, l, u, c, f, h, p = t[8] ? `update ${t[8]}` : "no updates";
         return {
             c() {
-                r = D("li"), n = D("button"), i = R("refresh"), s = L(), a = D("li"), l = D("button"), u = R(p), P(n, "class", "control svelte-nmk0ob"), n.disabled = t[5], P(r, "class", "svelte-nmk0ob"), P(l, "class", "control svelte-nmk0ob"), l.disabled = c = t[6] || t[5] || !t[8], P(a, "class", "svelte-nmk0ob")
+                r = C("li"), n = C("button"), i = L("refresh"), s = N(), a = C("li"), l = C("button"), u = L(p), j(n, "class", "control svelte-nmk0ob"), n.disabled = t[5], j(r, "class", "svelte-nmk0ob"), j(l, "class", "control svelte-nmk0ob"), l.disabled = c = t[6] || t[5] || !t[8], j(a, "class", "svelte-nmk0ob")
             },
             m(e, o) {
-                $(e, r, o), q(r, n), q(n, i), $(e, s, o), $(e, a, o), q(a, l), q(l, u), f || (h = [I(n, "click", t[24]), I(l, "click", t[25])], f = !0)
+                O(e, r, o), E(r, n), E(n, i), O(e, s, o), O(e, a, o), E(a, l), E(l, u), f || (h = [F(n, "click", t[24]), F(l, "click", t[25])], f = !0)
             },
             p(e, t) {
-                32 & t[0] && (n.disabled = e[5]), 256 & t[0] && p !== (p = e[8] ? `update ${e[8]}` : "no updates") && U(u, p), 352 & t[0] && c !== (c = e[6] || e[5] || !e[8]) && (l.disabled = c)
+                32 & t[0] && (n.disabled = e[5]), 256 & t[0] && p !== (p = e[8] ? `update ${e[8]}` : "no updates") && V(u, p), 352 & t[0] && c !== (c = e[6] || e[5] || !e[8]) && (l.disabled = c)
             },
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(s), e && O(a), f = !1, o(h)
+                e && (S(r), S(s), S(a)), f = !1, o(h)
             }
         }
     }
 
-    function Uh(e) {
-        let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, E, T, S, C, R, N, F, M = (e[0] === xh.Installed || e[0] === xh.ReconcileInstalled) && Dh(e),
-            j = e[0] !== xh.Reconcile && e[0] !== xh.ReconcileInstalled && Ch(e);
-        const U = [Lh, Rh],
+    function Vh(e) {
+        let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, q, T, $, D, R, L, I, M = (e[0] === Ah.Installed || e[0] === Ah.ReconcileInstalled) && Ch(e),
+            P = e[0] !== Ah.Reconcile && e[0] !== Ah.ReconcileInstalled && Rh(e);
+        const B = [Nh, Lh],
             V = [];
 
-        function z(e, t) {
-            return e[0] === xh.Reconcile ? 0 : e[0] !== xh.ReconcileInstalled ? 1 : -1
-        }~(b = z(e)) && (w = V[b] = U[b](e));
-        let H = e[7] && Ih(),
-            W = e[9] && Fh();
-        const G = [Bh, jh, Ph, Mh],
-            Z = [];
+        function H(e, t) {
+            return e[0] === Ah.Reconcile ? 0 : e[0] !== Ah.ReconcileInstalled ? 1 : -1
+        }~(b = H(e)) && (w = V[b] = B[b](e));
+        let W = e[7] && Fh(),
+            G = e[9] && Mh();
+        const Z = [Uh, Bh, jh, Ph],
+            J = [];
 
-        function J(e, t) {
-            return e[0] === xh.Installed ? 0 : e[0] === xh.Search || e[0] === xh.FilterInstalled ? 1 : e[0] === xh.Reconcile ? 2 : e[0] === xh.ReconcileInstalled ? 3 : -1
+        function Y(e, t) {
+            return e[0] === Ah.Installed ? 0 : e[0] === Ah.Search || e[0] === Ah.FilterInstalled ? 1 : e[0] === Ah.Reconcile ? 2 : e[0] === Ah.ReconcileInstalled ? 3 : -1
         }
-        return ~(T = J(e)) && (S = Z[T] = G[T](e)), R = B(e[15][0]), {
+        return ~(T = Y(e)) && ($ = J[T] = Z[T](e)), R = U(e[15][0]), {
             c() {
-                t = D("nav"), r = D("div"), n = D("menu"), i = D("li"), s = D("input"), a = L(), l = D("label"), l.textContent = "installed", u = L(), c = D("li"), f = D("input"), h = L(), p = D("label"), p.textContent = "unreconciled", d = L(), M && M.c(), m = L(), j && j.c(), g = L(), v = D("div"), y = D("menu"), w && w.c(), _ = L(), H && H.c(), k = L(), x = D("div"), W && W.c(), A = L(), E = D("menu"), S && S.c(), P(s, "class", "control svelte-nmk0ob"), P(s, "type", "radio"), P(s, "id", "__radio-installed"), s.__value = xh.Installed, s.value = s.__value, P(l, "class", "control svelte-nmk0ob"), P(l, "for", "__radio-installed"), P(i, "class", "segmented-control svelte-nmk0ob"), P(f, "class", "control svelte-nmk0ob"), P(f, "type", "radio"), P(f, "id", "__radio-unreconciled"), f.__value = xh.Reconcile, f.value = f.__value, P(p, "class", "control svelte-nmk0ob"), P(p, "for", "__radio-unreconciled"), P(c, "class", "segmented-control svelte-nmk0ob"), P(n, "class", "control-set svelte-nmk0ob"), P(r, "class", "svelte-nmk0ob"), P(y, "class", "control-set svelte-nmk0ob"), P(v, "class", "search svelte-nmk0ob"), P(E, "class", "control-set svelte-nmk0ob"), P(x, "class", "svelte-nmk0ob"), P(t, "class", "addon-list-nav svelte-nmk0ob"), R.p(s, f)
+                t = C("nav"), r = C("div"), n = C("menu"), i = C("li"), s = C("input"), a = N(), l = C("label"), l.textContent = "installed", u = N(), c = C("li"), f = C("input"), h = N(), p = C("label"), p.textContent = "unreconciled", d = N(), M && M.c(), m = N(), P && P.c(), g = N(), v = C("div"), y = C("menu"), w && w.c(), _ = N(), W && W.c(), k = N(), x = C("div"), G && G.c(), A = N(), q = C("menu"), $ && $.c(), j(s, "class", "control svelte-nmk0ob"), j(s, "type", "radio"), j(s, "id", "__radio-installed"), s.__value = Ah.Installed, z(s, s.__value), j(l, "class", "control svelte-nmk0ob"), j(l, "for", "__radio-installed"), j(i, "class", "segmented-control svelte-nmk0ob"), j(f, "class", "control svelte-nmk0ob"), j(f, "type", "radio"), j(f, "id", "__radio-unreconciled"), f.__value = Ah.Reconcile, z(f, f.__value), j(p, "class", "control svelte-nmk0ob"), j(p, "for", "__radio-unreconciled"), j(c, "class", "segmented-control svelte-nmk0ob"), j(n, "class", "control-set svelte-nmk0ob"), j(r, "class", "svelte-nmk0ob"), j(y, "class", "control-set svelte-nmk0ob"), j(v, "class", "search svelte-nmk0ob"), j(q, "class", "control-set svelte-nmk0ob"), j(x, "class", "svelte-nmk0ob"), j(t, "class", "addon-list-nav svelte-nmk0ob"), R.p(s, f)
             },
             m(o, w) {
-                $(o, t, w), q(t, r), q(r, n), q(n, i), q(i, s), s.checked = s.__value === e[0], q(i, a), q(i, l), q(n, u), q(n, c), q(c, f), f.checked = f.__value === e[0], q(c, h), q(c, p), q(n, d), M && M.m(n, null), q(n, m), j && j.m(n, null), q(t, g), q(t, v), q(v, y), ~b && V[b].m(y, null), q(v, _), H && H.m(v, null), q(t, k), q(t, x), W && W.m(x, null), q(x, A), q(x, E), ~T && Z[T].m(E, null), C = !0, N || (F = [I(window, "togaSimulateKeypress", e[13]), I(s, "change", e[14]), I(f, "change", e[16])], N = !0)
+                O(o, t, w), E(t, r), E(r, n), E(n, i), E(i, s), s.checked = s.__value === e[0], E(i, a), E(i, l), E(n, u), E(n, c), E(c, f), f.checked = f.__value === e[0], E(c, h), E(c, p), E(n, d), M && M.m(n, null), E(n, m), P && P.m(n, null), E(t, g), E(t, v), E(v, y), ~b && V[b].m(y, null), E(v, _), W && W.m(v, null), E(t, k), E(t, x), G && G.m(x, null), E(x, A), E(x, q), ~T && J[T].m(q, null), D = !0, L || (I = [F(window, "togaSimulateKeypress", e[13]), F(s, "change", e[14]), F(f, "change", e[16])], L = !0)
             },
             p(e, t) {
-                1 & t[0] && (s.checked = s.__value === e[0]), 1 & t[0] && (f.checked = f.__value === e[0]), e[0] === xh.Installed || e[0] === xh.ReconcileInstalled ? M ? (M.p(e, t), 1 & t[0] && Oe(M, 1)) : (M = Dh(e), M.c(), Oe(M, 1), M.m(n, m)) : M && (Te(), Se(M, 1, 1, (() => {
+                1 & t[0] && (s.checked = s.__value === e[0]), 1 & t[0] && (f.checked = f.__value === e[0]), e[0] === Ah.Installed || e[0] === Ah.ReconcileInstalled ? M ? (M.p(e, t), 1 & t[0] && Se(M, 1)) : (M = Ch(e), M.c(), Se(M, 1), M.m(n, m)) : M && ($e(), De(M, 1, 1, (() => {
                     M = null
-                })), $e()), e[0] !== xh.Reconcile && e[0] !== xh.ReconcileInstalled ? j ? (j.p(e, t), 1 & t[0] && Oe(j, 1)) : (j = Ch(e), j.c(), Oe(j, 1), j.m(n, null)) : j && (Te(), Se(j, 1, 1, (() => {
-                    j = null
-                })), $e());
+                })), Oe()), e[0] !== Ah.Reconcile && e[0] !== Ah.ReconcileInstalled ? P ? (P.p(e, t), 1 & t[0] && Se(P, 1)) : (P = Rh(e), P.c(), Se(P, 1), P.m(n, null)) : P && ($e(), De(P, 1, 1, (() => {
+                    P = null
+                })), Oe());
                 let r = b;
-                b = z(e), b === r ? ~b && V[b].p(e, t) : (w && (Te(), Se(V[r], 1, 1, (() => {
+                b = H(e), b === r ? ~b && V[b].p(e, t) : (w && ($e(), De(V[r], 1, 1, (() => {
                     V[r] = null
-                })), $e()), ~b ? (w = V[b], w ? w.p(e, t) : (w = V[b] = U[b](e), w.c()), Oe(w, 1), w.m(y, null)) : w = null), e[7] ? H ? 128 & t[0] && Oe(H, 1) : (H = Ih(), H.c(), Oe(H, 1), H.m(v, null)) : H && (Te(), Se(H, 1, 1, (() => {
-                    H = null
-                })), $e()), e[9] ? W ? 512 & t[0] && Oe(W, 1) : (W = Fh(), W.c(), Oe(W, 1), W.m(x, A)) : W && (Te(), Se(W, 1, 1, (() => {
+                })), Oe()), ~b ? (w = V[b], w ? w.p(e, t) : (w = V[b] = B[b](e), w.c()), Se(w, 1), w.m(y, null)) : w = null), e[7] ? W ? 128 & t[0] && Se(W, 1) : (W = Fh(), W.c(), Se(W, 1), W.m(v, null)) : W && ($e(), De(W, 1, 1, (() => {
                     W = null
-                })), $e());
+                })), Oe()), e[9] ? G ? 512 & t[0] && Se(G, 1) : (G = Mh(), G.c(), Se(G, 1), G.m(x, A)) : G && ($e(), De(G, 1, 1, (() => {
+                    G = null
+                })), Oe());
                 let i = T;
-                T = J(e), T === i ? ~T && Z[T].p(e, t) : (S && (Te(), Se(Z[i], 1, 1, (() => {
-                    Z[i] = null
-                })), $e()), ~T ? (S = Z[T], S ? S.p(e, t) : (S = Z[T] = G[T](e), S.c()), Oe(S, 1), S.m(E, null)) : S = null)
+                T = Y(e), T === i ? ~T && J[T].p(e, t) : ($ && ($e(), De(J[i], 1, 1, (() => {
+                    J[i] = null
+                })), Oe()), ~T ? ($ = J[T], $ ? $.p(e, t) : ($ = J[T] = Z[T](e), $.c()), Se($, 1), $.m(q, null)) : $ = null)
             },
             i(e) {
-                C || (Oe(M), Oe(j), Oe(w), Oe(H), Oe(W), Oe(S), C = !0)
+                D || (Se(M), Se(P), Se(w), Se(W), Se(G), Se($), D = !0)
             },
             o(e) {
-                Se(M), Se(j), Se(w), Se(H), Se(W), Se(S), C = !1
+                De(M), De(P), De(w), De(W), De(G), De($), D = !1
             },
             d(e) {
-                e && O(t), M && M.d(), j && j.d(), ~b && V[b].d(), H && H.d(), W && W.d(), ~T && Z[T].d(), R.r(), N = !1, o(F)
+                e && S(t), M && M.d(), P && P.d(), ~b && V[b].d(), W && W.d(), G && G.d(), ~T && J[T].d(), R.r(), L = !1, o(I)
             }
         }
     }
 
-    function Vh(e, t, r) {
+    function zh(e, t, r) {
         let {
             activeView: n,
             searchTerms: i,
             searchFilterInstalled: o,
             searchIsDirty: s,
             isRefreshing: a,
             isModifying: l,
             isSearching: u,
             installedOutdatedCount: c,
             reconcileInstallationInProgress: f,
             reconcileStage: h,
             canReconcile: p
         } = t;
-        const d = se();
+        const d = ae();
         let m;
         return e.$$set = e => {
             "activeView" in e && r(0, n = e.activeView), "searchTerms" in e && r(1, i = e.searchTerms), "searchFilterInstalled" in e && r(2, o = e.searchFilterInstalled), "searchIsDirty" in e && r(4, s = e.searchIsDirty), "isRefreshing" in e && r(5, a = e.isRefreshing), "isModifying" in e && r(6, l = e.isModifying), "isSearching" in e && r(7, u = e.isSearching), "installedOutdatedCount" in e && r(8, c = e.installedOutdatedCount), "reconcileInstallationInProgress" in e && r(9, f = e.reconcileInstallationInProgress), "reconcileStage" in e && r(3, h = e.reconcileStage), "canReconcile" in e && r(10, p = e.canReconcile)
         }, [n, i, o, h, s, a, l, u, c, f, p, m, d, e => {
                 const {
                     action: t
                 } = e.detail;
-                "activateViewInstalled" === t ? r(0, n = xh.Installed) : "activateViewReconcile" === t ? r(0, n = xh.Reconcile) : "activateViewSearch" === t ? (r(0, n = xh.Search), m.focus()) : "toggleSearchFilter" === t && (r(2, o = !o), o && m.focus())
+                "activateViewInstalled" === t ? r(0, n = Ah.Installed) : "activateViewReconcile" === t ? r(0, n = Ah.Reconcile) : "activateViewSearch" === t ? (r(0, n = Ah.Search), m.focus()) : "toggleSearchFilter" === t && (r(2, o = !o), o && m.focus())
             }, function() {
                 n = this.__value, r(0, n)
             },
             [
                 []
             ],
             function() {
                 n = this.__value, r(0, n)
             },
             function() {
                 n = this.__value, r(0, n)
             }, () => d("requestCycleListFormat"),
             function() {
-                h = W(this), r(3, h)
+                h = G(this), r(3, h)
             },
             function() {
                 o = this.checked, r(2, o)
             },
             function(e) {
-                fe[e ? "unshift" : "push"]((() => {
+                he[e ? "unshift" : "push"]((() => {
                     m = e, r(11, m)
                 }))
             },
             function() {
                 i = this.value, r(1, i)
             },
             e => "Enter" === e.key && d("requestSearch"), () => d("requestRefresh"), () => d("requestUpdateAll"), () => d("requestShowSearchOptionsModal"), () => d("requestInstallReconciled"), () => d("requestAutomateReconciliation"), () => d("requestInstallReconciledInstalled")
         ]
     }
-    class zh extends Ze {
+    class Hh extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Vh, Uh, a, {
+            super(), Je(this, e, zh, Vh, a, {
                 activeView: 0,
                 searchTerms: 1,
                 searchFilterInstalled: 2,
                 searchIsDirty: 4,
                 isRefreshing: 5,
                 isModifying: 6,
                 isSearching: 7,
@@ -18939,310 +18959,310 @@
                 reconcileInstallationInProgress: 9,
                 reconcileStage: 3,
                 canReconcile: 10
             }, null, [-1, -1])
         }
     }
     const {
-        window: Hh
-    } = A;
+        window: Wh
+    } = q;
 
-    function Wh(e) {
+    function Gh(e) {
         let t, r, n, i, s, a, l, u;
         const c = e[8].default,
             h = f(c, e, e[7], null);
         return {
             c() {
-                t = D("div"), r = D("div"), n = D("menu"), h && h.c(), P(n, "class", "svelte-1irf7oq"), P(r, "class", "context-menu svelte-1irf7oq"), P(r, "style", i = `\n      --menu-x-offset: ${e[4].x}px;\n      --menu-y-offset: ${e[4].y}px;\n    `), ge((() => e[10].call(r))), P(t, "class", "context-menu-wrapper svelte-1irf7oq"), P(t, "tabindex", "-1")
+                t = C("div"), r = C("div"), n = C("menu"), h && h.c(), j(n, "class", "svelte-1irf7oq"), j(r, "class", "context-menu svelte-1irf7oq"), j(r, "style", i = `\n      --menu-x-offset: ${e[4].x}px;\n      --menu-y-offset: ${e[4].y}px;\n    `), ve((() => e[10].call(r))), j(t, "class", "context-menu-wrapper svelte-1irf7oq"), j(t, "tabindex", "-1")
             },
             m(i, o) {
-                $(i, t, o), q(t, r), q(r, n), h && h.m(n, null), s = function(e, t) {
+                O(i, t, o), E(t, r), E(r, n), h && h.m(n, null), s = function(e, t) {
                     "static" === getComputedStyle(e).position && (e.style.position = "relative");
-                    const r = D("iframe");
+                    const r = C("iframe");
                     r.setAttribute("style", "display: block; position: absolute; top: 0; left: 0; width: 100%; height: 100%; overflow: hidden; border: 0; opacity: 0; pointer-events: none; z-index: -1;"), r.setAttribute("aria-hidden", "true"), r.tabIndex = -1;
-                    const n = Z();
+                    const n = J();
                     let i;
-                    return n ? (r.src = "data:text/html,<script>onresize=function(){parent.postMessage(0,'*')}<\/script>", i = I(window, "message", (e => {
+                    return n ? (r.src = "data:text/html,<script>onresize=function(){parent.postMessage(0,'*')}<\/script>", i = F(window, "message", (e => {
                         e.source === r.contentWindow && t()
                     }))) : (r.src = "about:blank", r.onload = () => {
-                        i = I(r.contentWindow, "resize", t), t()
-                    }), q(e, r), () => {
-                        (n || i && r.contentWindow) && i(), O(r)
+                        i = F(r.contentWindow, "resize", t), t()
+                    }), E(e, r), () => {
+                        (n || i && r.contentWindow) && i(), S(r)
                     }
-                }(r, e[10].bind(r)), a = !0, l || (u = [I(r, "click", M(e[9])), I(t, "click", e[0])], l = !0)
+                }(r, e[10].bind(r)), a = !0, l || (u = [F(r, "click", P(e[9])), F(t, "click", e[0])], l = !0)
             },
             p(e, t) {
-                h && h.p && (!a || 128 & t) && d(h, c, e, e[7], a ? p(c, e[7], t, null) : m(e[7]), null), (!a || 16 & t && i !== (i = `\n      --menu-x-offset: ${e[4].x}px;\n      --menu-y-offset: ${e[4].y}px;\n    `)) && P(r, "style", i)
+                h && h.p && (!a || 128 & t) && d(h, c, e, e[7], a ? p(c, e[7], t, null) : m(e[7]), null), (!a || 16 & t && i !== (i = `\n      --menu-x-offset: ${e[4].x}px;\n      --menu-y-offset: ${e[4].y}px;\n    `)) && j(r, "style", i)
             },
             i(e) {
-                a || (Oe(h, e), a = !0)
+                a || (Se(h, e), a = !0)
             },
             o(e) {
-                Se(h, e), a = !1
+                De(h, e), a = !1
             },
             d(e) {
-                e && O(t), h && h.d(e), s(), l = !1, o(u)
+                e && S(t), h && h.d(e), s(), l = !1, o(u)
             }
         }
     }
 
-    function Gh(e) {
-        let t, r, n, i, s = e[1] && Wh(e);
+    function Zh(e) {
+        let t, r, n, i, s = e[1] && Gh(e);
         return {
             c() {
-                s && s.c(), t = N()
+                s && s.c(), t = I()
             },
             m(o, a) {
-                s && s.m(o, a), $(o, t, a), r = !0, n || (i = [I(Hh, "keydown", e[5]), I(Hh, "resize", e[0])], n = !0)
+                s && s.m(o, a), O(o, t, a), r = !0, n || (i = [F(Wh, "keydown", e[5]), F(Wh, "resize", e[0])], n = !0)
             },
             p(e, [r]) {
-                e[1] ? s ? (s.p(e, r), 2 & r && Oe(s, 1)) : (s = Wh(e), s.c(), Oe(s, 1), s.m(t.parentNode, t)) : s && (Te(), Se(s, 1, 1, (() => {
+                e[1] ? s ? (s.p(e, r), 2 & r && Se(s, 1)) : (s = Gh(e), s.c(), Se(s, 1), s.m(t.parentNode, t)) : s && ($e(), De(s, 1, 1, (() => {
                     s = null
-                })), $e())
+                })), Oe())
             },
             i(e) {
-                r || (Oe(s), r = !0)
+                r || (Se(s), r = !0)
             },
             o(e) {
-                Se(s), r = !1
+                De(s), r = !1
             },
             d(e) {
-                s && s.d(e), e && O(t), n = !1, o(i)
+                e && S(t), s && s.d(e), n = !1, o(i)
             }
         }
     }
 
-    function Zh(e, t, r) {
+    function Jh(e, t, r) {
         let {
             $$slots: n = {},
             $$scope: i
         } = t;
-        const o = se();
+        const o = ae();
         let s, a, l, u = {
             x: 0,
             y: 0
         };
         const c = () => {
             r(1, s = void 0), o("hide")
         };
-        return ae("contextMenu", {
+        return le("contextMenu", {
             hide: c
         }), e.$$set = e => {
             "$$scope" in e && r(7, i = e.$$scope)
         }, e.$$.update = () => {
             14 & e.$$.dirty && s && (r(4, u.x = s.x + a < window.innerWidth ? s.x : s.x - a, u), r(4, u.y = s.y + l < window.innerHeight ? s.y : s.y - l, u))
         }, [c, s, a, l, u, e => {
             "Escape" === e.key && s && (c(), e.preventDefault())
         }, e => {
             r(1, s = e)
         }, i, n, function(t) {
-            ue.call(this, e, t)
+            ce.call(this, e, t)
         }, function() {
             l = this.offsetHeight, a = this.offsetWidth, r(3, l), r(2, a)
         }]
     }
-    class Jh extends Ze {
+    class Yh extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Zh, Gh, a, {
+            super(), Je(this, e, Jh, Zh, a, {
                 show: 6,
                 hide: 0
             })
         }
         get show() {
             return this.$$.ctx[6]
         }
         get hide() {
             return this.$$.ctx[0]
         }
     }
 
-    function Yh(e) {
+    function Kh(e) {
         let t, r, n, i;
         const o = e[3].default,
             s = f(o, e, e[2], null);
         return {
             c() {
-                t = D("button"), s && s.c(), P(t, "class", "svelte-1gyrn85")
+                t = C("button"), s && s.c(), j(t, "class", "svelte-1gyrn85")
             },
             m(o, a) {
-                $(o, t, a), s && s.m(t, null), r = !0, n || (i = I(t, "click", M(e[1])), n = !0)
+                O(o, t, a), s && s.m(t, null), r = !0, n || (i = F(t, "click", P(e[1])), n = !0)
             },
             p(e, t) {
                 s && s.p && (!r || 4 & t) && d(s, o, e, e[2], r ? p(o, e[2], t, null) : m(e[2]), null)
             },
             i(e) {
-                r || (Oe(s, e), r = !0)
+                r || (Se(s, e), r = !0)
             },
             o(e) {
-                Se(s, e), r = !1
+                De(s, e), r = !1
             },
             d(e) {
-                e && O(t), s && s.d(e), n = !1, i()
+                e && S(t), s && s.d(e), n = !1, i()
             }
         }
     }
 
-    function Kh(t) {
+    function Xh(t) {
         let r;
         return {
             c() {
-                r = D("hr"), P(r, "class", "svelte-1gyrn85")
+                r = C("hr"), j(r, "class", "svelte-1gyrn85")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             i: e,
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Xh(e) {
+    function Qh(e) {
         let t, r, n, i;
-        const o = [Kh, Yh],
+        const o = [Xh, Kh],
             s = [];
 
         function a(e, t) {
             return e[0] ? 0 : 1
         }
         return r = a(e), n = s[r] = o[r](e), {
             c() {
-                t = D("li"), n.c(), P(t, "class", "menu-item svelte-1gyrn85")
+                t = C("li"), n.c(), j(t, "class", "menu-item svelte-1gyrn85")
             },
             m(e, n) {
-                $(e, t, n), s[r].m(t, null), i = !0
+                O(e, t, n), s[r].m(t, null), i = !0
             },
             p(e, [i]) {
                 let l = r;
-                r = a(e), r === l ? s[r].p(e, i) : (Te(), Se(s[l], 1, 1, (() => {
+                r = a(e), r === l ? s[r].p(e, i) : ($e(), De(s[l], 1, 1, (() => {
                     s[l] = null
-                })), $e(), n = s[r], n ? n.p(e, i) : (n = s[r] = o[r](e), n.c()), Oe(n, 1), n.m(t, null))
+                })), Oe(), n = s[r], n ? n.p(e, i) : (n = s[r] = o[r](e), n.c()), Se(n, 1), n.m(t, null))
             },
             i(e) {
-                i || (Oe(n), i = !0)
+                i || (Se(n), i = !0)
             },
             o(e) {
-                Se(n), i = !1
+                De(n), i = !1
             },
             d(e) {
-                e && O(t), s[r].d()
+                e && S(t), s[r].d()
             }
         }
     }
 
-    function Qh(e, t, r) {
+    function ep(e, t, r) {
         let {
             $$slots: n = {},
             $$scope: i
         } = t, {
             divider: o = !1
         } = t;
-        const s = le("contextMenu"),
-            a = se();
+        const s = ue("contextMenu"),
+            a = ae();
         return e.$$set = e => {
             "divider" in e && r(0, o = e.divider), "$$scope" in e && r(2, i = e.$$scope)
         }, [o, () => {
             o || (s.hide(), a("click"))
         }, i, n]
     }
-    class ep extends Ze {
+    class tp extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Qh, Xh, a, {
+            super(), Je(this, e, ep, Qh, a, {
                 divider: 0
             })
         }
     }
 
-    function tp(e) {
+    function rp(e) {
         const t = e.slice(),
             r = t[1];
         return t[18] = r.addon, t
     }
 
-    function rp(e) {
+    function np(e) {
         let t, r, n, i;
-        const o = [ip, np],
+        const o = [op, ip],
             s = [];
 
         function a(e, t) {
             return e[1].installed ? 0 : 1
         }
         return t = a(e), r = s[t] = o[t](e), {
             c() {
-                r.c(), n = N()
+                r.c(), n = I()
             },
             m(e, r) {
-                s[t].m(e, r), $(e, n, r), i = !0
+                s[t].m(e, r), O(e, n, r), i = !0
             },
             p(e, i) {
                 let l = t;
-                t = a(e), t === l ? s[t].p(e, i) : (Te(), Se(s[l], 1, 1, (() => {
+                t = a(e), t === l ? s[t].p(e, i) : ($e(), De(s[l], 1, 1, (() => {
                     s[l] = null
-                })), $e(), r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Oe(r, 1), r.m(n.parentNode, n))
+                })), Oe(), r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Se(r, 1), r.m(n.parentNode, n))
             },
             i(e) {
-                i || (Oe(r), i = !0)
+                i || (Se(r), i = !0)
             },
             o(e) {
-                Se(r), i = !1
+                De(r), i = !1
             },
             d(e) {
-                s[t].d(e), e && O(n)
+                e && S(n), s[t].d(e)
             }
         }
     }
 
-    function np(e) {
+    function ip(e) {
         let t, r, n, i, o, s, a, l;
-        return t = new ep({
+        return t = new tp({
             props: {
                 $$slots: {
-                    default: [op]
+                    default: [sp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("click", (function() {
             return e[13](e[18])
-        })), n = new ep({
+        })), n = new tp({
             props: {
                 $$slots: {
-                    default: [sp]
+                    default: [ap]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), n.$on("click", (function() {
             return e[14](e[18])
-        })), o = new ep({
+        })), o = new tp({
             props: {
                 divider: !0
             }
-        }), a = new ep({
+        }), a = new tp({
             props: {
                 $$slots: {
-                    default: [ap]
+                    default: [lp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), a.$on("click", (function() {
             return e[15](e[18])
         })), {
             c() {
-                Ve(t.$$.fragment), r = L(), Ve(n.$$.fragment), i = L(), Ve(o.$$.fragment), s = L(), Ve(a.$$.fragment)
+                He(t.$$.fragment), r = N(), He(n.$$.fragment), i = N(), He(o.$$.fragment), s = N(), He(a.$$.fragment)
             },
             m(e, u) {
-                ze(t, e, u), $(e, r, u), ze(n, e, u), $(e, i, u), ze(o, e, u), $(e, s, u), ze(a, e, u), l = !0
+                We(t, e, u), O(e, r, u), We(n, e, u), O(e, i, u), We(o, e, u), O(e, s, u), We(a, e, u), l = !0
             },
             p(r, i) {
                 e = r;
                 const o = {};
                 524288 & i && (o.$$scope = {
                     dirty: i,
                     ctx: e
@@ -19255,94 +19275,94 @@
                 const l = {};
                 524288 & i && (l.$$scope = {
                     dirty: i,
                     ctx: e
                 }), a.$set(l)
             },
             i(e) {
-                l || (Oe(t.$$.fragment, e), Oe(n.$$.fragment, e), Oe(o.$$.fragment, e), Oe(a.$$.fragment, e), l = !0)
+                l || (Se(t.$$.fragment, e), Se(n.$$.fragment, e), Se(o.$$.fragment, e), Se(a.$$.fragment, e), l = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), Se(n.$$.fragment, e), Se(o.$$.fragment, e), Se(a.$$.fragment, e), l = !1
+                De(t.$$.fragment, e), De(n.$$.fragment, e), De(o.$$.fragment, e), De(a.$$.fragment, e), l = !1
             },
             d(e) {
-                He(t, e), e && O(r), He(n, e), e && O(i), He(o, e), e && O(s), He(a, e)
+                e && (S(r), S(i), S(s)), Ge(t, e), Ge(n, e), Ge(o, e), Ge(a, e)
             }
         }
     }
 
-    function ip(e) {
+    function op(e) {
         let t, r, n, i, o, s, a, l, u, c, f, h, p;
-        t = new ep({
+        t = new tp({
             props: {
                 $$slots: {
-                    default: [lp]
+                    default: [up]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("click", (function() {
             return e[5](e[18])
-        })), n = new ep({
+        })), n = new tp({
             props: {
                 $$slots: {
-                    default: [up]
+                    default: [cp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), n.$on("click", (function() {
             return e[6](e[18])
-        })), o = new ep({
+        })), o = new tp({
             props: {
                 $$slots: {
-                    default: [cp]
+                    default: [fp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), o.$on("click", (function() {
             return e[7](e[18])
-        })), a = new ep({
+        })), a = new tp({
             props: {
                 $$slots: {
-                    default: [fp]
+                    default: [hp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), a.$on("click", (function() {
             return e[8](e[18])
-        })), u = new ep({
+        })), u = new tp({
             props: {
                 divider: !0
             }
         });
-        let d = e[1].supportsRollback && hp(e);
-        return h = new ep({
+        let d = e[1].supportsRollback && pp(e);
+        return h = new tp({
             props: {
                 $$slots: {
-                    default: [bp]
+                    default: [wp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), h.$on("click", (function() {
             return e[12](e[18])
         })), {
             c() {
-                Ve(t.$$.fragment), r = L(), Ve(n.$$.fragment), i = L(), Ve(o.$$.fragment), s = L(), Ve(a.$$.fragment), l = L(), Ve(u.$$.fragment), c = L(), d && d.c(), f = L(), Ve(h.$$.fragment)
+                He(t.$$.fragment), r = N(), He(n.$$.fragment), i = N(), He(o.$$.fragment), s = N(), He(a.$$.fragment), l = N(), He(u.$$.fragment), c = N(), d && d.c(), f = N(), He(h.$$.fragment)
             },
             m(e, m) {
-                ze(t, e, m), $(e, r, m), ze(n, e, m), $(e, i, m), ze(o, e, m), $(e, s, m), ze(a, e, m), $(e, l, m), ze(u, e, m), $(e, c, m), d && d.m(e, m), $(e, f, m), ze(h, e, m), p = !0
+                We(t, e, m), O(e, r, m), We(n, e, m), O(e, i, m), We(o, e, m), O(e, s, m), We(a, e, m), O(e, l, m), We(u, e, m), O(e, c, m), d && d.m(e, m), O(e, f, m), We(h, e, m), p = !0
             },
             p(r, i) {
                 e = r;
                 const s = {};
                 524288 & i && (s.$$scope = {
                     dirty: i,
                     ctx: e
@@ -19357,788 +19377,788 @@
                     dirty: i,
                     ctx: e
                 }), o.$set(u);
                 const c = {};
                 524288 & i && (c.$$scope = {
                     dirty: i,
                     ctx: e
-                }), a.$set(c), e[1].supportsRollback ? d ? (d.p(e, i), 2 & i && Oe(d, 1)) : (d = hp(e), d.c(), Oe(d, 1), d.m(f.parentNode, f)) : d && (Te(), Se(d, 1, 1, (() => {
+                }), a.$set(c), e[1].supportsRollback ? d ? (d.p(e, i), 2 & i && Se(d, 1)) : (d = pp(e), d.c(), Se(d, 1), d.m(f.parentNode, f)) : d && ($e(), De(d, 1, 1, (() => {
                     d = null
-                })), $e());
+                })), Oe());
                 const p = {};
                 524288 & i && (p.$$scope = {
                     dirty: i,
                     ctx: e
                 }), h.$set(p)
             },
             i(e) {
-                p || (Oe(t.$$.fragment, e), Oe(n.$$.fragment, e), Oe(o.$$.fragment, e), Oe(a.$$.fragment, e), Oe(u.$$.fragment, e), Oe(d), Oe(h.$$.fragment, e), p = !0)
+                p || (Se(t.$$.fragment, e), Se(n.$$.fragment, e), Se(o.$$.fragment, e), Se(a.$$.fragment, e), Se(u.$$.fragment, e), Se(d), Se(h.$$.fragment, e), p = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), Se(n.$$.fragment, e), Se(o.$$.fragment, e), Se(a.$$.fragment, e), Se(u.$$.fragment, e), Se(d), Se(h.$$.fragment, e), p = !1
+                De(t.$$.fragment, e), De(n.$$.fragment, e), De(o.$$.fragment, e), De(a.$$.fragment, e), De(u.$$.fragment, e), De(d), De(h.$$.fragment, e), p = !1
             },
             d(e) {
-                He(t, e), e && O(r), He(n, e), e && O(i), He(o, e), e && O(s), He(a, e), e && O(l), He(u, e), e && O(c), d && d.d(e), e && O(f), He(h, e)
+                e && (S(r), S(i), S(s), S(l), S(c), S(f)), Ge(t, e), Ge(n, e), Ge(o, e), Ge(a, e), Ge(u, e), d && d.d(e), Ge(h, e)
             }
         }
     }
 
-    function op(e) {
+    function sp(e) {
         let t;
         return {
             c() {
-                t = R("Install and replace")
+                t = L("Install and replace")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function sp(e) {
+    function ap(e) {
         let t;
         return {
             c() {
-                t = R("View changelog")
+                t = L("View changelog")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function ap(e) {
+    function lp(e) {
         let t;
         return {
             c() {
-                t = R("Resolve")
+                t = L("Resolve")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function lp(e) {
+    function up(e) {
         let t;
         return {
             c() {
-                t = R("Visit home page")
+                t = L("Visit home page")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function up(e) {
+    function cp(e) {
         let t;
         return {
             c() {
-                t = R("View changelog")
+                t = L("View changelog")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function cp(e) {
+    function fp(e) {
         let t;
         return {
             c() {
-                t = R("Reveal folder")
+                t = L("Reveal folder")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function fp(e) {
+    function hp(e) {
         let t;
         return {
             c() {
-                t = R("Resolve")
+                t = L("Resolve")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function hp(e) {
-        let t, r, n, i, o, s = e[1].addon.logged_versions.length > 1 && pp(e);
-        const a = [gp, mp],
+    function pp(e) {
+        let t, r, n, i, o, s = e[1].addon.logged_versions.length > 1 && dp(e);
+        const a = [vp, gp],
             l = [];
 
         function u(e, t) {
             return e[1].addon.options.version_eq ? 0 : 1
         }
         return r = u(e), n = l[r] = a[r](e), {
             c() {
-                s && s.c(), t = L(), n.c(), i = N()
+                s && s.c(), t = N(), n.c(), i = I()
             },
             m(e, n) {
-                s && s.m(e, n), $(e, t, n), l[r].m(e, n), $(e, i, n), o = !0
+                s && s.m(e, n), O(e, t, n), l[r].m(e, n), O(e, i, n), o = !0
             },
             p(e, o) {
-                e[1].addon.logged_versions.length > 1 ? s ? (s.p(e, o), 2 & o && Oe(s, 1)) : (s = pp(e), s.c(), Oe(s, 1), s.m(t.parentNode, t)) : s && (Te(), Se(s, 1, 1, (() => {
+                e[1].addon.logged_versions.length > 1 ? s ? (s.p(e, o), 2 & o && Se(s, 1)) : (s = dp(e), s.c(), Se(s, 1), s.m(t.parentNode, t)) : s && ($e(), De(s, 1, 1, (() => {
                     s = null
-                })), $e());
+                })), Oe());
                 let c = r;
-                r = u(e), r === c ? l[r].p(e, o) : (Te(), Se(l[c], 1, 1, (() => {
+                r = u(e), r === c ? l[r].p(e, o) : ($e(), De(l[c], 1, 1, (() => {
                     l[c] = null
-                })), $e(), n = l[r], n ? n.p(e, o) : (n = l[r] = a[r](e), n.c()), Oe(n, 1), n.m(i.parentNode, i))
+                })), Oe(), n = l[r], n ? n.p(e, o) : (n = l[r] = a[r](e), n.c()), Se(n, 1), n.m(i.parentNode, i))
             },
             i(e) {
-                o || (Oe(s), Oe(n), o = !0)
+                o || (Se(s), Se(n), o = !0)
             },
             o(e) {
-                Se(s), Se(n), o = !1
+                De(s), De(n), o = !1
             },
             d(e) {
-                s && s.d(e), e && O(t), l[r].d(e), e && O(i)
+                e && (S(t), S(i)), s && s.d(e), l[r].d(e)
             }
         }
     }
 
-    function pp(e) {
+    function dp(e) {
         let t, r;
-        return t = new ep({
+        return t = new tp({
             props: {
                 $$slots: {
-                    default: [dp]
+                    default: [mp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("click", (function() {
             return e[9](e[18])
         })), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(r, n) {
                 e = r;
                 const i = {};
                 524288 & n && (i.$$scope = {
                     dirty: n,
                     ctx: e
                 }), t.$set(i)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function dp(e) {
+    function mp(e) {
         let t;
         return {
             c() {
-                t = R("Rollback")
+                t = L("Rollback")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function mp(e) {
+    function gp(e) {
         let t, r;
-        return t = new ep({
+        return t = new tp({
             props: {
                 $$slots: {
-                    default: [vp]
+                    default: [yp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("click", (function() {
             return e[11](e[18])
         })), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(r, n) {
                 e = r;
                 const i = {};
                 524288 & n && (i.$$scope = {
                     dirty: n,
                     ctx: e
                 }), t.$set(i)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function gp(e) {
+    function vp(e) {
         let t, r;
-        return t = new ep({
+        return t = new tp({
             props: {
                 $$slots: {
-                    default: [yp]
+                    default: [bp]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("click", (function() {
             return e[10](e[18])
         })), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(r, n) {
                 e = r;
                 const i = {};
                 524288 & n && (i.$$scope = {
                     dirty: n,
                     ctx: e
                 }), t.$set(i)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function vp(e) {
+    function yp(e) {
         let t;
         return {
             c() {
-                t = R("Pin")
+                t = L("Pin")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function yp(e) {
+    function bp(e) {
         let t;
         return {
             c() {
-                t = R("Unpin")
+                t = L("Unpin")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function bp(e) {
+    function wp(e) {
         let t;
         return {
             c() {
-                t = R("Unreconcile")
+                t = L("Unreconcile")
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function wp(e) {
-        let t, r, n = e[1] && rp(tp(e));
+    function _p(e) {
+        let t, r, n = e[1] && np(rp(e));
         return {
             c() {
-                n && n.c(), t = N()
+                n && n.c(), t = I()
             },
             m(e, i) {
-                n && n.m(e, i), $(e, t, i), r = !0
+                n && n.m(e, i), O(e, t, i), r = !0
             },
             p(e, r) {
-                e[1] ? n ? (n.p(tp(e), r), 2 & r && Oe(n, 1)) : (n = rp(tp(e)), n.c(), Oe(n, 1), n.m(t.parentNode, t)) : n && (Te(), Se(n, 1, 1, (() => {
+                e[1] ? n ? (n.p(rp(e), r), 2 & r && Se(n, 1)) : (n = np(rp(e)), n.c(), Se(n, 1), n.m(t.parentNode, t)) : n && ($e(), De(n, 1, 1, (() => {
                     n = null
-                })), $e())
+                })), Oe())
             },
             i(e) {
-                r || (Oe(n), r = !0)
+                r || (Se(n), r = !0)
             },
             o(e) {
-                Se(n), r = !1
+                De(n), r = !1
             },
             d(e) {
-                n && n.d(e), e && O(t)
+                e && S(t), n && n.d(e)
             }
         }
     }
 
-    function _p(e) {
+    function kp(e) {
         let t, r;
-        return t = new Jh({
+        return t = new Yh({
             props: {
                 $$slots: {
-                    default: [wp]
+                    default: [_p]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), e[16](t), t.$on("hide", e[2]), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(e, [r]) {
                 const n = {};
                 524290 & r && (n.$$scope = {
                     dirty: r,
                     ctx: e
                 }), t.$set(n)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(r) {
-                e[16](null), He(t, r)
+                e[16](null), Ge(t, r)
             }
         }
     }
 
-    function kp(e, t, r) {
-        const n = se();
+    function xp(e, t, r) {
+        const n = ae();
         let i, o;
-        const s = Wn.partial(n, "selectItem");
+        const s = Gn.partial(n, "selectItem");
         return [i, o, () => {
             r(1, o = void 0)
         }, s, (e, t) => {
             r(1, o = t), i.show(e)
         }, e => s({
             addon: e,
-            action: qh.VisitHomepage
+            action: Eh.VisitHomepage
         }), e => s({
             addon: e,
-            action: qh.ViewChangelog
+            action: Eh.ViewChangelog
         }), e => s({
             addon: e,
-            action: qh.RevealFolder
+            action: Eh.RevealFolder
         }), e => s({
             addon: e,
-            action: qh.Resolve
+            action: Eh.Resolve
         }), e => s({
             addon: e,
-            action: qh.Rollback
+            action: Eh.Rollback
         }), e => s({
             addon: e,
-            action: qh.Unpin
+            action: Eh.Unpin
         }), e => s({
             addon: e,
-            action: qh.Pin
+            action: Eh.Pin
         }), e => s({
             addon: e,
-            action: qh.Unreconcile
+            action: Eh.Unreconcile
         }), e => s({
             addon: e,
-            action: qh.InstallAndReplace
+            action: Eh.InstallAndReplace
         }), e => s({
             addon: e,
-            action: qh.ViewChangelog
+            action: Eh.ViewChangelog
         }), e => s({
             addon: e,
-            action: qh.Resolve
+            action: Eh.Resolve
         }), function(e) {
-            fe[e ? "unshift" : "push"]((() => {
+            he[e ? "unshift" : "push"]((() => {
                 i = e, r(0, i)
             }))
         }]
     }
-    class xp extends Ze {
+    class Ap extends Ye {
         constructor(e) {
-            super(), Ge(this, e, kp, _p, a, {
+            super(), Je(this, e, xp, kp, a, {
                 show: 4
             })
         }
         get show() {
             return this.$$.ctx[4]
         }
     }
 
-    function Ap(e) {
+    function qp(e) {
         let t, r, n = e[1].version + "";
         return {
             c() {
-                t = R("< "), r = R(n)
+                t = L("< "), r = L(n)
             },
             m(e, n) {
-                $(e, t, n), $(e, r, n)
+                O(e, t, n), O(e, r, n)
             },
             p(e, t) {
-                2 & t && n !== (n = e[1].version + "") && U(r, n)
+                2 & t && n !== (n = e[1].version + "") && V(r, n)
             },
             d(e) {
-                e && O(t), e && O(r)
+                e && (S(t), S(r))
             }
         }
     }
 
-    function qp(e) {
-        let t, r = Object.entries(e[1].options).filter(Lp).map(Np).join("") + "";
+    function Ep(e) {
+        let t, r = Object.entries(e[1].options).filter(Np).map(Ip).join("") + "";
         return {
             c() {
-                t = R(r)
+                t = L(r)
             },
             m(e, r) {
-                $(e, t, r)
+                O(e, t, r)
             },
             p(e, n) {
-                2 & n && r !== (r = Object.entries(e[1].options).filter(Lp).map(Np).join("") + "") && U(t, r)
+                2 & n && r !== (r = Object.entries(e[1].options).filter(Np).map(Ip).join("") + "") && V(t, r)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function Ep(e) {
+    function Tp(e) {
         let t, r, n, i, o, s, a = e[0].source + "",
             l = e[0].slug + "",
-            u = e[4] === Ah.Expanded && Tp(e);
+            u = e[4] === qh.Expanded && $p(e);
         return {
             c() {
-                t = D("li"), r = R(a), n = R(":"), i = R(l), o = L(), u && u.c(), s = N(), P(t, "class", "defn svelte-n5lp8")
+                t = C("li"), r = L(a), n = L(":"), i = L(l), o = N(), u && u.c(), s = I(), j(t, "class", "defn svelte-n5lp8")
             },
             m(e, a) {
-                $(e, t, a), q(t, r), q(t, n), q(t, i), $(e, o, a), u && u.m(e, a), $(e, s, a)
+                O(e, t, a), E(t, r), E(t, n), E(t, i), O(e, o, a), u && u.m(e, a), O(e, s, a)
             },
             p(e, t) {
-                1 & t && a !== (a = e[0].source + "") && U(r, a), 1 & t && l !== (l = e[0].slug + "") && U(i, l), e[4] === Ah.Expanded ? u ? u.p(e, t) : (u = Tp(e), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null)
+                1 & t && a !== (a = e[0].source + "") && V(r, a), 1 & t && l !== (l = e[0].slug + "") && V(i, l), e[4] === qh.Expanded ? u ? u.p(e, t) : (u = $p(e), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null)
             },
             d(e) {
-                e && O(t), e && O(o), u && u.d(e), e && O(s)
+                e && (S(t), S(o), S(s)), u && u.d(e)
             }
         }
     }
 
-    function Tp(e) {
+    function $p(e) {
         let t, r, n = (e[0].description || "No description.") + "";
         return {
             c() {
-                t = D("li"), r = R(n), P(t, "class", "description svelte-n5lp8")
+                t = C("li"), r = L(n), j(t, "class", "description svelte-n5lp8")
             },
             m(e, n) {
-                $(e, t, n), q(t, r)
+                O(e, t, n), E(t, r)
             },
             p(e, t) {
-                1 & t && n !== (n = (e[0].description || "No description.") + "") && U(r, n)
+                1 & t && n !== (n = (e[0].description || "No description.") + "") && V(r, n)
             },
             d(e) {
-                e && O(t)
+                e && S(t)
             }
         }
     }
 
-    function $p(e) {
+    function Op(e) {
         let t, r, n, i;
-        const o = [Dp, Sp],
+        const o = [Cp, Dp],
             s = [];
 
         function a(e, t) {
             return e[2] ? 0 : 1
         }
         return r = a(e), n = s[r] = o[r](e), {
             c() {
-                t = D("menu"), n.c(), P(t, "class", "addon-actions svelte-n5lp8")
+                t = C("menu"), n.c(), j(t, "class", "addon-actions svelte-n5lp8")
             },
             m(e, n) {
-                $(e, t, n), s[r].m(t, null), i = !0
+                O(e, t, n), s[r].m(t, null), i = !0
             },
             p(e, i) {
                 let l = r;
-                r = a(e), r === l ? s[r].p(e, i) : (Te(), Se(s[l], 1, 1, (() => {
+                r = a(e), r === l ? s[r].p(e, i) : ($e(), De(s[l], 1, 1, (() => {
                     s[l] = null
-                })), $e(), n = s[r], n ? n.p(e, i) : (n = s[r] = o[r](e), n.c()), Oe(n, 1), n.m(t, null))
+                })), Oe(), n = s[r], n ? n.p(e, i) : (n = s[r] = o[r](e), n.c()), Se(n, 1), n.m(t, null))
             },
             i(e) {
-                i || (Oe(n), i = !0)
+                i || (Se(n), i = !0)
             },
             o(e) {
-                Se(n), i = !1
+                De(n), i = !1
             },
             d(e) {
-                e && O(t), s[r].d()
+                e && S(t), s[r].d()
             }
         }
     }
 
-    function Op(e) {
+    function Sp(e) {
         let t, r, n, i;
-        return r = new Oh({
+        return r = new Sh({
             props: {
                 diameter: 18,
                 progress: e[6]
             }
         }), {
             c() {
-                t = D("div"), Ve(r.$$.fragment), P(t, "class", "progress-indicator svelte-n5lp8")
+                t = C("div"), He(r.$$.fragment), j(t, "class", "progress-indicator svelte-n5lp8")
             },
             m(e, n) {
-                $(e, t, n), ze(r, t, null), i = !0
+                O(e, t, n), We(r, t, null), i = !0
             },
             p(e, t) {
                 const n = {};
                 64 & t && (n.progress = e[6]), r.$set(n)
             },
             i(e) {
-                i || (Oe(r.$$.fragment, e), n || ge((() => {
-                    n = Ce(t, Ye, {}), n.start()
-                })), i = !0)
+                i || (Se(r.$$.fragment, e), e && (n || ve((() => {
+                    n = Re(t, Xe, {}), n.start()
+                }))), i = !0)
             },
             o(e) {
-                Se(r.$$.fragment, e), i = !1
+                De(r.$$.fragment, e), i = !1
             },
             d(e) {
-                e && O(t), He(r)
+                e && S(t), Ge(r)
             }
         }
     }
 
-    function Sp(t) {
+    function Dp(t) {
         let r, n, i, s, a, l, u, c, f, h, p, d, m;
-        return l = new Yn({
+        return l = new Kn({
             props: {
-                icon: cn
+                icon: fn
             }
-        }), h = new Yn({
+        }), h = new Kn({
             props: {
-                icon: _n
+                icon: kn
             }
         }), {
             c() {
-                r = D("li"), n = D("button"), n.textContent = "install", i = L(), s = D("li"), a = D("button"), Ve(l.$$.fragment), u = L(), c = D("li"), f = D("button"), Ve(h.$$.fragment), P(n, "class", "svelte-n5lp8"), P(r, "class", "svelte-n5lp8"), P(a, "aria-label", "open in browser"), P(a, "title", "open in browser"), P(a, "class", "svelte-n5lp8"), P(s, "class", "svelte-n5lp8"), P(f, "aria-label", "show options"), P(f, "title", "show options"), P(f, "class", "svelte-n5lp8"), P(c, "class", "svelte-n5lp8")
+                r = C("li"), n = C("button"), n.textContent = "install", i = N(), s = C("li"), a = C("button"), He(l.$$.fragment), u = N(), c = C("li"), f = C("button"), He(h.$$.fragment), j(n, "class", "svelte-n5lp8"), j(r, "class", "svelte-n5lp8"), j(a, "aria-label", "open in browser"), j(a, "title", "open in browser"), j(a, "class", "svelte-n5lp8"), j(s, "class", "svelte-n5lp8"), j(f, "aria-label", "show options"), j(f, "title", "show options"), j(f, "class", "svelte-n5lp8"), j(c, "class", "svelte-n5lp8")
             },
             m(e, o) {
-                $(e, r, o), q(r, n), $(e, i, o), $(e, s, o), q(s, a), ze(l, a, null), $(e, u, o), $(e, c, o), q(c, f), ze(h, f, null), p = !0, d || (m = [I(n, "click", M(t[14])), I(a, "click", M(t[15])), I(f, "click", M(t[16]))], d = !0)
+                O(e, r, o), E(r, n), O(e, i, o), O(e, s, o), E(s, a), We(l, a, null), O(e, u, o), O(e, c, o), E(c, f), We(h, f, null), p = !0, d || (m = [F(n, "click", P(t[14])), F(a, "click", P(t[15])), F(f, "click", P(t[16]))], d = !0)
             },
             p: e,
             i(e) {
-                p || (Oe(l.$$.fragment, e), Oe(h.$$.fragment, e), p = !0)
+                p || (Se(l.$$.fragment, e), Se(h.$$.fragment, e), p = !0)
             },
             o(e) {
-                Se(l.$$.fragment, e), Se(h.$$.fragment, e), p = !1
+                De(l.$$.fragment, e), De(h.$$.fragment, e), p = !1
             },
             d(e) {
-                e && O(r), e && O(i), e && O(s), He(l), e && O(u), e && O(c), He(h), d = !1, o(m)
+                e && (S(r), S(i), S(s), S(u), S(c)), Ge(l), Ge(h), d = !1, o(m)
             }
         }
     }
 
-    function Dp(e) {
-        let t, r, n, i, s, a, l, u, c, f, h, p = e[7] && Cp(e);
-        return i = new Yn({
+    function Cp(e) {
+        let t, r, n, i, s, a, l, u, c, f, h, p = e[7] && Rp(e);
+        return i = new Kn({
             props: {
-                icon: un
+                icon: cn
             }
-        }), u = new Yn({
+        }), u = new Kn({
             props: {
-                icon: _n
+                icon: kn
             }
         }), {
             c() {
-                p && p.c(), t = L(), r = D("li"), n = D("button"), Ve(i.$$.fragment), s = L(), a = D("li"), l = D("button"), Ve(u.$$.fragment), P(n, "aria-label", "remove"), P(n, "title", "remove"), n.disabled = e[5], P(n, "class", "svelte-n5lp8"), P(r, "class", "svelte-n5lp8"), P(l, "aria-label", "show options"), P(l, "title", "show options"), P(l, "class", "svelte-n5lp8"), P(a, "class", "svelte-n5lp8")
+                p && p.c(), t = N(), r = C("li"), n = C("button"), He(i.$$.fragment), s = N(), a = C("li"), l = C("button"), He(u.$$.fragment), j(n, "aria-label", "remove"), j(n, "title", "remove"), n.disabled = e[5], j(n, "class", "svelte-n5lp8"), j(r, "class", "svelte-n5lp8"), j(l, "aria-label", "show options"), j(l, "title", "show options"), j(l, "class", "svelte-n5lp8"), j(a, "class", "svelte-n5lp8")
             },
             m(o, d) {
-                p && p.m(o, d), $(o, t, d), $(o, r, d), q(r, n), ze(i, n, null), $(o, s, d), $(o, a, d), q(a, l), ze(u, l, null), c = !0, f || (h = [I(n, "click", M(e[12])), I(l, "click", M(e[13]))], f = !0)
+                p && p.m(o, d), O(o, t, d), O(o, r, d), E(r, n), We(i, n, null), O(o, s, d), O(o, a, d), E(a, l), We(u, l, null), c = !0, f || (h = [F(n, "click", P(e[12])), F(l, "click", P(e[13]))], f = !0)
             },
             p(e, r) {
-                e[7] ? p ? p.p(e, r) : (p = Cp(e), p.c(), p.m(t.parentNode, t)) : p && (p.d(1), p = null), (!c || 32 & r) && (n.disabled = e[5])
+                e[7] ? p ? p.p(e, r) : (p = Rp(e), p.c(), p.m(t.parentNode, t)) : p && (p.d(1), p = null), (!c || 32 & r) && (n.disabled = e[5])
             },
             i(e) {
-                c || (Oe(i.$$.fragment, e), Oe(u.$$.fragment, e), c = !0)
+                c || (Se(i.$$.fragment, e), Se(u.$$.fragment, e), c = !0)
             },
             o(e) {
-                Se(i.$$.fragment, e), Se(u.$$.fragment, e), c = !1
+                De(i.$$.fragment, e), De(u.$$.fragment, e), c = !1
             },
             d(e) {
-                p && p.d(e), e && O(t), e && O(r), He(i), e && O(s), e && O(a), He(u), f = !1, o(h)
+                e && (S(t), S(r), S(s), S(a)), p && p.d(e), Ge(i), Ge(u), f = !1, o(h)
             }
         }
     }
 
-    function Cp(e) {
+    function Rp(e) {
         let t, r, n, i, s, a, l, u;
         return {
             c() {
-                t = D("li"), r = D("button"), n = R("update"), i = L(), s = D("li"), a = D("button"), a.textContent = "changelog", r.disabled = e[5], P(r, "class", "svelte-n5lp8"), P(t, "class", "svelte-n5lp8"), P(a, "class", "svelte-n5lp8"), P(s, "class", "svelte-n5lp8")
+                t = C("li"), r = C("button"), n = L("update"), i = N(), s = C("li"), a = C("button"), a.textContent = "changelog", r.disabled = e[5], j(r, "class", "svelte-n5lp8"), j(t, "class", "svelte-n5lp8"), j(a, "class", "svelte-n5lp8"), j(s, "class", "svelte-n5lp8")
             },
             m(o, c) {
-                $(o, t, c), q(t, r), q(r, n), $(o, i, c), $(o, s, c), q(s, a), l || (u = [I(r, "click", M(e[10])), I(a, "click", M(e[11]))], l = !0)
+                O(o, t, c), E(t, r), E(r, n), O(o, i, c), O(o, s, c), E(s, a), l || (u = [F(r, "click", P(e[10])), F(a, "click", P(e[11]))], l = !0)
             },
             p(e, t) {
                 32 & t && (r.disabled = e[5])
             },
             d(e) {
-                e && O(t), e && O(i), e && O(s), l = !1, o(u)
+                e && (S(t), S(i), S(s)), l = !1, o(u)
             }
         }
     }
 
-    function Rp(e) {
+    function Lp(e) {
         let t, r, n, i, o, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _ = e[0].name + "",
             k = e[0].version + "",
-            x = pl.fromISO(e[1].date_published).toRelative() + "",
+            x = dl.fromISO(e[1].date_published).toRelative() + "",
             A = Object.values(e[1].options).some(Boolean),
-            E = e[7] && Ap(e),
-            T = A && qp(e),
-            S = e[4] !== Ah.Dense && Ep(e);
-        const C = [Op, $p],
-            N = [];
+            q = e[7] && qp(e),
+            T = A && Ep(e),
+            $ = e[4] !== qh.Dense && Tp(e);
+        const D = [Sp, Op],
+            R = [];
 
         function I(e, t) {
             return e[3] ? 0 : 1
         }
-        return y = I(e), b = N[y] = C[y](e), {
+        return y = I(e), b = R[y] = D[y](e), {
             c() {
-                t = D("div"), r = D("ul"), n = D("li"), i = R(_), o = L(), s = D("li"), a = R(k), l = L(), E && E.c(), u = L(), c = D("span"), f = R("("), h = R(x), p = R(")"), m = L(), T && T.c(), g = L(), S && S.c(), v = L(), b.c(), P(n, "class", "name svelte-n5lp8"), P(c, "class", "date svelte-n5lp8"), P(c, "title", d = e[1].date_published), P(s, "class", "versions svelte-n5lp8"), P(r, "class", "addon-details svelte-n5lp8"), J(r, "two-col", e[4] === Ah.Dense), P(t, "class", "addon svelte-n5lp8"), J(t, "status-outdated", e[7]), J(t, "status-pinned", e[0].options[Br.VersionEq]), J(t, "status-being-modified", e[3])
+                t = C("div"), r = C("ul"), n = C("li"), i = L(_), o = N(), s = C("li"), a = L(k), l = N(), q && q.c(), u = N(), c = C("span"), f = L("("), h = L(x), p = L(")"), m = N(), T && T.c(), g = N(), $ && $.c(), v = N(), b.c(), j(n, "class", "name svelte-n5lp8"), j(c, "class", "date svelte-n5lp8"), j(c, "title", d = e[1].date_published), j(s, "class", "versions svelte-n5lp8"), j(r, "class", "addon-details svelte-n5lp8"), Y(r, "two-col", e[4] === qh.Dense), j(t, "class", "addon svelte-n5lp8"), Y(t, "status-outdated", e[7]), Y(t, "status-pinned", e[0].options[Ur.VersionEq]), Y(t, "status-being-modified", e[3])
             },
             m(e, d) {
-                $(e, t, d), q(t, r), q(r, n), q(n, i), q(r, o), q(r, s), q(s, a), q(s, l), E && E.m(s, null), q(s, u), q(s, c), q(c, f), q(c, h), q(c, p), q(s, m), T && T.m(s, null), q(r, g), S && S.m(r, null), q(t, v), N[y].m(t, null), w = !0
+                O(e, t, d), E(t, r), E(r, n), E(n, i), E(r, o), E(r, s), E(s, a), E(s, l), q && q.m(s, null), E(s, u), E(s, c), E(c, f), E(c, h), E(c, p), E(s, m), T && T.m(s, null), E(r, g), $ && $.m(r, null), E(t, v), R[y].m(t, null), w = !0
             },
             p(e, [n]) {
-                (!w || 1 & n) && _ !== (_ = e[0].name + "") && U(i, _), (!w || 1 & n) && k !== (k = e[0].version + "") && U(a, k), e[7] ? E ? E.p(e, n) : (E = Ap(e), E.c(), E.m(s, u)) : E && (E.d(1), E = null), (!w || 2 & n) && x !== (x = pl.fromISO(e[1].date_published).toRelative() + "") && U(h, x), (!w || 2 & n && d !== (d = e[1].date_published)) && P(c, "title", d), 2 & n && (A = Object.values(e[1].options).some(Boolean)), A ? T ? T.p(e, n) : (T = qp(e), T.c(), T.m(s, null)) : T && (T.d(1), T = null), e[4] !== Ah.Dense ? S ? S.p(e, n) : (S = Ep(e), S.c(), S.m(r, null)) : S && (S.d(1), S = null), (!w || 16 & n) && J(r, "two-col", e[4] === Ah.Dense);
+                (!w || 1 & n) && _ !== (_ = e[0].name + "") && V(i, _), (!w || 1 & n) && k !== (k = e[0].version + "") && V(a, k), e[7] ? q ? q.p(e, n) : (q = qp(e), q.c(), q.m(s, u)) : q && (q.d(1), q = null), (!w || 2 & n) && x !== (x = dl.fromISO(e[1].date_published).toRelative() + "") && V(h, x), (!w || 2 & n && d !== (d = e[1].date_published)) && j(c, "title", d), 2 & n && (A = Object.values(e[1].options).some(Boolean)), A ? T ? T.p(e, n) : (T = Ep(e), T.c(), T.m(s, null)) : T && (T.d(1), T = null), e[4] !== qh.Dense ? $ ? $.p(e, n) : ($ = Tp(e), $.c(), $.m(r, null)) : $ && ($.d(1), $ = null), (!w || 16 & n) && Y(r, "two-col", e[4] === qh.Dense);
                 let o = y;
-                y = I(e), y === o ? N[y].p(e, n) : (Te(), Se(N[o], 1, 1, (() => {
-                    N[o] = null
-                })), $e(), b = N[y], b ? b.p(e, n) : (b = N[y] = C[y](e), b.c()), Oe(b, 1), b.m(t, null)), (!w || 128 & n) && J(t, "status-outdated", e[7]), (!w || 1 & n) && J(t, "status-pinned", e[0].options[Br.VersionEq]), (!w || 8 & n) && J(t, "status-being-modified", e[3])
+                y = I(e), y === o ? R[y].p(e, n) : ($e(), De(R[o], 1, 1, (() => {
+                    R[o] = null
+                })), Oe(), b = R[y], b ? b.p(e, n) : (b = R[y] = D[y](e), b.c()), Se(b, 1), b.m(t, null)), (!w || 128 & n) && Y(t, "status-outdated", e[7]), (!w || 1 & n) && Y(t, "status-pinned", e[0].options[Ur.VersionEq]), (!w || 8 & n) && Y(t, "status-being-modified", e[3])
             },
             i(e) {
-                w || (Oe(b), w = !0)
+                w || (Se(b), w = !0)
             },
             o(e) {
-                Se(b), w = !1
+                De(b), w = !1
             },
             d(e) {
-                e && O(t), E && E.d(), T && T.d(), S && S.d(), N[y].d()
+                e && S(t), q && q.d(), T && T.d(), $ && $.d(), R[y].d()
             }
         }
     }
-    const Lp = ([, e]) => e,
-        Np = ([e]) => ` @ ${e}`;
+    const Np = ([, e]) => e,
+        Ip = ([e]) => ` @ ${e}`;
 
-    function Ip(e, t, r) {
+    function Fp(e, t, r) {
         let n, i;
-        c(e, nn, (e => r(8, i = e)));
+        c(e, on, (e => r(8, i = e)));
         let {
             addon: o,
             otherAddon: s,
             isInstalled: a,
             beingModified: l,
             format: u,
             isRefreshing: f,
             downloadProgress: h
         } = t;
-        const p = se();
+        const p = ae();
         return e.$$set = e => {
             "addon" in e && r(0, o = e.addon), "otherAddon" in e && r(1, s = e.otherAddon), "isInstalled" in e && r(2, a = e.isInstalled), "beingModified" in e && r(3, l = e.beingModified), "format" in e && r(4, u = e.format), "isRefreshing" in e && r(5, f = e.isRefreshing), "downloadProgress" in e && r(6, h = e.downloadProgress)
         }, e.$$.update = () => {
             3 & e.$$.dirty && r(7, n = o.version !== s.version)
         }, [o, s, a, l, u, f, h, n, i, p, () => p("requestUpdate"), () => p("requestShowChangelogModal"), () => p("requestRemove"), e => p("requestShowAddonContextMenu", {
             mouseEvent: e
         }), () => p("requestInstall"), () => i.openUrl(o.url), e => p("requestShowAddonContextMenu", {
             mouseEvent: e
         })]
     }
-    class Fp extends Ze {
+    class Mp extends Ye {
         constructor(e) {
-            super(), Ge(this, e, Ip, Rp, a, {
+            super(), Je(this, e, Fp, Lp, a, {
                 addon: 0,
                 otherAddon: 1,
                 isInstalled: 2,
                 beingModified: 3,
                 format: 4,
                 isRefreshing: 5,
                 downloadProgress: 6
             })
         }
     }
 
-    function Mp(e, {
+    function Pp(e, {
         from: t,
         to: r
     }, n = {}) {
         const i = getComputedStyle(e),
             o = "none" === i.transform ? "" : i.transform,
             [a, l] = i.transformOrigin.split(" ").map(parseFloat),
             u = t.left + t.width * a / r.width - (r.left + a),
             c = t.top + t.height * l / r.height - (r.top + l),
             {
                 delay: f = 0,
                 duration: h = (e => 120 * Math.sqrt(e)),
-                easing: p = Je
+                easing: p = Ke
             } = n;
         return {
             delay: f,
             duration: s(h) ? h(Math.sqrt(u * u + c * c)) : h,
             easing: p,
             css: (e, n) => {
                 const i = n * u,
@@ -20146,15 +20166,15 @@
                     a = e + n * t.width / r.width,
                     l = e + n * t.height / r.height;
                 return `transform: ${o} translate(${i}px, ${s}px) scale(${a}, ${l});`
             }
         }
     }
 
-    function Pp(e) {
+    function jp(e) {
         switch (e._type) {
             case "document":
             case "block_quote":
             case "list":
             case "item":
             case "paragraph":
             case "heading":
@@ -20165,190 +20185,190 @@
             case "custom_inline":
             case "custom_block":
                 return !0;
             default:
                 return !1
         }
     }
-    var jp = function(e, t) {
+    var Bp = function(e, t) {
             this.current = e, this.entering = !0 === t
         },
-        Bp = function() {
+        Up = function() {
             var e = this.current,
                 t = this.entering;
             if (null === e) return null;
-            var r = Pp(e);
+            var r = jp(e);
             return t && r ? e._firstChild ? (this.current = e._firstChild, this.entering = !0) : this.entering = !1 : e === this.root ? this.current = null : null === e._next ? (this.current = e._parent, this.entering = !1) : (this.current = e._next, this.entering = !0), {
                 entering: t,
                 node: e
             }
         },
-        Up = function(e) {
+        Vp = function(e) {
             return {
                 current: e,
                 root: e,
                 entering: !0,
-                next: Bp,
-                resumeAt: jp
+                next: Up,
+                resumeAt: Bp
             }
         },
-        Vp = function(e, t) {
+        zp = function(e, t) {
             this._type = e, this._parent = null, this._firstChild = null, this._lastChild = null, this._prev = null, this._next = null, this._sourcepos = t, this._lastLineBlank = !1, this._lastLineChecked = !1, this._open = !0, this._string_content = null, this._literal = null, this._listData = {}, this._info = null, this._destination = null, this._title = null, this._isFenced = !1, this._fenceChar = null, this._fenceLength = 0, this._fenceOffset = null, this._level = null, this._onEnter = null, this._onExit = null
         },
-        zp = Vp.prototype;
-    Object.defineProperty(zp, "isContainer", {
+        Hp = zp.prototype;
+    Object.defineProperty(Hp, "isContainer", {
         get: function() {
-            return Pp(this)
+            return jp(this)
         }
-    }), Object.defineProperty(zp, "type", {
+    }), Object.defineProperty(Hp, "type", {
         get: function() {
             return this._type
         }
-    }), Object.defineProperty(zp, "firstChild", {
+    }), Object.defineProperty(Hp, "firstChild", {
         get: function() {
             return this._firstChild
         }
-    }), Object.defineProperty(zp, "lastChild", {
+    }), Object.defineProperty(Hp, "lastChild", {
         get: function() {
             return this._lastChild
         }
-    }), Object.defineProperty(zp, "next", {
+    }), Object.defineProperty(Hp, "next", {
         get: function() {
             return this._next
         }
-    }), Object.defineProperty(zp, "prev", {
+    }), Object.defineProperty(Hp, "prev", {
         get: function() {
             return this._prev
         }
-    }), Object.defineProperty(zp, "parent", {
+    }), Object.defineProperty(Hp, "parent", {
         get: function() {
             return this._parent
         }
-    }), Object.defineProperty(zp, "sourcepos", {
+    }), Object.defineProperty(Hp, "sourcepos", {
         get: function() {
             return this._sourcepos
         }
-    }), Object.defineProperty(zp, "literal", {
+    }), Object.defineProperty(Hp, "literal", {
         get: function() {
             return this._literal
         },
         set: function(e) {
             this._literal = e
         }
-    }), Object.defineProperty(zp, "destination", {
+    }), Object.defineProperty(Hp, "destination", {
         get: function() {
             return this._destination
         },
         set: function(e) {
             this._destination = e
         }
-    }), Object.defineProperty(zp, "title", {
+    }), Object.defineProperty(Hp, "title", {
         get: function() {
             return this._title
         },
         set: function(e) {
             this._title = e
         }
-    }), Object.defineProperty(zp, "info", {
+    }), Object.defineProperty(Hp, "info", {
         get: function() {
             return this._info
         },
         set: function(e) {
             this._info = e
         }
-    }), Object.defineProperty(zp, "level", {
+    }), Object.defineProperty(Hp, "level", {
         get: function() {
             return this._level
         },
         set: function(e) {
             this._level = e
         }
-    }), Object.defineProperty(zp, "listType", {
+    }), Object.defineProperty(Hp, "listType", {
         get: function() {
             return this._listData.type
         },
         set: function(e) {
             this._listData.type = e
         }
-    }), Object.defineProperty(zp, "listTight", {
+    }), Object.defineProperty(Hp, "listTight", {
         get: function() {
             return this._listData.tight
         },
         set: function(e) {
             this._listData.tight = e
         }
-    }), Object.defineProperty(zp, "listStart", {
+    }), Object.defineProperty(Hp, "listStart", {
         get: function() {
             return this._listData.start
         },
         set: function(e) {
             this._listData.start = e
         }
-    }), Object.defineProperty(zp, "listDelimiter", {
+    }), Object.defineProperty(Hp, "listDelimiter", {
         get: function() {
             return this._listData.delimiter
         },
         set: function(e) {
             this._listData.delimiter = e
         }
-    }), Object.defineProperty(zp, "onEnter", {
+    }), Object.defineProperty(Hp, "onEnter", {
         get: function() {
             return this._onEnter
         },
         set: function(e) {
             this._onEnter = e
         }
-    }), Object.defineProperty(zp, "onExit", {
+    }), Object.defineProperty(Hp, "onExit", {
         get: function() {
             return this._onExit
         },
         set: function(e) {
             this._onExit = e
         }
-    }), Vp.prototype.appendChild = function(e) {
+    }), zp.prototype.appendChild = function(e) {
         e.unlink(), e._parent = this, this._lastChild ? (this._lastChild._next = e, e._prev = this._lastChild, this._lastChild = e) : (this._firstChild = e, this._lastChild = e)
-    }, Vp.prototype.prependChild = function(e) {
+    }, zp.prototype.prependChild = function(e) {
         e.unlink(), e._parent = this, this._firstChild ? (this._firstChild._prev = e, e._next = this._firstChild, this._firstChild = e) : (this._firstChild = e, this._lastChild = e)
-    }, Vp.prototype.unlink = function() {
+    }, zp.prototype.unlink = function() {
         this._prev ? this._prev._next = this._next : this._parent && (this._parent._firstChild = this._next), this._next ? this._next._prev = this._prev : this._parent && (this._parent._lastChild = this._prev), this._parent = null, this._next = null, this._prev = null
-    }, Vp.prototype.insertAfter = function(e) {
+    }, zp.prototype.insertAfter = function(e) {
         e.unlink(), e._next = this._next, e._next && (e._next._prev = e), e._prev = this, this._next = e, e._parent = this._parent, e._next || (e._parent._lastChild = e)
-    }, Vp.prototype.insertBefore = function(e) {
+    }, zp.prototype.insertBefore = function(e) {
         e.unlink(), e._prev = this._prev, e._prev && (e._prev._next = e), e._next = this, this._prev = e, e._parent = this._parent, e._prev || (e._parent._firstChild = e)
-    }, Vp.prototype.walker = function() {
-        return new Up(this)
+    }, zp.prototype.walker = function() {
+        return new Vp(this)
     };
-    var Hp = {};
+    var Wp = {};
 
-    function Wp(e, t, r) {
+    function Gp(e, t, r) {
         var n, i, o, s, a, l = "";
-        for ("string" != typeof t && (r = t, t = Wp.defaultChars), void 0 === r && (r = !0), a = function(e) {
-                var t, r, n = Hp[e];
+        for ("string" != typeof t && (r = t, t = Gp.defaultChars), void 0 === r && (r = !0), a = function(e) {
+                var t, r, n = Wp[e];
                 if (n) return n;
-                for (n = Hp[e] = [], t = 0; t < 128; t++) r = String.fromCharCode(t), /^[0-9a-z]$/i.test(r) ? n.push(r) : n.push("%" + ("0" + t.toString(16).toUpperCase()).slice(-2));
+                for (n = Wp[e] = [], t = 0; t < 128; t++) r = String.fromCharCode(t), /^[0-9a-z]$/i.test(r) ? n.push(r) : n.push("%" + ("0" + t.toString(16).toUpperCase()).slice(-2));
                 for (t = 0; t < e.length; t++) n[e.charCodeAt(t)] = e[t];
                 return n
             }(t), n = 0, i = e.length; n < i; n++)
             if (o = e.charCodeAt(n), r && 37 === o && n + 2 < i && /^[0-9a-f]{2}$/i.test(e.slice(n + 1, n + 3))) l += e.slice(n, n + 3), n += 2;
             else if (o < 128) l += a[o];
         else if (o >= 55296 && o <= 57343) {
             if (o >= 55296 && o <= 56319 && n + 1 < i && (s = e.charCodeAt(n + 1)) >= 56320 && s <= 57343) {
                 l += encodeURIComponent(e[n] + e[n + 1]), n++;
                 continue
             }
             l += "%EF%BF%BD"
         } else l += encodeURIComponent(e[n]);
         return l
     }
-    Wp.defaultChars = ";/?:@&=+$,-_.!~*'()#", Wp.componentChars = "-_.!~*'()";
-    var Gp = Wp,
-        Zp = it(Gp),
-        Jp = {},
+    Gp.defaultChars = ";/?:@&=+$,-_.!~*'()#", Gp.componentChars = "-_.!~*'()";
+    var Zp = Gp,
+        Jp = st(Zp),
         Yp = {},
-        Kp = {
+        Kp = {},
+        Xp = {
             Aacute: "Á",
             aacute: "á",
             Abreve: "Ă",
             abreve: "ă",
             ac: "∾",
             acd: "∿",
             acE: "∾̳",
@@ -22467,15 +22487,15 @@
             zopf: "𝕫",
             Zopf: "ℤ",
             Zscr: "𝒵",
             zscr: "𝓏",
             zwj: "‍",
             zwnj: "‌"
         },
-        Xp = {
+        Qp = {
             Aacute: "Á",
             aacute: "á",
             Acirc: "Â",
             acirc: "â",
             acute: "´",
             AElig: "Æ",
             aelig: "æ",
@@ -22575,31 +22595,31 @@
             Uuml: "Ü",
             uuml: "ü",
             Yacute: "Ý",
             yacute: "ý",
             yen: "¥",
             yuml: "ÿ"
         },
-        Qp = {
+        ed = {
             amp: "&",
             apos: "'",
             gt: ">",
             lt: "<",
             quot: '"'
         },
-        ed = {},
-        td = nt && nt.__importDefault || function(e) {
+        td = {},
+        rd = ot && ot.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
-    Object.defineProperty(ed, "__esModule", {
+    Object.defineProperty(td, "__esModule", {
         value: !0
     });
-    var rd = td({
+    var nd = rd({
         0: 65533,
         128: 8364,
         130: 8218,
         131: 402,
         132: 8222,
         133: 8230,
         134: 8224,
@@ -22621,133 +22641,133 @@
         153: 8482,
         154: 353,
         155: 8250,
         156: 339,
         158: 382,
         159: 376
     });
-    ed.default = function(e) {
+    td.default = function(e) {
         if (e >= 55296 && e <= 57343 || e > 1114111) return "�";
-        e in rd.default && (e = rd.default[e]);
+        e in nd.default && (e = nd.default[e]);
         var t = "";
         return e > 65535 && (e -= 65536, t += String.fromCharCode(e >>> 10 & 1023 | 55296), e = 56320 | 1023 & e), t += String.fromCharCode(e)
     };
-    var nd = nt && nt.__importDefault || function(e) {
+    var id = ot && ot.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
         }
     };
-    Object.defineProperty(Yp, "__esModule", {
+    Object.defineProperty(Kp, "__esModule", {
         value: !0
-    }), Yp.decodeHTML = Yp.decodeHTMLStrict = Yp.decodeXML = void 0;
-    var id = nd(Kp),
-        od = nd(Xp),
-        sd = nd(Qp),
-        ad = nd(ed);
+    }), Kp.decodeHTML = Kp.decodeHTMLStrict = Kp.decodeXML = void 0;
+    var od = id(Xp),
+        sd = id(Qp),
+        ad = id(ed),
+        ld = id(td);
 
-    function ld(e) {
+    function ud(e) {
         var t = Object.keys(e).join("|"),
-            r = cd(e),
+            r = fd(e),
             n = new RegExp("&(?:" + (t += "|#[xX][\\da-fA-F]+|#\\d+") + ");", "g");
         return function(e) {
             return String(e).replace(n, r)
         }
     }
-    Yp.decodeXML = ld(sd.default), Yp.decodeHTMLStrict = ld(id.default);
-    var ud = function(e, t) {
+    Kp.decodeXML = ud(ad.default), Kp.decodeHTMLStrict = ud(od.default);
+    var cd = function(e, t) {
         return e < t ? 1 : -1
     };
 
-    function cd(e) {
+    function fd(e) {
         return function(t) {
             if ("#" === t.charAt(1)) {
                 var r = t.charAt(2);
-                return "X" === r || "x" === r ? ad.default(parseInt(t.substr(3), 16)) : ad.default(parseInt(t.substr(2), 10))
+                return "X" === r || "x" === r ? ld.default(parseInt(t.substr(3), 16)) : ld.default(parseInt(t.substr(2), 10))
             }
             return e[t.slice(1, -1)]
         }
     }
-    Yp.decodeHTML = function() {
-        for (var e = Object.keys(od.default).sort(ud), t = Object.keys(id.default).sort(ud), r = 0, n = 0; r < t.length; r++) e[n] === t[r] ? (t[r] += ";?", n++) : t[r] += ";";
+    Kp.decodeHTML = function() {
+        for (var e = Object.keys(sd.default).sort(cd), t = Object.keys(od.default).sort(cd), r = 0, n = 0; r < t.length; r++) e[n] === t[r] ? (t[r] += ";?", n++) : t[r] += ";";
         var i = new RegExp("&(?:" + t.join("|") + "|#[xX][\\da-fA-F]+;?|#\\d+;?)", "g"),
-            o = cd(id.default);
+            o = fd(od.default);
 
         function s(e) {
             return ";" !== e.substr(-1) && (e += ";"), o(e)
         }
         return function(e) {
             return String(e).replace(i, s)
         }
     }();
-    var fd = {},
-        hd = nt && nt.__importDefault || function(e) {
+    var hd = {},
+        pd = ot && ot.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
-    Object.defineProperty(fd, "__esModule", {
+    Object.defineProperty(hd, "__esModule", {
         value: !0
-    }), fd.escape = fd.encodeHTML = fd.encodeXML = void 0;
-    var pd = vd(hd(Qp).default),
-        dd = yd(pd);
-    fd.encodeXML = _d(pd, dd);
-    var md = vd(hd(Kp).default),
-        gd = yd(md);
+    }), hd.escape = hd.encodeHTML = hd.encodeXML = void 0;
+    var dd = yd(pd(ed).default),
+        md = bd(dd);
+    hd.encodeXML = kd(dd, md);
+    var gd = yd(pd(Xp).default),
+        vd = bd(gd);
 
-    function vd(e) {
+    function yd(e) {
         return Object.keys(e).sort().reduce((function(t, r) {
             return t[e[r]] = "&" + r + ";", t
         }), {})
     }
 
-    function yd(e) {
+    function bd(e) {
         for (var t = [], r = [], n = 0, i = Object.keys(e); n < i.length; n++) {
             var o = i[n];
             1 === o.length ? t.push("\\" + o) : r.push(o)
         }
         t.sort();
         for (var s = 0; s < t.length - 1; s++) {
             for (var a = s; a < t.length - 1 && t[a].charCodeAt(1) + 1 === t[a + 1].charCodeAt(1);) a += 1;
             var l = 1 + a - s;
             l < 3 || t.splice(s, l, t[s] + "-" + t[a])
         }
         return r.unshift("[" + t.join("") + "]"), new RegExp(r.join("|"), "g")
     }
-    fd.encodeHTML = _d(md, gd);
-    var bd = /(?:[\x80-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])/g;
+    hd.encodeHTML = kd(gd, vd);
+    var wd = /(?:[\x80-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF])/g;
 
-    function wd(e) {
+    function _d(e) {
         return "&#x" + e.codePointAt(0).toString(16).toUpperCase() + ";"
     }
 
-    function _d(e, t) {
+    function kd(e, t) {
         return function(r) {
             return r.replace(t, (function(t) {
                 return e[t]
-            })).replace(bd, wd)
+            })).replace(wd, _d)
         }
     }
-    var kd = yd(pd);
-    fd.escape = function(e) {
-            return e.replace(kd, wd).replace(bd, wd)
+    var xd = bd(dd);
+    hd.escape = function(e) {
+            return e.replace(xd, _d).replace(wd, _d)
         },
         function(e) {
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.encode = e.decodeStrict = e.decode = void 0;
-            var t = Yp,
-                r = fd;
+            var t = Kp,
+                r = hd;
             e.decode = function(e, r) {
                 return (!r || r <= 0 ? t.decodeXML : t.decodeHTML)(e)
             }, e.decodeStrict = function(e, r) {
                 return (!r || r <= 0 ? t.decodeXML : t.decodeHTMLStrict)(e)
             }, e.encode = function(e, t) {
                 return (!t || t <= 0 ? r.encodeXML : r.encodeHTML)(e)
             };
-            var n = fd;
+            var n = hd;
             Object.defineProperty(e, "encodeXML", {
                 enumerable: !0,
                 get: function() {
                     return n.encodeXML
                 }
             }), Object.defineProperty(e, "encodeHTML", {
                 enumerable: !0,
@@ -22766,15 +22786,15 @@
                 }
             }), Object.defineProperty(e, "encodeHTML5", {
                 enumerable: !0,
                 get: function() {
                     return n.encodeHTML
                 }
             });
-            var i = Yp;
+            var i = Kp;
             Object.defineProperty(e, "decodeXML", {
                 enumerable: !0,
                 get: function() {
                     return i.decodeXML
                 }
             }), Object.defineProperty(e, "decodeHTML", {
                 enumerable: !0,
@@ -22808,71 +22828,71 @@
                 }
             }), Object.defineProperty(e, "decodeXMLStrict", {
                 enumerable: !0,
                 get: function() {
                     return i.decodeXML
                 }
             })
-        }(Jp);
-    var xd, Ad = "&(?:#x[a-f0-9]{1,6}|#[0-9]{1,7}|[a-z][a-z0-9]{1,31});",
-        qd = "[A-Za-z][A-Za-z0-9-]*",
-        Ed = "<" + qd + "(?:\\s+[a-zA-Z_:][a-zA-Z0-9:._-]*(?:\\s*=\\s*(?:[^\"'=<>`\\x00-\\x20]+|'[^']*'|\"[^\"]*\"))?)*\\s*/?>",
-        Td = "</" + qd + "\\s*[>]",
-        $d = new RegExp("^" + ("(?:" + Ed + "|" + Td + "|\x3c!----\x3e|\x3c!--(?:-?[^>-])(?:-?[^-])*--\x3e|[<][?][\\s\\S]*?[?][>]|<![A-Z]+\\s+[^>]*>|<!\\[CDATA\\[[\\s\\S]*?\\]\\]>)")),
-        Od = /[\\&]/,
-        Sd = "[!\"#$%&'()*+,./:;<=>?@[\\\\\\]^_`{|}~-]",
-        Dd = new RegExp("\\\\" + Sd + "|" + Ad, "gi"),
-        Cd = new RegExp('[&<>"]', "g"),
-        Rd = function(e) {
-            return 92 === e.charCodeAt(0) ? e.charAt(1) : Jp.decodeHTML(e)
-        },
+        }(Yp);
+    var Ad, qd = "&(?:#x[a-f0-9]{1,6}|#[0-9]{1,7}|[a-z][a-z0-9]{1,31});",
+        Ed = "[A-Za-z][A-Za-z0-9-]*",
+        Td = "<" + Ed + "(?:\\s+[a-zA-Z_:][a-zA-Z0-9:._-]*(?:\\s*=\\s*(?:[^\"'=<>`\\x00-\\x20]+|'[^']*'|\"[^\"]*\"))?)*\\s*/?>",
+        $d = "</" + Ed + "\\s*[>]",
+        Od = new RegExp("^" + ("(?:" + Td + "|" + $d + "|\x3c!----\x3e|\x3c!--(?:-?[^>-])(?:-?[^-])*--\x3e|[<][?][\\s\\S]*?[?][>]|<![A-Z]+\\s+[^>]*>|<!\\[CDATA\\[[\\s\\S]*?\\]\\]>)")),
+        Sd = /[\\&]/,
+        Dd = "[!\"#$%&'()*+,./:;<=>?@[\\\\\\]^_`{|}~-]",
+        Cd = new RegExp("\\\\" + Dd + "|" + qd, "gi"),
+        Rd = new RegExp('[&<>"]', "g"),
         Ld = function(e) {
-            return Od.test(e) ? e.replace(Dd, Rd) : e
+            return 92 === e.charCodeAt(0) ? e.charAt(1) : Yp.decodeHTML(e)
         },
         Nd = function(e) {
+            return Sd.test(e) ? e.replace(Cd, Ld) : e
+        },
+        Id = function(e) {
             switch (e) {
                 case "&":
                     return "&amp;";
                 case "<":
                     return "&lt;";
                 case ">":
                     return "&gt;";
                 case '"':
                     return "&quot;";
                 default:
                     return e
             }
         },
-        Id = function(e) {
-            return Cd.test(e) ? e.replace(Cd, Nd) : e
+        Fd = function(e) {
+            return Rd.test(e) ? e.replace(Rd, Id) : e
         };
 
-    function Fd(e) {
-        return xd(e)
+    function Md(e) {
+        return Ad(e)
     }
-    if (String.fromCodePoint) xd = function(e) {
+    if (String.fromCodePoint) Ad = function(e) {
         try {
             return String.fromCodePoint(e)
         } catch (e) {
             if (e instanceof RangeError) return String.fromCharCode(65533);
             throw e
         }
     };
     else {
-        var Md = String.fromCharCode,
-            Pd = Math.floor;
-        xd = function() {
+        var Pd = String.fromCharCode,
+            jd = Math.floor;
+        Ad = function() {
             var e, t, r = [],
                 n = -1,
                 i = arguments.length;
             if (!i) return "";
             for (var o = ""; ++n < i;) {
                 var s = Number(arguments[n]);
-                if (!isFinite(s) || s < 0 || s > 1114111 || Pd(s) !== s) return String.fromCharCode(65533);
-                s <= 65535 ? r.push(s) : (e = 55296 + ((s -= 65536) >> 10), t = s % 1024 + 56320, r.push(e, t)), (n + 1 === i || r.length > 16384) && (o += Md.apply(null, r), r.length = 0)
+                if (!isFinite(s) || s < 0 || s > 1114111 || jd(s) !== s) return String.fromCharCode(65533);
+                s <= 65535 ? r.push(s) : (e = 55296 + ((s -= 65536) >> 10), t = s % 1024 + 56320, r.push(e, t)), (n + 1 === i || r.length > 16384) && (o += Pd.apply(null, r), r.length = 0)
             }
             return o
         }
     }
     /*! http://mths.be/repeat v0.2.0 by @mathias */
     String.prototype.repeat || function() {
         var e = function() {
@@ -22893,132 +22913,132 @@
             };
         e ? e(String.prototype, "repeat", {
             value: t,
             configurable: !0,
             writable: !0
         }) : String.prototype.repeat = t
     }();
-    var jd = function(e) {
+    var Bd = function(e) {
             try {
-                return Zp(e)
+                return Jp(e)
             } catch (t) {
                 return e
             }
         },
-        Bd = Ld,
-        Ud = 39,
-        Vd = 34,
-        zd = Sd,
-        Hd = "\\\\" + zd,
-        Wd = Ad,
-        Gd = $d,
-        Zd = new RegExp(/^[!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u0AF0\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E42\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC9\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDF3C-\uDF3E]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]/),
-        Jd = new RegExp('^(?:"(' + Hd + '|[^"\\x00])*"|\'(' + Hd + "|[^'\\x00])*'|\\((" + Hd + "|[^()\\x00])*\\))"),
-        Yd = /^(?:<(?:[^<>\n\\\x00]|\\.)*>)/,
-        Kd = new RegExp("^" + zd),
-        Xd = new RegExp("^" + Wd, "i"),
-        Qd = /`+/,
-        em = /^`+/,
-        tm = /\.\.\./g,
-        rm = /--+/g,
-        nm = /^<([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)>/,
-        im = /^<[A-Za-z][A-Za-z0-9.+-]{1,31}:[^<>\x00-\x20]*>/i,
-        om = /^ *(?:\n *)?/,
-        sm = /^[ \t\n\x0b\x0c\x0d]/,
-        am = /^\s/,
-        lm = / *$/,
-        um = /^ */,
-        cm = /^ *(?:\n|$)/,
-        fm = /^\[(?:[^\\\[\]]|\\.){0,1000}\]/s,
-        hm = /^[^\n`\[\]\\!<&*_'"]+/m,
-        pm = function(e) {
-            var t = new Vp("text");
+        Ud = Nd,
+        Vd = 39,
+        zd = 34,
+        Hd = Dd,
+        Wd = "\\\\" + Hd,
+        Gd = qd,
+        Zd = Od,
+        Jd = new RegExp(/^[!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u0AF0\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E42\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC9\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDF3C-\uDF3E]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]/),
+        Yd = new RegExp('^(?:"(' + Wd + '|[^"\\x00])*"|\'(' + Wd + "|[^'\\x00])*'|\\((" + Wd + "|[^()\\x00])*\\))"),
+        Kd = /^(?:<(?:[^<>\n\\\x00]|\\.)*>)/,
+        Xd = new RegExp("^" + Hd),
+        Qd = new RegExp("^" + Gd, "i"),
+        em = /`+/,
+        tm = /^`+/,
+        rm = /\.\.\./g,
+        nm = /--+/g,
+        im = /^<([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)>/,
+        om = /^<[A-Za-z][A-Za-z0-9.+-]{1,31}:[^<>\x00-\x20]*>/i,
+        sm = /^ *(?:\n *)?/,
+        am = /^[ \t\n\x0b\x0c\x0d]/,
+        lm = /^\s/,
+        um = / *$/,
+        cm = /^ */,
+        fm = /^ *(?:\n|$)/,
+        hm = /^\[(?:[^\\\[\]]|\\.){0,1000}\]/s,
+        pm = /^[^\n`\[\]\\!<&*_'"]+/m,
+        dm = function(e) {
+            var t = new zp("text");
             return t._literal = e, t
         },
-        dm = function(e) {
+        mm = function(e) {
             return e.slice(1, e.length - 1).trim().replace(/[ \t\r\n]+/, " ").toLowerCase().toUpperCase()
         },
-        mm = function(e) {
+        gm = function(e) {
             var t = e.exec(this.subject.slice(this.pos));
             return null === t ? null : (this.pos += t.index + t[0].length, t[0])
         },
-        gm = function() {
+        vm = function() {
             return this.pos < this.subject.length ? this.subject.charCodeAt(this.pos) : -1
         },
-        vm = function() {
-            return this.match(om), !0
+        ym = function() {
+            return this.match(sm), !0
         },
-        ym = function(e) {
-            var t = this.match(em);
+        bm = function(e) {
+            var t = this.match(tm);
             if (null === t) return !1;
-            for (var r, n, i, o = this.pos; null !== (r = this.match(Qd));)
-                if (r === t) return n = new Vp("code"), (i = this.subject.slice(o, this.pos - t.length).replace(/\n/gm, " ")).length > 0 && null !== i.match(/[^ ]/) && " " == i[0] && " " == i[i.length - 1] ? n._literal = i.slice(1, i.length - 1) : n._literal = i, e.appendChild(n), !0;
-            return this.pos = o, e.appendChild(pm(t)), !0
+            for (var r, n, i, o = this.pos; null !== (r = this.match(em));)
+                if (r === t) return n = new zp("code"), (i = this.subject.slice(o, this.pos - t.length).replace(/\n/gm, " ")).length > 0 && null !== i.match(/[^ ]/) && " " == i[0] && " " == i[i.length - 1] ? n._literal = i.slice(1, i.length - 1) : n._literal = i, e.appendChild(n), !0;
+            return this.pos = o, e.appendChild(dm(t)), !0
         },
-        bm = function(e) {
+        wm = function(e) {
             var t, r = this.subject;
-            return this.pos += 1, 10 === this.peek() ? (this.pos += 1, t = new Vp("linebreak"), e.appendChild(t)) : Kd.test(r.charAt(this.pos)) ? (e.appendChild(pm(r.charAt(this.pos))), this.pos += 1) : e.appendChild(pm("\\")), !0
+            return this.pos += 1, 10 === this.peek() ? (this.pos += 1, t = new zp("linebreak"), e.appendChild(t)) : Xd.test(r.charAt(this.pos)) ? (e.appendChild(dm(r.charAt(this.pos))), this.pos += 1) : e.appendChild(dm("\\")), !0
         },
-        wm = function(e) {
+        _m = function(e) {
             var t, r, n;
-            return (t = this.match(nm)) ? (r = t.slice(1, t.length - 1), (n = new Vp("link"))._destination = jd("mailto:" + r), n._title = "", n.appendChild(pm(r)), e.appendChild(n), !0) : !!(t = this.match(im)) && (r = t.slice(1, t.length - 1), (n = new Vp("link"))._destination = jd(r), n._title = "", n.appendChild(pm(r)), e.appendChild(n), !0)
+            return (t = this.match(im)) ? (r = t.slice(1, t.length - 1), (n = new zp("link"))._destination = Bd("mailto:" + r), n._title = "", n.appendChild(dm(r)), e.appendChild(n), !0) : !!(t = this.match(om)) && (r = t.slice(1, t.length - 1), (n = new zp("link"))._destination = Bd(r), n._title = "", n.appendChild(dm(r)), e.appendChild(n), !0)
         },
-        _m = function(e) {
-            var t = this.match(Gd);
+        km = function(e) {
+            var t = this.match(Zd);
             if (null === t) return !1;
-            var r = new Vp("html_inline");
+            var r = new zp("html_inline");
             return r._literal = t, e.appendChild(r), !0
         },
-        km = function(e) {
+        xm = function(e) {
             var t, r, n, i, o, s, a, l, u, c, f, h = 0,
                 p = this.pos;
-            if (e === Ud || e === Vd) h++, this.pos++;
+            if (e === Vd || e === zd) h++, this.pos++;
             else
                 for (; this.peek() === e;) h++, this.pos++;
-            return 0 === h ? null : (t = 0 === p ? "\n" : this.subject.charAt(p - 1), r = -1 === (n = this.peek()) ? "\n" : Fd(n), l = am.test(r), u = Zd.test(r), c = am.test(t), f = Zd.test(t), i = !l && (!u || c || f), o = !c && (!f || l || u), 95 === e ? (s = i && (!o || f), a = o && (!i || u)) : e === Ud || e === Vd ? (s = i && !o, a = o) : (s = i, a = o), this.pos = p, {
+            return 0 === h ? null : (t = 0 === p ? "\n" : this.subject.charAt(p - 1), r = -1 === (n = this.peek()) ? "\n" : Md(n), l = lm.test(r), u = Jd.test(r), c = lm.test(t), f = Jd.test(t), i = !l && (!u || c || f), o = !c && (!f || l || u), 95 === e ? (s = i && (!o || f), a = o && (!i || u)) : e === Vd || e === zd ? (s = i && !o, a = o) : (s = i, a = o), this.pos = p, {
                 numdelims: h,
                 can_open: s,
                 can_close: a
             })
         },
-        xm = function(e, t) {
+        Am = function(e, t) {
             var r = this.scanDelims(e);
             if (!r) return !1;
             var n, i = r.numdelims,
                 o = this.pos;
-            this.pos += i, n = e === Ud ? "’" : e === Vd ? "“" : this.subject.slice(o, this.pos);
-            var s = pm(n);
-            return t.appendChild(s), (r.can_open || r.can_close) && (this.options.smart || e !== Ud && e !== Vd) && (this.delimiters = {
+            this.pos += i, n = e === Vd ? "’" : e === zd ? "“" : this.subject.slice(o, this.pos);
+            var s = dm(n);
+            return t.appendChild(s), (r.can_open || r.can_close) && (this.options.smart || e !== Vd && e !== zd) && (this.delimiters = {
                 cc: e,
                 numdelims: i,
                 origdelims: i,
                 node: s,
                 previous: this.delimiters,
                 next: null,
                 can_open: r.can_open,
                 can_close: r.can_close
             }, null !== this.delimiters.previous && (this.delimiters.previous.next = this.delimiters)), !0
         },
-        Am = function(e) {
+        qm = function(e) {
             null !== e.previous && (e.previous.next = e.next), null === e.next ? this.delimiters = e.previous : e.next.previous = e.previous
         },
-        qm = function(e, t) {
+        Em = function(e, t) {
             e.next !== t && (e.next = t, t.previous = e)
         },
-        Em = function(e) {
+        Tm = function(e) {
             for (var t, r, n, i, o, s, a, l, u, c, f, h = [], p = !1, d = 0; d < 8; d++) h[d] = e;
             for (r = this.delimiters; null !== r && r.previous !== e;) r = r.previous;
             for (; null !== r;) {
                 var m = r.cc;
                 if (r.can_close) {
                     switch (t = r.previous, c = !1, m) {
-                        case Ud:
+                        case Vd:
                             f = 0;
                             break;
-                        case Vd:
+                        case zd:
                             f = 1;
                             break;
                         case 95:
                             f = 2;
                             break;
                         case 42:
                             f = 3 + (r.can_open ? 3 : 0) + r.origdelims % 3
@@ -23029,140 +23049,140 @@
                             break
                         }
                         t = t.previous
                     }
                     if (n = r, 42 === m || 95 === m)
                         if (c) {
                             a = r.numdelims >= 2 && t.numdelims >= 2 ? 2 : 1, i = t.node, o = r.node, t.numdelims -= a, r.numdelims -= a, i._literal = i._literal.slice(0, i._literal.length - a), o._literal = o._literal.slice(0, o._literal.length - a);
-                            var g = new Vp(1 === a ? "emph" : "strong");
+                            var g = new zp(1 === a ? "emph" : "strong");
                             for (l = i._next; l && l !== o;) u = l._next, l.unlink(), g.appendChild(l), l = u;
-                            i.insertAfter(g), qm(t, r), 0 === t.numdelims && (i.unlink(), this.removeDelimiter(t)), 0 === r.numdelims && (o.unlink(), s = r.next, this.removeDelimiter(r), r = s)
+                            i.insertAfter(g), Em(t, r), 0 === t.numdelims && (i.unlink(), this.removeDelimiter(t)), 0 === r.numdelims && (o.unlink(), s = r.next, this.removeDelimiter(r), r = s)
                         } else r = r.next;
-                    else m === Ud ? (r.node._literal = "’", c && (t.node._literal = "‘"), r = r.next) : m === Vd && (r.node._literal = "”", c && (t.node.literal = "“"), r = r.next);
+                    else m === Vd ? (r.node._literal = "’", c && (t.node._literal = "‘"), r = r.next) : m === zd && (r.node._literal = "”", c && (t.node.literal = "“"), r = r.next);
                     c || (h[f] = n.previous, n.can_open || this.removeDelimiter(n))
                 } else r = r.next
             }
             for (; null !== this.delimiters && this.delimiters !== e;) this.removeDelimiter(this.delimiters)
         },
-        Tm = function() {
-            var e = this.match(Jd);
-            return null === e ? null : Bd(e.substr(1, e.length - 2))
-        },
         $m = function() {
             var e = this.match(Yd);
+            return null === e ? null : Ud(e.substr(1, e.length - 2))
+        },
+        Om = function() {
+            var e = this.match(Kd);
             if (null === e) {
                 if (60 === this.peek()) return null;
                 for (var t, r = this.pos, n = 0; - 1 !== (t = this.peek());)
-                    if (92 === t && Kd.test(this.subject.charAt(this.pos + 1))) this.pos += 1, -1 !== this.peek() && (this.pos += 1);
+                    if (92 === t && Xd.test(this.subject.charAt(this.pos + 1))) this.pos += 1, -1 !== this.peek() && (this.pos += 1);
                     else if (40 === t) this.pos += 1, n += 1;
                 else if (41 === t) {
                     if (n < 1) break;
                     this.pos += 1, n -= 1
                 } else {
-                    if (null !== sm.exec(Fd(t))) break;
+                    if (null !== am.exec(Md(t))) break;
                     this.pos += 1
                 }
-                return this.pos === r && 41 !== t || 0 !== n ? null : (e = this.subject.substr(r, this.pos - r), jd(Bd(e)))
+                return this.pos === r && 41 !== t || 0 !== n ? null : (e = this.subject.substr(r, this.pos - r), Bd(Ud(e)))
             }
-            return jd(Bd(e.substr(1, e.length - 2)))
+            return Bd(Ud(e.substr(1, e.length - 2)))
         },
-        Om = function() {
-            var e = this.match(fm);
+        Sm = function() {
+            var e = this.match(hm);
             return null === e || e.length > 1001 ? 0 : e.length
         },
-        Sm = function(e) {
+        Dm = function(e) {
             var t = this.pos;
             this.pos += 1;
-            var r = pm("[");
+            var r = dm("[");
             return e.appendChild(r), this.addBracket(r, t, !1), !0
         },
-        Dm = function(e) {
+        Cm = function(e) {
             var t = this.pos;
             if (this.pos += 1, 91 === this.peek()) {
                 this.pos += 1;
-                var r = pm("![");
+                var r = dm("![");
                 e.appendChild(r), this.addBracket(r, t + 1, !0)
-            } else e.appendChild(pm("!"));
+            } else e.appendChild(dm("!"));
             return !0
         },
-        Cm = function(e) {
+        Rm = function(e) {
             var t, r, n, i, o, s, a = !1;
-            if (this.pos += 1, t = this.pos, null === (s = this.brackets)) return e.appendChild(pm("]")), !0;
-            if (!s.active) return e.appendChild(pm("]")), this.removeBracket(), !0;
+            if (this.pos += 1, t = this.pos, null === (s = this.brackets)) return e.appendChild(dm("]")), !0;
+            if (!s.active) return e.appendChild(dm("]")), this.removeBracket(), !0;
             r = s.image;
             var l = this.pos;
-            if (40 === this.peek() && (this.pos++, this.spnl() && null !== (n = this.parseLinkDestination()) && this.spnl() && (sm.test(this.subject.charAt(this.pos - 1)) && (i = this.parseLinkTitle()), 1) && this.spnl() && 41 === this.peek() ? (this.pos += 1, a = !0) : this.pos = l), !a) {
+            if (40 === this.peek() && (this.pos++, this.spnl() && null !== (n = this.parseLinkDestination()) && this.spnl() && (am.test(this.subject.charAt(this.pos - 1)) && (i = this.parseLinkTitle()), 1) && this.spnl() && 41 === this.peek() ? (this.pos += 1, a = !0) : this.pos = l), !a) {
                 var u = this.pos,
                     c = this.parseLinkLabel();
                 if (c > 2 ? o = this.subject.slice(u, u + c) : s.bracketAfter || (o = this.subject.slice(s.index, t)), 0 === c && (this.pos = l), o) {
-                    var f = this.refmap[dm(o)];
+                    var f = this.refmap[mm(o)];
                     f && (n = f.destination, i = f.title, a = !0)
                 }
             }
             if (a) {
-                var h, p, d = new Vp(r ? "image" : "link");
+                var h, p, d = new zp(r ? "image" : "link");
                 for (d._destination = n, d._title = i || "", h = s.node._next; h;) p = h._next, h.unlink(), d.appendChild(h), h = p;
                 if (e.appendChild(d), this.processEmphasis(s.previousDelimiter), this.removeBracket(), s.node.unlink(), !r)
                     for (s = this.brackets; null !== s;) s.image || (s.active = !1), s = s.previous;
                 return !0
             }
-            return this.removeBracket(), this.pos = t, e.appendChild(pm("]")), !0
+            return this.removeBracket(), this.pos = t, e.appendChild(dm("]")), !0
         },
-        Rm = function(e, t, r) {
+        Lm = function(e, t, r) {
             null !== this.brackets && (this.brackets.bracketAfter = !0), this.brackets = {
                 node: e,
                 previous: this.brackets,
                 previousDelimiter: this.delimiters,
                 index: t,
                 image: r,
                 active: !0
             }
         },
-        Lm = function() {
+        Nm = function() {
             this.brackets = this.brackets.previous
         },
-        Nm = function(e) {
+        Im = function(e) {
             var t;
-            return !!(t = this.match(Xd)) && (e.appendChild(pm(Jp.decodeHTML(t))), !0)
+            return !!(t = this.match(Qd)) && (e.appendChild(dm(Yp.decodeHTML(t))), !0)
         },
-        Im = function(e) {
+        Fm = function(e) {
             var t;
-            return !!(t = this.match(hm)) && (this.options.smart ? e.appendChild(pm(t.replace(tm, "…").replace(rm, (function(e) {
+            return !!(t = this.match(pm)) && (this.options.smart ? e.appendChild(dm(t.replace(rm, "…").replace(nm, (function(e) {
                 var t = 0,
                     r = 0;
                 return e.length % 3 == 0 ? r = e.length / 3 : e.length % 2 == 0 ? t = e.length / 2 : e.length % 3 == 2 ? (t = 1, r = (e.length - 2) / 3) : (t = 2, r = (e.length - 4) / 3), "—".repeat(r) + "–".repeat(t)
-            })))) : e.appendChild(pm(t)), !0)
+            })))) : e.appendChild(dm(t)), !0)
         },
-        Fm = function(e) {
+        Mm = function(e) {
             this.pos += 1;
             var t = e._lastChild;
             if (t && "text" === t.type && " " === t._literal[t._literal.length - 1]) {
                 var r = " " === t._literal[t._literal.length - 2];
-                t._literal = t._literal.replace(lm, ""), e.appendChild(new Vp(r ? "linebreak" : "softbreak"))
-            } else e.appendChild(new Vp("softbreak"));
-            return this.match(um), !0
+                t._literal = t._literal.replace(um, ""), e.appendChild(new zp(r ? "linebreak" : "softbreak"))
+            } else e.appendChild(new zp("softbreak"));
+            return this.match(cm), !0
         },
-        Mm = function(e, t) {
+        Pm = function(e, t) {
             var r, n, i, o;
             this.subject = e, this.pos = 0;
             var s = this.pos;
             if (0 === (o = this.parseLinkLabel())) return 0;
             if (r = this.subject.substr(0, o), 58 !== this.peek()) return this.pos = s, 0;
             if (this.pos++, this.spnl(), null === (n = this.parseLinkDestination())) return this.pos = s, 0;
             var a = this.pos;
             this.spnl(), this.pos !== a && (i = this.parseLinkTitle()), null === i && (i = "", this.pos = a);
             var l = !0;
-            if (null === this.match(cm) && ("" === i ? l = !1 : (i = "", this.pos = a, l = null !== this.match(cm))), !l) return this.pos = s, 0;
-            var u = dm(r);
+            if (null === this.match(fm) && ("" === i ? l = !1 : (i = "", this.pos = a, l = null !== this.match(fm))), !l) return this.pos = s, 0;
+            var u = mm(r);
             return "" === u ? (this.pos = s, 0) : (t[u] || (t[u] = {
                 destination: n,
                 title: i
             }), this.pos - s)
         },
-        Pm = function(e) {
+        jm = function(e) {
             var t = !1,
                 r = this.peek();
             if (-1 === r) return !1;
             switch (r) {
                 case 10:
                     t = this.parseNewline(e);
                     break;
@@ -23172,16 +23192,16 @@
                 case 96:
                     t = this.parseBackticks(e);
                     break;
                 case 42:
                 case 95:
                     t = this.handleDelim(r, e);
                     break;
-                case Ud:
                 case Vd:
+                case zd:
                     t = this.options.smart && this.handleDelim(r, e);
                     break;
                 case 91:
                     t = this.parseOpenBracket(e);
                     break;
                 case 33:
                     t = this.parseBang(e);
@@ -23194,113 +23214,113 @@
                     break;
                 case 38:
                     t = this.parseEntity(e);
                     break;
                 default:
                     t = this.parseString(e)
             }
-            return t || (this.pos += 1, e.appendChild(pm(Fd(r)))), !0
+            return t || (this.pos += 1, e.appendChild(dm(Md(r)))), !0
         },
-        jm = function(e) {
+        Bm = function(e) {
             for (this.subject = e._string_content.trim(), this.pos = 0, this.delimiters = null, this.brackets = null; this.parseInline(e););
             e._string_content = null, this.processEmphasis(null)
         };
 
-    function Bm(e) {
+    function Um(e) {
         return {
             subject: "",
             delimiters: null,
             brackets: null,
             pos: 0,
             refmap: {},
-            match: mm,
-            peek: gm,
-            spnl: vm,
-            parseBackticks: ym,
-            parseBackslash: bm,
-            parseAutolink: wm,
-            parseHtmlTag: _m,
-            scanDelims: km,
-            handleDelim: xm,
-            parseLinkTitle: Tm,
-            parseLinkDestination: $m,
-            parseLinkLabel: Om,
-            parseOpenBracket: Sm,
-            parseBang: Dm,
-            parseCloseBracket: Cm,
-            addBracket: Rm,
-            removeBracket: Lm,
-            parseEntity: Nm,
-            parseString: Im,
-            parseNewline: Fm,
-            parseReference: Mm,
-            parseInline: Pm,
-            processEmphasis: Em,
-            removeDelimiter: Am,
+            match: gm,
+            peek: vm,
+            spnl: ym,
+            parseBackticks: bm,
+            parseBackslash: wm,
+            parseAutolink: _m,
+            parseHtmlTag: km,
+            scanDelims: xm,
+            handleDelim: Am,
+            parseLinkTitle: $m,
+            parseLinkDestination: Om,
+            parseLinkLabel: Sm,
+            parseOpenBracket: Dm,
+            parseBang: Cm,
+            parseCloseBracket: Rm,
+            addBracket: Lm,
+            removeBracket: Nm,
+            parseEntity: Im,
+            parseString: Fm,
+            parseNewline: Mm,
+            parseReference: Pm,
+            parseInline: jm,
+            processEmphasis: Tm,
+            removeDelimiter: qm,
             options: e || {},
-            parse: jm
+            parse: Bm
         }
     }
-    var Um = [/./, /^<(?:script|pre|textarea|style)(?:\s|>|$)/i, /^<!--/, /^<[?]/, /^<![A-Z]/, /^<!\[CDATA\[/, /^<[/]?(?:address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[123456]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul)(?:\s|[/]?[>]|$)/i, new RegExp("^(?:" + Ed + "|" + Td + ")\\s*$", "i")],
-        Vm = [/./, /<\/(?:script|pre|textarea|style)>/i, /-->/, /\?>/, />/, /\]\]>/],
-        zm = /^(?:\*[ \t]*){3,}$|^(?:_[ \t]*){3,}$|^(?:-[ \t]*){3,}$/,
-        Hm = /^[#`~*+_=<>0-9-]/,
-        Wm = /[^ \t\f\v\r\n]/,
-        Gm = /^[*+-]/,
-        Zm = /^(\d{1,9})([.)])/,
-        Jm = /^#{1,6}(?:[ \t]+|$)/,
-        Ym = /^`{3,}(?!.*`)|^~{3,}/,
-        Km = /^(?:`{3,}|~{3,})(?= *$)/,
-        Xm = /^(?:=+|-+)[ \t]*$/,
-        Qm = /\r\n|\n|\r/,
-        eg = function(e) {
+    var Vm = [/./, /^<(?:script|pre|textarea|style)(?:\s|>|$)/i, /^<!--/, /^<[?]/, /^<![A-Z]/, /^<!\[CDATA\[/, /^<[/]?(?:address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[123456]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul)(?:\s|[/]?[>]|$)/i, new RegExp("^(?:" + Td + "|" + $d + ")\\s*$", "i")],
+        zm = [/./, /<\/(?:script|pre|textarea|style)>/i, /-->/, /\?>/, />/, /\]\]>/],
+        Hm = /^(?:\*[ \t]*){3,}$|^(?:_[ \t]*){3,}$|^(?:-[ \t]*){3,}$/,
+        Wm = /^[#`~*+_=<>0-9-]/,
+        Gm = /[^ \t\f\v\r\n]/,
+        Zm = /^[*+-]/,
+        Jm = /^(\d{1,9})([.)])/,
+        Ym = /^#{1,6}(?:[ \t]+|$)/,
+        Km = /^`{3,}(?!.*`)|^~{3,}/,
+        Xm = /^(?:`{3,}|~{3,})(?= *$)/,
+        Qm = /^(?:=+|-+)[ \t]*$/,
+        eg = /\r\n|\n|\r/,
+        tg = function(e) {
             return 32 === e || 9 === e
         },
-        tg = function(e, t) {
+        rg = function(e, t) {
             return t < e.length ? e.charCodeAt(t) : -1
         },
-        rg = function(e) {
+        ng = function(e) {
             for (; e;) {
                 if (e._lastLineBlank) return !0;
                 var t = e.type;
                 if (e._lastLineChecked || "list" !== t && "item" !== t) {
                     e._lastLineChecked = !0;
                     break
                 }
                 e._lastLineChecked = !0, e = e._lastChild
             }
             return !1
         },
-        ng = function() {
+        ig = function() {
             if (this.partiallyConsumedTab) {
                 this.offset += 1;
                 var e = 4 - this.column % 4;
                 this.tip._string_content += " ".repeat(e)
             }
             this.tip._string_content += this.currentLine.slice(this.offset) + "\n"
         },
-        ig = function(e, t) {
+        og = function(e, t) {
             for (; !this.blocks[this.tip.type].canContain(e);) this.finalize(this.tip, this.lineNumber - 1);
             var r = t + 1,
-                n = new Vp(e, [
+                n = new zp(e, [
                     [this.lineNumber, r],
                     [0, 0]
                 ]);
             return n._string_content = "", this.tip.appendChild(n), this.tip = n, n
         },
-        og = function() {
+        sg = function() {
             if (!this.allClosed) {
                 for (; this.oldtip !== this.lastMatchedContainer;) {
                     var e = this.oldtip._parent;
                     this.finalize(this.oldtip, this.lineNumber - 1), this.oldtip = e
                 }
                 this.allClosed = !0
             }
         },
-        sg = {
+        ag = {
             document: {
                 continue: function() {
                     return 0
                 },
                 finalize: function() {},
                 canContain: function(e) {
                     return "item" !== e
@@ -23309,20 +23329,20 @@
             },
             list: {
                 continue: function() {
                     return 0
                 },
                 finalize: function(e, t) {
                     for (var r = t._firstChild; r;) {
-                        if (rg(r) && r._next) {
+                        if (ng(r) && r._next) {
                             t._listData.tight = !1;
                             break
                         }
                         for (var n = r._firstChild; n;) {
-                            if (rg(n) && (r._next || n._next)) {
+                            if (ng(n) && (r._next || n._next)) {
                                 t._listData.tight = !1;
                                 break
                             }
                             n = n._next
                         }
                         r = r._next
                     }
@@ -23331,15 +23351,15 @@
                     return "item" === e
                 },
                 acceptsLines: !1
             },
             block_quote: {
                 continue: function(e) {
                     var t = e.currentLine;
-                    return e.indented || 62 !== tg(t, e.nextNonspace) ? 1 : (e.advanceNextNonspace(), e.advanceOffset(1, !1), eg(tg(t, e.offset)) && e.advanceOffset(1, !0), 0)
+                    return e.indented || 62 !== rg(t, e.nextNonspace) ? 1 : (e.advanceNextNonspace(), e.advanceOffset(1, !1), tg(rg(t, e.offset)) && e.advanceOffset(1, !0), 0)
                 },
                 finalize: function() {},
                 canContain: function(e) {
                     return "item" !== e
                 },
                 acceptsLines: !1
             },
@@ -23381,31 +23401,31 @@
                 acceptsLines: !1
             },
             code_block: {
                 continue: function(e, t) {
                     var r = e.currentLine,
                         n = e.indent;
                     if (t._isFenced) {
-                        var i = n <= 3 && r.charAt(e.nextNonspace) === t._fenceChar && r.slice(e.nextNonspace).match(Km);
+                        var i = n <= 3 && r.charAt(e.nextNonspace) === t._fenceChar && r.slice(e.nextNonspace).match(Xm);
                         if (i && i[0].length >= t._fenceLength) return e.lastLineLength = e.offset + n + i[0].length, e.finalize(t, e.lineNumber), 2;
-                        for (var o = t._fenceOffset; o > 0 && eg(tg(r, e.offset));) e.advanceOffset(1, !0), o--
+                        for (var o = t._fenceOffset; o > 0 && tg(rg(r, e.offset));) e.advanceOffset(1, !0), o--
                     } else if (n >= 4) e.advanceOffset(4, !0);
                     else {
                         if (!e.blank) return 1;
                         e.advanceNextNonspace()
                     }
                     return 0
                 },
                 finalize: function(e, t) {
                     if (t._isFenced) {
                         var r = t._string_content,
                             n = r.indexOf("\n"),
                             i = r.slice(0, n),
                             o = r.slice(n + 1);
-                        t.info = Ld(i.trim()), t._literal = o
+                        t.info = Nd(i.trim()), t._literal = o
                     } else t._literal = t._string_content.replace(/(\n *)+$/, "\n");
                     t._string_content = null
                 },
                 canContain: function() {
                     return !1
                 },
                 acceptsLines: !0
@@ -23423,114 +23443,114 @@
                 acceptsLines: !0
             },
             paragraph: {
                 continue: function(e) {
                     return e.blank ? 1 : 0
                 },
                 finalize: function(e, t) {
-                    for (var r, n = !1; 91 === tg(t._string_content, 0) && (r = e.inlineParser.parseReference(t._string_content, e.refmap));) t._string_content = t._string_content.slice(r), n = !0;
+                    for (var r, n = !1; 91 === rg(t._string_content, 0) && (r = e.inlineParser.parseReference(t._string_content, e.refmap));) t._string_content = t._string_content.slice(r), n = !0;
                     n && function(e) {
-                        return !Wm.test(e)
+                        return !Gm.test(e)
                     }(t._string_content) && t.unlink()
                 },
                 canContain: function() {
                     return !1
                 },
                 acceptsLines: !0
             }
         },
-        ag = [function(e) {
-            return e.indented || 62 !== tg(e.currentLine, e.nextNonspace) ? 0 : (e.advanceNextNonspace(), e.advanceOffset(1, !1), eg(tg(e.currentLine, e.offset)) && e.advanceOffset(1, !0), e.closeUnmatchedBlocks(), e.addChild("block_quote", e.nextNonspace), 1)
+        lg = [function(e) {
+            return e.indented || 62 !== rg(e.currentLine, e.nextNonspace) ? 0 : (e.advanceNextNonspace(), e.advanceOffset(1, !1), tg(rg(e.currentLine, e.offset)) && e.advanceOffset(1, !0), e.closeUnmatchedBlocks(), e.addChild("block_quote", e.nextNonspace), 1)
         }, function(e) {
             var t;
-            if (!e.indented && (t = e.currentLine.slice(e.nextNonspace).match(Jm))) {
+            if (!e.indented && (t = e.currentLine.slice(e.nextNonspace).match(Ym))) {
                 e.advanceNextNonspace(), e.advanceOffset(t[0].length, !1), e.closeUnmatchedBlocks();
                 var r = e.addChild("heading", e.nextNonspace);
                 return r.level = t[0].trim().length, r._string_content = e.currentLine.slice(e.offset).replace(/^[ \t]*#+[ \t]*$/, "").replace(/[ \t]+#+[ \t]*$/, ""), e.advanceOffset(e.currentLine.length - e.offset), 2
             }
             return 0
         }, function(e) {
             var t;
-            if (!e.indented && (t = e.currentLine.slice(e.nextNonspace).match(Ym))) {
+            if (!e.indented && (t = e.currentLine.slice(e.nextNonspace).match(Km))) {
                 var r = t[0].length;
                 e.closeUnmatchedBlocks();
                 var n = e.addChild("code_block", e.nextNonspace);
                 return n._isFenced = !0, n._fenceLength = r, n._fenceChar = t[0][0], n._fenceOffset = e.indent, e.advanceNextNonspace(), e.advanceOffset(r, !1), 2
             }
             return 0
         }, function(e, t) {
-            if (!e.indented && 60 === tg(e.currentLine, e.nextNonspace)) {
+            if (!e.indented && 60 === rg(e.currentLine, e.nextNonspace)) {
                 var r, n = e.currentLine.slice(e.nextNonspace);
                 for (r = 1; r <= 7; r++) {
-                    if (Um[r].test(n) && (r < 7 || "paragraph" !== t.type && (e.allClosed || e.blank || "paragraph" !== e.tip.type))) return e.closeUnmatchedBlocks(), e.addChild("html_block", e.offset)._htmlBlockType = r, 2
+                    if (Vm[r].test(n) && (r < 7 || "paragraph" !== t.type && (e.allClosed || e.blank || "paragraph" !== e.tip.type))) return e.closeUnmatchedBlocks(), e.addChild("html_block", e.offset)._htmlBlockType = r, 2
                 }
             }
             return 0
         }, function(e, t) {
             var r;
-            if (!e.indented && "paragraph" === t.type && (r = e.currentLine.slice(e.nextNonspace).match(Xm))) {
+            if (!e.indented && "paragraph" === t.type && (r = e.currentLine.slice(e.nextNonspace).match(Qm))) {
                 var n;
-                for (e.closeUnmatchedBlocks(); 91 === tg(t._string_content, 0) && (n = e.inlineParser.parseReference(t._string_content, e.refmap));) t._string_content = t._string_content.slice(n);
+                for (e.closeUnmatchedBlocks(); 91 === rg(t._string_content, 0) && (n = e.inlineParser.parseReference(t._string_content, e.refmap));) t._string_content = t._string_content.slice(n);
                 if (t._string_content.length > 0) {
-                    var i = new Vp("heading", t.sourcepos);
+                    var i = new zp("heading", t.sourcepos);
                     return i.level = "=" === r[0][0] ? 1 : 2, i._string_content = t._string_content, t.insertAfter(i), t.unlink(), e.tip = i, e.advanceOffset(e.currentLine.length - e.offset, !1), 2
                 }
                 return 0
             }
             return 0
         }, function(e) {
-            return !e.indented && zm.test(e.currentLine.slice(e.nextNonspace)) ? (e.closeUnmatchedBlocks(), e.addChild("thematic_break", e.nextNonspace), e.advanceOffset(e.currentLine.length - e.offset, !1), 2) : 0
+            return !e.indented && Hm.test(e.currentLine.slice(e.nextNonspace)) ? (e.closeUnmatchedBlocks(), e.addChild("thematic_break", e.nextNonspace), e.advanceOffset(e.currentLine.length - e.offset, !1), 2) : 0
         }, function(e, t) {
             var r, n, i;
             return e.indented && "list" !== t.type || !(r = function(e, t) {
                 var r, n, i, o, s = e.currentLine.slice(e.nextNonspace),
                     a = {
                         type: null,
                         tight: !0,
                         bulletChar: null,
                         start: null,
                         delimiter: null,
                         padding: null,
                         markerOffset: e.indent
                     };
                 if (e.indent >= 4) return null;
-                if (r = s.match(Gm)) a.type = "bullet", a.bulletChar = r[0][0];
+                if (r = s.match(Zm)) a.type = "bullet", a.bulletChar = r[0][0];
                 else {
-                    if (!(r = s.match(Zm)) || "paragraph" === t.type && 1 != r[1]) return null;
+                    if (!(r = s.match(Jm)) || "paragraph" === t.type && 1 != r[1]) return null;
                     a.type = "ordered", a.start = parseInt(r[1]), a.delimiter = r[2]
                 }
-                if (-1 !== (n = tg(e.currentLine, e.nextNonspace + r[0].length)) && 9 !== n && 32 !== n) return null;
-                if ("paragraph" === t.type && !e.currentLine.slice(e.nextNonspace + r[0].length).match(Wm)) return null;
+                if (-1 !== (n = rg(e.currentLine, e.nextNonspace + r[0].length)) && 9 !== n && 32 !== n) return null;
+                if ("paragraph" === t.type && !e.currentLine.slice(e.nextNonspace + r[0].length).match(Gm)) return null;
                 e.advanceNextNonspace(), e.advanceOffset(r[0].length, !0), i = e.column, o = e.offset;
                 do {
-                    e.advanceOffset(1, !0), n = tg(e.currentLine, e.offset)
-                } while (e.column - i < 5 && eg(n));
-                var l = -1 === tg(e.currentLine, e.offset),
+                    e.advanceOffset(1, !0), n = rg(e.currentLine, e.offset)
+                } while (e.column - i < 5 && tg(n));
+                var l = -1 === rg(e.currentLine, e.offset),
                     u = e.column - i;
-                return u >= 5 || u < 1 || l ? (a.padding = r[0].length + 1, e.column = i, e.offset = o, eg(tg(e.currentLine, e.offset)) && e.advanceOffset(1, !0)) : a.padding = r[0].length + u, a
+                return u >= 5 || u < 1 || l ? (a.padding = r[0].length + 1, e.column = i, e.offset = o, tg(rg(e.currentLine, e.offset)) && e.advanceOffset(1, !0)) : a.padding = r[0].length + u, a
             }(e, t)) ? 0 : (e.closeUnmatchedBlocks(), "list" === e.tip.type && (n = t._listData, i = r, n.type === i.type && n.delimiter === i.delimiter && n.bulletChar === i.bulletChar) || ((t = e.addChild("list", e.nextNonspace))._listData = r), (t = e.addChild("item", e.nextNonspace))._listData = r, 1)
         }, function(e) {
             return e.indented && "paragraph" !== e.tip.type && !e.blank ? (e.advanceOffset(4, !0), e.closeUnmatchedBlocks(), e.addChild("code_block", e.offset), 2) : 0
         }],
-        lg = function(e, t) {
+        ug = function(e, t) {
             for (var r, n, i, o = this.currentLine; e > 0 && (i = o[this.offset]);) "\t" === i ? (r = 4 - this.column % 4, t ? (this.partiallyConsumedTab = r > e, n = r > e ? e : r, this.column += n, this.offset += this.partiallyConsumedTab ? 0 : 1, e -= n) : (this.partiallyConsumedTab = !1, this.column += r, this.offset += 1, e -= 1)) : (this.partiallyConsumedTab = !1, this.offset += 1, this.column += 1, e -= 1)
         },
-        ug = function() {
+        cg = function() {
             this.offset = this.nextNonspace, this.column = this.nextNonspaceColumn, this.partiallyConsumedTab = !1
         },
-        cg = function() {
+        fg = function() {
             for (var e, t = this.currentLine, r = this.offset, n = this.column;
                 "" !== (e = t.charAt(r));)
                 if (" " === e) r++, n++;
                 else {
                     if ("\t" !== e) break;
                     r++, n += 4 - n % 4
                 } this.blank = "\n" === e || "\r" === e || "" === e, this.nextNonspace = r, this.nextNonspaceColumn = n, this.indent = this.nextNonspaceColumn - this.column, this.indented = this.indent >= 4
         },
-        fg = function(e) {
+        hg = function(e) {
             var t, r, n = !0,
                 i = this.doc;
             for (this.oldtip = this.tip, this.offset = 0, this.column = 0, this.blank = !1, this.partiallyConsumedTab = !1, this.lineNumber += 1, -1 !== e.indexOf("\0") && (e = e.replace(/\0/g, "�")), this.currentLine = e;
                 (r = i._lastChild) && r._open;) {
                 switch (i = r, this.findNextNonspace(), this.blocks[i.type].continue(this, i)) {
                     case 0:
                         break;
@@ -23544,16 +23564,16 @@
                 }
                 if (!n) {
                     i = i._parent;
                     break
                 }
             }
             this.allClosed = i === this.oldtip, this.lastMatchedContainer = i;
-            for (var o = "paragraph" !== i.type && sg[i.type].acceptsLines, s = this.blockStarts, a = s.length; !o;) {
-                if (this.findNextNonspace(), !this.indented && !Hm.test(e.slice(this.nextNonspace))) {
+            for (var o = "paragraph" !== i.type && ag[i.type].acceptsLines, s = this.blockStarts, a = s.length; !o;) {
+                if (this.findNextNonspace(), !this.indented && !Wm.test(e.slice(this.nextNonspace))) {
                     this.advanceNextNonspace();
                     break
                 }
                 for (var l = 0; l < a;) {
                     var u = s[l](this, i);
                     if (1 === u) {
                         i = this.tip;
@@ -23569,47 +23589,47 @@
                     this.advanceNextNonspace();
                     break
                 }
             }
             if (this.allClosed || this.blank || "paragraph" !== this.tip.type) {
                 this.closeUnmatchedBlocks(), this.blank && i.lastChild && (i.lastChild._lastLineBlank = !0), t = i.type;
                 for (var c = this.blank && !("block_quote" === t || "code_block" === t && i._isFenced || "item" === t && !i._firstChild && i.sourcepos[0][0] === this.lineNumber), f = i; f;) f._lastLineBlank = c, f = f._parent;
-                this.blocks[t].acceptsLines ? (this.addLine(), "html_block" === t && i._htmlBlockType >= 1 && i._htmlBlockType <= 5 && Vm[i._htmlBlockType].test(this.currentLine.slice(this.offset)) && (this.lastLineLength = e.length, this.finalize(i, this.lineNumber))) : this.offset < e.length && !this.blank && (i = this.addChild("paragraph", this.offset), this.advanceNextNonspace(), this.addLine())
+                this.blocks[t].acceptsLines ? (this.addLine(), "html_block" === t && i._htmlBlockType >= 1 && i._htmlBlockType <= 5 && zm[i._htmlBlockType].test(this.currentLine.slice(this.offset)) && (this.lastLineLength = e.length, this.finalize(i, this.lineNumber))) : this.offset < e.length && !this.blank && (i = this.addChild("paragraph", this.offset), this.advanceNextNonspace(), this.addLine())
             } else this.addLine();
             this.lastLineLength = e.length
         },
-        hg = function(e, t) {
+        pg = function(e, t) {
             var r = e._parent;
             e._open = !1, e.sourcepos[1] = [t, this.lastLineLength], this.blocks[e.type].finalize(this, e), this.tip = r
         },
-        pg = function(e) {
+        dg = function(e) {
             var t, r, n, i = e.walker();
             for (this.inlineParser.refmap = this.refmap, this.inlineParser.options = this.options; r = i.next();) n = (t = r.node).type, r.entering || "paragraph" !== n && "heading" !== n || this.inlineParser.parse(t)
         },
-        dg = function() {
-            return new Vp("document", [
+        mg = function() {
+            return new zp("document", [
                 [1, 1],
                 [0, 0]
             ])
         },
-        mg = function(e) {
-            this.doc = new dg, this.tip = this.doc, this.refmap = {}, this.lineNumber = 0, this.lastLineLength = 0, this.offset = 0, this.column = 0, this.lastMatchedContainer = this.doc, this.currentLine = "", this.options.time && console.time("preparing input");
-            var t = e.split(Qm),
+        gg = function(e) {
+            this.doc = new mg, this.tip = this.doc, this.refmap = {}, this.lineNumber = 0, this.lastLineLength = 0, this.offset = 0, this.column = 0, this.lastMatchedContainer = this.doc, this.currentLine = "", this.options.time && console.time("preparing input");
+            var t = e.split(eg),
                 r = t.length;
             10 === e.charCodeAt(e.length - 1) && (r -= 1), this.options.time && console.timeEnd("preparing input"), this.options.time && console.time("block parsing");
             for (var n = 0; n < r; n++) this.incorporateLine(t[n]);
             for (; this.tip;) this.finalize(this.tip, r);
             return this.options.time && console.timeEnd("block parsing"), this.options.time && console.time("inline parsing"), this.processInlines(this.doc), this.options.time && console.timeEnd("inline parsing"), this.doc
         };
 
-    function gg(e) {
+    function vg(e) {
         return {
-            doc: new dg,
-            blocks: sg,
-            blockStarts: ag,
+            doc: new mg,
+            blocks: ag,
+            blockStarts: lg,
             tip: this.doc,
             oldtip: this.doc,
             currentLine: "",
             lineNumber: 0,
             offset: 0,
             column: 0,
             nextNonspace: 0,
@@ -23618,137 +23638,137 @@
             indented: !1,
             blank: !1,
             partiallyConsumedTab: !1,
             allClosed: !0,
             lastMatchedContainer: this.doc,
             refmap: {},
             lastLineLength: 0,
-            inlineParser: new Bm(e),
-            findNextNonspace: cg,
-            advanceOffset: lg,
-            advanceNextNonspace: ug,
-            addLine: ng,
-            addChild: ig,
-            incorporateLine: fg,
-            finalize: hg,
-            processInlines: pg,
-            closeUnmatchedBlocks: og,
-            parse: mg,
+            inlineParser: new Um(e),
+            findNextNonspace: fg,
+            advanceOffset: ug,
+            advanceNextNonspace: cg,
+            addLine: ig,
+            addChild: og,
+            incorporateLine: hg,
+            finalize: pg,
+            processInlines: dg,
+            closeUnmatchedBlocks: sg,
+            parse: gg,
             options: e || {}
         }
     }
 
-    function vg() {}
-    vg.prototype.render = function(e) {
+    function yg() {}
+    yg.prototype.render = function(e) {
         var t, r, n = e.walker();
         for (this.buffer = "", this.lastOut = "\n"; t = n.next();) this[r = t.node.type] && this[r](t.node, t.entering);
         return this.buffer
-    }, vg.prototype.out = function(e) {
+    }, yg.prototype.out = function(e) {
         this.lit(e)
-    }, vg.prototype.lit = function(e) {
+    }, yg.prototype.lit = function(e) {
         this.buffer += e, this.lastOut = e
-    }, vg.prototype.cr = function() {
+    }, yg.prototype.cr = function() {
         "\n" !== this.lastOut && this.lit("\n")
-    }, vg.prototype.esc = function(e) {
+    }, yg.prototype.esc = function(e) {
         return e
     };
-    var yg = /^javascript:|vbscript:|file:|data:/i,
-        bg = /^data:image\/(?:png|gif|jpeg|webp)/i,
-        wg = function(e) {
-            return yg.test(e) && !bg.test(e)
+    var bg = /^javascript:|vbscript:|file:|data:/i,
+        wg = /^data:image\/(?:png|gif|jpeg|webp)/i,
+        _g = function(e) {
+            return bg.test(e) && !wg.test(e)
         };
 
-    function _g(e) {
-        (e = e || {}).softbreak = e.softbreak || "\n", this.esc = e.esc || Id, this.disableTags = 0, this.lastOut = "\n", this.options = e
+    function kg(e) {
+        (e = e || {}).softbreak = e.softbreak || "\n", this.esc = e.esc || Fd, this.disableTags = 0, this.lastOut = "\n", this.options = e
     }
-    _g.prototype = Object.create(vg.prototype), _g.prototype.text = function(e) {
+    kg.prototype = Object.create(yg.prototype), kg.prototype.text = function(e) {
         this.out(e.literal)
-    }, _g.prototype.html_inline = function(e) {
+    }, kg.prototype.html_inline = function(e) {
         this.options.safe ? this.lit("\x3c!-- raw HTML omitted --\x3e") : this.lit(e.literal)
-    }, _g.prototype.html_block = function(e) {
+    }, kg.prototype.html_block = function(e) {
         this.cr(), this.options.safe ? this.lit("\x3c!-- raw HTML omitted --\x3e") : this.lit(e.literal), this.cr()
-    }, _g.prototype.softbreak = function() {
+    }, kg.prototype.softbreak = function() {
         this.lit(this.options.softbreak)
-    }, _g.prototype.linebreak = function() {
+    }, kg.prototype.linebreak = function() {
         this.tag("br", [], !0), this.cr()
-    }, _g.prototype.link = function(e, t) {
+    }, kg.prototype.link = function(e, t) {
         var r = this.attrs(e);
-        t ? (this.options.safe && wg(e.destination) || r.push(["href", this.esc(e.destination)]), e.title && r.push(["title", this.esc(e.title)]), this.tag("a", r)) : this.tag("/a")
-    }, _g.prototype.image = function(e, t) {
-        t ? (0 === this.disableTags && (this.options.safe && wg(e.destination) ? this.lit('<img src="" alt="') : this.lit('<img src="' + this.esc(e.destination) + '" alt="')), this.disableTags += 1) : (this.disableTags -= 1, 0 === this.disableTags && (e.title && this.lit('" title="' + this.esc(e.title)), this.lit('" />')))
-    }, _g.prototype.emph = function(e, t) {
+        t ? (this.options.safe && _g(e.destination) || r.push(["href", this.esc(e.destination)]), e.title && r.push(["title", this.esc(e.title)]), this.tag("a", r)) : this.tag("/a")
+    }, kg.prototype.image = function(e, t) {
+        t ? (0 === this.disableTags && (this.options.safe && _g(e.destination) ? this.lit('<img src="" alt="') : this.lit('<img src="' + this.esc(e.destination) + '" alt="')), this.disableTags += 1) : (this.disableTags -= 1, 0 === this.disableTags && (e.title && this.lit('" title="' + this.esc(e.title)), this.lit('" />')))
+    }, kg.prototype.emph = function(e, t) {
         this.tag(t ? "em" : "/em")
-    }, _g.prototype.strong = function(e, t) {
+    }, kg.prototype.strong = function(e, t) {
         this.tag(t ? "strong" : "/strong")
-    }, _g.prototype.paragraph = function(e, t) {
+    }, kg.prototype.paragraph = function(e, t) {
         var r = e.parent.parent,
             n = this.attrs(e);
         null !== r && "list" === r.type && r.listTight || (t ? (this.cr(), this.tag("p", n)) : (this.tag("/p"), this.cr()))
-    }, _g.prototype.heading = function(e, t) {
+    }, kg.prototype.heading = function(e, t) {
         var r = "h" + e.level,
             n = this.attrs(e);
         t ? (this.cr(), this.tag(r, n)) : (this.tag("/" + r), this.cr())
-    }, _g.prototype.code = function(e) {
+    }, kg.prototype.code = function(e) {
         this.tag("code"), this.out(e.literal), this.tag("/code")
-    }, _g.prototype.code_block = function(e) {
+    }, kg.prototype.code_block = function(e) {
         var t = e.info ? e.info.split(/\s+/) : [],
             r = this.attrs(e);
         t.length > 0 && t[0].length > 0 && r.push(["class", "language-" + this.esc(t[0])]), this.cr(), this.tag("pre"), this.tag("code", r), this.out(e.literal), this.tag("/code"), this.tag("/pre"), this.cr()
-    }, _g.prototype.thematic_break = function(e) {
+    }, kg.prototype.thematic_break = function(e) {
         var t = this.attrs(e);
         this.cr(), this.tag("hr", t, !0), this.cr()
-    }, _g.prototype.block_quote = function(e, t) {
+    }, kg.prototype.block_quote = function(e, t) {
         var r = this.attrs(e);
         t ? (this.cr(), this.tag("blockquote", r), this.cr()) : (this.cr(), this.tag("/blockquote"), this.cr())
-    }, _g.prototype.list = function(e, t) {
+    }, kg.prototype.list = function(e, t) {
         var r = "bullet" === e.listType ? "ul" : "ol",
             n = this.attrs(e);
         if (t) {
             var i = e.listStart;
             null !== i && 1 !== i && n.push(["start", i.toString()]), this.cr(), this.tag(r, n), this.cr()
         } else this.cr(), this.tag("/" + r), this.cr()
-    }, _g.prototype.item = function(e, t) {
+    }, kg.prototype.item = function(e, t) {
         var r = this.attrs(e);
         t ? this.tag("li", r) : (this.tag("/li"), this.cr())
-    }, _g.prototype.custom_inline = function(e, t) {
+    }, kg.prototype.custom_inline = function(e, t) {
         t && e.onEnter ? this.lit(e.onEnter) : !t && e.onExit && this.lit(e.onExit)
-    }, _g.prototype.custom_block = function(e, t) {
+    }, kg.prototype.custom_block = function(e, t) {
         this.cr(), t && e.onEnter ? this.lit(e.onEnter) : !t && e.onExit && this.lit(e.onExit), this.cr()
-    }, _g.prototype.esc = Id, _g.prototype.out = function(e) {
+    }, kg.prototype.esc = Fd, kg.prototype.out = function(e) {
         this.lit(this.esc(e))
-    }, _g.prototype.tag = function(e, t, r) {
+    }, kg.prototype.tag = function(e, t, r) {
         if (!(this.disableTags > 0)) {
             if (this.buffer += "<" + e, t && t.length > 0)
                 for (var n, i = 0; void 0 !== (n = t[i]);) this.buffer += " " + n[0] + '="' + n[1] + '"', i++;
             r && (this.buffer += " /"), this.buffer += ">", this.lastOut = ">"
         }
-    }, _g.prototype.attrs = function(e) {
+    }, kg.prototype.attrs = function(e) {
         var t = [];
         if (this.options.sourcepos) {
             var r = e.sourcepos;
             r && t.push(["data-sourcepos", String(r[0][0]) + ":" + String(r[0][1]) + "-" + String(r[1][0]) + ":" + String(r[1][1])])
         }
         return t
     };
-    var kg = /\<[^>]*\>/;
+    var xg = /\<[^>]*\>/;
 
-    function xg(e) {
+    function Ag(e) {
         return e.replace(/([a-z])([A-Z])/g, "$1_$2").toLowerCase()
     }
 
-    function Ag(e) {
-        e = e || {}, this.disableTags = 0, this.lastOut = "\n", this.indentLevel = 0, this.indent = "  ", this.esc = e.esc || Id, this.options = e
+    function qg(e) {
+        e = e || {}, this.disableTags = 0, this.lastOut = "\n", this.indentLevel = 0, this.indent = "  ", this.esc = e.esc || Fd, this.options = e
     }
-    Ag.prototype = Object.create(vg.prototype), Ag.prototype.render = function(e) {
+    qg.prototype = Object.create(yg.prototype), qg.prototype.render = function(e) {
         var t, r;
         this.buffer = "";
         var n, i, o, s, a, l, u = e.walker(),
             c = this.options;
         for (c.time && console.time("rendering"), this.buffer += '<?xml version="1.0" encoding="UTF-8"?>\n', this.buffer += '<!DOCTYPE document SYSTEM "CommonMark.dtd">\n'; n = u.next();)
-            if (o = n.entering, l = (i = n.node).type, s = i.isContainer, a = "thematic_break" === l || "linebreak" === l || "softbreak" === l, r = xg(l), o) {
+            if (o = n.entering, l = (i = n.node).type, s = i.isContainer, a = "thematic_break" === l || "linebreak" === l || "softbreak" === l, r = Ag(l), o) {
                 switch (t = [], l) {
                     case "document":
                         t.push(["xmlns", "http://commonmark.org/xml/1.0"]);
                         break;
                     case "list":
                         null !== i.listType && t.push(["type", i.listType.toLowerCase()]), null !== i.listStart && t.push(["start", String(i.listStart)]), null !== i.listTight && t.push(["tight", i.listTight ? "true" : "false"]);
                         var f = i.listDelimiter;
@@ -23778,47 +23798,47 @@
                 if (this.cr(), this.out(this.tag(r, t, a)), s) this.indentLevel += 1;
                 else if (!s && !a) {
                     var d = i.literal;
                     d && this.out(this.esc(d)), this.out(this.tag("/" + r))
                 }
             } else this.indentLevel -= 1, this.cr(), this.out(this.tag("/" + r));
         return c.time && console.timeEnd("rendering"), this.buffer += "\n", this.buffer
-    }, Ag.prototype.out = function(e) {
-        this.disableTags > 0 ? this.buffer += e.replace(kg, "") : this.buffer += e, this.lastOut = e
-    }, Ag.prototype.cr = function() {
+    }, qg.prototype.out = function(e) {
+        this.disableTags > 0 ? this.buffer += e.replace(xg, "") : this.buffer += e, this.lastOut = e
+    }, qg.prototype.cr = function() {
         if ("\n" !== this.lastOut) {
             this.buffer += "\n", this.lastOut = "\n";
             for (var e = this.indentLevel; e > 0; e--) this.buffer += this.indent
         }
-    }, Ag.prototype.tag = function(e, t, r) {
+    }, qg.prototype.tag = function(e, t, r) {
         var n = "<" + e;
         if (t && t.length > 0)
             for (var i, o = 0; void 0 !== (i = t[o]);) n += " " + i[0] + '="' + this.esc(i[1]) + '"', o++;
         return r && (n += " /"), n += ">"
-    }, Ag.prototype.esc = Id;
+    }, qg.prototype.esc = Fd;
     const {
-        Boolean: qg
-    } = A;
+        Boolean: Eg
+    } = q;
 
-    function Eg(e, t, r) {
+    function Tg(e, t, r) {
         const n = e.slice();
         return n[90] = t[r][0], n[91] = t[r][1], n[92] = t[r][2], n[93] = t[r][3], n
     }
 
-    function Tg(e, t, r) {
+    function $g(e, t, r) {
         const n = e.slice();
         return n[87] = t[r].installed_addon, n[88] = t[r].alternative_addons, n[86] = r, n
     }
 
-    function $g(e, t, r) {
+    function Og(e, t, r) {
         const n = e.slice();
         return n[83] = t[r].folders, n[84] = t[r].matches, n[86] = r, n
     }
 
-    function Og(e) {
+    function Sg(e) {
         let t, r, n, i, o, s, a, l, u, c, f, h, p, d;
 
         function m(t) {
             e[42](t)
         }
 
         function g(t) {
@@ -23837,331 +23857,331 @@
             installedOutdatedCount: e[11],
             reconcileInstallationInProgress: e[7],
             canReconcile: e[16].length > 0,
             isRefreshing: e[6],
             isModifying: e[12].length > 0,
             isSearching: e[18] > 0
         };
-        void 0 !== e[1] && (b.activeView = e[1]), void 0 !== e[3] && (b.searchTerms = e[3]), void 0 !== e[4] && (b.searchFilterInstalled = e[4]), void 0 !== e[15] && (b.reconcileStage = e[15]), n = new zh({
+        void 0 !== e[1] && (b.activeView = e[1]), void 0 !== e[3] && (b.searchTerms = e[3]), void 0 !== e[4] && (b.searchFilterInstalled = e[4]), void 0 !== e[15] && (b.reconcileStage = e[15]), n = new Hh({
             props: b
-        }), fe.push((() => Ue(n, "activeView", m))), fe.push((() => Ue(n, "searchTerms", g))), fe.push((() => Ue(n, "searchFilterInstalled", v))), fe.push((() => Ue(n, "reconcileStage", y))), n.$on("requestSearch", e[46]), n.$on("requestShowSearchOptionsModal", e[47]), n.$on("requestRefresh", e[48]), n.$on("requestUpdateAll", e[49]), n.$on("requestInstallReconciled", e[50]), n.$on("requestAutomateReconciliation", e[51]), n.$on("requestInstallReconciledInstalled", e[52]), n.$on("requestCycleListFormat", e[53]);
-        u = new xp({
+        }), he.push((() => ze(n, "activeView", m))), he.push((() => ze(n, "searchTerms", g))), he.push((() => ze(n, "searchFilterInstalled", v))), he.push((() => ze(n, "reconcileStage", y))), n.$on("requestSearch", e[46]), n.$on("requestShowSearchOptionsModal", e[47]), n.$on("requestRefresh", e[48]), n.$on("requestUpdateAll", e[49]), n.$on("requestInstallReconciled", e[50]), n.$on("requestAutomateReconciliation", e[51]), n.$on("requestInstallReconciledInstalled", e[52]), n.$on("requestCycleListFormat", e[53]);
+        u = new Ap({
             props: {}
         }), e[54](u), u.$on("selectItem", e[55]);
-        let w = e[19] && Sg(e);
-        const _ = [Fg, Ig, Ng],
+        let w = e[19] && Dg(e);
+        const _ = [Mg, Fg, Ig],
             k = [];
 
         function x(e, t) {
-            return e[1] === xh.Reconcile ? 0 : e[1] === xh.ReconcileInstalled ? 1 : 2
+            return e[1] === Ah.Reconcile ? 0 : e[1] === Ah.ReconcileInstalled ? 1 : 2
         }
         return h = x(e), p = k[h] = _[h](e), {
             c() {
-                t = D("div"), r = D("div"), Ve(n.$$.fragment), l = L(), Ve(u.$$.fragment), c = L(), w && w.c(), f = L(), p.c(), P(r, "class", "addon-list-nav-wrapper svelte-1b3u0f7"), P(t, "class", "addon-list-wrapper svelte-1b3u0f7")
+                t = C("div"), r = C("div"), He(n.$$.fragment), l = N(), He(u.$$.fragment), c = N(), w && w.c(), f = N(), p.c(), j(r, "class", "addon-list-nav-wrapper svelte-1b3u0f7"), j(t, "class", "addon-list-wrapper svelte-1b3u0f7")
             },
             m(e, i) {
-                $(e, t, i), q(t, r), ze(n, r, null), q(t, l), ze(u, t, null), q(t, c), w && w.m(t, null), q(t, f), k[h].m(t, null), d = !0
+                O(e, t, i), E(t, r), We(n, r, null), E(t, l), We(u, t, null), E(t, c), w && w.m(t, null), E(t, f), k[h].m(t, null), d = !0
             },
             p(e, r) {
                 const l = {};
-                16384 & r[0] && (l.searchIsDirty = e[14]), 2048 & r[0] && (l.installedOutdatedCount = e[11]), 128 & r[0] && (l.reconcileInstallationInProgress = e[7]), 65536 & r[0] && (l.canReconcile = e[16].length > 0), 64 & r[0] && (l.isRefreshing = e[6]), 4096 & r[0] && (l.isModifying = e[12].length > 0), 262144 & r[0] && (l.isSearching = e[18] > 0), !i && 2 & r[0] && (i = !0, l.activeView = e[1], ve((() => i = !1))), !o && 8 & r[0] && (o = !0, l.searchTerms = e[3], ve((() => o = !1))), !s && 16 & r[0] && (s = !0, l.searchFilterInstalled = e[4], ve((() => s = !1))), !a && 32768 & r[0] && (a = !0, l.reconcileStage = e[15], ve((() => a = !1))), n.$set(l);
-                u.$set({}), e[19] ? w ? (w.p(e, r), 524288 & r[0] && Oe(w, 1)) : (w = Sg(e), w.c(), Oe(w, 1), w.m(t, f)) : w && (Te(), Se(w, 1, 1, (() => {
+                16384 & r[0] && (l.searchIsDirty = e[14]), 2048 & r[0] && (l.installedOutdatedCount = e[11]), 128 & r[0] && (l.reconcileInstallationInProgress = e[7]), 65536 & r[0] && (l.canReconcile = e[16].length > 0), 64 & r[0] && (l.isRefreshing = e[6]), 4096 & r[0] && (l.isModifying = e[12].length > 0), 262144 & r[0] && (l.isSearching = e[18] > 0), !i && 2 & r[0] && (i = !0, l.activeView = e[1], ye((() => i = !1))), !o && 8 & r[0] && (o = !0, l.searchTerms = e[3], ye((() => o = !1))), !s && 16 & r[0] && (s = !0, l.searchFilterInstalled = e[4], ye((() => s = !1))), !a && 32768 & r[0] && (a = !0, l.reconcileStage = e[15], ye((() => a = !1))), n.$set(l);
+                u.$set({}), e[19] ? w ? (w.p(e, r), 524288 & r[0] && Se(w, 1)) : (w = Dg(e), w.c(), Se(w, 1), w.m(t, f)) : w && ($e(), De(w, 1, 1, (() => {
                     w = null
-                })), $e());
+                })), Oe());
                 let c = h;
-                h = x(e), h === c ? k[h].p(e, r) : (Te(), Se(k[c], 1, 1, (() => {
+                h = x(e), h === c ? k[h].p(e, r) : ($e(), De(k[c], 1, 1, (() => {
                     k[c] = null
-                })), $e(), p = k[h], p ? p.p(e, r) : (p = k[h] = _[h](e), p.c()), Oe(p, 1), p.m(t, null))
+                })), Oe(), p = k[h], p ? p.p(e, r) : (p = k[h] = _[h](e), p.c()), Se(p, 1), p.m(t, null))
             },
             i(e) {
-                d || (Oe(n.$$.fragment, e), Oe(u.$$.fragment, e), Oe(w), Oe(p), d = !0)
+                d || (Se(n.$$.fragment, e), Se(u.$$.fragment, e), Se(w), Se(p), d = !0)
             },
             o(e) {
-                Se(n.$$.fragment, e), Se(u.$$.fragment, e), Se(w), Se(p), d = !1
+                De(n.$$.fragment, e), De(u.$$.fragment, e), De(w), De(p), d = !1
             },
             d(r) {
-                r && O(t), He(n), e[54](null), He(u), w && w.d(), k[h].d()
+                r && S(t), Ge(n), e[54](null), Ge(u), w && w.d(), k[h].d()
             }
         }
     }
 
-    function Sg(e) {
+    function Dg(e) {
         let t, r;
-        return t = new zn({
+        return t = new Hn({
             props: {
                 $$slots: {
-                    default: [Lg]
+                    default: [Ng]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), t.$on("dismiss", e[29]), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, n) {
-                ze(t, e, n), r = !0
+                We(t, e, n), r = !0
             },
             p(e, r) {
                 const n = {};
                 524592 & r[0] | 8 & r[3] && (n.$$scope = {
                     dirty: r,
                     ctx: e
                 }), t.$set(n)
             },
             i(e) {
-                r || (Oe(t.$$.fragment, e), r = !0)
+                r || (Se(t.$$.fragment, e), r = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), r = !1
+                De(t.$$.fragment, e), r = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function Dg(e) {
+    function Cg(e) {
         let t, r, n;
 
         function i(t) {
             e[57](t)
         }
         let o = {
             flavour: e[21].game_flavour,
             sources: e[8],
             searchFilterInstalled: e[4]
         };
-        return void 0 !== e[5] && (o.searchOptions = e[5]), t = new Al({
+        return void 0 !== e[5] && (o.searchOptions = e[5]), t = new ql({
             props: o
-        }), fe.push((() => Ue(t, "searchOptions", i))), t.$on("requestSearch", e[25]), t.$on("requestReset", e[36]), {
+        }), he.push((() => ze(t, "searchOptions", i))), t.$on("requestSearch", e[25]), t.$on("requestReset", e[36]), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, r) {
-                ze(t, e, r), n = !0
+                We(t, e, r), n = !0
             },
             p(e, n) {
                 const i = {};
-                256 & n[0] && (i.sources = e[8]), 16 & n[0] && (i.searchFilterInstalled = e[4]), !r && 32 & n[0] && (r = !0, i.searchOptions = e[5], ve((() => r = !1))), t.$set(i)
+                256 & n[0] && (i.sources = e[8]), 16 & n[0] && (i.searchFilterInstalled = e[4]), !r && 32 & n[0] && (r = !0, i.searchOptions = e[5], ye((() => r = !1))), t.$set(i)
             },
             i(e) {
-                n || (Oe(t.$$.fragment, e), n = !0)
+                n || (Se(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), n = !1
+                De(t.$$.fragment, e), n = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function Cg(e) {
+    function Rg(e) {
         let t, n;
         const i = [e[19].dynamicProps];
         let o = {};
         for (let e = 0; e < i.length; e += 1) o = r(o, i[e]);
-        return t = new Ol({
+        return t = new Sl({
             props: o
         }), t.$on("requestRollback", e[56]), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, r) {
-                ze(t, e, r), n = !0
+                We(t, e, r), n = !0
             },
             p(e, r) {
-                const n = 524288 & r[0] ? je(i, [Be(e[19].dynamicProps)]) : {};
+                const n = 524288 & r[0] ? Ue(i, [Ve(e[19].dynamicProps)]) : {};
                 t.$set(n)
             },
             i(e) {
-                n || (Oe(t.$$.fragment, e), n = !0)
+                n || (Se(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), n = !1
+                De(t.$$.fragment, e), n = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function Rg(e) {
+    function Lg(e) {
         let t, n;
         const i = [e[19].dynamicProps];
         let o = {};
         for (let e = 0; e < i.length; e += 1) o = r(o, i[e]);
-        return t = new fh({
+        return t = new hh({
             props: o
         }), {
             c() {
-                Ve(t.$$.fragment)
+                He(t.$$.fragment)
             },
             m(e, r) {
-                ze(t, e, r), n = !0
+                We(t, e, r), n = !0
             },
             p(e, r) {
-                const n = 524288 & r[0] ? je(i, [Be(e[19].dynamicProps)]) : {};
+                const n = 524288 & r[0] ? Ue(i, [Ve(e[19].dynamicProps)]) : {};
                 t.$set(n)
             },
             i(e) {
-                n || (Oe(t.$$.fragment, e), n = !0)
+                n || (Se(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Se(t.$$.fragment, e), n = !1
+                De(t.$$.fragment, e), n = !1
             },
             d(e) {
-                He(t, e)
+                Ge(t, e)
             }
         }
     }
 
-    function Lg(e) {
+    function Ng(e) {
         let t, r, n, i;
-        const o = [Rg, Cg, Dg],
+        const o = [Lg, Rg, Cg],
             s = [];
 
         function a(e, t) {
             return "changelog" === e[19].id ? 0 : "rollback" === e[19].id ? 1 : "searchOptions" === e[19].id ? 2 : -1
         }
         return ~(t = a(e)) && (r = s[t] = o[t](e)), {
             c() {
-                r && r.c(), n = N()
+                r && r.c(), n = I()
             },
             m(e, r) {
-                ~t && s[t].m(e, r), $(e, n, r), i = !0
+                ~t && s[t].m(e, r), O(e, n, r), i = !0
             },
             p(e, i) {
                 let l = t;
-                t = a(e), t === l ? ~t && s[t].p(e, i) : (r && (Te(), Se(s[l], 1, 1, (() => {
+                t = a(e), t === l ? ~t && s[t].p(e, i) : (r && ($e(), De(s[l], 1, 1, (() => {
                     s[l] = null
-                })), $e()), ~t ? (r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Oe(r, 1), r.m(n.parentNode, n)) : r = null)
+                })), Oe()), ~t ? (r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Se(r, 1), r.m(n.parentNode, n)) : r = null)
             },
             i(e) {
-                i || (Oe(r), i = !0)
+                i || (Se(r), i = !0)
             },
             o(e) {
-                Se(r), i = !1
+                De(r), i = !1
             },
             d(e) {
-                ~t && s[t].d(e), e && O(n)
+                e && S(n), ~t && s[t].d(e)
             }
         }
     }
 
-    function Ng(t) {
+    function Ig(t) {
         let r, n, i = t[1],
-            o = Pg(t);
+            o = jg(t);
         return {
             c() {
-                o.c(), r = N()
+                o.c(), r = I()
             },
             m(e, t) {
-                o.m(e, t), $(e, r, t), n = !0
+                o.m(e, t), O(e, r, t), n = !0
             },
             p(t, n) {
-                2 & n[0] && a(i, i = t[1]) ? (Te(), Se(o, 1, 1, e), $e(), o = Pg(t), o.c(), Oe(o, 1), o.m(r.parentNode, r)) : o.p(t, n)
+                2 & n[0] && a(i, i = t[1]) ? ($e(), De(o, 1, 1, e), Oe(), o = jg(t), o.c(), Se(o, 1), o.m(r.parentNode, r)) : o.p(t, n)
             },
             i(e) {
-                n || (Oe(o), n = !0)
+                n || (Se(o), n = !0)
             },
             o(e) {
-                Se(o), n = !1
+                De(o), n = !1
             },
             d(e) {
-                e && O(r), o.d(e)
+                e && S(r), o.d(e)
             }
         }
     }
 
-    function Ig(e) {
+    function Fg(e) {
         let t, r, n = {
             ctx: e,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: Hg,
-            then: Bg,
-            catch: jg,
+            pending: Wg,
+            then: Ug,
+            catch: Bg,
             value: 82,
             blocks: [, , , ]
         };
-        return Le(e[34](), n), {
+        return Ne(e[34](), n), {
             c() {
-                t = N(), n.block.c()
+                t = I(), n.block.c()
             },
             m(e, i) {
-                $(e, t, i), n.block.m(e, n.anchor = i), n.mount = () => t.parentNode, n.anchor = t, r = !0
+                O(e, t, i), n.block.m(e, n.anchor = i), n.mount = () => t.parentNode, n.anchor = t, r = !0
             },
             p(t, r) {
-                Ne(n, e = t, r)
+                Ie(n, e = t, r)
             },
             i(e) {
-                r || (Oe(n.block), r = !0)
+                r || (Se(n.block), r = !0)
             },
             o(e) {
                 for (let e = 0; e < 3; e += 1) {
-                    Se(n.blocks[e])
+                    De(n.blocks[e])
                 }
                 r = !1
             },
             d(e) {
-                e && O(t), n.block.d(e), n.token = null, n = null
+                e && S(t), n.block.d(e), n.token = null, n = null
             }
         }
     }
 
-    function Fg(e) {
+    function Mg(e) {
         let t, r, n, i = {
             ctx: e,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: Kg,
-            then: Gg,
-            catch: Wg,
+            pending: Xg,
+            then: Zg,
+            catch: Gg,
             value: 82,
             blocks: [, , , ]
         };
-        return Le(r = e[32](e[15]), i), {
+        return Ne(r = e[32](e[15]), i), {
             c() {
-                t = N(), i.block.c()
+                t = I(), i.block.c()
             },
             m(e, r) {
-                $(e, t, r), i.block.m(e, i.anchor = r), i.mount = () => t.parentNode, i.anchor = t, n = !0
+                O(e, t, r), i.block.m(e, i.anchor = r), i.mount = () => t.parentNode, i.anchor = t, n = !0
             },
             p(t, n) {
-                e = t, i.ctx = e, 32768 & n[0] && r !== (r = e[32](e[15])) && Le(r, i) || Ne(i, e, n)
+                e = t, i.ctx = e, 32768 & n[0] && r !== (r = e[32](e[15])) && Ne(r, i) || Ie(i, e, n)
             },
             i(e) {
-                n || (Oe(i.block), n = !0)
+                n || (Se(i.block), n = !0)
             },
             o(e) {
                 for (let e = 0; e < 3; e += 1) {
-                    Se(i.blocks[e])
+                    De(i.blocks[e])
                 }
                 n = !1
             },
             d(e) {
-                e && O(t), i.block.d(e), i.token = null, i = null
+                e && S(t), i.block.d(e), i.token = null, i = null
             }
         }
     }
 
-    function Mg(r, n) {
+    function Pg(r, n) {
         let i, o, s, a, l, u = e;
-        return o = new Fp({
+        return o = new Mp({
             props: {
                 addon: n[90],
                 otherAddon: n[91],
                 isInstalled: n[92],
                 beingModified: n[12].includes(n[93]),
-                format: n[1] === xh.Search ? n[10] : n[9],
+                format: n[1] === Ah.Search ? n[10] : n[9],
                 isRefreshing: n[6],
                 downloadProgress: n[13][n[93]] || 0
             }
         }), o.$on("requestInstall", (function() {
             return n[59](n[91])
         })), o.$on("requestUpdate", (function() {
             return n[60](n[91])
@@ -24171,29 +24191,29 @@
             return n[62](n[91])
         })), o.$on("requestShowAddonContextMenu", (function(...e) {
             return n[63](n[92], n[90], n[91], ...e)
         })), {
             key: r,
             first: null,
             c() {
-                i = D("li"), Ve(o.$$.fragment), s = L(), P(i, "class", "svelte-1b3u0f7"), this.first = i
+                i = C("li"), He(o.$$.fragment), s = N(), j(i, "class", "svelte-1b3u0f7"), this.first = i
             },
             m(e, t) {
-                $(e, i, t), ze(o, i, null), q(i, s), l = !0
+                O(e, i, t), We(o, i, null), E(i, s), l = !0
             },
             p(e, t) {
                 n = e;
                 const r = {};
-                6 & t[0] && (r.addon = n[90]), 6 & t[0] && (r.otherAddon = n[91]), 6 & t[0] && (r.isInstalled = n[92]), 4102 & t[0] && (r.beingModified = n[12].includes(n[93])), 1538 & t[0] && (r.format = n[1] === xh.Search ? n[10] : n[9]), 64 & t[0] && (r.isRefreshing = n[6]), 8198 & t[0] && (r.downloadProgress = n[13][n[93]] || 0), o.$set(r)
+                6 & t[0] && (r.addon = n[90]), 6 & t[0] && (r.otherAddon = n[91]), 6 & t[0] && (r.isInstalled = n[92]), 4102 & t[0] && (r.beingModified = n[12].includes(n[93])), 1538 & t[0] && (r.format = n[1] === Ah.Search ? n[10] : n[9]), 64 & t[0] && (r.isRefreshing = n[6]), 8198 & t[0] && (r.downloadProgress = n[13][n[93]] || 0), o.$set(r)
             },
             r() {
                 a = i.getBoundingClientRect()
             },
             f() {
-                re(i), u()
+                ne(i), u()
             },
             a() {
                 u(), u = function(r, n, i, o) {
                     if (!n) return e;
                     const s = r.getBoundingClientRect();
                     if (n.left === s.left && n.right === s.right && n.top === s.top && n.bottom === s.bottom) return e;
                     const {
@@ -24208,567 +24228,567 @@
                         from: n,
                         to: s
                     }, o);
                     let d, m = !0,
                         g = !1;
 
                     function v() {
-                        p && te(r, d), m = !1
+                        p && re(r, d), m = !1
                     }
                     return x((e => {
                         if (!g && e >= c && (g = !0), g && e >= f && (h(1, 0), v()), !m) return !1;
                         if (g) {
                             const t = 0 + 1 * u((e - c) / l);
                             h(t, 1 - t)
                         }
                         return !0
-                    })), p && (d = ee(r, 0, 1, l, a, u, p)), a || (g = !0), h(0, 1), v
-                }(i, a, Mp, {
+                    })), p && (d = te(r, 0, 1, l, a, u, p)), a || (g = !0), h(0, 1), v
+                }(i, a, Pp, {
                     duration: 250
                 })
             },
             i(e) {
-                l || (Oe(o.$$.fragment, e), l = !0)
+                l || (Se(o.$$.fragment, e), l = !0)
             },
             o(e) {
-                Se(o.$$.fragment, e), l = !1
+                De(o.$$.fragment, e), l = !1
             },
             d(e) {
-                e && O(i), He(o)
+                e && S(i), Ge(o)
             }
         }
     }
 
-    function Pg(e) {
+    function jg(e) {
         let t, r, n, i = [],
             o = new Map,
-            s = e[2][e[1]].map(ev);
+            s = Fe(e[2][e[1]].map(tv));
         const a = e => e[93];
         for (let t = 0; t < s.length; t += 1) {
-            let r = Eg(e, s, t),
+            let r = Tg(e, s, t),
                 n = a(r);
-            o.set(n, i[t] = Mg(n, r))
+            o.set(n, i[t] = Pg(n, r))
         }
         return {
             c() {
-                t = D("ul");
+                t = C("ul");
                 for (let e = 0; e < i.length; e += 1) i[e].c();
-                P(t, "class", "addon-list svelte-1b3u0f7")
+                j(t, "class", "addon-list svelte-1b3u0f7")
             },
             m(e, r) {
-                $(e, t, r);
+                O(e, t, r);
                 for (let e = 0; e < i.length; e += 1) i[e] && i[e].m(t, null);
                 n = !0
             },
             p(e, r) {
                 if (1237333574 & r[0]) {
-                    s = e[2][e[1]].map(ev), Te();
+                    s = Fe(e[2][e[1]].map(tv)), $e();
                     for (let e = 0; e < i.length; e += 1) i[e].r();
-                    i = Pe(i, r, a, 1, e, s, o, t, Me, Mg, null, Eg);
+                    i = Be(i, r, a, 1, e, s, o, t, je, Pg, null, Tg);
                     for (let e = 0; e < i.length; e += 1) i[e].a();
-                    $e()
+                    Oe()
                 }
             },
             i(e) {
                 if (!n) {
-                    for (let e = 0; e < s.length; e += 1) Oe(i[e]);
-                    r || ge((() => {
-                        r = Ce(t, Ke, {
+                    for (let e = 0; e < s.length; e += 1) Se(i[e]);
+                    e && (r || ve((() => {
+                        r = Re(t, Qe, {
                             duration: 250
                         }), r.start()
-                    })), n = !0
+                    }))), n = !0
                 }
             },
             o(e) {
-                for (let e = 0; e < i.length; e += 1) Se(i[e]);
+                for (let e = 0; e < i.length; e += 1) De(i[e]);
                 n = !1
             },
             d(e) {
-                e && O(t);
+                e && S(t);
                 for (let e = 0; e < i.length; e += 1) i[e].d()
             }
         }
     }
 
-    function jg(t) {
+    function Bg(t) {
         return {
             c: e,
             m: e,
             p: e,
             i: e,
             o: e,
             d: e
         }
     }
 
-    function Bg(e) {
+    function Ug(e) {
         let t, r, n, i;
-        const o = [Vg, Ug],
+        const o = [zg, Vg],
             s = [];
         return t = function(e, t) {
             return e[82].length ? 0 : 1
         }(e), r = s[t] = o[t](e), {
             c() {
-                r.c(), n = N()
+                r.c(), n = I()
             },
             m(e, r) {
-                s[t].m(e, r), $(e, n, r), i = !0
+                s[t].m(e, r), O(e, n, r), i = !0
             },
             p(e, t) {
                 r.p(e, t)
             },
             i(e) {
-                i || (Oe(r), i = !0)
+                i || (Se(r), i = !0)
             },
             o(e) {
-                Se(r), i = !1
+                De(r), i = !1
             },
             d(e) {
-                s[t].d(e), e && O(n)
+                e && S(n), s[t].d(e)
             }
         }
     }
 
-    function Ug(t) {
+    function Vg(t) {
         let r, n;
         return {
             c() {
-                r = D("div"), r.innerHTML = '<div class="svelte-1b3u0f7">No alternative sources available.</div>', P(r, "class", "placeholder svelte-1b3u0f7")
+                r = C("div"), r.innerHTML = '<div class="svelte-1b3u0f7">No alternative sources available.</div>', j(r, "class", "placeholder svelte-1b3u0f7")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             i(e) {
-                n || ge((() => {
-                    n = Ce(r, Ye, {}), n.start()
-                }))
+                e && (n || ve((() => {
+                    n = Re(r, Xe, {}), n.start()
+                })))
             },
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Vg(e) {
-        let t, r, n = e[82],
+    function zg(e) {
+        let t, r, n = Fe(e[82]),
             i = [];
-        for (let t = 0; t < n.length; t += 1) i[t] = zg(Tg(e, n, t));
-        const o = e => Se(i[e], 1, 1, (() => {
+        for (let t = 0; t < n.length; t += 1) i[t] = Hg($g(e, n, t));
+        const o = e => De(i[e], 1, 1, (() => {
             i[e] = null
         }));
         return {
             c() {
-                t = D("ul");
+                t = C("ul");
                 for (let e = 0; e < i.length; e += 1) i[e].c();
-                P(t, "class", "addon-list svelte-1b3u0f7")
+                j(t, "class", "addon-list svelte-1b3u0f7")
             },
             m(e, n) {
-                $(e, t, n);
+                O(e, t, n);
                 for (let e = 0; e < i.length; e += 1) i[e] && i[e].m(t, null);
                 r = !0
             },
             p(e, r) {
                 if (131072 & r[0] | 8 & r[1]) {
                     let s;
-                    for (n = e[82], s = 0; s < n.length; s += 1) {
-                        const o = Tg(e, n, s);
-                        i[s] ? (i[s].p(o, r), Oe(i[s], 1)) : (i[s] = zg(o), i[s].c(), Oe(i[s], 1), i[s].m(t, null))
+                    for (n = Fe(e[82]), s = 0; s < n.length; s += 1) {
+                        const o = $g(e, n, s);
+                        i[s] ? (i[s].p(o, r), Se(i[s], 1)) : (i[s] = Hg(o), i[s].c(), Se(i[s], 1), i[s].m(t, null))
                     }
-                    for (Te(), s = n.length; s < i.length; s += 1) o(s);
-                    $e()
+                    for ($e(), s = n.length; s < i.length; s += 1) o(s);
+                    Oe()
                 }
             },
             i(e) {
                 if (!r) {
-                    for (let e = 0; e < n.length; e += 1) Oe(i[e]);
+                    for (let e = 0; e < n.length; e += 1) Se(i[e]);
                     r = !0
                 }
             },
             o(e) {
-                i = i.filter(qg);
-                for (let e = 0; e < i.length; e += 1) Se(i[e]);
+                i = i.filter(Eg);
+                for (let e = 0; e < i.length; e += 1) De(i[e]);
                 r = !1
             },
             d(e) {
-                e && O(t), S(i, e)
+                e && S(t), D(i, e)
             }
         }
     }
 
-    function zg(e) {
+    function Hg(e) {
         let t, r, n, i;
-        return r = new kh({
+        return r = new xh({
             props: {
                 selections: e[17],
                 folders: [{
                     name: e[87].name,
                     version: ""
                 }],
                 choices: [e[87], ...e[88]],
                 idx: e[86],
                 expanded: !0
             }
         }), {
             c() {
-                t = D("li"), Ve(r.$$.fragment), n = L(), P(t, "class", "svelte-1b3u0f7")
+                t = C("li"), He(r.$$.fragment), n = N(), j(t, "class", "svelte-1b3u0f7")
             },
             m(e, o) {
-                $(e, t, o), ze(r, t, null), q(t, n), i = !0
+                O(e, t, o), We(r, t, null), E(t, n), i = !0
             },
             p(e, t) {
                 const n = {};
                 131072 & t[0] && (n.selections = e[17]), r.$set(n)
             },
             i(e) {
-                i || (Oe(r.$$.fragment, e), i = !0)
+                i || (Se(r.$$.fragment, e), i = !0)
             },
             o(e) {
-                Se(r.$$.fragment, e), i = !1
+                De(r.$$.fragment, e), i = !1
             },
             d(e) {
-                e && O(t), He(r)
+                e && S(t), Ge(r)
             }
         }
     }
 
-    function Hg(t) {
+    function Wg(t) {
         let r, n;
         return {
             c() {
-                r = D("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Hold on tight!</div>', P(r, "class", "placeholder svelte-1b3u0f7")
+                r = C("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Hold on tight!</div>', j(r, "class", "placeholder svelte-1b3u0f7")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             i(e) {
-                n || ge((() => {
-                    n = Ce(r, Ye, {}), n.start()
-                }))
+                e && (n || ve((() => {
+                    n = Re(r, Xe, {}), n.start()
+                })))
             },
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Wg(t) {
+    function Gg(t) {
         return {
             c: e,
             m: e,
             p: e,
             i: e,
             o: e,
             d: e
         }
     }
 
-    function Gg(e) {
+    function Zg(e) {
         let t, r, n, i;
-        const o = [Jg, Zg],
+        const o = [Yg, Jg],
             s = [];
 
         function a(e, t) {
             return e[82] && e[82].length ? 0 : 1
         }
         return t = a(e), r = s[t] = o[t](e), {
             c() {
-                r.c(), n = N()
+                r.c(), n = I()
             },
             m(e, r) {
-                s[t].m(e, r), $(e, n, r), i = !0
+                s[t].m(e, r), O(e, n, r), i = !0
             },
             p(e, i) {
                 let l = t;
-                t = a(e), t === l ? s[t].p(e, i) : (Te(), Se(s[l], 1, 1, (() => {
+                t = a(e), t === l ? s[t].p(e, i) : ($e(), De(s[l], 1, 1, (() => {
                     s[l] = null
-                })), $e(), r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Oe(r, 1), r.m(n.parentNode, n))
+                })), Oe(), r = s[t], r ? r.p(e, i) : (r = s[t] = o[t](e), r.c()), Se(r, 1), r.m(n.parentNode, n))
             },
             i(e) {
-                i || (Oe(r), i = !0)
+                i || (Se(r), i = !0)
             },
             o(e) {
-                Se(r), i = !1
+                De(r), i = !1
             },
             d(e) {
-                s[t].d(e), e && O(n)
+                e && S(n), s[t].d(e)
             }
         }
     }
 
-    function Zg(t) {
+    function Jg(t) {
         let r, n;
         return {
             c() {
-                r = D("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Reconciliation complete.</div>', P(r, "class", "placeholder svelte-1b3u0f7")
+                r = C("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Reconciliation complete.</div>', j(r, "class", "placeholder svelte-1b3u0f7")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             i(e) {
-                n || ge((() => {
-                    n = Ce(r, Ye, {}), n.start()
-                }))
+                e && (n || ve((() => {
+                    n = Re(r, Xe, {}), n.start()
+                })))
             },
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Jg(e) {
+    function Yg(e) {
         let t, r, n, i, o, s, a;
-        r = new Yn({
+        r = new Kn({
             props: {
-                icon: mn
+                icon: gn
             }
         });
-        let l = e[82],
+        let l = Fe(e[82]),
             u = [];
-        for (let t = 0; t < l.length; t += 1) u[t] = Yg($g(e, l, t));
-        const c = e => Se(u[e], 1, 1, (() => {
+        for (let t = 0; t < l.length; t += 1) u[t] = Kg(Og(e, l, t));
+        const c = e => De(u[e], 1, 1, (() => {
             u[e] = null
         }));
         return {
             c() {
-                t = D("div"), Ve(r.$$.fragment), n = L(), i = D("p"), i.innerHTML = "Reconciliation is the process by which installed add-ons are linked with add-ons from\n              sources. This is done in three stages in decreasing order of accuracy. Add-ons do not\n              always carry source metadata and <i>instawow</i>\n              employs a number of heuristics to reconcile add-ons which cannot be positively\n              identified. If you trust <i>instawow</i>\n              to do this without supervision, press &quot;<b>automate</b>&quot;.\n              Otherwise, review your selections below and press &quot;<b>install</b>&quot;\n              to proceed to the next stage. Reconciled add-ons will be reinstalled.", o = L(), s = D("ul");
+                t = C("div"), He(r.$$.fragment), n = N(), i = C("p"), i.innerHTML = "Reconciliation is the process by which installed add-ons are linked with add-ons from\n              sources. This is done in three stages in decreasing order of accuracy. Add-ons do not\n              always carry source metadata and <i>instawow</i>\n              employs a number of heuristics to reconcile add-ons which cannot be positively\n              identified. If you trust <i>instawow</i>\n              to do this without supervision, press &quot;<b>automate</b>&quot;.\n              Otherwise, review your selections below and press &quot;<b>install</b>&quot;\n              to proceed to the next stage. Reconciled add-ons will be reinstalled.", o = N(), s = C("ul");
                 for (let e = 0; e < u.length; e += 1) u[e].c();
-                P(i, "class", "svelte-1b3u0f7"), P(t, "class", "preamble svelte-1b3u0f7"), P(s, "class", "addon-list svelte-1b3u0f7")
+                j(i, "class", "svelte-1b3u0f7"), j(t, "class", "preamble svelte-1b3u0f7"), j(s, "class", "addon-list svelte-1b3u0f7")
             },
             m(e, l) {
-                $(e, t, l), ze(r, t, null), q(t, n), q(t, i), $(e, o, l), $(e, s, l);
+                O(e, t, l), We(r, t, null), E(t, n), E(t, i), O(e, o, l), O(e, s, l);
                 for (let e = 0; e < u.length; e += 1) u[e] && u[e].m(s, null);
                 a = !0
             },
             p(e, t) {
                 if (98304 & t[0] | 2 & t[1]) {
                     let r;
-                    for (l = e[82], r = 0; r < l.length; r += 1) {
-                        const n = $g(e, l, r);
-                        u[r] ? (u[r].p(n, t), Oe(u[r], 1)) : (u[r] = Yg(n), u[r].c(), Oe(u[r], 1), u[r].m(s, null))
+                    for (l = Fe(e[82]), r = 0; r < l.length; r += 1) {
+                        const n = Og(e, l, r);
+                        u[r] ? (u[r].p(n, t), Se(u[r], 1)) : (u[r] = Kg(n), u[r].c(), Se(u[r], 1), u[r].m(s, null))
                     }
-                    for (Te(), r = l.length; r < u.length; r += 1) c(r);
-                    $e()
+                    for ($e(), r = l.length; r < u.length; r += 1) c(r);
+                    Oe()
                 }
             },
             i(e) {
                 if (!a) {
-                    Oe(r.$$.fragment, e);
-                    for (let e = 0; e < l.length; e += 1) Oe(u[e]);
+                    Se(r.$$.fragment, e);
+                    for (let e = 0; e < l.length; e += 1) Se(u[e]);
                     a = !0
                 }
             },
             o(e) {
-                Se(r.$$.fragment, e), u = u.filter(qg);
-                for (let e = 0; e < u.length; e += 1) Se(u[e]);
+                De(r.$$.fragment, e), u = u.filter(Eg);
+                for (let e = 0; e < u.length; e += 1) De(u[e]);
                 a = !1
             },
             d(e) {
-                e && O(t), He(r), e && O(o), e && O(s), S(u, e)
+                e && (S(t), S(o), S(s)), Ge(r), D(u, e)
             }
         }
     }
 
-    function Yg(e) {
+    function Kg(e) {
         let t, r, n, i, o;
 
         function s(t) {
             e[58](t)
         }
         let a = {
             folders: e[83],
             choices: e[84],
             idx: e[86]
         };
-        return void 0 !== e[16] && (a.selections = e[16]), r = new kh({
+        return void 0 !== e[16] && (a.selections = e[16]), r = new xh({
             props: a
-        }), fe.push((() => Ue(r, "selections", s))), {
+        }), he.push((() => ze(r, "selections", s))), {
             c() {
-                t = D("li"), Ve(r.$$.fragment), i = L(), P(t, "class", "svelte-1b3u0f7")
+                t = C("li"), He(r.$$.fragment), i = N(), j(t, "class", "svelte-1b3u0f7")
             },
             m(e, n) {
-                $(e, t, n), ze(r, t, null), q(t, i), o = !0
+                O(e, t, n), We(r, t, null), E(t, i), o = !0
             },
             p(e, t) {
                 const i = {};
-                32768 & t[0] && (i.folders = e[83]), 32768 & t[0] && (i.choices = e[84]), !n && 65536 & t[0] && (n = !0, i.selections = e[16], ve((() => n = !1))), r.$set(i)
+                32768 & t[0] && (i.folders = e[83]), 32768 & t[0] && (i.choices = e[84]), !n && 65536 & t[0] && (n = !0, i.selections = e[16], ye((() => n = !1))), r.$set(i)
             },
             i(e) {
-                o || (Oe(r.$$.fragment, e), o = !0)
+                o || (Se(r.$$.fragment, e), o = !0)
             },
             o(e) {
-                Se(r.$$.fragment, e), o = !1
+                De(r.$$.fragment, e), o = !1
             },
             d(e) {
-                e && O(t), He(r)
+                e && S(t), Ge(r)
             }
         }
     }
 
-    function Kg(t) {
+    function Xg(t) {
         let r, n;
         return {
             c() {
-                r = D("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Hold on tight!</div>', P(r, "class", "placeholder svelte-1b3u0f7")
+                r = C("div"), r.innerHTML = '<div class="svelte-1b3u0f7">Hold on tight!</div>', j(r, "class", "placeholder svelte-1b3u0f7")
             },
             m(e, t) {
-                $(e, r, t)
+                O(e, r, t)
             },
             p: e,
             i(e) {
-                n || ge((() => {
-                    n = Ce(r, Ye, {}), n.start()
-                }))
+                e && (n || ve((() => {
+                    n = Re(r, Xe, {}), n.start()
+                })))
             },
             o: e,
             d(e) {
-                e && O(r)
+                e && S(r)
             }
         }
     }
 
-    function Xg(e) {
-        let t, r, n = e[0] && Og(e);
+    function Qg(e) {
+        let t, r, n = e[0] && Sg(e);
         return {
             c() {
-                n && n.c(), t = N()
+                n && n.c(), t = I()
             },
             m(e, i) {
-                n && n.m(e, i), $(e, t, i), r = !0
+                n && n.m(e, i), O(e, t, i), r = !0
             },
             p(e, r) {
-                e[0] ? n ? (n.p(e, r), 1 & r[0] && Oe(n, 1)) : (n = Og(e), n.c(), Oe(n, 1), n.m(t.parentNode, t)) : n && (Te(), Se(n, 1, 1, (() => {
+                e[0] ? n ? (n.p(e, r), 1 & r[0] && Se(n, 1)) : (n = Sg(e), n.c(), Se(n, 1), n.m(t.parentNode, t)) : n && ($e(), De(n, 1, 1, (() => {
                     n = null
-                })), $e())
+                })), Oe())
             },
             i(e) {
-                r || (Oe(n), r = !0)
+                r || (Se(n), r = !0)
             },
             o(e) {
-                Se(n), r = !1
+                De(n), r = !1
             },
             d(e) {
-                n && n.d(e), e && O(t)
+                e && S(t), n && n.d(e)
             }
         }
     }
-    const Qg = e => [e.source, e.id || e.alias].join(":"),
-        ev = ([e, ...t]) => [e, ...t, Qg(e)],
-        tv = (e, t) => e.source === t.source && e.id === t.id,
-        rv = Object.values(Vr),
-        nv = {
+    const ev = e => [e.source, e.id || e.alias].join(":"),
+        tv = ([e, ...t]) => [e, ...t, ev(e)],
+        rv = (e, t) => e.source === t.source && e.id === t.id,
+        nv = Object.values(zr),
+        iv = {
             fromAlias: !1,
             limit: 20,
             sources: [],
             startDate: null,
             strategies: {
-                [Br.AnyFlavour]: !1,
-                [Br.AnyReleaseType]: !1,
-                [Br.VersionEq]: ""
+                [Ur.AnyFlavour]: !1,
+                [Ur.AnyReleaseType]: !1,
+                [Ur.VersionEq]: ""
             }
         },
-        iv = (e, t) => t === Ur.Markdown ? {
+        ov = (e, t) => t === Vr.Markdown ? {
             renderAsHtml: !0,
-            changelog: (new _g).render((new gg).parse(e))
+            changelog: (new kg).render((new vg).parse(e))
         } : {
-            renderAsHtml: t === Ur.Html,
+            renderAsHtml: t === Vr.Html,
             changelog: e
         },
-        ov = e => {
+        sv = e => {
             const t = e + 1;
-            return Ah[t] ? t : Ah.Dense
+            return qh[t] ? t : qh.Dense
         };
 
-    function sv(e, t, r) {
+    function av(e, t, r) {
         let n, i, o;
-        c(e, tt, (e => r(66, n = e))), c(e, nn, (e => r(67, i = e))), c(e, an, (e => r(68, o = e)));
+        c(e, nt, (e => r(66, n = e))), c(e, on, (e => r(67, i = e))), c(e, ln, (e => r(68, o = e)));
         let {
             profile: s,
             isActive: a,
             statusMessage: l
         } = t;
         const u = o[s],
             f = i.withProfile(s);
         let h, p, d = {},
-            m = xh.Installed,
-            g = Ah.Compact,
-            y = Ah.Expanded,
+            m = Ah.Installed,
+            g = qh.Compact,
+            y = qh.Expanded,
             b = [],
             w = [],
             _ = [];
         const k = {
-            [xh.Installed]: [],
-            [xh.FilterInstalled]: [],
-            [xh.Search]: []
+            [Ah.Installed]: [],
+            [Ah.FilterInstalled]: [],
+            [Ah.Search]: []
         };
         let x, A, q, E, T = {},
             $ = "",
             O = !1,
-            S = Gn.cloneDeep(nv),
+            S = Zn.cloneDeep(iv),
             D = !1,
-            C = rv[0],
+            C = nv[0],
             R = [],
             L = !1,
             N = 0,
             I = !1;
         const F = (e, t) => {
                 const r = t.filter((e => "success" !== e[1].status)).map((([t, r]) => ({
-                    heading: `failed to ${e} ${t.name} (${Qg(t)})`,
+                    heading: `failed to ${e} ${t.name} (${ev(t)})`,
                     message: r.message
                 })));
-                v(tt, n = {
+                v(nt, n = {
                     ...n,
                     [s]: [...r, ...n[s] ?? []]
                 }, n)
             },
             M = async (e, t, n = {}) => {
-                const i = t.map(Qg);
+                const i = t.map(ev);
                 r(12, _ = [..._, ...i]);
                 try {
                     const i = await (async (e, t) => {
                             const n = setInterval((async () => {
                                 const e = await f.getDownloadProgress();
                                 r(13, T = Object.fromEntries(e.map((({
                                     defn: e,
                                     progress: t
-                                }) => [Qg(e), t]))))
+                                }) => [ev(e), t]))))
                             }), t);
                             try {
                                 return await e
                             } finally {
                                 clearInterval(n)
                             }
-                        })(f.modifyAddons(e, t.map(Wr), n), 1e3),
+                        })(f.modifyAddons(e, t.map(Gr), n), 1e3),
                         o = i.filter((e => "success" === e.status)).map((({
                             addon: e
                         }) => e));
                     if (o.length) {
-                        const t = [...k[xh.Installed]];
+                        const t = [...k[Ah.Installed]];
                         for (const r of [...o].reverse()) {
                             const n = [r, r, "remove" !== e],
-                                i = k[xh.Installed].findIndex((([e]) => tv(e, r))); - 1 === i ? t.unshift(n) : t[i] = n
+                                i = k[Ah.Installed].findIndex((([e]) => rv(e, r))); - 1 === i ? t.unshift(n) : t[i] = n
                         }
-                        r(2, k[xh.Installed] = t, k)
+                        r(2, k[Ah.Installed] = t, k)
                     }
                     F(e, t.map(((e, t) => [e, i[t]])))
                 } finally {
-                    r(12, _ = Gn.difference(_, i))
+                    r(12, _ = Zn.difference(_, i))
                 }
             }, P = async (e, t = !1) => {
                 await M("install", e, {
                     replace: t
                 })
             }, j = async e => {
                 if (!0 === e) {
-                    const e = k[xh.Installed].filter((([{
+                    const e = k[Ah.Installed].filter((([{
                         version: e
                     }, {
                         version: t
                     }]) => e !== t)).map((([, e]) => e));
                     await M("update", e)
                 } else await M("update", e)
             }, B = async (e, t) => {
@@ -24778,58 +24798,66 @@
             }, U = async () => {
                 r(18, N++, N);
                 try {
                     const e = $;
                     if (e) {
                         let t;
                         const n = Object.fromEntries(Object.entries(S.strategies).map((([e, t]) => [e, t || null])));
-                        if (S.fromAlias) t = await f.resolve([{
-                            source: "*",
-                            alias: e,
-                            strategies: n
-                        }]);
-                        else {
+                        if (S.fromAlias) {
+                            let r = "*",
+                                i = e;
+                            const o = e.indexOf(":");
+                            if (-1 !== o) {
+                                const t = e.slice(0, o);
+                                t in d && (r = t, i = e.slice(o + 1))
+                            }
+                            t = await f.resolve([{
+                                source: r,
+                                alias: i,
+                                strategies: n
+                            }])
+                        } else {
                             const i = await f.search(e, S.limit, S.sources, S.startDate, O);
                             if (e !== $) return;
-                            if (O) return r(40, b = i), void r(1, m = xh.FilterInstalled);
+                            if (O) return r(40, b = i), void r(1, m = Ah.FilterInstalled);
                             const o = i.map((e => ({
                                 source: e.source,
                                 alias: e.id,
                                 strategies: n
                             })));
                             t = await f.resolve(o)
                         }
                         if (e !== $) return;
                         r(41, w = t.filter((e => "success" === e.status)).map((({
                             addon: e
-                        }) => e))), r(1, m = xh.Search)
+                        }) => e))), r(1, m = Ah.Search)
                     }
                 } finally {
                     r(18, N--, N)
                 }
             }, V = async (e = !1) => {
                 if (!L) {
                     r(6, L = !0);
                     try {
                         const t = await f.list();
-                        e && r(2, k[xh.Installed] = t.map((e => [e, e, !0])), k);
-                        const n = await f.resolve(t.map(Wr)),
+                        e && r(2, k[Ah.Installed] = t.map((e => [e, e, !0])), k);
+                        const n = await f.resolve(t.map(Gr)),
                             i = t.map(((e, t) => [e, n[t]]));
-                        r(2, k[xh.Installed] = Gn.sortBy(i.map((([e, t]) => [e, "success" === t.status ? t.addon : e, !0])), (([e, {
+                        r(2, k[Ah.Installed] = Zn.sortBy(i.map((([e, t]) => [e, "success" === t.status ? t.addon : e, !0])), (([e, {
                             version: t
                         }]) => [e.version === t, e.name.toLowerCase()])), k), F("resolve", i)
                     } finally {
                         setTimeout((() => r(6, L = !1)), 500)
                     }
                 }
             }, z = async e => {
                 const t = await f.getChangelog(e.source, e.changelog_url);
                 r(19, q = {
                     id: "changelog",
-                    dynamicProps: iv(t, d[e.source].changelog_format)
+                    dynamicProps: ov(t, d[e.source].changelog_format)
                 })
             }, H = () => {
                 r(19, q = {
                     id: "searchOptions"
                 })
             }, W = (e, t, {
                 clientX: r,
@@ -24841,113 +24869,113 @@
                 }, {
                     addon: e,
                     installed: t,
                     supportsRollback: Y(e)
                 })
             }, G = (e, t) => {
                 switch (t) {
-                    case qh.VisitHomepage:
+                    case Eh.VisitHomepage:
                         f.openUrl(e.url);
                         break;
-                    case qh.ViewChangelog:
+                    case Eh.ViewChangelog:
                         z(e);
                         break;
-                    case qh.RevealFolder: {
+                    case Eh.RevealFolder: {
                         const {
                             folders: [{
                                 name: t
                             }]
                         } = e;
                         f.revealFolder([u.addon_dir, t]);
                         break
                     }
-                    case qh.Resolve:
+                    case Eh.Resolve:
                         r(5, S = {
-                            ...Gn.cloneDeep(nv),
+                            ...Zn.cloneDeep(iv),
                             fromAlias: !0,
                             strategies: {
                                 ...e.options,
-                                [Br.VersionEq]: e.options[Br.VersionEq] ? e.version : ""
+                                [Ur.VersionEq]: e.options[Ur.VersionEq] ? e.version : ""
                             }
-                        }), r(3, $ = Qg(e)), U();
+                        }), r(3, $ = `${e.source}:${e.slug}`), U();
                         break;
-                    case qh.Rollback:
+                    case Eh.Rollback:
                         (e => {
                             r(19, q = {
                                 id: "rollback",
                                 dynamicProps: {
                                     addon: e
                                 }
                             })
                         })(e);
                         break;
-                    case qh.Pin:
-                    case qh.Unpin: {
-                        const r = Gn.merge(e);
-                        r.options.version_eq = t === qh.Pin, (async e => {
+                    case Eh.Pin:
+                    case Eh.Unpin: {
+                        const r = Zn.merge(e);
+                        r.options.version_eq = t === Eh.Pin, (async e => {
                             await M("pin", e)
                         })([r]);
                         break
                     }
-                    case qh.Unreconcile:
+                    case Eh.Unreconcile:
                         B([e], !0);
                         break;
-                    case qh.InstallAndReplace:
+                    case Eh.InstallAndReplace:
                         P([e], !0)
                 }
             }, Z = async (e, t, n) => {
                 r(7, I = !0);
                 try {
                     console.debug(s, "installing selections from", e), await P(t.filter(Boolean), !0);
-                    const i = rv[rv.indexOf(e) + 1];
+                    const i = nv[nv.indexOf(e) + 1];
                     if (i)
                         if (n) {
                             const t = (await f.reconcile(e)).filter((e => e.matches.length)).map((({
                                 matches: [e]
                             }) => e));
                             await Z(i, t, !0)
                         } else r(15, C = i);
-                    else r(15, C = rv[rv.indexOf(e) || 0])
+                    else r(15, C = nv[nv.indexOf(e) || 0])
                 } finally {
                     r(7, I = !1)
                 }
             }, J = async () => {
                 r(7, I = !0);
                 try {
-                    const e = A.map(((e, t) => [e, x[t]])).filter((([e, t]) => e && !tv(e, t)));
-                    await B(e.map((([, e]) => e)), !1), await P(e.map((([e]) => e)), !1), r(1, m = xh.Installed)
+                    const e = A.map(((e, t) => [e, x[t]])).filter((([e, t]) => e && !rv(e, t)));
+                    await B(e.map((([, e]) => e)), !1), await P(e.map((([e]) => e)), !1), r(1, m = Ah.Installed)
                 } finally {
                     r(7, I = !1)
                 }
-            }, Y = e => !!d[e.source]?.strategies.includes(Br.VersionEq), K = () => {
-                r(5, S = Gn.cloneDeep(nv))
+            }, Y = e => !!d[e.source]?.strategies.includes(Ur.VersionEq), K = () => {
+                r(5, S = Zn.cloneDeep(iv))
             }, X = () => {
-                m === xh.Installed || m === xh.FilterInstalled ? r(9, g = ov(g)) : m === xh.Search && r(10, y = ov(y))
+                m === Ah.Installed || m === Ah.FilterInstalled ? r(9, g = sv(g)) : m === Ah.Search && r(10, y = sv(y))
             };
-        oe((async () => {
-            r(8, d = await f.listSources()), h = [...Object.keys(d), "http", "https"].map((e => `${e}:`)), await V(!0), k[xh.Installed].length || r(1, m = xh.Reconcile)
+        se((async () => {
+            r(8, d = await f.listSources()), h = [...Object.keys(d), "http", "https"].map((e => `${e}:`)), await V(!0), k[Ah.Installed].length || r(1, m = Ah.Reconcile)
         }));
         return e.$$set = e => {
             "profile" in e && r(39, s = e.profile), "isActive" in e && r(0, a = e.isActive), "statusMessage" in e && r(38, l = e.statusMessage)
         }, e.$$.update = () => {
-            10 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && m !== xh.Search && "" === $ && (console.debug(s, "resetting search state"), K()), 16 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (console.debug(s, "filter status changed, resetting search state"), K()), 8 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && r(5, S.fromAlias = (console.debug(s, "updating `searchFromAlias`"), h?.some((e => $.startsWith(e)))), S), 32 & e.$$.dirty[0] && r(14, D = !Gn.isEqual([S.sources, S.startDate, S.strategies], [nv.sources, nv.startDate, nv.strategies])), 2 & e.$$.dirty[0] && m === xh.Reconcile && r(15, C = rv[0]), 4 & e.$$.dirty[0] | 512 & e.$$.dirty[1] && (k[xh.Installed], r(2, k[xh.FilterInstalled] = k[xh.Installed].filter((([e]) => b.some((t => e.source === t.source && e.id === t.id)))), k)), 4 & e.$$.dirty[0] | 1024 & e.$$.dirty[1] && (k[xh.Installed], r(2, k[xh.Search] = w.map((e => {
-                const t = k[xh.Installed].find((([t]) => tv(t, e)));
+            10 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && m !== Ah.Search && "" === $ && (console.debug(s, "resetting search state"), K()), 16 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (console.debug(s, "filter status changed, resetting search state"), K()), 8 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && r(5, S.fromAlias = (console.debug(s, "updating `searchFromAlias`"), h?.some((e => $.startsWith(e)))), S), 32 & e.$$.dirty[0] && r(14, D = !Zn.isEqual([S.sources, S.startDate, S.strategies], [iv.sources, iv.startDate, iv.strategies])), 2 & e.$$.dirty[0] && m === Ah.Reconcile && r(15, C = nv[0]), 4 & e.$$.dirty[0] | 512 & e.$$.dirty[1] && (k[Ah.Installed], r(2, k[Ah.FilterInstalled] = k[Ah.Installed].filter((([e]) => b.some((t => e.source === t.source && e.id === t.id)))), k)), 4 & e.$$.dirty[0] | 1024 & e.$$.dirty[1] && (k[Ah.Installed], r(2, k[Ah.Search] = w.map((e => {
+                const t = k[Ah.Installed].find((([t]) => rv(t, e)));
                 if (t) {
                     const [r, , n] = t;
                     return [r, e, n]
                 }
                 return [e, e, !1]
-            })), k)), 4 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (k[xh.Installed], console.debug(s, "recounting updates"), r(11, p = k[xh.Installed].reduce(((e, [t, r]) => e + (r && t.version !== r.version ? 1 : 0)), 0))), 197 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (k[xh.Installed], console.debug(s, "updating status message"), a && r(38, l = L ? "refreshing…" : I ? "installing…" : `installed add-ons: ${k[xh.Installed].reduce(((e,[,,t])=>e+ +t),0)}`))
+            })), k)), 4 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (k[Ah.Installed], console.debug(s, "recounting updates"), r(11, p = k[Ah.Installed].reduce(((e, [t, r]) => e + (r && t.version !== r.version ? 1 : 0)), 0))), 197 & e.$$.dirty[0] | 256 & e.$$.dirty[1] && (k[Ah.Installed], console.debug(s, "updating status message"), a && r(38, l = L ? "refreshing…" : I ? "installing…" : `installed add-ons: ${k[Ah.Installed].reduce(((e,[,,t])=>e+ +t),0)}`))
         }, [a, m, k, $, O, S, L, I, d, g, y, p, _, T, D, C, R, A, N, q, E, u, P, j, B, U, V, z, H, () => {
             r(19, q = void 0)
         }, W, G, async e => {
             const t = await (async e => {
-                for (const [t, r] of Array.from(rv.entries()).slice(rv.indexOf(e))) {
+                for (const [t, r] of Array.from(nv.entries()).slice(nv.indexOf(e))) {
                     const e = await f.reconcile(r);
-                    if (e.some((e => e.matches.length)) || !(t + 1 in rv)) return [r, e]
+                    if (e.some((e => e.matches.length)) || !(t + 1 in nv)) return [r, e]
                 }
             })(e);
             if (t) {
                 r(15, [C] = t, C);
                 const [, e] = t;
                 return r(16, R = []), e
             }
@@ -24966,15 +24994,15 @@
             function(e) {
                 O = e, r(4, O)
             },
             function(e) {
                 C = e, r(15, C), r(1, m)
             }, () => U(), () => H(), () => V(), () => j(!0), () => Z(C, R), () => Z(C, R, !0), () => J(), () => X(),
             function(e) {
-                fe[e ? "unshift" : "push"]((() => {
+                he[e ? "unshift" : "push"]((() => {
                     E = e, r(20, E)
                 }))
             }, ({
                 detail: {
                     addon: e,
                     action: t
                 }
@@ -24990,296 +25018,295 @@
                 R = e, r(16, R)
             }, e => P([e]), e => j([e]), e => B([e], !1), e => z(e), (e, t, r, {
                 detail: {
                     mouseEvent: n
                 }
             }) => W(e ? t : r, e, n)]
     }
-    class av extends Ze {
+    class lv extends Ye {
         constructor(e) {
-            super(), Ge(this, e, sv, Xg, a, {
+            super(), Je(this, e, av, Qg, a, {
                 profile: 39,
                 isActive: 0,
                 statusMessage: 38
             }, null, [-1, -1, -1, -1])
         }
     }
 
-    function lv(e) {
+    function uv(e) {
         const t = e.slice(),
             r = t[0][t[1]];
         return t[7] = r, t
     }
 
-    function uv(e) {
-        let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, E, T = e[7].heading + "",
-            S = e[7].message + "";
-        return p = new Yn({
+    function cv(e) {
+        let t, r, n, i, s, a, l, u, c, f, h, p, d, m, g, v, y, b, w, _, k, x, A, q, T = e[7].heading + "",
+            $ = e[7].message + "";
+        return p = new Kn({
             props: {
-                icon: vn
+                icon: yn
             }
-        }), v = new Yn({
+        }), v = new Kn({
             props: {
-                icon: xn
+                icon: An
             }
-        }), w = new Yn({
+        }), w = new Kn({
             props: {
-                icon: gn
+                icon: vn
             }
         }), {
             c() {
-                t = D("div"), r = D("div"), n = D("div"), i = D("h1"), s = R(T), a = L(), l = D("p"), u = R(S), c = L(), f = D("div"), h = D("button"), Ve(p.$$.fragment), m = L(), g = D("button"), Ve(v.$$.fragment), y = L(), b = D("button"), Ve(w.$$.fragment), P(i, "class", "svelte-jtijg8"), P(n, "class", "current-alert svelte-jtijg8"), P(h, "title", "previous alert"), h.disabled = d = !(e[1] - 1 in e[0]), P(h, "class", "svelte-jtijg8"), P(g, "title", "dismiss alerts"), P(g, "class", "svelte-jtijg8"), P(b, "title", "next alert"), b.disabled = _ = !(e[1] + 1 in e[0]), P(b, "class", "svelte-jtijg8"), P(f, "class", "alert-nav svelte-jtijg8"), P(r, "class", "alerts svelte-jtijg8"), P(r, "role", "alert"), P(t, "class", "alerts-wrapper svelte-jtijg8")
+                t = C("div"), r = C("div"), n = C("div"), i = C("h1"), s = L(T), a = N(), l = C("p"), u = L($), c = N(), f = C("div"), h = C("button"), He(p.$$.fragment), m = N(), g = C("button"), He(v.$$.fragment), y = N(), b = C("button"), He(w.$$.fragment), j(i, "class", "svelte-jtijg8"), j(n, "class", "current-alert svelte-jtijg8"), j(h, "title", "previous alert"), h.disabled = d = !(e[1] - 1 in e[0]), j(h, "class", "svelte-jtijg8"), j(g, "title", "dismiss alerts"), j(g, "class", "svelte-jtijg8"), j(b, "title", "next alert"), b.disabled = _ = !(e[1] + 1 in e[0]), j(b, "class", "svelte-jtijg8"), j(f, "class", "alert-nav svelte-jtijg8"), j(r, "class", "alerts svelte-jtijg8"), j(r, "role", "alert"), j(t, "class", "alerts-wrapper svelte-jtijg8")
             },
             m(o, d) {
-                $(o, t, d), q(t, r), q(r, n), q(n, i), q(i, s), q(n, a), q(n, l), q(l, u), q(r, c), q(r, f), q(f, h), ze(p, h, null), q(f, m), q(f, g), ze(v, g, null), q(f, y), q(f, b), ze(w, b, null), x = !0, A || (E = [I(h, "click", e[5]), I(g, "click", e[2]), I(b, "click", e[6])], A = !0)
+                O(o, t, d), E(t, r), E(r, n), E(n, i), E(i, s), E(n, a), E(n, l), E(l, u), E(r, c), E(r, f), E(f, h), We(p, h, null), E(f, m), E(f, g), We(v, g, null), E(f, y), E(f, b), We(w, b, null), x = !0, A || (q = [F(h, "click", e[5]), F(g, "click", e[2]), F(b, "click", e[6])], A = !0)
             },
             p(e, t) {
-                (!x || 3 & t) && T !== (T = e[7].heading + "") && U(s, T), (!x || 3 & t) && S !== (S = e[7].message + "") && U(u, S), (!x || 3 & t && d !== (d = !(e[1] - 1 in e[0]))) && (h.disabled = d), (!x || 3 & t && _ !== (_ = !(e[1] + 1 in e[0]))) && (b.disabled = _)
+                (!x || 3 & t) && T !== (T = e[7].heading + "") && V(s, T), (!x || 3 & t) && $ !== ($ = e[7].message + "") && V(u, $), (!x || 3 & t && d !== (d = !(e[1] - 1 in e[0]))) && (h.disabled = d), (!x || 3 & t && _ !== (_ = !(e[1] + 1 in e[0]))) && (b.disabled = _)
             },
             i(e) {
-                x || (Oe(p.$$.fragment, e), Oe(v.$$.fragment, e), Oe(w.$$.fragment, e), ge((() => {
-                    x && (k || (k = Re(r, Ye, {
+                x || (Se(p.$$.fragment, e), Se(v.$$.fragment, e), Se(w.$$.fragment, e), e && ve((() => {
+                    x && (k || (k = Le(r, Xe, {
                         duration: 200
                     }, !0)), k.run(1))
                 })), x = !0)
             },
             o(e) {
-                Se(p.$$.fragment, e), Se(v.$$.fragment, e), Se(w.$$.fragment, e), k || (k = Re(r, Ye, {
+                De(p.$$.fragment, e), De(v.$$.fragment, e), De(w.$$.fragment, e), e && (k || (k = Le(r, Xe, {
                     duration: 200
-                }, !1)), k.run(0), x = !1
+                }, !1)), k.run(0)), x = !1
             },
             d(e) {
-                e && O(t), He(p), He(v), He(w), e && k && k.end(), A = !1, o(E)
+                e && S(t), Ge(p), Ge(v), Ge(w), e && k && k.end(), A = !1, o(q)
             }
         }
     }
 
-    function cv(e) {
-        let t, r, n = e[1] in e[0] && uv(lv(e));
+    function fv(e) {
+        let t, r, n = e[1] in e[0] && cv(uv(e));
         return {
             c() {
-                n && n.c(), t = N()
+                n && n.c(), t = I()
             },
             m(e, i) {
-                n && n.m(e, i), $(e, t, i), r = !0
+                n && n.m(e, i), O(e, t, i), r = !0
             },
             p(e, [r]) {
-                e[1] in e[0] ? n ? (n.p(lv(e), r), 3 & r && Oe(n, 1)) : (n = uv(lv(e)), n.c(), Oe(n, 1), n.m(t.parentNode, t)) : n && (Te(), Se(n, 1, 1, (() => {
+                e[1] in e[0] ? n ? (n.p(uv(e), r), 3 & r && Se(n, 1)) : (n = cv(uv(e)), n.c(), Se(n, 1), n.m(t.parentNode, t)) : n && ($e(), De(n, 1, 1, (() => {
                     n = null
-                })), $e())
+                })), Oe())
             },
             i(e) {
-                r || (Oe(n), r = !0)
+                r || (Se(n), r = !0)
             },
             o(e) {
-                Se(n), r = !1
+                De(n), r = !1
             },
             d(e) {
-                n && n.d(e), e && O(t)
+                e && S(t), n && n.d(e)
             }
         }
     }
 
-    function fv(e, t, r) {
+    function hv(e, t, r) {
         let n, i;
-        c(e, ln, (e => r(3, n = e))), c(e, tt, (e => r(4, i = e)));
+        c(e, un, (e => r(3, n = e))), c(e, nt, (e => r(4, i = e)));
         let o = [],
             s = 0;
         return e.$$.update = () => {
             24 & e.$$.dirty && (r(0, o = [i["*"], i[n]].filter(Boolean).flat()), r(1, s = 0))
         }, [o, s, () => {
-            v(tt, i = {}, i)
+            v(nt, i = {}, i)
         }, n, i, () => r(1, s -= 1), () => r(1, s += 1)]
     }
-    class hv extends Ze {
+    class pv extends Ye {
         constructor(e) {
-            super(), Ge(this, e, fv, cv, a, {})
+            super(), Je(this, e, hv, fv, a, {})
         }
     }
 
-    function pv(e, t, r) {
+    function dv(e, t, r) {
         const n = e.slice();
         return n[10] = t[r], n
     }
 
-    function dv(t) {
+    function mv(t) {
         return {
             c: e,
             m: e,
             p: e,
             i: e,
             o: e,
             d: e
         }
     }
 
-    function mv(e) {
+    function gv(e) {
         let t, r, n, i, o, s, a, l, u, c, f, h, p, d, m, g, v, y = (e[2] ? `${e[1]} < ${e[2]}` : e[1]) + "",
             b = [],
             w = new Map;
-        r = new pi({});
-        let _ = Object.keys(e[3]);
+        r = new di({});
+        let _ = Fe(Object.keys(e[3]));
         const k = e => e[10];
         for (let t = 0; t < _.length; t += 1) {
-            let r = pv(e, _, t),
+            let r = dv(e, _, t),
                 n = k(r);
-            w.set(n, b[t] = gv(n, r))
+            w.set(n, b[t] = vv(n, r))
         }
         return {
             c() {
-                t = D("header"), Ve(r.$$.fragment), n = L(), i = D("div"), o = D("b"), o.textContent = "instawow", s = D("br"), a = L(), l = D("span"), u = R(y), c = L(), f = D("main");
+                t = C("header"), He(r.$$.fragment), n = N(), i = C("div"), o = C("b"), o.textContent = "instawow", s = C("br"), a = N(), l = C("span"), u = L(y), c = N(), f = C("main");
                 for (let e = 0; e < b.length; e += 1) b[e].c();
-                h = L(), p = D("footer"), d = D("div"), m = R(e[0]), P(l, "class", "svelte-tax5nz"), P(i, "class", "instawow-version svelte-tax5nz"), P(t, "class", "section menubar svelte-tax5nz"), P(f, "class", "section main svelte-tax5nz"), P(d, "class", "status svelte-tax5nz"), P(p, "class", "section statusbar svelte-tax5nz")
+                h = N(), p = C("footer"), d = C("div"), m = L(e[0]), j(l, "class", "svelte-tax5nz"), j(i, "class", "instawow-version svelte-tax5nz"), j(t, "class", "section menubar svelte-tax5nz"), j(f, "class", "section main svelte-tax5nz"), j(d, "class", "status svelte-tax5nz"), j(p, "class", "section statusbar svelte-tax5nz")
             },
             m(e, g) {
-                $(e, t, g), ze(r, t, null), q(t, n), q(t, i), q(i, o), q(i, s), q(i, a), q(i, l), q(l, u), $(e, c, g), $(e, f, g);
+                O(e, t, g), We(r, t, null), E(t, n), E(t, i), E(i, o), E(i, s), E(i, a), E(i, l), E(l, u), O(e, c, g), O(e, f, g);
                 for (let e = 0; e < b.length; e += 1) b[e] && b[e].m(f, null);
-                $(e, h, g), $(e, p, g), q(p, d), q(d, m), v = !0
+                O(e, h, g), O(e, p, g), E(p, d), E(d, m), v = !0
             },
             p(e, t) {
-                (!v || 6 & t) && y !== (y = (e[2] ? `${e[1]} < ${e[2]}` : e[1]) + "") && U(u, y), 25 & t && (_ = Object.keys(e[3]), Te(), b = Pe(b, t, k, 1, e, _, w, f, Fe, gv, null, pv), $e()), (!v || 1 & t) && U(m, e[0])
+                (!v || 6 & t) && y !== (y = (e[2] ? `${e[1]} < ${e[2]}` : e[1]) + "") && V(u, y), 25 & t && (_ = Fe(Object.keys(e[3])), $e(), b = Be(b, t, k, 1, e, _, w, f, Pe, vv, null, dv), Oe()), (!v || 1 & t) && V(m, e[0])
             },
             i(e) {
                 if (!v) {
-                    Oe(r.$$.fragment, e);
-                    for (let e = 0; e < _.length; e += 1) Oe(b[e]);
-                    g || ge((() => {
-                        g = Ce(d, Ye, {}), g.start()
-                    })), v = !0
+                    Se(r.$$.fragment, e);
+                    for (let e = 0; e < _.length; e += 1) Se(b[e]);
+                    e && (g || ve((() => {
+                        g = Re(d, Xe, {}), g.start()
+                    }))), v = !0
                 }
             },
             o(e) {
-                Se(r.$$.fragment, e);
-                for (let e = 0; e < b.length; e += 1) Se(b[e]);
+                De(r.$$.fragment, e);
+                for (let e = 0; e < b.length; e += 1) De(b[e]);
                 v = !1
             },
             d(e) {
-                e && O(t), He(r), e && O(c), e && O(f);
-                for (let e = 0; e < b.length; e += 1) b[e].d();
-                e && O(h), e && O(p)
+                e && (S(t), S(c), S(f), S(h), S(p)), Ge(r);
+                for (let e = 0; e < b.length; e += 1) b[e].d()
             }
         }
     }
 
-    function gv(e, t) {
+    function vv(e, t) {
         let r, n, i, o;
 
         function s(e) {
             t[7](e)
         }
         let a = {
             profile: t[10],
             isActive: t[10] === t[4]
         };
-        return void 0 !== t[0] && (a.statusMessage = t[0]), n = new av({
+        return void 0 !== t[0] && (a.statusMessage = t[0]), n = new lv({
             props: a
-        }), fe.push((() => Ue(n, "statusMessage", s))), {
+        }), he.push((() => ze(n, "statusMessage", s))), {
             key: e,
             first: null,
             c() {
-                r = N(), Ve(n.$$.fragment), this.first = r
+                r = I(), He(n.$$.fragment), this.first = r
             },
             m(e, t) {
-                $(e, r, t), ze(n, e, t), o = !0
+                O(e, r, t), We(n, e, t), o = !0
             },
             p(e, r) {
                 t = e;
                 const o = {};
-                8 & r && (o.profile = t[10]), 24 & r && (o.isActive = t[10] === t[4]), !i && 1 & r && (i = !0, o.statusMessage = t[0], ve((() => i = !1))), n.$set(o)
+                8 & r && (o.profile = t[10]), 24 & r && (o.isActive = t[10] === t[4]), !i && 1 & r && (i = !0, o.statusMessage = t[0], ye((() => i = !1))), n.$set(o)
             },
             i(e) {
-                o || (Oe(n.$$.fragment, e), o = !0)
+                o || (Se(n.$$.fragment, e), o = !0)
             },
             o(e) {
-                Se(n.$$.fragment, e), o = !1
+                De(n.$$.fragment, e), o = !1
             },
             d(e) {
-                e && O(r), He(n, e)
+                e && S(r), Ge(n, e)
             }
         }
     }
 
-    function vv(t) {
+    function yv(t) {
         let r, n, i, o, s;
         return {
             c() {
-                r = D("header"), n = L(), i = D("main"), o = L(), s = D("footer"), s.innerHTML = '<div class="status svelte-tax5nz">loading…</div>', P(r, "class", "section menubar svelte-tax5nz"), P(i, "class", "section main svelte-tax5nz"), P(s, "class", "section statusbar svelte-tax5nz")
+                r = C("header"), n = N(), i = C("main"), o = N(), s = C("footer"), s.innerHTML = '<div class="status svelte-tax5nz">loading…</div>', j(r, "class", "section menubar svelte-tax5nz"), j(i, "class", "section main svelte-tax5nz"), j(s, "class", "section statusbar svelte-tax5nz")
             },
             m(e, t) {
-                $(e, r, t), $(e, n, t), $(e, i, t), $(e, o, t), $(e, s, t)
+                O(e, r, t), O(e, n, t), O(e, i, t), O(e, o, t), O(e, s, t)
             },
             p: e,
             i: e,
             o: e,
             d(e) {
-                e && O(r), e && O(n), e && O(i), e && O(o), e && O(s)
+                e && (S(r), S(n), S(i), S(o), S(s))
             }
         }
     }
 
-    function yv(e) {
+    function bv(e) {
         let t, r, n, i, o, s, a = {
             ctx: e,
             current: null,
             token: null,
             hasCatch: !1,
-            pending: vv,
-            then: mv,
-            catch: dv,
+            pending: yv,
+            then: gv,
+            catch: mv,
             blocks: [, , , ]
         };
-        return Le(e[6](), a), o = new hv({}), {
+        return Ne(e[6](), a), o = new pv({}), {
             c() {
-                t = D("style"), t.textContent = '.modal {\n  -webkit-backdrop-filter: blur(6px);\n  backdrop-filter: blur(6px);\n}\n\n.modal {\n  border-radius: 0.75em;\n  box-shadow: 0 1rem 3rem var(--inverse-color-alpha-10);\n}\n\n:root {\n  --base-color: rgb(236, 236, 236);\n  --base-color-tone-a: #f9f9f9;\n  --base-color-tone-a-alpha-85: rgba(249, 249, 249, 0.85);\n  --base-color-tone-b: rgba(19, 19, 19, 0.1);\n  --base-color-alpha-65: rgba(236, 236, 236, 0.65);\n  --inverse-color: #131313;\n  --inverse-color-alpha-05: rgba(19, 19, 19, 0.05);\n  --inverse-color-alpha-10: rgba(19, 19, 19, 0.1);\n  --inverse-color-alpha-20: rgba(19, 19, 19, 0.2);\n  --inverse-color-tone-a: #2d2d2d;\n  --inverse-color-tone-b: #464646;\n  --dropdown-arrow: url(\'data:image/svg+xml;utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="%23131313" d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"></path></svg>\');\n  --alert-background-color: rgba(250, 128, 114, 0.5);\n}\n\n@media (prefers-color-scheme: dark) {\n  :root {\n    --base-color: rgb(51, 54, 55);\n    --base-color-tone-a: #2e3132;\n    --base-color-tone-a-alpha-85: rgba(46, 49, 50, 0.85);\n    --base-color-tone-b: #1a1c1d;\n    --base-color-alpha-65: rgba(51, 54, 55, 0.65);\n    --inverse-color: #ccc9c8;\n    --inverse-color-alpha-05: rgba(204, 201, 200, 0.05);\n    --inverse-color-alpha-10: rgba(204, 201, 200, 0.1);\n    --inverse-color-alpha-20: rgba(204, 201, 200, 0.2);\n    --inverse-color-tone-a: #c0bcbb;\n    --inverse-color-tone-b: #b3afae;\n    --dropdown-arrow: url(\'data:image/svg+xml;utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="%23ccc9c8" d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"></path></svg>\');\n  }\n}\n*,\n*::before,\n*::after {\n  box-sizing: border-box;\n}\n\n:root {\n  color-scheme: light dark;\n}\n\n:focus {\n  outline-style: none;\n}\n\nbody {\n  color: var(--inverse-color);\n  margin: 0;\n  font-family: -apple-system, system-ui;\n  overflow: hidden;\n}\n\ninput,\nbutton,\nselect,\ntextarea {\n  font: inherit;\n  background-color: inherit;\n  color: inherit;\n}\n\na {\n  text-decoration: none;\n}\n\nbutton[role=link] {\n  background-color: var(--inverse-color-alpha-05);\n  margin: 0;\n  padding: 0 0.2rem;\n  border: none;\n  border-radius: 3px;\n  cursor: pointer;\n  transition: background-color 0.2s;\n}\nbutton[role=link]:hover {\n  background-color: var(--inverse-color-alpha-10);\n}\n\nmenu,\nnav {\n  -webkit-user-select: none;\n  user-select: none;\n}\n\nselect {\n  -webkit-appearance: none;\n  appearance: none;\n}\nselect:disabled {\n  pointer-events: none;\n}\n\ncode {\n  -webkit-user-select: text;\n  user-select: text;\n}\n\n.modal {\n  background: none;\n  position: unset;\n  max-width: 75vw;\n  padding: 0;\n  border: 0;\n  color: var(--inverse-color);\n}\n.modal .content,\n.modal .title-bar {\n  padding: 1.25rem;\n  background-color: var(--base-color-alpha-65);\n}\n.modal .title-bar {\n  padding: 0.65rem 1.25rem;\n  border-radius: 0.75em 0.75em 0 0;\n  background-color: var(--inverse-color-alpha-10);\n  font-size: 0.9em;\n  font-weight: 600;\n}\n.modal .content {\n  border-radius: 0 0 0.75em 0.75em;\n}\n.modal .content:first-child {\n  border-radius: 0.75em;\n}\n.modal label {\n  line-height: 1.75em;\n}\n.modal .form-control {\n  display: flex;\n  align-items: center;\n  width: 100%;\n  line-height: 1.75em;\n  margin: 0;\n  padding: 0 0.5em;\n  border: 0;\n  border-radius: 0.4375em;\n  background-color: var(--inverse-color-alpha-10);\n  transition: background-color 0.2s;\n}\n.modal .form-control:disabled {\n  opacity: 0.5;\n}\n.modal .form-control:focus {\n  background-color: var(--inverse-color-alpha-20);\n}\n.modal .form-control.error {\n  background-color: salmon;\n}\n.modal .form-control .icon {\n  height: 1rem;\n  width: 1rem;\n  fill: var(--inverse-color-tone-b);\n  vertical-align: text-bottom;\n}\n.modal button.form-control {\n  justify-content: center;\n  font-weight: 500;\n}\n.modal button.form-control.primary, .modal button.form-control[type=submit] {\n  background-color: rgb(24, 136, 255);\n  color: #efefef;\n}\n.modal button.form-control.primary:focus, .modal button.form-control[type=submit]:focus {\n  background-color: rgb(0, 104, 217);\n}\n.modal select.form-control {\n  min-width: 12rem;\n}\n.modal select.form-control:not([multiple]) {\n  padding-right: 1.25rem;\n  background-image: var(--dropdown-arrow);\n  background-size: 10px;\n  background-repeat: no-repeat;\n  background-position: top 9px right 7px;\n}\n.modal select.form-control[multiple] {\n  padding-top: 0.35rem;\n  padding-bottom: 0.35rem;\n}\n.modal .row + .row {\n  margin-top: 0.5rem;\n}\n.modal .input-array {\n  display: flex;\n}\n.modal .input-array .form-control {\n  margin: 0;\n  border-radius: 0.2916666667em;\n}\n.modal .input-array .form-control + button,\n.modal .input-array .form-control + input {\n  margin-left: 4px;\n}\n.modal .input-array button.form-control {\n  width: auto;\n}\n.modal .input-array > :first-child {\n  flex-grow: 1;\n  border-top-left-radius: 0.4375em;\n  border-bottom-left-radius: 0.4375em;\n}\n.modal .input-array > :last-child {\n  border-top-right-radius: 0.4375em;\n  border-bottom-right-radius: 0.4375em;\n}\n.modal .error-text {\n  line-height: 1;\n  color: salmon;\n  font-size: 0.9em;\n}\n.modal .error-text :not(:first-child) {\n  padding-top: 0.25rem;\n}', r = L(), n = D("div"), a.block.c(), i = L(), Ve(o.$$.fragment), P(t, "lang", "scss"), P(n, "class", "wrapper svelte-tax5nz"), P(n, "style", e[5]())
+                t = C("style"), t.textContent = '.modal {\n  -webkit-backdrop-filter: blur(6px);\n  backdrop-filter: blur(6px);\n}\n\n.modal {\n  border-radius: 0.75em;\n  box-shadow: 0 1rem 3rem var(--inverse-color-alpha-10);\n}\n\n:root {\n  --base-color: rgb(236, 236, 236);\n  --base-color-tone-a: #f9f9f9;\n  --base-color-tone-a-alpha-85: rgba(249, 249, 249, 0.85);\n  --base-color-tone-b: rgba(19, 19, 19, 0.1);\n  --base-color-alpha-65: rgba(236, 236, 236, 0.65);\n  --inverse-color: #131313;\n  --inverse-color-alpha-05: rgba(19, 19, 19, 0.05);\n  --inverse-color-alpha-10: rgba(19, 19, 19, 0.1);\n  --inverse-color-alpha-20: rgba(19, 19, 19, 0.2);\n  --inverse-color-tone-a: #2d2d2d;\n  --inverse-color-tone-b: #464646;\n  --dropdown-arrow: url(\'data:image/svg+xml;utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="%23131313" d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"></path></svg>\');\n  --alert-background-color: rgba(250, 128, 114, 0.5);\n}\n\n@media (prefers-color-scheme: dark) {\n  :root {\n    --base-color: rgb(51, 54, 55);\n    --base-color-tone-a: #2e3132;\n    --base-color-tone-a-alpha-85: rgba(46, 49, 50, 0.85);\n    --base-color-tone-b: #1a1c1d;\n    --base-color-alpha-65: rgba(51, 54, 55, 0.65);\n    --inverse-color: #ccc9c8;\n    --inverse-color-alpha-05: rgba(204, 201, 200, 0.05);\n    --inverse-color-alpha-10: rgba(204, 201, 200, 0.1);\n    --inverse-color-alpha-20: rgba(204, 201, 200, 0.2);\n    --inverse-color-tone-a: #c0bcbb;\n    --inverse-color-tone-b: #b3afae;\n    --dropdown-arrow: url(\'data:image/svg+xml;utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="%23ccc9c8" d="M224 416c-8.188 0-16.38-3.125-22.62-9.375l-192-192c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0L224 338.8l169.4-169.4c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25l-192 192C240.4 412.9 232.2 416 224 416z"></path></svg>\');\n  }\n}\n*,\n*::before,\n*::after {\n  box-sizing: border-box;\n}\n\n:root {\n  color-scheme: light dark;\n}\n\n:focus {\n  outline-style: none;\n}\n\nbody {\n  color: var(--inverse-color);\n  margin: 0;\n  font-family: -apple-system, system-ui;\n  overflow: hidden;\n}\n\ninput,\nbutton,\nselect,\ntextarea {\n  font: inherit;\n  background-color: inherit;\n  color: inherit;\n}\n\na {\n  text-decoration: none;\n}\n\nbutton[role=link] {\n  background-color: var(--inverse-color-alpha-05);\n  margin: 0;\n  padding: 0 0.2rem;\n  border: none;\n  border-radius: 3px;\n  cursor: pointer;\n  transition: background-color 0.2s;\n}\nbutton[role=link]:hover {\n  background-color: var(--inverse-color-alpha-10);\n}\n\nmenu,\nnav {\n  -webkit-user-select: none;\n  user-select: none;\n}\n\nselect {\n  -webkit-appearance: none;\n  appearance: none;\n}\nselect:disabled {\n  pointer-events: none;\n}\n\ncode {\n  -webkit-user-select: text;\n  user-select: text;\n}\n\n.modal {\n  background: none;\n  position: unset;\n  max-width: 75vw;\n  padding: 0;\n  border: 0;\n  color: var(--inverse-color);\n}\n.modal .content,\n.modal .title-bar {\n  padding: 1.25rem;\n  background-color: var(--base-color-alpha-65);\n}\n.modal .title-bar {\n  padding: 0.65rem 1.25rem;\n  border-radius: 0.75em 0.75em 0 0;\n  background-color: var(--inverse-color-alpha-10);\n  font-size: 0.9em;\n  font-weight: 600;\n}\n.modal .content {\n  border-radius: 0 0 0.75em 0.75em;\n}\n.modal .content:first-child {\n  border-radius: 0.75em;\n}\n.modal label {\n  line-height: 1.75em;\n}\n.modal .form-control {\n  display: flex;\n  align-items: center;\n  width: 100%;\n  line-height: 1.75em;\n  margin: 0;\n  padding: 0 0.5em;\n  border: 0;\n  border-radius: 0.4375em;\n  background-color: var(--inverse-color-alpha-10);\n  transition: background-color 0.2s;\n}\n.modal .form-control:disabled {\n  opacity: 0.5;\n}\n.modal .form-control:focus {\n  background-color: var(--inverse-color-alpha-20);\n}\n.modal .form-control.error {\n  background-color: salmon;\n}\n.modal .form-control .icon {\n  height: 1rem;\n  width: 1rem;\n  fill: var(--inverse-color-tone-b);\n  vertical-align: text-bottom;\n}\n.modal button.form-control {\n  justify-content: center;\n  font-weight: 500;\n}\n.modal button.form-control.primary, .modal button.form-control[type=submit] {\n  background-color: rgb(24, 136, 255);\n  color: #efefef;\n}\n.modal button.form-control.primary:focus, .modal button.form-control[type=submit]:focus {\n  background-color: rgb(0, 104, 217);\n}\n.modal select.form-control {\n  min-width: 12rem;\n}\n.modal select.form-control:not([multiple]) {\n  padding-right: 1.25rem;\n  background-image: var(--dropdown-arrow);\n  background-size: 10px;\n  background-repeat: no-repeat;\n  background-position: top 9px right 7px;\n}\n.modal select.form-control[multiple] {\n  padding-top: 0.35rem;\n  padding-bottom: 0.35rem;\n}\n.modal .row + .row {\n  margin-top: 0.5rem;\n}\n.modal .input-array {\n  display: flex;\n}\n.modal .input-array .form-control {\n  margin: 0;\n  border-radius: 0.2916666667em;\n}\n.modal .input-array .form-control + button,\n.modal .input-array .form-control + input {\n  margin-left: 4px;\n}\n.modal .input-array button.form-control {\n  width: auto;\n}\n.modal .input-array > :first-child {\n  flex-grow: 1;\n  border-top-left-radius: 0.4375em;\n  border-bottom-left-radius: 0.4375em;\n}\n.modal .input-array > :last-child {\n  border-top-right-radius: 0.4375em;\n  border-bottom-right-radius: 0.4375em;\n}\n.modal .error-text {\n  line-height: 1;\n  color: salmon;\n  font-size: 0.9em;\n}\n.modal .error-text :not(:first-child) {\n  padding-top: 0.25rem;\n}', r = N(), n = C("div"), a.block.c(), i = N(), He(o.$$.fragment), j(t, "lang", "scss"), j(n, "class", "wrapper svelte-tax5nz"), j(n, "style", e[5]())
             },
             m(e, l) {
-                q(document.head, t), $(e, r, l), $(e, n, l), a.block.m(n, a.anchor = null), a.mount = () => n, a.anchor = i, q(n, i), ze(o, n, null), s = !0
+                E(document.head, t), O(e, r, l), O(e, n, l), a.block.m(n, a.anchor = null), a.mount = () => n, a.anchor = i, E(n, i), We(o, n, null), s = !0
             },
             p(t, [r]) {
-                Ne(a, e = t, r)
+                Ie(a, e = t, r)
             },
             i(e) {
-                s || (Oe(a.block), Oe(o.$$.fragment, e), s = !0)
+                s || (Se(a.block), Se(o.$$.fragment, e), s = !0)
             },
             o(e) {
                 for (let e = 0; e < 3; e += 1) {
-                    Se(a.blocks[e])
+                    De(a.blocks[e])
                 }
-                Se(o.$$.fragment, e), s = !1
+                De(o.$$.fragment, e), s = !1
             },
             d(e) {
-                O(t), e && O(r), e && O(n), a.block.d(), a.token = null, a = null, He(o)
+                e && (S(r), S(n)), S(t), a.block.d(), a.token = null, a = null, Ge(o)
             }
         }
     }
 
-    function bv(e, t, r) {
+    function wv(e, t, r) {
         let n, i, o;
-        c(e, an, (e => r(3, n = e))), c(e, ln, (e => r(4, i = e))), c(e, nn, (e => r(8, o = e)));
+        c(e, ln, (e => r(3, n = e))), c(e, un, (e => r(4, i = e))), c(e, on, (e => r(8, o = e)));
         const s = ["#dd0531", "#007fff", "#f9e64f", "#1857a4", "#215732", "#61dafb", "#832561", "#ff3d00", "#42b883"];
         let a, l, u = " ";
         return [u, a, l, n, i, () => {
             const e = Math.max(0, Math.round(Math.random() * s.length) - 1);
             return `\n      --random-border-color: ${s[e]};\n    `
         }, async () => {
                 r(1, ({
                     installed_version: a,
                     new_version: l
                 } = await o.getVersion()), a, r(2, l));
                 const e = await o.listProfiles(),
                     t = await Promise.allSettled(e.map((e => o.readProfile(e))));
-                v(an, n = Object.fromEntries(t.filter((e => "fulfilled" === e.status)).map((({
+                v(ln, n = Object.fromEntries(t.filter((e => "fulfilled" === e.status)).map((({
                     value: e
-                }) => [e.profile, e]))), n), v(ln, [i] = Object.keys(n), i)
+                }) => [e.profile, e]))), n), v(un, [i] = Object.keys(n), i)
             },
             function(e) {
                 u = e, r(0, u)
             }]
     }
-    return new class extends Ze {
+    return new class extends Ye {
         constructor(e) {
-            super(), Ge(this, e, bv, yv, a, {})
+            super(), Je(this, e, wv, bv, a, {})
         }
     }({
         target: document.body
     })
 }();
```

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/json_rpc_server.py` & `instawow-3.0.1/gui-webview/src/instawow_gui/json_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 from collections.abc import Awaitable, Callable, Iterator, Set
 from contextlib import AsyncExitStack, contextmanager
 from datetime import datetime
 from functools import partial
 from itertools import chain
 from pathlib import Path
-from typing import Any, Literal, TypeVar, cast
+from typing import Any, Literal, TypeVar
 
 import aiohttp
 import aiohttp.typedefs
 import aiohttp.web
 import anyio
 import cattrs
 import click
@@ -77,17 +77,14 @@
 
 
 def _transform_validation_errors(
     exc: cattrs.ClassValidationError | cattrs.IterableValidationError | BaseException,
     path: tuple[str | int, ...] = (),
 ) -> Iterator[_ValidationErrorResponse]:
     if isinstance(exc, cattrs.IterableValidationError):
-        exc = cast(
-            cattrs.IterableValidationError, exc
-        )  # FIXME: Rm once a new ver of cattrs is out
         with_notes, _ = exc.group_exceptions()
         for exc, note in with_notes:
             new_path = (*path, note.index)
             if isinstance(exc, (cattrs.ClassValidationError, cattrs.IterableValidationError)):
                 yield from _transform_validation_errors(exc, new_path)
             else:
                 yield {
```

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns` & `instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.icns`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico` & `instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.ico`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/gui-webview/src/instawow_gui/resources/instawow_gui.png` & `instawow-3.0.1/gui-webview/src/instawow_gui/resources/instawow_gui.png`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/pyproject.toml` & `instawow-3.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 substitution.files = ["src/instawow/_version.py"]
 
 [tool.poetry]
 name = "instawow"
-version = "3.0.0"
+version = "3.0.1"
 description = "World of Warcraft add-on manager"
 license = "GPL-3.0-or-later"
 authors = [
   "layday <layday@protonmail.com>",
 ]
 readme = "README.rst"
 urls.homepage = "http://github.com/layday/instawow"
@@ -98,15 +98,14 @@
   "UP",  # pyupgrade
   "W",   # pycodestyle
   "YTT", # flake8-2020
 ]
 ignore = [
   "E501",   # pycodestyle: line-too-long
   "TRY003", # tryceratops: raise-vanilla-args
-  "UP007",  # pyupgrade: non-pep604-annotation; enable after raising the min Python version to 3.10
 ]
 line-length = 99
 target-version = "py39"
 
 [tool.ruff.per-file-ignores]
 "**.py" = [
   "PYI",
@@ -129,14 +128,18 @@
   "instawow",
   "instawow_gui",
 ]
 required-imports = [
   "from __future__ import annotations",
 ]
 
+[tool.ruff.pyupgrade]
+keep-runtime-typing = true
+
+
 [tool.black]
 line-length = 99
 skip-string-normalization = true
 target-version = ["py39", "py310", "py311"]
 
 
 [tool.coverage.run]
```

### Comparing `instawow-3.0.0/src/instawow/_addon_hashing.py` & `instawow-3.0.1/src/instawow/_addon_hashing.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_cli_prompts.py` & `instawow-3.0.1/src/instawow/_cli_prompts.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_custom_slpp.py` & `instawow-3.0.1/src/instawow/_custom_slpp.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_http_cache_db.py` & `instawow-3.0.1/src/instawow/_http_cache_db.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_import_wrapper.py` & `instawow-3.0.1/src/instawow/_import_wrapper.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/alembic.ini` & `instawow-3.0.1/src/instawow/_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/env.py` & `instawow-3.0.1/src/instawow/_migrations/env.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py` & `instawow-3.0.1/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py` & `instawow-3.0.1/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py` & `instawow-3.0.1/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py` & `instawow-3.0.1/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py` & `instawow-3.0.1/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py` & `instawow-3.0.1/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py` & `instawow-3.0.1/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py` & `instawow-3.0.1/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py` & `instawow-3.0.1/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py` & `instawow-3.0.1/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py` & `instawow-3.0.1/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py` & `instawow-3.0.1/src/instawow/_migrations/versions/e13430219249_add_cascade.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py` & `instawow-3.0.1/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py` & `instawow-3.0.1/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py` & `instawow-3.0.1/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_sources/cfcore.py` & `instawow-3.0.1/src/instawow/_sources/cfcore.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_sources/github.py` & `instawow-3.0.1/src/instawow/_sources/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # Not exhaustive (as you might've guessed).  Reference:
 # https://docs.github.com/en/rest/reference/repos
 class _GithubRepo(TypedDict):
     id: int  # Unique, stable repository ID
     name: str  # the repo in user-or-org/repo
     full_name: str  # user-or-org/repo
     description: str | None
+    url: str
     html_url: str
 
 
 class _GithubRelease(TypedDict):
     tag_name: str  # Hopefully the version
     published_at: str  # ISO datetime
     assets: list[_GithubRelease_Asset]
@@ -86,15 +87,15 @@
             }
         ),
         changelog_format=ChangelogFormat.Markdown,
         addon_toc_key=None,
     )
     requires_access_token = None
 
-    _repos_api_url = URL('https://api.github.com/repos')
+    _api_url = URL('https://api.github.com/')
 
     _generated_catalogue_csv_url = (
         'https://raw.githubusercontent.com/layday/github-wow-addon-catalogue/main/addons.csv'
     )
 
     @classmethod
     def get_alias_from_url(cls, url: URL) -> str | None:
@@ -329,28 +330,36 @@
             None,
         )
         return matching_asset
 
     async def resolve_one(self, defn: Defn, metadata: None) -> pkg_models.Pkg:
         github_headers = await self.make_request_headers()
 
-        repo_url = self._repos_api_url / defn.alias
+        if (
+            defn.id
+            # Back compat; ID used to be equal to the full name.
+            and defn.id.isdigit()
+        ):
+            repo_url = self._api_url / 'repositories' / defn.id
+        else:
+            repo_url = self._api_url / 'repos' / defn.alias
+
         async with self._manager.web_client.get(
             repo_url, expire_after=timedelta(hours=1), headers=github_headers
         ) as response:
             if response.status == 404:
                 raise R.PkgNonexistent
             response.raise_for_status()
             project: _GithubRepo = await response.json()
 
         if defn.strategies.version_eq:
-            release_url = repo_url / 'releases/tags' / defn.strategies.version_eq
+            release_url = URL(project['url']) / 'releases/tags' / defn.strategies.version_eq
         else:
             # Includes pre-releases
-            release_url = (repo_url / 'releases').with_query(
+            release_url = (URL(project['url']) / 'releases').with_query(
                 # Default is 30 but we're more conservative
                 per_page='10'
             )
 
         async with self._manager.web_client.get(
             release_url, expire_after=timedelta(minutes=5), headers=github_headers
         ) as response:
```

### Comparing `instawow-3.0.0/src/instawow/_sources/instawow.py` & `instawow-3.0.1/src/instawow/_sources/instawow.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 from .. import results as R
 from ..cataloguer import CatalogueEntry
 from ..common import ChangelogFormat, Defn, Flavour, SourceMetadata
 from ..http import ClientSessionType
 from ..resolvers import BaseResolver
 from ..utils import run_in_thread
 
+_ADDONS = {
+    ('0', 'weakauras-companion'),
+    ('1', 'weakauras-companion-autoupdate'),
+}
+
 
 class InstawowResolver(BaseResolver):
     metadata = SourceMetadata(
         id='instawow',
         name='instawow',
         strategies=frozenset(),
         changelog_format=ChangelogFormat.Markdown,
         addon_toc_key=None,
     )
     requires_access_token = None
 
-    _ADDONS = {
-        ('0', 'weakauras-companion'),
-        ('1', 'weakauras-companion-autoupdate'),
-    }
-
     async def resolve_one(self, defn: Defn, metadata: None) -> pkg_models.Pkg:
         try:
-            source_id, slug = next(p for p in self._ADDONS if defn.alias in p)
+            source_id, slug = next(p for p in _ADDONS if defn.alias in p)
         except StopIteration:
             raise R.PkgNonexistent
 
         from ..wa_updater import WaCompanionBuilder
 
         builder = WaCompanionBuilder(self._manager)
         if source_id == '1':
```

### Comparing `instawow-3.0.0/src/instawow/_sources/tukui.py` & `instawow-3.0.1/src/instawow/_sources/tukui.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_sources/wago.py` & `instawow-3.0.1/src/instawow/_sources/wago.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_sources/wowi.py` & `instawow-3.0.1/src/instawow/_sources/wowi.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_version.py` & `instawow-3.0.1/src/instawow/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import timedelta
 
 from typing_extensions import TypedDict
 
 from . import config
 
-__version__ = '3.0.0'
+__version__ = '3.0.1'
 
 
 class _SimpleApiProject(TypedDict):
     versions: list[str]
 
 
 async def is_outdated(global_config: config.GlobalConfig) -> tuple[bool, str]:
```

### Comparing `instawow-3.0.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion` & `instawow-3.0.1/src/instawow/_wa_templates/COPYING.WeakAuras-Companion`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/_wa_templates/init.lua` & `instawow-3.0.1/src/instawow/_wa_templates/init.lua`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/cataloguer.py` & `instawow-3.0.1/src/instawow/cataloguer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Set
 from datetime import datetime
 from functools import cached_property
 from typing import Any
 
-from attrs import frozen
+from attrs import field, frozen
 from cattrs import Converter
 from cattrs.preconf.json import configure_converter
 from typing_extensions import Self
 
 from .config import Flavour
 from .utils import bucketise, normalise_names
 
@@ -37,16 +37,16 @@
 class CatalogueEntry(AddonKey):
     slug: str = ''
     name: str
     url: str
     game_flavours: frozenset[Flavour]
     download_count: int
     last_updated: datetime
-    folders: list[frozenset[str]] = []
-    same_as: list[AddonKey] = []
+    folders: list[frozenset[str]] = field(factory=list)
+    same_as: list[AddonKey] = field(factory=list)
 
 
 @frozen(kw_only=True)
 class ComputedCatalogueEntry(CatalogueEntry):
     normalised_name: str
     derived_download_score: float
```

### Comparing `instawow-3.0.0/src/instawow/cli.py` & `instawow-3.0.1/src/instawow/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import enum
+import sys
 import textwrap
 from collections.abc import Awaitable, Callable, Collection, Iterable, Mapping, Sequence
 from datetime import datetime, timezone
 from functools import cached_property, partial
 from itertools import chain, repeat
 from pathlib import Path
 from typing import Any, Generic, NoReturn, TypeVar, overload
@@ -25,36 +26,50 @@
 from .plugins import load_plugins
 from .utils import StrEnum, all_eq, gather, reveal_folder, tabulate, uniq
 
 _T = TypeVar('_T')
 _TStrEnum = TypeVar('_TStrEnum', bound=StrEnum)
 
 
+def _patch_asyncio():
+    # See https://github.com/aio-libs/aiohttp/issues/4324.
+    # We are not using pipes on Windows or async subprocesses so it's ok
+    # to just override the loop policy.
+    if sys.platform == 'win32' and sys.version_info < (3, 10):
+        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+
+
+@logger.catch(reraise=True)
+def main(*args: Any, **kwargs: Any) -> None:
+    _patch_asyncio()
+    cli(*args, **kwargs)
+
+
 class Report:
     SUCCESS_SYMBOL = click.style('✓', fg='green')
     FAILURE_SYMBOL = click.style('✗', fg='red')
     WARNING_SYMBOL = click.style('!', fg='blue')
 
     def __init__(
         self,
-        results: Iterable[tuple[Defn, R.ManagerResult]],
-        filter_fn: Callable[[R.ManagerResult], bool] = lambda _: True,
+        results: Iterable[tuple[Defn, R.Result]],
+        filter_fn: Callable[[R.Result], bool] = lambda _: True,
     ) -> None:
         self.results = list(results)
         self.filter_fn = filter_fn
 
     @property
     def exit_code(self) -> int:
         return any(
             isinstance(r, (R.ManagerError, R.InternalError)) and self.filter_fn(r)
             for _, r in self.results
         )
 
     @classmethod
-    def _result_type_to_symbol(cls, result: R.ManagerResult) -> str:
+    def _result_type_to_symbol(cls, result: R.Result) -> str:
         if isinstance(result, R.InternalError):
             return cls.WARNING_SYMBOL
         elif isinstance(result, R.ManagerError):
             return cls.FAILURE_SYMBOL
         else:
             return cls.SUCCESS_SYMBOL
 
@@ -270,15 +285,19 @@
 def _parse_debug_option(
     _: click.Context, __: click.Parameter, value: float
 ) -> tuple[bool, bool, bool]:
     return (value > 0, value > 1, value > 2)
 
 
 @_register_plugin_commands
-@click.group(context_settings={'help_option_names': ('-h', '--help')})
+@click.group(
+    # Redundant; overload w/out type var default remains unsolved: https://github.com/pallets/click/issues/2558
+    cls=None,
+    context_settings={'help_option_names': ('-h', '--help')},
+)
 @click.version_option(__version__, prog_name=__spec__.parent)
 @click.option(
     '--debug',
     '-d',
     count=True,
     help='Log incrementally more things.  Additive.',
     callback=_parse_debug_option,
@@ -297,17 +316,14 @@
 )
 @click.pass_context
 def cli(ctx: click.Context, **__: object) -> None:
     "Add-on manager for World of Warcraft."
     ctx.obj = _CtxObjWrapper(ctx)
 
 
-main = logger.catch(reraise=True)(cli)
-
-
 @overload
 def _parse_uri(
     manager: _manager.Manager,
     value: str,
     *,
     raise_invalid: bool = True,
     include_strategies: bool = False,
@@ -418,15 +434,15 @@
     addons: Sequence[Defn],
     retain_strategies: bool,
     dry_run: bool,
 ) -> None:
     "Update installed add-ons."
     import sqlalchemy as sa
 
-    def filter_results(result: R.ManagerResult):
+    def filter_results(result: R.Result):
         # Hide packages from output if they are up to date
         # and ``update`` was invoked without args,
         # provided that they are not pinned
         if addons or not isinstance(result, R.PkgUpToDate):
             return True
         else:
             return result.is_pinned
```

### Comparing `instawow-3.0.0/src/instawow/common.py` & `instawow-3.0.1/src/instawow/common.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/config.py` & `instawow-3.0.1/src/instawow/config.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/github_auth.py` & `instawow-3.0.1/src/instawow/github_auth.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/http.py` & `instawow-3.0.1/src/instawow/http.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/manager.py` & `instawow-3.0.1/src/instawow/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, contextmanager
 from datetime import datetime, timedelta
 from functools import cached_property, lru_cache, wraps
 from itertools import chain, filterfalse, product, repeat, starmap
 from pathlib import Path, PurePath
 from shutil import move
 from tempfile import NamedTemporaryFile
-from typing import Literal, NoReturn, TypeVar
+from typing import Literal, TypeVar
 
 import sqlalchemy as sa
 from attrs import evolve
 from loguru import logger
-from typing_extensions import Concatenate, ParamSpec, Self, TypeAlias
+from typing_extensions import Concatenate, Never, ParamSpec, Self, TypeAlias
 from yarl import URL
 
 from . import http, pkg_db, pkg_models
 from . import results as R
 from ._sources.cfcore import CfCoreResolver
 from ._sources.github import GithubResolver
 from ._sources.instawow import InstawowResolver
@@ -62,34 +62,32 @@
     trash,
     uniq,
 )
 from .utils import run_in_thread as t
 
 _P = ParamSpec('_P')
 _T = TypeVar('_T')
-_ResultOrError: TypeAlias = '_T | R.ManagerError | R.InternalError'
 
 _AsyncNamedTemporaryFile = t(NamedTemporaryFile)
 _move_async = t(move)
 
 
-_ERROR_CLASSES = (R.ManagerError, R.InternalError)
-
-
 def bucketise_results(
-    value: Iterable[tuple[Defn, _ResultOrError[_T]]],
-) -> tuple[Mapping[Defn, _T], Mapping[Defn, _ResultOrError[NoReturn]]]:
-    def get_bucket_dict(key: bool):
-        return dict(buckets.get(key, ()))
-
-    buckets = bucketise(value, lambda v: isinstance(v[1], _ERROR_CLASSES))
-    return (
-        get_bucket_dict(False),
-        get_bucket_dict(True),
-    )  # pyright: ignore[reportGeneralTypeIssues]
+    values: Iterable[tuple[Defn, R.AnyResult[_T]]],
+) -> tuple[Mapping[Defn, _T], Mapping[Defn, R.AnyResult[Never]]]:
+    ts: dict[Defn, _T] = {}
+    errors: dict[Defn, R.AnyResult[Never]] = {}
+
+    for defn, value in values:
+        if isinstance(value, (R.ManagerError, R.InternalError)):
+            errors[defn] = value
+        else:
+            ts[defn] = value
+
+    return ts, errors
 
 
 @asynccontextmanager
 async def _open_temp_writer_async():
     fh = await _AsyncNamedTemporaryFile(delete=False)
     path = Path(fh.name)
     try:
@@ -114,24 +112,24 @@
         names = archive.namelist()
         base_dirs = {h for _, h in find_addon_zip_tocs(names)}
         yield (base_dirs, extract)
 
 
 @object.__new__
 class _DummyResolver:
-    async def resolve(self, defns: Sequence[Defn]) -> dict[Defn, _ResultOrError[pkg_models.Pkg]]:
+    async def resolve(self, defns: Sequence[Defn]) -> dict[Defn, R.AnyResult[pkg_models.Pkg]]:
         return dict.fromkeys(defns, R.PkgSourceInvalid())
 
     async def get_changelog(self, uri: URL) -> str:
         raise R.PkgSourceInvalid
 
 
 async def capture_manager_exc_async(
     awaitable: Awaitable[_T],
-) -> _ResultOrError[_T]:
+) -> R.AnyResult[_T]:
     "Capture and log an exception raised in a coroutine."
     from aiohttp import ClientError
 
     try:
         return await awaitable
     except (R.ManagerError, R.InternalError) as error:
         return error
@@ -509,16 +507,16 @@
                 | get_addon_toc_defns(p.source, folders_per_pkg[p])
                 | hashed_folder_defns[p],
             )
             if d
         }
 
     async def _resolve_deps(
-        self, results: Collection[_ResultOrError[pkg_models.Pkg]]
-    ) -> Mapping[Defn, _ResultOrError[pkg_models.Pkg]]:
+        self, results: Collection[R.AnyResult[pkg_models.Pkg]]
+    ) -> Mapping[Defn, R.AnyResult[pkg_models.Pkg]]:
         """Resolve package dependencies.
 
         The resolver will not follow dependencies
         more than one level deep.  This is to avoid unnecessary
         complexity for something that I would never expect to
         encounter in the wild.
         """
@@ -537,15 +535,15 @@
             evolve(d, alias=r.slug) if isinstance(r, pkg_models.Pkg) else d: r
             for d, r in deps.items()
         }
         return pretty_deps
 
     async def resolve(
         self, defns: Collection[Defn], with_deps: bool = False
-    ) -> Mapping[Defn, _ResultOrError[pkg_models.Pkg]]:
+    ) -> Mapping[Defn, R.AnyResult[pkg_models.Pkg]]:
         "Resolve definitions into packages."
         if not defns:
             return {}
 
         defns_by_source = bucketise(defns, key=lambda v: v.source)
         results = await gather(
             (self.resolvers.get(s, _DummyResolver).resolve(b) for s, b in defns_by_source.items()),
@@ -697,15 +695,15 @@
         return old_pkg.version != new_pkg.version or (
             not await self._check_installed_pkg_integrity(old_pkg)
         )
 
     @_with_lock(_StandardLocks.MutatePkgs)
     async def install(
         self, defns: Sequence[Defn], replace: bool, dry_run: bool = False
-    ) -> Mapping[Defn, _ResultOrError[R.PkgInstalled]]:
+    ) -> Mapping[Defn, R.AnyResult[R.PkgInstalled]]:
         "Install packages from a definition list."
 
         # We'll weed out installed deps from the results after resolving -
         # doing it this way isn't particularly efficient but avoids having to
         # deal with local state in ``resolve``
         resolve_results = await self.resolve(
             [d for d in defns if not self.check_pkg_exists(d)], with_deps=True
@@ -735,15 +733,15 @@
                 for d, a in archive_paths.items()
             }
         )
 
     @_with_lock(_StandardLocks.MutatePkgs)
     async def update(
         self, defns: Sequence[Defn], retain_defn_strategy: bool, dry_run: bool = False
-    ) -> Mapping[Defn, _ResultOrError[R.PkgInstalled | R.PkgUpdated]]:
+    ) -> Mapping[Defn, R.AnyResult[R.PkgInstalled | R.PkgUpdated]]:
         """Update installed packages from a definition list.
 
         A ``retain_defn_strategy`` value of false will instruct ``update``
         to extract the strategy from the installed package; otherwise
         the ``Defn`` strategy will be used.
         """
 
@@ -805,28 +803,28 @@
                 for o, n in (updatables[d],)
             }
         )
 
     @_with_lock(_StandardLocks.MutatePkgs)
     async def remove(
         self, defns: Sequence[Defn], keep_folders: bool
-    ) -> Mapping[Defn, _ResultOrError[R.PkgRemoved]]:
+    ) -> Mapping[Defn, R.AnyResult[R.PkgRemoved]]:
         "Remove packages by their definition."
         return {
             d: (
                 await capture_manager_exc_async(self._remove_pkg(p, keep_folders))
                 if p
                 else R.PkgNotInstalled()
             )
             for d in defns
             for p in (self.get_pkg(d),)
         }
 
     @_with_lock(_StandardLocks.MutatePkgs)
-    async def pin(self, defns: Sequence[Defn]) -> Mapping[Defn, _ResultOrError[R.PkgInstalled]]:
+    async def pin(self, defns: Sequence[Defn]) -> Mapping[Defn, R.AnyResult[R.PkgInstalled]]:
         """Pin and unpin installed packages.
 
         instawow does not have true pinning.  This flips ``Strategy.VersionEq``
         on for installed packages from sources that support it.
         The net effect is the same as if the package
         had been reinstalled with the ``VersionEq`` strategy.
         """
```

### Comparing `instawow-3.0.0/src/instawow/matchers.py` & `instawow-3.0.1/src/instawow/matchers.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/pkg_db.py` & `instawow-3.0.1/src/instawow/pkg_db.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/pkg_models.py` & `instawow-3.0.1/src/instawow/pkg_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 
 import sqlalchemy as sa
-from attrs import asdict, frozen
+from attrs import asdict, field, frozen
 from cattrs import Converter
 from typing_extensions import Self
 
 from . import pkg_db
 from .common import Defn, StrategyValues
 
 _db_pkg_converter = Converter()
@@ -52,17 +52,17 @@
     description: str
     url: str
     download_url: str
     date_published: datetime
     version: str
     changelog_url: str
     options: PkgOptions  # pkg_options
-    folders: list[PkgFolder] = []  # pkg_folder
-    deps: list[PkgDep] = []  # pkg_dep
-    logged_versions: list[PkgLoggedVersion] = []  # pkg_version_log
+    folders: list[PkgFolder] = field(factory=list)  # pkg_folder
+    deps: list[PkgDep] = field(factory=list)  # pkg_dep
+    logged_versions: list[PkgLoggedVersion] = field(factory=list)  # pkg_version_log
 
     @classmethod
     def from_row_mapping(cls, connection: sa.Connection, row_mapping: sa.RowMapping) -> Self:
         source_and_id = {'pkg_source': row_mapping['source'], 'pkg_id': row_mapping['id']}
         return _db_pkg_converter.structure(
             {
                 **row_mapping,
```

### Comparing `instawow-3.0.0/src/instawow/plugins.py` & `instawow-3.0.1/src/instawow/plugins.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/resolvers.py` & `instawow-3.0.1/src/instawow/resolvers.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/results.py` & `instawow-3.0.1/src/instawow/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from __future__ import annotations
 
 from collections.abc import Collection
-from typing import Any, Final, Protocol
+from typing import Any, Final, Protocol, TypeVar
 
 from attrs import asdict
+from typing_extensions import TypeAlias
 
 from . import pkg_models
 from .common import Strategy, StrategyValues
 
+_T = TypeVar('_T')
 
-class ManagerResult(Protocol):
+AnyResult: TypeAlias = '_T | ManagerError | InternalError'
+
+
+class Result(Protocol):
     @property
     def message(self) -> str:
         ...
 
 
 class _SuccessResult:
     status: Final = 'success'
 
 
-class PkgInstalled(ManagerResult, _SuccessResult):
+class PkgInstalled(Result, _SuccessResult):
     def __init__(self, pkg: pkg_models.Pkg, *, dry_run: bool = False) -> None:
         super().__init__()
         self.pkg = pkg
         self.dry_run = dry_run
 
     @property
     def message(self) -> str:
         return f'{"would have installed" if self.dry_run else "installed"} {self.pkg.version}'
 
 
-class PkgUpdated(ManagerResult, _SuccessResult):
+class PkgUpdated(Result, _SuccessResult):
     def __init__(
         self, old_pkg: pkg_models.Pkg, new_pkg: pkg_models.Pkg, *, dry_run: bool = False
     ) -> None:
         super().__init__()
         self.old_pkg = old_pkg
         self.new_pkg = new_pkg
         self.dry_run = dry_run
@@ -56,25 +61,25 @@
             message += '; '.join(
                 f'{s}={v!r}' for s, v in new_strategies.items() - old_strategies.items()
             )
 
         return message
 
 
-class PkgRemoved(ManagerResult, _SuccessResult):
+class PkgRemoved(Result, _SuccessResult):
     def __init__(self, old_pkg: pkg_models.Pkg) -> None:
         super().__init__()
         self.old_pkg = old_pkg
 
     @property
     def message(self) -> str:
         return 'removed'
 
 
-class ManagerError(ManagerResult, Exception):
+class ManagerError(Result, Exception):
     status: Final = 'failure'
 
     @property
     def message(self) -> str:
         raise NotImplementedError
 
 
@@ -165,13 +170,13 @@
         self.strategies = strategies
 
     @property
     def message(self) -> str:
         return f'strategies are not valid for source: {", ".join(self.strategies)}'
 
 
-class InternalError(Exception, ManagerResult):
+class InternalError(Result, Exception):
     status: Final = 'error'
 
     @property
     def message(self) -> str:
         return f'internal error: "{self.args[0]}"'
```

### Comparing `instawow-3.0.0/src/instawow/utils.py` & `instawow-3.0.1/src/instawow/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 def fill(it: Iterable[_T], fill: _T, length: int) -> Iterable[_T]:
     "Fill an iterable of specified length."
     return islice(chain(it, repeat(fill)), 0, length)
 
 
 def bucketise(iterable: Iterable[_U], key: Callable[[_U], _T]) -> dict[_T, list[_U]]:
     "Place the elements of an iterable in a bucket according to ``key``."
-    bucket: defaultdict[_T, list[_U]] = defaultdict(list)
+    bucket = defaultdict[_T, list[_U]](list)
     for value in iterable:
         bucket[key(value)].append(value)
     return dict(bucket)
 
 
 def chain_dict(
     keys: Iterable[_T], default: _U, *overrides: Iterable[tuple[_T, _U]]
```

### Comparing `instawow-3.0.0/src/instawow/wa_updater.py` & `instawow-3.0.1/src/instawow/wa_updater.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/src/instawow/wow_installations.py` & `instawow-3.0.1/src/instawow/wow_installations.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/conftest.py` & `instawow-3.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/__init__.py` & `instawow-3.0.1/tests/fixtures/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,18 @@
                 match_querystring=True,
             ),
             Route(
                 URL('//api.github.com/repos/nebularg/PackagerTest/releases/assets/37156458'),
                 _load_json_fixture('github-release-release-json-release-json.json'),
             ),
             Route(
+                URL('//api.github.com/repositories/388670'),
+                _load_json_fixture('github-repo-molinari.json'),
+            ),
+            Route(
                 URL('//api.github.com/repos/p3lim-wow/Molinari'),
                 _load_json_fixture('github-repo-molinari.json'),
                 case_insensitive=True,
             ),
             Route(
                 URL('//api.github.com/repos/p3lim-wow/Molinari/releases?per_page=10'),
                 _load_json_fixture('github-release-molinari.json'),
```

### Comparing `instawow-3.0.0/tests/fixtures/http/base-catalogue-v7.compact.json` & `instawow-3.0.1/tests/fixtures/http/base-catalogue-v7.compact.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/curse-addon--all.json` & `instawow-3.0.1/tests/fixtures/http/curse-addon--all.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/curse-addon-files.json` & `instawow-3.0.1/tests/fixtures/http/curse-addon-files.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-release-molinari.json` & `instawow-3.0.1/tests/fixtures/http/github-release-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-release-no-assets.json` & `instawow-3.0.1/tests/fixtures/http/github-release-no-assets.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-release-no-release-json.json` & `instawow-3.0.1/tests/fixtures/http/github-release-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-release-release-json.json` & `instawow-3.0.1/tests/fixtures/http/github-release-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-repo-molinari.json` & `instawow-3.0.1/tests/fixtures/http/github-repo-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-repo-no-release-json.json` & `instawow-3.0.1/tests/fixtures/http/github-repo-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-repo-no-releases.json` & `instawow-3.0.1/tests/fixtures/http/github-repo-no-releases.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/github-repo-release-json.json` & `instawow-3.0.1/tests/fixtures/http/github-repo-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/regen.sh` & `instawow-3.0.1/tests/fixtures/http/regen.sh`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/tukui-ui--elvui.json` & `instawow-3.0.1/tests/fixtures/http/tukui-ui--elvui.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/tukui-ui--tukui.json` & `instawow-3.0.1/tests/fixtures/http/tukui-ui--tukui.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/wago-match-addons.json` & `instawow-3.0.1/tests/fixtures/http/wago-match-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/wowi-filedetails.json` & `instawow-3.0.1/tests/fixtures/http/wowi-filedetails.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/fixtures/http/wowi-filelist.json` & `instawow-3.0.1/tests/fixtures/http/wowi-filelist.json`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/plugin/instawow_test_plugin.py` & `instawow-3.0.1/tests/plugin/instawow_test_plugin.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test__slpp.py` & `instawow-3.0.1/tests/test__slpp.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test__sources.py` & `instawow-3.0.1/tests/test__sources.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test__version.py` & `instawow-3.0.1/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_cli.py` & `instawow-3.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_common.py` & `instawow-3.0.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_config.py` & `instawow-3.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_github_zip_parsing.py` & `instawow-3.0.1/tests/test_github_zip_parsing.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_json_rpc_api.py` & `instawow-3.0.1/tests/test_json_rpc_api.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_manager.py` & `instawow-3.0.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_matchers.py` & `instawow-3.0.1/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_utils.py` & `instawow-3.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_wa_updater.py` & `instawow-3.0.1/tests/test_wa_updater.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/tests/test_wow_installations.py` & `instawow-3.0.1/tests/test_wow_installations.py`

 * *Files identical despite different names*

### Comparing `instawow-3.0.0/PKG-INFO` & `instawow-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instawow
-Version: 3.0.0
+Version: 3.0.1
 Summary: World of Warcraft add-on manager
 License: GPL-3.0-or-later
 Author: layday
 Author-email: layday@protonmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

