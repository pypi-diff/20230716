# Comparing `tmp/dhooks_lite-1.0.0a1.tar.gz` & `tmp/dhooks_lite-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhooks_lite-1.0.0a1.tar", last modified: Tue Apr 18 15:42:42 2023, max compression
+gzip compressed data, was "dhooks_lite-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dhooks_lite-1.0.0a1.tar` & `dhooks_lite-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6360 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5180 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.229715 dhooks_lite-1.0.0a1/dhooks_lite/
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8414 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/client.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/dhooks_lite/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10914 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/embed.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-18 14:51:45.000000 dhooks_lite-1.0.0a1/dhooks_lite/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:42:42.229715 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6360 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 15:42:42.000000 dhooks_lite-1.0.0a1/dhooks_lite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:42:42.233715 dhooks_lite-1.0.0a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-18 15:23:27.000000 dhooks_lite-1.0.0a1/setup.py
+-rw-r--r--   0        0        0     1070 2023-07-16 11:54:05.121899 dhooks_lite-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5255 2023-07-16 12:42:39.080362 dhooks_lite-1.1.0/README.md
+-rw-r--r--   0        0        0      374 2023-07-16 13:19:05.757526 dhooks_lite-1.1.0/dhooks_lite/__init__.py
+-rw-r--r--   0        0        0     8723 2023-07-16 13:42:29.268283 dhooks_lite-1.1.0/dhooks_lite/client.py
+-rw-r--r--   0        0        0      143 2023-07-16 12:42:39.080362 dhooks_lite-1.1.0/dhooks_lite/constants.py
+-rw-r--r--   0        0        0    11834 2023-07-16 14:00:16.286616 dhooks_lite-1.1.0/dhooks_lite/embed.py
+-rw-r--r--   0        0        0      351 2023-07-16 12:42:39.080362 dhooks_lite-1.1.0/dhooks_lite/serializers.py
+-rw-r--r--   0        0        0     1900 2023-07-16 13:19:05.757526 dhooks_lite-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6706 1970-01-01 00:00:00.000000 dhooks_lite-1.1.0/PKG-INFO
```

### Comparing `dhooks_lite-1.0.0a1/LICENSE` & `dhooks_lite-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dhooks_lite-1.0.0a1/PKG-INFO` & `dhooks_lite-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
-Name: dhooks_lite
-Version: 1.0.0a1
-Summary: Another simple class wrapper for interacting with Discord webhooks in Python 3
-Home-page: https://github.com/ErikKalkoken/dhooks-lite
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Keywords: discord,webhooks,discordwebhooks,discordhooks
+Name: dhooks-lite
+Version: 1.1.0
+Summary: Another simple class wrapper for interacting with Discord webhooks.
+Keywords: discord,discordhooks,discordwebhooks,webhooks
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: requests
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://dhooks-lite.readthedocs.io/en/latest/
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/dhooks-lite
+Project-URL: Source, https://gitlab.com/ErikKalkoken/dhooks-lite
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/dhooks-lite/-/issues
 
 # dhooks-lite
 
