# Comparing `tmp/slrfield-0.2.0-py3-none-any.whl.zip` & `tmp/slrfield-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20126 bytes, number of entries: 16
--rw-r--r--  2.0 unx      727 b- defN 22-Feb-23 14:49 slrfield/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-23 13:33 slrfield/cpf/__init__.py
--rw-r--r--  2.0 unx    18310 b- defN 22-Feb-23 13:45 slrfield/cpf/cpf_download.py
+Zip file size: 19854 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      739 b- defN 23-Jul-16 13:53 slrfield/__init__.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-11 03:36 slrfield/cpf/__init__.py
+-rw-r--r--  2.0 unx    18486 b- defN 23-Jul-16 14:41 slrfield/cpf/cpf_download.py
 -rw-r--r--  2.0 unx    18944 b- defN 22-Feb-24 06:56 slrfield/cpf/cpf_interpolate.py
 -rw-r--r--  2.0 unx     5052 b- defN 22-Feb-23 14:01 slrfield/cpf/cpf_read.py
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-23 14:01 slrfield/slrclasses/__init__.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-11 03:36 slrfield/slrclasses/__init__.py
 -rw-r--r--  2.0 unx     9379 b- defN 22-Feb-24 06:45 slrfield/slrclasses/cpfclass.py
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-23 14:18 slrfield/utils/__init__.py
--rw-r--r--  2.0 unx     1488 b- defN 22-Feb-23 14:18 slrfield/utils/data_download.py
--rw-r--r--  2.0 unx      291 b- defN 22-Feb-23 01:47 slrfield/utils/data_prepare.py
--rw-r--r--  2.0 unx     2425 b- defN 22-Feb-23 01:41 slrfield/utils/try_download.py
--rw-r--r--  2.0 unx     1073 b- defN 22-Feb-24 07:18 slrfield-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9357 b- defN 22-Feb-24 07:18 slrfield-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-24 07:18 slrfield-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Feb-24 07:18 slrfield-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1314 b- defN 22-Feb-24 07:18 slrfield-0.2.0.dist-info/RECORD
-16 files, 68461 bytes uncompressed, 17948 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-11 03:36 slrfield/utils/__init__.py
+-rw-r--r--  2.0 unx     2618 b- defN 23-Jul-16 14:06 slrfield/utils/data_download.py
+-rw-r--r--  2.0 unx      429 b- defN 23-Jul-16 14:29 slrfield/utils/data_prepare.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jul-16 14:28 slrfield/utils/try_download.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-16 15:44 slrfield-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9430 b- defN 23-Jul-16 15:44 slrfield-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 15:44 slrfield-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-16 15:44 slrfield-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1316 b- defN 23-Jul-16 15:44 slrfield-0.2.1.dist-info/RECORD
+16 files, 68136 bytes uncompressed, 17676 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: slrfield/utils/data_prepare.py
 Comment: 
 
 Filename: slrfield/utils/try_download.py
 Comment: 
 
-Filename: slrfield-0.2.0.dist-info/LICENSE
+Filename: slrfield-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: slrfield-0.2.0.dist-info/METADATA
+Filename: slrfield-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: slrfield-0.2.0.dist-info/WHEEL
+Filename: slrfield-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: slrfield-0.2.0.dist-info/top_level.txt
+Filename: slrfield-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: slrfield-0.2.0.dist-info/RECORD
+Filename: slrfield-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slrfield/__init__.py

```diff
@@ -10,9 +10,9 @@
 4. Predict the azimuth, altitude, distance of targets, and the time of flight for laser pulse etc.;
 """
 
 from .cpf.cpf_download import cpf_download,get_cpf_satlist
 from .slrclasses.cpfclass import CPF
 from .utils import data_prepare
 
-# Load and update the EOP and time files
-data_prepare.time_load()
+# Load and update the EOP file and Leap Second file
+data_prepare.iers_load()
```

