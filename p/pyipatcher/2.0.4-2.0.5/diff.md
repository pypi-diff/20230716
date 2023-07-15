# Comparing `tmp/pyipatcher-2.0.4.tar.gz` & `tmp/pyipatcher-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipatcher-2.0.4.tar", max compression
+gzip compressed data, was "pyipatcher-2.0.5.tar", max compression
```

## Comparing `pyipatcher-2.0.4.tar` & `pyipatcher-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-2.0.4/LICENSE
--rw-r--r--   0        0        0     1029 2023-06-10 14:08:14.786228 pyipatcher-2.0.4/README.md
--rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-2.0.4/pyipatcher/__init__.py
--rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-2.0.4/pyipatcher/__main__.py
--rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-2.0.4/pyipatcher/cli/ibootpatcher.py
--rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-2.0.4/pyipatcher/cli/kernelpatcher.py
--rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-2.0.4/pyipatcher/cli/ramdiskpatcher.py
--rw-r--r--   0        0        0     9635 2023-07-14 16:58:28.682318 pyipatcher-2.0.4/pyipatcher/ipatcher.py
--rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-2.0.4/pyipatcher/logger.py
--rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-2.0.4/pyipatcher/patchfinder/asrpatchfinder.py
--rw-r--r--   0        0        0    24222 2023-07-15 00:18:44.840815 pyipatcher-2.0.4/pyipatcher/patchfinder/ibootpatchfinder.py
--rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-2.0.4/pyipatcher/patchfinder/insn.py
--rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-2.0.4/pyipatcher/patchfinder/kernelpatchfinder.py
--rw-r--r--   0        0        0     5818 2023-07-15 00:13:09.129788 pyipatcher-2.0.4/pyipatcher/patchfinder/patchfinder64.py
--rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-2.0.4/pyipatcher/patchfinder/rextpatchfinder.py
--rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-2.0.4/pyipatcher/wikiproxy.py
--rw-r--r--   0        0        0      927 2023-07-14 18:59:59.472364 pyipatcher-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 pyipatcher-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-2.0.5/LICENSE
+-rw-r--r--   0        0        0     1029 2023-06-10 14:08:14.786228 pyipatcher-2.0.5/README.md
+-rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-2.0.5/pyipatcher/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-2.0.5/pyipatcher/__main__.py
+-rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-2.0.5/pyipatcher/cli/ibootpatcher.py
+-rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-2.0.5/pyipatcher/cli/kernelpatcher.py
+-rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-2.0.5/pyipatcher/cli/ramdiskpatcher.py
+-rw-r--r--   0        0        0     9635 2023-07-14 16:58:28.682318 pyipatcher-2.0.5/pyipatcher/ipatcher.py
+-rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-2.0.5/pyipatcher/logger.py
+-rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-2.0.5/pyipatcher/patchfinder/asrpatchfinder.py
+-rw-r--r--   0        0        0    24635 2023-07-15 23:34:31.900298 pyipatcher-2.0.5/pyipatcher/patchfinder/ibootpatchfinder.py
+-rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-2.0.5/pyipatcher/patchfinder/insn.py
+-rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-2.0.5/pyipatcher/patchfinder/kernelpatchfinder.py
+-rw-r--r--   0        0        0     5818 2023-07-15 00:13:09.129788 pyipatcher-2.0.5/pyipatcher/patchfinder/patchfinder64.py
+-rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-2.0.5/pyipatcher/patchfinder/rextpatchfinder.py
+-rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-2.0.5/pyipatcher/wikiproxy.py
+-rw-r--r--   0        0        0      927 2023-07-15 23:18:12.692065 pyipatcher-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 pyipatcher-2.0.5/PKG-INFO
```

### Comparing `pyipatcher-2.0.4/LICENSE` & `pyipatcher-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/README.md` & `pyipatcher-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/cli/ibootpatcher.py` & `pyipatcher-2.0.5/pyipatcher/cli/ibootpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/cli/kernelpatcher.py` & `pyipatcher-2.0.5/pyipatcher/cli/kernelpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/cli/ramdiskpatcher.py` & `pyipatcher-2.0.5/pyipatcher/cli/ramdiskpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/ipatcher.py` & `pyipatcher-2.0.5/pyipatcher/ipatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/logger.py` & `pyipatcher-2.0.5/pyipatcher/logger.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/asrpatchfinder.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/asrpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/ibootpatchfinder.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/ibootpatchfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,28 +97,38 @@
             return -1
         logger.debug(f'cmd_ref={hex(cmd_ref + self.base)}')
         self.apply_patch(cmd_ref+8, ptr.to_bytes(8, byteorder='little'))
         return 0
         
     def get_unlock_nvram_patch(self):
         logger = get_my_logger(self.verbose)
