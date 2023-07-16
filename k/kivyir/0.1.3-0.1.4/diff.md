# Comparing `tmp/kivyir-0.1.3.tar.gz` & `tmp/kivyir-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kivyir-0.1.3.tar", last modified: Thu Oct 27 22:56:25 2022, max compression
+gzip compressed data, was "dist\kivyir-0.1.4.tar", last modified: Sun Jul 16 07:53:33 2023, max compression
```

## Comparing `kivyir-0.1.3.tar` & `kivyir-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-10-27 22:56:25.000000 kivyir-0.1.3/
--rw-rw-rw-   0        0        0     3109 2022-10-27 22:56:25.000000 kivyir-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2022-10-27 22:51:22.000000 kivyir-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir/
--rw-rw-rw-   0        0        0    25787 2022-10-27 22:53:57.000000 kivyir-0.1.3/kivyir/ConfigBase.py
--rw-rw-rw-   0        0        0      446 2022-10-26 20:59:53.000000 kivyir-0.1.3/kivyir/IrLabel.py
--rw-rw-rw-   0        0        0     4010 2022-10-27 14:18:06.000000 kivyir-0.1.3/kivyir/IrTextInput.py
--rw-rw-rw-   0        0        0      258 2022-10-27 22:51:22.000000 kivyir-0.1.3/kivyir/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir/font/
--rw-rw-rw-   0        0        0    76372 2020-02-21 17:22:52.000000 kivyir-0.1.3/kivyir/font/Sahel-Bold.ttf
--rw-rw-rw-   0        0        0    75308 2020-02-21 17:22:57.000000 kivyir-0.1.3/kivyir/font/Sahel.ttf
-drwxrwxrwx   0        0        0        0 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/
--rw-rw-rw-   0        0        0     3109 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-10-27 22:56:25.000000 kivyir-0.1.3/kivyir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-27 22:56:25.000000 kivyir-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1821 2022-10-27 22:55:11.000000 kivyir-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-27 22:56:25.000000 kivyir-0.1.3/test/
--rw-rw-rw-   0        0        0      915 2022-10-27 22:54:03.000000 kivyir-0.1.3/test/main.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/
+-rw-rw-rw-   0        0        0     1069 2023-07-14 09:57:59.000000 kivyir-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2755 2023-07-16 07:53:33.000000 kivyir-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1487 2023-07-14 09:57:59.000000 kivyir-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir/
+-rw-rw-rw-   0        0        0    26727 2023-07-16 07:52:04.000000 kivyir-0.1.4/kivyir/ConfigBase.py
+-rw-rw-rw-   0        0        0      422 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/IrLabel.py
+-rw-rw-rw-   0        0        0     4010 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/IrTextInput.py
+-rw-rw-rw-   0        0        0      258 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir/font/
+-rw-rw-rw-   0        0        0    76372 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/font/Sahel-Bold.ttf
+-rw-rw-rw-   0        0        0    75308 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/font/Sahel.ttf
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/
+-rw-rw-rw-   0        0        0     2755 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 07:53:33.000000 kivyir-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2023-07-16 07:25:57.000000 kivyir-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/test/
+-rw-rw-rw-   0        0        0     1216 2023-07-16 07:32:53.000000 kivyir-0.1.4/test/main.py
```

### Comparing `kivyir-0.1.3/PKG-INFO` & `kivyir-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivyir
-Version: 0.1.3
+Version: 0.1.4
 Summary: Improving the display of Persian text for Persian speakers
 Home-page: https://github.com/goldaaa/kivyir
 Download-URL: https://github.com/goldaaa/kivyir/tarball/master
 Author: navid nasiri
 Author-email: goldaaa.program@gmail.com
 Maintainer: navid nasiri
 Maintainer-email: goldaaa.program@gmail.com
@@ -22,28 +22,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# kivyir | kivy persian | kivy فارسی
+# kivy persian
 
-The first kivy Persian users for Iranians.
+The first kivy Persian users.
 
 I converted the kivy library into Farsi for Iranians so that Iranians can use it.
 
-کتابخانه کیوی را برای ایرانیان به فارسی تبدیل کردم تا ایرانی ها بتوانند از آن استفاده کنند.
-
 I have added a sample test file so you can understand how to use it.
 
-یک نمونه فایل تست اضافه کردم تا بتوانید نحوه استفاده از آن را بدانید.
-
-
 Download
 --------
 You can install this from pypi.
 
     pip install kivyir
     
 You can also install from this repository.
