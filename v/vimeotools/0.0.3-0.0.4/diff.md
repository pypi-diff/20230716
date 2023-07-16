# Comparing `tmp/vimeotools-0.0.3.tar.gz` & `tmp/vimeotools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vimeotools-0.0.3.tar", last modified: Thu Jul 13 18:40:32 2023, max compression
+gzip compressed data, was "dist/vimeotools-0.0.4.tar", last modified: Sun Jul 16 10:59:40 2023, max compression
```

## Comparing `vimeotools-0.0.3.tar` & `vimeotools-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.549229 vimeotools-0.0.3/
--rw-r--r--   0 georg      (502) staff       (20)     3268 2023-07-13 18:40:32.549522 vimeotools-0.0.3/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.3/README.md
--rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-13 18:40:32.550680 vimeotools-0.0.3/setup.cfg
--rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.3/setup.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.536781 vimeotools-0.0.3/src/
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.544996 vimeotools-0.0.3/src/vimeotools/
--rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.3/src/vimeotools/__init__.py
--rw-r--r--   0 georg      (502) staff       (20)    14614 2023-07-13 10:51:12.000000 vimeotools-0.0.3/src/vimeotools/vimeo_base.py
--rw-r--r--   0 georg      (502) staff       (20)     1597 2023-07-13 04:27:52.000000 vimeotools-0.0.3/src/vimeotools/vimeo_connection.py
--rw-r--r--   0 georg      (502) staff       (20)    19344 2023-07-13 09:54:51.000000 vimeotools-0.0.3/src/vimeotools/vimeo_constants.py
--rw-r--r--   0 georg      (502) staff       (20)    34543 2023-07-13 18:33:41.000000 vimeotools-0.0.3/src/vimeotools/vimeo_data.py
--rw-r--r--   0 georg      (502) staff       (20)     9041 2023-07-13 18:15:06.000000 vimeotools-0.0.3/src/vimeotools/vimeo_folder.py
--rw-r--r--   0 georg      (502) staff       (20)    11963 2023-07-13 18:25:06.000000 vimeotools-0.0.3/src/vimeotools/vimeo_showcase.py
--rw-r--r--   0 georg      (502) staff       (20)    12553 2023-07-13 05:54:15.000000 vimeotools-0.0.3/src/vimeotools/vimeo_video.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-13 18:40:32.548613 vimeotools-0.0.3/src/vimeotools.egg-info/
--rw-r--r--   0 georg      (502) staff       (20)     3268 2023-07-13 18:40:31.000000 vimeotools-0.0.3/src/vimeotools.egg-info/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/SOURCES.txt
--rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-13 18:40:31.000000 vimeotools-0.0.3/src/vimeotools.egg-info/dependency_links.txt
--rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/requires.txt
--rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-13 18:40:32.000000 vimeotools-0.0.3/src/vimeotools.egg-info/top_level.txt
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-16 10:59:40.330845 vimeotools-0.0.4/
+-rw-r--r--   0 georg      (502) staff       (20)     3636 2023-07-16 10:59:40.331119 vimeotools-0.0.4/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)     1229 2023-07-08 16:58:08.000000 vimeotools-0.0.4/README.md
+-rw-r--r--   0 georg      (502) staff       (20)      806 2023-07-16 10:59:40.332060 vimeotools-0.0.4/setup.cfg
+-rw-r--r--   0 georg      (502) staff       (20)       69 2023-07-07 15:14:58.000000 vimeotools-0.0.4/setup.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-16 10:59:40.319771 vimeotools-0.0.4/src/
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-16 10:59:40.327445 vimeotools-0.0.4/src/vimeotools/
+-rw-r--r--   0 georg      (502) staff       (20)      335 2023-07-07 15:14:58.000000 vimeotools-0.0.4/src/vimeotools/__init__.py
+-rw-r--r--   0 georg      (502) staff       (20)    16218 2023-07-16 10:50:01.000000 vimeotools-0.0.4/src/vimeotools/vimeo_base.py
+-rw-r--r--   0 georg      (502) staff       (20)     1597 2023-07-13 04:27:52.000000 vimeotools-0.0.4/src/vimeotools/vimeo_connection.py
+-rw-r--r--   0 georg      (502) staff       (20)    19720 2023-07-16 06:14:38.000000 vimeotools-0.0.4/src/vimeotools/vimeo_constants.py
+-rw-r--r--   0 georg      (502) staff       (20)    35472 2023-07-16 07:47:45.000000 vimeotools-0.0.4/src/vimeotools/vimeo_data.py
+-rw-r--r--   0 georg      (502) staff       (20)     9041 2023-07-13 18:15:06.000000 vimeotools-0.0.4/src/vimeotools/vimeo_folder.py
+-rw-r--r--   0 georg      (502) staff       (20)    12084 2023-07-16 10:25:27.000000 vimeotools-0.0.4/src/vimeotools/vimeo_showcase.py
+-rw-r--r--   0 georg      (502) staff       (20)    12553 2023-07-13 05:54:15.000000 vimeotools-0.0.4/src/vimeotools/vimeo_video.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-07-16 10:59:40.330405 vimeotools-0.0.4/src/vimeotools.egg-info/
+-rw-r--r--   0 georg      (502) staff       (20)     3636 2023-07-16 10:59:39.000000 vimeotools-0.0.4/src/vimeotools.egg-info/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      465 2023-07-16 10:59:40.000000 vimeotools-0.0.4/src/vimeotools.egg-info/SOURCES.txt
+-rw-r--r--   0 georg      (502) staff       (20)        1 2023-07-16 10:59:39.000000 vimeotools-0.0.4/src/vimeotools.egg-info/dependency_links.txt
+-rw-r--r--   0 georg      (502) staff       (20)        8 2023-07-16 10:59:40.000000 vimeotools-0.0.4/src/vimeotools.egg-info/requires.txt
+-rw-r--r--   0 georg      (502) staff       (20)       11 2023-07-16 10:59:40.000000 vimeotools-0.0.4/src/vimeotools.egg-info/top_level.txt
```

### Comparing `vimeotools-0.0.3/PKG-INFO` & `vimeotools-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,14 +40,21 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.4 (2023-07-16)
+- **VimeoBaseItem**: method **set_temp_data** (for use in Restricted Python where methods with the setter-decorator do not work because attributes cannot be changed)
+- **VimeoBaseItem**: new attribute *\_temp_attributes* for storing volatile "attributes" on the object and the methods needed:
+	- get_attribute
+	- get_attributes
+	- set_attribute
+
 ## 0.0.3 (2023-07-13)
 - **VimeoShocase** und **VimeoFolder**: property **nb_videos**
 - **VimeoData** changed property names
 	- video_count -> nb_videos
 	- showcases_count -> nb_showcases
 	- folders_count -> nb_folders
