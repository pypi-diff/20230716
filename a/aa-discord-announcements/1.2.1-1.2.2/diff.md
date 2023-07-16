# Comparing `tmp/aa_discord_announcements-1.2.1.tar.gz` & `tmp/aa_discord_announcements-1.2.2.tar.gz`

## Comparing `aa_discord_announcements-1.2.1.tar` & `aa_discord_announcements-1.2.2.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/admin.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/app_settings.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/apps.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/constants.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/forms.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/models.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/urls.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/views.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/helper/discord_webhook.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/django.pot
--rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0002_translation_updates.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/base.html
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/index.html
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/LICENSE
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/README.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/admin.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/app_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/apps.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/constants.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/forms.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/models.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/urls.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/docs/screenshots/weblate/.gitkeep
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/helper/discord_webhook.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/django.pot
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0002_translation_updates.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/base.html
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/index.html
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/README.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.2/PKG-INFO
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/admin.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/models.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     # Restrictions
     restricted_to_group = models.ManyToManyField(
         Group,
         blank=True,
         related_name="discord_announcement_pingtarget_required_groups",
         verbose_name=_("Group restrictions"),
-        help_text=_("Restrict ping rights to the following group(s) …"),
+        help_text=_("Restrict ping rights to the following groups …"),
     )
 
     # Notes
     notes = models.TextField(
         default="",
         blank=True,
         verbose_name=_("Notes"),
@@ -184,15 +184,15 @@
 
     # Restrictions
     restricted_to_group = models.ManyToManyField(
         Group,
         blank=True,
         related_name="discord_announcement_webhook_required_groups",
         verbose_name=_("Group restrictions"),
-        help_text=_("Restrict ping rights to the following group(s) …"),
+        help_text=_("Restrict ping rights to the following groups …"),
     )
 
     # Webhook notes
     notes = models.TextField(
         default="",
         blank=True,
         verbose_name=_("Notes"),
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/views.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/helper/discord_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from aa_discord_announcements.helper.announcement_context import (
     get_webhook_announcement_context,
 )
 
 
 def send_to_discord_webhook(announcement_context: dict, user: User):
     """
-    Send announcement to a Discord webhook
+    Send the announcement to a Discord webhook
     :param announcement_context:
     :param user:
     :return:
     """
 
     discord_webhook = Webhook(announcement_context["announcement_channel"]["webhook"])
     webhook_announcement_context = get_webhook_announcement_context(
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/django.pot` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"PO-Revision-Date: 2023-04-18 23:17+0000\n"
+"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
@@ -34,39 +35,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
+msgstr "Este campo es obligatorio"
+
+#: forms.py:42
+msgid "Discord Markdown"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -89,15 +105,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18\n"
+"X-Generator: Weblate 4.18.1\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
 msgid "Announcement Channel"
 msgstr "Ankündigungskanal"
 
@@ -37,17 +37,23 @@
 
 msgid "Create Announcement"
 msgstr "Ankündigung erstellen"
 
 msgid "Discord Announcements"
 msgstr "Discord-Ankündigungen"
 
+msgid "Discord Announcements v{__version__}"
+msgstr "Discord Announcements v{__version__}"
+
 msgid "Discord ID"
 msgstr "Discord ID"
 
+msgid "Discord Markdown"
+msgstr "Discord Markdown"
+
 msgid "Discord Ping Target"
 msgstr "Discord Pingziel"
 
 msgid "Discord Ping Targets"
 msgstr "Discord Pingziele"
 
 msgid "Discord channel"
@@ -71,14 +77,18 @@
 
 msgid "Group name"
 msgstr "Gruppenname"
 
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+"Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
+
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
@@ -114,16 +124,16 @@
 
 msgid "None, just format it for me"
 msgstr "Keiner, einfach nur den Text formatieren"
 
 msgid "Notes"
 msgstr "Notizen"
 
-msgid "Restrict ping rights to the following group(s) …"
-msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) …"
+msgid "Restrict ping rights to the following groups …"
+msgstr "Beschränkt die Ping-Rechte auf die folgenden Gruppen …"
 
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Wähle einen Kanal in dem die Ankündigung gesendet werden soll."
 
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Erfolg! Der Ankündigungstext wurde in die Zwischenablage kopiert."
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
-"PO-Revision-Date: 2023-06-19 10:18+0000\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"PO-Revision-Date: 2023-06-28 14:37+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr "Discord-Ankündigungen"
 
 #: admin.py:32 models.py:79
@@ -35,39 +35,55 @@
 msgid "Discord channel"
 msgstr "Discord-Kanal"
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr "Webhook URL"
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr "Discord Announcements v{__version__}"
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr "Dies ist ein Pflichtfeld"
 
-#: forms.py:37
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr "Discord Markdown"
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+"Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr "Ankündigungsziel"
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr "Wen möchtest Du pingen?"
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr "Ankündigungskanal"
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Wähle einen Kanal in dem die Ankündigung gesendet werden soll."
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr "Ankündigungstext"
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr "Deine Ankündigung …"
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
@@ -93,16 +109,16 @@
 msgstr "Discord ID"
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
-msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) …"
+msgid "Restrict ping rights to the following groups …"
+msgstr "Beschränkt die Ping-Rechte auf die folgenden Gruppen …"
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr "Notizen"
 
 #: models.py:111
 msgid "You can add notes about this configuration here if you want"
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/es/>\n"
-"Language: es\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/fr/>\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
@@ -35,39 +35,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
-msgstr "Este campo es obligatorio"
+msgstr "Ce champ est obligatoire"
+
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
 
-#: forms.py:37
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -90,15 +105,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/fr/>\n"
-"Language: fr_FR\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
@@ -35,39 +35,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "Questo campo è obbligatorio"
+
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
 
-#: forms.py:37
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -90,15 +105,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/django.pot`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
-"PO-Revision-Date: 2023-04-18 23:17+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/it/>\n"
-"Language: it_IT\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.4\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
@@ -35,39 +34,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+msgstr ""
+
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
 
-#: forms.py:37
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -90,15 +104,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
@@ -35,39 +34,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -90,15 +104,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr ""
 
 #: admin.py:32 models.py:79
@@ -34,39 +35,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -89,15 +105,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18\n"
+"X-Generator: Weblate 4.18.1\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
 msgid "Announcement Channel"
 msgstr "Канал объявления"
 
@@ -37,17 +37,23 @@
 
 msgid "Create Announcement"
 msgstr "Создать объявление"
 
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
+msgid "Discord Announcements v{__version__}"
+msgstr "Объявления Discord v{__version__}"
+
 msgid "Discord ID"
 msgstr "Идентификатор Discord"
 
+msgid "Discord Markdown"
+msgstr "Разметка Discord"
+
 msgid "Discord Ping Target"
 msgstr "Цель пинга Discrod"
 
 msgid "Discord Ping Targets"
 msgstr "Цели пинга Discord"
 
 msgid "Discord channel"
@@ -71,14 +77,19 @@
 
 msgid "Group name"
 msgstr "Название группы"
 
 msgid "Group restrictions"
 msgstr "Ограничения групп"
 
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+"Подсказка: Вы можете использовать {discord_markdown_link} для форматирования "
+"текста."
+
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
@@ -113,16 +124,16 @@
 
 msgid "None, just format it for me"
 msgstr "Нет, только отформатируй"
 
 msgid "Notes"
 msgstr "Примечания"
 
-msgid "Restrict ping rights to the following group(s) …"
-msgstr "Разрешить пинговать следующим группам …"
+msgid "Restrict ping rights to the following groups …"
+msgstr "Ограничить право пинговать для следующих групп …"
 
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Выберите канал для автоматической отправки объявлений."
 
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Успех! Объявление скопировано в буфер обмена."
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
-"PO-Revision-Date: 2023-06-19 10:18+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
+"PO-Revision-Date: 2023-06-24 13:57+0000\n"
+"Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: __init__.py:12 templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
 #: admin.py:32 models.py:79
@@ -37,39 +37,56 @@
 msgid "Discord channel"
 msgstr "Канал Discord"
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr "Вебхук URL"
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr "Объявления Discord v{__version__}"
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr "Обязательное поле"
 
-#: forms.py:37
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr "Разметка Discord"
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+"Подсказка: Вы можете использовать {discord_markdown_link} для форматирования "
+"текста."
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr "Цель объявления"
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr "Кого Вы хотите пинговать?"
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr "Канал объявления"
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Выберите канал для автоматической отправки объявлений."
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr "Текст объявления"
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr "Ваше объявление …"
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
@@ -94,16 +111,16 @@
 msgstr "Идентификатор Discord"
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
-msgstr "Разрешить пинговать следующим группам …"
+msgid "Restrict ping rights to the following groups …"
+msgstr "Ограничить право пинговать для следующих групп …"
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr "Примечания"
 
 #: models.py:111
 msgid "You can add notes about this configuration here if you want"
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Kristof <kristof@teh.ninja>, 2023.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: 2023-06-14 17:18+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -40,39 +40,56 @@
 
 #: admin.py:66 models.py:176
 #, fuzzy
 #| msgid "Webhook"
 msgid "Webhook URL"
 msgstr "Веб-хук"
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:42
+#, fuzzy
+#| msgid "Discord Markdown"
+msgid "Discord Markdown"
+msgstr "Discord markdown"
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr "Кого ви хочете пінгувати?"
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Виберіть канал для автоматичного відправлення оголошення."
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr "Текст оголошення"
 
-#: forms.py:55
+#: forms.py:79
 #, fuzzy
 #| msgid "Your announcement…"
 msgid "Your announcement …"
 msgstr "Ваше оголошення…"
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
@@ -101,15 +118,17 @@
 msgstr "Discord markdown"
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+#, fuzzy
+#| msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr "Обмежити права на пінг для наступних груп …"
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.2/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"POT-Creation-Date: 2023-06-23 18:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -35,39 +35,54 @@
 msgid "Discord channel"
 msgstr ""
 
 #: admin.py:66 models.py:176
 msgid "Webhook URL"
 msgstr ""
 
-#: forms.py:20
+#. Translators: This is the app name and version, which will appear in the Django Backend
+#: apps.py:21
+#, python-brace-format
+msgid "Discord Announcements v{__version__}"
+msgstr ""
+
+#: forms.py:21
 msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:42
+msgid "Discord Markdown"
+msgstr ""
+
+#: forms.py:49
+#, python-brace-format
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+
+#: forms.py:61
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:39
+#: forms.py:63
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:43
+#: forms.py:67
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:49
+#: forms.py:73
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:55
+#: forms.py:79
 msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
@@ -90,15 +105,15 @@
 msgstr ""
 
 #: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
 #: models.py:103 models.py:191
-msgid "Restrict ping rights to the following group(s) …"
+msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
 #: models.py:110 models.py:198
 msgid "Notes"
 msgstr ""
 
 #: models.py:111
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0002_translation_updates.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/migrations/0002_translation_updates.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.2.2/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.2.2/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,30 +35,30 @@
         # User can access aa_discord_announcements
         cls.user_1002 = create_fake_user(
             1002, "Bruce Wayne", permissions=["aa_discord_announcements.basic_access"]
         )
 
     def test_has_no_access(self):
         """
-        Test that a user without access get a 302
+        Test that a user without access gets a 302
         :return:
         """
 
         # given
         self.client.force_login(self.user_1001)
 
         # when
         res = self.client.get(reverse("aa_discord_announcements:index"))
 
         # then
         self.assertEqual(res.status_code, HTTPStatus.FOUND)
 
     def test_has_access(self):
         """
-        Test that a user with access get to see it
+        Test that a user with access gets to see it
         :return:
         """
 
         # given
         self.client.force_login(self.user_1002)
 
         # when
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         res = self.client.get(reverse("aa_discord_announcements:ajax_get_webhooks"))
 
         # then
         self.assertEqual(res.status_code, HTTPStatus.OK)
 
     def test_ajax_create_announcement_no_access(self):
         """
-        Test ajax call to create announcement available for
+        Test ajax call to create an announcement is not available for
         a user without access to it
         :return:
         """
 
         # given
         self.client.force_login(self.user_1001)
 
@@ -119,15 +119,15 @@
         )
 
         # then
         self.assertEqual(res.status_code, HTTPStatus.FOUND)
 
     def test_ajax_create_announcement_general(self):
         """
-        Test ajax call to create announcement for the current user
+        Test ajax call to create an announcement is available for the current user
         :return:
         """
 
         # given
         self.client.force_login(self.user_1002)
 
         # when
@@ -136,15 +136,15 @@
         )
 
         # then
         self.assertEqual(res.status_code, HTTPStatus.OK)
 
     def test_ajax_create_announcement_with_form_data(self):
         """
-        Test ajax call to create announcement for the current user with form data
+        Test ajax call to create an announcement for the current user with form data
         :return:
         """
 
         # given
         self.client.force_login(self.user_1002)
         form_data = {
             "announcement_target": "@here",
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from django.test import TestCase, modify_settings
 
 # AA Discord Announcements
 from aa_discord_announcements.app_settings import discord_service_installed
 
 
 class TestModulesInstalled(TestCase):
+    """
+    Test for installed modules
+    """
+
     @classmethod
     def setUpClass(cls) -> None:
         """
         Set up groups and users
         """
 
         super().setUpClass()
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/test_templatetags.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         Test versioned static template tag
         :return:
         """
 
         context = Context({"version": __version__})
         template_to_render = Template(
             "{% load aa_discord_announcements_versioned_static %}"
-            "{% aa_discord_announcements_static 'aa_discord_announcements/css/aa-discord-announcements.min.css' %}"
+            "{% aa_discord_announcements_static 'aa_discord_announcements/css/aa-discord-announcements.min.css' %}"  # pylint: disable=line-too-long
         )
 
         rendered_template = template_to_render.render(context)
 
         self.assertInHTML(
-            f'/static/aa_discord_announcements/css/aa-discord-announcements.min.css?v={context["version"]}',
+            f'/static/aa_discord_announcements/css/aa-discord-announcements.min.css?v={context["version"]}',  # pylint: disable=line-too-long
             rendered_template,
         )
```

### Comparing `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.2.2/aa_discord_announcements/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     corporation_name: str = None,
     corporation_ticker: str = None,
     alliance_id: int = None,
     alliance_name: str = None,
     permissions: List[str] = None,
 ) -> User:
     """
-    Create a fake user incl. main character and (optional) permissions.
+    Create a fake user incl. Main character and (optional) permissions.
     """
 
     username = re.sub(r"[^\w\d@\.\+-]", "_", character_name)
     user = AuthUtils.create_user(username)
 
     if not corporation_id:
         corporation_id = 2001
```

### Comparing `aa_discord_announcements-1.2.1/LICENSE` & `aa_discord_announcements-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.1/README.md` & `aa_discord_announcements-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![Python](https://img.shields.io/pypi/pyversions/aa-discord-announcements)](https://pypi.org/project/aa-discord-announcements/)
 [![Django](https://img.shields.io/pypi/djversions/aa-discord-announcements?label=django)](https://pypi.org/project/aa-discord-announcements/)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
 [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
 [![Checks](https://github.com/ppfeufer/aa-discord-announcements/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-discord-announcements/actions/workflows/automated-checks.yml)
 [![codecov](https://codecov.io/gh/ppfeufer/aa-discord-announcements/branch/master/graph/badge.svg?token=9I6HQB6W6J)](https://codecov.io/gh/ppfeufer/aa-discord-announcements)
+[![Translation Status](https://weblate.ppfeufer.de/widgets/alliance-auth-apps/-/aa-discord-announcements/svg-badge.svg)](https://weblate.ppfeufer.de/engage/alliance-auth-apps/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
@@ -40,17 +41,19 @@
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
 (See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
 
-**⚠️ You also want to make sure that you have the
+> **Note**
+>
+> You also want to make sure that you have the
 [Discord service](https://allianceauth.readthedocs.io/en/latest/features/services/discord.html)
-installed, configured and activated before installing this app. ⚠️**
+installed, configured and activated before installing this app.
 
 
 ### Step 1: Install the App
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
```

### Comparing `aa_discord_announcements-1.2.1/pyproject.toml` & `aa_discord_announcements-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aa-discord-announcements"
-version = "1.2.1"
+version = "1.2.2"
 description = "Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth."
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
```

### Comparing `aa_discord_announcements-1.2.1/PKG-INFO` & `aa_discord_announcements-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discord-announcements
-Version: 1.2.1
+Version: 1.2.2
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Project-URL: Homepage, https://github.com/ppfeufer/aa-discord-announcements
 Project-URL: Documentation, https://github.com/ppfeufer/aa-discord-announcements/blob/master/README.md
 Project-URL: Source, https://github.com/ppfeufer/aa-discord-announcements.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/ppfeufer/aa-discord-announcements/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
@@ -38,14 +38,15 @@
 [![Python](https://img.shields.io/pypi/pyversions/aa-discord-announcements)](https://pypi.org/project/aa-discord-announcements/)
 [![Django](https://img.shields.io/pypi/djversions/aa-discord-announcements?label=django)](https://pypi.org/project/aa-discord-announcements/)
 ![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](http://black.readthedocs.io/en/latest/)
 [![Discord](https://img.shields.io/discord/790364535294132234?label=discord)](https://discord.gg/zmh52wnfvM)
 [![Checks](https://github.com/ppfeufer/aa-discord-announcements/actions/workflows/automated-checks.yml/badge.svg)](https://github.com/ppfeufer/aa-discord-announcements/actions/workflows/automated-checks.yml)
 [![codecov](https://codecov.io/gh/ppfeufer/aa-discord-announcements/branch/master/graph/badge.svg?token=9I6HQB6W6J)](https://codecov.io/gh/ppfeufer/aa-discord-announcements)
+[![Translation Status](https://weblate.ppfeufer.de/widgets/alliance-auth-apps/-/aa-discord-announcements/svg-badge.svg)](https://weblate.ppfeufer.de/engage/alliance-auth-apps/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
@@ -73,17 +74,19 @@
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
 (See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
 
-**⚠️ You also want to make sure that you have the
+> **Note**
+>
+> You also want to make sure that you have the
 [Discord service](https://allianceauth.readthedocs.io/en/latest/features/services/discord.html)
-installed, configured and activated before installing this app. ⚠️**
+installed, configured and activated before installing this app.
 
 
 ### Step 1: Install the App
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
```

