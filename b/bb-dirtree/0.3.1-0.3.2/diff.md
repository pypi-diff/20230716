# Comparing `tmp/bb_dirtree-0.3.1.tar.gz` & `tmp/bb_dirtree-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.3.1.tar", max compression
+gzip compressed data, was "bb_dirtree-0.3.2.tar", max compression
```

## Comparing `bb_dirtree-0.3.1.tar` & `bb_dirtree-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.3.1/LICENSE
--rw-r--r--   0        0        0     4869 2023-07-15 21:07:59.020363 bb_dirtree-0.3.1/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.3.1/bbdirtree/COLORS.py
--rw-r--r--   0        0        0      125 2023-07-15 21:08:10.373696 bb_dirtree-0.3.1/bbdirtree/__init__.py
--rw-r--r--   0        0        0    25319 2023-07-15 21:07:27.760362 bb_dirtree-0.3.1/bbdirtree/__main__.py
--rw-r--r--   0        0        0      577 2023-07-15 21:08:08.160363 bb_dirtree-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 bb_dirtree-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5082 2023-07-16 00:27:22.950588 bb_dirtree-0.3.2/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.3.2/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0      125 2023-07-16 00:26:34.300588 bb_dirtree-0.3.2/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    25116 2023-07-16 00:26:18.767254 bb_dirtree-0.3.2/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      577 2023-07-16 00:26:35.340587 bb_dirtree-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 bb_dirtree-0.3.2/PKG-INFO
```

### Comparing `bb_dirtree-0.3.1/LICENSE` & `bb_dirtree-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.1/README.md` & `bb_dirtree-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -160,7 +160,14 @@
 - changed the way the title is generated
 - updated README to reflect changes
 - cleaned up some code
 
 #### v0.3.1 - 7-15-2023
 
 - fixed title when printing to tty
+
+#### v0.3.2 - 7-15-2023
+
+- added colorized tree for symlinked directories
+- prevent symlinks from causing infinite recursion
+    - colored recursive directory links red
+- moved formatting code to class instances
```

#### html2text {}

```diff
@@ -66,8 +66,11 @@
 7-10-2023 - fixed typo in __main__ #### v0.2.6 - 7-10-2023 - bugfixes ####
 v0.3.0 - 7-15-2023 - added bb_apputils to dependencies - added bblogger for
 logging - removed __doc__ from init.py - added verbose options - added option
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
 README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
-fixed title when printing to tty
+fixed title when printing to tty #### v0.3.2 - 7-15-2023 - added colorized tree
+for symlinked directories - prevent symlinks from causing infinite recursion -
+colored recursive directory links red - moved formatting code to class
+instances
```

### Comparing `bb_dirtree-0.3.1/bbdirtree/COLORS.py` & `bb_dirtree-0.3.2/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.1/bbdirtree/__main__.py` & `bb_dirtree-0.3.2/bbdirtree/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,78 +11,111 @@
 from glob import glob
 from .COLORS import *
 
 log = logging.getLogger(__name__)
 
 class DirTree:
     """
-    Create and print a directory tree from the given directory
-        directory     = directory to create tree of [default current dir]
-        depth         = depth of directory to recurse into [default 999999]
-        dotfiles      = show/not show hidden files [default False]
-        exclude_dirs  = directories to ignore
-        exclude files = files to ignore
-        regex_ex      = regex format of files to exclude
-        regex_in      = regex format to only include files
-        title         = title for top of directory tree [default 'BB-DirTree']
-                          - detects 'git' and 'python project' directories to title automatically
-                          - can be 'None'
+    Create a nice looking directory tree
     """
