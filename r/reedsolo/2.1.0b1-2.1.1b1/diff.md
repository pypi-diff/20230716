# Comparing `tmp/reedsolo-2.1.0b1.tar.gz` & `tmp/reedsolo-2.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reedsolo-2.1.0b1.tar", last modified: Tue Apr 11 12:36:05 2023, max compression
+gzip compressed data, was "reedsolo-2.1.1b1.tar", last modified: Sat Jul 15 22:09:18 2023, max compression
```

## Comparing `reedsolo-2.1.0b1.tar` & `reedsolo-2.1.1b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43543 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.682986 reedsolo-2.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/creedsolo/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2240244 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/creedsolo.c
--rw-r--r--   0 runner    (1001) docker     (123)    85611 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/creedsolo/creedsolo.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/reedsolo/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/reedsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78312 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/src/reedsolo/reedsolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/src/reedsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43543 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 12:36:05.000000 reedsolo-2.1.0b1/src/reedsolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:36:05.686987 reedsolo-2.1.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/tests/test_creedsolo.py
--rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-04-11 12:35:57.000000 reedsolo-2.1.0b1/tests/test_reedsolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.833787 reedsolo-2.1.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    45021 2023-07-15 22:09:18.833787 reedsolo-2.1.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39531 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:09:18.833787 reedsolo-2.1.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.825787 reedsolo-2.1.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.829787 reedsolo-2.1.1b1/src/creedsolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/src/creedsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2240244 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/src/creedsolo/creedsolo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    85611 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/src/creedsolo/creedsolo.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.829787 reedsolo-2.1.1b1/src/reedsolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/src/reedsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78556 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/src/reedsolo/reedsolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.833787 reedsolo-2.1.1b1/src/reedsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45021 2023-07-15 22:09:18.000000 reedsolo-2.1.1b1/src/reedsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 22:09:18.000000 reedsolo-2.1.1b1/src/reedsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:09:18.000000 reedsolo-2.1.1b1/src/reedsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-15 22:09:18.000000 reedsolo-2.1.1b1/src/reedsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 22:09:18.000000 reedsolo-2.1.1b1/src/reedsolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:09:18.833787 reedsolo-2.1.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/tests/test_creedsolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34462 2023-07-15 22:09:05.000000 reedsolo-2.1.1b1/tests/test_reedsolo.py
```

### Comparing `reedsolo-2.1.0b1/LICENSE` & `reedsolo-2.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `reedsolo-2.1.0b1/MANIFEST.in` & `reedsolo-2.1.1b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `reedsolo-2.1.0b1/PKG-INFO` & `reedsolo-2.1.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reedsolo
-Version: 2.1.0b1
+Version: 2.1.1b1
 Summary: Pythonic universal errors-and-erasures Reed-Solomon codec to protect your data from errors and bitrot, with a future-proof zero-dependencies pure-python implementation and an optional speed-optimized Cython/C extension.
 Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: The software is available under your choice of
         Unlicense (SPDX short identifier: Unlicense) or
         MIT No Attribution License (SPDX short identifier: MIT-0):
         
@@ -52,40 +52,42 @@
 Project-URL: Source, https://github.com/tomerfiliba-org/reedsolomon
 Project-URL: Tracker, https://github.com/tomerfiliba-org/reedsolomon/issues
 Project-URL: Download, https://github.com/tomerfiliba-org/reedsolomon/releases
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
 Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: testmeta
 Provides-Extra: testoptional
 License-File: LICENSE
 
@@ -128,38 +130,38 @@
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 .. code:: sh
 
     pip install --upgrade git+https://github.com/tomerfiliba-org/reedsolomon
 
-If you have some issues installing through pip, maybe this command may help:
+If you have some issues installing through pip, maybe this command may help, by forcing the use of sdist instead of wheels:
 
 .. code:: sh
 
-    pip install reedsolo --no-binary={reedsolo}
+    pip install reedsolo --no-binary="reedsolo" --no-cache
 
 Note: for Python 2.7 and Python <= 3.6, please use v1.7.0:
 
 .. code:: sh
 
     pip install --upgrade reedsolo==1.7.0
 
 Through wheels/pip, a pure-python implementation called ``reedsolo`` is installed, and for platforms supported by ``cibuildwheel``, a precompiled speed-optimized ``creedsolo`` module is included. For other platforms or to compile from source (this requires ``cython>=3.0.0b2`` and a C compiler), a build option can be specified:
 
 .. code:: sh
 
     # To compile from the latest stable release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
     # To compile from the latest development release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
     # To compile from the cutting edge code:
-    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
+    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
 
