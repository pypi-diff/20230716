# Comparing `tmp/bb_dirtree-0.3.2.tar.gz` & `tmp/bb_dirtree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.3.2.tar", max compression
+gzip compressed data, was "bb_dirtree-0.4.0.tar", max compression
```

## Comparing `bb_dirtree-0.3.2.tar` & `bb_dirtree-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.3.2/LICENSE
--rw-r--r--   0        0        0     5082 2023-07-16 00:27:22.950588 bb_dirtree-0.3.2/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.3.2/bbdirtree/COLORS.py
--rw-r--r--   0        0        0      125 2023-07-16 00:26:34.300588 bb_dirtree-0.3.2/bbdirtree/__init__.py
--rw-r--r--   0        0        0    25116 2023-07-16 00:26:18.767254 bb_dirtree-0.3.2/bbdirtree/__main__.py
--rw-r--r--   0        0        0      577 2023-07-16 00:26:35.340587 bb_dirtree-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 bb_dirtree-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5582 2023-07-16 12:00:26.428041 bb_dirtree-0.4.0/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.4.0/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0      125 2023-07-16 10:04:23.941243 bb_dirtree-0.4.0/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    33551 2023-07-16 11:59:35.901374 bb_dirtree-0.4.0/bbdirtree/__main__.py
+-rw-r--r--   0        0        0     2236 2023-07-16 08:24:42.264463 bb_dirtree-0.4.0/bbdirtree/unixvolumeinfo.py
+-rw-r--r--   0        0        0     3528 2023-07-16 03:57:58.694161 bb_dirtree-0.4.0/bbdirtree/winvolumeinfo.py
+-rw-r--r--   0        0        0      577 2023-07-16 10:04:26.731243 bb_dirtree-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 bb_dirtree-0.4.0/PKG-INFO
```

### Comparing `bb_dirtree-0.3.2/LICENSE` & `bb_dirtree-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.2/README.md` & `bb_dirtree-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 
 ```bash
 dirtree [OPTIONS] [ARGS]
 ```
 
 ### _**Options:**_
 