+    _FORMAT = { 'tty': { 'dir'     : f"{C_b()}_-_{C__()}",               # blue
+                         'dirname' : f"{C_c()}_-_{C__()}",               # light cyan
+                         'text'    : f"{C_Gr()}_-_{C__()}",              # dark gray
+                         'file'    : f"{C_gri()}_-_{C__()}",             # italic gray
+                         'link'    : f"{C_Ci()}_-_{C__()}",              # cyan italic
+                         'filelink': f"{C_Gri()}_-_{C__()}",             # dark gray italic
+                         'dirlink' : f"{C_bi()}_-_{C__()}",              # light blue italic
+                         'replink' : f"{C_ri()}_-_{C__()}",              # light red italic
+                         'tree'    : f"{C_g()}_-_{C__()}",               # green
+                         'treelink': f"{C_C()}_-_{C__()}",               # cyan
+                         'pre'     : f"\n{C_W()}    {F_U()}_-_{C__()}",  # White
+                         'title'   : f"{C_O()} {F_U()}_-_{C__()}",       # orange
+                         'post'    : "",
+                         'nl'      : '\n' },
+                'html': { 'dir'     : "<font color=\"Blue\">_-_</font>",              # cyan
+                          'dirname' : "<font color=\"DarkCyan\">_-_</font>",          # light cyan
+                          'text'    : "<font color=\"Gray\">_-_</font>",              # gray
+                          'file'    : "<font color=\"Gray\">_-_</font>",              # light gray
+                          'link'    : "<font color=\"Cyan\"><i>_-_</i></font>",       # cyan italic
+                          'filelink': "<font color=\"DarkGray\"><i>_-_</i></font>",   # dark gray italic
+                          'dirlink' : "<font color=\"Blue\"><i>_-_</i></font>",       # light blue italic
+                          'replink' : "<font color=\"Red\"><i>_-_</i></font>",        # red italic
+                          'tree'    : "<font color=\"LightGreen\">_-_</font>",        # green
+                          'treelink': "<font color=\"Cyan\">_-_</font>",              # light cyan
+                          'pre'     : "<body style=\"background-color: Black;\"><pre><font color=\"White\">  <u>_-_</u></font>",
+                          'title'   : "<font color=\"Orange\">  <u>_-_</u></font>",
+                          'post'    : "</pre></body>",
+                          'nl'      : "<br>" }}
+    _LINK_LIST = []
 
     def __init__( self,
                   directory     = None,
                   depth         = 999999, *,
                   dotfiles      = False,
                   exclude_dirs  = [],
                   exclude_files = [],
-                  follow_links  = False,                # NEW
-                  ignore_errors = False,                # NEW
+                  follow_links  = False,
+                  ignore_errors = False,
                   regex_ex      = [],
-                  regex_in      = [],
-                  title         = 'BB-DirTree' ):
+                  regex_in      = []    ):
+        """
+        Create and print a directory tree from the given directory
+            directory     = directory to create tree of [default current dir]
+            depth         = depth of directory to recurse into [default 999999]
+            dotfiles      = show/not show hidden files [default False]
+            exclude_dirs  = directories to ignore
+            exclude files = files to ignore
+            follow_links  = follows symlinks for directories
+            ignore_errors = continue to parse directories, regardless of errors
+            regex_ex      = regex format of files to exclude
+            regex_in      = regex format to only include files
+        """
 
         if not directory:
             directory = os.getcwd()
 
         elif not isdir( directory ):
             try:
                 assert isdir( join( os.getcwd(), directory ))
                 directory = join( os.getcwd(), directory )
             except:
                 directory = os.getcwd()
 
         self.base_dir      = directory
         self.depth         = depth
         self.dotfiles      = dotfiles
-        self.ignore_errors = ignore_errors              # NEW
-        self.follow_links  = follow_links               # NEW
+        self.ignore_errors = ignore_errors
+        self.follow_links  = follow_links
         self.regex_ex      = regex_ex
         self.regex_in      = regex_in
         self.exclude_dirs  = exclude_dirs
         self.exclude_files = exclude_files
-        self.title         = title
+        self._output       = []
+        self._output_data  = []
+        self._output_type  = ''
 
         self.__getBase()
 
     def __getBase(self):
         """
         Recursive scan of base directory
             Returns layered dictionary { 'dirs': {}, 'files': [] }
         """
         @staticmethod
         def create_subdir():
-            subdir = { 'dirs' : {},
-                       'files': [],
-                       'path' : '' }
+            subdir = { 'dirs'  : {},
+                       'files' : [],
+                       'path'  : '' }
             return subdir
 
         base_dir     = self.base_dir
         dotfiles     = self.dotfiles
         scandirs     = []
         self.listing = create_subdir()
+        self.listing['path'] = base_dir
 
         def iterDir(directory):
             def has_hidden_attr(filepath):
                 try:
                     attrs = ctypes.windll.kernel32.GetFileAttributesW(unicode(filepath))
                     assert attrs != -1
                     result = bool(attrs & 2)
