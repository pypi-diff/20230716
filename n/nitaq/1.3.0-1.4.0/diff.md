# Comparing `tmp/nitaq-1.3.0.tar.gz` & `tmp/nitaq-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitaq-1.3.0.tar", last modified: Sun Jul 16 10:37:49 2023, max compression
+gzip compressed data, was "nitaq-1.4.0.tar", last modified: Sun Jul 16 11:00:21 2023, max compression
```

## Comparing `nitaq-1.3.0.tar` & `nitaq-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:37:49.822606 nitaq-1.3.0/
--rw-rw-rw-   0        0        0      199 2023-07-16 10:37:49.822606 nitaq-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:37:49.807607 nitaq-1.3.0/nitaq/
--rw-rw-rw-   0        0        0       25 2023-07-16 10:37:29.000000 nitaq-1.3.0/nitaq/__init__.py
--rw-rw-rw-   0        0        0     3066 2023-07-16 10:17:21.000000 nitaq-1.3.0/nitaq/nitaq.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:37:49.820605 nitaq-1.3.0/nitaq.egg-info/
--rw-rw-rw-   0        0        0      199 2023-07-16 10:37:49.000000 nitaq-1.3.0/nitaq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-16 10:37:49.000000 nitaq-1.3.0/nitaq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:37:49.000000 nitaq-1.3.0/nitaq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 10:37:49.000000 nitaq-1.3.0/nitaq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 10:37:49.000000 nitaq-1.3.0/nitaq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:37:49.823607 nitaq-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      251 2023-07-16 10:37:44.000000 nitaq-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.416874 nitaq-1.4.0/
+-rw-rw-rw-   0        0        0      199 2023-07-16 11:00:21.415874 nitaq-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.388873 nitaq-1.4.0/nitaq/
+-rw-rw-rw-   0        0        0       25 2023-07-16 10:37:29.000000 nitaq-1.4.0/nitaq/__init__.py
+-rw-rw-rw-   0        0        0     3130 2023-07-16 11:00:06.000000 nitaq-1.4.0/nitaq/nitaq.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.413874 nitaq-1.4.0/nitaq.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 11:00:21.416874 nitaq-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      251 2023-07-16 11:00:16.000000 nitaq-1.4.0/setup.py
```

### Comparing `nitaq-1.3.0/nitaq/nitaq.py` & `nitaq-1.4.0/nitaq/nitaq.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,18 @@
     return df_modified
 
 def ener_engi(df, column_name):
     df_filtered = df[df[column_name].str.lower().str.contains('engineering|energy', case=False)]
     return df_filtered
 
 def yearly_basis(file_name):
-    df = pd.read_excel(file_name)
+    try:
+        df = pd.read_excel(file_name)
+    except:
+        df = pd.read_csv(file_name)
     # get lob
     lob = get_lob(df)
     # get quarter names
     columns = quarters(df)
     # energy and engineering only
     removed_rows = ener_engi(df,lob)
     # yearly basis
```

