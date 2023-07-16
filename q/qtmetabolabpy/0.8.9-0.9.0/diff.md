# Comparing `tmp/qtmetabolabpy-0.8.9.tar.gz` & `tmp/qtmetabolabpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.8.9.tar", last modified: Thu Feb 16 14:19:26 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.9.0.tar", last modified: Sun Jul 16 14:36:48 2023, max compression
```

## Comparing `qtmetabolabpy-0.8.9.tar` & `qtmetabolabpy-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.473433 qtmetabolabpy-0.8.9/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2022-10-18 16:45:07.000000 qtmetabolabpy-0.8.9/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)      311 2022-10-18 18:34:32.000000 qtmetabolabpy-0.8.9/MANIFEST.in
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-16 14:19:26.473235 qtmetabolabpy-0.8.9/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2022-10-18 16:44:50.000000 qtmetabolabpy-0.8.9/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.464948 qtmetabolabpy-0.8.9/qtmetabolabpy/
--rw-r--r--   0 ludwigc    (501) staff       (20)      210 2022-12-12 19:03:28.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc    (501) staff       (20)   370456 2023-02-16 14:09:43.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.467090 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.469274 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc    (501) staff       (20)      884 2022-10-18 18:24:17.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc    (501) staff       (20)        9 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.469778 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc    (501) staff       (20)        0 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Icon
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.472853 qtmetabolabpy-0.8.9/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc    (501) staff       (20)   241807 2023-02-12 22:56:40.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.466951 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      545 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      119 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      321 2022-11-17 22:52:22.000000 qtmetabolabpy-0.8.9/requirements.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-02-16 14:19:26.473482 qtmetabolabpy-0.8.9/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2022-10-18 18:11:50.000000 qtmetabolabpy-0.8.9/setup.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.636703 qtmetabolabpy-0.9.0/
+-rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/LICENSE
+-rw-r--r--   0 ludwigc    (501) staff       (20)      364 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/MANIFEST.in
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-16 14:36:48.636572 qtmetabolabpy-0.9.0/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/README.rst
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.631636 qtmetabolabpy-0.9.0/qtmetabolabpy/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      210 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)     4987 2023-07-14 21:37:30.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634344 qtmetabolabpy-0.9.0/qtmetabolabpy/bash/
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)      556 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/bash/fix_pyside2
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634592 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634928 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      884 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc    (501) staff       (20)        9 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.635244 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc    (501) staff       (20)        0 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Icon
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)   376356 2023-07-14 15:26:36.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/qtMetaboLabPy.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.635754 qtmetabolabpy-0.9.0/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   242944 2023-07-14 21:07:45.000000 qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-16 14:36:48.634209 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)      607 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)      119 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-07-16 14:36:48.000000 qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)      321 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/requirements.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-07-16 14:36:48.636744 qtmetabolabpy-0.9.0/setup.cfg
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.0/setup.py
```

### Comparing `qtmetabolabpy-0.8.9/LICENSE` & `qtmetabolabpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.9/PKG-INFO` & `qtmetabolabpy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.8.9/README.rst` & `qtmetabolabpy-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.9.0/qtmetabolabpy/qtMetaboLabPy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,80 @@
 #!/usr/bin/env ython
 import sys  # pragma: no cover
 import matplotlib  # pragma: no cover
-import inspect
+import inspect   # pragma: no cover
+import importlib   # pragma: no cover
+
+matplotlib.use("Agg")  # pragma: no cover
+matplotlib.rcParams['agg.path.chunksize'] = 64000  # pragma: no cover
+## matplotlib.rc('xtick', labelsize=8)
+## matplotlib.rc('ytick', labelsize=8)
+import platform  # pragma: no cover
+import os  # pragma: no cover
+
 
-matplotlib.use("Agg")
-matplotlib.rcParams['agg.path.chunksize'] = 64000  # 64_000_000_000
-# matplotlib.rc('xtick', labelsize=8)
-# matplotlib.rc('ytick', labelsize=8)
 
 try:
     from PySide2.QtUiTools import QUiLoader  # pragma: no cover
     from PySide2.QtCore import QFile  # pragma: no cover
     from PySide2.QtCore import QCoreApplication  # pragma: no cover
     from PySide2.QtWidgets import *  # pragma: no cover
     from PySide2 import QtWidgets  # pragma: no cover
     from PySide2.QtGui import *  # pragma: no cover
     from PySide2 import QtGui  # pragma: no cover
     from PySide2 import QtCore  # pragma: no cover
     from PySide2.QtWidgets import QFileDialog  # pragma: no cover
     from PySide2 import QtWidgets  # pragma: no cover
     from PySide2.QtCore import SIGNAL  # pragma: no cover
-    from PySide2.QtWebEngineWidgets import QWebEngineView  # , QWebEngineProfile, QWebEnginePage, \
-    #    QWebEngineSettings  # pragma: no cover
     from PySide2.QtCore import QUrl, Qt  # pragma: no cover
-    from PySide2.QtWebEngineCore import QWebEngineUrlSchemeHandler  # pragma: no cover
     import PySide2  # pragma: no cover
     import qtmodern.styles  # pragma: no cover
     from PySide2.QtGui import QPixmap
 except:
     pass
 
+try:
+    from PySide2.QtWebEngineWidgets import QWebEngineView, QWebEngineSettings  # pragma: no cover
+    from PySide2.QtWebEngineCore import QWebEngineUrlSchemeHandler  # pragma: no cover
+except:
+    if platform.system() == 'Darwin' and platform.machine() == 'arm64':  # pragma: no cover
+        find_pyside2 = importlib.util.find_spec('PySide2')  # pragma: no cover
+        if find_pyside2.__str__() == None:  # pragma: no cover
+            print('PySide2 not installed!')  # pragma: no cover
+            sys.exit()  # pragma: no cover
+        else:  # pragma: no cover
+            script_name = os.path.join(os.path.dirname(__file__), 'bash', 'fix_pyside2')  # pragma: no cover
+            print('Error: Could not load QWebEngineView')  # pragma: no cover
+            answer = input("Do you want to fix the issue automatically (y, n) or display the fixing bash script (d)? [y, n, d]: ")  # pragma: no cover
+            while answer not in ['y', 'Y', 'n', 'N', 'd', 'D']:  # pragma: no cover
+                print('Please input y, n or d only')  # pragma: no cover
+                answer = input("Do you want to fix the issue automatically (y, n) or display the fixing bash script (d)? [y, n, d]: ")  # pragma: no cover
+
+            if answer in ['n', 'N']:  # pragma: no cover
+                print('Good luck!')  # pragma: no cover
+                sys.exit()  # pragma: no cover
+
+            if answer in ['d', 'D']:  # pragma: no cover
+                print('\n=== Bash script to fix the issue ========================================================\n')  # pragma: no cover
+                os.system('cat ' + script_name)  # pragma: no cover
+                print('\n=== End of bash script ==================================================================\n')  # pragma: no cover
+                while answer not in ['y', 'Y', 'n', 'N']:  # pragma: no cover
+                    answer = input("Do you want to fix the issue automatically? [y, n]: ")  # pragma: no cover
+                    if answer not in ['y', 'Y', 'n', 'N']:  # pragma: no cover
+                        print('Please input y or n only')  # pragma: no cover
+
+            if answer in ['n', 'N']:  # pragma: no cover
+                print('Good luck!')  # pragma: no cover
+                sys.exit()  # pragma: no cover
+
+            print('Fixing issue (PySide2/Darwin arm64 anaconda3)...')  # pragma: no cover
+            os.system(script_name)  # pragma: no cover
+            print('Fixed M1/M2 mac arm64 anaconda PySide2 issue, please start qtmetabolabpy again!')  # pragma: no cover
+            sys.exit()  # pragma: no cover
+
 import darkdetect
 import webbrowser
 import pandas as pd
 #import matplotlib.pyplot as pl  # pragma: no cover
 
 if "linux" in sys.platform:  # pragma: no cover
     gui_env = ['TkAgg', 'GTKAgg', 'Qt5Agg', 'WXAgg']  # pragma: no cover
@@ -75,19 +116,18 @@
 from metabolabpy.nmr import nmrDataSet  # pragma: no cover
 from metabolabpy.GUI import phCorr  # pragma: no cover
 from metabolabpy.nmr import nmrHsqc  # pragma: no cover
 import time  # pragma: no cover
 ##import platform  # pragma: no cover
 import math  # pragma: no cover
 from metabolabpy.nmr import nmrConfig  # pragma: no cover
-import os  # pragma: no cover
 import traceback  # pragma: no cover
 import shutil  # pragma: no cover
 import scipy.io  # pragma: no cover
-##import inspect
+#import inspect
 from io import StringIO
 import contextlib
 import zipfile
 from collections import defaultdict
 from notebook import notebookapp
 import multiprocess
 import subprocess
@@ -250,29 +290,30 @@
             print("QWebEngineView2")
 
     # ------------------ QWebEngineView2 -------------
 except:
     pass
 
 
-class main_w(object):  # pragma: no cover
+class QtMetaboLabPy(object):  # pragma: no cover
     def __init__(self):
         self.exited_peak_picking = False
         self.zoom_was_on = True
         self.pan_was_on = False
         self.std_pos_col1 = (0.0, 0.0, 1.0)
         self.std_neg_col1 = (1.0, 0.0, 0.0)
         self.std_pos_col2 = (0.8, 0.8, 1.0)
         self.std_neg_col2 = (1.0, 0.8, 0.8)
         self.n_clicks = 1
         self.cur_clicks = 0
         self.xy = [[]]
         self.xdata = []
         self.ydata = []
         self.temp_shift = 0.0
+        self.find_maximum = True
         self.nd = nmrDataSet.NmrDataSet()
         self.__version__ = self.nd.__version__
         self.ph_corr = phCorr.PhCorr()
         # load ui; create w
         f_name = os.path.join(os.path.dirname(__file__), "ui", "metabolabpy_mainwindow.ui")
         self.file = QFile(f_name)
         self.file.open(QFile.ReadOnly)
@@ -290,15 +331,15 @@
         self.hide_peak_picking()
         self.w.preprocessing.setVisible(False)
         self.w.splinebaseline.setVisible(False)
         self.w.peakPicking.setVisible(False)
         self.w.preProcPeak.setVisible(False)
         self.w.hsqcAnalysis.setVisible(False)
         self.w.multipletAnalysis.setVisible(False)
-        self.w.isotopomerAnalysis.setVisible(False)
+        #self.w.isotopomerAnalysis.setVisible(False)
         self.w.nmrSpectrum.setTabEnabled(1, False)
         self.w.nmrSpectrum.setTabEnabled(2, False)
         self.w.nmrSpectrum.setTabEnabled(3, False)
         self.w.nmrSpectrum.setTabEnabled(4, False)
         self.w.nmrSpectrum.setStyleSheet(
             "QTabBar::tab::disabled {width: 0; height: 0; margin: 0; padding: 0; border: none;} ")
         # connections
@@ -365,59 +406,58 @@
         self.w.compressAddButton.clicked.connect(self.select_add_compress_pre_proc)
         self.w.selectAllButton.clicked.connect(self.select_all_pre_proc)
         self.w.selectEvenButton.clicked.connect(self.select_even_pre_proc)
         self.w.selectOddButton.clicked.connect(self.select_odd_pre_proc)
         self.w.selectClassButton.clicked.connect(self.select_class_pre_proc)
         self.w.selectClassLE.textChanged.connect(self.select_class_pre_proc)
         self.w.cmdLine.returnPressed.connect(self.exec_cmd)