@@ -91,42 +124,42 @@
                 return result
 
             dirs, files = [], []
             try:
                 _E = None
                 log.debug(f"Scanning directory - '{directory}'")
                 for i in os.listdir(directory):
-                    if ( match( '^\.+', i ) or has_hidden_attr( join( directory, i )) ) and not dotfiles:
+                    path = join( directory, i )
+
+                    if ( match( '^\.+', i ) or has_hidden_attr( path )) and not dotfiles:
                         continue
 
-                    elif islink( join( directory, i )):                         # NEW -----------------
+                    elif islink( path ):
                         if self.follow_links:
-                            if isdir( join( directory, i )):
-                                dirs.append((i, 'link', f' --> {realpath(join(directory, i))}'))
-                                # log.debug(f"Added directory link '{dirs[-1]}'")
+                            if ( basename( path ), realpath( path )) in self._LINK_LIST:
+                                log.warning(f"Avoiding continuous recursion from symlink - '{path}'")
+                                files.append((i, 'replink', f' --> {realpath( path )}'))
+                            elif isdir( path ):
+                                self._LINK_LIST.append(( basename( path ), realpath( path )))
+                                dirs.append((i, 'link', f' --> {realpath( path )}'))
                             else:
-                                files.append((i, 'link', f' --> {realpath(join(directory, i))}'))
-                                # log.debug(f"Added file link '{files[-1]}'")
+                                files.append((i, 'filelink', f' --> {realpath( path )}'))
                         elif isdir( join( directory, i )):
-                            files.append((i, 'dirlink', f' --> {realpath(join(directory, i))}'))
-                            # log.debug(f"Added directory link as file '{files[-1]}'")
+                            files.append((i, 'dirlink', f' --> {realpath( path )}'))
                         else:
-                            files.append((i, 'link', f' --> {realpath(join(directory, i))}'))
-                            # log.debug(f"Added file link '{files[-1]}'")
-                                                                                # ---------------------
-                    elif isdir( join( directory, i )):
+                            files.append((i, 'filelink', f' --> {realpath( path )}'))
+
+                    elif isdir( path ):
                         dirs.append((i, 'dir'))
-                        # log.debug(f"Added directory '{dirs[-1]}'")
 
                     else:
                         files.append((i, 'file'))
-                        # log.debug(f"Added file '{files[-1]}'")
 
-                dirs = sorted( dirs, key = lambda x:x[0] )              # NEW
-                files = sorted( files, key = lambda x:x[0] )            # NEW
+                dirs = sorted( dirs, key = lambda x:x[0] )
+                files = sorted( files, key = lambda x:x[0] )
 
             except PermissionError as E:
                 log.warning( str(E) )
                 _E = E
 
             except Exception as E:
                 log.exception(E)
@@ -140,26 +173,27 @@
 
         level = 0
         scandirs = [( self.listing, base_dir, level )]
 
         scan = True
         while scan:
             try:
-                current, scandir, level = scandirs.pop(0)           # NEW
+                current, scandir, level = scandirs.pop(0)
             except:
                 scan = False
                 continue
 
             F, D, path = iterDir(scandir)
             current['path'] = path
+
             for d in D:
-                if self.__chk_exclude(d[0], ftype = 'dir'):         # NEW
+                if self.__chk_exclude(d[0], ftype = 'dir'):
                     current['dirs'][d] = create_subdir()
                     if level < self.depth:
-                        scandirs.append(( current['dirs'][d], join(scandir, d[0]), level + 1 ))     # NEW
+                        scandirs.append(( current['dirs'][d], join(scandir, d[0]), level + 1 ))
                     else:
                         log.info(f"Level of depth '({self.depth})' has been reached")
 
             for f in F:
                 if self.__chk_exclude(f[0]):
                     current['files'].append(f)
 
@@ -206,103 +240,91 @@
 
             return True
 
     def list_tty(self):
         """
         Return directory tree formatted for terminal view
         """