-The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension.
+The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension. The ``--no-binary "reedsolo"`` and ``--no-cache`` options are necessary `since pip 23.1 <https://github.com/pypa/pip/issues/11453#issuecomment-1523964029>`__ to force the use of the sdist instead of wheels.
     
 or locally with:
 
 .. code:: sh
 
     pip install --upgrade . --config-setting="--build-option=--cythonize" --verbose
 
@@ -172,15 +174,15 @@
 
     pip install build
     # With cythonization (from *.pyx to *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--cythonize"
     # or skip cythonization and only compile from the already transpiled c extension (from *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--native-compile"
 
-The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
+The ``setup.py`` will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as ``import creedsolo`` instead of ``import reedsolo``, with the same features between both modules. Note: Make sure to use ``--config-setting`` singular, because ``build`` does not (`yet <https://github.com/pypa/build/issues/608>`__) recognize the plural form contrary to ``pip``.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
 
     conda install -c conda-forge reedsolo
 
@@ -395,15 +397,15 @@
 
     >> import cython
     >> cimport cython
     >> cimport creedsolo.creedsolo as crs
 
 Low-level functions allow to construct new APIs on top of this codec, such as
 `an automatic Reed-Solomon decoder <https://github.com/lrq3000/pyFileFixity/blob/0b18728608f2bceac9eafe5356e0abc573af2768/pyFileFixity/lib/eccman.py#L63>`_
-that can search for any viable set of codec parameters if they are apriori unknown.
+that can search for viable parameters to decode from an unknown Reed-Solomon codec.
 
 If you want to learn more about which internal functions to use and for what purposes,
 read the sourcecode's comments (we follow literate programming principles)
 for more info about how it works and the various parameters
 you can setup if you need to interface with other RS codecs.
 
 Extended description
@@ -543,14 +545,21 @@
 Recommended reading
 -------------------
 
 * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
 * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
 * If you want a more mathematically transparent but less optimized implementation, read the sibling open-source project `unireedsolomon <https://github.com/lrq3000/unireedsolomon>`_, also co-authored by the maintainer of reedsolo, so that the codebase is very similar (although reedsolo is more mature and has more bugfixes - unireedsolomon should only be used for learning purposes!).
 
+Similar projects
+----------------
+
+Here is a non-exhaustive list of similar projects (ie, projects implementing a Reed-Solomon codec):
+* `galois <https://github.com/mhostetter/galois>`_, a Numba JIT-optimized extension module for Numpy, which implements a Reed-Solomon codec and NTT transforms.
+* `generalizedReedSolomon <https://github.com/raeudigerRaeffi/generalizedReedSolomon>`__, a variant of an implementation of Reed-Solomon that is more parallelizable and interestingly can encode messages of arbitrary length without chunking (the chunking is kind of integrated in the parallelization). Internally uses numpy’s fft and ifft. Maybe translatable to use `Number Theoretic Transform (NTT) <https://github.com/Bulat-Ziganshin/FastECC>`__ instead of FFT.
+
 Authors
 -------
 
 This module was conceived and developed by Tomer Filiba in 2012.
 
 It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
```

### Comparing `reedsolo-2.1.0b1/README.rst` & `reedsolo-2.1.1b1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,38 +37,38 @@
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 .. code:: sh
 
     pip install --upgrade git+https://github.com/tomerfiliba-org/reedsolomon
 
-If you have some issues installing through pip, maybe this command may help:
+If you have some issues installing through pip, maybe this command may help, by forcing the use of sdist instead of wheels:
 
 .. code:: sh
 
-    pip install reedsolo --no-binary={reedsolo}
+    pip install reedsolo --no-binary="reedsolo" --no-cache
 
 Note: for Python 2.7 and Python <= 3.6, please use v1.7.0:
 
 .. code:: sh
 
     pip install --upgrade reedsolo==1.7.0
 
 Through wheels/pip, a pure-python implementation called ``reedsolo`` is installed, and for platforms supported by ``cibuildwheel``, a precompiled speed-optimized ``creedsolo`` module is included. For other platforms or to compile from source (this requires ``cython>=3.0.0b2`` and a C compiler), a build option can be specified:
 
 .. code:: sh
 
     # To compile from the latest stable release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
     # To compile from the latest development release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
     # To compile from the cutting edge code:
-    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
+    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
 
-The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension.
+The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension. The ``--no-binary "reedsolo"`` and ``--no-cache`` options are necessary `since pip 23.1 <https://github.com/pypa/pip/issues/11453#issuecomment-1523964029>`__ to force the use of the sdist instead of wheels.
     
 or locally with:
 
 .. code:: sh
 
     pip install --upgrade . --config-setting="--build-option=--cythonize" --verbose
 