## slrfield/cpf/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 2320 5468 6973 2066 696c 6520 6973 2069  # This file is i
+00000010: 6e74 656e 7469 6f6e 616c 6c79 2065 6d70  ntentionally emp
+00000020: 7479                                     ty
```

## slrfield/cpf/cpf_download.py

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from ftplib import FTP
 import requests
 from bs4 import BeautifulSoup
 from astropy.time import Time
 from warnings import warn
 
-from ..utils.try_download import tqdm_ftp,tqdm_request_cpf
+from ..utils.try_download import wget_download
 
 def download_bycurrent(source,satnames=None,keep=True):
     """
     Download the latest CPF ephemeris files at the current moment.
 
     Usage: 
         server,dir_cpf_from, dir_cpf_to,cpf_files = download_bycurrent('CDDIS')
@@ -256,49 +256,53 @@
     missing_cpf_files = []
     
     if date is None:
         server,dir_cpf_from, dir_cpf_to,cpf_files = download_bycurrent(source,satnames,keep)  
 
         if source == 'CDDIS':
             for cpf_file in cpf_files:
+                dir_cpf_file = dir_cpf_to + cpf_file
                 url = server+dir_cpf_from+cpf_file
                 desc = 'Downloading {:s}'.format(cpf_file)
-                missing_cpf_file = tqdm_request_cpf(url,dir_cpf_to,cpf_file,desc)
+                missing_cpf_file = wget_download(url,dir_cpf_file,desc)
                 if missing_cpf_file is not None: missing_cpf_files.append(missing_cpf_file)
                 
         if source == 'EDC':
             ftp = FTP(server,timeout=200)    
             ftp.login()  
             ftp.cwd(dir_cpf_from) 
             for cpf_file in cpf_files:
+                dir_cpf_file = dir_cpf_to + cpf_file
                 desc = 'Downloading {:s}'.format(cpf_file)
-                missing_cpf_file = tqdm_ftp(ftp,dir_cpf_to,cpf_file,desc)
+                missing_cpf_file = wget_download(ftp,dir_cpf_file,desc)
                 if missing_cpf_file is not None: missing_cpf_files.append(missing_cpf_file)
 
             ftp.quit()  
             ftp.close()    
                 
     else:    
         server,dirs_cpf_from, dir_cpf_to,cpf_files = download_bydate(source,date,satnames,keep)  
 
         if source == 'CDDIS':
             for dir_cpf_from,cpf_file in zip(dirs_cpf_from,cpf_files):
+                dir_cpf_file = dir_cpf_to + cpf_file
                 url = server+dir_cpf_from+cpf_file
                 desc = 'Downloading {:s}'.format(cpf_file)
-                missing_cpf_file = tqdm_request_cpf(url,dir_cpf_to,cpf_file,desc)
+                missing_cpf_file = wget_download(url,dir_cpf_file,desc)
                 if missing_cpf_file is not None: missing_cpf_files.append(missing_cpf_file)
 
         if source == 'EDC': 
             ftp = FTP(server,timeout=200)    
             ftp.login()  
 
             for dir_cpf_from,cpf_file in zip(dirs_cpf_from,cpf_files):
+                dir_cpf_file = dir_cpf_to + cpf_file
                 ftp.cwd(dir_cpf_from)
                 desc = 'Downloading {:s}'.format(cpf_file)
-                missing_cpf_file = tqdm_ftp(ftp,dir_cpf_to,cpf_file,desc)
+                missing_cpf_file = wget_download(ftp,dir_cpf_file,desc)
                 if missing_cpf_file is not None: missing_cpf_files.append(missing_cpf_file)
 
             ftp.quit()  
             ftp.close()    
 
     return dir_cpf_to,cpf_files,missing_cpf_files
```

## slrfield/slrclasses/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 2320 5468 6973 2066 696c 6520 6973 2069  # This file is i
+00000010: 6e74 656e 7469 6f6e 616c 6c79 2065 6d70  ntentionally emp
+00000020: 7479                                     ty
```

## slrfield/utils/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 2320 5468 6973 2066 696c 6520 6973 2069  # This file is i
+00000010: 6e74 656e 7469 6f6e 616c 6c79 2065 6d70  ntentionally emp
+00000020: 7479                                     ty
```

## slrfield/utils/data_download.py