-        self.w.noiseThresholdLE.textChanged.connect(self.set_noise_reg_pre_proc)
-        self.w.noiseRegionStartLE.textChanged.connect(self.set_noise_reg_pre_proc)
-        self.w.noiseRegionEndLE.textChanged.connect(self.set_noise_reg_pre_proc)
-        self.w.thLineWidthLE.textChanged.connect(self.set_noise_reg_pre_proc)
-        self.w.bucketPpmLE.textChanged.connect(self.set_bucket_ppm_pre_proc)
-        self.w.bucketDataPointsLE.textChanged.connect(self.set_bucket_points_pre_proc)
+        self.w.noiseThresholdLE.returnPressed.connect(self.set_noise_reg_pre_proc)
+        self.w.noiseRegionStartLE.returnPressed.connect(self.set_noise_reg_pre_proc)
+        self.w.noiseRegionEndLE.returnPressed.connect(self.set_noise_reg_pre_proc)
+        self.w.thLineWidthLE.returnPressed.connect(self.set_noise_reg_pre_proc)
+        self.w.bucketPpmLE.returnPressed.connect(self.set_bucket_ppm_pre_proc)
+        self.w.bucketDataPointsLE.returnPressed.connect(self.set_bucket_points_pre_proc)
         self.w.actionAutomatic_Referencing.triggered.connect(self.automatic_referencing)
         self.w.actionVertical_AutoScale.triggered.connect(self.vertical_auto_scale)
         self.w.actionHorizontal_AutoScale.triggered.connect(self.horizontal_auto_scale)
         self.w.actionZoom.triggered.connect(self.set_zoom)
         self.w.actionPan.triggered.connect(self.set_pan)
         self.w.actionShow_Next_Tab.triggered.connect(self.next_tab)
         self.w.actionShow_Previous_Tab.triggered.connect(self.previous_tab)
         self.w.actionPlot_spc.triggered.connect(self.plot_spc)
         self.w.actionSave.triggered.connect(self.save_button)
         self.w.actionLoad.triggered.connect(self.load_button)
-
         self.w.actionOpen_NMRPipe.triggered.connect(self.read_nmrpipe_spc)
         self.w.actionActivate_Command_Line.triggered.connect(self.activate_command_line)
         self.w.actionPrevious_command.triggered.connect(self.previous_command)
         self.w.actionNext_command.triggered.connect(self.next_command)
         self.w.actionCorrect_Phase.triggered.connect(self.start_stop_ph_corr)
         self.w.actionUpdate_MetaboLabPy_requires_restart.triggered.connect(self.update_metabolabpy)
         # self.w.actionZoomCorrect_Phase.triggered.connect(self.zoom_ph_corr)
         self.w.maResetButton.clicked.connect(self.hsqc_spin_sys_reset)
         self.w.zoomPhCorr1d.clicked.connect(self.zoom_ph_corr)
         self.w.exitZoomPhCorr1d.clicked.connect(self.zoom_ph_corr)
         self.w.exitPhCorr1d.clicked.connect(self.start_stop_ph_corr)
         self.w.actionClear.triggered.connect(self.clear)
-        self.w.lambdaLE.textChanged.connect(self.set_var_lambda)
-        self.w.y0LE.textChanged.connect(self.set_var_y0)
+        self.w.lambdaLE.returnPressed.connect(self.set_var_lambda)
+        self.w.y0LE.returnPressed.connect(self.set_var_y0)
         self.w.actionRead_NMR_Spectrum.triggered.connect(self.read_nmr_spc)
         self.w.preprocessing.stateChanged.connect(self.set_pre_processing)
         self.w.peakPicking.stateChanged.connect(self.set_peak_picking)
         self.w.splinebaseline.stateChanged.connect(self.set_spline_baseline)
         self.w.peakAddButton.clicked.connect(self.add_peak)
         self.w.peakClearButton.clicked.connect(self.clear_peak)
         self.w.peakWidget.cellChanged.connect(self.set_add_peak)
         self.w.peakExportButton.clicked.connect(self.export_peak)
         self.w.intAllDS.stateChanged.connect(self.set_datasets_exps)
         self.w.intAllExps.stateChanged.connect(self.set_datasets_exps)
         self.w.exportFormatCB.currentIndexChanged.connect(self.set_datasets_exps)
         self.w.hsqcAnalysis.stateChanged.connect(self.set_hsqc_analysis)
         self.w.multipletAnalysis.stateChanged.connect(self.set_multiplet_analysis)
-        self.w.isotopomerAnalysis.stateChanged.connect(self.set_isotopomer_analysis)
+        #self.w.isotopomerAnalysis.stateChanged.connect(self.set_isotopomer_analysis)
         self.w.preserveOverallScale.stateChanged.connect(self.set_preserve_overall_scale)
         self.w.actionReset.triggered.connect(self.reset_plot)
         self.w.actionShow_NMR_Spectrum.triggered.connect(self.show_nmr_spectrum)
         self.w.actionSetup_Processing_Parameters.triggered.connect(self.setup_processing_parameters)
         self.w.actionShow_Display_Parameters.triggered.connect(self.show_display_parameters)
         self.w.actionShow_Acquisition_Parameters.triggered.connect(self.show_acquisition_parameters)
         self.w.actionShow_Title_File_Information.triggered.connect(self.show_title_file_information)
@@ -530,15 +570,15 @@
         self.show_version()
         self.keep_zoom = False
         self.keep_x_zoom = False
         self.ph_corr_active = False
         self.set_font_size()
         self.cf = nmrConfig.NmrConfig()
         self.cf.read_config()
-        self.w.autoPlot.setChecked(self.cf.auto_plot)
+        #self.w.autoPlot.setChecked(self.cf.auto_plot)
         self.w.keepZoom.setChecked(self.cf.keep_zoom)
         self.w.fontSize.setValue(self.cf.font_size)
         self.std_pos_col1 = (self.cf.pos_col10, self.cf.pos_col11, self.cf.pos_col12)
         self.std_neg_col1 = (self.cf.neg_col10, self.cf.neg_col11, self.cf.neg_col12)
         self.std_pos_col2 = (self.cf.pos_col20, self.cf.pos_col21, self.cf.pos_col22)
         self.std_neg_col2 = (self.cf.neg_col20, self.cf.neg_col21, self.cf.neg_col22)
         self.w.actionSave_as_Default.triggered.connect(self.save_config)
@@ -558,14 +598,16 @@
         self.w.iSpc_p4.textChanged.connect(self.get_i_spc_p4)
         self.w.iSpc_p5.textChanged.connect(self.get_i_spc_p5)
         self.w.iSpc_p6.textChanged.connect(self.get_i_spc_p6)
         self.set_font_size()
         self.w.MplWidget.toolbar.setVisible(False)
         self.w.hsqcMultiplet.toolbar.setVisible(False)
         self.w.hsqcPeak.toolbar.setVisible(False)
+        self.w.startNotebookButton.setVisible(False)
+        self.w.stopNotebookButton.setVisible(False)
         # self.w.isotopomerHsqcPeak.toolbar.setVisible(False)
         # self.w.isotopomerMultiplet.toolbar.setVisible(False)
         self.w.MplWidget.setFocus()
         self.set_zoom()
         self.w.pickRowColPhCorr2d.clicked.connect(self.pick_col_row)
         self.w.emptyRowColPhCorr2d.clicked.connect(self.empty_col_row)
         self.w.removeRowColPhCorr2d.clicked.connect(self.remove_last_col_row)
@@ -598,15 +640,15 @@
         self.w.actionreInitialise_plot_colours.triggered.connect(self.set_standard_plot_colours)
         self.w.clearAssignedHsqc.clicked.connect(self.clear_assigned_hsqc)
         self.w.displayMetaboliteInformation.clicked.connect(self.display_metabolite_information)
         self.w.hsqcAddPeak.clicked.connect(lambda: self.ginput_hsqc(0))
         self.w.hsqcRemovePeak.clicked.connect(lambda: self.ginput_hsqc2(0))
         self.w.metaboliteResetButton.clicked.connect(self.metabolite_reset)
         self.w.metaboliteAutoButton.clicked.connect(self.autopick_hsqc)
-        self.w.metaboliteAutofitButton.clicked.connect(self.ma_fit_hsqc_1d)
+        self.w.metaboliteAutofitButton.clicked.connect(self.autofit_hsqc)
         self.w.maSimButton.clicked.connect(self.ma_sim_hsqc_1d)
         self.buttons = {}
         # print(sys.platform)
         if sys.platform == 'darwin':
             self.w.actionCreate.setText('Create Launchpad Icon')
             self.w.actionCreate.triggered.connect(self.create_icon_mac)
         elif sys.platform == 'win' or sys.platform == 'win32' or sys.platform == 'win64':
@@ -653,29 +695,35 @@
 
     def autofit_hsqc(self, metabolite_list=False):
         if metabolite_list is False:
             metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
         elif len(metabolite_list[0]) == 0:
             metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
 
+        if self.w.maAutoScale.isChecked():
+            hsqc = self.nd.nmrdat[self.nd.s][self.nd.s].hsqc
+            for k in range(len(hsqc.hsqc_data[hsqc.cur_metabolite].intensities)):
+                self.nd.nmrdat[self.nd.s][self.nd.s].hsqc.hsqc_data[hsqc.cur_metabolite].intensities[k] = 1
+
+
         if len(metabolite_list[0]) == 0:
             return
 
         no_peak_selected = False
         if self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak == -1:
             no_peak_selected = True
             cur_peak = 1
         else:
             cur_peak = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak
 
         if self.w.hsqcAnalysis.isChecked() == False:
             self.w.hsqcAnalysis.setChecked(True)
             self.w.hsqcAnalysis.setChecked(False)
 
-        self.nd.nmrdat[self.nd.s][self.nd.e].autopick_hsqc(metabolite_list)
+        self.nd.nmrdat[self.nd.s][self.nd.e].autofit_hsqc(metabolite_list)
         for metabolite_name in metabolite_list:
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite = metabolite_name
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak = cur_peak
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.read_metabolite_information(metabolite_name)
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.set_metabolite_information(metabolite_name,
                                                                                  self.nd.nmrdat[self.nd.s][
                                                                                      self.nd.e].hsqc.metabolite_information)
@@ -693,14 +741,45 @@
             idx1 = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.metabolite_list.index(metabolite_list[0])
             self.w.hsqcMetabolites.setCurrentIndex(self.w.hsqcMetabolites.model().index(idx1, 0))
 
         self.set_hsqc_metabolite()
         self.plot_metabolite_peak(cur_peak)
         # end autofit_hsqc
 
+    def autofit_hsqc(self, metabolite_list=False):
+        if metabolite_list is False:
+            metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
+        elif len(metabolite_list[0]) == 0:
+            metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
+
+        if len(metabolite_list[0]) == 0:
+            return
+
+        if self.w.hsqcAnalysis.isChecked() == False:
+            self.w.hsqcAnalysis.setChecked(True)
+            self.w.hsqcAnalysis.setChecked(False)
+
+        no_peak_selected = False
+        if self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak == -1:
+            no_peak_selected = True
+            cur_peak = 1
+        else:
+            cur_peak = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak
+
+        self.nd.nmrdat[self.nd.s][self.nd.e].autofit_hsqc(metabolite_list)
+        if no_peak_selected:
+            self.w.hsqcAnalysis.setChecked(False)
+            self.w.hsqcAnalysis.setChecked(True)
+            idx1 = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.metabolite_list.index(metabolite_list[0])
+            self.w.hsqcMetabolites.setCurrentIndex(self.w.hsqcMetabolites.model().index(idx1, 0))
+
+        self.set_hsqc_metabolite()
+        self.plot_metabolite_peak(cur_peak)
+        # end autofit_hsqc
+
     def autopick_hsqc(self, metabolite_list=False):
         if metabolite_list is False:
             metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
         elif len(metabolite_list[0]) == 0:
             metabolite_list = [self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_metabolite]
 
         if len(metabolite_list[0]) == 0:
@@ -788,14 +867,15 @@
         self.show_ph_corr2d()
         self.set_proc_pars()
         self.show_acquisition_parameters()
         self.show_nmr_spectrum()
         # end apply_2d_ph_corr
 
     def autobaseline(self):
+        #print("autobaseline")
         #print(self.nd.nmrdat[self.nd.s][self.nd.e].dim)
         if self.nd.nmrdat[self.nd.s][self.nd.e].dim == 1:
             self.autobaseline1d()
         elif self.nd.nmrdat[self.nd.s][self.nd.e].dim == 2:
             self.autobaseline2d()
 
         # end autobaseline
@@ -810,15 +890,48 @@
             elif self.nd.nmrdat[self.nd.s][self.nd.e].dim == 2:
                 self.autobaseline2d()
 
         self.nd.e = ce
         self.plot_spc()
         # end autobaseline
 
-    def autobaseline1d(self):
+    def autobaseline1d(self, alg='jbcd', lam=1000000, max_iter=50, alpha=0.1, beta=10, gamma=15, beta_mult=0.98, gamma_mult=0.94, half_window=None):
+        code_out = io.StringIO()
+        code_err = io.StringIO()
+        sys.stdout = code_out
+        sys.stderr = code_err
+        self.show_auto_baseline()
+        self.nd.ft()
+        self.nd.auto_ref()
+        self.nd.autobaseline1d(alg=alg, lam=lam, max_iter=max_iter, alpha=alpha, beta=beta, gamma=gamma, beta_mult=beta_mult, gamma_mult=gamma_mult, half_window=half_window)
+        self.nd.auto_ref()
+        self.show_version()
+        self.w.nmrSpectrum.setCurrentIndex(0)
+        self.change_data_set_exp()
+        self.plot_spc(True)
+        self.nd.nmrdat[self.nd.s][self.nd.e].proc.autobaseline = True
+        self.set_autobaseline()
+        sys.stdout = sys.__stdout__
+        sys.stderr = sys.__stderr__
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            txt_col = QColor.fromRgbF(1.0, 1.0, 1.0, 1.0)
+            err_col = QColor.fromRgbF(1.0, 0.5, 0.5, 1.0)
+        else:
+            txt_col = QColor.fromRgbF(0.0, 0.0, 0.0, 1.0)
+            err_col = QColor.fromRgbF(1.0, 0.0, 0.0, 1.0)
+
+        self.w.console.setTextColor(txt_col)
+        self.w.console.append(code_out.getvalue())
+        self.w.console.setTextColor(err_col)
+        self.w.console.append(code_err.getvalue())
+        code_out.close()
+        code_err.close()
+        # end autobaseline1d
+
+    def autobaseline1d_old(self):
         code_out = io.StringIO()
         code_err = io.StringIO()
         sys.stdout = code_out
         sys.stderr = code_err
         self.show_auto_baseline()
         self.nd.ft()
         self.nd.auto_ref()
@@ -843,15 +956,15 @@
 
         self.w.console.setTextColor(txt_col)
         self.w.console.append(code_out.getvalue())
         self.w.console.setTextColor(err_col)
         self.w.console.append(code_err.getvalue())
         code_out.close()
         code_err.close()
-        # end autobaseline1d
+        # end autobaseline1d_old
 
     def autobaseline2d(self, poly_order=[16, 16], threshold=0.05):
         code_out = io.StringIO()
         code_err = io.StringIO()
         sys.stdout = code_out
         sys.stderr = code_err
         self.show_auto_baseline()
@@ -879,20 +992,22 @@
 
     def autobaseline1d_all(self):
         code_out = io.StringIO()
         code_err = io.StringIO()
         sys.stdout = code_out
         sys.stderr = code_err
         self.show_auto_baseline()
-        self.nd.ft()
-        self.nd.auto_ref()
+        self.nd.nmrdat[self.nd.s][self.nd.e].proc.autobaseline = True
+        self.set_autobaseline()
+        self.nd.ft_all()
+        self.nd.auto_ref_all()
         self.nd.autobaseline1d_all()
-        self.w.baselineCorrection.setCurrentIndex(1)
-        self.nd.ft()
-        self.nd.baseline1d()
+        #self.w.baselineCorrection.setCurrentIndex(1)
+        #self.nd.ft()
+        #self.nd.baseline1d()
         # self.w.baselineCorrection.setCurrentIndex(1)
         self.set_proc_pars()
         self.show_version()
         self.w.nmrSpectrum.setCurrentIndex(0)
         self.change_data_set_exp()
         self.plot_spc(True)
         sys.stdout = sys.__stdout__
@@ -909,46 +1024,46 @@
         self.w.console.setTextColor(err_col)
         self.w.console.append(code_err.getvalue())
         code_out.close()
         code_err.close()
         # end autobaseline1d_all
 
     def autophase1d(self):
-        code_out = io.StringIO()
-        code_err = io.StringIO()
-        sys.stdout = code_out
-        sys.stderr = code_err
+        #code_out = io.StringIO()
+        #code_err = io.StringIO()
+        #sys.stdout = code_out
+        #sys.stderr = code_err
         self.show_auto_phase()
         self.nd.ft()
         self.nd.auto_ref()
         self.nd.autophase1d()
         # self.w.baselineCorrection.setCurrentIndex(1)
         # self.nd.ft()
         # self.nd.baseline1d()
         # self.plot_spc()
         self.set_proc_pars()
         self.show_version()
         self.w.nmrSpectrum.setCurrentIndex(0)
         self.change_data_set_exp()
         self.plot_spc(True)
-        sys.stdout = sys.__stdout__
-        sys.stderr = sys.__stderr__
-        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
-            txt_col = QColor.fromRgbF(1.0, 1.0, 1.0, 1.0)
-            err_col = QColor.fromRgbF(1.0, 0.5, 0.5, 1.0)
-        else:
-            txt_col = QColor.fromRgbF(0.0, 0.0, 0.0, 1.0)
-            err_col = QColor.fromRgbF(1.0, 0.0, 0.0, 1.0)
-
-        self.w.console.setTextColor(txt_col)
-        self.w.console.append(code_out.getvalue())
-        self.w.console.setTextColor(err_col)
-        self.w.console.append(code_err.getvalue())
-        code_out.close()
-        code_err.close()
+        #sys.stdout = sys.__stdout__
+        #sys.stderr = sys.__stderr__
+        #if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+        #    txt_col = QColor.fromRgbF(1.0, 1.0, 1.0, 1.0)
+        #    err_col = QColor.fromRgbF(1.0, 0.5, 0.5, 1.0)
+        #else:
+        #    txt_col = QColor.fromRgbF(0.0, 0.0, 0.0, 1.0)
+        #    err_col = QColor.fromRgbF(1.0, 0.0, 0.0, 1.0)
+
+        #self.w.console.setTextColor(txt_col)
+        #self.w.console.append(code_out.getvalue())
+        #self.w.console.setTextColor(err_col)
+        #self.w.console.append(code_err.getvalue())
+        #code_out.close()
+        #code_err.close()
         # end autophase1d
 
     def autophase1d_all(self):
         code_out = io.StringIO()
         code_err = io.StringIO()
         sys.stdout = code_out
         sys.stderr = code_err
@@ -1107,31 +1222,35 @@
                     self.w.setBox.setValue(len(self.nd.nmrdat))
 
                 self.nd.s = self.w.setBox.value() - 1
                 if (self.w.expBox.value() > len(self.nd.nmrdat[self.nd.s])):
                     self.w.expBox.setValue(len(self.nd.nmrdat[self.nd.s]))
 
                 self.nd.e = self.w.expBox.value() - 1
+                if len(self.nd.nmrdat) > (self.nd.s + 1):
+                    if self.nd.nmrdat[self.nd.s][old_exp].display.display_spc != True and self.nd.nmrdat[self.nd.s+1][old_exp].display.display_spc == True:
+                        self.nd.nmrdat[self.nd.s+1][old_exp].display.display_spc = False
+                        self.nd.nmrdat[self.nd.s+1][self.nd.e].display.display_spc = True
                 keep_zoom = self.w.keepZoom.isChecked()
                 if not ((old_set == self.nd.s) and (old_exp == self.nd.e)):
                     if (self.nd.nmrdat[old_set][old_exp].dim != self.nd.nmrdat[self.nd.s][self.nd.e].dim):
                         self.keep_x_zoom = True
                         self.keep_zoom = False
                         self.w.keepZoom.setChecked(False)
 
                     self.set_disp_pars()
                     self.set_proc_pars()
                     self.set_acq_pars()
                     self.set_title_file()
                     self.set_pulse_program()
                     if (self.ph_corr_active == False):
-                        if (self.w.autoPlot.isChecked()):
-                            self.plot_spc(True)
-                        elif (self.w.nmrSpectrum.currentIndex() == 0):
-                            self.plot_spc(True)
+                        #if (self.w.autoPlot.isChecked()):
+                        #    self.plot_spc(True)
+                        #elif (self.w.nmrSpectrum.currentIndex() == 0):
+                        self.plot_spc(True)
 
                     else:
                         if self.nd.nmrdat[self.nd.s][self.nd.e].dim == 1:
                             self.ph_corr.spc = self.nd.nmrdat[self.nd.s][self.nd.e].spc
                             self.ph_corr_plot_spc()
                         else:
                             self.plot_spc(True)
@@ -1434,14 +1553,17 @@
 
         self.plot_spc(True)
         # end corr_spline_baseline
 
     def create_icon_mac(self):
         home_dir = os.path.expanduser('~')
         app_dir2 = os.path.join(home_dir, 'Applications')
+        if not os.path.isdir(app_dir2):
+            os.makedirs(app_dir2)
+
         app_dir = os.path.join(app_dir2, 'QtMetaboLabPy.app')
         app_dir1 = 'QtMetaboLabPy'
         try:
             shutil.rmtree(app_dir)
         except:
             pass
 
@@ -1457,20 +1579,20 @@
         os.chmod(appify, 0o777)
         ml_starter = os.path.join(os.path.dirname(__file__), 'mlStarter')
         contents = os.path.join(ml_starter, 'Contents')
         icon = os.path.join(ml_starter, 'Icon')
         starter = os.path.join(app_dir2, 'createStarter')
         f = open(starter, 'w')
         f.write('#!/usr/bin/env bash\n\n')
-        f.write(appify + ' $(which qtmetabolabpy) ' + app_dir2 + ' ' + app_dir1 + '\n')
-        f.write('cp -r ' + contents + ' ' + app_dir + '\n')
-        f.write("cp " + icon + " " + app_dir + "/Icon$'\\r'\n")
+        f.write(appify.replace(' ', '\ ') + ' $(which qtmetabolabpy) ' + app_dir2.replace(' ', '\ ') + ' ' + app_dir1.replace(' ', '\ ') + '\n')
+        f.write('cp -r ' + contents.replace(' ', '\ ') + ' ' + app_dir.replace(' ', '\ ') + '\n')
+        f.write("cp " + icon.replace(' ', '\ ') + " " + app_dir.replace(' ', '\ ') + "/Icon$'\\r'\n")
         f.close()
         os.chmod(starter, 0o777)
-        subprocess.os.system(starter)
+        subprocess.os.system(starter.replace(' ', '\ '))
         os.remove(appify)
         os.remove(starter)
         # end create_icon_mac
 
     def create_icon_linux(self):
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
@@ -3062,15 +3184,21 @@
         self.nd.nmrdat[self.nd.s][self.nd.e].proc = p
         # end get_proc_pars25
 
     def get_proc_pars26(self):
         p = self.nd.nmrdat[self.nd.s][self.nd.e].proc
         p.strip_end = int(self.w.stripTransformEnd.text())
         self.nd.nmrdat[self.nd.s][self.nd.e].proc = p
