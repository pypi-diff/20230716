# Comparing `tmp/pyathena-3.0.5.tar.gz` & `tmp/pyathena-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.5.tar", max compression
+gzip compressed data, was "pyathena-3.0.6.tar", max compression
```

## Comparing `pyathena-3.0.5.tar` & `pyathena-3.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-07-12 05:00:18.290483 pyathena-3.0.5/LICENSE
--rw-r--r--   0        0        0    71913 2023-07-12 05:00:18.290483 pyathena-3.0.5/README.rst
--rw-r--r--   0        0        0     1959 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2590 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9791 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5409 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21206 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/common.py
--rw-r--r--   0        0        0    10452 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/connection.py
--rw-r--r--   0        0        0     4245 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/converter.py
--rw-r--r--   0        0        0     5835 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20510 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1252 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/formatter.py
--rw-r--r--   0        0        0    17910 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5865 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1866 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13625 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9858 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/py.typed
--rw-r--r--   0        0        0    25140 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    39146 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1246 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1984 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyproject.toml
--rw-r--r--   0        0        0    73152 1970-01-01 00:00:00.000000 pyathena-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-16 15:46:36.882544 pyathena-3.0.6/LICENSE
+-rw-r--r--   0        0        0    71913 2023-07-16 15:46:36.882544 pyathena-3.0.6/README.rst
+-rw-r--r--   0        0        0     1959 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2590 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9791 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5409 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21206 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/common.py
+-rw-r--r--   0        0        0    10452 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/connection.py
+-rw-r--r--   0        0        0     4245 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/converter.py
+-rw-r--r--   0        0        0     5835 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20510 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1252 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/formatter.py
+-rw-r--r--   0        0        0    17910 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5865 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1866 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13625 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9858 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/py.typed
+-rw-r--r--   0        0        0    25140 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      659 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    39145 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      882 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1246 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     2465 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-07-16 15:46:36.886544 pyathena-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0    73152 1970-01-01 00:00:00.000000 pyathena-3.0.6/PKG-INFO
```

### Comparing `pyathena-3.0.5/LICENSE` & `pyathena-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/README.rst` & `pyathena-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/__init__.py` & `pyathena-3.0.6/pyathena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.5"
+__version__: str = "3.0.6"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.5/pyathena/arrow/async_cursor.py` & `pyathena-3.0.6/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/arrow/converter.py` & `pyathena-3.0.6/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/arrow/cursor.py` & `pyathena-3.0.6/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/arrow/result_set.py` & `pyathena-3.0.6/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/arrow/util.py` & `pyathena-3.0.6/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/async_cursor.py` & `pyathena-3.0.6/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/common.py` & `pyathena-3.0.6/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/connection.py` & `pyathena-3.0.6/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/converter.py` & `pyathena-3.0.6/pyathena/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import binascii
 import json
 import logging
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from datetime import date, datetime, time
 from decimal import Decimal
-from distutils.util import strtobool
 from typing import Any, Callable, Dict, Optional, Type
 
+from pyathena.util import strtobool
+
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 def _to_date(varchar_value: Optional[str]) -> Optional[date]:
     if varchar_value is None:
         return None
     return datetime.strptime(varchar_value, "%Y-%m-%d").date()
```

### Comparing `pyathena-3.0.5/pyathena/cursor.py` & `pyathena-3.0.6/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/error.py` & `pyathena-3.0.6/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/fastparquet/util.py` & `pyathena-3.0.6/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/filesystem/s3.py` & `pyathena-3.0.6/pyathena/filesystem/s3.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/filesystem/s3_object.py` & `pyathena-3.0.6/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/formatter.py` & `pyathena-3.0.6/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/model.py` & `pyathena-3.0.6/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/pandas/async_cursor.py` & `pyathena-3.0.6/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/pandas/converter.py` & `pyathena-3.0.6/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/pandas/cursor.py` & `pyathena-3.0.6/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/pandas/result_set.py` & `pyathena-3.0.6/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/pandas/util.py` & `pyathena-3.0.6/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/result_set.py` & `pyathena-3.0.6/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.6/pyathena/sqlalchemy/arrow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
-from distutils.util import strtobool
-
 from pyathena.sqlalchemy.base import AthenaDialect
+from pyathena.util import strtobool
 
 
 class AthenaArrowDialect(AthenaDialect):
     driver = "arrow"
     supports_statement_cache = True
 
     def create_connect_args(self, url):
```

### Comparing `pyathena-3.0.5/pyathena/sqlalchemy/base.py` & `pyathena-3.0.6/pyathena/sqlalchemy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import re
-from distutils.util import strtobool
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Mapping,
     MutableMapping,
@@ -36,14 +35,15 @@
 from pyathena.model import (
     AthenaFileFormat,
     AthenaPartitionTransform,
     AthenaRowFormatSerde,
 )
 from pyathena.sqlalchemy.types import AthenaDate, AthenaTimestamp
 from pyathena.sqlalchemy.util import _HashableDict
+from pyathena.util import strtobool
 
 if TYPE_CHECKING:
     from types import ModuleType
 
     from sqlalchemy import (
         URL,
         Cast,
```

### Comparing `pyathena-3.0.5/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.6/pyathena/sqlalchemy/pandas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
-from distutils.util import strtobool
-
 from pyathena.sqlalchemy.base import AthenaDialect
+from pyathena.util import strtobool
 
 
 class AthenaPandasDialect(AthenaDialect):
     driver = "pandas"
     supports_statement_cache = True
 
     def create_connect_args(self, url):
```

### Comparing `pyathena-3.0.5/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.6/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/sqlalchemy/types.py` & `pyathena-3.0.6/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.5/pyathena/util.py` & `pyathena-3.0.6/pyathena/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,29 @@
     match = PATTERN_OUTPUT_LOCATION.search(output_location)
     if match:
         return match.group("bucket"), match.group("key")
     else:
         raise DataError("Unknown `output_location` format.")
 
 
+def strtobool(val):
+    """
+    Since the distutils module has been deprecated, the distutils.util.strtobool method is ported.
+    https://peps.python.org/pep-0632/
+    https://github.com/pypa/distutils/blob/main/distutils/util.py#L340-L353
+    """
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError(f"invalid truth value {val!r}")
+
+
 class RetryConfig:
     def __init__(
         self,
         exceptions: Iterable[str] = (
             "ThrottlingException",
             "TooManyRequestsException",
         ),
```

### Comparing `pyathena-3.0.5/pyproject.toml` & `pyathena-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.5"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.6"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.5/PKG-INFO` & `pyathena-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