-**Short**  | **Long**               | **Description**
----------- | ---------------------- | ---------------------------------------------------------
-    -b     |   --base-dir           |  Set base directory <br> *Uses current directory if not specified*
-    -d     |   --depth              |  Integer to set the depth of directory tree <br> *ex: '0' will only print the base directory list*
-    -D     |   --dotfiles           |  Include hidden files in tree
-    -e     |   --exclude            |  Filenames/directories to exclude from the tree <br> *See Exclusions*
-    -h     |   --help               |  This help message
-    -I     |   --ignore-errors      |  Ignore read errors (such as permission errors) - Default is to error and exit
-    -l     |   --follow-symlinks    |  Follow links to directories - default is NOT to follow
-    -q     |   --qt-html            |  Print in html format for use with QT
-    -r     |   --regex              |  Use regex to include/exclude files/directories in tree <br> *See Regex*
-    -v     |   --verbose            |  Set verbose level (1-5) or 'debug' = 1
-           |   --no-print           |  Don't print any output
+**Short**  | **Long**           | **Description**
+---------- | ------------------ | ---------------------------------------------------------
+    -b     |   --base-dir       |  Set base directory <br> *Uses current directory if not specified*
+    -d     |   --depth          |  Integer to set the depth of directory tree <br> *ex: '0' will only print the base directory list*
+    -D     |   --dotfiles       |  Include hidden files in tree
+    -e     |   --exclude        |  Filenames/directories to exclude from the tree <br> *See Exclusions*
+    -h     |   --help           |  This help message
+    -L     |   --follow-links   |  Follow links to directories - default is NOT to follow
+    -q     |   --qt-html        |  Print in html format for use with QT
+    -r     |   --regex          |  Use regex to include/exclude files/directories in tree <br> *See Regex*
+    -v     |   --verbose        |  Set verbose level (1-5) or 'debug' = 1
+           |   --ignore-errors  |  Ignore read errors (such as permission errors) - Default is to error and exit
+           |   --no-print       |  Don't print any output
+           |   --version        |  Print version info and exit
 
 >It is recommended to quote all paths
 
 ### *Exclusions*
 
 >Provide names of files or directories to exclude. To exclude multiple files/directories, quote entire list and seperate with a colon (**:**). Add a forward slash (**/**) to specify a directory name to exclude.
 
@@ -167,7 +168,26 @@
 
 #### v0.3.2 - 7-15-2023
 
 - added colorized tree for symlinked directories
 - prevent symlinks from causing infinite recursion
     - colored recursive directory links red
 - moved formatting code to class instances
+
+#### v0.3.4 - 7-15-2023
+
+- fixed hidden file detection in windows
+- added more title methods
+
+#### v0.4.0 - 7-16-2023
+
+- updated bb_appdirs
+- changed some log messages
+- added more title methods
+- added a fancy title header
+- added winvolumeinfo module
+- added unixvolumeinfo module
+- added option to print version info
+- adjusted output for when base directory is a link
+- changed html colors to hex values and adjusted
+- changed tty colors to rgb values
+- changed some option arguments
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
  # DirTree -------------------------------------------- ##### Create a nice
 looking directory tree -------------------------------------------- ##
 Installation: ```bash python -m pip install "BB-DirTree" ``` ## DirTree usage
 ```bash dirtree [OPTIONS] [ARGS] ``` ### _**Options:**_ **Short** | **Long** |
-**Description** ---------- | ---------------------- | -------------------------
--------------------------------- -b | --base-dir | Set base directory
+**Description** ---------- | ------------------ | -----------------------------
+---------------------------- -b | --base-dir | Set base directory
 *Uses current directory if not specified* -d | --depth | Integer to set the
 depth of directory tree
 *ex: '0' will only print the base directory list* -D | --dotfiles | Include
 hidden files in tree -e | --exclude | Filenames/directories to exclude from the
 tree
-*See Exclusions* -h | --help | This help message -I | --ignore-errors | Ignore
-read errors (such as permission errors) - Default is to error and exit -l | --
-follow-symlinks | Follow links to directories - default is NOT to follow -q | -
--qt-html | Print in html format for use with QT -r | --regex | Use regex to
-include/exclude files/directories in tree
-*See Regex* -v | --verbose | Set verbose level (1-5) or 'debug' = 1 | --no-
-print | Don't print any output >It is recommended to quote all paths ###
-*Exclusions* >Provide names of files or directories to exclude. To exclude
-multiple files/directories, quote entire list and seperate with a colon (**:
-**). Add a forward slash (**/**) to specify a directory name to exclude. #####
-**Example:** ```bash dirtree --exclude "excluded dir:excluded file" ``` ###
-*Regex* >Prefix regex with *include=* or *exclude=* >Seperate each regex with a
-space, quoting each individual argument. ##### _**Examples:**_ ```bash dirtree
---regex "exclude=.*\.ini$" # will exclude any files that have a *.ini*
-extension. dirtree --regex "include=.*\.mp3$" # will include only files with a
-*.mp3* extension. ``` >This has no effect on directories >Multiple regex can be
-used by specifying **--regex** multiple times. ## License ==========
+*See Exclusions* -h | --help | This help message -L | --follow-links | Follow
+links to directories - default is NOT to follow -q | --qt-html | Print in html
+format for use with QT -r | --regex | Use regex to include/exclude files/
+directories in tree
+*See Regex* -v | --verbose | Set verbose level (1-5) or 'debug' = 1 | --ignore-
+errors | Ignore read errors (such as permission errors) - Default is to error
+and exit | --no-print | Don't print any output | --version | Print version info
+and exit >It is recommended to quote all paths ### *Exclusions* >Provide names
+of files or directories to exclude. To exclude multiple files/directories,
+quote entire list and seperate with a colon (**:**). Add a forward slash (**/
+**) to specify a directory name to exclude. ##### **Example:** ```bash dirtree
+--exclude "excluded dir:excluded file" ``` ### *Regex* >Prefix regex with
+*include=* or *exclude=* >Seperate each regex with a space, quoting each
+individual argument. ##### _**Examples:**_ ```bash dirtree --regex
+"exclude=.*\.ini$" # will exclude any files that have a *.ini* extension.
+dirtree --regex "include=.*\.mp3$" # will include only files with a *.mp3*
+extension. ``` >This has no effect on directories >Multiple regex can be used
+by specifying **--regex** multiple times. ## License ==========
     MIT License
 
     Copyright (c) [2022] [Erik Beebe]
 
     Permission is hereby granted, free of charge, to any person obtaining a
 copy
     of this software and associated documentation files (the "Software"), to
@@ -69,8 +70,14 @@
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
 README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
 fixed title when printing to tty #### v0.3.2 - 7-15-2023 - added colorized tree
 for symlinked directories - prevent symlinks from causing infinite recursion -
 colored recursive directory links red - moved formatting code to class
-instances
+instances #### v0.3.4 - 7-15-2023 - fixed hidden file detection in windows -
+added more title methods #### v0.4.0 - 7-16-2023 - updated bb_appdirs - changed
+some log messages - added more title methods - added a fancy title header -
+added winvolumeinfo module - added unixvolumeinfo module - added option to
+print version info - adjusted output for when base directory is a link -
+changed html colors to hex values and adjusted - changed tty colors to rgb
+values - changed some option arguments
```

### Comparing `bb_dirtree-0.3.2/bbdirtree/COLORS.py` & `bb_dirtree-0.4.0/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.2/bbdirtree/__main__.py` & `bb_dirtree-0.4.0/bbdirtree/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,65 @@
-import sys, os, ctypes, logging
-from configparser import ConfigParser
+import sys, os, logging, stat
 from re import match
 from os.path import ( isdir,
                       isfile,
                       islink,
                       join,
                       basename,
                       dirname,
                       realpath  )
-from glob import glob
-from .COLORS import *
 
 log = logging.getLogger(__name__)
 
+from .COLORS import *
+from . import __version__
+
 class DirTree:
     """
     Create a nice looking directory tree
     """
