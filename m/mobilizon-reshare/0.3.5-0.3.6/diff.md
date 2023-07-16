# Comparing `tmp/mobilizon-reshare-0.3.5.tar.gz` & `tmp/mobilizon-reshare-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilizon-reshare-0.3.5.tar", max compression
+gzip compressed data, was "mobilizon-reshare-0.3.6.tar", max compression
```

## Comparing `mobilizon-reshare-0.3.5.tar` & `mobilizon-reshare-0.3.6.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    29018 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/LICENSE
--rw-r--r--   0        0        0     2601 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/README.md
--rw-r--r--   0        0        0      884 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/.secrets.toml
--rw-r--r--   0        0        0        5 2023-06-10 21:27:31.415630 mobilizon-reshare-0.3.5/mobilizon_reshare/VERSION
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/__init__.py
--rw-r--r--   0        0        0      786 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/__init__.py
--rw-r--r--   0        0        0     7120 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/cli.py
--rw-r--r--   0        0        0       75 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/format/__init__.py
--rw-r--r--   0        0        0      635 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/format/format.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/list/__init__.py
--rw-r--r--   0        0        0     2265 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/list/list_event.py
--rw-r--r--   0        0        0     1540 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/list/list_publication.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0      356 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/publish/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/pull/__init__.py
--rw-r--r--   0        0        0      141 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/pull/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/recap/__init__.py
--rw-r--r--   0        0        0      453 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/recap/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/retry/__init__.py
--rw-r--r--   0        0        0      374 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/retry/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/start/__init__.py
--rw-r--r--   0        0        0      429 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/start/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/__init__.py
--rw-r--r--   0        0        0      118 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/command.py
--rw-r--r--   0        0        0     4918 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/config.py
--rw-r--r--   0        0        0     1849 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/notifiers.py
--rw-r--r--   0        0        0     3325 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/publishers.py
--rw-r--r--   0        0        0      343 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/config/strategies.py
--rw-r--r--   0        0        0      445 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/__init__.py
--rw-r--r--   0        0        0     5478 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/event.py
--rw-r--r--   0        0        0      805 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/event_publication_status.py
--rw-r--r--   0        0        0     2282 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/publication.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/event/__init__.py
--rw-r--r--   0        0        0     3090 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/event/event_selection_strategies.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/formatting/__init__.py
--rw-r--r--   0        0        0      789 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/formatting/description.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/__init__.py
--rw-r--r--   0        0        0     2972 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/publish.py
--rw-r--r--   0        0        0      770 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/pull.py
--rw-r--r--   0        0        0     2309 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/recap.py
--rw-r--r--   0        0        0     1875 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/retry.py
--rw-r--r--   0        0        0      547 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/main/start.py
--rwxr-xr-x   0        0        0     1488 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/postgres/models/0_20221006223256_init.sql
--rw-r--r--   0        0        0      108 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/postgres/pyproject.toml
--rw-r--r--   0        0        0     1396 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql
--rw-r--r--   0        0        0      155 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/sqlite/models/1_20211218165547_add column last_update_time for event.sql
--rw-r--r--   0        0        0      107 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/sqlite/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/mobilizon/__init__.py
--rw-r--r--   0        0        0     3261 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/mobilizon/events.py
--rw-r--r--   0        0        0      169 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/models/__init__.py
--rw-r--r--   0        0        0     1843 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/models/event.py
--rw-r--r--   0        0        0      638 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/models/notification.py
--rw-r--r--   0        0        0      686 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/models/publication.py
--rw-r--r--   0        0        0      401 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/models/publisher.py
--rw-r--r--   0        0        0      434 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/__init__.py
--rw-r--r--   0        0        0     5590 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/abstract.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinator.py
--rw-r--r--   0        0        0      731 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/__init__.py
--rw-r--r--   0        0        0     2298 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py
--rw-r--r--   0        0        0      915 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/dry_run.py
--rw-r--r--   0        0        0     4213 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/notify.py
--rw-r--r--   0        0        0     2895 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/publish.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/recap_publishing/__init__.py
--rw-r--r--   0        0        0      637 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/recap_publishing/dry_run.py
--rw-r--r--   0        0        0     2620 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/recap_publishing/recap.py
--rw-r--r--   0        0        0      911 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/__init__.py
--rw-r--r--   0        0        0     2922 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/facebook.py
--rw-r--r--   0        0        0     3211 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/mastodon.py
--rw-r--r--   0        0        0     1783 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/platform_mapping.py
--rw-r--r--   0        0        0     4378 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/telegram.py
--rw-r--r--   0        0        0     2644 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/twitter.py
--rw-r--r--   0        0        0     4028 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/zulip.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/__init__.py
--rw-r--r--   0        0        0      263 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/facebook.tmpl.j2
--rw-r--r--   0        0        0      244 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/facebook_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/facebook_recap_header.tmpl.j2
--rw-r--r--   0        0        0      238 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/mastodon.tmpl.j2
--rw-r--r--   0        0        0      234 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/mastodon_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/mastodon_recap_header.tmpl.j2
--rw-r--r--   0        0        0      290 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/telegram.tmpl.j2
--rw-r--r--   0        0        0      270 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/telegram_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/telegram_recap_header.tmpl.j2
--rw-r--r--   0        0        0      239 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/twitter.tmpl.j2
--rw-r--r--   0        0        0      236 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/twitter_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/twitter_recap_header.tmpl.j2
--rw-r--r--   0        0        0      267 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/zulip.tmpl.j2
--rw-r--r--   0        0        0      248 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/zulip_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/templates/zulip_recap_header.tmpl.j2
--rw-r--r--   0        0        0      929 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/settings.toml
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/__init__.py
--rw-r--r--   0        0        0     3010 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/db.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/__init__.py
--rw-r--r--   0        0        0      181 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/exceptions.py
--rw-r--r--   0        0        0     2960 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/read.py
--rw-r--r--   0        0        0     4036 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/write.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/events/__init__.py
--rw-r--r--   0        0        0      341 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/events/endpoints.py
--rw-r--r--   0        0        0     1077 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/main.py
--rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/publications/__init__.py
--rw-r--r--   0        0        0      391 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/publications/endpoints.py
--rw-r--r--   0        0        0     1269 2023-06-10 21:27:31.415630 mobilizon-reshare-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5234 2023-06-10 21:27:35.320427 mobilizon-reshare-0.3.5/setup.py
--rw-r--r--   0        0        0     3901 2023-06-10 21:27:35.320693 mobilizon-reshare-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    29018 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2601 2023-07-11 21:02:17.601151 mobilizon-reshare-0.3.6/README.md
+-rw-r--r--   0        0        0      933 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/.secrets.toml
+-rw-r--r--   0        0        0        5 2023-07-16 13:33:23.230742 mobilizon-reshare-0.3.6/mobilizon_reshare/VERSION
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-11 21:02:17.601151 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/__init__.py
+-rw-r--r--   0        0        0     7422 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/cli.py
+-rw-r--r--   0        0        0       75 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/format/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/format/format.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/list/__init__.py
+-rw-r--r--   0        0        0     2265 2023-07-11 14:20:59.708155 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/list/list_event.py
+-rw-r--r--   0        0        0     1549 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/list/list_publication.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.765298 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/publish/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/pull/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/pull/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/recap/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/recap/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/retry/__init__.py
+-rw-r--r--   0        0        0      374 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/retry/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/start/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/start/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/config/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/config/command.py
+-rw-r--r--   0        0        0     5156 2023-07-11 21:02:17.605151 mobilizon-reshare-0.3.6/mobilizon_reshare/config/config.py
+-rw-r--r--   0        0        0     1917 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/config/notifiers.py
+-rw-r--r--   0        0        0     3394 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/config/publishers.py
+-rw-r--r--   0        0        0      343 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/config/strategies.py
+-rw-r--r--   0        0        0      445 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/__init__.py
+-rw-r--r--   0        0        0     5660 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/event.py
+-rw-r--r--   0        0        0      805 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/event_publication_status.py
+-rw-r--r--   0        0        0     2282 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/publication.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/event/__init__.py
+-rw-r--r--   0        0        0     3090 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/event/event_selection_strategies.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/formatting/__init__.py
+-rw-r--r--   0        0        0      789 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/formatting/description.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/main/__init__.py
+-rw-r--r--   0        0        0     3280 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/main/publish.py
+-rw-r--r--   0        0        0      770 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/main/pull.py
+-rw-r--r--   0        0        0     2309 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/main/recap.py
+-rw-r--r--   0        0        0     1875 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/main/retry.py
+-rw-r--r--   0        0        0      547 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/main/start.py
+-rwxr-xr-x   0        0        0     1488 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/postgres/models/0_20221006223256_init.sql
+-rw-r--r--   0        0        0      108 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/postgres/pyproject.toml
+-rw-r--r--   0        0        0     1396 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql
+-rw-r--r--   0        0        0      155 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/sqlite/models/1_20211218165547_add column last_update_time for event.sql
+-rw-r--r--   0        0        0      107 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/sqlite/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/mobilizon/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/mobilizon/events.py
+-rw-r--r--   0        0        0      169 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/models/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/models/event.py
+-rw-r--r--   0        0        0      638 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/models/notification.py
+-rw-r--r--   0        0        0      686 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/models/publication.py
+-rw-r--r--   0        0        0      401 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/models/publisher.py
+-rw-r--r--   0        0        0      434 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/__init__.py
+-rw-r--r--   0        0        0     5590 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/abstract.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinator.py
+-rw-r--r--   0        0        0      731 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/__init__.py
+-rw-r--r--   0        0        0     2298 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/dry_run.py
+-rw-r--r--   0        0        0     4213 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/notify.py
+-rw-r--r--   0        0        0     2895 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/publish.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/recap_publishing/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/recap_publishing/dry_run.py
+-rw-r--r--   0        0        0     2620 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/recap_publishing/recap.py
+-rw-r--r--   0        0        0      911 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/__init__.py
+-rw-r--r--   0        0        0     2922 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/facebook.py
+-rw-r--r--   0        0        0     3211 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/mastodon.py
+-rw-r--r--   0        0        0     1783 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/platform_mapping.py
+-rw-r--r--   0        0        0     4532 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/telegram.py
+-rw-r--r--   0        0        0     2644 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/twitter.py
+-rw-r--r--   0        0        0     4028 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/zulip.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/facebook.tmpl.j2
+-rw-r--r--   0        0        0      244 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/facebook_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/facebook_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      238 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/mastodon.tmpl.j2
+-rw-r--r--   0        0        0      234 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/mastodon_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/mastodon_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      290 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/telegram.tmpl.j2
+-rw-r--r--   0        0        0      270 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/telegram_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/telegram_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      239 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/twitter.tmpl.j2
+-rw-r--r--   0        0        0      236 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/twitter_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/twitter_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      267 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/zulip.tmpl.j2
+-rw-r--r--   0        0        0      248 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/zulip_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/templates/zulip_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      976 2023-07-16 13:28:31.390392 mobilizon-reshare-0.3.6/mobilizon_reshare/settings.toml
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/__init__.py
+-rw-r--r--   0        0        0     2886 2023-07-11 21:02:17.605151 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/db.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/exceptions.py
+-rw-r--r--   0        0        0     2960 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/read.py
+-rw-r--r--   0        0        0     4036 2023-06-18 11:38:59.473963 mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/write.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/events/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/events/endpoints.py
+-rw-r--r--   0        0        0     1161 2023-07-11 21:02:17.605151 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/main.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/publications/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-10 21:24:01.769299 mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/publications/endpoints.py
+-rw-r--r--   0        0        0     1269 2023-07-16 13:33:23.234742 mobilizon-reshare-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5234 2023-07-16 13:33:27.194939 mobilizon-reshare-0.3.6/setup.py
+-rw-r--r--   0        0        0     3901 2023-07-16 13:33:27.195208 mobilizon-reshare-0.3.6/PKG-INFO
```

### Comparing `mobilizon-reshare-0.3.5/LICENSE` & `mobilizon-reshare-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/README.md` & `mobilizon-reshare-0.3.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 to install the tool in your system or virtualenv.
 
 This should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available
 commands and their description.
 
 ### Guix package
 