-        _FORMAT = { 'dir'     : f"{C_b()}_-_{C__()}",     # blue
-                    'dirname' : f"{C_c()}_-_{C__()}",     # light cyan
-                    'text'    : f"{C_Gr()}_-_{C__()}",    # dark gray
-                    'file'    : f"{C_gri()}_-_{C__()}",   # italic gray
-                    'link'    : f"{C_Ci()}_-_{C__()}",    # cyan italic              # NEW
-                    'filelink': f"{C_Gri()}_-_{C__()}",   # dark gray italic         # NEW
-                    'dirlink' : f"{C_bi()}_-_{C__()}",    # light blue italic        # NEW
-                    'tree'    : f"{C_g()}_-_{C__()}",     # green
-                    'pre'     : f"\n{C_W()}    {F_U()}_-_{C__()}",  # White
-                    'title'   : f"{C_O()} {F_U()}_-_{C__()}",    # orange
-                    'post'    : "",
-                    'nl'      : '\n' }
-
-        self.__getBase()
-        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
+        self._output_type = 'TTY'
+        list_tree = self.get_tree( self._FORMAT['tty'] )
 
         return list_tree
 
     def list_gui(self):
         """
         Return directory tree in html formatting
         """
-        _FORMAT = { 'dir'     : "<font color=\"Blue\">_-_</font>",               # cyan
-                    'dirname' : "<font color=\"DarkCyan\">_-_</font>",           # light cyan
-                    'text'    : "<font color=\"Gray\">_-_</font>",               # gray
-                    'file'    : "<font color=\"Gray\">_-_</font>",               # light gray
-                    'link'    : "<font color=\"Cyan\"><i>_-_</i></font>",        # cyan italic          # NEW
-                    'filelink': "<font color=\"DarkGray\"><i>_-_</i></font>",       # dark gray italic     # NEW
-                    'dirlink' : "<font color=\"Blue\"><i>_-_</i></font>",    # light blue italic    # NEW
-                    'tree'    : "<font color=\"LightGreen\">_-_</font>",        # green
-                    'pre'     : "<body style=\"background-color: Black;\"><pre><font color=\"White\">  <u>_-_</u></font>",
-                    'title'   : "<font color=\"Orange\">  <u>_-_</u></font>",
-                    'post'    : "</pre></body>",
-                    'nl'      : "<br>" }
-
-        self.__getBase()
-        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
+        self._output_type = 'HTML'
+        list_tree = self.get_tree( self._FORMAT['html'] )
 
         return list_tree
 
-    @staticmethod
-    def get_tree( listing, F, skel, TITLE ):
+    def get_tree(self, F):
+        link_levels = []
+        level = 0
+        listing = dict( self.listing.items() )
+        base_dir = self.base_dir
+        passbar = {0: False}
+
         def tree(f):
             T, B, L = '     ├', '──', '     └'
+            R = ''
 
             if f == 'T':
-                return T + B
+                R = T + B
 
             elif f == 'L':
-                return L + B
+                R = L + B
 
             else:
                 raise RuntimeError(f"Invalid key for 'f' - '{f}'")
 
+            if level in link_levels:
+                return F['treelink'].replace('_-_', R)
+            else:
+                return F['tree'].replace('_-_', R)
+
         def indentText(num):
             pbT = '     │'
             pbF = '      '
             R = ''
 
             if num == 0:
                 return ''
 
             for i in range(0, num):
                 if passbar[i]:
-                    R = R + pbT
+                    if i in link_levels:
+                        R = R + F['treelink'].replace('_-_', pbT)
+                    else:
+                        R = R + F['tree'].replace('_-_', pbT)
                 else:
                     R = R + pbF
 
             return R
 
         def getlist(obj):
             log.debug( f"Getting file list" )
             if not obj['dirs'] and not obj['files']:
                 log.debug("Nothing to add")
-                return [], []
+                return [], [], obj['path']
 
             d = []
             for i in obj['dirs']:
                 if len(i) == 3:
                     d.append(( obj['dirs'][i], i[0], i[1], i[2] ))
                 else:
                     d.append(( obj['dirs'][i], i[0], i[1] ))
                 log.debug( f"Appended '{d[-1]}' to file list" )
 
 
             log.debug( f"Files in list = '{obj['files']}'" )
             f = obj['files']
 
-            return d, f
+            return d, f, obj['path']
 
         def get_title(D):
             def findPyProjectName(D):           # Search for python project name
                 cd = D
                 name = None
                 file, file_lines = None, []
                 while True:
@@ -360,81 +382,88 @@
 
             name = findGitProjectName(D)
             if name:
                 return f"Git Project: {name}"
 
             return ''
 
-        title = get_title(skel)
+        title = get_title(base_dir)
         if not title:
             if os.getcwd() == os.path.expanduser('~'):
                 title = f'Home Directory:\x1b[0;0;33m {basename(os.getcwd()).title()}'