@@ -81,15 +81,15 @@
 
     pip install build
     # With cythonization (from *.pyx to *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--cythonize"
     # or skip cythonization and only compile from the already transpiled c extension (from *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--native-compile"
 
-The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
+The ``setup.py`` will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as ``import creedsolo`` instead of ``import reedsolo``, with the same features between both modules. Note: Make sure to use ``--config-setting`` singular, because ``build`` does not (`yet <https://github.com/pypa/build/issues/608>`__) recognize the plural form contrary to ``pip``.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
 
     conda install -c conda-forge reedsolo
 
@@ -304,15 +304,15 @@
 
     >> import cython
     >> cimport cython
     >> cimport creedsolo.creedsolo as crs
 
 Low-level functions allow to construct new APIs on top of this codec, such as
 `an automatic Reed-Solomon decoder <https://github.com/lrq3000/pyFileFixity/blob/0b18728608f2bceac9eafe5356e0abc573af2768/pyFileFixity/lib/eccman.py#L63>`_
-that can search for any viable set of codec parameters if they are apriori unknown.
+that can search for viable parameters to decode from an unknown Reed-Solomon codec.
 
 If you want to learn more about which internal functions to use and for what purposes,
 read the sourcecode's comments (we follow literate programming principles)
 for more info about how it works and the various parameters
 you can setup if you need to interface with other RS codecs.
 
 Extended description
@@ -452,14 +452,21 @@
 Recommended reading
 -------------------
 
 * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
 * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
 * If you want a more mathematically transparent but less optimized implementation, read the sibling open-source project `unireedsolomon <https://github.com/lrq3000/unireedsolomon>`_, also co-authored by the maintainer of reedsolo, so that the codebase is very similar (although reedsolo is more mature and has more bugfixes - unireedsolomon should only be used for learning purposes!).
 
+Similar projects
+----------------
+
+Here is a non-exhaustive list of similar projects (ie, projects implementing a Reed-Solomon codec):
+* `galois <https://github.com/mhostetter/galois>`_, a Numba JIT-optimized extension module for Numpy, which implements a Reed-Solomon codec and NTT transforms.
+* `generalizedReedSolomon <https://github.com/raeudigerRaeffi/generalizedReedSolomon>`__, a variant of an implementation of Reed-Solomon that is more parallelizable and interestingly can encode messages of arbitrary length without chunking (the chunking is kind of integrated in the parallelization). Internally uses numpy’s fft and ifft. Maybe translatable to use `Number Theoretic Transform (NTT) <https://github.com/Bulat-Ziganshin/FastECC>`__ instead of FFT.
+
 Authors
 -------
 
 This module was conceived and developed by Tomer Filiba in 2012.
 
 It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
```

### Comparing `reedsolo-2.1.0b1/pyproject.toml` & `reedsolo-2.1.1b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 # SPDX-License-Identifier: Unlicense OR MIT-0
 # Inspired by: https://hynek.me/articles/python-recursive-optional-dependencies/
-# We here use a single-module distribution style https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#single-module-distribution
+# We here use a src-layout distribution style https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
 
 [build-system]
 # never uppercap requirements unless we have evidence it won't work https://iscinumpy.dev/post/bound-version-constraints/ 
 # cython cannot be placed in optional-dependencies, Cython won't be able to do its magic to make it importable in setup.py
 requires = ["setuptools>59", "cython>=3.0.0b2"]
 build-backend = "setuptools.build_meta"
 
 [project]  # beware if using setuptools: setup.py still gets executed, and even if pyproject.toml fields take precedence, if there is any code error in setup.py, building will fail!
 name = "reedsolo"
-version = "2.1.0b1"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases
+version = "2.1.1b1"  # see PEP 440 https://peps.python.org/pep-0440/#pre-releases
 description = "Pythonic universal errors-and-erasures Reed-Solomon codec to protect your data from errors and bitrot, with a future-proof zero-dependencies pure-python implementation and an optional speed-optimized Cython/C extension."
 authors = [
     {name = "Tomer Filiba", email = "tomerfiliba@gmail.com"},
     {name = "Stephen Karl Larroque", email = "lrq3000@gmail.com"},
     ]
 maintainers = [
     {name = "Stephen Karl Larroque", email = "lrq3000@gmail.com"},
     ]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["data", "protection", "correction", "recovery", "restore", "save", "data-recovery", "reed-solomon", "error-correction-code", "qr", "qr-codes", "barcodes"]
 classifiers = [
     "Development Status :: 6 - Mature",
     "Intended Audience :: Developers",
+    "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: The Unlicense (Unlicense)",  # Unlicense OR MIT-0 at the user preference
     "License :: OSI Approved :: MIT No Attribution License (MIT-0)",
-    'Operating System :: Microsoft :: Windows',
-    'Operating System :: MacOS :: MacOS X',
-    'Operating System :: POSIX :: Linux',
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: MicroPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Cython",
     "Topic :: Communications",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving",
     "Topic :: System :: Archiving :: Backup",
     "Topic :: System :: Recovery Tools",
     "Topic :: Utilities",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: System Administrators",
 ]
 dependencies = [
     #"typing-extensions; python_version<'3.8'",
     #"importlib_metadata;python_version<'3.8'",
 ]
 
 [project.urls]