-        # end get_proc_pars25
+        # end get_proc_pars26
+
+    def get_proc_pars27(self):
+        p = self.nd.nmrdat[self.nd.s][self.nd.e].proc
+        p.autobaseline = self.w.autobaselineBox.isChecked()
+        self.nd.nmrdat[self.nd.s][self.nd.e].proc = p
+        # end get_proc_pars27
 
     def get_bottom_top(self, line):
         margin = 0.1
         xd = line.get_xdata()
         yd = line.get_ydata()
         lo, hi = self.w.MplWidget.canvas.axes.get_xlim()
         y_displayed = yd[((xd > min(lo, hi)) & (xd < max(lo, hi)))]
@@ -3708,15 +3836,15 @@
         self.w.correctAllButton.setHidden(True)
         # end hide_spline_baseline
 
     def html(self, url=''):
         if len(url) == 0:
             nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
             base_dir = os.path.split(nmr_dir)[0]
-            f_name = os.path.join(base_dir, "nmr", "web", "introductionDark", "index.html")
+            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
             url = "file:///" + f_name.replace('\\', '/')
 
         self.w.helpView.setUrl(url)
         self.w.nmrSpectrum.setCurrentIndex(12)
         # end html
 
     def show_peak_picking(self):
@@ -3961,15 +4089,15 @@
             self.w.maAutoSim.setChecked(False)
 
         # end load_button
 
     def load_config(self):
         self.cf.read_config()
         self.w.phRefColour.setCurrentIndex(self.nd.nmrdat[0][0].display.colours2.get(self.cf.phase_reference_colour))
-        self.w.autoPlot.setChecked(self.cf.auto_plot)
+        #self.w.autoPlot.setChecked(self.cf.auto_plot)
         self.w.keepZoom.setChecked(self.cf.keep_zoom)
         self.w.fontSize.setValue(self.cf.font_size)
         self.std_pos_col1 = (self.cf.pos_col10, self.cf.pos_col11, self.cf.pos_col12)
         self.std_neg_col1 = (self.cf.neg_col10, self.cf.neg_col11, self.cf.neg_col12)
         self.std_pos_col2 = (self.cf.pos_col20, self.cf.pos_col21, self.cf.pos_col22)
         self.std_neg_col2 = (self.cf.neg_col20, self.cf.neg_col21, self.cf.neg_col22)
         self.set_standard_colours()
@@ -4008,15 +4136,15 @@
             self.nd.nmrdat[self.nd.s][k].display.pos_col_rgb = self.std_pos_col2
             self.nd.nmrdat[self.nd.s][k].display.neg_col_rgb = self.std_neg_col2
 
         idx = self.w.helpComboBox.currentIndex()
         url = []
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
-        f_name = os.path.join(base_dir, "nmr", "web", "introductionDark", "index.html")
+        f_name = os.path.join(base_dir, "nmr", "web", "index.html")
         url.append("file:///" + f_name.replace('\\', '/'))
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
@@ -4103,15 +4231,15 @@
             self.nd.nmrdat[self.nd.s][k].display.pos_col_rgb = self.std_pos_col1
             self.nd.nmrdat[self.nd.s][k].display.neg_col_rgb = self.std_neg_col1
 
         idx = self.w.helpComboBox.currentIndex()
         url = []
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
-        f_name = os.path.join(base_dir, "nmr", "web", "introduction", "index.html")
+        f_name = os.path.join(base_dir, "nmr", "web", "index.html")
         url.append("file:///" + f_name.replace('\\', '/'))
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
@@ -4681,15 +4809,22 @@
                                                   self.nd.nmrdat[d.ph_ref_ds - 1][d.ph_ref_exp - 1].spc[0].real,
                                                   color=ref_col)
 
             self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[self.nd.s][self.nd.e].ppm1, self.ph_corr.spc[0].real,
                                               color=pos_col)
             self.w.MplWidget.canvas.axes.plot([self.ph_corr.pivot, self.ph_corr.pivot],
                                               [2.0 * self.ph_corr.spc_max, -2.0 * self.ph_corr.spc_max], color='r')
-            self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
+            if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+                bg = (42 / 255, 42 / 255, 42 / 255)
+                fg = (255 / 255, 255 / 255, 255 / 255)
+            else:
+                bg = (255 / 255, 255 / 255, 255 / 255)
+                fg = (0 / 255, 0 / 255, 0 / 255)
+
+            self.w.MplWidget.canvas.axes.set_xlabel(xlabel, color=fg)
             self.w.MplWidget.canvas.axes.invert_xaxis()
             self.w.MplWidget.canvas.axes.set_xlim(xlim)
             self.w.MplWidget.canvas.axes.set_ylim(ylim)
 
         self.set_proc_pars()
         self.w.MplWidget.canvas.draw()
         # This is a messy solution to force the matplotlib widget to update the plot by introducing an error (calling
@@ -4726,15 +4861,23 @@
         if not keep_zoom:
             xlim = self.w.MplWidget.canvas.axes.get_xlim()
             ylim = self.w.MplWidget.canvas.axes.get_ylim()
 
         self.w.MplWidget.canvas.axes.plot(
             [self.ph_corr.pivot2d[self.ph_corr.dim], self.ph_corr.pivot2d[self.ph_corr.dim]],
             [2.0 * self.ph_corr.spc_max, -2.0 * self.ph_corr.spc_max], color='r')
-        self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
+
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            bg = (42 / 255, 42 / 255, 42 / 255)
+            fg = (255 / 255, 255 / 255, 255 / 255)
+        else:
+            bg = (255 / 255, 255 / 255, 255 / 255)
+            fg = (0 / 255, 0 / 255, 0 / 255)
+
+        self.w.MplWidget.canvas.axes.set_xlabel(xlabel, color=fg)
         self.w.MplWidget.canvas.axes.invert_xaxis()
         self.w.MplWidget.canvas.axes.set_xlim(xlim)
         self.w.MplWidget.canvas.axes.set_ylim(ylim)
         self.w.MplWidget.canvas.draw()
         # This is a messy solution to force the matplotlib widget to update the plot by introducing an error (calling
         # a figure object and redirecting the error output
         code_err = io.StringIO()
@@ -4912,16 +5055,23 @@
                                                      color=col2, linewidth=4)
 
         if len(h1_picked[spin_number - 1]) == 1:
             xlabel += " (Peak {}, {} signal picked)".format(spin_number, len(h1_picked[spin_number - 1]))
         else:
             xlabel += " (Peak {}, {} signals picked)".format(spin_number, len(h1_picked[spin_number - 1]))
 
-        self.w.hsqcPeak.canvas.axes.set_xlabel(xlabel)
-        self.w.hsqcPeak.canvas.axes.set_ylabel(ylabel)
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            bg = (42 / 255, 42 / 255, 42 / 255)
+            fg = (255 / 255, 255 / 255, 255 / 255)
+        else:
+            bg = (255 / 255, 255 / 255, 255 / 255)
+            fg = (0 / 255, 0 / 255, 0 / 255)
+
+        self.w.hsqcPeak.canvas.axes.set_xlabel(xlabel, color=fg)
+        self.w.hsqcPeak.canvas.axes.set_ylabel(ylabel, color=fg)
         self.w.hsqcPeak.canvas.draw()
         self.w.hsqcMultiplet.canvas.axes.clear()
         if len(h1_picked[spin_number - 1]) > 0:
             h1_pos = np.mean(h1_picked[spin_number - 1])
         else:
             h1_pos = h1_shift
 
@@ -4931,15 +5081,22 @@
                                               self.nd.nmrdat[self.nd.s][self.nd.e].spc.real[c13_pts1:c13_pts2, h1_pts],
                                               color=col1, linewidth=2)
         if len(hd.sim_spc[spin_number - 1]) > 0:
             self.w.hsqcMultiplet.canvas.axes.plot(self.nd.nmrdat[self.nd.s][self.nd.e].ppm2[c13_pts1:c13_pts2],
                                                   hd.sim_spc[spin_number - 1][c13_pts1:c13_pts2], color=col2,
                                                   linewidth=2)
 
-        self.w.hsqcMultiplet.canvas.axes.set_xlabel(ylabel)
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            bg = (42 / 255, 42 / 255, 42 / 255)
+            fg = (255 / 255, 255 / 255, 255 / 255)
+        else:
+            bg = (255 / 255, 255 / 255, 255 / 255)
+            fg = (0 / 255, 0 / 255, 0 / 255)
+
+        self.w.hsqcMultiplet.canvas.axes.set_xlabel(ylabel, color=fg)
         self.w.hsqcMultiplet.canvas.axes.autoscale()
         self.w.hsqcMultiplet.canvas.axes.invert_xaxis()
         self.w.hsqcMultiplet.canvas.draw()
         self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.set_peak_information()
         # self.clear_hsqc_spin_sys()
         self.set_hsqc_spin_sys()
         if self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.autosim:
@@ -5021,40 +5178,42 @@
         pos_col = matplotlib.colors.to_hex(pos_col)
         neg_col = matplotlib.colors.to_hex(neg_col)
         xlabel = d.x_label + " [" + d.axis_type1 + "]"
         ylabel = d.y_label + " [" + d.axis_type2 + "]"
         # print(self.nd.nmrdat[self.nd.s][self.nd.e].dim)
         if (self.nd.nmrdat[s][e].dim == 1):
             self.w.MplWidget.canvas.axes.clear()
-            for k in range(len(self.nd.nmrdat[s])):
-                if ((k != e) and (self.nd.nmrdat[s][k].display.display_spc == True)):
-                    d = self.nd.nmrdat[s][k].display
-                    if (d.pos_col == "RGB"):
-                        pos_col = d.pos_col_rgb
-                    else:
-                        pos_col = d.pos_col
+            for s1 in range(len(self.nd.nmrdat)):
+                for k in range(len(self.nd.nmrdat[s1])):
+                    if ((k != e) or (s1 != s)) and (self.nd.nmrdat[s1][k].display.display_spc == True):
+                        #d = self.nd.nmrdat[s1][k].display
+                        if (self.nd.nmrdat[s1][k].display.pos_col == "RGB"):
+                            pos_col = self.nd.nmrdat[s1][k].display.pos_col_rgb
+                        else:
+                            pos_col = self.nd.nmrdat[s1][k].display.pos_col
 
-                    if (d.neg_col == "RGB"):
-                        neg_col = d.neg_col_rgb
-                    else:
-                        neg_col = d.neg_col
+                        if (self.nd.nmrdat[s1][k].display.neg_col == "RGB"):
+                            neg_col = self.nd.nmrdat[s1][k].display.neg_col_rgb
+                        else:
+                            neg_col = self.nd.nmrdat[s1][k].display.neg_col
 
-                    pos_col = matplotlib.colors.to_hex(pos_col)
-                    neg_col = matplotlib.colors.to_hex(neg_col)
-                    self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
-                                                      self.nd.nmrdat[s][k].spc[0].real, color=pos_col)
-
-                    if self.w.splinebaseline.isChecked():
-                        if len(self.nd.nmrdat[s][k].spline_baseline.baseline_points) > 0:
-                            self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].spline_baseline.baseline_points,
-                                                              self.nd.nmrdat[s][k].spline_baseline.baseline_values, 'o', color="lightgreen")
-                            if plot_spline_baseline:
-                                self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
-                                                                  self.nd.nmrdat[s][k].calc_spline_baseline(),
-                                                                  color="lightgreen")
+                        pos_col = matplotlib.colors.to_hex(pos_col)
+                        neg_col = matplotlib.colors.to_hex(neg_col)
+                        #print(f'Dataset: {s1}, Exp: {k}, pos_col: {pos_col}')
+                        self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s1][k].ppm1,
+                                                          self.nd.nmrdat[s1][k].spc[0].real, color=pos_col)
+
+                        if self.w.splinebaseline.isChecked() and s1 == s:
+                            if len(self.nd.nmrdat[s][k].spline_baseline.baseline_points) > 0:
+                                self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].spline_baseline.baseline_points,
+                                                                  self.nd.nmrdat[s][k].spline_baseline.baseline_values, 'o', color="lightgreen")
+                                if plot_spline_baseline:
+                                    self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
+                                                                      self.nd.nmrdat[s][k].calc_spline_baseline(),
+                                                                      color="lightgreen")
 
             d = self.nd.nmrdat[s][e].display
             if (d.pos_col == "RGB"):
                 pos_col = d.pos_col_rgb
             else:
                 pos_col = d.pos_col
 