-            elif TITLE:
-                title = TITLE
             else:
                 title = 'BB-DirTree'
-        if title.find(':') >= 0:                # NEW ---------------------------------------------------------------------------------------------------------------
+
+        Ilist = []
+
+        if title.find(':') >= 0:
             t0, t1 = title.split(':')
-            Ilist, Plist = [], [ F['pre'].replace( '_-_', t0 + ':' ) + F['title'].replace( '_-_', t1.strip() ), F['dirname'].replace('_-_', '      ' + skel + os.path.sep ) ]
+            self._output = Plist = [ F['pre'].replace( '_-_', t0 + ':' ) + F['title'].replace( '_-_', t1.strip() ), F['dirname'].replace('_-_', '      ' + base_dir + os.path.sep ) ]
         else:
-            Ilist, Plist = [], [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + skel + os.path.sep ) ]
-                                                # -------------------------------------------------------------------------------------------------------------------
-        form = F
+            self._output = Plist = [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + base_dir + os.path.sep ) ]
 
-        dirs, files = getlist(listing)
-        passbar = {0: False}
+        dirs, files, path = getlist(listing)
         level = 1
-        passbar[level] = True
         Plist.append( f"{F['tree'].replace('_-_', indentText(level))}" )
+
         if len(dirs) + len(files) <= 1:
             passbar[level] = False
+        else:
+            passbar[level] = True
 
-        Ilist.append(( dirs, files, level ))
+        Ilist.append(( dirs, files, level, path ))
         dirs, files = [], []
 
         while True:
+            while link_levels and link_levels[-1] > level:
+                link_levels.pop(-1)
+
+            if islink(path):
+                link_levels = sorted( link_levels + [level] )
+
             try:
                 nextdir = dirs[0][0]
+                log.debug(f"nextdir = '{nextdir}'")
 
                 if len(dirs) + len(files) == 1:
-                    if dirs[0][2] == 'link':                 # NEW
-                        Plist.append( f"{F['tree'].replace('_-_', indentText(level) + tree('L'))} {F['dirlink'].replace('_-_', dirs[0][1] + '/')} {F['link'].replace('_-_', dirs[0][3] + '/')}" )    # NEW
-                    else:
-                        Plist.append( f"{F['tree'].replace('_-_', indentText(level) + tree('L'))} {F['dir'].replace('_-_', dirs[0][1] + '/')}" )
+                    _tree = indentText(level) + tree('L')
                     passbar[level] = False
                 else:
-                    if dirs[0][2] == 'link':                 # NEW
-                        Plist.append( f"{F['tree'].replace('_-_', indentText(level) + tree('T'))} {F['dirlink'].replace('_-_', dirs[0][1] + '/')} {F['link'].replace('_-_', dirs[0][3] + '/')}" )    # NEW
-                    else:
-                        Plist.append( f"{F['tree'].replace('_-_', indentText(level) + tree('T'))} {F['dir'].replace('_-_', dirs[0][1] + '/')}" )
+                    _tree = indentText(level) + tree('T')
                     passbar[level] = True
 
+                if dirs[0][2] == 'link':
+                    _txt = f" {F['dirlink'].replace('_-_', dirs[0][1] + '/')} {F['link'].replace('_-_', dirs[0][3] + '/')}"
+                else:
+                    _txt = f" {F['dir'].replace('_-_', dirs[0][1] + '/')}"
+
+                Plist.append( _tree + _txt )
                 dirs.pop(0)
-                Ilist.append(( dirs, files, level ))
+                Ilist.append(( dirs, files, level, path ))
                 level += 1
-                dirs, files = getlist(nextdir)
+                dirs, files, path = getlist(nextdir)
 
             except IndexError:
                 for i in range(0, len(files)):
                     if i == len(files) - 1:
                         t = 'L'
                     else:
                         t = 'T'
 
                     preT = F['tree'].replace('_-_', indentText(level) + tree(t))