```

### Comparing `reedsolo-2.1.0b1/setup.py` & `reedsolo-2.1.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 # Authors:
 # Tomer Filiba
 # Stephen Larroque
 # Rotorgit
 # Angus Gratton
 #
 # Licensed under the Unlicense or MIT-0 License at your convenience (essentially equivalent to Public Domain).
+#
+# Purpose: Most of the packaging is done in pyproject.toml, but to compile Cythonized and C extensions with setuptools, a setup.py file is still required.
+# Note: Even if setuptools implement in the future a declarative form for cythonized and C extensions, an empty setup.py is required for retrocompatibility with older versions of pip that do not support pyproject.toml-only projects, especially to install in editable mode, see: https://github.com/pypa/setuptools/issues/2816
+
 
 # See:
 # https://docs.python.org/2/distutils/setupscript.html
 # http://docs.cython.org/src/reference/compilation.html
 # https://docs.python.org/2/extending/building.html
 # http://docs.cython.org/src/userguide/source_files_and_compilation.html
```

### Comparing `reedsolo-2.1.0b1/src/creedsolo/creedsolo.c` & `reedsolo-2.1.1b1/src/creedsolo/creedsolo.c`

 * *Files identical despite different names*

### Comparing `reedsolo-2.1.0b1/src/creedsolo/creedsolo.pyx` & `reedsolo-2.1.1b1/src/creedsolo/creedsolo.pyx`

 * *Files identical despite different names*

### Comparing `reedsolo-2.1.0b1/src/reedsolo/reedsolo.py` & `reedsolo-2.1.1b1/src/reedsolo/reedsolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,18 @@
     # Recopy the original message bytes (overwrites the part where the quotient was computed)
     msg_out[:msg_in_len] = msg_in # equivalent to c = mprime - b, where mprime is msg_in padded with [0]*nsym
     return msg_out
 
 
 ################### REED-SOLOMON DECODING ###################
 
+def inverted(msg):
+    '''Implements msg[::-1] explicitly to make the library compatible with MicroPython which does not support stepped slices.'''
+    return list(reversed(msg))
+
 def rs_calc_syndromes(msg, nsym, fcr=0, generator=2):
     '''Given the received codeword msg and the number of error correcting symbols (nsym), computes the syndromes polynomial.
     Mathematically, it's essentially equivalent to a Fourrier Transform (Chien search being the inverse).
     '''
     # Note the "[0] +" : we add a 0 coefficient for the lowest degree (the constant). This effectively shifts the syndrome, and will shift every computations depending on the syndromes (such as the errors locator polynomial, errors evaluator polynomial, etc. but not the errors positions).
     # This is not necessary as anyway syndromes are defined such as there are only non-zero coefficients (the only 0 is the shift of the constant here) and subsequent computations will/must account for the shift by skipping the first iteration (eg, the often seen range(1, n-k+1)), but you can also avoid prepending the 0 coeff and adapt every subsequent computations to start from 0 instead of 1.
     return [0] + [gf_poly_eval(msg, gf_pow(generator, i+fcr)) for i in xrange(nsym)]
@@ -573,15 +577,15 @@
     '''Forney algorithm, computes the values (error magnitude) to correct the input message.'''
     global field_charac
     msg = _bytearray(msg_in)
     # calculate errata locator polynomial to correct both errors and erasures (by combining the errors positions given by the error locator polynomial found by BM with the erasures positions given by caller)
     coef_pos = [len(msg) - 1 - p for p in err_pos] # need to convert the positions to coefficients degrees for the errata locator algo to work (eg: instead of [0, 1, 2] it will become [len(msg)-1, len(msg)-2, len(msg) -3])
     err_loc = rs_find_errata_locator(coef_pos, generator)
     # calculate errata evaluator polynomial (often called Omega or Gamma in academic papers)