@@ -5081,15 +5240,22 @@
                 if len(self.nd.nmrdat[s][k].spline_baseline.baseline_points) > 0:
                     self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].spline_baseline.baseline_points,
                                                       self.nd.nmrdat[s][e].spline_baseline.baseline_values, 'o', color="lightgreen")
                     if plot_spline_baseline:
                         baseline = self.nd.nmrdat[s][e].calc_spline_baseline()
                         self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].ppm1, baseline, color="lightgreen")
 
-            self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
+            if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+                bg = (42 / 255, 42 / 255, 42 / 255)
+                fg = (255 / 255, 255 / 255, 255 / 255)
+            else:
+                bg = (255 / 255, 255 / 255, 255 / 255)
+                fg = (0 / 255, 0 / 255, 0 / 255)
+
+            self.w.MplWidget.canvas.axes.set_xlabel(xlabel, color=fg)
             self.w.MplWidget.canvas.axes.autoscale()
             self.w.MplWidget.canvas.axes.invert_xaxis()
             if (self.keep_zoom == True):
                 self.w.MplWidget.canvas.axes.set_xlim(xlim)
                 self.w.MplWidget.canvas.axes.set_ylim(ylim)
 
             # self.w.MplWidget.canvas.toolbar.update()
@@ -5109,16 +5275,24 @@
                                                  self.nd.nmrdat[self.nd.s][self.nd.e].ppm2,
                                                  self.nd.nmrdat[self.nd.s][self.nd.e].spc.real, pos_lev, colors=pos_col,
                                                  linestyles='solid', antialiased=True)
             self.w.MplWidget.canvas.axes.contour(self.nd.nmrdat[self.nd.s][self.nd.e].ppm1,
                                                  self.nd.nmrdat[self.nd.s][self.nd.e].ppm2,
                                                  self.nd.nmrdat[self.nd.s][self.nd.e].spc.real, neg_lev, colors=neg_col,
                                                  linestyles='solid', antialiased=True)
-            self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
-            self.w.MplWidget.canvas.axes.set_ylabel(ylabel)
+
+            if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+                bg = (42 / 255, 42 / 255, 42 / 255)
+                fg = (255 / 255, 255 / 255, 255 / 255)
+            else:
+                bg = (255 / 255, 255 / 255, 255 / 255)
+                fg = (0 / 255, 0 / 255, 0 / 255)
+
+            self.w.MplWidget.canvas.axes.set_xlabel(xlabel, color=fg)
+            self.w.MplWidget.canvas.axes.set_ylabel(ylabel, color=fg)
             self.w.MplWidget.canvas.axes.autoscale()
             self.w.MplWidget.canvas.axes.invert_xaxis()
             self.w.MplWidget.canvas.axes.invert_yaxis()
             if (self.keep_zoom == True):
                 self.w.MplWidget.canvas.axes.set_xlim(xlim)
                 self.w.MplWidget.canvas.axes.set_ylim(ylim)
             else:
@@ -5214,15 +5388,22 @@
         if (self.w.preProcessingWidget.currentIndex() == 5):
             for k in range(len(self.nd.pp.compress_start)):
                 self.w.MplWidget.canvas.axes.axvspan(self.nd.pp.compress_start[k], self.nd.pp.compress_end[k],
                                                      alpha=self.nd.pp.alpha, color=self.nd.pp.colour)
 
         d = self.nd.nmrdat[self.nd.s][self.nd.e].display
         xlabel = d.x_label + " [" + d.axis_type1 + "]"
-        self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            bg = (42 / 255, 42 / 255, 42 / 255)
+            fg = (255 / 255, 255 / 255, 255 / 255)
+        else:
+            bg = (255 / 255, 255 / 255, 255 / 255)
+            fg = (0 / 255, 0 / 255, 0 / 255)
+
+        self.w.MplWidget.canvas.axes.set_xlabel(xlabel, color=fg)
         self.w.MplWidget.canvas.axes.autoscale()
         self.w.MplWidget.canvas.axes.invert_xaxis()
         if (self.keep_zoom == True):
             self.w.MplWidget.canvas.axes.set_xlim(xlim)
             self.w.MplWidget.canvas.axes.set_ylim(ylim)
 
         # self.w.MplWidget.canvas.toolbar.update()
@@ -5458,22 +5639,23 @@
                 self.temp_ref_shift = ref_shift
                 self.w.MplWidget.canvas.setFocus()
                 self.show_nmr_spectrum()
                 self.ginput_ref_1d(1)
 
         # end reference1d
 
-    def reference1d_all(self, new_shift):
+    def reference1d_all(self, new_shift, find_maximum=True):
         self.w.nmrSpectrum.setCurrentIndex(0)
         self.temp_shift = new_shift
+        self.find_maximum = find_maximum
         self.ginput_ref_1d_all(1)
         # end reference1d_all
 
     def reference1d_all_2(self):
-        self.nd.reference1d_all(self.xdata[0], self.temp_shift)
+        self.nd.reference1d_all(self.xdata[0], self.temp_shift, self.find_maximum)
         self.xdata = []
         self.ydata = []
         self.temp_shift = 0.0
         self.plot_spc()
         # end reference1d_all_2
 
     def reference2d(self, ref_shift=[0.0, 0.0], peak_number=-1):
@@ -5573,17 +5755,17 @@
         self.w.MplWidget.canvas.draw()
         # end data_pre_processing
 
     def reset_help(self):
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
         if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
-            f_name = os.path.join(base_dir, "nmr", "web", "introductionDark", "index.html")
+            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
         else:
-            f_name = os.path.join(base_dir, "nmr", "web", "introduction", "index.html")
+            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
 
         url = "file:///" + f_name.replace('\\', '/')
         self.w.helpView.setUrl(url)
         self.w.nmrSpectrum.setCurrentIndex(12)
         # end reset_help
 
     def reset_ml_info(self):
@@ -5641,15 +5823,15 @@
     def save_hsqc_data(self):
         pf_name = QFileDialog.getSaveFileName(None, "Save HSQC Data", "", "*.xlsx", "*.xlsx")
         f_name = pf_name[0].rstrip('.xlsx').rstrip(' ').rstrip('/').rstrip('.xlsx') + '.xlsx'
         self.nd.export_hsqc_data(f_name)
         # end save_hsqc_data
 
     def save_config(self):
-        self.cf.auto_plot = self.w.autoPlot.isChecked()
+        #self.cf.auto_plot = self.w.autoPlot.isChecked()
         self.cf.keep_zoom = self.w.keepZoom.isChecked()
         self.cf.font_size = self.w.fontSize.value()
         self.cf.phase_reference_colour = self.nd.nmrdat[0][0].display.ph_ref_col
         self.cf.pos_col10 = self.std_pos_col1[0]
         self.cf.pos_col11 = self.std_pos_col1[1]
         self.cf.pos_col12 = self.std_pos_col1[2]
         self.cf.neg_col10 = self.std_neg_col1[0]
@@ -6076,14 +6258,18 @@
         acq_str += "groupDelay           [us]     " + "% 9.2f\n" % a.group_delay
         acq_str += "decim                         " + "% 6d\n" % a.decim
         acq_str += "dspfvs                        " + "% 6d\n" % a.dspfvs
         acq_str += "temperature          [K]      " + "% 9.2f\n" % a.temperature
         self.w.acqPars.setText(acq_str)
         # end set_acq_pars
 
+    def set_autobaseline(self):
+        self.w.autobaselineBox.setChecked(self.nd.nmrdat[self.nd.s][self.nd.e].proc.autobaseline)
+        # end set_autobaseline
+
     def set_avoid_neg_values(self):
         if (self.nd.pp.pre_proc_fill == False):
             if (self.w.avoidNegValues.isChecked() == True):
                 self.nd.pp.avoid_negative_values = True
             else:
                 self.nd.pp.avoid_negative_values = False
 
@@ -6642,17 +6828,17 @@
 
     def set_help(self):
         url = []
         idx = self.w.helpComboBox.currentIndex()
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
         if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
-            f_name = os.path.join(base_dir, "nmr", "web", "introductionDark", "index.html")
+            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
         else:
-            f_name = os.path.join(base_dir, "nmr", "web", "introduction", "index.html")
+            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
 
         url.append("file:///" + f_name.replace('\\', '/'))
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
@@ -6803,18 +6989,25 @@
             if idx_key_str in hsqc.hsqc_data[hsqc.cur_metabolite].c13_offset.keys():
                 offset = QTableWidgetItem(str(hsqc.hsqc_data[hsqc.cur_metabolite].c13_offset[idx_key_str]))
             else:
                 offset = QTableWidgetItem("0")
 
             j_cc = QTableWidgetItem(' '.join(str(e) for e in spin_sys['j_cc'][k]))
             perc = QTableWidgetItem(str(spin_sys['contribution'][k]))
-            idx.setTextAlignment(QtCore.Qt.AlignLeft)
-            offset.setTextAlignment(QtCore.Qt.AlignHCenter)
-            j_cc.setTextAlignment(QtCore.Qt.AlignLeft)
-            perc.setTextAlignment(QtCore.Qt.AlignHCenter)
+            try:
+                idx.setTextAlignment(QtCore.Qt.AlignLeft)
+                offset.setTextAlignment(QtCore.Qt.AlignHCenter)
+                j_cc.setTextAlignment(QtCore.Qt.AlignLeft)
+                perc.setTextAlignment(QtCore.Qt.AlignmentFlag.AlignHCenter)
+            except:
+                idx.setTextAlignment(0) #QtCore.Qt.AlignLeft)
+                offset.setTextAlignment(4) #QtCore.Qt.AlignHCenter)
+                j_cc.setTextAlignment(0) #QtCore.Qt.AlignLeft)
+                perc.setTextAlignment(4) #QtCore.Qt.AlignmentFlag.AlignHCenter)
+
             self.w.hsqcSpinSys.setItem(k, 0, idx)
             self.w.hsqcSpinSys.setItem(k, 1, offset)
             self.w.hsqcSpinSys.setItem(k, 2, j_cc)
             self.w.hsqcSpinSys.setItem(k, 3, perc)
             # self.w.hsqcSpinSys.item(k, 0).setText(' '.join(str(e) for e in spin_sys['c13_shifts'][k]))
             # self.w.hsqcSpinSys.item(k, 1).setText('0') # '.join(str(e) for e in spin_sys['c13_shifts'][k]))
             # self.w.hsqcSpinSys.item(k, 2).setText(' '.join(str(e) for e in spin_sys['j_cc'][k]))
@@ -7055,15 +7248,15 @@
             # header.setStretchLastSection(True)
             self.w.displayAssignedMetabolites.setVisible(True)
             self.w.displayLibraryShifts.setVisible(True)
             self.w.displaySelectedMetabolite.setVisible(True)
             self.nd.old_data_set = self.nd.s
             self.nd.old_data_exp = self.nd.e
             self.w.multipletAnalysis.setVisible(False)