```

### Comparing `vimeotools-0.0.3/README.md` & `vimeotools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.3/setup.cfg` & `vimeotools-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vimeotools
-version = 0.0.3
+version = 0.0.4
 author = Georg Pfolz
 author_email = georg.pfolz@invesy.at
 description = Tools for Vimeo
 long_description = file: README.md,HISTORY.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
```

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_base.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 """
 =============================
 Vimeo Tools Vimeo Base Module
 =============================
 
 This module contains the base classes VimeoChild and VimeoItem, as well as
 functions used by the other classes.
+
+:Author: Georg Pfolz
+
+Concering names used for variables and functions:
+    - The term "property" is used for the data coming from returned by the Vimeo API.
+      It's what's called "parameters" in the Vimeo API documentation.
+    - The term "attribute" is used for the data stored in the VimeoItem objects.
+      These are temporary data that are lost when the object is deleted.
 """
 
 from typing import TYPE_CHECKING, Dict, Optional, List, Union, Any, Literal
 import json
 from vimeo_constants import (
     GETTER_STR,
     SETTER_STR,
@@ -21,14 +29,17 @@
     from vimeo_folder import VimeoFolder
     from vimeo_connection import VimeoConnection
     from vimeo_data import VimeoData
 
 def transform_returning(
     returning: str
 ) -> str:
+    if not returning:
+        return ''
+    
     returning = returning.lower()
 
     try:
         return RETURNING_MAP[returning]
     except KeyError:
         raise ValueError(f'Unknown value for returning: {returning}')
 
@@ -257,14 +268,18 @@
     @property
     def temp_data(self) -> Dict[str, Any]:
         return self._temp_data
     
     @temp_data.setter
     def temp_data(self, value: Dict[str, Any]) -> None:
         self._temp_data = value
+    
+    @property
+    def attributes(self) -> Dict[str, Any]:
+        return self._temp_attributes
 
     for key, val in PROPERTIES_BASE.items():
         exec(GETTER_STR.format(prop=key))
         if val['type'] == 'str' and val.get('setable'):
             key = val.get('set_key', key)
             exec(SETTER_STR.format(prop=key))
 
@@ -276,14 +291,21 @@
         data: Optional[Dict[str, Any]] = None,
         data_object: Optional['VimeoData'] = None
     ):
         self.connection = connection
         self.client = connection.client
         self._live = live
         self._temp_data = {}  # temporary data storage for the object
+
+        # temporary properties storage for the object
+        # this may seem a bit redundant with _temp_data, but this way,
+        # _temp_data can be overwritten without consideration for the
+        # properties that are stored in _temp_attributes
+        self._temp_attributes = {}
+
         data_object = data_object
 
         if data_object and not data:
             data = data_object._data
 
         if data:
             self._data = data
@@ -306,32 +328,43 @@
         allowed_keys = [key.split(' ')[0] for key in self.allowed_keys_to_set] # type: ignore (in child class)
 
         if key in allowed_keys:
             return True
         
         return False
 
+    def get_attribute(
+        self,
+        name: str
+    ) -> Any:
+        return self._temp_attributes.get(name, None)
+    
+    def get_attributes(
+        self
+    ) -> Dict[str, Any]:
+        return self._temp_attributes
+
     def set_property(
         self,
-        key: str,
+        name: str,
         value: Any
     ):
         """
         Set a property of the item. The property must be setable.
 
         :param key: The key can be provided in dotted notation, e.g. "privacy.view"
         :param value: The value to set
         """
-        if not self._keys_is_allowed_to_set(key=key):
+        if not self._keys_is_allowed_to_set(key=name):
             raise ValueError(
-                f'Invalid key "{key}". Allowed keys are: {self.allowed_keys_to_set}' # type: ignore (in child class)
+                f'Invalid key "{name}". Allowed keys are: {self.allowed_keys_to_set}' # type: ignore (in child class)
             )
         
         uri = self.uri  # from the child class
-        update_data = denest_key(key, value)
+        update_data = denest_key(name, value)
         
         # client also comes from the child class
         response = self.client.patch(
             uri,
             data=update_data
         )
         
@@ -465,14 +498,33 @@
     def description(self):
         return self.get_property('description')
     
     @description.setter
     def description(self, value: str):
         self.set_property('description', value)
 
+    def set_temp_data(self, value: Dict[str, Any]) -> None:
+        """
+        despite there begin a setter, this is needed to set
+        temp_data from Restricted Python (Zope)
+        """
+        self._temp_data = value
+
+    def set_attribute(
+        self,
+        name: str,
+        value: Any
+    ) -> None:
+        """
+        This stores temporary attributes in the object. This is useful
+        for storing data that's needed e.g. for program logic but not to
+        be stored on Vimeo.
+        """
+        self._temp_attributes[name] = value
+
     def store_json(
         self,
         path: Optional[str] = None,
         refresh: bool = False
     ):
         """
         Store data as a json file.
```

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_connection.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_connection.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_constants.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+import json
+import pickle
 """
 =====================
 Vimeo Tools Constants
 =====================
 
 This module contains constants used by the Vimeo Tools package.
 """