```diff
@@ -1,48 +1,59 @@
 
 from datetime import datetime,timedelta
 from os import path,makedirs,remove
 from pathlib import Path
-from ftplib import FTP
 
-from .try_download import tqdm_ftp
+from .try_download import wget_download 
 
-def download_eop(out_days=7,dir_to=None):
+def download_iers(out_days=7,dir_to=None):
     """
-    Download or update the Earth Orientation Parameters(EOP) file from IERS
+    Download or update the Earth Orientation Parameters(EOP) file and Leap Second file from IERS
 
     Usage: 
-        >>> eop_file = download_eop()
-
-    Parameters: 
-        out_days -> [int, default = 7] Update cycle of the EOP file
-        dir_to   -> [str, default = None] Directory for storing EOP file
-    
+        >>> dir_to,dir_eop_file,dir_leapsecond_file = download_iers()
+    Inputs: 
+        out_days -> [int, optional, default = 7] Updating cycle of the IERS files
+        dir_to   -> [str, optional, default = None] Directory for storing EOP file
     Outputs: 
-        eop_file -> [str] Path of the EOP file
+        dir_to -> [str] Directory of the IERS files
+        dir_eop_file -> [str] Path of the EOP file
+        dir_leapsecond_file -> [str] Path of the Leap Second file
     """
     if dir_to is None:
         home = str(Path.home())
-        dir_to = home + '/src/eop-data/'
+        dir_to = home + '/src/iers/'
     
-    file = 'finals2000A.all'
-    dir_file = dir_to + file
+    eop_file = 'finals2000A.all'
+    leapsecond_file = 'Leap_Second.dat'
+    dir_eop_file = dir_to + eop_file
+    dir_leapsecond_file = dir_to + leapsecond_file
 
-    server = 'ftp.iers.org'
-    src_dir = '~/products/eop/rapid/standard/'
+    url_eop = 'https://datacenter.iers.org/products/eop/rapid/standard/finals2000A.all'
+    url_leapsecond = 'https://hpiers.obspm.fr/iers/bul/bulc/Leap_Second.dat'
 
     if not path.exists(dir_to): makedirs(dir_to)
-    if not path.exists(dir_file):
-        ftp_access(server,src_dir)
-        desc = "Downloading the latest EOP '{:s}' from IERS".format(file)
-        tqdm_ftp(ftp,dir_to,file,desc)
+    if not path.exists(dir_eop_file):
+        desc = "Downloading the latest EOP file '{:s}' from IERS".format(eop_file)
+        wget_out = wget_download(url_eop,dir_eop_file,desc)
+    else:
+        modified_time = datetime.fromtimestamp(path.getmtime(dir_eop_file))
+        if datetime.now() > modified_time + timedelta(days=out_days):
+            remove(dir_eop_file)
+            desc = "Updating the EOP file '{:s}' from IERS".format(eop_file)
+            wget_out = wget_download(url_eop,dir_eop_file,desc)
+        else:
+            print("The EOP file '{:s}' in {:s} is already the latest.".format(eop_file,dir_to)) 
+
+    if not path.exists(dir_leapsecond_file):
+        desc = "Downloading the latest Leap Second file '{:s}' from IERS".format(leapsecond_file)
+        wget_out = wget_download(url_leapsecond,dir_leapsecond_file,desc)
     else:
-        modified_time = datetime.fromtimestamp(path.getmtime(dir_file))
+        modified_time = datetime.fromtimestamp(path.getmtime(dir_leapsecond_file))
         if datetime.now() > modified_time + timedelta(days=out_days):
-            remove(dir_file)
-            ftp_access(server,src_dir)
-            desc = "Updating EOP '{:s}' from IERS".format(file)
-            tqdm_ftp(ftp,dir_to,file,desc)
+            remove(dir_leapsecond_file)
+            desc = "Updating the Leap Second file '{:s}' from IERS".format(leapsecond_file)
+            wget_out = wget_download(url_leapsecond,dir_leapsecond_file,desc)
         else:
-            print("EOP '{0:s}' in {1:s} is already the latest.".format(file,dir_to)) 
+            print("The Leap Second file '{:s}' in {:s} is already the latest.".format(leapsecond_file,dir_to))        
 
-    return dir_file  
+    return dir_to,dir_eop_file,dir_leapsecond_file
```

## slrfield/utils/data_prepare.py

```diff
@@ -1,11 +1,11 @@
 from astropy.utils import iers as iers_astropy
-from .data_download import download_eop
+from .data_download import download_iers
 
-def time_load():
+def iers_load():
 
     # load the EOP file
-    eop_file = download_eop()
-
-    # for astropy
+    dir_iers,eop_file,leapsecond_file = download_iers()
+    iers_astropy.conf.auto_download = False
     iers_a = iers_astropy.IERS_A.open(eop_file)
-    eop_table = iers_astropy.earth_orientation_table.set(iers_a)
+    leapsecond = iers_astropy.LeapSeconds.from_iers_leap_seconds(leapsecond_file)
+    eop_table = iers_astropy.earth_orientation_table.set(iers_a)
```

## slrfield/utils/try_download.py

