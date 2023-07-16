# Comparing `tmp/unkey_py-0.2.0.tar.gz` & `tmp/unkey_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unkey_py-0.2.0.tar", max compression
+gzip compressed data, was "unkey_py-0.3.0.tar", max compression
```

## Comparing `unkey_py-0.2.0.tar` & `unkey_py-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-25 00:52:34.797648 unkey_py-0.2.0/LICENSE
--rw-r--r--   0        0        0     1851 2023-06-25 00:52:34.797648 unkey_py-0.2.0/README.md
--rw-r--r--   0        0        0     2262 2023-06-25 00:52:34.797648 unkey_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1399 2023-06-25 00:52:34.881647 unkey_py-0.2.0/unkey/__init__.py
--rw-r--r--   0        0        0      643 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/__main__.py
--rw-r--r--   0        0        0     2492 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/client.py
--rw-r--r--   0        0        0      332 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/constants.py
--rw-r--r--   0        0        0      434 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/errors.py
--rw-r--r--   0        0        0      274 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/__init__.py
--rw-r--r--   0        0        0      729 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/apis.py
--rw-r--r--   0        0        0     1615 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/base.py
--rw-r--r--   0        0        0      388 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/http.py
--rw-r--r--   0        0        0     2393 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/models/keys.py
--rw-r--r--   0        0        0        0 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/py.typed
--rw-r--r--   0        0        0     2230 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/result.py
--rw-r--r--   0        0        0     2089 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/routes.py
--rw-r--r--   0        0        0     3445 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/serializer.py
--rw-r--r--   0        0        0      151 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/__init__.py
--rw-r--r--   0        0        0     1833 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/apis.py
--rw-r--r--   0        0        0     1229 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/base.py
--rw-r--r--   0        0        0     4331 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/http.py
--rw-r--r--   0        0        0     3459 2023-06-25 00:52:34.797648 unkey_py-0.2.0/unkey/services/keys.py
--rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 unkey_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-16 16:38:10.043501 unkey_py-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1851 2023-07-16 16:38:10.043501 unkey_py-0.3.0/README.md
+-rw-r--r--   0        0        0     2311 2023-07-16 16:38:10.043501 unkey_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1416 2023-07-16 16:38:10.155500 unkey_py-0.3.0/unkey/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/__main__.py
+-rw-r--r--   0        0        0     2492 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/client.py
+-rw-r--r--   0        0        0      332 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/constants.py
+-rw-r--r--   0        0        0      436 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/errors.py
+-rw-r--r--   0        0        0      291 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/apis.py
+-rw-r--r--   0        0        0     1615 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/base.py
+-rw-r--r--   0        0        0      840 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/http.py
+-rw-r--r--   0        0        0     2897 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/keys.py
+-rw-r--r--   0        0        0        0 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/py.typed
+-rw-r--r--   0        0        0     2230 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/result.py
+-rw-r--r--   0        0        0     2089 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/routes.py
+-rw-r--r--   0        0        0     3581 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/serializer.py
+-rw-r--r--   0        0        0      151 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/__init__.py
+-rw-r--r--   0        0        0     2353 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/apis.py
+-rw-r--r--   0        0        0     1229 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/base.py
+-rw-r--r--   0        0        0     4388 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/http.py
+-rw-r--r--   0        0        0     3970 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/keys.py
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 unkey_py-0.3.0/PKG-INFO
```

### Comparing `unkey_py-0.2.0/LICENSE` & `unkey_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/README.md` & `unkey_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/pyproject.toml` & `unkey_py-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "unkey.py"
-version = "0.2.0"
+version = "0.3.0"
 description = "An asynchronous Python SDK for unkey.dev."
 authors = ["Jonxslays"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/unkey.py"
 repository = "https://github.com/Jonxslays/unkey.py"
 packages = [
     { include = "unkey" },
     { include = "unkey/py.typed" },
 ]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    # "Development Status :: 1 - Planning",
     # "Development Status :: 2 - Pre-Alpha",
     # "Development Status :: 3 - Alpha",
-    # "Development Status :: 4 - Beta",
+    "Development Status :: 4 - Beta",
     # "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -36,29 +36,29 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 aiohttp = ">3.8.1"
 attrs = ">=22"
 
 [tool.poetry.group.dev.dependencies]
-black = "==23.3.0"
+black = "==23.7.0"
 coverage = "==7.2.7"
 flake8 = { version = "==6.0.0", python = ">=3.8.1" }
 griffe = ">=0.28.2"
 isort = "==5.12.0"
 len8 = { version = "==0.7.3.post0", python = "<3.12" }
 mike = "==1.1.2"
 mkdocs-include-markdown-plugin = { version = "==4.0.4", python = "<3.12" }
-mkdocs-material = "==9.1.16"
+mkdocs-material = "==9.1.18"
 mkdocstrings = { version = "==0.22.0", extras = ["python"] }
-mypy = "==1.4.0"
+mypy = "==1.4.1"
 nox = "==2023.4.22"
-pyright = "==1.1.315"
-pytest = "==7.3.2"
-pytest-asyncio = "==0.21.0"
+pyright = "==1.1.317"
+pytest = "==7.4.0"
+pytest-asyncio = "==0.21.1"
 pytest-testdox = "==3.0.1"
 types-toml = "==0.10.8.6"
 toml = "==0.10.2"
 
 [tool.black]
 line-length = 99
 
@@ -76,10 +76,13 @@
 packages = ["unkey"]
 strict = true
 
 [tool.pyright]
 include = ["unkey"]
 typeCheckingMode = "strict"
 
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `unkey_py-0.2.0/unkey/__init__.py` & `unkey_py-0.3.0/unkey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "unkey.py"
-__version__: Final[str] = "0.2.0"
+__version__: Final[str] = "0.3.0"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous Python SDK for unkey.dev."
 __url__: Final[str] = "https://github.com/Jonxslays/unkey.py"
 __docs__: Final[str] = "https://jonxslays.github.io/unkey.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "GPL-3.0"
-__git_sha__: Final[str] = "[420e875]"
+__git_sha__: Final[str] = "[3c333fd]"
 
 from . import client
 from . import constants
 from . import errors
 from . import models
 from . import result
 from . import routes
@@ -47,14 +47,15 @@
     "BaseEnum",
     "BaseError",
     "BaseModel",
     "BaseService",
     "Client",
     "CompiledRoute",
     "Err",
+    "ErrorCode",
     "HttpResponse",
     "HttpService",
     "KeyService",
     "Ok",
     "Ratelimit",
     "RatelimitType",
     "Result",
```

### Comparing `unkey_py-0.2.0/unkey/__main__.py` & `unkey_py-0.3.0/unkey/__main__.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/client.py` & `unkey_py-0.3.0/unkey/client.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/models/apis.py` & `unkey_py-0.3.0/unkey/models/apis.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/models/base.py` & `unkey_py-0.3.0/unkey/models/base.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/models/keys.py` & `unkey_py-0.3.0/unkey/models/keys.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import typing as t
 
 import attrs
 
 from .base import BaseEnum
 from .base import BaseModel
+from .http import ErrorCode
 
 __all__ = ("ApiKey", "ApiKeyMeta", "ApiKeyVerification", "Ratelimit", "RatelimitType")
 
 
 class RatelimitType(BaseEnum):
     Fast = "fast"
     Consistent = "consistent"
@@ -74,14 +75,20 @@
     """The optional ratelimit associated with this key."""
 
     meta: t.Optional[t.Dict[str, t.Any]]
     """The dynamic mapping of data used during key creation, if
     the key was found.
     """
 
+    remaining: t.Optional[int]
+    """The remaining verifications before this key is invalidated.
+    If `None`, this field was not used in the keys creation and can
+    be ignored.
+    """
+
 
 @attrs.define(init=False, weakref_slot=False)
 class ApiKeyVerification(BaseModel):
     """Data about whether this api key is valid."""
 
     valid: bool
     """Whether or not this key is valid and passes ratelimit."""
@@ -90,9 +97,18 @@
     """The id of the owner for this key, if the key was found."""
 
     meta: t.Optional[t.Dict[str, t.Any]]
     """Dynamic mapping of data used during key creation, if the
     key was found.
     """
 
+    remaining: t.Optional[int]
+    """The remaining verifications before this key is invalidated.
+    If `None`, this field was not used in the keys creation and can
+    be ignored.
+    """
+
+    code: t.Optional[ErrorCode]
+    """The optional error code returned by the unkey api."""
+
     error: t.Optional[str]
     """The error message if the key was invalid."""
```

### Comparing `unkey_py-0.2.0/unkey/result.py` & `unkey_py-0.3.0/unkey/result.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/routes.py` & `unkey_py-0.3.0/unkey/routes.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/serializer.py` & `unkey_py-0.3.0/unkey/serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,15 +64,19 @@
     def to_api_key(self, data: DictT) -> models.ApiKey:
         model = models.ApiKey()
         self._set_attrs_cased(model, data, "key", "key_id")
         return model
 
     def to_api_key_verification(self, data: DictT) -> models.ApiKeyVerification:
         model = models.ApiKeyVerification()
-        self._set_attrs_cased(model, data, "valid", "owner_id", "meta", "error", maybe=True)
+        model.code = models.ErrorCode.from_str_maybe(data.get("code", ""))
+        self._set_attrs_cased(
+            model, data, "valid", "owner_id", "meta", "remaining", "error", maybe=True
+        )
+
         return model
 
     def to_api(self, data: DictT) -> models.Api:
         model = models.Api()
         self._set_attrs_cased(model, data, "id", "name", "workspace_id")
         return model
 
@@ -92,14 +96,15 @@
             model,
             data,
             "id",
             "meta",
             "start",
             "api_id",
             "expires",
+            "remaining",
             "owner_id",
             "created_at",
             "workspace_id",
             maybe=True,
         )
 
         return model