+        # check stage first
+        if self.stage1:
+            logger.debug('iBootStage1/iBSS detected, not patching nvram')
+            return 0
+        logger.debug('Not iBootStage1/iBSS, continuing')
         debuguart_loc = self.memmem(b'debug-uarts')
         if debuguart_loc == -1:
             logger.error('Could not find debug-uarts string')
             return -1
         logger.debug(f'debuguart_loc={hex(debuguart_loc + self.base)}')
         debuguart_ref = self.iboot_memmem(debuguart_loc)
         logger.debug(f'debuguart_ref={hex(debuguart_ref + self.base)}')
         setenv_whitelist = debuguart_ref
-        try:
-            while self.get_ptr_loc(setenv_whitelist):
-                setenv_whitelist -= 8
-        except:
-            pass
-        setenv_whitelist += 8
+        if self.cpid in (7001, 8000, 8003):
+            logger.debug('a8x/a9')
+            setenv_whitelist -= 16
+        else:
+            logger.debug('not a8x/a9')
+            try:
+                while self.get_ptr_loc(setenv_whitelist):
+                    setenv_whitelist -= 8
+            except:
+                pass
+            setenv_whitelist += 8
         logger.debug(f'setenv_whitelist={hex(setenv_whitelist + self.base)}')
         blacklistfunc = self.xref(setenv_whitelist)
         if blacklistfunc == 0:
             logger.error('Could not find setenv whitelist ref')
             return -1
         logger.debug(f'blacklistfunc={hex(blacklistfunc + self.base)}')
         blacklistfunc_begin = self.bof(blacklistfunc)
@@ -140,23 +150,23 @@
             logger.error('Could not find env whitelist ref')
             return -1
         logger.debug(f'blacklistfunc2={hex(blacklistfunc2 + self.base)}')
         blacklistfunc2_begin = self.bof(blacklistfunc2)
         if blacklistfunc_begin == 0:
             logger.error('Could not find beginning of blacklistfunc2')
             return -1
-        logger.debug(f'blacklistfunc2_begin={hex(blacklistfunc_begin + self.base)}')
+        logger.debug(f'blacklistfunc2_begin={hex(blacklistfunc2_begin + self.base)}')
         self.apply_patch(blacklistfunc2_begin, b'\x00\x00\x80\xd2\xc0\x03_\xd6')
         com_apple_system_loc = self.memmem(b'com.apple.System.\0')
         if com_apple_system_loc == -1:
             logger.error('Could not find com_apple_system_loc')
             return -1
         logger.debug(f'com_apple_system_loc={hex(com_apple_system_loc + self.base)}')
         com_apple_system_ref = self.xref(com_apple_system_loc)
-        logger.debug(f'com_apple_system_ref={hex(com_apple_system_ref)}')
+        logger.debug(f'com_apple_system_ref={hex(com_apple_system_ref + self.base)}')
         com_apple_system_begin = self.bof(com_apple_system_ref)
         if com_apple_system_begin == 0:
             logger.error('Could not find com_apple_system_begin')
             return -1
         logger.debug(f'com_apple_system_begin={hex(com_apple_system_begin + self.base)}')
         self.apply_patch(com_apple_system_begin, b'\x00\x00\x80\xd2\xc0\x03_\xd6')
         return 0
@@ -446,15 +456,15 @@
             logger.error('Could not find noncefun2')
             return -1
         logger.debug(f'noncefun2={hex(noncefun2 + self.base)}')
         noncefun2_blref = self.xrefcode(noncefun2)
         if noncefun2_blref == 0:
             logger.error('Could not find noncefun2_blref')
             return -1
-        logger.debug(f'noncefun2_blref={noncefun2_blref + self.base}')
+        logger.debug(f'noncefun2_blref={hex(noncefun2_blref + self.base)}')
         noncefun2_blref -= 4
         while insn.supertype(insn.get_type(self.get_insn(noncefun2_blref))) != 'sut_branch_imm':
             noncefun2_blref -= 4
         branch_loc = noncefun2_blref
         logger.debug(f'branch_loc={hex(branch_loc + self.base)}')
         self.apply_patch(branch_loc, b'\x1F\x20\x03\xD5')
         return 0
```

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/insn.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/insn.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/kernelpatchfinder.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/kernelpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/patchfinder64.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/patchfinder64.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/patchfinder/rextpatchfinder.py` & `pyipatcher-2.0.5/pyipatcher/patchfinder/rextpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyipatcher/wikiproxy.py` & `pyipatcher-2.0.5/pyipatcher/wikiproxy.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.4/pyproject.toml` & `pyipatcher-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyipatcher"
-version = "2.0.4"
+version = "2.0.5"
 description = "iOS ARM64 patchfinder & iOS ARM64 bootchain patcher"
 authors = ["mini_exploit <61931266+Mini-Exploit@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/Mini-Exploit/pyipatcher"
 
 [tool.poetry.dependencies]
```

### Comparing `pyipatcher-2.0.4/PKG-INFO` & `pyipatcher-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipatcher
-Version: 2.0.4
+Version: 2.0.5
 Summary: iOS ARM64 patchfinder & iOS ARM64 bootchain patcher
 Home-page: https://github.com/Mini-Exploit/pyipatcher
 License: GPL-3.0-only
 Author: mini_exploit
 Author-email: 61931266+Mini-Exploit@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

