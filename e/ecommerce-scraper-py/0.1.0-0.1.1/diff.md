# Comparing `tmp/ecommerce-scraper-py-0.1.0.tar.gz` & `tmp/ecommerce-scraper-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecommerce-scraper-py-0.1.0.tar", last modified: Sat Jul 15 18:54:43 2023, max compression
+gzip compressed data, was "ecommerce-scraper-py-0.1.1.tar", last modified: Sun Jul 16 03:54:47 2023, max compression
```

## Comparing `ecommerce-scraper-py-0.1.0.tar` & `ecommerce-scraper-py-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.484152 ecommerce-scraper-py-0.1.0/
--rw-rw-rw-   0        0        0     1095 2023-05-05 00:40:16.000000 ecommerce-scraper-py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2082 2023-07-15 18:54:43.483156 ecommerce-scraper-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.398118 ecommerce-scraper-py-0.1.0/amazon/
--rw-rw-rw-   0        0        0       61 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/amazon/__init__.py
--rw-rw-rw-   0        0        0    24225 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/amazon/amazon.py
--rw-rw-rw-   0        0        0     3296 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/amazon/currencies.py
--rw-rw-rw-   0        0        0      435 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/amazon/languages.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.409116 ecommerce-scraper-py-0.1.0/ebay/
--rw-rw-rw-   0        0        0       53 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/ebay/__init__.py
--rw-rw-rw-   0        0        0      909 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/ebay/domains.py
--rw-rw-rw-   0        0        0    12229 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/ebay/ebay.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.439118 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/
--rw-rw-rw-   0        0        0     2082 2023-07-15 18:54:43.000000 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2023-07-15 18:54:43.000000 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 18:54:43.000000 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-07-15 18:54:43.000000 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2023-07-15 18:54:43.000000 ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.464118 ecommerce-scraper-py-0.1.0/google_shopping/
--rw-rw-rw-   0        0        0       96 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/google_shopping/__init__.py
--rw-rw-rw-   0        0        0    13956 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/google_shopping/countries.py
--rw-rw-rw-   0        0        0    26809 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/google_shopping/domains.py
--rw-rw-rw-   0        0        0    10097 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/google_shopping/google_shopping.py
--rw-rw-rw-   0        0        0     8614 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/google_shopping/languages.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.467117 ecommerce-scraper-py-0.1.0/home_depot/
--rw-rw-rw-   0        0        0       59 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/home_depot/__init__.py
--rw-rw-rw-   0        0        0     5871 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/home_depot/home_depot.py
--rw-rw-rw-   0        0        0       42 2023-07-15 18:54:43.484152 ecommerce-scraper-py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2152 2023-07-15 18:42:34.000000 ecommerce-scraper-py-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:54:43.482121 ecommerce-scraper-py-0.1.0/walmart/
--rw-rw-rw-   0        0        0       67 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/walmart/__init__.py
--rw-rw-rw-   0        0        0   535068 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/walmart/stores.py
--rw-rw-rw-   0        0        0     8808 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.0/walmart/walmart.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.858178 ecommerce-scraper-py-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-05 00:40:16.000000 ecommerce-scraper-py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    10204 2023-07-16 03:54:47.857179 ecommerce-scraper-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8739 2023-07-16 03:54:41.000000 ecommerce-scraper-py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.721638 ecommerce-scraper-py-0.1.1/amazon/
+-rw-rw-rw-   0        0        0       61 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/amazon/__init__.py
+-rw-rw-rw-   0        0        0    24225 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/amazon/amazon.py
+-rw-rw-rw-   0        0        0     3296 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/amazon/currencies.py
+-rw-rw-rw-   0        0        0      435 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/amazon/languages.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.741631 ecommerce-scraper-py-0.1.1/ebay/
+-rw-rw-rw-   0        0        0       53 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/ebay/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/ebay/domains.py
+-rw-rw-rw-   0        0        0    12229 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/ebay/ebay.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.772179 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/
+-rw-rw-rw-   0        0        0    10204 2023-07-16 03:54:47.000000 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2023-07-16 03:54:47.000000 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 03:54:47.000000 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-16 03:54:47.000000 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2023-07-16 03:54:47.000000 ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.816180 ecommerce-scraper-py-0.1.1/google_shopping/
+-rw-rw-rw-   0        0        0       96 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/google_shopping/__init__.py
+-rw-rw-rw-   0        0        0    13956 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/google_shopping/countries.py
+-rw-rw-rw-   0        0        0    26809 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/google_shopping/domains.py
+-rw-rw-rw-   0        0        0    10097 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/google_shopping/google_shopping.py
+-rw-rw-rw-   0        0        0     8614 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/google_shopping/languages.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.831179 ecommerce-scraper-py-0.1.1/home_depot/
+-rw-rw-rw-   0        0        0       59 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/home_depot/__init__.py
+-rw-rw-rw-   0        0        0     5871 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/home_depot/home_depot.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 03:54:47.858178 ecommerce-scraper-py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2152 2023-07-16 03:40:52.000000 ecommerce-scraper-py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:54:47.856180 ecommerce-scraper-py-0.1.1/walmart/
+-rw-rw-rw-   0        0        0       67 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/walmart/__init__.py
+-rw-rw-rw-   0        0        0   535068 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/walmart/stores.py
+-rw-rw-rw-   0        0        0     8808 2023-05-29 22:07:59.000000 ecommerce-scraper-py-0.1.1/walmart/walmart.py
```

### Comparing `ecommerce-scraper-py-0.1.0/LICENSE` & `ecommerce-scraper-py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/amazon/amazon.py` & `ecommerce-scraper-py-0.1.1/amazon/amazon.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/amazon/currencies.py` & `ecommerce-scraper-py-0.1.1/amazon/currencies.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/ebay/domains.py` & `ecommerce-scraper-py-0.1.1/ebay/domains.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/ebay/ebay.py` & `ecommerce-scraper-py-0.1.1/ebay/ebay.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/ecommerce_scraper_py.egg-info/SOURCES.txt` & `ecommerce-scraper-py-0.1.1/ecommerce_scraper_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/google_shopping/countries.py` & `ecommerce-scraper-py-0.1.1/google_shopping/countries.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/google_shopping/domains.py` & `ecommerce-scraper-py-0.1.1/google_shopping/domains.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/google_shopping/google_shopping.py` & `ecommerce-scraper-py-0.1.1/google_shopping/google_shopping.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/google_shopping/languages.py` & `ecommerce-scraper-py-0.1.1/google_shopping/languages.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/home_depot/home_depot.py` & `ecommerce-scraper-py-0.1.1/home_depot/home_depot.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/setup.py` & `ecommerce-scraper-py-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='ecommerce-scraper-py',
     description = 'Scrape ecommerce websites such as Amazon, eBay, Walmart, Home Depot, Google Shopping from a single module in Python🐍',
     url='https://github.com/dimitryzub/ecommerce-scraper-py',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     author='Artur Chukhrai',
     author_email='chukhraiartur@gmail.com',
     maintainer='Artur Chukhrai, Dmitiry Zub',
     maintainer_email='chukhraiartur@gmail.com, dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
```

### Comparing `ecommerce-scraper-py-0.1.0/walmart/stores.py` & `ecommerce-scraper-py-0.1.1/walmart/stores.py`

 * *Files identical despite different names*

### Comparing `ecommerce-scraper-py-0.1.0/walmart/walmart.py` & `ecommerce-scraper-py-0.1.1/walmart/walmart.py`

 * *Files identical despite different names*