@@ -86,16 +82,21 @@
     from kivyir import IrLabel, IrTextInput
 
 [Sample image tested](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
 
 ![](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
 
 
-If you are interested in financial support, you can send a message through Gmail if you have any questions.
+Install the required package
+--------
+    kivy
+    facleaning
+
 
-اگر قصد حمایت مالی یا سوال دارید می توانید از طریق جیمیل پیام ارسال کنید.
+
+If you are interested in financial support, you can send a message through Gmail if you have any questions.
 
 gmail: goldaaa.program@gmail.com
 
-[Telegram group of this project: t.me/kivyiran](http://t.me/kivyiran)
+[github kivy persian](https://github.com/goldaaa/kivyir)
 
-[github facleaning](https://github.com/goldaaa/kivyir)
+If you Arab speaking friends need to use it, let me know so that I can apply it for you too.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kivyir-0.1.3/README.md` & `kivyir-0.1.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# kivyir | kivy persian | kivy فارسی
-
-The first kivy Persian users for Iranians.
-
-I converted the kivy library into Farsi for Iranians so that Iranians can use it.
-
-کتابخانه کیوی را برای ایرانیان به فارسی تبدیل کردم تا ایرانی ها بتوانند از آن استفاده کنند.
-
-I have added a sample test file so you can understand how to use it.
-
-یک نمونه فایل تست اضافه کردم تا بتوانید نحوه استفاده از آن را بدانید.
-
-
-Download
---------
-You can install this from pypi.
-
-    pip install kivyir
-    
-You can also install from this repository.
-
-    git clone https://github.com/goldaaa/kivyir.git
-
-Then, install the library with
-
-    python setup.py install
-
-
-Importing
----------
-
-Import kivyir commands, menus, and the shell
-
-    from kivyir import *        # Line 1 should always be placed
-
-
-Commands
---------
-
-Commands that can be used
-    
-Some changes if needed
-
-    from kivyir import *
-    config = Config()
-    config.change(
-        direction='ltr',
-        font_name='Sahel',
-        file_regular='{path}.ttf',
-        file_bold='{path}.ttf',
-        file_italic='{path}.ttf',
-        file_bolditalic='{path}.ttf'
-    )
-
-Custom made
-
-    from kivyir import IrLabel, IrTextInput
-
-[Sample image tested](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
-
-![](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
-
-
-If you are interested in financial support, you can send a message through Gmail if you have any questions.
-
-اگر قصد حمایت مالی یا سوال دارید می توانید از طریق جیمیل پیام ارسال کنید.
-
-gmail: goldaaa.program@gmail.com
-
-[Telegram group of this project: t.me/kivyiran](http://t.me/kivyiran)
-
-[github facleaning](https://github.com/goldaaa/kivyir)
+# kivy persian
+
+The first kivy Persian users.
+
+I converted the kivy library into Farsi for Iranians so that Iranians can use it.
+
+I have added a sample test file so you can understand how to use it.
+
+Download
+--------
+You can install this from pypi.
+
+    pip install kivyir
+    
+You can also install from this repository.
+
+    git clone https://github.com/goldaaa/kivyir.git
+
+Then, install the library with
+
+    python setup.py install
+
+
+Importing
+---------
+
+Import kivyir commands, menus, and the shell
+
+    from kivyir import *        # Line 1 should always be placed
+
+
+Commands
+--------
+
+Commands that can be used
+    
+Some changes if needed
+
+    from kivyir import *
+    config = Config()
+    config.change(
+        direction='ltr',
+        font_name='Sahel',
+        file_regular='{path}.ttf',
+        file_bold='{path}.ttf',
+        file_italic='{path}.ttf',
+        file_bolditalic='{path}.ttf'
+    )
+
+Custom made
+
+    from kivyir import IrLabel, IrTextInput
+
+[Sample image tested](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
+
+![](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
+
+
+Install the required package
+--------
+    kivy
+    facleaning
+
+
+
+If you are interested in financial support, you can send a message through Gmail if you have any questions.
+
+gmail: goldaaa.program@gmail.com
+
+[github kivy persian](https://github.com/goldaaa/kivyir)
+
+If you Arab speaking friends need to use it, let me know so that I can apply it for you too.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kivyir-0.1.3/kivyir/ConfigBase.py` & `kivyir-0.1.4/kivyir/ConfigBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,18 @@
             italic=False, underline=False, strikethrough=False, font_family=None,
             halign='left', valign='bottom', shorten=False,
             text_size=None, mipmap=False, color=None, line_height=1.0, strip=False,
             strip_reflow=True, shorten_from='center', split_str=' ',
             unicode_errors='replace',
             font_hinting='normal', font_kerning=True, font_blended=True,
             outline_width=None, outline_color=None, font_context=None,
-            font_features=None, base_direction=None, text_language=None,
+            font_features=None, base_direction=None, font_direction='ltr',
+            font_script_name='Latin', text_language=None,
             **kwargs):
+
         # Include system fonts_dir in resource paths.
         # This allows us to specify a font from those dirs.
         self.get_system_fonts_dir()
 
         options = {'text': text, 'font_size': font_size,
                    'font_name': font_name, 'bold': bold, 'italic': italic,
                    'underline': underline, 'strikethrough': strikethrough,
@@ -46,20 +48,37 @@
                    'font_hinting': font_hinting,
                    'font_kerning': font_kerning,
                    'font_blended': font_blended,
                    'outline_width': outline_width,
                    'font_context': font_context,
                    'font_features': font_features,
                    'base_direction': base_direction,
+                   'font_direction': font_direction,
+                   'font_script_name': font_script_name,
                    'text_language': text_language}
 
         kwargs_get = kwargs.get
         options['color'] = color or (1, 1, 1, 1)
         options['outline_color'] = outline_color or (0, 0, 0, 1)
-        options['padding'] = kwargs_get('padding', (0, 0))
+
+        options['padding'] = kwargs_get('padding', [0, 0, 0, 0])
+        if isinstance(options['padding'], (int, float)):
+            options['padding'] = [options['padding']] * 4
+        elif (isinstance(options['padding'], (list, tuple)) and len(options['padding']) != 4):
+            if len(options['padding']) == 1:
+                options['padding'] = options['padding'] * 4
+            elif len(options['padding']) == 2:
+                options['padding'] = options['padding'] * 2
+            else:
+                raise ValueError(
+                    "padding should be int|float or a list|tuple with 1, 2 or "
+                    f"4 elements, got {type(options['padding'])} with "
+                    f"{len(options['padding'])} elements."
+                )
+
         if not isinstance(options['padding'], (list, tuple)):
             options['padding'] = (options['padding'], options['padding'])
         options['padding_x'] = kwargs_get('padding_x', options['padding'][0]) + 10
         options['padding_y'] = kwargs_get('padding_y', options['padding'][1])
 
         if 'size' in kwargs:
             options['text_size'] = kwargs['size']
@@ -74,14 +93,15 @@
         self._internal_size = 0, 0  # the real computed text size (inclds pad)
         self._cached_lines = []
 
         self.options = options
         self.texture = None
         self.is_shortened = False
         self.resolve_font_name()
+        self._migrate_deprecated_padding_xy()
 
     def render(self, real=False):
         '''Return a tuple (width, height) to create the image
         with the user constraints. (width, height) includes the padding.
         '''
         if real:
             return self._render_real()
@@ -610,11 +630,7 @@
         text._default_font_paths = self.font_files
         text.DEFAULT_FONT = self.font_name
         text.LabelBase.register(self.font_name, *self.font_files)
         return True
 
 
 Config().change()
-
-
-
-
```

### Comparing `kivyir-0.1.3/kivyir/IrTextInput.py` & `kivyir-0.1.4/kivyir/IrTextInput.py`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.3/kivyir/font/Sahel-Bold.ttf` & `kivyir-0.1.4/kivyir/font/Sahel-Bold.ttf`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.3/kivyir/font/Sahel.ttf` & `kivyir-0.1.4/kivyir/font/Sahel.ttf`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.3/kivyir.egg-info/PKG-INFO` & `kivyir-0.1.4/kivyir.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivyir
-Version: 0.1.3
+Version: 0.1.4
 Summary: Improving the display of Persian text for Persian speakers
 Home-page: https://github.com/goldaaa/kivyir
 Download-URL: https://github.com/goldaaa/kivyir/tarball/master
 Author: navid nasiri
 Author-email: goldaaa.program@gmail.com
 Maintainer: navid nasiri
 Maintainer-email: goldaaa.program@gmail.com
@@ -22,28 +22,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# kivyir | kivy persian | kivy فارسی
+# kivy persian
 
-The first kivy Persian users for Iranians.
+The first kivy Persian users.
 
 I converted the kivy library into Farsi for Iranians so that Iranians can use it.
 
-کتابخانه کیوی را برای ایرانیان به فارسی تبدیل کردم تا ایرانی ها بتوانند از آن استفاده کنند.
-
 I have added a sample test file so you can understand how to use it.
 
-یک نمونه فایل تست اضافه کردم تا بتوانید نحوه استفاده از آن را بدانید.
-
-
 Download
 --------
 You can install this from pypi.
 
     pip install kivyir
     
 You can also install from this repository.
@@ -86,16 +82,21 @@
     from kivyir import IrLabel, IrTextInput
 
 [Sample image tested](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
 
 ![](https://github.com/goldaaa/kivyir/blob/main/test/sampel_test.png)
 
 
-If you are interested in financial support, you can send a message through Gmail if you have any questions.
+Install the required package
+--------
+    kivy
+    facleaning
+
 
-اگر قصد حمایت مالی یا سوال دارید می توانید از طریق جیمیل پیام ارسال کنید.
+
+If you are interested in financial support, you can send a message through Gmail if you have any questions.
 
 gmail: goldaaa.program@gmail.com
 
-[Telegram group of this project: t.me/kivyiran](http://t.me/kivyiran)
+[github kivy persian](https://github.com/goldaaa/kivyir)
 
-[github facleaning](https://github.com/goldaaa/kivyir)
+If you Arab speaking friends need to use it, let me know so that I can apply it for you too.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kivyir-0.1.3/setup.py` & `kivyir-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#!/usr/bin/env python
-# coding=utf-8
-
-from setuptools import setup
-import io
-
-with io.open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="kivyir",
-    description="Improving the display of Persian text for Persian speakers",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    version='0.1.3',
-    platforms="ALL",
-    license="MIT",
-    packages=['kivyir', 'test'],
-    install_requires=["kivy>=2.0.0", "pillow", "facleaning"],
-    author="navid nasiri",
-    author_email="goldaaa.program@gmail.com",
-    maintainer="navid nasiri",
-    maintainer_email="goldaaa.program@gmail.com",
-    package_dir={'kivyir': 'kivyir'},
-    test_suite='kivyir.test',
-    include_package_data=True,
-    keywords="kivy persian farsi iran",
-    url="https://github.com/goldaaa/kivyir",
-    download_url="https://github.com/goldaaa/kivyir/tarball/master",
-    package_data={
-        "kivyir": ["font/*.ttf",]
-    },
-    setup_requires=[],
-    python_requires=">=3.5",
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: Persian',
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        'Topic :: Software Development :: User Interfaces',
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],  # https://test.pypi.org/pypi?%3Aaction=list_classifiers
-)
+#!/usr/bin/env python
+# coding=utf-8
+
+from setuptools import setup
+import io
+
+with io.open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="kivyir",
+    description="Improving the display of Persian text for Persian speakers",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    version='0.1.4',
+    platforms="ALL",
+    license="MIT",
+    packages=['kivyir', 'test'],
+    install_requires=["kivy>=2.0.0", "pillow", "facleaning"],
+    author="navid nasiri",
+    author_email="goldaaa.program@gmail.com",
+    maintainer="navid nasiri",
+    maintainer_email="goldaaa.program@gmail.com",
+    package_dir={'kivyir': 'kivyir'},
+    test_suite='kivyir.test',
+    include_package_data=True,
+    keywords="kivy persian farsi iran",
+    url="https://github.com/goldaaa/kivyir",
+    download_url="https://github.com/goldaaa/kivyir/tarball/master",
+    package_data={
+        "kivyir": ["font/*.ttf",]
+    },
+    setup_requires=[],
+    python_requires=">=3.5",
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: Persian',
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        'Topic :: Software Development :: User Interfaces',
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
+)
```

### Comparing `kivyir-0.1.3/test/main.py` & `kivyir-0.1.4/test/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,38 @@
+from kivy import Config
+Config.set('graphics', 'multisamples', '0')
+
 from kivyir import *
+config = Config()
+config.change(
+    direction='rtl',
+    # font_name='Sahel',
+    # file_regular='{path}.ttf',
+    # file_bold='{path}.ttf',
+    # file_italic='{path}.ttf',
+    # file_bolditalic='{path}.ttf'
+)
+
 from kivy.app import App
 from kivy.lang import Builder
 
 
 kv = Builder.load_string("""
 BoxLayout:
     orientation: 'vertical'
 
     IrLabel:
         text: 'این یک متن برای تست می باشد, این دو متن برای تست می باشد, این سه متن برای تست می باشد.'
         height: 200
-        valign: 'center'
         halign: 'right'
-
+        
     IrTextInput:
-        base_direction: 'rtl'
+        # base_direction: 'rtl'
         text: 'این یک متن برای تست می باشد, این دو متن برای تست می باشد, این سه متن برای تست می باشد.'
-
+        halign: 'right'
         use_handles: True
         cursor_color: (1, 0, 0, 1)
         cursor_width: '2sp'
         foreground_color: (0, 0, 0, 1)
         background_color: (1, 1, 1, 1)
 """)
```