```diff
@@ -1,66 +1,19 @@
-from os import remove
-import requests
-from tqdm import tqdm
-from colorama import Fore
-from time import sleep
+import wget
 
-def tqdm_ftp(ftp,dir_to,file,desc):
+def wget_download(url,dir_file,desc=None):
     """
-    Try to download files from remote server by ftp with a colored progress bar.
-    """
-    dir_file = dir_to + file
-    total_size = int(ftp.size(file))
-    bar_format = "{l_bar}%s{bar}%s{r_bar}" % (Fore.BLUE, Fore.RESET)
+    download files by wget command
 
-    for idownload in range(5):
-        try:
-            local_file =  open(dir_file, 'wb')
-            pos = local_file.tell()
-            pbar = tqdm(desc = desc,total=total_size,unit='B',unit_scale=True,position=0,initial=pos,bar_format=bar_format)
-            def progressbar(chunk):
-                local_file.write(chunk)
-                pbar.update(len(chunk))
-            res = ftp.retrbinary('RETR ' + file, progressbar) # RETR is an FTP command
-            break       
-        except:
-            sleep(2)
-            if idownload == 4:
-                remove(dir_file)
-                print('No response, skip {:s}'.format(file))
-        finally:
-            pbar.close()
-            local_file.close()       
+    Inputs:
+        url -> [str] URL of the file to be downloaded
+        dir_file -> [str] path of the file to be downloaded
+        desc -> [str,optional] description of the downloading   
+    Outpits:
+        wget_out -> [str] path of the file downloaded
 
-def tqdm_request_cpf(url,dir_cpf_to,cpf_file,desc):
-    """
-    Try to download cpf files from url with a colored progress bar.
     """
-    block_size = 1024*10
-    missing_flag = False
-    bar_format = "{l_bar}%s{bar}%s{r_bar}" % (Fore.BLUE, Fore.RESET)
-    for idownload in range(5):
-        try:
-            local_file = open(dir_cpf_to + cpf_file, 'wb')
-            pos = local_file.tell()
-            res = requests.get(url,stream=True,timeout=200,headers={'Accept-Encoding': None,'Range': f'bytes={pos}-'})
-            total_size = int(res.headers.get('Content-Length'))
-            pbar = tqdm(desc = desc,total=total_size,unit='B',unit_scale=True,bar_format = bar_format,position=0,initial=pos)
-            for chunk in res.iter_content(block_size):
-                local_file.write(chunk)  
-                pbar.update(len(chunk))   
-            pbar.close()   
-            res.close()  
-            break
-        except: 
-            sleep(3)
-            if idownload == 4:
-                remove(dir_cpf_to + cpf_file)
-                print('No response, skip {:s}'.format(cpf_file)) 
-                missing_flag = True
-        finally:    
-            local_file.close() 
-            if missing_flag: 
-                return cpf_file  
-            else:
-                return None      
-                      
+    if desc: print(desc)
+    wget_out = wget.download(url,dir_file)
+    print()
+
+    return wget_out
```

