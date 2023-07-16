# Comparing `tmp/invenhost-core-0.1.0.tar.gz` & `tmp/invenhost-core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenhost-core-0.1.0.tar", last modified: Sun Jul 16 21:10:46 2023, max compression
+gzip compressed data, was "invenhost-core-0.2.0.tar", last modified: Sun Jul 16 21:40:25 2023, max compression
```

## Comparing `invenhost-core-0.1.0.tar` & `invenhost-core-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-16 21:10:46.243579 invenhost-core-0.1.0/
--rw-r--r--   0 matmair    (501) staff       (20)       34 2023-07-16 15:12:23.000000 invenhost-core-0.1.0/MANIFEST.in
--rw-r--r--   0 matmair    (501) staff       (20)     1703 2023-07-16 21:10:46.243681 invenhost-core-0.1.0/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)      859 2023-07-16 20:43:38.000000 invenhost-core-0.1.0/README.md
--rw-r--r--   0 matmair    (501) staff       (20)     1209 2023-07-16 20:22:47.000000 invenhost-core-0.1.0/pyproject.toml
--rw-r--r--   0 matmair    (501) staff       (20)      143 2023-07-16 21:10:46.243990 invenhost-core-0.1.0/setup.cfg
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-16 21:10:46.240357 invenhost-core-0.1.0/src/
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-16 21:10:46.241999 invenhost-core-0.1.0/src/invenhost_core/
--rw-r--r--   0 matmair    (501) staff       (20)     5620 2023-07-16 20:43:51.000000 invenhost-core-0.1.0/src/invenhost_core/InvenHostCore.py
--rw-r--r--   0 matmair    (501) staff       (20)      246 2023-07-16 20:38:34.000000 invenhost-core-0.1.0/src/invenhost_core/__init__.py
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-16 21:10:46.243392 invenhost-core-0.1.0/src/invenhost_core.egg-info/
--rw-r--r--   0 matmair    (501) staff       (20)     1703 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)      367 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/SOURCES.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/dependency_links.txt
--rw-r--r--   0 matmair    (501) staff       (20)       66 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/entry_points.txt
--rw-r--r--   0 matmair    (501) staff       (20)       31 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/requires.txt
--rw-r--r--   0 matmair    (501) staff       (20)       15 2023-07-16 21:10:46.000000 invenhost-core-0.1.0/src/invenhost_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:40:25.681405 invenhost-core-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 21:40:09.000000 invenhost-core-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-16 21:40:25.681405 invenhost-core-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-16 21:40:09.000000 invenhost-core-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-16 21:40:09.000000 invenhost-core-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-16 21:40:25.681405 invenhost-core-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:40:25.677405 invenhost-core-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:40:25.681405 invenhost-core-0.2.0/src/invenhost_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-16 21:40:09.000000 invenhost-core-0.2.0/src/invenhost_core/InvenHostCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-16 21:40:09.000000 invenhost-core-0.2.0/src/invenhost_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:40:25.681405 invenhost-core-0.2.0/src/invenhost_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 21:40:25.000000 invenhost-core-0.2.0/src/invenhost_core.egg-info/top_level.txt
```

### Comparing `invenhost-core-0.1.0/PKG-INFO` & `invenhost-core-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenhost-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: InvenHost integration plugin
 Author-email: Matthias Mair <code@mjmair.com>
 License: UNLICENSED
 Project-URL: Repository, https://github.com/matmair/invenhost-core
 Project-URL: Bug Tracker, https://github.com/matmair/invenhost-core/issues
 Keywords: inventree,inventree-plugin,invenhost-core
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invenhost-core-0.1.0/README.md` & `invenhost-core-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `invenhost-core-0.1.0/pyproject.toml` & `invenhost-core-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2023 Matthias Mair<code@mjmair.com>
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invenhost-core"
-version =  "0.1.0"
+version =  "0.2.0"
 description="InvenHost integration plugin"
 readme = "README.md"
 license = {text = "UNLICENSED"}
 keywords = ["inventree", "inventree-plugin", "invenhost-core"]
 authors = [
     {name = "Matthias Mair", email =  "code@mjmair.com"}
 ]
```