```

### Comparing `unkey_py-0.2.0/unkey/services/apis.py` & `unkey_py-0.3.0/unkey/services/apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,23 @@
         """
         route = routes.GET_API.compile(api_id)
         data = await self._http.fetch(route)
 
         if isinstance(data, models.HttpResponse):
             return result.Err(data)
 
+        if "error" in data:
+            return result.Err(
+                models.HttpResponse(
+                    404,
+                    data["error"],
+                    models.ErrorCode.from_str_maybe(data.get("code", "unknown")),
+                )
+            )
+
         return result.Ok(self._serializer.to_api(data))
 
     async def list_keys(
         self, api_id: str, *, owner_id: t.Optional[str] = None, limit: int = 100, offset: int = 0
     ) -> ResultT[models.ApiKeyList]:
         """Gets a paginated list of keys for the given api.
 
@@ -52,15 +61,23 @@
 
             offset: How many keys to offset by, for pagination.
 
         Returns:
             A result containing api key list or an error.
         """
         params = self._generate_map(ownerId=owner_id, limit=limit, offset=offset)
-        print(params)
         route = routes.GET_KEYS.compile(api_id).with_params(params)
         data = await self._http.fetch(route)
 
         if isinstance(data, models.HttpResponse):
             return result.Err(data)
 
+        if "error" in data:
+            return result.Err(
+                models.HttpResponse(
+                    404,
+                    data["error"],
+                    models.ErrorCode.from_str_maybe(data.get("code", "unknown")),
+                )
+            )
+
         return result.Ok(self._serializer.to_api_key_list(data))
```

### Comparing `unkey_py-0.2.0/unkey/services/base.py` & `unkey_py-0.3.0/unkey/services/base.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.2.0/unkey/services/http.py` & `unkey_py-0.3.0/unkey/services/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = ("HttpService",)
 
 T = t.TypeVar("T")
 
 
 class HttpService:
-    """The HTTP service used to make requests to the WOM API.
+    """The HTTP service used to make requests to the unkey API.
 
     Args:
         api_key: The api key to use.
 
         api_version: The optional version of the api to use.
 
         api_base_url: The optional api base url to use.
@@ -69,15 +69,17 @@
         if isinstance(data, models.HttpResponse):
             return data
 
         # Skipping 404's seems hacky but whatever
         if response.status not in (*self._ok_responses, 404):
             return models.HttpResponse(
                 response.status,
-                data.get("message", "An unexpected error occurred while making the request."),
+                data.get("error")
+                or data.get("message")
+                or "An unexpected error occurred while making the request.",
             )
 
         return data
 
     def _get_request_func(self, method: str) -> t.Callable[..., t.Awaitable[t.Any]]:
         if not hasattr(self, "_method_mapping"):
             raise RuntimeError("HttpService.start was never called, aborting...")
```

### Comparing `unkey_py-0.2.0/unkey/services/keys.py` & `unkey_py-0.3.0/unkey/services/keys.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 
     async def create_key(
         self,
         api_id: str,
         owner_id: str,
         prefix: str,
         *,
-        byte_length: int = 16,
-        meta: t.Dict[str, t.Any] = {},
+        byte_length: t.Optional[int] = None,
+        meta: t.Optional[t.Dict[str, t.Any]] = None,
         expires: t.Optional[int] = None,
+        remaining: t.Optional[int] = None,
         ratelimit: t.Optional[models.Ratelimit] = None,
     ) -> ResultT[models.ApiKey]:
         """Creates a new api key.
 
         Args:
             api_id: The id of the api this key is for.
 