-            self.w.isotopomerAnalysis.setVisible(False)
+            #self.w.isotopomerAnalysis.setVisible(False)
             self.w.nmrSpectrum.setTabEnabled(1, True)
             # self.w.nmrSpectrum.setTabEnabled(2, True)
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.set_metabolite_list()
             model = QtGui.QStandardItemModel()
             if self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.autoscale_j == True:
                 if len(self.nd.nmrdat[self.nd.s][self.nd.e].acq.cnst) > 0:
                     self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.j_scale = self.nd.nmrdat[self.nd.s][self.nd.e].acq.cnst[
@@ -7127,17 +7320,17 @@
             self.w.displayAssignedMetabolites.setChecked(False)
             self.w.displayAssignedMetabolites.setVisible(False)
             self.w.displayLibraryShifts.setChecked(False)
             self.w.displayLibraryShifts.setVisible(False)
             self.w.displaySelectedMetabolite.setChecked(False)
             self.w.displaySelectedMetabolite.setVisible(False)
             self.w.multipletAnalysis.setChecked(False)
-            self.w.isotopomerAnalysis.setChecked(False)
+            #self.w.isotopomerAnalysis.setChecked(False)
             self.w.multipletAnalysis.setVisible(False)
-            self.w.isotopomerAnalysis.setVisible(False)
+            #self.w.isotopomerAnalysis.setVisible(False)
             self.w.nmrSpectrum.setTabEnabled(1, False)
             self.w.nmrSpectrum.setTabEnabled(2, False)
             self.w.openWeb.clear()
             self.w.hsqcMetabolites.setCurrentIndex(self.w.hsqcMetabolites.model().index(-1, 0))
             self.w.hsqcAssignedMetabolites.setCurrentIndex(self.w.hsqcMetabolites.model().index(-1, 0))
             for k in range(len(self.nd.nmrdat)):
                 for l in range(len(self.nd.nmrdat[k])):
@@ -7242,27 +7435,14 @@
             self.w.nmrSpectrum.setTabEnabled(3, False)
             self.w.nmrSpectrum.setStyleSheet(
                 "QTabBar::tab::disabled {width: 0; height: 0; margin: 0; padding: 0; border: none;} ")
             self.w.nmrSpectrum.setCurrentIndex(1)
 
         # end set_multiplet_analysis
 
-    def set_isotopomer_analysis(self):
-        if (self.w.isotopomerAnalysis.isChecked() == True):
-            self.w.nmrSpectrum.setTabEnabled(4, True)
-            self.w.nmrSpectrum.setStyleSheet(
-                "QTabBar::tab::disabled {width: 0; height: 0; margin: 0; padding: 0; border: none;} ")
-            self.w.nmrSpectrum.setCurrentIndex(4)
-        else:
-            self.w.nmrSpectrum.setTabEnabled(4, False)
-            self.w.nmrSpectrum.setStyleSheet(
-                "QTabBar::tab::disabled {width: 0; height: 0; margin: 0; padding: 0; border: none;} ")
-            self.w.nmrSpectrum.setCurrentIndex(1)
-
-        # end set_isotopomer_analysis
 
     def set_pre_processing_options(self):
         cur_idx = self.w.preProcessingSelect.currentIndex()
         self.w.preProcessingWidget.setCurrentIndex(cur_idx)
         if self.nd.nmrdat[self.nd.s][0].acq.manufacturer == 'Bruker':
             if self.w.exportMethod.count() == 5:
                 self.w.exportMethod.addItem('Bruker Dataset')
@@ -7705,19 +7885,24 @@
         else:
             jupyterthemes.install_theme('grade3')
 
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
         jupyter_path = os.path.join(base_dir, "nmr", "jupyter")
         jobs = []
-        self.process = multiprocess.Process(target=notebookapp.main,
-                                      args=([jupyter_path, '--no-browser', '--ip=127.0.0.1', '--port=9997', '--NotebookApp.token=''', '--NotebookApp.password='''],))
+        print("-----------------")
+        self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--ip=127.0.0.1', '--port=9997'],))
+        #self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--no-browser', '--ip=127.0.0.1', '--port=9997', '--NotebookApp.token=''', '--NotebookApp.password='''],))
+        print('=======================')
         jobs.append(self.process)
+        print('#########################')
         self.process.start()
+        print('//////////////////////////')
         sleep(2)
+        print('__________________________')
         self.w.helpView.setUrl('http://127.0.0.1:9997')
         self.w.nmrSpectrum.setCurrentIndex(12)
         # end startNotebook
 
     def stop_notebook(self):
         try:
             self.process.terminate()
@@ -7894,15 +8079,15 @@
                 self.w.hsqcAnalysis.setVisible(False)
 
         else:
             self.w.hsqcAnalysis.setChecked(False)
             self.w.hsqcAnalysis.setVisible(False)
 
         self.w.multipletAnalysis.setVisible(False)
-        self.w.isotopomerAnalysis.setVisible(False)
+        #self.w.isotopomerAnalysis.setVisible(False)
         return "updated GUI"
         # end update_gui
 
     def update_metabolabpy(self):
         code_out = io.StringIO()
         code_err = io.StringIO()
         sys.stdout = code_out
@@ -8195,103 +8380,7 @@
         self.w.console.setTextColor(err_col)
         self.w.console.append(code_err.getvalue())
         code_out.close()
         code_err.close()
         self.w.nmrSpectrum.setCurrentIndex(11)
 
 
-def main():  # pragma: no cover
-    sys.argv.append('None')
-    ap = argparse.ArgumentParser()
-    ap.add_argument("-s", "--script", required=False, help="optional script argument")
-    ap.add_argument("-ns", "--noSplash", required=False, help="turn splash screen off", action="store_true")
-    ap.add_argument("-fs", "--FullScreen", required=False, help="open applicatin in full screen mode",
-                    action="store_true")
-    ap.add_argument("-k", "--KioskMode", required=False,
-                    help="open applicatin in full screen mode without windowed mode available",
-                    action="store_true")
-    ap.add_argument("fileName", metavar="fileName", type=str, help="load MetaboLabPy DataSet File")
-    dd = ap.parse_known_args()
-    # dd = ap.parse_known_intermixed_args()
-    if len(dd[1]) > 0:
-        sys.argv.pop()
-
-    args = vars(ap.parse_args())
-    QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
-    app = QApplication(['MetaboLabPy'])
-    icon = QIcon()
-    nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-    base_dir = os.path.split(nmr_dir)[0]
-    p_name = os.path.join(base_dir, "icon")
-    icon.addFile(os.path.join(p_name, "icon-16.png"), QtCore.QSize(16, 16))
-    icon.addFile(os.path.join(p_name, "icon-24.png"), QtCore.QSize(24, 24))
-    icon.addFile(os.path.join(p_name, "icon-32.png"), QtCore.QSize(32, 32))
-    icon.addFile(os.path.join(p_name, "icon-48.png"), QtCore.QSize(48, 48))
-    icon.addFile(os.path.join(p_name, "icon-256.png"), QtCore.QSize(256, 256))
-    app.setWindowIcon(icon)
-    app.setApplicationDisplayName("MetaboLabPy")
-    w = main_w()
-    if args["FullScreen"] == True or args["KioskMode"] == True:
-        w.w.showFullScreen()
-
-    if args["KioskMode"] == True:
-        w.w.actionToggle_FullScreen.triggered.disconnect()
-
-    if args["noSplash"] == False:
-        ##
-        # Create and display the splash screen
-        nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-        base_dir = os.path.split(nmr_dir)[0]
-        p_name = os.path.join(base_dir, "png")
-        cf = nmrConfig.NmrConfig()
-        cf.read_config()
-        if cf.mode == 'dark' or (cf.mode == 'system' and darkdetect.isDark()):
-            splash_pix = QPixmap(os.path.join(p_name, "metabolabpy_dark.png"))
-        else:
-            splash_pix = QPixmap(os.path.join(p_name, "metabolabpy.png"))
-
-        splash = QSplashScreen(splash_pix)
-        splash.setMask(splash_pix.mask())
-        # adding progress bar
-        splash.show()
-        app.processEvents()
-        max_time = 2
-        max_range = 30
-        time_inc = max_range
-        for i in range(max_range):
-            # Simulate something that takes time
-            time.sleep(max_time / float(max_range))
-
-        splash.close()
-        ## End of splash screen
-
-    if args["fileName"] != "None":
-        try:
-            w.load_file(args["fileName"])
-        except:
-            if (args["script"] != None):
-                w.open_script(args["script"])
-                w.script_editor()
-                w.exec_script()
-
-    else:
-        if (args["script"] != None):
-            w.open_script(args["script"])
-            w.script_editor()
-            w.exec_script()
-
-    if cf.mode == 'system':
-        if darkdetect.isDark():
-            qtmodern.styles.dark(app)
-        else:
-            qtmodern.styles.light(app)
-    elif cf.mode == 'light':
-        qtmodern.styles.light(app)
-    else:
-        qtmodern.styles.dark(app)
-
-    w.show()
-    sys.exit(app.exec_())
-
-
-if __name__ == "__main__":  # pragma: no cover
-    main()
```

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.9.0/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files 0% similar despite different names*

#### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.0/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

```diff
@@ -3,61 +3,47 @@
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1914</width>
-        <height>895</height>
+        <height>917</height>
       </rect>
     </property>
     <property name="font">
       <font>
         <pointsize>14</pointsize>
       </font>
     </property>
     <property name="windowTitle">
       <string>MetaboLabPy GUI</string>
     </property>
     <widget class="QWidget" name="centralWidget">
       <layout class="QGridLayout" name="gridLayout_13">
-        <item row="2" column="0">
-          <layout class="QHBoxLayout" name="horizontalLayout_43">
-            <item>
-              <widget class="QLabel" name="label_57">
-                <property name="text">
-                  <string>&gt;&gt;&gt;</string>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QLineEdit" name="cmdLine"/>
-            </item>
-          </layout>
-        </item>
         <item row="1" column="0">
           <layout class="QHBoxLayout" name="horizontalLayout">
             <item>
               <widget class="QLabel" name="label">
                 <property name="text">
-                  <string>DataSet</string>
+                  <string>Set</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QSpinBox" name="setBox">
                 <property name="maximum">
                   <number>99999</number>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QLabel" name="label_2">
                 <property name="text">
-                  <string>Experiment</string>
+                  <string>Exp</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QSpinBox" name="expBox">
                 <property name="maximum">
                   <number>99999</number>
@@ -99,15 +85,15 @@
                   <string>Peak Picking</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QCheckBox" name="splinebaseline">
                 <property name="text">
-                  <string>Spline Baseline Correction</string>
+                  <string>Spline BC</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QCheckBox" name="hsqcAnalysis">
                 <property name="text">
                   <string>HSQC Analysis</string>
@@ -118,44 +104,27 @@
               <widget class="QCheckBox" name="multipletAnalysis">
                 <property name="text">
                   <string>Multiplet Analysis</string>
                 </property>
               </widget>
             </item>
             <item>
-              <widget class="QCheckBox" name="isotopomerAnalysis">
-                <property name="text">
-                  <string>Isotopomer Analysis</string>
-                </property>
-              </widget>
-            </item>
-            <item>
               <spacer name="horizontalSpacer_2">
                 <property name="orientation">
                   <enum>Qt::Horizontal</enum>
                 </property>
                 <property name="sizeHint" stdset="0">
                   <size>
                     <width>41</width>
                     <height>20</height>
                   </size>
                 </property>
               </spacer>
             </item>
             <item>
-              <widget class="QCheckBox" name="autoPlot">
-                <property name="text">
-                  <string>AutoPlot |</string>
-                </property>
-                <property name="checked">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
               <widget class="QCheckBox" name="keepZoom">
                 <property name="text">
                   <string>keepZoom |</string>
                 </property>
                 <property name="checked">
                   <bool>true</bool>
                 </property>
@@ -176,15 +145,15 @@
                 <property name="maximum">
                   <number>999</number>
                 </property>
                 <property name="singleStep">
                   <number>1</number>
                 </property>
                 <property name="value">
-                  <number>13</number>
+                  <number>10</number>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QPushButton" name="loadButton">
                 <property name="text">
                   <string>Load</string>
@@ -203,27 +172,41 @@
                 <property name="text">
                   <string>Quit</string>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
+        <item row="2" column="0">
+          <layout class="QHBoxLayout" name="horizontalLayout_43">
+            <item>
+              <widget class="QLabel" name="label_57">
+                <property name="text">
+                  <string>&gt;&gt;&gt;</string>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QLineEdit" name="cmdLine"/>
+            </item>
+          </layout>
+        </item>
         <item row="0" column="0">
           <widget class="QTabWidget" name="nmrSpectrum">
             <property name="enabled">
               <bool>true</bool>
             </property>
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="currentIndex">
-              <number>0</number>
+              <number>1</number>
             </property>
             <widget class="QWidget" name="spcTab">
               <attribute name="title">
                 <string>NMR Spectrum</string>
               </attribute>
               <layout class="QGridLayout" name="gridLayout_26">
                 <item row="0" column="0">
@@ -232,16 +215,16 @@
                       <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                         <horstretch>90</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
                     </property>
                     <property name="minimumSize">
                       <size>
-                        <width>500</width>
-                        <height>500</height>
+                        <width>400</width>
+                        <height>400</height>
                       </size>
                     </property>
                     <property name="mouseTracking">
                       <bool>false</bool>
                     </property>
                   </widget>
                 </item>
@@ -2499,15 +2482,15 @@
                               <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                                 <horstretch>0</horstretch>
                                 <verstretch>0</verstretch>
                               </sizepolicy>
                             </property>
                             <property name="minimumSize">
                               <size>
-                                <width>400</width>
+                                <width>200</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="midLineWidth">
                               <number>1</number>
                             </property>
                             <property name="rowCount">
@@ -2964,18 +2947,24 @@
                               <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                 <horstretch>180</horstretch>
                                 <verstretch>0</verstretch>
                               </sizepolicy>
                             </property>
                             <property name="minimumSize">
                               <size>
-                                <width>450</width>
+                                <width>280</width>
                                 <height>0</height>
                               </size>
                             </property>
+                            <property name="maximumSize">
+                              <size>
+                                <width>16777215</width>
+                                <height>16777215</height>
+                              </size>
+                            </property>
                             <property name="sizeIncrement">
                               <size>
                                 <width>0</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="mouseTracking">
@@ -2997,15 +2986,15 @@
                                   <property name="sizePolicy">
                                     <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                       <horstretch>3</horstretch>
                                       <verstretch>0</verstretch>
                                     </sizepolicy>
                                   </property>
                                   <property name="text">
-                                    <string>Fit up to # bonds</string>
+                                    <string># bonds</string>
                                   </property>
                                 </widget>
                                 <widget class="QComboBox" name="fitUpToBonds">
                                   <property name="sizePolicy">
                                     <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                                       <horstretch>10</horstretch>
                                       <verstretch>0</verstretch>
@@ -3038,15 +3027,15 @@
                                     <property name="text">
                                       <string>4</string>
                                     </property>
                                   </item>
                                 </widget>
                                 <widget class="QLabel" name="label_93">
                                   <property name="text">
-                                    <string>Coefficient of Determination</string>
+                                    <string>Coeff. of Det.</string>
                                   </property>
                                 </widget>
                                 <widget class="QLCDNumber" name="coefficientOfDetermination">
                                   <property name="value" stdset="0">
                                     <double>-1.000000000000000</double>
                                   </property>
                                 </widget>
@@ -3058,15 +3047,15 @@
                                   <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                     <horstretch>45</horstretch>
                                     <verstretch>40</verstretch>
                                   </sizepolicy>
                                 </property>
                                 <property name="minimumSize">
                                   <size>
-                                    <width>50</width>
+                                    <width>400</width>
                                     <height>0</height>
                                   </size>
                                 </property>
                                 <property name="maximumSize">
                                   <size>
                                     <width>600</width>
                                     <height>16777215</height>
@@ -3080,15 +3069,15 @@
                                   <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                                     <horstretch>0</horstretch>
                                     <verstretch>40</verstretch>
                                   </sizepolicy>
                                 </property>
                                 <property name="maximumSize">
                                   <size>
-                                    <width>16777215</width>
+                                    <width>500</width>
                                     <height>100</height>
                                   </size>
                                 </property>
                                 <property name="frameShape">
                                   <enum>QFrame::StyledPanel</enum>
                                 </property>
                                 <property name="frameShadow">
@@ -3199,110 +3188,116 @@
                               <size>
                                 <width>0</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="maximumSize">
                               <size>
-                                <width>16777215</width>
+                                <width>500</width>
                                 <height>16777215</height>
                               </size>
                             </property>
                             <property name="currentIndex">
                               <number>0</number>
                             </property>
                             <widget class="QWidget" name="hsqcPeakPickingTab">
                               <attribute name="title">
                                 <string>HSQC Peak Picking</string>
                               </attribute>
                               <layout class="QGridLayout" name="gridLayout_22">
-                                <item row="2" column="8">
-                                  <widget class="QLabel" name="label_74">
+                                <item row="0" column="0">
+                                  <widget class="QPushButton" name="hsqcAddPeak">
+                                    <property name="toolTip">
+                                      <string extracomment="Add Peak"/>
+                                    </property>
                                     <property name="text">
-                                      <string>Metabolites</string>
+                                      <string>+</string>
                                     </property>
-                                    <property name="alignment">
-                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                  </widget>
+                                </item>
+                                <item row="0" column="1">
+                                  <widget class="QPushButton" name="hsqcRemovePeak">
+                                    <property name="toolTip">
+                                      <string extracomment="Remove Peak"/>
+                                    </property>
+                                    <property name="text">
+                                      <string>-</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="0" column="6" colspan="3">
-                                  <widget class="QLabel" name="metaboliteLabel">
-                                    <property name="font">
-                                      <font>
-                                        <pointsize>18</pointsize>
-                                        <weight>75</weight>
-                                        <bold>true</bold>
-                                      </font>
+                                <item row="0" column="2">
+                                  <spacer name="horizontalSpacer_41">
+                                    <property name="orientation">
+                                      <enum>Qt::Horizontal</enum>
                                     </property>
+                                    <property name="sizeHint" stdset="0">
+                                      <size>
+                                        <width>40</width>
+                                        <height>20</height>
+                                      </size>
+                                    </property>
+                                  </spacer>
+                                </item>
+                                <item row="0" column="3" colspan="2">
+                                  <widget class="QPushButton" name="metaboliteResetButton">
                                     <property name="text">
-                                      <string>Metabolite</string>
+                                      <string>Reset</string>
                                     </property>
-                                    <property name="alignment">
-                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                  </widget>
+                                </item>
+                                <item row="0" column="5" colspan="2">
+                                  <widget class="QPushButton" name="metaboliteAutoButton">
+                                    <property name="text">
+                                      <string>Autopick</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="2" column="1" colspan="2">
-                                  <widget class="QPushButton" name="displayMetaboliteInformation">
+                                <item row="0" column="7">
+                                  <widget class="QPushButton" name="metaboliteAutofitButton">
                                     <property name="text">
-                                      <string>Display Info</string>
+                                      <string>Autofit</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="2" column="0">
-                                  <widget class="QLabel" name="label_72">
+                                <item row="1" column="0" colspan="8">
+                                  <widget class="QGraphicsView" name="metaboliteImage">
                                     <property name="sizePolicy">
-                                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                                      <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                                         <horstretch>0</horstretch>
                                         <verstretch>0</verstretch>
                                       </sizepolicy>
                                     </property>
-                                    <property name="text">
-                                      <string>Search</string>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item row="2" column="7">
-                                  <spacer name="horizontalSpacer_42">
-                                    <property name="orientation">
-                                      <enum>Qt::Horizontal</enum>
+                                    <property name="minimumSize">
+                                      <size>
+                                        <width>0</width>
+                                        <height>120</height>
+                                      </size>
                                     </property>
-                                    <property name="sizeHint" stdset="0">
+                                    <property name="maximumSize">
                                       <size>
-                                        <width>18</width>
-                                        <height>20</height>
+                                        <width>16777215</width>
+                                        <height>16777215</height>
                                       </size>
                                     </property>
-                                  </spacer>
+                                  </widget>
                                 </item>
-                                <item row="3" column="0" colspan="3">
-                                  <widget class="QLineEdit" name="searchHsqcMetabolites">
-                                    <property name="enabled">
-                                      <bool>false</bool>
-                                    </property>
+                                <item row="2" column="0">
+                                  <widget class="QLabel" name="label_72">
                                     <property name="sizePolicy">
-                                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
-                                        <horstretch>5</horstretch>
+                                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                                        <horstretch>0</horstretch>
                                         <verstretch>0</verstretch>
                                       </sizepolicy>
                                     </property>
-                                  </widget>
-                                </item>
-                                <item row="0" column="0">
-                                  <widget class="QPushButton" name="hsqcAddPeak">
-                                    <property name="toolTip">
-                                      <string extracomment="Add Peak"/>
-                                    </property>
                                     <property name="text">
-                                      <string>+</string>
+                                      <string>Search</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="2" column="3" colspan="4">
+                                <item row="2" column="6" colspan="2">
                                   <widget class="QComboBox" name="openWeb">
                                     <property name="sizePolicy">
                                       <sizepolicy hsizetype="Preferred" vsizetype="Maximum">
                                         <horstretch>0</horstretch>
                                         <verstretch>0</verstretch>
                                       </sizepolicy>
                                     </property>
@@ -3310,22 +3305,28 @@
                                       <size>
                                         <width>120</width>
                                         <height>0</height>
                                       </size>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="0" column="2" colspan="2">
-                                  <widget class="QPushButton" name="metaboliteResetButton">
-                                    <property name="text">
-                                      <string>Reset</string>
+                                <item row="3" column="0" colspan="3">
+                                  <widget class="QLineEdit" name="searchHsqcMetabolites">
+                                    <property name="enabled">
+                                      <bool>false</bool>
+                                    </property>
+                                    <property name="sizePolicy">
+                                      <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+                                        <horstretch>5</horstretch>
+                                        <verstretch>0</verstretch>
+                                      </sizepolicy>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="3" column="3" colspan="6">
+                                <item row="3" column="4" colspan="4">
                                   <widget class="QComboBox" name="hsqcPathwaySelect">
                                     <property name="enabled">
                                       <bool>false</bool>
                                     </property>
                                     <property name="sizePolicy">
                                       <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                                         <horstretch>5</horstretch>
@@ -3405,15 +3406,15 @@
                                     <item>
                                       <property name="text">
                                         <string>Vitamin B6 Metabolism</string>
                                       </property>
                                     </item>
                                   </widget>
                                 </item>
-                                <item row="4" column="0" colspan="9">
+                                <item row="4" column="0" colspan="8">
                                   <widget class="QListView" name="hsqcMetabolites">
                                     <property name="sizePolicy">
                                       <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                                         <horstretch>0</horstretch>
                                         <verstretch>0</verstretch>
                                       </sizepolicy>
                                     </property>
@@ -3421,59 +3422,65 @@
                                       <size>
                                         <width>16777215</width>
                                         <height>16777215</height>
                                       </size>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="1" column="0" colspan="9">
-                                  <widget class="QGraphicsView" name="metaboliteImage">
-                                    <property name="sizePolicy">
-                                      <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-                                        <horstretch>0</horstretch>
-                                        <verstretch>0</verstretch>
-                                      </sizepolicy>
+                                <item row="2" column="1">
+                                  <spacer name="horizontalSpacer_42">
+                                    <property name="orientation">
+                                      <enum>Qt::Horizontal</enum>
                                     </property>
-                                    <property name="minimumSize">
+                                    <property name="sizeHint" stdset="0">
                                       <size>
-                                        <width>0</width>
-                                        <height>120</height>
+                                        <width>18</width>
+                                        <height>20</height>
                                       </size>
                                     </property>
-                                    <property name="maximumSize">
+                                  </spacer>
+                                </item>
+                                <item row="2" column="5">
+                                  <spacer name="horizontalSpacer_46">
+                                    <property name="orientation">
+                                      <enum>Qt::Horizontal</enum>
+                                    </property>
+                                    <property name="sizeHint" stdset="0">
                                       <size>
-                                        <width>16777215</width>
-                                        <height>16777215</height>
+                                        <width>40</width>
+                                        <height>20</height>
                                       </size>
                                     </property>
-                                  </widget>
-                                </item>
-                                <item row="0" column="4">
-                                  <widget class="QPushButton" name="metaboliteAutoButton">
-                                    <property name="text">
-                                      <string>Autopick</string>
-                                    </property>
-                                  </widget>
+                                  </spacer>
                                 </item>
-                                <item row="0" column="1">
-                                  <widget class="QPushButton" name="hsqcRemovePeak">
-                                    <property name="toolTip">
-                                      <string extracomment="Remove Peak"/>
+                                <item row="2" column="4">
+                                  <widget class="QPushButton" name="displayMetaboliteInformation">
+                                    <property name="minimumSize">
+                                      <size>
+                                        <width>120</width>
+                                        <height>0</height>
+                                      </size>
                                     </property>
                                     <property name="text">
-                                      <string>-</string>
+                                      <string>Display Info</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="0" column="5">
-                                  <widget class="QPushButton" name="metaboliteAutofitButton">
-                                    <property name="text">
-                                      <string>Autofit</string>
+                                <item row="2" column="2">
+                                  <spacer name="horizontalSpacer_48">
+                                    <property name="orientation">
+                                      <enum>Qt::Horizontal</enum>
                                     </property>
-                                  </widget>
+                                    <property name="sizeHint" stdset="0">
+                                      <size>
+                                        <width>40</width>
+                                        <height>20</height>
+                                      </size>
+                                    </property>
+                                  </spacer>
                                 </item>
                               </layout>
                             </widget>
                             <widget class="QWidget" name="hsqcMultipletAnalysisTab">
                               <attribute name="title">
                                 <string>Multiplet Analysis</string>
                               </attribute>
@@ -4458,14 +4465,92 @@
                                     </item>
                                   </widget>
                                 </item>
                               </layout>
                             </item>
                           </layout>
                         </item>
+                        <item row="2" column="0" colspan="2">
+                          <layout class="QHBoxLayout" name="horizontalLayout_52">
+                            <item>
+                              <widget class="QLabel" name="label_58">
+                                <property name="text">
+                                  <string>Strip Transform</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <spacer name="horizontalSpacer_37">
+                                <property name="orientation">
+                                  <enum>Qt::Horizontal</enum>
+                                </property>
+                                <property name="sizeHint" stdset="0">
+                                  <size>
+                                    <width>40</width>
+                                    <height>20</height>
+                                  </size>
+                                </property>
+                              </spacer>
+                            </item>
+                            <item>
+                              <spacer name="horizontalSpacer_38">
+                                <property name="orientation">
+                                  <enum>Qt::Horizontal</enum>
+                                </property>
+                                <property name="sizeHint" stdset="0">
+                                  <size>
+                                    <width>40</width>
+                                    <height>20</height>
+                                  </size>
+                                </property>
+                              </spacer>
+                            </item>
+                            <item>
+                              <spacer name="horizontalSpacer_39">
+                                <property name="orientation">
+                                  <enum>Qt::Horizontal</enum>
+                                </property>
+                                <property name="sizeHint" stdset="0">
+                                  <size>
+                                    <width>40</width>
+                                    <height>20</height>
+                                  </size>
+                                </property>
+                              </spacer>
+                            </item>
+                            <item>
+                              <widget class="QLabel" name="label_65">
+                                <property name="text">
+                                  <string>Start</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QLineEdit" name="stripTransformStart">
+                                <property name="alignment">
+                                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QLabel" name="label_71">
+                                <property name="text">
+                                  <string>End</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QLineEdit" name="stripTransformEnd">
+                                <property name="alignment">
+                                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
                         <item row="1" column="0" colspan="2">
                           <layout class="QHBoxLayout" name="horizontalLayout_32">
                             <item>
                               <widget class="QLabel" name="label_51">
                                 <property name="text">
                                   <string>Baseline Correction</string>
                                 </property>
@@ -4753,106 +4838,15 @@
                                     </item>
                                   </layout>
                                 </item>
                               </layout>
                             </item>
                           </layout>
                         </item>
-                        <item row="2" column="0" colspan="2">
-                          <layout class="QHBoxLayout" name="horizontalLayout_52">
-                            <item>
-                              <widget class="QLabel" name="label_58">
-                                <property name="text">
-                                  <string>Strip Transform</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <spacer name="horizontalSpacer_37">
-                                <property name="orientation">
-                                  <enum>Qt::Horizontal</enum>
-                                </property>
-                                <property name="sizeHint" stdset="0">
-                                  <size>
-                                    <width>40</width>
-                                    <height>20</height>
-                                  </size>
-                                </property>
-                              </spacer>
-                            </item>
-                            <item>
-                              <spacer name="horizontalSpacer_38">
-                                <property name="orientation">
-                                  <enum>Qt::Horizontal</enum>
-                                </property>
-                                <property name="sizeHint" stdset="0">
-                                  <size>
-                                    <width>40</width>
-                                    <height>20</height>
-                                  </size>
-                                </property>
-                              </spacer>
-                            </item>
-                            <item>
-                              <spacer name="horizontalSpacer_39">
-                                <property name="orientation">
-                                  <enum>Qt::Horizontal</enum>
-                                </property>
-                                <property name="sizeHint" stdset="0">
-                                  <size>
-                                    <width>40</width>
-                                    <height>20</height>
-                                  </size>
-                                </property>
-                              </spacer>
-                            </item>
-                            <item>
-                              <widget class="QLabel" name="label_65">
-                                <property name="text">
-                                  <string>Start</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QLineEdit" name="stripTransformStart">
-                                <property name="alignment">
-                                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QLabel" name="label_71">
-                                <property name="text">
-                                  <string>End</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QLineEdit" name="stripTransformEnd">
-                                <property name="alignment">
-                                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                                </property>
-                              </widget>
-                            </item>
-                          </layout>
-                        </item>
-                        <item row="4" column="0">
-                          <spacer name="verticalSpacer">
-                            <property name="orientation">
-                              <enum>Qt::Vertical</enum>
-                            </property>
-                            <property name="sizeHint" stdset="0">
-                              <size>
-                                <width>20</width>
-                                <height>40</height>
-                              </size>
-                            </property>
-                          </spacer>
-                        </item>
-                        <item row="5" column="0" colspan="2">
+                        <item row="6" column="0" colspan="2">
                           <layout class="QHBoxLayout" name="horizontalLayout_12">
                             <item>
                               <spacer name="horizontalSpacer_10">
                                 <property name="orientation">
                                   <enum>Qt::Horizontal</enum>
                                 </property>
                                 <property name="sizeHint" stdset="0">
@@ -4878,28 +4872,48 @@
                               <widget class="QCheckBox" name="invertMatrix_1">
                                 <property name="text">
                                   <string>Invert Matrix</string>
                                 </property>
                               </widget>
                             </item>
                             <item>
+                              <widget class="QCheckBox" name="autobaselineBox">
+                                <property name="text">
+                                  <string>Autobaseline</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
                               <spacer name="horizontalSpacer_25">
                                 <property name="orientation">
                                   <enum>Qt::Horizontal</enum>
                                 </property>
                                 <property name="sizeHint" stdset="0">
                                   <size>
                                     <width>40</width>
                                     <height>20</height>
                                   </size>
                                 </property>
                               </spacer>
                             </item>
                           </layout>
                         </item>
+                        <item row="5" column="0">
+                          <spacer name="verticalSpacer">
+                            <property name="orientation">
+                              <enum>Qt::Vertical</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>20</width>
+                                <height>40</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
                       </layout>
                     </widget>
                     <widget class="QWidget" name="dim2tab">
                       <attribute name="title">
                         <string>Dim2</string>
                       </attribute>
                       <layout class="QGridLayout" name="gridLayout_7">
@@ -6104,15 +6118,19 @@
                       <widget class="QLabel" name="label_48">
                         <property name="text">
                           <string>phaseReference Experiment</string>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="QSpinBox" name="phRefExp"/>
+                      <widget class="QSpinBox" name="phRefExp">
+                        <property name="maximum">
+                          <number>99999</number>
+                        </property>
+                      </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_49">
                         <property name="text">
                           <string>Colour</string>
                         </property>
                       </widget>
@@ -6431,15 +6449,33 @@
                   <widget class="QPushButton" name="startNotebookButton">
                     <property name="text">
                       <string>(Re-)Start Notebook Server</string>
                     </property>
                   </widget>
                 </item>
                 <item row="0" column="0" colspan="6">
-                  <widget class="QWebEngineView2" name="helpView" native="true"/>
+                  <widget class="QWebEngineView2" name="helpView" native="true">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="maximumSize">
+                      <size>
+                        <width>16777215</width>
+                        <height>16777215</height>
+                      </size>
+                    </property>
+                    <property name="font">
+                      <font>
+                        <pointsize>8</pointsize>
+                      </font>
+                    </property>
+                  </widget>
                 </item>
                 <item row="1" column="4">
                   <spacer name="horizontalSpacer_24">
                     <property name="orientation">
                       <enum>Qt::Horizontal</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
@@ -6521,15 +6557,15 @@
     </widget>
     <widget class="QMenuBar" name="menuBar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1914</width>
-          <height>24</height>
+          <height>22</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionSave"/>
@@ -7010,15 +7046,15 @@
       </property>
     </action>
     <action name="actionExecute_Script">
       <property name="text">
         <string>Execute Script</string>
       </property>
       <property name="shortcut">
-        <string>Meta+X</string>
+        <string>Ctrl+X</string>
       </property>
     </action>
     <action name="actionScale_2D_Spectrum_Up">
       <property name="text">
         <string>Scale 2D Spectrum Up</string>
       </property>
       <property name="shortcut">
```

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.9.0/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 qtmetabolabpy/__init__.py
 qtmetabolabpy/__main__.py
+qtmetabolabpy/qtMetaboLabPy.py
 qtmetabolabpy.egg-info/PKG-INFO
 qtmetabolabpy.egg-info/SOURCES.txt
 qtmetabolabpy.egg-info/dependency_links.txt
 qtmetabolabpy.egg-info/entry_points.txt
 qtmetabolabpy.egg-info/requires.txt
 qtmetabolabpy.egg-info/top_level.txt
+qtmetabolabpy/bash/fix_pyside2
 qtmetabolabpy/mlStarter/Icon
 qtmetabolabpy/mlStarter/Contents/Info.plist
 qtmetabolabpy/mlStarter/Contents/PkgInfo
 qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
 qtmetabolabpy/ui/metabolabpy_mainwindow.ui
```

### Comparing `qtmetabolabpy-0.8.9/setup.py` & `qtmetabolabpy-0.9.0/setup.py`

 * *Files identical despite different names*