-If you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://github.com/fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.
+If you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://git.sr.ht/~fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.
 
 
 
 
 To run `mobilizon-reshare` from master you can run the following command from the root of the repository:
 
 ``` shell
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/.secrets.toml` & `mobilizon-reshare-0.3.6/mobilizon_reshare/.secrets.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [default.publisher.telegram]
 active=true
 chat_id="xxx"
+message_thread_id="xxx"
 token="xxx"
 username="xxx"
 [default.publisher.zulip]
 active=true
 instance="xxx"
 chat_id="xxx"
 subject="xxx"
@@ -27,14 +28,15 @@
 
 active=true
 page_access_token="xxx"
 
 [default.notifier.telegram]
 active=true
 chat_id="xxx"
+message_thread_id="xxx"
 token="xxx"
 username="xxx"
 [default.notifier.zulip]
 active=true
 instance="xxx"
 chat_id="xxx"
 subject="xxx"
@@ -47,8 +49,8 @@
 access_token="xxx"
 access_secret="xxx"
 [default.notifier.mastodon]
 active=false
 
 [default.notifier.facebook]
 active=false
-page_access_token="xxx"
+page_access_token="xxx"
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/cli/__init__.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import functools
 import logging
 import sys
 import traceback
 
 from mobilizon_reshare.config.command import CommandConfig
+from mobilizon_reshare.config.config import init_logging
 from mobilizon_reshare.storage.db import tear_down, init
 
 logger = logging.getLogger(__name__)
 
 
 async def graceful_exit():
     await tear_down()
 
 
 async def _safe_execution(function):
+    init_logging()
     await init()
 
     return_code = 1
     try:
         return_code = await function()
     except Exception:
         traceback.print_exc()
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/cli/cli.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 from mobilizon_reshare.cli.commands.recap.main import recap_command as recap_main
 from mobilizon_reshare.cli.commands.retry.main import (
     retry_event_command,
     retry_publication_command,
 )
 from mobilizon_reshare.cli.commands.start.main import start_command as start_main
 from mobilizon_reshare.config.command import CommandConfig
-from mobilizon_reshare.config.config import current_version, get_settings
+from mobilizon_reshare.config.config import current_version, get_settings, init_logging
 from mobilizon_reshare.config.publishers import publisher_names
 from mobilizon_reshare.dataclasses.event import _EventPublicationStatus
 from mobilizon_reshare.models.publication import PublicationStatus
 from mobilizon_reshare.publishers import get_active_publishers
 
 
 def test_settings(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
-    get_settings()
+    settings = get_settings()
+    init_logging(settings)
     click.echo("OK!")
     ctx.exit()
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
@@ -83,34 +84,29 @@
 )
 publication_status_argument = click.argument(
     "status",
     type=click.Choice(list(status_name_to_enum["publication"].keys())),
     default="all",
     expose_value=True,
 )
-event_uuid_option = click.option(
-    "-E",
-    "--event",
+force_publish_option = click.option(
+    "-F",
+    "--force",
     type=click.UUID,
     expose_value=True,
-    help="Publish the given event.",
-)
-publication_uuid_option = click.option(
-    "-P",
-    "--publication",
-    type=click.UUID,
-    expose_value=True,
-    help="Publish the given publication.",
+    help="Publish the given event, bypassing all selection logic. This command WILL publish"
+    "regardless of the configured strategy, so use it with care.",
 )
 platform_name_option = click.option(
     "-p",
     "--platform",
     type=str,
     expose_value=True,
-    help="Publish to the given platform. This makes sense only for events.",
+    help="Restrict the platforms where the event will be published. This makes sense only in"
+    " case of force-publishing.",
 )
 list_supported_option = click.option(
     "--list-platforms",
     is_flag=True,
     callback=print_platforms,
     expose_value=False,
     is_eager=True,
@@ -177,19 +173,27 @@
     safe_execution(pull_main,)
 
 
 @mobilizon_reshare.command(
     help="Select an event with the current configured strategy"
     " and publish it to all active platforms."
 )
-@event_uuid_option
-@publication_uuid_option
+@force_publish_option
 @platform_name_option
-def publish():
-    safe_execution(publish_main,)
+@click.option(
+    "--dry-run",
+    "dry_run",
+    is_flag=True,
+    help="Prevents data to be published to platforms.",
+    default=False,
+)
+def publish(event, platform, dry_run):
+    safe_execution(functools.partial(
+            publish_main, event, platform
+        ), CommandConfig(dry_run=dry_run))
 
 
 @mobilizon_reshare.group(help="Operations that pertain to events")
 def event():
     pass
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/format/format.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/format/format.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/list/list_event.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/list/list_event.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/cli/commands/list/list_publication.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/cli/commands/list/list_publication.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     click.echo_via_pager("\n".join(map(pretty, publications)))
 
 
 def pretty(publication: Publication):
     return (
         f"{str(publication.id) : <40}{publication.timestamp.isoformat() : <36}"
         f"{click.style(publication.status.name, fg=status_to_color[publication.status]) : <22}"
-        f"{publication.publisher.name : <12}{str(publication.event.id)}"
+        f"{publication.publisher.name : <12}{str(publication.event.mobilizon_id)}"
     )
 
 
 async def list_publications(
     status: PublicationStatus = None,
     frm: Optional[datetime] = None,
     to: Optional[datetime] = None,
 ):
-
     frm = Arrow.fromdatetime(frm) if frm else None
     to = Arrow.fromdatetime(to) if to else None
     if status is None:
         publications = await get_all_publications(from_date=frm, to_date=to)
     else:
         publications = await publications_with_status(status, from_date=frm, to_date=to)
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/config/config.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import importlib.resources
 import logging
+from logging.config import dictConfig
 from pathlib import Path
 from typing import Optional
 
 import pkg_resources
 from appdirs import AppDirs
 from dynaconf import Dynaconf, Validator
 
@@ -34,14 +35,20 @@
 
 
 def current_version() -> str:
     with importlib.resources.open_text(mobilizon_reshare, "VERSION") as fp:
         return fp.read()
 
 
+def init_logging(settings: Optional[Dynaconf] = None):
+    if settings is None:
+        settings = get_settings()
+    dictConfig(settings["logging"])
+
+
 def get_settings_files_paths() -> Optional[str]:
 
     dirs = AppDirs(appname="mobilizon-reshare", version=current_version())
     bundled_settings_path = pkg_resources.resource_filename(
         "mobilizon_reshare", "settings.toml"
     )
     for config_path in [
@@ -50,15 +57,15 @@
         bundled_settings_path,
     ]:
         if config_path and Path(config_path).exists():
             logger.debug(f"Loading configuration from {config_path}")
             return config_path
 
 
-def build_settings(validators: Optional[list[Validator]] = None):
+def build_settings(validators: Optional[list[Validator]] = None) -> Dynaconf:
     """
     Creates a Dynaconf base object. Configuration files are checked in this order:
 
       1. User configuration directory. On Linux that's `$XDG_CONFIG_HOME/mobilizon_reshare/<mobilizon-reshare-version>`;
       2. System configuration directory. On Linux that's the first element of
          `$XDG_CONFIG_DIRS` + `/mobilizon_reshare/<mobilizon-reshare-version>`.
       3. The default configuration distributed with the package.
@@ -74,15 +81,15 @@
     )
 
     # TODO use validation control in dynaconf 3.2.0 once released
     config.validators.validate()
     return config
 
 
-def build_and_validate_settings():
+def build_and_validate_settings() -> Dynaconf:
     """
     Creates a settings object to be used in the application. It collects and apply generic validators and validators
     specific for each publisher, notifier and publication strategy.
     """
 
     # we first do a preliminary load of the settings without validation. We will later use them to determine which
     # publishers, notifiers and strategy have been selected
@@ -124,13 +131,13 @@
         self.settings = build_and_validate_settings()
 
     @classmethod
     def clear(cls):
         cls._instance = None
 
 
-def get_settings():
+def get_settings() -> Dynaconf:
     return CustomConfig.get_instance().settings
 
 
-def get_settings_without_validation():
+def get_settings_without_validation() -> Dynaconf:
     return build_settings()
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/config/notifiers.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/config/notifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterator
 
 from dynaconf import Validator
 
 telegram_validators = [
     Validator("notifier.telegram.chat_id", must_exist=True),
+    Validator("notifier.telegram.message_thread_id", default=None),
     Validator("notifier.telegram.token", must_exist=True),
     Validator("notifier.telegram.username", must_exist=True),
 ]
 zulip_validators = [
     Validator("notifier.zulip.chat_id", must_exist=True),
     Validator("notifier.zulip.subject", must_exist=True),
     Validator("notifier.zulip.bot_token", must_exist=True),
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/config/publishers.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/config/publishers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dynaconf import Validator
 
 
 telegram_validators = [
     Validator("publisher.telegram.chat_id", must_exist=True),
+    Validator("publisher.telegram.message_thread_id", default=None),
     Validator("publisher.telegram.msg_template_path", must_exist=True, default=None),
     Validator("publisher.telegram.recap_template_path", must_exist=True, default=None),
     Validator(
         "publisher.telegram.recap_header_template_path", must_exist=True, default=None
     ),
     Validator("publisher.telegram.token", must_exist=True),
     Validator("publisher.telegram.username", must_exist=True),
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/event.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     async def retrieve(cls, mobilizon_id):
         return cls.from_model(await get_event(mobilizon_id))
 
 
 async def get_all_mobilizon_events(
     from_date: Optional[Arrow] = None, to_date: Optional[Arrow] = None,
 ) -> list[_MobilizonEvent]:
-    return [_MobilizonEvent.from_model(event) for event in await get_all_events()]
+    return [_MobilizonEvent.from_model(event) for event in await get_all_events(from_date, to_date)]
 
 
 async def get_published_events(
     from_date: Optional[Arrow] = None, to_date: Optional[Arrow] = None
 ) -> Iterable[_MobilizonEvent]:
     """
     Retrieves events that are not waiting. Function could be renamed to something more fitting
@@ -151,7 +151,14 @@
 ) -> list[_MobilizonEvent]:
     return [
         _MobilizonEvent.from_model(event)
         for event in await get_events_without_publications(
             from_date=from_date, to_date=to_date
         )
     ]
+
+
+async def get_mobilizon_event_by_id(
+    event_id: UUID,
+) -> _MobilizonEvent:
+    event = await get_event(event_id)
+    return _MobilizonEvent.from_model(event)
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/event_publication_status.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/event_publication_status.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/dataclasses/publication.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/dataclasses/publication.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/event/event_selection_strategies.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/event/event_selection_strategies.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/formatting/description.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/formatting/description.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/main/publish.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/main/publish.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, Iterator
 
 from mobilizon_reshare.config.command import CommandConfig
 from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.dataclasses.event import (
     get_published_events,
     get_mobilizon_events_without_publications,
+    get_mobilizon_event_by_id,
 )
 from mobilizon_reshare.dataclasses.publication import (
     _EventPublication,
     build_publications_for_event,
 )
 from mobilizon_reshare.event.event_selection_strategies import select_event_to_publish
 from mobilizon_reshare.publishers import get_active_publishers
@@ -64,14 +65,23 @@
     if command_config.dry_run:
         logger.info("Executing in dry run mode. No event is going to be published.")
         return perform_dry_run(publications)
     else:
         return await publish_publications(publications)
 
 
+async def publish_by_mobilizon_id(
+    event_mobilizon_id,
+    command_config: CommandConfig,
+    publishers: Optional[Iterator[str]] = None,
+):
+    event = await get_mobilizon_event_by_id(event_mobilizon_id)
+    return await publish_event(event, command_config, publishers)
+
+
 async def select_and_publish(
     command_config: CommandConfig,
     unpublished_events: Optional[list[MobilizonEvent]] = None,
 ) -> Optional[PublisherCoordinatorReport]:
     """
     STUB
     :return:
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/main/pull.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/main/pull.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/main/recap.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/main/recap.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/main/retry.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/main/retry.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/main/start.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/main/start.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/postgres/models/0_20221006223256_init.sql` & `mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/postgres/models/0_20221006223256_init.sql`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql` & `mobilizon-reshare-0.3.6/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/mobilizon/events.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/mobilizon/events.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/models/event.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/models/event.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/models/notification.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/models/notification.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/models/publication.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/models/publication.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/abstract.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/abstract.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/__init__.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/__init__.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/dry_run.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/dry_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,36 @@
+import logging
 from typing import List, Sequence
 
 from mobilizon_reshare.dataclasses import _EventPublication
 from mobilizon_reshare.models.publication import PublicationStatus
 from mobilizon_reshare.publishers.coordinators.event_publishing.publish import (
     PublisherCoordinator,
     EventPublicationReport,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class DryRunPublisherCoordinator(PublisherCoordinator):
     """
     Coordinator to perform a dry-run on the event publication
     """
 
     def _publish(self, publications: Sequence[_EventPublication]) -> List[EventPublicationReport]:
-        return [
+        reports = [
             EventPublicationReport(
                 status=PublicationStatus.COMPLETED,
                 publication=publication,
                 reason=None,
                 published_content=publication.formatter.get_message_from_event(
                     publication.event
                 ),
             )
             for publication in publications
         ]
+        logger.info("The following events would be published:")
+        for r in reports:
+            event_name = r.publication.event.name
+            publisher_name = r.publication.publisher.name
+            logger.info(f"{event_name} → {publisher_name}")
+        return reports
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/notify.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/notify.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/event_publishing/publish.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/event_publishing/publish.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/recap_publishing/dry_run.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/recap_publishing/dry_run.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/coordinators/recap_publishing/recap.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/coordinators/recap_publishing/recap.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/exceptions.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/exceptions.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/facebook.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/facebook.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/mastodon.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/mastodon.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/platform_mapping.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/platform_mapping.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/telegram.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/telegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,22 @@
 
         if not self.conf.username == data.get("result", {}).get("username"):
             self._log_error(
                 "Found a different bot than the expected one", raise_error=InvalidBot,
             )
 
     def _send(self, message: str, event: Optional[MobilizonEvent] = None) -> Response:
+        json_message = {"chat_id": self.conf.chat_id, "text": message, "parse_mode": "html"}
+
+        if self.conf.message_thread_id:
+            json_message["message_thread_id"] = self.conf.message_thread_id
+
         return requests.post(
             url=f"https://api.telegram.org/bot{self.conf.token}/sendMessage",
-            json={"chat_id": self.conf.chat_id, "text": message, "parse_mode": "html"},
+            json=json_message,
         )
 
     def _validate_response(self, res):
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as e:
             self._log_error(
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/twitter.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/twitter.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/publishers/platforms/zulip.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/publishers/platforms/zulip.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/storage/db.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/storage/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from logging.config import dictConfig
 from pathlib import Path
 
 import pkg_resources
 import urllib3.util
 from aerich import Command
 from tortoise import Tortoise
 
@@ -88,19 +87,15 @@
                 self.path.parent.mkdir(parents=True, exist_ok=True)
 
 
 async def tear_down():
     return await Tortoise.close_connections()
 
 
-async def init(init_logging=True):
-
-    if init_logging:
-        dictConfig(get_settings()["logging"])
-
+async def init():
     # init storage
     url = get_db_url()
     if url.scheme == "sqlite":
         db = MoReSQLiteDB()
     else:
         db = MoReDB()
     await db.setup()
```

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/read.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/read.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/storage/query/write.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/storage/query/write.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.5/mobilizon_reshare/web/backend/main.py` & `mobilizon-reshare-0.3.6/mobilizon_reshare/web/backend/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from fastapi import FastAPI
 from fastapi_pagination import add_pagination
 
+from mobilizon_reshare.config.config import init_logging as init_log
 from mobilizon_reshare.storage.db import init as init_db, get_db_url
 from mobilizon_reshare.web.backend.events.endpoints import (
     register_endpoints as register_event_endpoints,
 )
 from mobilizon_reshare.web.backend.publications.endpoints import (
     register_endpoints as register_publication_endpoints,
 )
@@ -34,11 +35,13 @@
 
     register_endpoints(app)
     add_pagination(app)
 
 
 @app.on_event("startup")
 async def init_app(init_logging=True):
+    if init_logging:
+        init_log()
     check_database()
-    await init_db(init_logging=init_logging)
+    await init_db()
     init_endpoints(app)
     return app
```

### Comparing `mobilizon-reshare-0.3.5/pyproject.toml` & `mobilizon-reshare-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mobilizon-reshare"
-version = "0.3.5"
+version = "0.3.6"
 description = "A suite to reshare Mobilizon events on a broad selection of platforms"
 readme = "README.md"
 homepage = "https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare"
 repository = "https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare"
 authors = ["Simone Robutti <simone.robutti@protonmail.com>"]
 license = "Coopyleft"
```

### Comparing `mobilizon-reshare-0.3.5/setup.py` & `mobilizon-reshare-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 
 entry_points = \
 {'console_scripts': ['mobilizon-reshare = '
                      'mobilizon_reshare.cli.cli:mobilizon_reshare']}
 
 setup_kwargs = {
     'name': 'mobilizon-reshare',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'A suite to reshare Mobilizon events on a broad selection of platforms',
-    'long_description': "[![CI](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml)\n\nThe goal of `mobilizon_reshare` is to provide a suite to reshare Mobilizon events on a broad selection of platforms. This\ntool enables an organization to automate their social media strategy in regards\nto events and their promotion. \n\n# Platforms\n\n`mobilizon-reshare` currently supports the following social platforms:\n\n- Facebook\n- Mastodon\n- Twitter\n- Telegram\n- Zulip\n\n# Usage\n\n## Scheduling and temporal logic\n\nThe tool is designed to work in combination with a scheduler that executes it at\nregular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when\nto publish an event, with the minimization of human effort as its first priority.\n\n## Installation\n\n`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/twcita/mobilizon-reshare). Use\n\n```shell\n$ pip install mobilizon-reshare\n```\n\nto install the tool in your system or virtualenv.\n\nThis should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available\ncommands and their description.\n\n### Guix package\n\nIf you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://github.com/fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.\n\n\n\n\nTo run `mobilizon-reshare` from master you can run the following command from the root of the repository:\n\n``` shell\n$ guix time-machine -C channels-lock.scm -- install -L . mobilizon-reshare.git\n```\n\n## Run on your local system\n\nOnce you have installed `mobilizon_reshare` you can schedule the refresh from Mobilizon with your system's `cron`:\n\n```bash\n$ sudo crontab -l\n*/15 * * * * mobilizon-reshare start\n```\n\n## Deploying through Docker Compose\n\nTo run `mobilizon_reshare` in a production environment you can use the image published to DockerHub. We also provide an example [`docker-compose.yml`](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/docker-compose.yml).\n\n# Contributing\n\nWe welcome contributions from anybody. Currently our process is not structured but feel free to open or take issues through Github in case you want to help us. We have setup some instructions to setup a development environment [here](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/doc/contributing.md).\n",
+    'long_description': "[![CI](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml)\n\nThe goal of `mobilizon_reshare` is to provide a suite to reshare Mobilizon events on a broad selection of platforms. This\ntool enables an organization to automate their social media strategy in regards\nto events and their promotion. \n\n# Platforms\n\n`mobilizon-reshare` currently supports the following social platforms:\n\n- Facebook\n- Mastodon\n- Twitter\n- Telegram\n- Zulip\n\n# Usage\n\n## Scheduling and temporal logic\n\nThe tool is designed to work in combination with a scheduler that executes it at\nregular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when\nto publish an event, with the minimization of human effort as its first priority.\n\n## Installation\n\n`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/twcita/mobilizon-reshare). Use\n\n```shell\n$ pip install mobilizon-reshare\n```\n\nto install the tool in your system or virtualenv.\n\nThis should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available\ncommands and their description.\n\n### Guix package\n\nIf you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://git.sr.ht/~fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.\n\n\n\n\nTo run `mobilizon-reshare` from master you can run the following command from the root of the repository:\n\n``` shell\n$ guix time-machine -C channels-lock.scm -- install -L . mobilizon-reshare.git\n```\n\n## Run on your local system\n\nOnce you have installed `mobilizon_reshare` you can schedule the refresh from Mobilizon with your system's `cron`:\n\n```bash\n$ sudo crontab -l\n*/15 * * * * mobilizon-reshare start\n```\n\n## Deploying through Docker Compose\n\nTo run `mobilizon_reshare` in a production environment you can use the image published to DockerHub. We also provide an example [`docker-compose.yml`](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/docker-compose.yml).\n\n# Contributing\n\nWe welcome contributions from anybody. Currently our process is not structured but feel free to open or take issues through Github in case you want to help us. We have setup some instructions to setup a development environment [here](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/doc/contributing.md).\n",
     'author': 'Simone Robutti',
     'author_email': 'simone.robutti@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mobilizon-reshare-0.3.5/PKG-INFO` & `mobilizon-reshare-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilizon-reshare
-Version: 0.3.5
+Version: 0.3.6
 Summary: A suite to reshare Mobilizon events on a broad selection of platforms
 Home-page: https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare
 License: Coopyleft
 Author: Simone Robutti
 Author-email: simone.robutti@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -65,15 +65,15 @@
 to install the tool in your system or virtualenv.
 
 This should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available
 commands and their description.
 
 ### Guix package
 
-If you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://github.com/fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.
+If you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://git.sr.ht/~fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.
 
 
 
 
 To run `mobilizon-reshare` from master you can run the following command from the root of the repository:
 
 ``` shell
```

