# Comparing `tmp/spkg-0.5.3.tar.gz` & `tmp/spkg-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spkg-0.5.3.tar", last modified: Fri Jun  3 07:56:50 2022, max compression
+gzip compressed data, was "spkg-0.6.0.tar", last modified: Sun Jul 16 13:23:58 2023, max compression
```

## Comparing `spkg-0.5.3.tar` & `spkg-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xuanzhi    (501) staff       (20)        0 2022-06-03 07:56:50.589966 spkg-0.5.3/
--rw-r--r--   0 xuanzhi    (501) staff       (20)    35149 2022-06-03 05:53:17.000000 spkg-0.5.3/LICENSE
--rw-r--r--   0 xuanzhi    (501) staff       (20)     2243 2022-06-03 07:56:50.589455 spkg-0.5.3/PKG-INFO
--rw-r--r--   0 xuanzhi    (501) staff       (20)     1713 2022-06-03 05:58:30.000000 spkg-0.5.3/README.md
--rw-r--r--   0 xuanzhi    (501) staff       (20)       38 2022-06-03 07:56:50.591128 spkg-0.5.3/setup.cfg
--rw-r--r--   0 xuanzhi    (501) staff       (20)      892 2022-06-03 07:56:49.000000 spkg-0.5.3/setup.py
-drwxr-xr-x   0 xuanzhi    (501) staff       (20)        0 2022-06-03 07:56:50.578485 spkg-0.5.3/spkg/
--rw-r--r--   0 xuanzhi    (501) staff       (20)        0 2022-06-02 14:27:35.000000 spkg-0.5.3/spkg/__init__.py
--rw-r--r--   0 xuanzhi    (501) staff       (20)     5785 2022-06-03 07:56:39.000000 spkg-0.5.3/spkg/__main__.py
-drwxr-xr-x   0 xuanzhi    (501) staff       (20)        0 2022-06-03 07:56:50.586735 spkg-0.5.3/spkg.egg-info/
--rw-r--r--   0 xuanzhi    (501) staff       (20)     2243 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/PKG-INFO
--rw-r--r--   0 xuanzhi    (501) staff       (20)      230 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/SOURCES.txt
--rw-r--r--   0 xuanzhi    (501) staff       (20)        1 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/dependency_links.txt
--rw-r--r--   0 xuanzhi    (501) staff       (20)       45 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/entry_points.txt
--rw-r--r--   0 xuanzhi    (501) staff       (20)        6 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/requires.txt
--rw-r--r--   0 xuanzhi    (501) staff       (20)        5 2022-06-03 07:56:50.000000 spkg-0.5.3/spkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:58.268511 spkg-0.6.0/
+-rw-rw-rw-   0        0        0    35149 2022-06-03 05:53:17.000000 spkg-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2306 2023-07-16 13:23:58.266510 spkg-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1713 2022-06-03 05:58:30.000000 spkg-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 13:23:58.268511 spkg-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-07-16 13:23:13.000000 spkg-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:58.219388 spkg-0.6.0/spkg/
+-rw-rw-rw-   0        0        0        0 2022-06-02 14:27:35.000000 spkg-0.6.0/spkg/__init__.py
+-rw-rw-rw-   0        0        0     6125 2023-07-16 12:58:07.000000 spkg-0.6.0/spkg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:58.265511 spkg-0.6.0/spkg.egg-info/
+-rw-rw-rw-   0        0        0     2306 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-16 13:23:58.000000 spkg-0.6.0/spkg.egg-info/top_level.txt
```

### Comparing `spkg-0.5.3/LICENSE` & `spkg-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spkg-0.5.3/PKG-INFO` & `spkg-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-Metadata-Version: 2.1
-Name: spkg
-Version: 0.5.3
-Summary: Simple Packager - A command line tools for setting up and uploading python packages
-Home-page: https://github.com/xuanzhi33/spkg
-Author: xuanzhi33
-Author-email: xuanzhi33@qq.com
-License: GPL-3.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# SPKG
-
-Language: [English](https://github.com/xuanzhi33/spkg/blob/master/README.md) |
-[中文文档](https://github.com/xuanzhi33/spkg/blob/master/README_cn.md)
-
-
-## Introduction
-
-SPKG (Simple Packager) - A command line tools for setting up and uploading python packages.
-
-一个简单的命令行工具，用于快速的打包和上传python包到pypi。
-
-## Install
-
-```
-pip3 install spkg
-```
-
-## Usage
-
-Make sure you are in **the directory of your package** and run the following command:
-
-```
-spkg [command]
-```
-
-### Commands
-
-- `help`, `-h`: show this help message and exit (default)
-- `upload`, `-u`: upload the package to pypi (equals to 'twine upload dist/*')
-- `setup`, `-s`: setup the package (equals to 'python3 setup.py sdist')
-- `clear`, `-c`: delete all .tar.gz files in 'dist' folder
-- `pkg`, `-p`: clear, setup, and upload the package
-- `info`, `-in`: show package info
-- `setver`, `-sv`: set package version
-- `install`, `-i`: install a package from pypi using 'pip3 install --upgrade [package]'
-
-The commands below can change package version quickly and then run 'pkg' command:
-(They will modify the version in 'setup.py')
-- `patch`, `-pa`: Release patch update (e.g. 1.0.1 -> 1.0.2)
-- `minor`, `-mi` : Release minor update (e.g. 1.0.3 -> 1.1.0)
-- `major`, `-ma`: Release major update (e.g. 1.1.1 -> 2.0.0)
-
-### Examples
-
-- To upload all files in 'dist' folder to pypi:
-
-```
-spkg upload
-```
-
-- To setup and upload the package:
-
-```
-spkg pkg
-```
-
-- If your package's version is 1.4.2, you can run the following command to change the `version` in 'setup.py' to 1.4.3 and upload the package to pypi:
-
-```
-spkg patch
-```
-
-- To install or update a package from pypi:
-
-```
-spkg install [package]
-```
-
-
+Metadata-Version: 2.1
+Name: spkg
+Version: 0.6.0
+Summary: Simple Packager - A command line tools for setting up and uploading python packages
+Home-page: https://github.com/xuanzhi33/spkg
+Author: xuanzhi33
+Author-email: xuanzhi33@qq.com
+License: GPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SPKG
+
+Language: [English](https://github.com/xuanzhi33/spkg/blob/master/README.md) |
+[中文文档](https://github.com/xuanzhi33/spkg/blob/master/README_cn.md)
+
+
+## Introduction
+
+SPKG (Simple Packager) - A command line tools for setting up and uploading python packages.
+
+一个简单的命令行工具，用于快速的打包和上传python包到pypi。
+
+## Install
+
+```
+pip3 install spkg
+```
+
+## Usage
+
+Make sure you are in **the directory of your package** and run the following command:
+
+```
+spkg [command]
+```
+
+### Commands
+
+- `help`, `-h`: show this help message and exit (default)
+- `upload`, `-u`: upload the package to pypi (equals to 'twine upload dist/*')
+- `setup`, `-s`: setup the package (equals to 'python3 setup.py sdist')
+- `clear`, `-c`: delete all .tar.gz files in 'dist' folder
+- `pkg`, `-p`: clear, setup, and upload the package
+- `info`, `-in`: show package info
+- `setver`, `-sv`: set package version
+- `install`, `-i`: install a package from pypi using 'pip3 install --upgrade [package]'
+
+The commands below can change package version quickly and then run 'pkg' command:
+(They will modify the version in 'setup.py')
+- `patch`, `-pa`: Release patch update (e.g. 1.0.1 -> 1.0.2)
+- `minor`, `-mi` : Release minor update (e.g. 1.0.3 -> 1.1.0)
+- `major`, `-ma`: Release major update (e.g. 1.1.1 -> 2.0.0)
+
+### Examples
+
+- To upload all files in 'dist' folder to pypi:
+
+```
+spkg upload
+```
+
+- To setup and upload the package:
+
+```
+spkg pkg
+```
+
+- If your package's version is 1.4.2, you can run the following command to change the `version` in 'setup.py' to 1.4.3 and upload the package to pypi:
+
+```
+spkg patch
+```
+
+- To install or update a package from pypi:
+
+```
+spkg install [package]
+```
```

### Comparing `spkg-0.5.3/README.md` & `spkg-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `spkg-0.5.3/setup.py` & `spkg-0.6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="spkg",
-    version="0.5.3",
-    author="xuanzhi33",
-    author_email="xuanzhi33@qq.com",
-    url="https://github.com/xuanzhi33/spkg",
-    description="Simple Packager - A command line tools for setting up and uploading python packages",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: OS Independent",
-    ],
-    license="GPL-3.0",
-    install_requires=["twine"],
-    packages=find_packages(),
-    python_requires=">=3.6",
-    entry_points = {
-        "console_scripts": [
-            "spkg = spkg.__main__:main"
-        ]
-    }
-)
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="spkg",
+    version="0.6.0",
+    author="xuanzhi33",
+    author_email="xuanzhi33@qq.com",
+    url="https://github.com/xuanzhi33/spkg",
+    description="Simple Packager - A command line tools for setting up and uploading python packages",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Operating System :: OS Independent",
+    ],
+    license="GPL-3.0",
+    install_requires=["twine"],
+    packages=find_packages(),
+    python_requires=">=3.6",
+    entry_points = {
+        "console_scripts": [
+            "spkg = spkg.__main__:main"
+        ]
+    }
+)
```

### Comparing `spkg-0.5.3/spkg/__main__.py` & `spkg-0.6.0/spkg/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     output("Uploading package to \033[34mpypi\033[0m...")
     run_cmd("twine upload dist/*")
     print_done("Package uploaded.")
     
 
 def setup():
     output("Setting up package...")
-    run_cmd("python3 setup.py sdist")
+    python = sys.executable
+    run_cmd(python + " setup.py sdist")
     print_done("Setup successfully.")
 
 def clear():
     output("Deleting all .tar.gz files in 'dist' folder...")
     if os.path.exists("dist"):
         files = os.listdir("dist")
         for file in files:
@@ -144,25 +145,33 @@
     if info[1] == "":
         print_error("Package version not found in setup.py")
         return None
     
     return info
 
 def install_pkg(pkg):
-    run_cmd("pip3 install --upgrade " + pkg)
+    python = sys.executable
+    run_cmd(python + " -m pip install --upgrade " + pkg)
+
+def install_pkg_using_mirror(pkg):
+    mirror = "https://pypi.tuna.tsinghua.edu.cn/simple"
+    python = sys.executable
+    run_cmd(python + " -m pip install --upgrade " + pkg + " -i " + mirror)
 
 def main():
     argv = sys.argv
     if len(argv) == 1:
         help()
     elif argv[1] == "-h" or argv[1] == "help":
         help()
     elif argv[1] == "-i" or argv[1] == "install":
         if len(argv) == 3:
             install_pkg(argv[2])
+        elif len(argv) == 4:
+            install_pkg_using_mirror(argv[3])
         else:
             pkgname = input("package name: ")
             install_pkg(pkgname)
     else:
         pkginfo = check_pkg()
         if pkginfo is not None:
             if argv[1] == "-u" or argv[1] == "upload":
```

### Comparing `spkg-0.5.3/spkg.egg-info/PKG-INFO` & `spkg-0.6.0/spkg.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-Metadata-Version: 2.1
-Name: spkg
-Version: 0.5.3
-Summary: Simple Packager - A command line tools for setting up and uploading python packages
-Home-page: https://github.com/xuanzhi33/spkg
-Author: xuanzhi33
-Author-email: xuanzhi33@qq.com
-License: GPL-3.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# SPKG
-
-Language: [English](https://github.com/xuanzhi33/spkg/blob/master/README.md) |
-[中文文档](https://github.com/xuanzhi33/spkg/blob/master/README_cn.md)
-
-
-## Introduction
-
-SPKG (Simple Packager) - A command line tools for setting up and uploading python packages.
-
-一个简单的命令行工具，用于快速的打包和上传python包到pypi。
-
-## Install
-
-```
-pip3 install spkg
-```
-
-## Usage
-
-Make sure you are in **the directory of your package** and run the following command:
-
-```
-spkg [command]
-```
-
-### Commands
-
-- `help`, `-h`: show this help message and exit (default)
-- `upload`, `-u`: upload the package to pypi (equals to 'twine upload dist/*')
-- `setup`, `-s`: setup the package (equals to 'python3 setup.py sdist')
-- `clear`, `-c`: delete all .tar.gz files in 'dist' folder
-- `pkg`, `-p`: clear, setup, and upload the package
-- `info`, `-in`: show package info
-- `setver`, `-sv`: set package version
-- `install`, `-i`: install a package from pypi using 'pip3 install --upgrade [package]'
-
-The commands below can change package version quickly and then run 'pkg' command:
-(They will modify the version in 'setup.py')
-- `patch`, `-pa`: Release patch update (e.g. 1.0.1 -> 1.0.2)
-- `minor`, `-mi` : Release minor update (e.g. 1.0.3 -> 1.1.0)
-- `major`, `-ma`: Release major update (e.g. 1.1.1 -> 2.0.0)
-
-### Examples
-
-- To upload all files in 'dist' folder to pypi:
-
-```
-spkg upload
-```
-
-- To setup and upload the package:
-
-```
-spkg pkg
-```
-
-- If your package's version is 1.4.2, you can run the following command to change the `version` in 'setup.py' to 1.4.3 and upload the package to pypi:
-
-```
-spkg patch
-```
-
-- To install or update a package from pypi:
-
-```
-spkg install [package]
-```
-
-
+Metadata-Version: 2.1
+Name: spkg
+Version: 0.6.0
+Summary: Simple Packager - A command line tools for setting up and uploading python packages
+Home-page: https://github.com/xuanzhi33/spkg
+Author: xuanzhi33
+Author-email: xuanzhi33@qq.com
+License: GPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SPKG
+
+Language: [English](https://github.com/xuanzhi33/spkg/blob/master/README.md) |
+[中文文档](https://github.com/xuanzhi33/spkg/blob/master/README_cn.md)
+
+
+## Introduction
+
+SPKG (Simple Packager) - A command line tools for setting up and uploading python packages.
+
+一个简单的命令行工具，用于快速的打包和上传python包到pypi。
+
+## Install
+
+```
+pip3 install spkg
+```
+
+## Usage
+
+Make sure you are in **the directory of your package** and run the following command:
+
+```
+spkg [command]
+```
+
+### Commands
+
+- `help`, `-h`: show this help message and exit (default)
+- `upload`, `-u`: upload the package to pypi (equals to 'twine upload dist/*')
+- `setup`, `-s`: setup the package (equals to 'python3 setup.py sdist')
+- `clear`, `-c`: delete all .tar.gz files in 'dist' folder
+- `pkg`, `-p`: clear, setup, and upload the package
+- `info`, `-in`: show package info
+- `setver`, `-sv`: set package version
+- `install`, `-i`: install a package from pypi using 'pip3 install --upgrade [package]'
+
+The commands below can change package version quickly and then run 'pkg' command:
+(They will modify the version in 'setup.py')
+- `patch`, `-pa`: Release patch update (e.g. 1.0.1 -> 1.0.2)
+- `minor`, `-mi` : Release minor update (e.g. 1.0.3 -> 1.1.0)
+- `major`, `-ma`: Release major update (e.g. 1.1.1 -> 2.0.0)
+
+### Examples
+
+- To upload all files in 'dist' folder to pypi:
+
+```
+spkg upload
+```
+
+- To setup and upload the package:
+
+```
+spkg pkg
+```
+
+- If your package's version is 1.4.2, you can run the following command to change the `version` in 'setup.py' to 1.4.3 and upload the package to pypi:
+
+```
+spkg patch
+```
+
+- To install or update a package from pypi:
+
+```
+spkg install [package]
+```
```

