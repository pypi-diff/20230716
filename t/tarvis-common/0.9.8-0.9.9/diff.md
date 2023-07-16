# Comparing `tmp/tarvis-common-0.9.8.tar.gz` & `tmp/tarvis-common-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.8.tar", last modified: Wed Jun 28 14:50:34 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.9.tar", last modified: Thu Jul  6 22:23:57 2023, max compression
```

## Comparing `tarvis-common-0.9.8.tar` & `tarvis-common-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.184755 tarvis-common-0.9.8/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.184755 tarvis-common-0.9.8/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.184755 tarvis-common-0.9.8/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.184755 tarvis-common-0.9.8/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3982 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     6252 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     4398 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6436 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)    11112 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-28 14:50:34.000000 tarvis-common-0.9.8/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2023-06-28 14:50:34.000000 tarvis-common-0.9.8/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 14:50:34.000000 tarvis-common-0.9.8/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-28 14:50:34.000000 tarvis-common-0.9.8/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-28 14:50:34.000000 tarvis-common-0.9.8/tarvis_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 14:50:34.188756 tarvis-common-0.9.8/test/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/test/test_cache_local.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-06-28 14:50:23.000000 tarvis-common-0.9.8/test/test_secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.377208 tarvis-common-0.9.9/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.377208 tarvis-common-0.9.9/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.377208 tarvis-common-0.9.9/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.377208 tarvis-common-0.9.9/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.377208 tarvis-common-0.9.9/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     6252 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)    11855 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-06 22:23:57.000000 tarvis-common-0.9.9/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-06 22:23:57.000000 tarvis-common-0.9.9/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:23:57.000000 tarvis-common-0.9.9/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-06 22:23:57.000000 tarvis-common-0.9.9/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 22:23:57.000000 tarvis-common-0.9.9/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:23:57.381209 tarvis-common-0.9.9/test/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/test/test_cache_local.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-06 22:23:47.000000 tarvis-common-0.9.9/test/test_secrets.py
```

### Comparing `tarvis-common-0.9.8/LICENSE.txt` & `tarvis-common-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/setup.py` & `tarvis-common-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.8",
+    version="0.9.9",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.8/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.9/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.9/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/config/__init__.py` & `tarvis-common-0.9.9/tarvis/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.9/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.9/tarvis/common/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.9/tarvis/common/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.9/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/time/__init__.py` & `tarvis-common-0.9.9/tarvis/common/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.9/tarvis/common/trading/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -127,39 +127,51 @@
         minimum_order_value: Decimal | float = None,
         maximum_order_value: Decimal | float = None,
         quantity_decimals: int = None,
         quantity_precision: Decimal = None,
         price_decimals: int = None,
         price_precision: Decimal = None,
     ):
+        if quantity_precision is not None:
+            quantity_precision = Decimal(quantity_precision)
+
+        if price_precision is not None:
+            price_precision = Decimal(price_precision)
+
         if (quantity_decimals is None) and quantity_precision:
             quantity_decimals = int(-math.log10(quantity_precision))
         self._quantity_decimals = quantity_decimals
 
         if (price_decimals is None) and price_precision:
             price_decimals = int(-math.log10(price_precision))
         self._price_decimals = price_decimals
 
-        # Ensure the minimum is aligned
-        self._minimum_order_quantity = self.align_quantity(minimum_order_quantity)
-
-        if maximum_order_quantity is None:
-            self._maximum_order_quantity = None
-        else:
-            self._maximum_order_quantity = Decimal(maximum_order_quantity)
+        self._minimum_order_quantity = self.align_quantity(
+            minimum_order_quantity, decimal.ROUND_UP
+        )
+
+        if maximum_order_quantity is not None:
+            maximum_order_quantity = self.align_quantity(
+                maximum_order_quantity, decimal.ROUND_DOWN
+            )
+        self._maximum_order_quantity = maximum_order_quantity
 
         if minimum_order_value is None:
-            self._minimum_order_value = 0
+            minimum_order_value = Decimal(0)
         else:
-            self._minimum_order_value = Decimal(minimum_order_value)
-
-        if maximum_order_value is None:
-            self._maximum_order_value = None
-        else:
-            self._maximum_order_value = Decimal(maximum_order_value)
+            minimum_order_value = self.align_price(
+                minimum_order_value, decimal.ROUND_UP
+            )
+        self._minimum_order_value = minimum_order_value
+
+        if maximum_order_value is not None:
+            maximum_order_value = self.align_price(
+                maximum_order_value, decimal.ROUND_DOWN
+            )
+        self._maximum_order_value = maximum_order_value
 
     @staticmethod
     def _align(value: Decimal | float | int, decimals: int | None, rounding) -> Decimal:
         value = Decimal(value)
         if decimals is not None:
             with decimal.localcontext() as ctx:
                 ctx.rounding = rounding
@@ -197,14 +209,22 @@
         return self.align_quantity(quantity)
 
     def align_price(
         self, price: Decimal | float | int, rounding=decimal.ROUND_HALF_EVEN
     ) -> Decimal:
         return self._align(price, self._price_decimals, rounding)
 
+    def limit_value(self, value: Decimal) -> Decimal:
+        if value < self._minimum_order_value:
+            value = self._minimum_order_value
+        if self._maximum_order_value is not None:
+            if value > self._maximum_order_value:
+                value = self._maximum_order_value
+        return value
+
 
 class Order:
     def __init__(
         self,
         base_asset: str,
         quote_asset: str,
         side: OrderSide,
```

### Comparing `tarvis-common-0.9.8/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.9/tarvis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.8/test/test_cache_local.py` & `tarvis-common-0.9.9/test/test_cache_local.py`

 * *Files identical despite different names*

