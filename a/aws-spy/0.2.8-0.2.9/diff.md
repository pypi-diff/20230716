# Comparing `tmp/aws_spy-0.2.8.tar.gz` & `tmp/aws_spy-0.2.9.tar.gz`

## Comparing `aws_spy-0.2.8.tar` & `aws_spy-0.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 aws_spy-0.2.8/Makefile
--rw-r--r--   0        0        0    81872 2020-02-02 00:00:00.000000 aws_spy-0.2.8/pdm.lock
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.8/.vscode/settings.json
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/dependencies.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/main.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/responses.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/encoders.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/event_utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/exceptions.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/logging.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/params.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/params_alias.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/responses.py
--rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/schemas.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/schemas_utils.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/core/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/helpers/__init__.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/helpers/cli.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/helpers/documentation.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/helpers/exceptions.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/helpers/utils.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy-layer.yml
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/annotated_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/annotated_types/py.typed
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/__init__.py
--rwxr-xr-x   0        0        0  4145120 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.cpython-310-aarch64-linux-gnu.so
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0        0        0   129458 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/core_schema.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/integration/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/integration/test_params.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/integration/test_request_body.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/integration/test_response_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/integration/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/test_encoders.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/test_event_utils.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/test_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/test_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.8/tests/unit/test_utils.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 aws_spy-0.2.8/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.8/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.8/README.md
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aws_spy-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 aws_spy-0.2.9/Makefile
+-rw-r--r--   0        0        0    81872 2020-02-02 00:00:00.000000 aws_spy-0.2.9/pdm.lock
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aws_spy-0.2.9/.vscode/settings.json
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/dependencies.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/main.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/responses.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/encoders.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/event_utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/exceptions.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/logging.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/params.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/params_alias.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/responses.py
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/schemas.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/schemas_utils.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/core/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/helpers/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/helpers/cli.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/helpers/documentation.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/helpers/exceptions.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/helpers/utils.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy-layer.yml
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/annotated_types/py.typed
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/__init__.py
+-rwxr-xr-x   0        0        0  4145120 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.cpython-310-aarch64-linux-gnu.so
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0        0        0   129551 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/core_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/integration/test_params.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/integration/test_request_body.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/integration/test_response_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/integration/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/test_encoders.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/test_event_utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/test_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/test_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_spy-0.2.9/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 aws_spy-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aws_spy-0.2.9/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aws_spy-0.2.9/README.md
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aws_spy-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aws_spy-0.2.9/PKG-INFO
```

### Comparing `aws_spy-0.2.8/.pre-commit-config.yaml` & `aws_spy-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/Makefile` & `aws_spy-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/pdm.lock` & `aws_spy-0.2.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/__init__.py` & `aws_spy-0.2.9/aws_spy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ServerlessPy package ;D"""
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 from aws_spy import responses
 from aws_spy.core.logging import logger
 from aws_spy.core.params_alias import Header, Path, Query
 from aws_spy.core.schemas import (
     CORS,
     VPC,
```

### Comparing `aws_spy-0.2.8/aws_spy/dependencies.py` & `aws_spy-0.2.9/aws_spy/dependencies.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/main.py` & `aws_spy-0.2.9/aws_spy/main.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/responses.py` & `aws_spy-0.2.9/aws_spy/responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/test.py` & `aws_spy-0.2.9/aws_spy/test.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/core/event_utils.py` & `aws_spy-0.2.9/aws_spy/core/event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/core/schemas.py` & `aws_spy-0.2.9/aws_spy/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/core/schemas_utils.py` & `aws_spy-0.2.9/aws_spy/core/schemas_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,39 +51,42 @@
         ParamType.HEADER: {},
         ParamType.PATH: {},
         ParamType.QUERY: {},
     }
     request_body = None
     request_body_arg_name = None
     for arg_name, arg_value in inspect.signature(handler).parameters.items():
-        if _is_request_body(arg_value) and request_body is None:
-            request_body = arg_value.annotation
-            request_body_arg_name = arg_name
-            continue
-        if _is_param(arg_value):
-            param: Param = arg_value.default
-            param_name = param.name if param.name is not None else arg_name
-            if param_name in params[param.in_].keys():
-                msg = f'{handler.__name__} expects two same {param.in_} params: "{param_name}"!'
-                raise RouteDefinitionError(msg)
+        try:
+            if _is_request_body(arg_value) and request_body is None:
+                request_body = arg_value.annotation
+                request_body_arg_name = arg_name
+                continue
+            if _is_param(arg_value):
+                param: Param = arg_value.default
+                param_name = param.name if param.name is not None else arg_name
+                if param_name in params[param.in_].keys():
+                    msg = f'{handler.__name__} expects two same {param.in_} params: "{param_name}"!'
+                    raise RouteDefinitionError(msg)
 
-            enum = None
-            is_required = types.is_type_required(arg_value.annotation)
-            annotation = arg_value.annotation if is_required else types.get_type_from_optional(arg_value.annotation)
-            if issubclass(annotation, Enum):
-                enum = [e.value for e in annotation]
+                enum = None
+                is_required = types.is_type_required(arg_value.annotation)
+                annotation = arg_value.annotation if is_required else types.get_type_from_optional(arg_value.annotation)
+                if issubclass(annotation, Enum):
+                    enum = [e.value for e in annotation]
 
-            params[param.in_][param_name] = ParamSchema(
-                name=param_name,
-                in_=arg_value.default,
-                arg_name=arg_name,
-                annotation=annotation,
-                enum=enum,
-                is_required=is_required,
-            )
+                params[param.in_][param_name] = ParamSchema(
+                    name=param_name,
+                    in_=arg_value.default,
+                    arg_name=arg_name,
+                    annotation=annotation,
+                    enum=enum,
+                    is_required=is_required,
+                )
+        except TypeError:
+            continue
 
     return HandlerArgs(
         query=params[ParamType.QUERY],
         path=params[ParamType.PATH],
         header=params[ParamType.HEADER],
         request_body=request_body,
         request_body_arg_name=request_body_arg_name,
```

### Comparing `aws_spy-0.2.8/aws_spy/core/types.py` & `aws_spy-0.2.9/aws_spy/core/types.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/helpers/cli.py` & `aws_spy-0.2.9/aws_spy/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/helpers/documentation.py` & `aws_spy-0.2.9/aws_spy/helpers/documentation.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/helpers/utils.py` & `aws_spy-0.2.9/aws_spy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/layer/spy/python/annotated_types/__init__.py` & `aws_spy-0.2.9/aws_spy/layer/spy/python/annotated_types/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/__init__.py` & `aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     to_jsonable_python,
 )
 from .core_schema import CoreConfig, CoreSchema, CoreSchemaType, ErrorType
 
 if _sys.version_info < (3, 11):
     from typing_extensions import NotRequired as _NotRequired
 else:
-    from typing import NotRequired as _NotRequired
+    from typing import NotRequired as _NotRequired  # type: ignore
 
 if _sys.version_info < (3, 9):
     from typing_extensions import TypedDict as _TypedDict
 else:
     from typing import TypedDict as _TypedDict
 
 __all__ = [
```

### Comparing `aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.cpython-310-aarch64-linux-gnu.so` & `aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.cpython-310-aarch64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi` & `aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/_pydantic_core.pyi`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/aws_spy/layer/spy/python/pydantic_core/core_schema.py` & `aws_spy-0.2.9/aws_spy/layer/spy/python/pydantic_core/core_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 """
 
 from __future__ import annotations as _annotations
 
 import sys
 from collections.abc import Mapping
 from datetime import date, datetime, time, timedelta
