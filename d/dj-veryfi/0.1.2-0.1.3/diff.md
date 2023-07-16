# Comparing `tmp/dj-veryfi-0.1.2.tar.gz` & `tmp/dj-veryfi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-veryfi-0.1.2.tar", last modified: Sun Jul 16 00:06:45 2023, max compression
+gzip compressed data, was "dist/dj-veryfi-0.1.3.tar", last modified: Sun Jul 16 00:10:14 2023, max compression
```

## Comparing `dj-veryfi-0.1.2.tar` & `dj-veryfi-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/
--rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.2/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)       35 2023-07-16 00:00:43.000000 dj-veryfi-0.1.2/MANIFEST.in
--rw-r--r--   0 tony      (1000) tony      (1000)      577 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     2915 2023-07-16 00:05:32.000000 dj-veryfi-0.1.2/README.rst
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)      577 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      278 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/dj_veryfi.egg-info/top_level.txt
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/migrations/
--rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.2/migrations/0001_initial.py
--rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.2/migrations/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.2/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:06:45.000000 dj-veryfi-0.1.2/setup.cfg
--rw-r--r--   0 tony      (1000) tony      (1000)       38 2023-07-16 00:06:04.000000 dj-veryfi-0.1.2/setup.py
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/
+-rw-r--r--   0 tony      (1000) tony      (1000)     1139 2023-07-15 23:02:53.000000 dj-veryfi-0.1.3/LICENSE
+-rw-r--r--   0 tony      (1000) tony      (1000)       31 2023-07-16 00:09:24.000000 dj-veryfi-0.1.3/MANIFEST.in
+-rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     2884 2023-07-16 00:08:30.000000 dj-veryfi-0.1.3/README
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     3502 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      274 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       50 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/requires.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)       11 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/dj_veryfi.egg-info/top_level.txt
+drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/migrations/
+-rw-r--r--   0 tony      (1000) tony      (1000)      615 2023-07-15 22:04:41.000000 dj-veryfi-0.1.3/migrations/0001_initial.py
+-rw-r--r--   0 tony      (1000) tony      (1000)        0 2023-07-15 18:29:43.000000 dj-veryfi-0.1.3/migrations/__init__.py
+-rw-r--r--   0 tony      (1000) tony      (1000)       88 2023-07-15 23:03:01.000000 dj-veryfi-0.1.3/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      694 2023-07-16 00:10:14.000000 dj-veryfi-0.1.3/setup.cfg
+-rw-r--r--   0 tony      (1000) tony      (1000)       83 2023-07-16 00:10:10.000000 dj-veryfi-0.1.3/setup.py
```

### Comparing `dj-veryfi-0.1.2/LICENSE` & `dj-veryfi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.2/README.rst` & `dj-veryfi-0.1.3/README`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,61 @@
-Django Veryfi OCR API Integration
-=================================
 
-As the title says, its a *Django* integration for *Veryfi OCR API*. For
-now, it can auto OCR receipts or invoices documents by using
-**dj_veryfi.fields.OCRInvoiceOrReceiptField** model field. It derives
-from **django.db.models.JSONField** model field and, takes a additional
-parameter **upload_to** which specifies the path where the file should
-be saved according to current defined Django STORAGE.
-
-Requirements
-------------
-
-   Python 3 Django >= 3.2.20 Veryfi 3.3.0
-
-How it works
-------------
-
-Once you have defined a model field as
-**dj_veryfi.fields.OCRInvoiceOrReceiptField**, you can assign a
-file-like instance to an instance model field of
-**dj_veryfi.fields.OCRInvoiceOrReceiptField**, then, before saving the
-model, it gonna hit the Veryfi OCR API to extract information and
-persists it as JSON into datababse. When the field instance is acceesed
-after extraction it returns a **OCRData** instance which has the file descriptor and the JSON data.
-
-How to install
---------------
-
-::
-
-   pip install dj-veryfi
-
-Setup
------
-
-Add **dj_veryfi** into *INSTALLED_APPS* and set the *Veryfi API*
-authentication information into *settings.py* as described bellow:
-
-::
-
-   ...
-   INSTALLED_APS = [
-   ...
-   "dj_veryfi"
-   ]
-   ...
-   # Veryfi access settings
-   VERYFI_CLIENT_ID = "Your client ID"
-   VERYFI_CLIENT_SECRET = "Your client secret"
-   VERYFI_USERNAME = "Your username"
-   VERYFI_API_KEY = "Your api key"
-
-Usage
------
-
-Once you have a django project, dj-veryfi installed and setedup, just
-declare your model field as
-**dj_veryfi.fields.OCRInvoiceOrReceiptField**, as bellow.
-
-::
-
-   from django.db import models
-   from dj_veryfi.fields import OCRInvoiceOrReceiptField
-
-   class Document(models.Model):
-       created_at = models.Datetime.FIeld(auto_now_add=True)
-       name = models.CharFied(max_length=100)
-       ocr_data = OCRInvoiceOrReceiptField(upload_to="receipts/")
-
-Note, the **upload_to** attribute is a relative path which will append
-to MEDIA_ROOT settings variable.
-
-Now, you can just assign a file-like object to **Document.ocr_data**
-save the model and, the information from receipt or invoice file will be
-extracted and saved as json into database.
-
-Trade-Offs
-----------
-
-I have chosen to extend the field from **django.db.models.JSONField**
-because the extracted data comes as JSON and I had to do nothing related
-to querying.
-
-If I had chosen another model field type like **FileField** to get a
-shortcut to manage files and save them as JSON, I would have had trouble
-with how to query it into the database, due to JSON querying definition
-is not that simple.
-
-So, it seems easier to me to avoid dealing with querying definitions
-when it comes to JSON querying, due to **JSONField** comes with “query
-thing” already done and deal with managing the files from where the
-information was extracted is easier.
+# Django Veryfi OCR API Integration
+
+As the title says, its a *Django* integration for *Veryfi OCR API*.
+For now, it can auto OCR receipts or invoices documents by using ***dj_veryfi.fields.OCRInvoiceOrReceiptField*** model field. It derives from ***django.db.models.JSONField*** model field and, takes a additional parameter ***upload_to*** which specifies the path where the file should be saved according to current defined Django STORAGE.
+
+## Requirements
+
+> Python 3
+> Django >= 3.2.20 
+> Veryfi 3.3.0
+
+## How it works
+Once you have defined a model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, you can assign a file-like instance to an instance model field of ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, then, before saving the model, it gonna hit the Veryfi OCR API to extract information and persists it as JSON into datababse.
+When the field instance is acceesed after extraction it returns a ***OCRData*** instance which has the file descriptor and the JSON data.
+
+## How to install
+
+    pip install dj-veryfi
+
+## Setup
+Add ***dj_veryfi*** into *INSTALLED_APPS* and set the *Veryfi API* authentication information into *settings.py* as described bellow:
+		
+    ...
+    INSTALLED_APS = [
+    ...
+    "dj_veryfi"
+    ]
+    ...
+    # Veryfi access settings
+    VERYFI_CLIENT_ID = "Your client ID"
+    VERYFI_CLIENT_SECRET = "Your client secret"
+    VERYFI_USERNAME = "Your username"
+    VERYFI_API_KEY = "Your api key"
+
+
+## Usage
+Once you have a django project, dj-veryfi installed and setedup, just declare your model field as ***dj_veryfi.fields.OCRInvoiceOrReceiptField***, as bellow.
+   
+    from django.db import models
+    from dj_veryfi.fields import OCRInvoiceOrReceiptField
+    
+    class Document(models.Model):
+        created_at = models.Datetime.FIeld(auto_now_add=True)
+        name = models.CharFied(max_length=100)
+        ocr_data = OCRInvoiceOrReceiptField(upload_to="receipts/") 
+
+Note, the ***upload_to*** attribute is a relative path which will append to MEDIA_ROOT settings variable.
+
+Now, you can just assign a file-like object to ***Document.ocr_data*** save the model and, the information from receipt or invoice file will be extracted and saved as json into database.
+
+## Trade-Offs
+I have chosen to extend the field from ***django.db.models.JSONField*** because the extracted data comes as JSON and I had to do nothing related to querying. 
+
+If I had chosen another model field type like ***FileField*** to get a shortcut to manage files and save them as JSON, I would have had trouble with how to query it into the database, due to JSON querying definition is not that simple.
+
+So, it seems easier to me to avoid dealing with querying definitions when it comes to JSON querying, due to ***JSONField*** comes with "query thing" already done and deal with managing the files from where the information was extracted is easier. 
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dj-veryfi-0.1.2/migrations/0001_initial.py` & `dj-veryfi-0.1.3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-veryfi-0.1.2/setup.cfg` & `dj-veryfi-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-veryfi
-version = 0.1.2
+version = 0.1.3
 description = Django integration for Veryfi OCR API.
 long_description = file: README
 url = https://github.com/tonykamillo/dj-veryfi
 author = Tony Kamillo
 author_email = tonykamillo@gmail.com
 license = DBAD
 classifiers =
```