### Comparing `invenhost-core-0.1.0/src/invenhost_core/InvenHostCore.py` & `invenhost-core-0.2.0/src/invenhost_core/InvenHostCore.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 
 import requests
 from django.conf.urls import url
 # from django.http import JsonResponse
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
+from InvenTree.config import get_plugin_file
 from plugin import InvenTreePlugin, registry
 from plugin.mixins import EventMixin, SettingsMixin, UrlsMixin
 
 logger = logging.getLogger('inventree')
 
 LICENSE_ACCOUNT = 'd61ba105-f3f1-40ac-8bd8-55d741bebf21'
 DEFAULT_HEADERS = {"Content-Type": "application/vnd.api+json", "Accept": "application/vnd.api+json"}
 
 
 def superuser_check(user):
     """Check if a user is a superuser."""
     return user.is_superuser
 
 
+# region licensing
 def set_license_setting(setting):
     """Check licensing key setting."""
     if setting is not None and setting.value is not None:
         key = setting.value
         check_license_online(key, setting.plugin.set_metadata)
+        setting.plugin.check_pugins_file(key)
 
 
 def check_license_online(key, set_fnc):
     """Check a licensing key online."""
     logger.info(f'Checking license key {key}')
     resp = requests.post(f'https://api.keygen.sh/v1/accounts/{LICENSE_ACCOUNT}/licenses/actions/validate-key', json={"meta": {"key": key}}, headers=DEFAULT_HEADERS)
     resp_data = resp.json()
@@ -56,14 +59,15 @@
         return plg.license_key_valid()
     return True
 
 
 def ready():
     """Return if the core is ready."""
     return core_is_active()
+# endregion
 
 
 class InvenHostCore(EventMixin, UrlsMixin, SettingsMixin, InvenTreePlugin):
     """InvenHost integration plugin."""
 
     NAME = 'InvenHostCore'
     SLUG = 'invenhost-core'
@@ -83,32 +87,50 @@
             'after_save': set_license_setting,
         },
     }
 
     def process_event(self, event, *args, **kwargs):
         """Process received events."""
         if event == 'plugins_loaded':
-            check_license_online(self.get_setting('LICENSE'), self.db.set_metadata)
+            key = self.get_setting('LICENSE')
+            check_license_online(key, self.db.set_metadata)
+            self.check_pugins_file(key)
 
     def license_key_valid(self):
         """Return if the license key is valid."""
         return self.db.get_metadata('inventree-core:license_valid', False)
 
     def license_key_data(self):
         """Return the license key data."""
         data = self.db.get_metadata('inventree-core:license_data', None)
         if data is not None and data != {}:
             return json.loads(data)
         return None
 
+    def check_pugins_file(self, key):
+        """Check if the source is set correctly in the plugin file."""
+        if ready():
+            logger.info(('License file check started'))
+            # Create license file
+            lic_url = f'https://license:{key}@get.keygen.sh/mjmair-com/stable/'
+            source = get_plugin_file()
+            plugin_text = source.read_text()
+            if lic_url not in plugin_text:
+                plugin_text += f'\n--extra-index-url {lic_url}\n'
+                source.write_text(plugin_text)
+                logger.info(('License file appended'))
+            logger.info(('License file check done'))
+
     def view_check(self, request, pk=None, led=None, context=None):
         """Register an LED."""
         if not superuser_check(request.user):
             raise PermissionError("Only superusers can register an instance.")
-        check_license_online(self.get_setting('LICENSE'), self.db.set_metadata)
+        key = self.get_setting('LICENSE')
+        check_license_online(key, self.db.set_metadata)
+        self.check_pugins_file(key)
         return redirect(self.settings_url)
 
     def setup_urls(self):
         """Return the URLs defined by this plugin."""
         return [
             url(r'check/', self.view_check, name='check'),
         ]
```

### Comparing `invenhost-core-0.1.0/src/invenhost_core.egg-info/PKG-INFO` & `invenhost-core-0.2.0/src/invenhost_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenhost-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: InvenHost integration plugin
 Author-email: Matthias Mair <code@mjmair.com>
 License: UNLICENSED
 Project-URL: Repository, https://github.com/matmair/invenhost-core
 Project-URL: Bug Tracker, https://github.com/matmair/invenhost-core/issues
 Keywords: inventree,inventree-plugin,invenhost-core
 Classifier: Programming Language :: Python :: 3
```