-    err_eval = rs_find_error_evaluator(synd[::-1], err_loc, len(err_loc)-1)[::-1]
+    err_eval = inverted(rs_find_error_evaluator(inverted(synd), err_loc, len(err_loc)-1))
 
     # Second part of Chien search to get the error location polynomial X from the error positions in err_pos (the roots of the error locator polynomial, ie, where it evaluates to 0)
     X = _bytearray(len(coef_pos)) # will store the position of the errors
     for i in xrange(len(coef_pos)):
         l = field_charac - coef_pos[i]
         X[i] = gf_pow(generator, -l)
 
@@ -613,15 +617,15 @@
         # Test if we could find the errata locator, else we raise an Exception (because else since we divide y by err_loc_prime to compute the magnitude, we will get a ZeroDivisionError exception otherwise)
         if err_loc_prime == 0:
             raise ReedSolomonError("Decoding failed: Forney algorithm could not properly detect where the errors are located (errata locator prime is 0).")
 
         # Compute y (evaluation of the errata evaluator polynomial)
         # This is a more faithful translation of the theoretical equation contrary to the old forney method. Here it is exactly copy/pasted from the included presentation decoding_rs.pdf: Yl = omega(Xl.inverse()) / prod(1 - Xj*Xl.inverse()) for j in len(X) (in the paper it's for j in s, but it's useless when len(X) < s because we compute neutral terms 1 for nothing, and wrong when correcting more than s erasures or erasures+errors since it prevents computing all required terms).
         # Thus here this method works with erasures too because firstly we fixed the equation to be like the theoretical one (don't know why it was modified in _old_forney(), if it's an optimization, it doesn't enhance anything), and secondly because we removed the product bound on s, which prevented computing errors and erasures above the s=(n-k)//2 bound.
-        y = gf_poly_eval(err_eval[::-1], Xi_inv) # numerator of the Forney algorithm (errata evaluator evaluated)
+        y = gf_poly_eval(inverted(err_eval), Xi_inv) # numerator of the Forney algorithm (errata evaluator evaluated)
         y = gf_mul(gf_pow(Xi, 1-fcr), y) # adjust to fcr parameter
         
         # Compute the magnitude
         magnitude = gf_div(y, err_loc_prime) # magnitude value of the error, calculated by the Forney algorithm (an equation in fact): dividing the errata evaluator with the errata locator derivative gives us the errata magnitude (ie, value to repair) the ith symbol
         E[err_pos[i]] = magnitude # store the magnitude for this error into the magnitude polynomial
 
     # Apply the correction of values to get our message corrected! (note that the ecc bytes also gets corrected!)
@@ -653,21 +657,21 @@
         if erase_loc: # if an erasures locator polynomial was provided to init the errors locator polynomial, then we must skip the FIRST erase_count iterations (not the last iterations, this is very important!)
             K = erase_count+i+synd_shift
         else: # if erasures locator is not provided, then either there's no erasures to account or we use the Forney syndromes, so we don't need to use erase_count nor erase_loc (the erasures have been trimmed out of the Forney syndromes).
             K = i+synd_shift
 
         # Compute the discrepancy Delta
         # Here is the close-to-the-books operation to compute the discrepancy Delta: it's a simple polynomial multiplication of error locator with the syndromes, and then we get the Kth element.
-        #delta = gf_poly_mul(err_loc[::-1], synd)[K] # theoretically it should be gf_poly_add(synd[::-1], [1])[::-1] instead of just synd, but it seems it's not absolutely necessary to correctly decode.
+        #delta = gf_poly_mul(inverted(err_loc), synd)[K] # theoretically it should be inverted(gf_poly_add(inverted(synd), [1])) instead of just synd, but it seems it's not absolutely necessary to correctly decode.
         # But this can be optimized: since we only need the Kth element, we don't need to compute the polynomial multiplication for any other element but the Kth. Thus to optimize, we compute the polymul only at the item we need, skipping the rest (avoiding a nested loop, thus we are linear time instead of quadratic).
         # This optimization is actually described in several figures of the book "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press.
         delta = synd[K]
         for j in xrange(1, len(err_loc)):  # range 1:256 is important: if you use range 0:255, if the last byte of the ecc symbols is corrupted, it won't be correctable! You need to use the range 1,256 to include this last byte.
             delta ^= gf_mul(err_loc[-(j+1)], synd[K - j]) # delta is also called discrepancy. Here we do a partial polynomial multiplication (ie, we compute the polynomial multiplication only for the term of degree K). Should be equivalent to brownanrs.polynomial.mul_at().