-from typing import TYPE_CHECKING, Any, Callable, Dict, Hashable, List, Optional, Set, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Hashable,
+    List,
+    Optional,
+    Set,
+    Type,
+    Union,
+)
 
 if sys.version_info < (3, 11):
     from typing_extensions import Protocol, Required, TypeAlias
 else:
     from typing import Protocol, Required, TypeAlias
 
 if sys.version_info < (3, 9):
@@ -909,20 +920,20 @@
 class DatetimeSchema(TypedDict, total=False):
     type: Required[Literal['datetime']]
     strict: bool
     le: datetime
     ge: datetime
     lt: datetime
     gt: datetime
-    now_op: Literal['past', 'future']
-    tz_constraint: Union[Literal['aware', 'naive'], int]
+    now_op: Literal['past', 'future']  # type: ignore
+    tz_constraint: Union[Literal['aware', 'naive'], int]  # type: ignore
     # defaults to current local utc offset from `time.localtime().tm_gmtoff`
     # value is restricted to -86_400 < offset < 86_400 by bounds in generate_self_schema.py
     now_utc_offset: int
-    microseconds_precision: Literal['truncate', 'error'] = ('truncate',)
+    microseconds_precision: Literal['truncate', 'error'] = ('truncate',)  # type: ignore
     ref: str
     metadata: Any
     serialization: SerSchema
 
 
 def datetime_schema(
     *,
```

### Comparing `aws_spy-0.2.8/tests/conftest.py` & `aws_spy-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/test_app.py` & `aws_spy-0.2.9/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from aws_spy import ServerlessConfig, SpyAPI, SpyRouter, __version__
 from aws_spy.core.schemas import Methods
 
 
 def test_app() -> None:
-    assert __version__ == "0.2.8"
+    assert __version__ == "0.2.9"
 
 
 def test_app_conf(app: SpyAPI, config: ServerlessConfig) -> None:
     assert app.config == config
 
 
 @pytest.mark.parametrize("prefix", ["api", "/api", "/somet_other_prefix"])
```

### Comparing `aws_spy-0.2.8/tests/integration/test_params.py` & `aws_spy-0.2.9/tests/integration/test_params.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/integration/test_request_body.py` & `aws_spy-0.2.9/tests/integration/test_request_body.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/integration/test_response_class.py` & `aws_spy-0.2.9/tests/integration/test_response_class.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/unit/test_encoders.py` & `aws_spy-0.2.9/tests/unit/test_encoders.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/unit/test_event_utils.py` & `aws_spy-0.2.9/tests/unit/test_event_utils.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/tests/unit/test_responses.py` & `aws_spy-0.2.9/tests/unit/test_responses.py`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/.gitignore` & `aws_spy-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/LICENSE` & `aws_spy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/pyproject.toml` & `aws_spy-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_spy-0.2.8/PKG-INFO` & `aws_spy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-spy
-Version: 0.2.8
+Version: 0.2.9
 Project-URL: Homepage, https://github.com/PiochU19/aws-spy
 Project-URL: Documentation, https://github.com/PiochU19/aws-spy#readme
 Project-URL: Issues, https://github.com/PiochU19/aws-spy/issues
 Project-URL: Source, https://github.com/PiochU19/aws-spy
 Author-email: Dominik Pioś <792954018@wp.pl>
 License: The MIT License (MIT)
```