@@ -46,25 +47,30 @@
 
             meta: An optional dynamic mapping of information used to
                 provide context around this keys user.
 
             expires: The optional number of milliseconds into the future
                 when this key should expire.
 
+            remaining: The optional max number of times this key can be
+                used. Useful for creating long lived keys but with a
+                limit on total uses.
+
             ratelimit: The optional Ratelimit to set on this key.
 
         Returns:
             A result containing the requested information or an error.
         """
         route = routes.CREATE_KEY.compile()
         payload = self._generate_map(
             meta=meta,
             apiId=api_id,
             prefix=prefix,
             ownerId=owner_id,
+            remaining=remaining,
             byteLength=byte_length,
             expires=self._expires_in(milliseconds=expires or 0),
             ratelimit=None
             if not ratelimit
             else self._generate_map(
                 limit=ratelimit.limit,
                 type=ratelimit.type.value,
@@ -104,13 +110,22 @@
         Args:
             key_id: The id of the key to revoke.
 
         Returns:
             A result containing the http response or an error.
         """
         route = routes.REVOKE_KEY.compile(key_id)
-        data: str | models.HttpResponse = await self._http.fetch(route)  # type: ignore
+        data = await self._http.fetch(route)
 
         if isinstance(data, models.HttpResponse):
             return result.Err(data)
 
-        return result.Ok(models.HttpResponse(202, data))
+        if "error" in data:
+            return result.Err(
+                models.HttpResponse(
+                    404,
+                    data["error"],
+                    models.ErrorCode.from_str_maybe(data.get("code", "unknown")),
+                )
+            )
+
+        return result.Ok(models.HttpResponse(200, "OK"))
```

### Comparing `unkey_py-0.2.0/PKG-INFO` & `unkey_py-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: unkey-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: An asynchronous Python SDK for unkey.dev.
 Home-page: https://github.com/Jonxslays/unkey.py
 License: GPL-3.0-only
 Author: Jonxslays
 Requires-Python: >=3.8
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