+Another simple class wrapper for interacting with Discord webhooks.
+
 [![release](https://img.shields.io/pypi/v/dhooks-lite?label=release)](https://pypi.org/project/dhooks-lite/)
 [![python](https://img.shields.io/pypi/pyversions/dhooks-lite)](https://pypi.org/project/dhooks-lite/)
 [![pipeline status](https://gitlab.com/ErikKalkoken/dhooks-lite/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/commits/master)
 [![codecov](https://codecov.io/gl/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg?token=9YNL3HEJ5D)](https://codecov.io/gl/ErikKalkoken/dhooks-lite)
 [![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
@@ -42,26 +46,26 @@
 
 - [Overview](#overview)
 - [Functionality](#functionality)
 - [Examples](#examples)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Contribution](#contribution)
-- [Change Log](CHANGELOG.md)
 
 ## Overview
 
 **dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
 
 This library aims to differentiate itself from similar libraries with the following properties:
 
 - is fully tested
 - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
 - has logging
 - requests are automatically retried and have sensible timeouts
+- works with older Python versions
 
 ## Functionality
 
 This library provides following functionality:
 
 - Posting messages in Discord channels via webhooks (synchronous calls only)
 - Attaching Embeds to messages
@@ -169,7 +173,8 @@
 If you want to help further improve this library please feel free to issue a merge request. Please adhere to the following requirements in your change:
 
 - Code should be compliant with [PEP8](https://www.python.org/dev/peps/pep-0008/)
 - Full overage by unit tests
 - All classes should be immutable
 - All classes and their public methods must have docstring documentation
 - All changes must be documented in the Change Log
+
```

### Comparing `dhooks_lite-1.0.0a1/README.md` & `dhooks_lite-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # dhooks-lite
 
+Another simple class wrapper for interacting with Discord webhooks.
+
 [![release](https://img.shields.io/pypi/v/dhooks-lite?label=release)](https://pypi.org/project/dhooks-lite/)
 [![python](https://img.shields.io/pypi/pyversions/dhooks-lite)](https://pypi.org/project/dhooks-lite/)
 [![pipeline status](https://gitlab.com/ErikKalkoken/dhooks-lite/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/commits/master)
 [![codecov](https://codecov.io/gl/ErikKalkoken/dhooks-lite/branch/master/graph/badge.svg?token=9YNL3HEJ5D)](https://codecov.io/gl/ErikKalkoken/dhooks-lite)
 [![Documentation Status](https://readthedocs.org/projects/dhooks-lite/badge/?version=latest)](https://dhooks-lite.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/dhooks-lite/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
@@ -14,26 +16,26 @@
 
 - [Overview](#overview)
 - [Functionality](#functionality)
 - [Examples](#examples)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Contribution](#contribution)
-- [Change Log](CHANGELOG.md)
 
 ## Overview
 
 **dhooks-lite** is a library with a set of classes for interacting with Discord webhooks written in Python 3.
 
 This library aims to differentiate itself from similar libraries with the following properties:
 
 - is fully tested
 - simple to use (only one way of doing things, same name of attributes and objects as in the [official Discord documentation](https://discordapp.com/developers/docs/resources/webhook#execute-webhook))
 - has logging
 - requests are automatically retried and have sensible timeouts
+- works with older Python versions
 
 ## Functionality
 
 This library provides following functionality:
 
 - Posting messages in Discord channels via webhooks (synchronous calls only)
 - Attaching Embeds to messages
```

### Comparing `dhooks_lite-1.0.0a1/dhooks_lite/client.py` & `dhooks_lite-1.1.0/dhooks_lite/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from dhooks_lite.embed import Embed
+"""Client objects."""
+
 import json
 import logging
-import requests
 from time import sleep
 from typing import List, Optional
 
+import requests
+
+from dhooks_lite.embed import Embed
+
 from .constants import APP_NAME, APP_VERSION, HOMEPAGE_URL
 from .serializers import JsonDateTimeEncoder
 
-
 logger = logging.getLogger(__name__)
 
 REQUESTS_TIMEOUT = (5.0, 30.0)
 MAX_RETRIES = 3
 BACKOFF_FACTOR = 0.3
 
 HTTP_BAD_GATEWAY = 502
@@ -65,26 +68,29 @@
             version: Version of the application
         """
         self._name = str(name)
         self._url = str(url)
         self._version = str(version)
 
     def __str__(self) -> str:
-        return "{} ({}, {})".format(self.name, self.url, self.version)
+        return f"{self.name} ({self.url}, {self.version})"
 
     @property
     def name(self) -> str:
+        """Return user agent's name."""
         return self._name
 
     @property
     def url(self) -> str:
+        """Return user agent's URL."""
         return self._url
 
     @property
     def version(self) -> str:
+        """Return user agent's version."""
         return self._version
 
 
 class Webhook:
     """A Discord Webhook"""
 
     MAX_CHARACTERS = 2000
@@ -113,26 +119,30 @@
         self._user_agent = user_agent
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}(url='{self.url}'')"
 
     @property
     def url(self) -> str:
+        """Return URL for this webhook."""
         return self._url
 
     @property
     def username(self) -> Optional[str]:
+        """Return username for this webhook."""
         return self._username
 
     @property
     def avatar_url(self) -> Optional[str]:
+        """Return the avatar's URL for this webhook."""
         return self._avatar_url
 
     @property
     def user_agent(self) -> UserAgent:
+        """Return the user agent for this webhook."""
         return (
             self._user_agent
             if self._user_agent
             else UserAgent(APP_NAME, HOMEPAGE_URL, APP_VERSION)
         )
 
     def execute(
@@ -165,78 +175,59 @@
         Returns:
             response from webhook as WebhookResponse object
 
         """
         if not content and not embeds:
             raise ValueError("need content or embeds")
 
-        payload = dict()
+        payload = {}
         self._set_content(payload, content)
         self._set_embeds(payload, embeds)
         self._set_username(payload, username)
         self._set_avatar_url(payload, avatar_url)
         self._set_tts(payload, tts)
 
         retry_count = 0
-        r = None
-        for retry_count in range(int(max_retries) + 1):
-            logger.debug("Sending request to '%s' with payload: %s", self._url, payload)
-            params = {"wait": bool(wait_for_response)}
-            headers = {
-                "Content-Type": "application/json",
-                "User-Agent": str(self.user_agent),
-            }
-            data = json.dumps(payload, cls=JsonDateTimeEncoder)
-            r = requests.post(
-                url=self._url,
-                params=params,
-                headers=headers,
-                data=data,
-                timeout=REQUESTS_TIMEOUT,
-            )
-            if not r.ok:
-                logger.warning("HTTP status code: %s", r.status_code)
-            else:
-                logger.debug("HTTP status code: %s", r.status_code)
-
-            logger.debug("Response headers from Discord: %s", r.headers)
-            logger.debug("Response from Discord: %s", r.content)
+        while True:
+            r = self._send_request_to_webhook(payload, bool(wait_for_response))
+            if r.ok:
+                break
 
             if r.status_code in [
                 HTTP_BAD_GATEWAY,
                 HTTP_GATEWAY_TIMEOUT,
                 HTTP_SERVICE_UNAVAILABLE,
             ]:
                 retry_count += 1
-                if retry_count <= max_retries:
-                    logger.warning("Retry %d / %d", retry_count, max_retries)
-                    if retry_count > 1:
-                        wait_secs = BACKOFF_FACTOR * (2 ** (retry_count - 1))
-                        sleep(wait_secs)
+                if retry_count > max_retries:
+                    break
+
+                logger.warning("Retry %d / %d", retry_count, max_retries)
+                if retry_count > 1:
+                    wait_secs = BACKOFF_FACTOR * (2 ** (retry_count - 1))
+                    sleep(wait_secs)
+
             else:
                 break
 
-        if r is None:
-            raise RuntimeError("No request object")  # this should never be reached
-
         try:
             content_returned = r.json()
         except ValueError:
             content_returned = None
 
         response = WebhookResponse(
             headers=dict(r.headers), status_code=r.status_code, content=content_returned
         )
         return response
 
     def _set_content(self, payload: dict, content: Optional[str]) -> None:
         if content:
             content = str(content)
             if len(content) > self.MAX_CHARACTERS:
-                raise ValueError("content exceeds {}".format(self.MAX_CHARACTERS))
+                raise ValueError(f"content exceeds {self.MAX_CHARACTERS}")
             payload["content"] = content
 
     def _set_embeds(self, payload: dict, embeds: Optional[list]) -> None:
         if embeds:
             if not isinstance(embeds, list):
                 raise TypeError("embeds must be of type list")
 
@@ -262,7 +253,31 @@
 
     def _set_tts(self, payload: dict, tts: Optional[bool]) -> None:
         if tts is not None:
             if not isinstance(tts, bool):
                 raise TypeError("tts must be of type bool")
 
             payload["tts"] = tts
+
+    def _send_request_to_webhook(self, payload: dict, wait_for_response: bool):
+        logger.debug("Sending request to '%s' with payload: %s", self._url, payload)
+        params = {"wait": wait_for_response}
+        headers = {
+            "Content-Type": "application/json",
+            "User-Agent": str(self.user_agent),
+        }
+        data = json.dumps(payload, cls=JsonDateTimeEncoder)
+        r = requests.post(
+            url=self._url,
+            params=params,
+            headers=headers,
+            data=data,
+            timeout=REQUESTS_TIMEOUT,
+        )
+        if not r.ok:
+            logger.warning("HTTP status code: %s", r.status_code)
+        else:
+            logger.debug("HTTP status code: %s", r.status_code)
+
+        logger.debug("Response headers from Discord: %s", r.headers)
+        logger.debug("Response from Discord: %s", r.content)
+        return r
```

### Comparing `dhooks_lite-1.0.0a1/dhooks_lite/embed.py` & `dhooks_lite-1.1.0/dhooks_lite/embed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+"""Discord Embed."""
+
+import json
 import logging
 from datetime import datetime
-import json
-from typing import Any, List, get_type_hints, Union, Optional
+from typing import Any, List, Optional, Union, get_type_hints
 
 from .serializers import JsonDateTimeEncoder
 
 logger = logging.getLogger(__name__)
 
 
 class _EmbedObject:
@@ -25,48 +27,48 @@
         return not self.__eq__(other)
 
     def asdict(self) -> dict:
         """returns a dict representation of this object
 
         will not include properties that are None
         """
-        arr = dict()
+        arr = {}
         for key, value in self.__dict__.items():
             if value is not None:
                 if isinstance(value, list):
-                    v_list = list()
+                    v_list = []
                     for elem in value:
                         if isinstance(elem, _EmbedObject):
                             v_list.append(elem.asdict())
                         else:
                             raise NotImplementedError()
                     arr[key[1:]] = v_list
                 else:
                     if isinstance(value, _EmbedObject):
                         arr[key[1:]] = value.asdict()
                     else:
                         arr[key[1:]] = value
         return arr
 
     @classmethod
-    def from_dict(cls, obj_dict: dict) -> "_EmbedObject":
+    def from_dict(cls, obj_dict: dict):
         """creates a new object from the given dict"""
-        args = dict()
+        args = {}
         for param_name, param_type in get_type_hints(cls.__init__).items():
             if param_name in obj_dict and param_name != "return":
                 if hasattr(param_type, "__origin__") and param_type.__origin__ == Union:
                     param_type = param_type.__args__[0]
                 try:
                     origin_type = param_type.__origin__
                 except AttributeError:
                     origin_type = param_type
 
                 if issubclass(origin_type, list):
-                    MyType = list(param_type.__args__).pop()
-                    value = [MyType(**obj) for obj in obj_dict[param_name]]
+                    my_type = list(param_type.__args__).pop()
+                    value = [my_type(**obj) for obj in obj_dict[param_name]]
 
                 elif issubclass(origin_type, _EmbedObject):
                     value = param_type.from_dict(obj_dict[param_name])
 
                 else:
                     value = obj_dict[param_name]
 
@@ -91,26 +93,30 @@
         self._name = str(name)
         self._url = str(url) if url else None
         self._icon_url = str(icon_url) if icon_url else None
         self._proxy_icon_url = str(proxy_icon_url) if proxy_icon_url else None
 
     @property
     def name(self) -> str:
+        """Return author name."""
         return self._name
 
     @property
     def url(self) -> Optional[str]:
+        """Return author URL."""
         return self._url
 
     @property
     def icon_url(self) -> Optional[str]:
+        """Return author's icon URL."""
         return self._icon_url
 
     @property
     def proxy_icon_url(self) -> Optional[str]:
+        """Return author's proxy icon URL."""
         return self._proxy_icon_url
 
 
 class Field(_EmbedObject):
     """Field in an Embed"""
 
     MAX_CHARACTERS_NAME = 256
@@ -123,36 +129,39 @@
             raise ValueError("value can not be None")
         if not isinstance(inline, bool):
             raise TypeError("inline must be of type bool")
 
         name = str(name)
         if len(name) > self.MAX_CHARACTERS_NAME:
             raise ValueError(
-                "name can not exceed {} characters".format(self.MAX_CHARACTERS_NAME)
+                f"name can not exceed {self.MAX_CHARACTERS_NAME} characters"
             )
         value = str(value)
         if len(value) > self.MAX_CHARACTERS_VALUE:
             raise ValueError(
-                "value can not exceed {} characters".format(self.MAX_CHARACTERS_VALUE)
+                f"value can not exceed {self.MAX_CHARACTERS_VALUE} characters"
             )
 
         self._name = name
         self._value = value
         self._inline = inline
 
     @property
     def name(self) -> str:
+        """Return field name."""
         return self._name
 
     @property
     def value(self) -> str:
+        """Return field value."""
         return self._value
 
     @property
     def inline(self) -> Optional[bool]:
+        """Return field inline."""
         return self._inline
 
 
 class Footer(_EmbedObject):
     """Footer in an Embed"""
 
     def __init__(
@@ -166,22 +175,25 @@
 
         self._text = str(text)
         self._icon_url = str(icon_url) if icon_url else None
         self._proxy_icon_url = str(proxy_icon_url) if proxy_icon_url else None
 
     @property
     def text(self) -> str:
+        """Return Footer text."""
         return self._text
 
     @property
     def icon_url(self) -> Optional[str]:
+        """Return footer's icon URL."""
         return self._icon_url
 
     @property
     def proxy_icon_url(self) -> Optional[str]:
+        """Return footer's proxy icon URL."""
         return self._proxy_icon_url
 
 
 class Image(_EmbedObject):
     """Image in an Embed"""
 
     def __init__(
@@ -201,35 +213,41 @@
         self._url = str(url)
         self._proxy_url = str(proxy_url) if proxy_url else None
         self._height = int(height) if height else None
         self._width = int(width) if width else None
 
     @property
     def url(self) -> str:
+        """Return image URL."""
         return self._url
 
     @property
     def proxy_url(self) -> Optional[str]:
+        """Return image's proxy URL."""
         return self._proxy_url
 
     @property
     def height(self) -> Optional[int]:
+        """Return image height."""
         return self._height
 
     @property
     def width(self) -> Optional[int]:
+        """Return image width."""
         return self._width
 
 
 class Thumbnail(Image):
-    """Thumbnail in an Embed"""
+    """Thumbnail in an Embed."""
 
 
 class Embed(_EmbedObject):
-    """Embedded content for a message"""
+    """Embedded content for a message."""
+
+    # pylint: disable=too-many-instance-attributes
 
     MAX_CHARACTERS = 6000
     MAX_TITLE = 256
     MAX_DESCRIPTION = 2048
     MAX_FIELDS = 25
 
     def __init__(
@@ -262,44 +280,44 @@
         Exceptions:
             TypeException: when passing variables of wrong type
             ValueException: when embed size exceeds hard limit
 
         """
         if timestamp and not isinstance(timestamp, datetime):
             raise TypeError("timestamp must be a datetime object")
+
         if footer and not isinstance(footer, Footer):
             raise TypeError("footer must be a Footer object")
+
         if image and not isinstance(image, Image):
             raise TypeError("image must be an Image object")
+
         if thumbnail and not isinstance(thumbnail, Thumbnail):
             raise TypeError("thumbnail must be a Thumbnail object")
+
         if author and not isinstance(author, Author):
             raise TypeError("author must be a Author object")
+
         if fields and not isinstance(fields, list):
             raise TypeError("fields must be a list")
+
         if fields:
             if len(fields) > self.MAX_FIELDS:
-                raise ValueError(
-                    "Fields can not exceed {} objects".format(self.MAX_FIELDS)
-                )
-            for f in fields:
-                if not isinstance(f, Field):
+                raise ValueError(f"Fields can not exceed {self.MAX_FIELDS} objects")
+            for field in fields:
+                if not isinstance(field, Field):
                     raise TypeError("all elements in fields must be a Field")
 
         if description and len(description) > self.MAX_DESCRIPTION:
             raise ValueError(
-                "description exceeds max length of {} characters".format(
-                    self.MAX_DESCRIPTION
-                )
+                f"description exceeds max length of {self.MAX_DESCRIPTION} characters"
             )
 
         if title and len(title) > self.MAX_TITLE:
-            raise ValueError(
-                "title exceeds max length of {} characters".format(self.MAX_TITLE)
-            )
+            raise ValueError(f"title exceeds max length of {self.MAX_TITLE} characters")
 
         self._title = str(title) if title else None
         self._type = "rich"
         self._description = str(description) if description else None
         self._url = str(url) if url else None
         self._timestamp = timestamp
         self._color = int(color) if color else None
@@ -307,56 +325,67 @@
         self._image = image
         self._thumbnail = thumbnail
         self._author = author
         self._fields = fields
 
         d_json = json.dumps(self.asdict(), cls=JsonDateTimeEncoder)
         if len(d_json) > self.MAX_CHARACTERS:
+            limit = len(d_json) - self.MAX_CHARACTERS
             raise ValueError(
-                "Embed exceeds maximum allowed char size of {} by {}".format(
-                    self.MAX_CHARACTERS, len(d_json) - self.MAX_CHARACTERS
-                )
+                f"Embed exceeds maximum allowed char size of {self.MAX_CHARACTERS} "
+                f"by {limit}"
             )
 
     @property
     def description(self) -> Optional[str]:
+        """Return embed's description."""
         return self._description
 
     @property
     def title(self) -> Optional[str]:
+        """Return embed's title or None."""
         return self._title
 
     @property
     def type(self) -> Optional[str]:
+        """Return embed's type or None."""
         return self._type
 
     @property
     def url(self) -> Optional[str]:
+        """Return embed's URL or None."""
         return self._url
 
     @property
     def timestamp(self) -> Optional[datetime]:
+        """Return embed's timestamp or None."""
         return self._timestamp
 
     @property
     def color(self) -> Optional[int]:
+        """Return embed's color or None."""
         return self._color
 
     @property
     def footer(self) -> Optional[Footer]:
+        """Return embed's footer or None."""
         return self._footer
 
     @property
     def image(self) -> Optional[Image]:
+        """Return embed's image or None."""
         return self._image
 
     @property
     def thumbnail(self) -> Optional[Thumbnail]:
+        """Return embed's thumbnail or None."""
         return self._thumbnail
 
     @property
     def author(self) -> Optional[Author]:
+        """Return embed's author or None."""
         return self._author
 
     @property
     def fields(self) -> Optional[List[Field]]:
+        """Return embed's fields or None."""
         return self._fields
```

