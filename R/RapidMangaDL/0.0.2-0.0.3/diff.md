# Comparing `tmp/RapidMangaDL-0.0.2.tar.gz` & `tmp/RapidMangaDL-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RapidMangaDL-0.0.2.tar", last modified: Sun Jul 16 17:30:21 2023, max compression
+gzip compressed data, was "RapidMangaDL-0.0.3.tar", last modified: Sun Jul 16 17:35:41 2023, max compression
```

## Comparing `RapidMangaDL-0.0.2.tar` & `RapidMangaDL-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.989537 RapidMangaDL-0.0.2/
--rw-rw-rw-   0        0        0     4743 2023-07-16 17:30:21.987534 RapidMangaDL-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3339 2023-07-16 17:29:13.000000 RapidMangaDL-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.898511 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/
--rw-rw-rw-   0        0        0     4743 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 17:30:21.000000 RapidMangaDL-0.0.2/RapidMangaDL.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.913541 RapidMangaDL-0.0.2/manga_dl/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:52:51.000000 RapidMangaDL-0.0.2/manga_dl/__init__.py
--rw-rw-rw-   0        0        0     6763 2023-07-16 15:26:29.000000 RapidMangaDL-0.0.2/manga_dl/app.py
--rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.0.2/manga_dl/jsconfig.json
--rw-rw-rw-   0        0        0     6287 2023-07-16 16:02:19.000000 RapidMangaDL-0.0.2/manga_dl/main.py
--rw-rw-rw-   0        0        0    23640 2023-07-16 15:27:37.000000 RapidMangaDL-0.0.2/manga_dl/manga.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.947530 RapidMangaDL-0.0.2/manga_dl/public/
--rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.0.2/manga_dl/public/bootstrap530.css
--rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.0.2/manga_dl/public/bootstrap530.js
--rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.0.2/manga_dl/public/error.png
--rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.0.2/manga_dl/public/jquery321.js
--rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.0.2/manga_dl/public/loading-fast.gif
--rw-rw-rw-   0        0        0     6615 2023-07-16 06:37:18.000000 RapidMangaDL-0.0.2/manga_dl/public/manga.js
--rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.0.2/manga_dl/public/search.js
--rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.0.2/manga_dl/public/style.css
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.958532 RapidMangaDL-0.0.2/manga_dl/templates/
--rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.0.2/manga_dl/templates/chapter.html
--rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.0.2/manga_dl/templates/layout.html
--rw-rw-rw-   0        0        0    13010 2023-07-16 06:36:57.000000 RapidMangaDL-0.0.2/manga_dl/templates/manga.html
--rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.0.2/manga_dl/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-16 17:30:21.985528 RapidMangaDL-0.0.2/manga_dl/tools/
--rw-rw-rw-   0        0        0      130 2023-07-15 17:00:11.000000 RapidMangaDL-0.0.2/manga_dl/tools/__init__.py
--rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.0.2/manga_dl/tools/create_pdf.py
--rw-rw-rw-   0        0        0     9657 2023-07-13 17:42:34.000000 RapidMangaDL-0.0.2/manga_dl/tools/download.py
--rw-rw-rw-   0        0        0     6643 2023-07-16 17:18:45.000000 RapidMangaDL-0.0.2/manga_dl/tools/downloader2.py
--rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.0.2/manga_dl/tools/downloader3.py
--rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.0.2/manga_dl/tools/exceptions.py
--rw-rw-rw-   0        0        0     1323 2023-07-16 05:03:19.000000 RapidMangaDL-0.0.2/manga_dl/tools/models.py
--rw-rw-rw-   0        0        0    22761 2023-07-16 14:34:36.000000 RapidMangaDL-0.0.2/manga_dl/tools/sources.py
--rw-rw-rw-   0        0        0     4435 2023-07-16 15:16:03.000000 RapidMangaDL-0.0.2/manga_dl/tools/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-16 17:30:21.990534 RapidMangaDL-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2187 2023-07-16 17:30:06.000000 RapidMangaDL-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.563409 RapidMangaDL-0.0.3/
+-rw-rw-rw-   0        0        0     4741 2023-07-16 17:35:41.562406 RapidMangaDL-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3337 2023-07-16 17:35:03.000000 RapidMangaDL-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.500063 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/
+-rw-rw-rw-   0        0        0     4741 2023-07-16 17:35:40.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-07-16 17:35:41.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:35:40.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 17:35:40.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2023-07-16 17:35:40.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 17:35:40.000000 RapidMangaDL-0.0.3/RapidMangaDL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.511594 RapidMangaDL-0.0.3/manga_dl/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:52:51.000000 RapidMangaDL-0.0.3/manga_dl/__init__.py
+-rw-rw-rw-   0        0        0     6763 2023-07-16 15:26:29.000000 RapidMangaDL-0.0.3/manga_dl/app.py
+-rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.0.3/manga_dl/jsconfig.json
+-rw-rw-rw-   0        0        0     6287 2023-07-16 16:02:19.000000 RapidMangaDL-0.0.3/manga_dl/main.py
+-rw-rw-rw-   0        0        0    23640 2023-07-16 15:27:37.000000 RapidMangaDL-0.0.3/manga_dl/manga.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.531749 RapidMangaDL-0.0.3/manga_dl/public/
+-rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.0.3/manga_dl/public/bootstrap530.css
+-rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.0.3/manga_dl/public/bootstrap530.js
+-rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.0.3/manga_dl/public/error.png
+-rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.0.3/manga_dl/public/jquery321.js
+-rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.0.3/manga_dl/public/loading-fast.gif
+-rw-rw-rw-   0        0        0     6615 2023-07-16 06:37:18.000000 RapidMangaDL-0.0.3/manga_dl/public/manga.js
+-rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.0.3/manga_dl/public/search.js
+-rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.0.3/manga_dl/public/style.css
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.540288 RapidMangaDL-0.0.3/manga_dl/templates/
+-rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.0.3/manga_dl/templates/chapter.html
+-rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.0.3/manga_dl/templates/layout.html
+-rw-rw-rw-   0        0        0    13010 2023-07-16 06:36:57.000000 RapidMangaDL-0.0.3/manga_dl/templates/manga.html
+-rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.0.3/manga_dl/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:41.559371 RapidMangaDL-0.0.3/manga_dl/tools/
+-rw-rw-rw-   0        0        0      130 2023-07-15 17:00:11.000000 RapidMangaDL-0.0.3/manga_dl/tools/__init__.py
+-rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.0.3/manga_dl/tools/create_pdf.py
+-rw-rw-rw-   0        0        0     9657 2023-07-13 17:42:34.000000 RapidMangaDL-0.0.3/manga_dl/tools/download.py
+-rw-rw-rw-   0        0        0     6643 2023-07-16 17:18:45.000000 RapidMangaDL-0.0.3/manga_dl/tools/downloader2.py
+-rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.0.3/manga_dl/tools/downloader3.py
+-rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.0.3/manga_dl/tools/exceptions.py
+-rw-rw-rw-   0        0        0     1323 2023-07-16 05:03:19.000000 RapidMangaDL-0.0.3/manga_dl/tools/models.py
+-rw-rw-rw-   0        0        0    22761 2023-07-16 14:34:36.000000 RapidMangaDL-0.0.3/manga_dl/tools/sources.py
+-rw-rw-rw-   0        0        0     4435 2023-07-16 15:16:03.000000 RapidMangaDL-0.0.3/manga_dl/tools/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 17:35:41.564406 RapidMangaDL-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2187 2023-07-16 17:34:50.000000 RapidMangaDL-0.0.3/setup.py
```

### Comparing `RapidMangaDL-0.0.2/PKG-INFO` & `RapidMangaDL-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.0.2
+Version: 0.0.3
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
@@ -58,29 +58,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/cli_demo.gif)
+![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/web_demo.gif)
+![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 # Command Line Interface (CLI)
 
 The CLI mode allows you to interact with the application using command-line arguments. Here's an example of how you can use it:
 
 ```bash
 manga-dl cli -m https://manganato.com/manga-az963307 -c 1-10 -f epub -q 90
```

### Comparing `RapidMangaDL-0.0.2/README.md` & `RapidMangaDL-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/cli_demo.gif)
+![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/web_demo.gif)
+![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 # Command Line Interface (CLI)
 
 The CLI mode allows you to interact with the application using command-line arguments. Here's an example of how you can use it:
 
 ```bash
 manga-dl cli -m https://manganato.com/manga-az963307 -c 1-10 -f epub -q 90
```

### Comparing `RapidMangaDL-0.0.2/RapidMangaDL.egg-info/PKG-INFO` & `RapidMangaDL-0.0.3/RapidMangaDL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.0.2
+Version: 0.0.3
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
@@ -58,29 +58,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/cli_demo.gif)
+![Interactive CLI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/blob/main/web_demo.gif)
+![Web-based GUI Demo](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 # Command Line Interface (CLI)
 
 The CLI mode allows you to interact with the application using command-line arguments. Here's an example of how you can use it:
 
 ```bash
 manga-dl cli -m https://manganato.com/manga-az963307 -c 1-10 -f epub -q 90
```

### Comparing `RapidMangaDL-0.0.2/RapidMangaDL.egg-info/SOURCES.txt` & `RapidMangaDL-0.0.3/RapidMangaDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/app.py` & `RapidMangaDL-0.0.3/manga_dl/app.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/main.py` & `RapidMangaDL-0.0.3/manga_dl/main.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/manga.py` & `RapidMangaDL-0.0.3/manga_dl/manga.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/bootstrap530.css` & `RapidMangaDL-0.0.3/manga_dl/public/bootstrap530.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/bootstrap530.js` & `RapidMangaDL-0.0.3/manga_dl/public/bootstrap530.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/error.png` & `RapidMangaDL-0.0.3/manga_dl/public/error.png`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/jquery321.js` & `RapidMangaDL-0.0.3/manga_dl/public/jquery321.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/loading-fast.gif` & `RapidMangaDL-0.0.3/manga_dl/public/loading-fast.gif`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/manga.js` & `RapidMangaDL-0.0.3/manga_dl/public/manga.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/search.js` & `RapidMangaDL-0.0.3/manga_dl/public/search.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/public/style.css` & `RapidMangaDL-0.0.3/manga_dl/public/style.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/templates/chapter.html` & `RapidMangaDL-0.0.3/manga_dl/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/templates/layout.html` & `RapidMangaDL-0.0.3/manga_dl/templates/layout.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/templates/manga.html` & `RapidMangaDL-0.0.3/manga_dl/templates/manga.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/templates/search.html` & `RapidMangaDL-0.0.3/manga_dl/templates/search.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/create_pdf.py` & `RapidMangaDL-0.0.3/manga_dl/tools/create_pdf.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/download.py` & `RapidMangaDL-0.0.3/manga_dl/tools/download.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/downloader2.py` & `RapidMangaDL-0.0.3/manga_dl/tools/downloader2.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/downloader3.py` & `RapidMangaDL-0.0.3/manga_dl/tools/downloader3.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/models.py` & `RapidMangaDL-0.0.3/manga_dl/tools/models.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/sources.py` & `RapidMangaDL-0.0.3/manga_dl/tools/sources.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/manga_dl/tools/utils.py` & `RapidMangaDL-0.0.3/manga_dl/tools/utils.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.0.2/setup.py` & `RapidMangaDL-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
 package_name = "RapidMangaDL"
-package_version = "0.0.2"
+package_version = "0.0.3"
 package_description = "Swiftly download manga from multiple sources."
 package_author = "sifat"
 package_author_email = "hossain0338@gmail.com"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