-        #print "delta", K, delta, list(gf_poly_mul(err_loc[::-1], synd)) # debugline
+        #print "delta", K, delta, list(gf_poly_mul(inverted(err_loc), synd)) # debugline
 
         # Shift polynomials to compute the next degree
         old_loc = old_loc + _bytearray([0])
 
         # Iteratively estimate the errata locator and evaluator polynomials
         if delta != 0: # Update only if there's a discrepancy
             if len(old_loc) > len(err_loc): # Rule B (rule A is implicitly defined because rule A just says that we skip any modification for this iteration)
@@ -739,15 +743,15 @@
         for j in xrange(len(fsynd) - 1):
             fsynd[j] = gf_mul(fsynd[j], x) ^ fsynd[j + 1]
         #fsynd.pop() # useless? it doesn't change the results of computations to leave it there
 
     # Theoretical way of computing the modified Forney syndromes: fsynd = (erase_loc * synd) % x^(n-k) -- although the trimming by using x^(n-k) is maybe not necessary as many books do not even mention it (and it works without trimming)
     # See Shao, H. M., Truong, T. K., Deutsch, L. J., & Reed, I. S. (1986, April). A single chip VLSI Reed-Solomon decoder. In Acoustics, Speech, and Signal Processing, IEEE International Conference on ICASSP'86. (Vol. 11, pp. 2151-2154). IEEE.ISO 690
     #erase_loc = rs_find_errata_locator(erase_pos_reversed, generator=generator) # computing the erasures locator polynomial
-    #fsynd = gf_poly_mul(erase_loc[::-1], synd[1:]) # then multiply with the syndrome to get the untrimmed forney syndrome
+    #fsynd = gf_poly_mul(inverted(erase_loc), synd[1:]) # then multiply with the syndrome to get the untrimmed forney syndrome
     #fsynd = fsynd[len(pos):] # then trim the first erase_pos coefficients which are useless. Seems to be not necessary, but this reduces the computation time later in BM (thus it's an optimization).
 
     return fsynd
 
 def rs_correct_msg(msg_in, nsym, fcr=0, generator=2, erase_pos=None, only_erasures=False):
     '''Reed-Solomon main decoding function'''
     global field_charac
@@ -777,15 +781,15 @@
         err_pos = _bytearray()
     else:
         # compute the Forney syndromes, which hide the erasures from the original syndrome (so that BM will just have to deal with errors, not erasures)
         fsynd = rs_forney_syndromes(synd, erase_pos, len(msg_out), generator)
         # compute the error locator polynomial using Berlekamp-Massey
         err_loc = rs_find_error_locator(fsynd, nsym, erase_count=len(erase_pos))
         # locate the message errors using Chien search (or bruteforce search)
-        err_pos = rs_find_errors(err_loc[::-1], len(msg_out), generator)
+        err_pos = rs_find_errors(inverted(err_loc), len(msg_out), generator)
         if err_pos is None:
             raise ReedSolomonError("Could not locate error")
 
     # Find errors values and apply them to correct the message
     # compute errata evaluator and errata magnitude polynomials, then correct errors and erasures
     msg_out = rs_correct_errata(msg_out, synd, erase_pos + err_pos, fcr, generator) # note that we here use the original syndrome, not the forney syndrome (because we will correct both errors and erasures, so we need the full syndrome)
     # check if the final message is fully repaired
@@ -823,24 +827,24 @@
     #erase_eval = None
     erase_count = 0
     if erase_pos:
         erase_count = len(erase_pos)
         msg_out_len = len(msg_out)  # cache to avoid recalculations inside loop
         erase_pos_reversed = [msg_out_len-1-eras for eras in erase_pos]
         erase_loc = rs_find_errata_locator(erase_pos_reversed, generator=generator)
-        #erase_eval = rs_find_error_evaluator(synd[::-1], erase_loc, len(erase_loc)-1)
+        #erase_eval = rs_find_error_evaluator(inverted(synd), erase_loc, len(erase_loc)-1)
 
     # prepare errors/errata locator polynomial
     if only_erasures:
-        err_loc = erase_loc[::-1]
-        #err_eval = erase_eval[::-1]
+        err_loc = inverted(erase_loc)
+        #err_eval = inverted(erase_eval)
     else:
         err_loc = rs_find_error_locator(synd, nsym, erase_loc=erase_loc, erase_count=erase_count)