-                    if files[i][1] == 'link':                                                       # NEW -----------------------
-                        Plist.append( f"{preT} {F['filelink'].replace('_-_', files[i][0])} {F['link'].replace('_-_', files[i][2])}" )
-                    elif files[i][1] == 'dirlink':
-                        Plist.append( f"{preT} {F['dirlink'].replace('_-_', files[i][0])} {F['link'].replace('_-_', files[i][2] + '/')}" )
+                    if files[i][1] == 'filelink':
+                        Plist.append( f"{preT} {F[ 'filelink' ].replace('_-_', files[i][0])} {F['link'].replace('_-_', files[i][2])}" )
+                    elif files[i][1] in ( 'replink', 'dirlink' ):
+                        Plist.append( f"{preT} {F[ files[i][1] ].replace('_-_', files[i][0] + '/')} {F['link'].replace('_-_', files[i][2] + '/')}" )
                     else:
                         Plist.append( f"{preT} {F['file'].replace('_-_', files[i][0])}" )
-                                                                                                    # ---------------------------
-                try:
-                    dirs, files, level = Ilist.pop(-1)
 
+                try:
+                    dirs, files, level, path = Ilist.pop(-1)
+                    self._output_data.append({'path': path, 'dirs': dirs, 'files': files, 'level': level})
                 except IndexError:
                     Plist.append( F['post'] )
                     break
 
         return F['nl'].join(Plist)
 
 def err(s):
@@ -450,21 +479,21 @@
 
         body = []
 
         opts = [ ( "-b", "--base-dir", f"Set base directory{C__()}\n{C_Gri()}  -uses current directory if not specified" ),
                  ( "-d", "--depth", f"Integer to set the depth of directory tree{C__()}\n{C_Gri()}  -ex: '0' will only print the base directory list" ),
                  ( "-D", "--dotfiles", f"Include hidden files in tree" ),
                  ( "-e", "--exclude", f"Filenames/directories to exclude from the tree{C__()}\n{C_Gri()}  -see *Exclusions*" ),
-                 ( "-I", "--ignore-errors", "Ignore read errors (such as permission errors) - Default is to error and exit" ),        # NEW
+                 ( "-I", "--ignore-errors", "Ignore read errors (such as permission errors) - Default is to error and exit" ),
                  ( "-h", "--help", "This help message" ),
-                 ( "-l", "--follow-symlinks", "Follow links to directories - default is NOT to follow" ),               # NEW
+                 ( "-l", "--follow-symlinks", "Follow links to directories - default is NOT to follow" ),
                  ( "-q", "--qt-html", "Print in html format for use with QT - works with some browsers too" ),
                  ( "-r", "--regex", f"Use regex to include/exclude files in tree{C__()}\n{C_Gri()}  -see *Regex*" ),
-                 ( "-v", "--verbose", "Set verbose level [1-5] <or> 'debug' = 1" ),             # NEW
-                 ( "", "--no-print", "Don't print any output" )]         # NEW
+                 ( "-v", "--verbose", "Set verbose level [1-5] <or> 'debug' = 1" ),
+                 ( "", "--no-print", "Don't print any output" )]
 
         table = []
         for i in opts:
             table.append([ C_Y() + i[0] + C__(),
                            C_Y() + i[1] + C__(),
                            C_Gr() + i[2] + C__() ])
 
@@ -512,17 +541,17 @@
 
     BASE_DIR      = os.getcwd()
     DEPTH         = 999999
     DOTFILES      = False
     EXCLUDE_FILES = []
     EXCLUDE_DIRS  = []
     HTML          = False
-    IGNORE_ERRORS = False       # NEW
-    FOLLOW_LINKS  = False       # NEW
-    NO_PRINT      = False       # NEW
+    IGNORE_ERRORS = False
+    FOLLOW_LINKS  = False
+    NO_PRINT      = False
     REGEX_IN      = []
     REGEX_EX      = []
 
     for opt, arg in opts:
         if opt in ('-b', '--base-dir'):
             bdir = arg
             if not isdir(bdir):
@@ -543,32 +572,32 @@
                 return 1
 
             DEPTH = dpth
 
         elif opt in ('-D', '--dotfiles'):
             DOTFILES = True
 
-        elif opt in ('-I', '--ignore-errors'):         # NEW
+        elif opt in ('-I', '--ignore-errors'):
             IGNORE_ERRORS = True
 
         elif opt in ('-e', '--exclude'):
             for i in arg.split(':'):
                 if match( '.*/$', arg ):
                     EXCLUDE_DIRS.append(i[:-1])
                 else:
                     EXCLUDE_FILES.append(i)
 
         elif opt in ('-h', '--help'):
             help_message()
             sys.exit(0)
 
-        elif opt in ('-l', '--follow-symlinks'):         # NEW
+        elif opt in ('-l', '--follow-symlinks'):
             FOLLOW_LINKS = True
 