## Comparing `slrfield-0.2.0.dist-info/LICENSE` & `slrfield-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `slrfield-0.2.0.dist-info/METADATA` & `slrfield-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: slrfield
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to handle the SLR(Satellite Laser Ranging) data
 Home-page: https://github.com/lcx366/SLRfield
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: SLR,CPF
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: astropy (>=4.3.1)
-Requires-Dist: tqdm
-Requires-Dist: colorama
+Requires-Dist: wget
 Requires-Dist: beautifulsoup4
 
 # Welcome to the SLRfield package
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/slrfield.svg)](https://pypi.python.org/pypi/slrfield/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/slrfield.svg)](https://pypi.python.org/pypi/slrfield/) [![PyPI status](https://img.shields.io/pypi/status/slrfield.svg)](https://pypi.python.org/pypi/slrfield/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/SLRfield.svg)](https://GitHub.com/lcx366/SLRfield/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/SLRfield/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/SLRfield.svg)](https://github.com/lcx366/SLRfield/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/pystmos/badge/?version=latest)](http://slrfield.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/SLRfield.svg?branch=master)](https://travis-ci.org/lcx366/SLRfield)
 
 This package is an archive of scientific routines for data processing related to SLR(Satellite Laser Ranging). 
@@ -155,14 +153,17 @@
 t_increment = 5 # second
 
 cpf_data_cddis.pred_xyz(t_start,t_end,t_increment)
 ```
 
 ## Change log
 
+- **0.2.1 — jul 16, 2023**
+  - Added time system for loading/updating the EOP file and Leap Second file from IERS
+
 - **0.2.0 — Feb 24, 2022**
   
   - Added support for calculating the cartesian coordinates of targets in GCRF
   
   - Added support for quickly computing the passing-site prediction 
   
   - Removed the module related to TLE data
@@ -212,9 +213,7 @@
 ## Reference
 
 - [Python package for satellite laser ranging file formats](https://github.com/dronir/SLRdata)
 - [Consolidated Laser Ranging Prediction Format Version 1.01](https://ilrs.gsfc.nasa.gov/docs/2006/cpf_1.01.pdf)
 - [sample code](https://ilrs.gsfc.nasa.gov/docs/2017/cpf_sample_code_v1.01d.tgz) on [ILRS](https://ilrs.gsfc.nasa.gov/data_and_products/formats/cpf.html)
   
   
-
-
```

## Comparing `slrfield-0.2.0.dist-info/RECORD` & `slrfield-0.2.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-slrfield/__init__.py,sha256=2RV8q4iNTh7l6NBiIa3kXHM1zbXLjR6SnaaVf1_r3R4,727
-slrfield/cpf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-slrfield/cpf/cpf_download.py,sha256=pXWTpieMCBWpHoZyhS7vbBrs0qStr5AGTfmjbqGbKUo,18310
+slrfield/__init__.py,sha256=6T6pXLyayJbHOgnm0m2e3SbFg90JndsNeGjowV6V13U,739
+slrfield/cpf/__init__.py,sha256=KlZOXnhH7TwEHuyTopyhlpxWXyBshLIShcpNLPs6G-0,34
+slrfield/cpf/cpf_download.py,sha256=78yE8bEnqw4w6hZKnDLPk_nQj0CanpiweARhhB16OqY,18486
 slrfield/cpf/cpf_interpolate.py,sha256=P31pN4cs_aAIfmTiMb9oUxGTiSfR5HNlm53VK4WjxQk,18944
 slrfield/cpf/cpf_read.py,sha256=SU9MF4naiBLLQuWeglKcycem55BOEHwX124WmQiVi70,5052
-slrfield/slrclasses/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+slrfield/slrclasses/__init__.py,sha256=KlZOXnhH7TwEHuyTopyhlpxWXyBshLIShcpNLPs6G-0,34
 slrfield/slrclasses/cpfclass.py,sha256=gOAT7wp8zHkl87mPXevc8TzbLuC2hMiCQvFKF5JvGjo,9379
-slrfield/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-slrfield/utils/data_download.py,sha256=k5kpw2wYCMuEtPWg2YdUHopKoJcx3uq5-o3sAoidPHk,1488
-slrfield/utils/data_prepare.py,sha256=5hnCLpsuW71k-dEW0-vf0EV_UlzNoBnkJKkVmIVr1Z8,291
-slrfield/utils/try_download.py,sha256=Wr94CdbM2A5okxYKMoJGbyuDQAxplsxx7xzbepTZS68,2425
-slrfield-0.2.0.dist-info/LICENSE,sha256=K9ixHn0oyM1250Q4v3bXfUN43iykKHBrUlwr-IzZlJg,1073
-slrfield-0.2.0.dist-info/METADATA,sha256=dyDRj7H_SUSDcY5M3qaS1MOBhzFjscAx-36GodItwcg,9357
-slrfield-0.2.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-slrfield-0.2.0.dist-info/top_level.txt,sha256=cFRz41ekdADfHDrJ8qsRr2XKv73ZKHOipj_U7C-eSGY,9
-slrfield-0.2.0.dist-info/RECORD,,
+slrfield/utils/__init__.py,sha256=KlZOXnhH7TwEHuyTopyhlpxWXyBshLIShcpNLPs6G-0,34
+slrfield/utils/data_download.py,sha256=vp9JEoK9w90mrpYpSvMt25ppF-GtX3KZ8bDbffsH6NU,2618
+slrfield/utils/data_prepare.py,sha256=7GZJ84m8Tpjhbb5xf1dUnw8_Cv5I3D9d7a1y1IGR4cM,429
+slrfield/utils/try_download.py,sha256=S8ivqwc92KORGeDri3-v9p66lzMBWGtual18bko1P1I,467
+slrfield-0.2.1.dist-info/LICENSE,sha256=K9ixHn0oyM1250Q4v3bXfUN43iykKHBrUlwr-IzZlJg,1073
+slrfield-0.2.1.dist-info/METADATA,sha256=DaZ2nwjVdE89LCs6YQIMUUPSAIHMtyKmejtoDphl9iw,9430
+slrfield-0.2.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+slrfield-0.2.1.dist-info/top_level.txt,sha256=cFRz41ekdADfHDrJ8qsRr2XKv73ZKHOipj_U7C-eSGY,9
+slrfield-0.2.1.dist-info/RECORD,,
```