-        err_loc = err_loc[::-1]
-        #err_eval = rs_find_error_evaluator(synd[::-1], err_loc[::-1], len(err_loc)-1)[::-1] # find error/errata evaluator polynomial (not really necessary since we already compute it at the same time as the error locator poly in BM)
+        err_loc = inverted(err_loc)
+        #err_eval = inverted(rs_find_error_evaluator(inverted(synd), inverted(err_loc), len(err_loc)-1)) # find error/errata evaluator polynomial (not really necessary since we already compute it at the same time as the error locator poly in BM)
 
     # locate the message errors
     err_pos = rs_find_errors(err_loc, len(msg_out), generator) # find the roots of the errata locator polynomial (ie: the positions of the errors/errata)
     if err_pos is None:
         raise ReedSolomonError("Could not locate error")
 
     # compute errata evaluator and errata magnitude polynomials, then correct errors and erasures
```

### Comparing `reedsolo-2.1.0b1/src/reedsolo.egg-info/PKG-INFO` & `reedsolo-2.1.1b1/src/reedsolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reedsolo
-Version: 2.1.0b1
+Version: 2.1.1b1
 Summary: Pythonic universal errors-and-erasures Reed-Solomon codec to protect your data from errors and bitrot, with a future-proof zero-dependencies pure-python implementation and an optional speed-optimized Cython/C extension.
 Author-email: Tomer Filiba <tomerfiliba@gmail.com>, Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: The software is available under your choice of
         Unlicense (SPDX short identifier: Unlicense) or
         MIT No Attribution License (SPDX short identifier: MIT-0):
         
@@ -52,40 +52,42 @@
 Project-URL: Source, https://github.com/tomerfiliba-org/reedsolomon
 Project-URL: Tracker, https://github.com/tomerfiliba-org/reedsolomon/issues
 Project-URL: Download, https://github.com/tomerfiliba-org/reedsolomon/releases
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/reedsolo
 Keywords: data,protection,correction,recovery,restore,save,data-recovery,reed-solomon,error-correction-code,qr,qr-codes,barcodes
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Communications
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: testmeta
 Provides-Extra: testoptional
 License-File: LICENSE
 
@@ -128,38 +130,38 @@
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 .. code:: sh
 
     pip install --upgrade git+https://github.com/tomerfiliba-org/reedsolomon
 
-If you have some issues installing through pip, maybe this command may help:
+If you have some issues installing through pip, maybe this command may help, by forcing the use of sdist instead of wheels:
 
 .. code:: sh
 
-    pip install reedsolo --no-binary={reedsolo}
+    pip install reedsolo --no-binary="reedsolo" --no-cache
 
 Note: for Python 2.7 and Python <= 3.6, please use v1.7.0:
 
 .. code:: sh
 
     pip install --upgrade reedsolo==1.7.0
 
 Through wheels/pip, a pure-python implementation called ``reedsolo`` is installed, and for platforms supported by ``cibuildwheel``, a precompiled speed-optimized ``creedsolo`` module is included. For other platforms or to compile from source (this requires ``cython>=3.0.0b2`` and a C compiler), a build option can be specified:
 
 .. code:: sh
 
     # To compile from the latest stable release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
     # To compile from the latest development release:
-    pip install --upgrade reedsolo --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
+    pip install --upgrade reedsolo --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
     # To compile from the cutting edge code:
-    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --config-setting="--build-option=--cythonize" --use-pep517 --isolated --verbose
+    pip install --upgrade "reedsolo @ git+https://github.com/tomerfiliba-org/reedsolomon" --no-binary "reedsolo" --no-cache --config-setting="--build-option=--cythonize" --use-pep517 --isolated --pre --verbose
 
-The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension.
+The ``--config-setting="--build-option=--cythonize"`` flag signals to the ``setuptools`` backend to propagate to ``reedsolo's setup.py`` to build the optional cythonized extension. The ``--no-binary "reedsolo"`` and ``--no-cache`` options are necessary `since pip 23.1 <https://github.com/pypa/pip/issues/11453#issuecomment-1523964029>`__ to force the use of the sdist instead of wheels.
     
 or locally with:
 
 .. code:: sh
 
     pip install --upgrade . --config-setting="--build-option=--cythonize" --verbose
 
@@ -172,15 +174,15 @@
 
     pip install build
     # With cythonization (from *.pyx to *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--cythonize"
     # or skip cythonization and only compile from the already transpiled c extension (from *.c to *.pyd)
     python -sBm build --config-setting="--build-option=--native-compile"
 
-The setup.py will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as `import creedsolo` instead of `import reedsolo`, with the same features between both modules.
+The ``setup.py`` will then try to build the Cython optimized module ``creedsolo.pyx`` if Cython is installed, which can then be imported as ``import creedsolo`` instead of ``import reedsolo``, with the same features between both modules. Note: Make sure to use ``--config-setting`` singular, because ``build`` does not (`yet <https://github.com/pypa/build/issues/608>`__) recognize the plural form contrary to ``pip``.
 
 As an alternative, use `conda <https://docs.conda.io/en/latest/>`_ to install a compiled version for various platforms:
 
 .. code:: sh
 
     conda install -c conda-forge reedsolo
 