-    _FORMAT = { 'tty': { 'dir'     : f"{C_b()}_-_{C__()}",               # blue
-                         'dirname' : f"{C_c()}_-_{C__()}",               # light cyan
-                         'text'    : f"{C_Gr()}_-_{C__()}",              # dark gray
-                         'file'    : f"{C_gri()}_-_{C__()}",             # italic gray
-                         'link'    : f"{C_Ci()}_-_{C__()}",              # cyan italic
-                         'filelink': f"{C_Gri()}_-_{C__()}",             # dark gray italic
-                         'dirlink' : f"{C_bi()}_-_{C__()}",              # light blue italic
-                         'replink' : f"{C_ri()}_-_{C__()}",              # light red italic
-                         'tree'    : f"{C_g()}_-_{C__()}",               # green
-                         'treelink': f"{C_C()}_-_{C__()}",               # cyan
-                         'pre'     : f"\n{C_W()}    {F_U()}_-_{C__()}",  # White
-                         'title'   : f"{C_O()} {F_U()}_-_{C__()}",       # orange
+    _FORMAT = { 'tty': { 'dir'     : f"\x1b[38;2;0;0;255m_-_{C__()}",                   # blue
+                         'dirname' : f"\x1b[38;2;29;84;173;1m_-_{C__()}",               # kinda blue, kinda purple BOLD
+                         'text'    : f"\x1b[38;2;144;144;144m_-_{C__()}",               # gray
+                         'file'    : f"\x1b[38;2;202;202;202m_-_{C__()}",               # light gray
+                         'link'    : f"\x1b[38;2;19;245;234;3m_-_{C__()}",              # cyan italic
+                         'filelink': f"\x1b[38;2;91;91;91;3m_-_{C__()}",                # dark gray italic
+                         'dirlink' : f"\x1b[38;2;88;154;252;3m_-_{C__()}",              # light blue italic
+                         'replink' : f"\x1b[38;2;184;0;0;3m_-_{C__()}",                 # red italic
+                         'tree'    : f"\x1b[38;2;99;184;105m_-_{C__()}",                # light green
+                         'treelink': f"\x1b[38;2;117;175;184m_-_{C__()}",               # light blue/green
+                         'title'   : f"\x1b[38;2;255;255;255m{F_U()}_-_{C__()}",        # White UNDERLINE
+                         'title2'  : f"\x1b[38;2;221;221;221;1m_-_{C__()}",             # offwhite BOLD
+                         'pre'     : '',
                          'post'    : "",
                          'nl'      : '\n' },
-                'html': { 'dir'     : "<font color=\"Blue\">_-_</font>",              # cyan
-                          'dirname' : "<font color=\"DarkCyan\">_-_</font>",          # light cyan
-                          'text'    : "<font color=\"Gray\">_-_</font>",              # gray
-                          'file'    : "<font color=\"Gray\">_-_</font>",              # light gray
-                          'link'    : "<font color=\"Cyan\"><i>_-_</i></font>",       # cyan italic
-                          'filelink': "<font color=\"DarkGray\"><i>_-_</i></font>",   # dark gray italic
-                          'dirlink' : "<font color=\"Blue\"><i>_-_</i></font>",       # light blue italic
-                          'replink' : "<font color=\"Red\"><i>_-_</i></font>",        # red italic
-                          'tree'    : "<font color=\"LightGreen\">_-_</font>",        # green
-                          'treelink': "<font color=\"Cyan\">_-_</font>",              # light cyan
-                          'pre'     : "<body style=\"background-color: Black;\"><pre><font color=\"White\">  <u>_-_</u></font>",
-                          'title'   : "<font color=\"Orange\">  <u>_-_</u></font>",
+                'html': { 'dir'     : "<font color=\"#0000ff\">_-_</font>",             # blue
+                          'dirname' : "<font color=\"#1d54ad\"><b>_-_</b></font>",      # kinda blue, kinda purple BOLD
+                          'text'    : "<font color=\"#909090\">_-_</font>",             # gray
+                          'file'    : "<font color=\"#cacaca\">_-_</font>",             # light gray
+                          'link'    : "<font color=\"#13f5ea\"><i>_-_</i></font>",      # cyan italic
+                          'filelink': "<font color=\"#5b5b5b\"><i>_-_</i></font>",      # dark gray italic
+                          'dirlink' : "<font color=\"#589afc\"><i>_-_</i></font>",      # light blue italic
+                          'replink' : "<font color=\"#b80000\"><i>_-_</i></font>",      # red italic
+                          'tree'    : "<font color=\"#63b869\">_-_</font>",             # light green
+                          'treelink': "<font color=\"#75afb8\">_-_</font>",             # light blue/green
+                          'title'   : "<font color=\"#ffffff\">  <u>_-_</u></font>",    # white UNDERLINE
+                          'title2'  : "<font color=\"#dddddd\"><b>_-_</b></font>",      # offwhite BOLD
+                          'pre'     : "<body style=\"background-color: #000000; color: #ffffff;\"><pre>",
                           'post'    : "</pre></body>",
                           'nl'      : "<br>" }}
     _LINK_LIST = []
+    count = { 'dirs'          : 0,
+              'files'         : 0,
+              'followed_links': 0,
+              'linkdirs'      : 0,
+              'linkfiles'     : 0,
+              'hidden_files'  : 0,
+              'hidden_dirs'   : 0,
+              'hidden_links'  : 0 }
 
     def __init__( self,
                   directory     = None,
                   depth         = 999999, *,
                   dotfiles      = False,
                   exclude_dirs  = [],
                   exclude_files = [],
@@ -100,107 +110,157 @@
         Recursive scan of base directory
             Returns layered dictionary { 'dirs': {}, 'files': [] }
         """
         @staticmethod
         def create_subdir():
             subdir = { 'dirs'  : {},
                        'files' : [],
-                       'path'  : '' }
+                       'path'  : '',
+                       'error' : False }
             return subdir
 
         base_dir     = self.base_dir
         dotfiles     = self.dotfiles
         scandirs     = []
         self.listing = create_subdir()
         self.listing['path'] = base_dir
 
-        def iterDir(directory):
-            def has_hidden_attr(filepath):
-                try:
-                    attrs = ctypes.windll.kernel32.GetFileAttributesW(unicode(filepath))
-                    assert attrs != -1
-                    result = bool(attrs & 2)
-                except (AttributeError, AssertionError):
-                    result = False
-                return result
 
-            dirs, files = [], []
+        def isHidden(path):
+            R = False
+            try:
+                if sys.platform == 'windows':
+                    x = os.stat(path)
+                    if x.st_file_attributes % 4 == stat.FILE_ATTRIBUTE_HIDDEN:
+                        R = True
+                elif match( '^\.+', basename(path) ):
+                    R = True
+            except Exception as E:
+                log.exception(E)
+            finally:
+                return R
+
+        def iterDir(directory, count):
+            dirs, files, ERROR = [], [], False
             try:
+                toIter = os.listdir(directory)
                 _E = None
                 log.debug(f"Scanning directory - '{directory}'")
-                for i in os.listdir(directory):
+                for i in toIter:
                     path = join( directory, i )
+                    _islink = False
+                    _isdir  = False
+                    _hidden = isHidden(path)
 
-                    if ( match( '^\.+', i ) or has_hidden_attr( path )) and not dotfiles:
+                    if not dotfiles and _hidden:
                         continue
 
                     elif islink( path ):
+                        _islink = True
                         if self.follow_links:
                             if ( basename( path ), realpath( path )) in self._LINK_LIST:
-                                log.warning(f"Avoiding continuous recursion from symlink - '{path}'")
+                                log.warning(f"Found infinite recursion loop from symlink to '{realpath(path)}'")
                                 files.append((i, 'replink', f' --> {realpath( path )}'))
                             elif isdir( path ):
+                                _isdir = True
+                                log.info(f"Following symlink - '{path}'")
+                                count['followed_links'] += 1
+                                count['linkdirs'] += 1
                                 self._LINK_LIST.append(( basename( path ), realpath( path )))
                                 dirs.append((i, 'link', f' --> {realpath( path )}'))
                             else:
+                                log.debug(f"Found file symlink - '{path}'")
+                                count['linkfiles'] += 1
                                 files.append((i, 'filelink', f' --> {realpath( path )}'))
                         elif isdir( join( directory, i )):
+                            _isdir = True
+                            log.debug(f"Found directory symlink - '{path}'")
+                            count['linkdirs'] += 1
                             files.append((i, 'dirlink', f' --> {realpath( path )}'))
                         else:
+                            log.debug(f"Found file symlink - '{path}'")
+                            count['linkfiles'] += 1
                             files.append((i, 'filelink', f' --> {realpath( path )}'))
 
                     elif isdir( path ):
+                        _isdir = True
+                        count['dirs'] += 1
                         dirs.append((i, 'dir'))
 
                     else:
+                        count['files'] += 1
                         files.append((i, 'file'))
 
+                    if _hidden:
+                        if _islink:
+                            count['hidden_links'] += 1
+                        elif _isdir:
+                            count['hidden_dirs'] += 1
+                        else:
+                            count['hidden_files'] += 1
+
                 dirs = sorted( dirs, key = lambda x:x[0] )
                 files = sorted( files, key = lambda x:x[0] )
 
             except PermissionError as E:
-                log.warning( str(E) )
+                ERROR = True
                 _E = E
 
             except Exception as E:
-                log.exception(E)
+                ERROR = True
                 _E = E
 
             finally:
-                if _E and not self.ignore_errors:
-                    raise _E
+                if _E:
+                    if self.ignore_errors:
+                        log.warning( str(_E) )
+                    else:
+                        log.error( str(_E) )
+                        sys.exit(2)
 
-                return files, dirs, directory
+                return files, dirs, directory, ERROR
 
         level = 0
         scandirs = [( self.listing, base_dir, level )]
 
         scan = True
         while scan:
             try:
                 current, scandir, level = scandirs.pop(0)
             except:
                 scan = False
                 continue
 
-            F, D, path = iterDir(scandir)
+            F, D, path, ERROR = iterDir(scandir, self.count)
             current['path'] = path
+            current['error'] = ERROR
 
             for d in D:
                 if self.__chk_exclude(d[0], ftype = 'dir'):
                     current['dirs'][d] = create_subdir()
                     if level < self.depth:
                         scandirs.append(( current['dirs'][d], join(scandir, d[0]), level + 1 ))
                     else:
-                        log.info(f"Level of depth '({self.depth})' has been reached")
+                        log.debug(f"Level of depth '({self.depth})' has been reached")
+                        if self.follow_links and d[1] == 'link':
+                            log.info(f"Removing followed link count for '{join(scandir, d[0])}' - max depth reached")
+                            self.count['followed_links'] -= 1
 
             for f in F:
                 if self.__chk_exclude(f[0]):
                     current['files'].append(f)
 
+        if self.depth < 999999:
+            log.info(f"Recursion depth limited to {self.depth}")
+
+        log.info(f"Found {self.count['files'] + self.count['linkfiles']} files and {self.count['dirs'] + self.count['linkdirs']} directories")
+        log.info(f"Found {self.count['linkfiles']} symlinked files")
+        log.info(f"Found {self.count['linkdirs']} symlinked directories")
+        log.info(f"Followed {self.count['followed_links']} symlinked directories")
+
     def __chk_reg(func):
         def __wrapper(self, item, ftype = 'file'):
             if ( not self.regex_ex and not self.regex_in ) or ftype == 'dir':
                 R = func(self, item, ftype)
                 return R
 
             exclude = False
@@ -340,15 +400,15 @@
                     if file:
                         with open( file, 'r' ) as f:
                             file_lines = [ i.strip() for i in f.read().strip().split('\n') ]
 
                         for line in file_lines:
                             if line.startswith('name'):
                                 name = line.split('=')[1].replace('"', '').replace("'", '').strip()
-                                return name
+                                return f"Python Project: {name}"
 
                         if not name:
                             return 'Python Project'
 
                     else:
                         cd = dirname(cd)
 
@@ -364,64 +424,164 @@
                         file = join( cd, '.SRCINFO' )
                         with open( file, 'r' ) as f:
                             file_lines = [ i.strip() for i in f.read().strip().split('\n') ]
 
                         for line in file_lines:
                             if line.startswith('pkgbase'):
                                 name = line.split('=')[1].replace('"', '').replace("'", '').strip()
-                                return name
+                                return f"Git Project: {name}"
 
                         if not name:
                             return 'Git Project'
 
                     else:
                         cd = dirname(cd)
 
+            def getWinTitle(D):
+                for P in os.path.getvars('%PATH%').split(';'):
+                    if D == P:
+                        if D.startswith( os.path.expanduser('~') ):
+                            return "User Path Directory"
+                        else:
+                            return "System Path Directory"
+
+                if D.startswith( os.path.expanduser('~') ):
+                    return f"User Directory: {basename(D)}"
+
+                elif D.startswith( os.path.expandvars('%SystemRoot%')):
+                    if D == os.path.expandvars('%SystemRoot%'):
+                        return f"Windows Root Directory"
+                    else:
+                        return f"Windows Root: {basename(D)}"
+
+
+                root_drive = os.path.abspath( os.path.sep )
+                drive = os.path.abspath( D ).split( os.path.sep )[0] + os.path.sep
+                if D.startswith( root_drive ):
+                    return f"System: {basename(D)}"
+
+                from .winvolumeinfo import VolumeInfo
+                vi = VolumeInfo( drive )
+                if vi.disk_label:
+                    return f"Disk: {vi.disk_label}"
+                elif vi.serial:
+                    return f"Disk: {vi.serial}"
+                else:
+                    return 'BB-DirTree'
+
+            def getUnixTitle(D):
+                for P in os.environ['PATH'].split(':'):
+                    if D == P:
+                        if D.startswith( os.path.expanduser('~') ):
+                            return "User Path Directory"
+                        else:
+                            return "System Path Directory"
+
+                if D.startswith( os.path.expanduser('~') ):
+                    return f"User Directory: {basename(D)}"
+
+                from .unixvolumeinfo import VolumeInfo
+                vi = VolumeInfo()
+                part = vi.fromPath( D )
+
+                if part['MOUNTPOINT'] == os.path.abspath( os.path.sep ):
+                    if D == os.path.abspath( os.path.sep ):
+                        return f"Linux Root"
+                    else:
+                        return f"Root: {basename(D)}"
+
+                elif part:
+                    if part['LABEL']:
+                        return f"Disk: {part['LABEL']}"
+
+                    elif part['PATH']:
+                        return f"Disk: {part['PATH']}"
+
+                return 'BB-DirTree'
+
             name = findPyProjectName(D)
             if name:
-                return f"Python Project: {name}"
+                return name
 
             name = findGitProjectName(D)
             if name:
-                return f"Git Project: {name}"
+                return name
 
-            return ''
+            if D == os.path.expanduser('~'):
+                name = f'Home Directory:\x1b[0;0;33m {basename(D).title()}'
 
-        title = get_title(base_dir)
-        if not title:
-            if os.getcwd() == os.path.expanduser('~'):
-                title = f'Home Directory:\x1b[0;0;33m {basename(os.getcwd()).title()}'
             else:
-                title = 'BB-DirTree'
+                if sys.platform == 'windows':
+                    name = getWinTitle(D)
+                elif sys.platform == 'linux':
+                    name = getUnixTitle(D)
+                # elif sys.platform == "darwin":        # TODO add darwin specific titles
+                #     pass
+                else:
+                    name = f"BB-DirTree"
 
-        Ilist = []
+            return name
+
+        def getFancyTitle(T):
+            try:
+                width = os.get_terminal_size().columns
+            except:
+                width = 80
+
+            if width >= 80:
+                w = 68
+            else:
+                w = width - 12
+
+            divider = f"    ┉╼{'':═^{w}}╾┉"
+            return [ divider, f'          {T}', divider ]
+
+        _TITLE = ''
+        title = get_title(base_dir)
 
         if title.find(':') >= 0:
             t0, t1 = title.split(':')
-            self._output = Plist = [ F['pre'].replace( '_-_', t0 + ':' ) + F['title'].replace( '_-_', t1.strip() ), F['dirname'].replace('_-_', '      ' + base_dir + os.path.sep ) ]
+            _TITLE = F['title'].replace( '_-_', t0.strip() + ':' ) + '  ' + F['title2'].replace( '_-_', t1.strip() )
         else:
-            self._output = Plist = [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + base_dir + os.path.sep ) ]
+            _TITLE = F['title'].replace( '_-_', title.strip() )
+
+        bd = base_dir
+        while len(bd) < 5:
+            bd = ' ' + bd
+
+        if base_dir == base_dir.split( os.path.sep )[0] + os.path.sep:
+            _basedir = F['dirname'].replace( '_-_', '       ' + bd )
+        elif islink( base_dir ):
+            _TITLE = f"{_TITLE}  {F['replink'].replace( '_-_', '(link)' )}"
+            _basedir = F['dirname'].replace( '_-_', '      ' + bd + os.path.sep ) + F['link'].replace( '_-_', " --> " + realpath(base_dir) + os.path.sep )
+        else:
+            _basedir = F['dirname'].replace( '_-_', '      ' + bd + os.path.sep )
+
+        Ilist = []
 
         dirs, files, path = getlist(listing)
         level = 1
-        Plist.append( f"{F['tree'].replace('_-_', indentText(level))}" )
+        if islink(path):
+            link_levels.append(level)
 
         if len(dirs) + len(files) <= 1:
             passbar[level] = False
         else:
             passbar[level] = True
 
+        self._output = Plist = [ F['pre'], *getFancyTitle(_TITLE), _basedir, indentText(2) ]
+
         Ilist.append(( dirs, files, level, path ))
         dirs, files = [], []
 
         while True:
             while link_levels and link_levels[-1] > level:
                 link_levels.pop(-1)
 
-            if islink(path):
+            if islink(path) and level not in link_levels:
                 link_levels = sorted( link_levels + [level] )
 
             try:
                 nextdir = dirs[0][0]
                 log.debug(f"nextdir = '{nextdir}'")
 
                 if len(dirs) + len(files) == 1:
@@ -462,38 +622,36 @@
                     self._output_data.append({'path': path, 'dirs': dirs, 'files': files, 'level': level})
                 except IndexError:
                     Plist.append( F['post'] )
                     break
 
         return F['nl'].join(Plist)
 
-def err(s):
-    print(f"\x1b[1;31m  [ERROR]\x1b[0;1;30;3m {s}\x1b[0m")
-
 def main():
     from getopt import getopt
     from tabulate import tabulate
     from time import sleep
 
     def help_message():
         headers = [ f"{C_W()}Short{C__()}", f"{C_W()}Long{C__()}", f"{C_W()}Description{C__()}" ]
 
         body = []
 
         opts = [ ( "-b", "--base-dir", f"Set base directory{C__()}\n{C_Gri()}  -uses current directory if not specified" ),
                  ( "-d", "--depth", f"Integer to set the depth of directory tree{C__()}\n{C_Gri()}  -ex: '0' will only print the base directory list" ),
                  ( "-D", "--dotfiles", f"Include hidden files in tree" ),
                  ( "-e", "--exclude", f"Filenames/directories to exclude from the tree{C__()}\n{C_Gri()}  -see *Exclusions*" ),
-                 ( "-I", "--ignore-errors", "Ignore read errors (such as permission errors) - Default is to error and exit" ),
                  ( "-h", "--help", "This help message" ),
-                 ( "-l", "--follow-symlinks", "Follow links to directories - default is NOT to follow" ),
+                 ( "-L", "--follow-links", "Follow links to directories - default is NOT to follow links" ),
                  ( "-q", "--qt-html", "Print in html format for use with QT - works with some browsers too" ),
                  ( "-r", "--regex", f"Use regex to include/exclude files in tree{C__()}\n{C_Gri()}  -see *Regex*" ),
                  ( "-v", "--verbose", "Set verbose level [1-5] <or> 'debug' = 1" ),
-                 ( "", "--no-print", "Don't print any output" )]
+                 ( "", "--ignore-errors", "Ignore read errors (such as permission errors) - Default is to error and exit" ),
+                 ( "", "--no-print", "Don't print any output" ),
+                 ( "", "--version", "Print version info and exit" )]
 
         table = []
         for i in opts:
             table.append([ C_Y() + i[0] + C__(),
                            C_Y() + i[1] + C__(),
                            C_Gr() + i[2] + C__() ])
 
@@ -521,25 +679,26 @@
                            "          exclude any files that have an 'ini' extension.",
                            f"{C_P()}        bbdirtree{C_Y()} --regex{C_Gri()} \"include=.*\\.mp3$\"{C_gri()}",
                            "          include only files with an 'mp3' extension.\n",
                            "      This has no effect on directories. Multiple regex can be",
                            f"    used by specifying{C__()}{C_Y()} --regex{C_gri()} multiple times.\n\n" ]))
 
     try:
-        opts, args = getopt( sys.argv[1:], "b:d:De:hIlqr:v:", [ "base-dir=",
-                                                                "depth=",
-                                                                "dotfiles",
-                                                                "exclude=",
-                                                                "ignore-errors",
-                                                                "follow-symlinks",
-                                                                "help",
-                                                                "no-print",
-                                                                "qt-html",
-                                                                "regex=",
-                                                                "verbose=" ])
+        opts, args = getopt( sys.argv[1:], "b:d:De:hLqr:v:", [ "base-dir=",
+                                                               "depth=",
+                                                               "dotfiles",
+                                                               "exclude=",
+                                                               "ignore-errors",
+                                                               "follow-links",
+                                                               "help",
+                                                               "no-print",
+                                                               "qt-html",
+                                                               "regex=",
+                                                               "verbose=",
+                                                               "version" ])
     except:
         opts = []
 
     BASE_DIR      = os.getcwd()
     DEPTH         = 999999
     DOTFILES      = False
     EXCLUDE_FILES = []
@@ -555,83 +714,99 @@
         if opt in ('-b', '--base-dir'):
             bdir = arg
             if not isdir(bdir):
                 bdir = join( os.getcwd(), bdir )
                 if isdir(bdir):
                     BASE_DIR = bdir
                 else:
-                    err(f"Can't find directory - '{arg}'")
+                    log.error(f"Can't find directory - '{arg}'")
                     return 1
             else:
                 BASE_DIR = arg
 
         elif opt in ('-d', '--depth'):
             try:
                 dpth = int(arg)
             except:
-                err("Depth must be an integer")
+                log.error("Depth must be an integer")
                 return 1
 
             DEPTH = dpth
 
         elif opt in ('-D', '--dotfiles'):
             DOTFILES = True
 
-        elif opt in ('-I', '--ignore-errors'):
-            IGNORE_ERRORS = True
-
         elif opt in ('-e', '--exclude'):
             for i in arg.split(':'):
                 if match( '.*/$', arg ):
                     EXCLUDE_DIRS.append(i[:-1])
                 else:
                     EXCLUDE_FILES.append(i)
 
         elif opt in ('-h', '--help'):
             help_message()
             sys.exit(0)
 
-        elif opt in ('-l', '--follow-symlinks'):
+        elif opt in ('-L', '--follow-links'):
             FOLLOW_LINKS = True
 
-        elif opt == "--no-print":
-            NO_PRINT = True
-
         elif opt in ('-q', '--qt-html'):
             HTML = True
 
         elif opt in ('-r', '--regex'):
             try:
                 m = arg.split('=', 1)[0]
                 reg = arg.split('=', 1)[1]
             except:
-                err("Invalid format for regex option. See 'dirtree --help'")
+                log.error("Invalid format for regex option. See 'dirtree --help'")
                 return 1
 
             if m == 'include':
                 REGEX_IN.append(reg)
             elif m == 'exclude':
                 REGEX_EX.append(reg)
             else:
-                err(f"Invalid regex option '{m}'. See 'dirtree --help'")
+                log.error(f"Invalid regex option '{m}'. See 'dirtree --help'")
                 return 1
 
         elif opt in ('-v', '--verbose'):
             try:
                 if arg.lower() in ( '1', 'debug' ):
                     log.set_format( 'debug' )
                 else:
                     log.set_level( int(arg) )
             except TypeError:
-                err("Verbosity must be a number 1-5 <or> 'debug'")
+                log.error("Verbosity must be a number 1-5 <or> 'debug'")
                 return 1
             except Exception as E:
                 log.exception(E)
                 raise E
 
+        elif opt == '--ignore-errors':
+            IGNORE_ERRORS = True
+
+        elif opt == "--no-print":
+            NO_PRINT = True
+
+        elif opt == '--version':
+            print( '\n'.join([ '',
+                               f"{C_W()}    ╭╼═════════════════════════════════════════════════════════╾╮",
+                               f"{C_W()}    ╽                                                           ╽",
+                               f"{C_W()}    ║     {F_U()}BB-DirTree{C__()}{C_Gri()}  - print a nice looking directory tree{C_W()}     ║",
+                               f"{C_W()}    ║                                                           ║",
+                               f"{C_W()}    ║{C_gri()}      version:{C_Gr()}   {__version__}{C_W()}                                     ║",
+                               f"{C_W()}    ║{C_gri()}      developer:{C_Gr()} Erik Beebe{C_W()}                                ║",
+                               f"{C_W()}    ║{C_gri()}      webpage:{C_C()}   https://pypi.org/project/bb-dirtree/{C_W()}      ║",
+                               f"{C_W()}    ║{C_gri()}      debugging:{C_C()} beebeapps_debugging@tuta.io{C_W()}               ║",
+                               f"{C_W()}    ║{C_gri()}      feedback:{C_C()}  beebeapps_feedback@tuta.io{C_W()}                ║",
+                               f"{C_W()}    ╿                                                           ╿",
+                               f"{C_W()}    ╰╼═════════════════════════════════════════════════════════╾╯",
+                               '' ]))
+            sys.exit(0)
+
     x = DirTree( BASE_DIR,
                  DEPTH,
                  dotfiles = DOTFILES,
                  exclude_dirs = EXCLUDE_DIRS,
                  exclude_files = EXCLUDE_FILES,
                  regex_ex = REGEX_EX,
                  regex_in = REGEX_IN,
```

### Comparing `bb_dirtree-0.3.2/pyproject.toml` & `bb_dirtree-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.3.2"
+version = "0.4.0"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
 
 [tool.poetry.scripts]
 dirtree = 'bbdirtree.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tabulate = "^0.8.9"
-bb-apputils = "^0.3.9"
+bb-apputils = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bb_dirtree-0.3.2/PKG-INFO` & `bb_dirtree-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.3.2
+Version: 0.4.0
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bb-apputils (>=0.3.9,<0.4.0)
+Requires-Dist: bb-apputils (>=0.4.0,<0.5.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Description-Content-Type: text/markdown
 
 <style> table { text-align: center; } </style>
 
 # DirTree
 
@@ -33,27 +33,28 @@
 
 ```bash
 dirtree [OPTIONS] [ARGS]
 ```
 
 ### _**Options:**_
 
-**Short**  | **Long**               | **Description**
----------- | ---------------------- | ---------------------------------------------------------
-    -b     |   --base-dir           |  Set base directory <br> *Uses current directory if not specified*
-    -d     |   --depth              |  Integer to set the depth of directory tree <br> *ex: '0' will only print the base directory list*
-    -D     |   --dotfiles           |  Include hidden files in tree
-    -e     |   --exclude            |  Filenames/directories to exclude from the tree <br> *See Exclusions*
-    -h     |   --help               |  This help message
-    -I     |   --ignore-errors      |  Ignore read errors (such as permission errors) - Default is to error and exit
-    -l     |   --follow-symlinks    |  Follow links to directories - default is NOT to follow
-    -q     |   --qt-html            |  Print in html format for use with QT
-    -r     |   --regex              |  Use regex to include/exclude files/directories in tree <br> *See Regex*
-    -v     |   --verbose            |  Set verbose level (1-5) or 'debug' = 1
-           |   --no-print           |  Don't print any output
+**Short**  | **Long**           | **Description**
+---------- | ------------------ | ---------------------------------------------------------
+    -b     |   --base-dir       |  Set base directory <br> *Uses current directory if not specified*
+    -d     |   --depth          |  Integer to set the depth of directory tree <br> *ex: '0' will only print the base directory list*
+    -D     |   --dotfiles       |  Include hidden files in tree
+    -e     |   --exclude        |  Filenames/directories to exclude from the tree <br> *See Exclusions*
+    -h     |   --help           |  This help message
+    -L     |   --follow-links   |  Follow links to directories - default is NOT to follow
+    -q     |   --qt-html        |  Print in html format for use with QT
+    -r     |   --regex          |  Use regex to include/exclude files/directories in tree <br> *See Regex*
+    -v     |   --verbose        |  Set verbose level (1-5) or 'debug' = 1
+           |   --ignore-errors  |  Ignore read errors (such as permission errors) - Default is to error and exit
+           |   --no-print       |  Don't print any output
+           |   --version        |  Print version info and exit
 
 >It is recommended to quote all paths
 
 ### *Exclusions*
 
 >Provide names of files or directories to exclude. To exclude multiple files/directories, quote entire list and seperate with a colon (**:**). Add a forward slash (**/**) to specify a directory name to exclude.
 
@@ -185,7 +186,26 @@
 #### v0.3.2 - 7-15-2023
 
 - added colorized tree for symlinked directories
 - prevent symlinks from causing infinite recursion
     - colored recursive directory links red
 - moved formatting code to class instances
 
+#### v0.3.4 - 7-15-2023
+
+- fixed hidden file detection in windows
+- added more title methods
+
+#### v0.4.0 - 7-16-2023
+
+- updated bb_appdirs
+- changed some log messages
+- added more title methods
+- added a fancy title header
+- added winvolumeinfo module
+- added unixvolumeinfo module
+- added option to print version info
+- adjusted output for when base directory is a link
+- changed html colors to hex values and adjusted
+- changed tty colors to rgb values
+- changed some option arguments
+
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: bb-dirtree Version: 0.3.2 Summary: Create a nice
+Metadata-Version: 2.1 Name: bb-dirtree Version: 0.4.0 Summary: Create a nice
 looking directory tree with options License: MIT Keywords: script,qt,files
 Author: Erik Beebe Author-email: beebeapps_feedback@tuta.io Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: bb-
-apputils (>=0.3.9,<0.4.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
+apputils (>=0.4.0,<0.5.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
 Content-Type: text/markdown
  # DirTree -------------------------------------------- ##### Create a nice
 looking directory tree -------------------------------------------- ##
 Installation: ```bash python -m pip install "BB-DirTree" ``` ## DirTree usage
 ```bash dirtree [OPTIONS] [ARGS] ``` ### _**Options:**_ **Short** | **Long** |
-**Description** ---------- | ---------------------- | -------------------------
--------------------------------- -b | --base-dir | Set base directory
+**Description** ---------- | ------------------ | -----------------------------
+---------------------------- -b | --base-dir | Set base directory
 *Uses current directory if not specified* -d | --depth | Integer to set the
 depth of directory tree
 *ex: '0' will only print the base directory list* -D | --dotfiles | Include
 hidden files in tree -e | --exclude | Filenames/directories to exclude from the
 tree
-*See Exclusions* -h | --help | This help message -I | --ignore-errors | Ignore
-read errors (such as permission errors) - Default is to error and exit -l | --
-follow-symlinks | Follow links to directories - default is NOT to follow -q | -
--qt-html | Print in html format for use with QT -r | --regex | Use regex to
-include/exclude files/directories in tree
-*See Regex* -v | --verbose | Set verbose level (1-5) or 'debug' = 1 | --no-
-print | Don't print any output >It is recommended to quote all paths ###
-*Exclusions* >Provide names of files or directories to exclude. To exclude
-multiple files/directories, quote entire list and seperate with a colon (**:
-**). Add a forward slash (**/**) to specify a directory name to exclude. #####
-**Example:** ```bash dirtree --exclude "excluded dir:excluded file" ``` ###
-*Regex* >Prefix regex with *include=* or *exclude=* >Seperate each regex with a
-space, quoting each individual argument. ##### _**Examples:**_ ```bash dirtree
---regex "exclude=.*\.ini$" # will exclude any files that have a *.ini*
-extension. dirtree --regex "include=.*\.mp3$" # will include only files with a
-*.mp3* extension. ``` >This has no effect on directories >Multiple regex can be
-used by specifying **--regex** multiple times. ## License ==========
+*See Exclusions* -h | --help | This help message -L | --follow-links | Follow
+links to directories - default is NOT to follow -q | --qt-html | Print in html
+format for use with QT -r | --regex | Use regex to include/exclude files/
+directories in tree
+*See Regex* -v | --verbose | Set verbose level (1-5) or 'debug' = 1 | --ignore-
+errors | Ignore read errors (such as permission errors) - Default is to error
+and exit | --no-print | Don't print any output | --version | Print version info
+and exit >It is recommended to quote all paths ### *Exclusions* >Provide names
+of files or directories to exclude. To exclude multiple files/directories,
+quote entire list and seperate with a colon (**:**). Add a forward slash (**/
+**) to specify a directory name to exclude. ##### **Example:** ```bash dirtree
+--exclude "excluded dir:excluded file" ``` ### *Regex* >Prefix regex with
+*include=* or *exclude=* >Seperate each regex with a space, quoting each
+individual argument. ##### _**Examples:**_ ```bash dirtree --regex
+"exclude=.*\.ini$" # will exclude any files that have a *.ini* extension.
+dirtree --regex "include=.*\.mp3$" # will include only files with a *.mp3*
+extension. ``` >This has no effect on directories >Multiple regex can be used
+by specifying **--regex** multiple times. ## License ==========
     MIT License
 
     Copyright (c) [2022] [Erik Beebe]
 
     Permission is hereby granted, free of charge, to any person obtaining a
 copy
     of this software and associated documentation files (the "Software"), to
@@ -77,8 +78,14 @@
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
 README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
 fixed title when printing to tty #### v0.3.2 - 7-15-2023 - added colorized tree
 for symlinked directories - prevent symlinks from causing infinite recursion -
 colored recursive directory links red - moved formatting code to class
-instances
+instances #### v0.3.4 - 7-15-2023 - fixed hidden file detection in windows -
+added more title methods #### v0.4.0 - 7-16-2023 - updated bb_appdirs - changed
+some log messages - added more title methods - added a fancy title header -
+added winvolumeinfo module - added unixvolumeinfo module - added option to
+print version info - adjusted output for when base directory is a link -
+changed html colors to hex values and adjusted - changed tty colors to rgb
+values - changed some option arguments
```