@@ -16,14 +18,32 @@
 SETTER_STR = """
 @{prop}.setter
 def {prop}(self, value: str):
     self._data['{prop}'] = value
     self.set_property('{set_key}', value)
 """
 
+# this might be a little bit silly ;)
+SAVE_FMT_MAP = {
+    'json': {
+        'suffix': '.json',
+        'dump': json.dump,
+        'mode': 'w',
+        'kwargs': {
+            'indent': 4
+        }
+    },
+    'pickle': {
+        'suffix': '.pickle',
+        'dump': pickle.dump,
+        'mode': 'wb',
+        'kwargs': {}
+    }
+}
+
 # properties that are common to VimeoVideo, VimeoShowcase, VimeoFolder
 
 PROPERTIES_BASE = {
     'name': {'type': str, 'setable': True},
     'created_time': {'type': str},
     'modified_time': {'type': str},
     'duration': {'type': int},
@@ -326,14 +346,15 @@
     'account': ACCOUNT_MIN_IGNORE,
     'videos': VIDEOS_MIN_IGNORE,
     'albums': SHOWCASES_MIN_IGNORE,
     'projects': FOLDER_MIN_IGNORE
 }
 
 WHAT_MAP = {
+    'all': 'all',
     'account': 'account',
     'video': 'videos',
     'videos': 'videos',
     'album': 'albums',
     'albums': 'albums',
     'showcase': 'albums',
     'showcases': 'albums',
@@ -364,8 +385,8 @@
     'account': 'object',
     'code': 'code',
     'codes': 'code',
     'uri': 'uri',
     'uris': 'uri',
     'json': 'json',
     'lines': 'lines'
-}
+}
```

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_data.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 information about a Vimeo account and its videos, folders and albums.
 """
 from typing import TYPE_CHECKING, Dict, Optional, List, Union, Any, Literal
 from pathlib import Path
 import json
 import pickle
 from vimeo_constants import (
-    MIN_KEYS
+    MIN_KEYS,
+    SAVE_FMT_MAP
 )
 from vimeo_base import (
     get_lines,
     nested_value,
     transform_returning,
     transform_what
 )
@@ -154,17 +155,16 @@
             'dict',
             'list',
             'json',
             'code',
             'codes',
             'uri',
             'uris',
-            'None',
-            None
-        ] = None,
+            'None'
+        ] = 'object',
         refresh: bool = False
     ) -> Union[
             Dict[str, Any],
             List[Dict[str, Any]], List[VimeoVideo], List[VimeoShowcase],
             str,
             None  # ValueError
         ]:
@@ -174,29 +174,27 @@
         :param localpath: If it exists, fetches data from local file.
         :param returning:
         - If 'dict', returns the video data as a dict, as provided by Vimeo.
         - If 'list', returns a list of dicts (one dict per video, as in the 'data' key of the Vimeo response)
         - If 'json', returns a json string.
         """
         # set returning to singular
-        returning = transform_returning(returning=returning)  # type: ignore
+        returning = transform_returning(returning=returning)
 
         data = {'data': []}
 
         data_stored = self._data_stored(what=what)
         items_stored = self._items_stored(what=what)
         
         if not refresh:
             if returning == 'dict' and data_stored:
                 return data_stored
             elif returning == 'object' and items_stored:
-
                 return items_stored
 
-        if not refresh:
             if what == 'videos' and self._videos_data:
                 data['data'] = self._videos_data.get('data', [])
             elif what == 'albums' and self._albums_data:
                 data['data'] = self._albums_data.get('data', [])
             elif what == 'projects' and self._folders_data:
                 data['data'] = self._folders_data.get('data', [])
         
@@ -783,14 +781,22 @@
 
     def load(
         self,
         file: Union[Path, str] = Path('vimeo_data.json'),
         format: Optional[Literal['json', 'pickle']] = None,
         refresh: bool = False
     ) -> None:
+        """
+        Load the data from a file.
+
+        :param file: Path or str
+        :param format: 'js
+        :param refresh: bool
+        :return: None
+        """
         if isinstance(file, str):
             file = Path(file)
 
         if not file.exists():
             raise FileNotFoundError(f'File not found: {file}')
         
         if not format:
@@ -811,15 +817,15 @@
         self._data = data
 
         # redundant!
         self._account_data = data['account']
         self._videos_data = data['videos']
         self._folders_data = data['projects']
         self._albums_data = data['albums']
-        
+
     @property
     def nb_folders(
         self
     ) -> int:
         """
         Get the number of folders.
         """
@@ -847,27 +853,49 @@
         Get the number of videos.
         :param refresh: bool
         :return: int
         """
         return self.get_count(
             what='videos'
         )
+
+    reload = load  # alias, reload might be more explicit and intuitive in some cases
+    """
+    Load the data from a file.
+
+    :param file: Path or str
+    :param format: 'js
+    :param refresh: bool
+    :return: None
+
+    Alias for load.
+
+    Its purpose is to reload the data from a file if the data might have been modified,
+    but the object is still the same (such as in a module from which functions are imported,
+    but the data object is not created anew each time)
+    """
     
     def refresh(
         self,
         what: Literal[
             'videos',
             'albums',
             'showcases',
             'account',
             'all'
         ] = 'all'
     ) -> None:
         """
         Refresh data.
+
+        :param what: str
+        :param live: bool
+        :return: None
+
+        Fetching data from the API (live)
         """
         what = transform_what(what) # type: ignore
 
         if what in ('account', 'all'):
             self._get_account_data(
                 refresh=True
             )
@@ -1025,23 +1053,31 @@
         return self.get_videos(
             returning='objects'
         ) # type: ignore
 
     def save(
         self,
         file: Union[Path, str] = Path('vimeo_data.json'),
-        format: Optional[Literal['json', 'pickle']] = None,
+        format: Optional[
+            Union[
+                Literal['json', 'pickle'],
+                List[Literal['json', 'pickle']]
+            ]
+        ] = None,
         refresh: bool = False
     ) -> None:
         if isinstance(file, str):
             file = Path(file)
         
         if not format:
             format = file.suffix[1:]  # type: ignore (impossible that it's not a Path)
 
+        if isinstance(format, str):
+            format = [format]
+
         data_to_save = {
             'account': self._get_account_data(
                 returning='dict',
                 refresh=refresh
             ),
             'videos': self._get_items(
                 what='videos',
@@ -1055,24 +1091,23 @@
             ),
             'projects': self.get_folders(
                 returning='dict',
                 refresh=refresh
             )
         }
 
-        print(f'Saving data to {file}...')
-        
-        if format == 'json':
-            with open(file, 'w') as f:
-                json.dump(data_to_save, f, indent=4)
-        elif format == 'pickle':
-            with open(file, 'wb') as f:
-                pickle.dump(data_to_save, f)
-        else:
-            raise ValueError(f'Unknown format: {format}')
+        for fmt in format:  # type: ignore (at this point, format is a list)
+            # change file suffix to format
+
+            file = file.with_suffix(SAVE_FMT_MAP[fmt]['suffix'])
+
+            print(f'Saving data to {file}...')
+
+            with open(file, SAVE_FMT_MAP[fmt]['mode']) as f:
+                SAVE_FMT_MAP[fmt]['dump'](data_to_save, f, **SAVE_FMT_MAP[fmt]['kwargs'])
 
     def show_account(
         self,
         mode: str = 'default',
         ignore_keys: List[str] = [],
         show_keys: List[str] = [],
         indent: int = 0,
```

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_folder.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_folder.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_showcase.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_showcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,20 @@
         if videos:
             for video in videos:
                 lines.append(f'    - {video.name} ({video.code})') # type: ignore
 
         lines.append(f'  - more keys: ' + ', '.join(ignore_keys))
         return '\n'.join(lines)
 
