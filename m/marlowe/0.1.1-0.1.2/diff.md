# Comparing `tmp/marlowe-0.1.1-cp311-none-win_amd64.whl.zip` & `tmp/marlowe-0.1.2-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 816455 bytes, number of entries: 5
--rw-r--r--  4.6 unx     1400 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx      111 b- defN 23-Jul-14 21:35 marlowe/__init__.py
--rwxr-xr-x  4.6 unx  2411520 b- defN 23-Jul-14 21:35 marlowe/marlowe.cp311-win_amd64.pyd
--rw-r--r--  4.6 unx      376 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/RECORD
-5 files, 2413502 bytes uncompressed, 815763 bytes compressed:  66.2%
+Zip file size: 872477 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     1494 b- defN 23-Jul-16 13:17 marlowe-0.1.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jul-16 13:17 marlowe-0.1.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx      111 b- defN 23-Jul-16 13:17 marlowe/__init__.py
+-rwxr-xr-x  4.6 unx  2591744 b- defN 23-Jul-16 13:17 marlowe/marlowe.cp311-win_amd64.pyd
+-rw-r--r--  4.6 unx      376 b- defN 23-Jul-16 13:17 marlowe-0.1.2.dist-info/RECORD
+5 files, 2593820 bytes uncompressed, 871785 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: marlowe-0.1.1.dist-info/METADATA
+Filename: marlowe-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: marlowe-0.1.1.dist-info/WHEEL
+Filename: marlowe-0.1.2.dist-info/WHEEL
 Comment: 
 
 Filename: marlowe/__init__.py
 Comment: 
 
 Filename: marlowe/marlowe.cp311-win_amd64.pyd
 Comment: 
 
-Filename: marlowe-0.1.1.dist-info/RECORD
+Filename: marlowe-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `marlowe-0.1.1.dist-info/METADATA` & `marlowe-0.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: marlowe
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: marlowe-rs bindings for using cardano marlowe in python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
+[![PyPI version](https://badge.fury.io/py/marlowe.svg)](https://pypi.org/project/marlowe/)
+
 ## MARLOWE-PY
 
 **Python bindings for Marlowe_Lang [marlowe-rs](https://github.com/OlofBlomqvist/marlowe-rs).**
 
 ### Features
 
 - Deserialize contracts from: cbor-hex, dsl, json.
```

