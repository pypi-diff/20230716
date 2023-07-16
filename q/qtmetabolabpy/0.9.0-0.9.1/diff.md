# Comparing `tmp/qtmetabolabpy-0.9.0.tar.gz` & `tmp/qtmetabolabpy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.9.0.tar", last modified: Sun Jul 16 14:36:48 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.9.1.tar", last modified: Sun Jul 16 20:09:30 2023, max compression
```

## Comparing `qtmetabolabpy-0.9.0.tar` & `qtmetabolabpy-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.636703 qtmetabolabpy-0.9.0/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)      364 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/MANIFEST.in
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-16 14:36:48.636572 qtmetabolabpy-0.9.0/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.631636 qtmetabolabpy-0.9.0/qtmetabolabpy/
--rw-r--r--   0 ludwigc    (501) staff       (20)      210 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc    (501) staff       (20)     4987 2023-07-14 21:37:30.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634344 qtmetabolabpy-0.9.0/qtmetabolabpy/bash/
--rwxr-xr-x   0 ludwigc    (501) staff       (20)      556 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/bash/fix_pyside2
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634592 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634928 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc    (501) staff       (20)      884 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc    (501) staff       (20)        9 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.635244 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc    (501) staff       (20)        0 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Icon
--rwxr-xr-x   0 ludwigc    (501) staff       (20)   376356 2023-07-14 15:26:36.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/qtMetaboLabPy.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.635754 qtmetabolabpy-0.9.0/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc    (501) staff       (20)   242944 2023-07-14 21:07:45.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634209 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      607 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      119 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      321 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/requirements.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-07-16 14:36:48.636744 qtmetabolabpy-0.9.0/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.642557 qtmetabolabpy-0.9.1/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.1/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-16 20:09:30.642385 qtmetabolabpy-0.9.1/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.639481 qtmetabolabpy-0.9.1/qtmetabolabpy/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      210 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.641083 qtmetabolabpy-0.9.1/qtmetabolabpy/bash/
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/bash/fix_pyside2
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.641331 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.641641 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.641812 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Icon
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079   376356 2023-07-14 16:04:48.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/qtMetaboLabPy.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.642098 qtmetabolabpy-0.9.1/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079   243141 2023-07-16 20:05:39.000000 qtmetabolabpy-0.9.1/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-16 20:09:30.640972 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      607 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       62 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      119 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       14 2023-07-16 20:09:30.000000 qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      321 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-16 20:09:30.642593 qtmetabolabpy-0.9.1/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.1/setup.py
```

### Comparing `qtmetabolabpy-0.9.0/LICENSE` & `qtmetabolabpy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/PKG-INFO` & `qtmetabolabpy-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.0/README.rst` & `qtmetabolabpy-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.9.1/qtmetabolabpy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,18 @@
     screen_width = app.desktop().screenGeometry().width()
     screen_height = app.desktop().screenGeometry().height()
     w_width = 1600 #w.w.size().width()
     w_height = w.w.size().height()
     ww = min(w_width, screen_width)
     wh = min(w_height, screen_height)
     w.show()
-    w.w.showNormal()
-    w.w.move(0, 0)
+    if ww < 1300:
+        w.w.showNormal()
+        w.w.move(0, 0)
+
     app.processEvents()
     if w_width > screen_width:
         w.w.setMaximumWidth(screen_width)
         app.processEvents()
 
     if w_height > screen_height:
         w.w.setMaximumWidth(screen_height)
```

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/bash/fix_pyside2` & `qtmetabolabpy-0.9.1/qtmetabolabpy/bash/fix_pyside2`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.9.1/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/qtMetaboLabPy.py` & `qtmetabolabpy-0.9.1/qtmetabolabpy/qtMetaboLabPy.py`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.1/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files 0% similar despite different names*

#### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.1/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

```diff
@@ -198,15 +198,15 @@
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="currentIndex">
-              <number>1</number>
+              <number>0</number>
             </property>
             <widget class="QWidget" name="spcTab">
               <attribute name="title">
                 <string>NMR Spectrum</string>
               </attribute>
               <layout class="QGridLayout" name="gridLayout_26">
                 <item row="0" column="0">
@@ -3067,17 +3067,23 @@
                               <widget class="QFrame" name="peakSelection">
                                 <property name="sizePolicy">
                                   <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                     <horstretch>0</horstretch>
                                     <verstretch>40</verstretch>
                                   </sizepolicy>
                                 </property>
+                                <property name="minimumSize">
+                                  <size>
+                                    <width>400</width>
+                                    <height>0</height>
+                                  </size>
+                                </property>
                                 <property name="maximumSize">
                                   <size>
-                                    <width>500</width>
+                                    <width>600</width>
                                     <height>100</height>
                                   </size>
                                 </property>
                                 <property name="frameShape">
                                   <enum>QFrame::StyledPanel</enum>
                                 </property>
                                 <property name="frameShadow">
@@ -6557,15 +6563,15 @@
     </widget>
     <widget class="QMenuBar" name="menuBar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1914</width>
-          <height>22</height>
+          <height>43</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionSave"/>
```

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.9.1/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.0/setup.py` & `qtmetabolabpy-0.9.1/setup.py`

 * *Files identical despite different names*