+    def get_test_data(self):
+        """
+        Get test data for the showcase.
+        """
+        return 'TEST DATA'
+
     def add_logo(
         self,
         picture: str
     ):
         """
         Add a logo to the showcase.
         """
```

### Comparing `vimeotools-0.0.3/src/vimeotools/vimeo_video.py` & `vimeotools-0.0.4/src/vimeotools/vimeo_video.py`

 * *Files identical despite different names*

### Comparing `vimeotools-0.0.3/src/vimeotools.egg-info/PKG-INFO` & `vimeotools-0.0.4/src/vimeotools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vimeotools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for Vimeo
 Home-page: https://github.com/georgpfolz/vimeotools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/georgpfolz/vimeotools/issues
 Project-URL: Documentation, https://georgpfolz.github.io/vimeotools
@@ -40,14 +40,21 @@
 
 You can also opt to create or set an object in live mode, so everytime a property is queried, the appropriate request is made on Vimeo first.
 
 ## documentation
 The (Sphinx) documentation is very crude (created with autodoc) currently and will be improved in subsequent versions.
 
 # History
+## 0.0.4 (2023-07-16)
+- **VimeoBaseItem**: method **set_temp_data** (for use in Restricted Python where methods with the setter-decorator do not work because attributes cannot be changed)
+- **VimeoBaseItem**: new attribute *\_temp_attributes* for storing volatile "attributes" on the object and the methods needed:
+	- get_attribute
+	- get_attributes
+	- set_attribute
+
 ## 0.0.3 (2023-07-13)
 - **VimeoShocase** und **VimeoFolder**: property **nb_videos**
 - **VimeoData** changed property names
 	- video_count -> nb_videos
 	- showcases_count -> nb_showcases
 	- folders_count -> nb_folders
```