@@ -395,15 +397,15 @@
 
     >> import cython
     >> cimport cython
     >> cimport creedsolo.creedsolo as crs
 
 Low-level functions allow to construct new APIs on top of this codec, such as
 `an automatic Reed-Solomon decoder <https://github.com/lrq3000/pyFileFixity/blob/0b18728608f2bceac9eafe5356e0abc573af2768/pyFileFixity/lib/eccman.py#L63>`_
-that can search for any viable set of codec parameters if they are apriori unknown.
+that can search for viable parameters to decode from an unknown Reed-Solomon codec.
 
 If you want to learn more about which internal functions to use and for what purposes,
 read the sourcecode's comments (we follow literate programming principles)
 for more info about how it works and the various parameters
 you can setup if you need to interface with other RS codecs.
 
 Extended description
@@ -543,14 +545,21 @@
 Recommended reading
 -------------------
 
 * "`Reed-Solomon codes for coders <https://en.wikiversity.org/wiki/Reed%E2%80%93Solomon_codes_for_coders>`_", free practical beginner's tutorial with Python code examples on WikiVersity. Partially written by one of the authors of the present software.
 * "Algebraic codes for data transmission", Blahut, Richard E., 2003, Cambridge university press. `Readable online on Google Books <https://books.google.fr/books?id=eQs2i-R9-oYC&lpg=PR11&ots=atCPQJm3OJ&dq=%22Algebraic%20codes%20for%20data%20transmission%22%2C%20Blahut%2C%20Richard%20E.%2C%202003%2C%20Cambridge%20university%20press.&lr&hl=fr&pg=PA193#v=onepage&q=%22Algebraic%20codes%20for%20data%20transmission%22,%20Blahut,%20Richard%20E.,%202003,%20Cambridge%20university%20press.&f=false>`_. This book was pivotal in helping to understand the intricacies of the universal Berlekamp-Massey algorithm (see figures 7.5 and 7.10).
 * If you want a more mathematically transparent but less optimized implementation, read the sibling open-source project `unireedsolomon <https://github.com/lrq3000/unireedsolomon>`_, also co-authored by the maintainer of reedsolo, so that the codebase is very similar (although reedsolo is more mature and has more bugfixes - unireedsolomon should only be used for learning purposes!).
 
+Similar projects
+----------------
+
+Here is a non-exhaustive list of similar projects (ie, projects implementing a Reed-Solomon codec):
+* `galois <https://github.com/mhostetter/galois>`_, a Numba JIT-optimized extension module for Numpy, which implements a Reed-Solomon codec and NTT transforms.
+* `generalizedReedSolomon <https://github.com/raeudigerRaeffi/generalizedReedSolomon>`__, a variant of an implementation of Reed-Solomon that is more parallelizable and interestingly can encode messages of arbitrary length without chunking (the chunking is kind of integrated in the parallelization). Internally uses numpy’s fft and ifft. Maybe translatable to use `Number Theoretic Transform (NTT) <https://github.com/Bulat-Ziganshin/FastECC>`__ instead of FFT.
+
 Authors
 -------
 
 This module was conceived and developed by Tomer Filiba in 2012.
 
 It was further extended and is currently maintained by Stephen Karl Larroque since 2015.
```

### Comparing `reedsolo-2.1.0b1/tests/test_creedsolo.py` & `reedsolo-2.1.1b1/tests/test_creedsolo.py`

 * *Files identical despite different names*

### Comparing `reedsolo-2.1.0b1/tests/test_reedsolo.py` & `reedsolo-2.1.1b1/tests/test_reedsolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,10 +551,15 @@
         rs = RSCodec(10)
         rs.maxerrata(verbose=True)
         rs.maxerrata(erasures=2, verbose=True)
         rs.maxerrata(errors=4, verbose=True)
         sys.stdout = sys.__stdout__
         self.assertEqual(output.getvalue(), "This codec can correct up to 5 errors and 10 erasures independently\nThis codec can correct up to 4 errors and 2 erasures simultaneously\nThis codec can correct up to 4 errors and 2 erasures simultaneously\n")
 
+    def test_inverted(self):
+        '''Only for other envs than MicroPython: test if inverted() == inverted stepped slicing'''
+        l = [1, 2, 3, 2, 4]
+        self.assertTrue(inverted(l) == l[::-1])
+
 
 if __name__ == "__main__":
     unittest.main()
```