-        elif opt == "--no-print":         # NEW
+        elif opt == "--no-print":
             NO_PRINT = True
 
         elif opt in ('-q', '--qt-html'):
             HTML = True
 
         elif opt in ('-r', '--regex'):
             try:
@@ -582,15 +611,15 @@
                 REGEX_IN.append(reg)
             elif m == 'exclude':
                 REGEX_EX.append(reg)
             else:
                 err(f"Invalid regex option '{m}'. See 'dirtree --help'")
                 return 1
 
-        elif opt in ('-v', '--verbose'):         # NEW
+        elif opt in ('-v', '--verbose'):
             try:
                 if arg.lower() in ( '1', 'debug' ):
                     log.set_format( 'debug' )
                 else:
                     log.set_level( int(arg) )
             except TypeError:
                 err("Verbosity must be a number 1-5 <or> 'debug'")
@@ -602,23 +631,23 @@
     x = DirTree( BASE_DIR,
                  DEPTH,
                  dotfiles = DOTFILES,
                  exclude_dirs = EXCLUDE_DIRS,
                  exclude_files = EXCLUDE_FILES,
                  regex_ex = REGEX_EX,
                  regex_in = REGEX_IN,
-                 follow_links = FOLLOW_LINKS,         # NEW
-                 ignore_errors = IGNORE_ERRORS  )         # NEW
+                 follow_links = FOLLOW_LINKS,
+                 ignore_errors = IGNORE_ERRORS  )
 
     if HTML:
         to_print = x.list_gui()
     else:
         to_print = x.list_tty()
 
-    if NO_PRINT:            # NEW
+    if NO_PRINT:
         return 0
 
     print(to_print)
     return 0
 
 if __name__ == "__main__":
     sys.exit( main() )
```

### Comparing `bb_dirtree-0.3.1/pyproject.toml` & `bb_dirtree-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.3.1"
+version = "0.3.2"
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
-bb-apputils = "^0.3.8"
+bb-apputils = "^0.3.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bb_dirtree-0.3.1/PKG-INFO` & `bb_dirtree-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.3.1
+Version: 0.3.2
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
-Requires-Dist: bb-apputils (>=0.3.8,<0.4.0)
+Requires-Dist: bb-apputils (>=0.3.9,<0.4.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Description-Content-Type: text/markdown
 
 <style> table { text-align: center; } </style>
 
 # DirTree
 
@@ -178,7 +178,14 @@
 - updated README to reflect changes
 - cleaned up some code
 
 #### v0.3.1 - 7-15-2023
 
 - fixed title when printing to tty
 
+#### v0.3.2 - 7-15-2023
+
+- added colorized tree for symlinked directories
+- prevent symlinks from causing infinite recursion
+    - colored recursive directory links red
+- moved formatting code to class instances
+
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: bb-dirtree Version: 0.3.1 Summary: Create a nice
+Metadata-Version: 2.1 Name: bb-dirtree Version: 0.3.2 Summary: Create a nice
 looking directory tree with options License: MIT Keywords: script,qt,files
 Author: Erik Beebe Author-email: beebeapps_feedback@tuta.io Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: bb-
-apputils (>=0.3.8,<0.4.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
+apputils (>=0.3.9,<0.4.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
 Content-Type: text/markdown
  # DirTree -------------------------------------------- ##### Create a nice
 looking directory tree -------------------------------------------- ##
 Installation: ```bash python -m pip install "BB-DirTree" ``` ## DirTree usage
 ```bash dirtree [OPTIONS] [ARGS] ``` ### _**Options:**_ **Short** | **Long** |
 **Description** ---------- | ---------------------- | -------------------------
 -------------------------------- -b | --base-dir | Set base directory
@@ -74,8 +74,11 @@
 7-10-2023 - fixed typo in __main__ #### v0.2.6 - 7-10-2023 - bugfixes ####
 v0.3.0 - 7-15-2023 - added bb_apputils to dependencies - added bblogger for
 logging - removed __doc__ from init.py - added verbose options - added option
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
 README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
-fixed title when printing to tty
+fixed title when printing to tty #### v0.3.2 - 7-15-2023 - added colorized tree
+for symlinked directories - prevent symlinks from causing infinite recursion -
+colored recursive directory links red - moved formatting code to class
+instances
```

