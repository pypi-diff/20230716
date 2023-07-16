# Comparing `tmp/pymovie-3.8.0.tar.gz` & `tmp/pymovie-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymovie-3.8.0.tar", last modified: Thu Jul 13 21:33:04 2023, max compression
+gzip compressed data, was "pymovie-3.8.1.tar", last modified: Sun Jul 16 16:55:25 2023, max compression
```

## Comparing `pymovie-3.8.0.tar` & `pymovie-3.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 21:33:04.007579 pymovie-3.8.0/
--rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.8.0/LICENSE
--rw-rw-rw-   0        0        0     1474 2023-07-13 21:33:04.007579 pymovie-3.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.8.0/README.rst
--rw-rw-rw-   0        0        0       80 2023-07-13 21:33:04.012588 pymovie-3.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:33:03.974509 pymovie-3.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 21:33:03.998579 pymovie-3.8.0/src/pymovie/
--rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.8.0/src/pymovie/NE3Lut.p
--rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.8.0/src/pymovie/PyMovie-doc.pdf
--rw-rw-rw-   0        0        0   633433 2023-07-13 21:31:24.000000 pymovie-3.8.0/src/pymovie/PyMovie-info.pdf
--rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/PyMovie.bat
--rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.8.0/src/pymovie/SER.py
--rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.8.0/src/pymovie/__init__.py
--rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.8.0/src/pymovie/alias_lnk_resolver.py
--rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.8.0/src/pymovie/aperture.py
--rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.8.0/src/pymovie/apertureEdit.py
--rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.8.0/src/pymovie/apertureEditDialog.py
--rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.8.0/src/pymovie/apertureNameDialog.py
--rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.8.0/src/pymovie/aperturesFileTagDialog.py
--rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/astrometry_client.py
--rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.8.0/src/pymovie/checkForNewerVersion.py
--rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.8.0/src/pymovie/gammaUtils.py
--rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.8.0/src/pymovie/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.8.0/src/pymovie/helpDialog.py
--rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.8.0/src/pymovie/hotPixelDialog.py
--rw-rw-rw-   0        0        0   456966 2023-07-13 21:23:15.000000 pymovie-3.8.0/src/pymovie/main.py
--rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.8.0/src/pymovie/ocr.py
--rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.8.0/src/pymovie/ocrCharacterBox.py
--rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.8.0/src/pymovie/ocrProfileNameDialog.py
--rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.8.0/src/pymovie/play-Temp.py
--rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.8.0/src/pymovie/play-introspection.py
--rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.8.0/src/pymovie/run-pymovie-mac.bat
--rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.8.0/src/pymovie/selectHotPixelProfile.py
--rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.8.0/src/pymovie/selectProfile.py
--rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.8.0/src/pymovie/stacker.py
--rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.8.0/src/pymovie/starPositionDialog.py
--rw-rw-rw-   0        0        0       36 2023-07-13 20:33:37.000000 pymovie-3.8.0/src/pymovie/version.py
--rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.8.0/src/pymovie/wcs_helper_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:33:04.006580 pymovie-3.8.0/src/pymovie.egg-info/
--rw-rw-rw-   0        0        0     1474 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.8.0/src/pymovie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      247 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 21:33:03.000000 pymovie-3.8.0/src/pymovie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:25.888417 pymovie-3.8.1/
+-rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1474 2023-07-16 16:55:25.888417 pymovie-3.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.8.1/README.rst
+-rw-rw-rw-   0        0        0       80 2023-07-16 16:55:25.904024 pymovie-3.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:25.716520 pymovie-3.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:25.888417 pymovie-3.8.1/src/pymovie/
+-rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.8.1/src/pymovie/NE3Lut.p
+-rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.8.1/src/pymovie/PyMovie-doc.pdf
+-rw-rw-rw-   0        0        0   634348 2023-07-16 16:53:34.000000 pymovie-3.8.1/src/pymovie/PyMovie-info.pdf
+-rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.8.1/src/pymovie/PyMovie.bat
+-rw-rw-rw-   0        0        0     6283 2023-05-12 20:27:48.000000 pymovie-3.8.1/src/pymovie/SER.py
+-rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.8.1/src/pymovie/__init__.py
+-rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.8.1/src/pymovie/alias_lnk_resolver.py
+-rw-rw-rw-   0        0        0     6094 2023-05-18 11:24:11.000000 pymovie-3.8.1/src/pymovie/aperture.py
+-rw-rw-rw-   0        0        0    15254 2023-06-27 02:54:33.000000 pymovie-3.8.1/src/pymovie/apertureEdit.py
+-rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.8.1/src/pymovie/apertureEditDialog.py
+-rw-rw-rw-   0        0        0     3962 2023-06-26 17:44:10.000000 pymovie-3.8.1/src/pymovie/apertureNameDialog.py
+-rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.8.1/src/pymovie/aperturesFileTagDialog.py
+-rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.8.1/src/pymovie/astrometry_client.py
+-rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.8.1/src/pymovie/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.8.1/src/pymovie/gammaUtils.py
+-rw-rw-rw-   0        0        0   233704 2023-06-26 17:44:13.000000 pymovie-3.8.1/src/pymovie/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-24 18:07:02.000000 pymovie-3.8.1/src/pymovie/helpDialog.py
+-rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.8.1/src/pymovie/hotPixelDialog.py
+-rw-rw-rw-   0        0        0   459752 2023-07-16 16:48:45.000000 pymovie-3.8.1/src/pymovie/main.py
+-rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.8.1/src/pymovie/ocr.py
+-rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.8.1/src/pymovie/ocrCharacterBox.py
+-rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.8.1/src/pymovie/ocrProfileNameDialog.py
+-rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.8.1/src/pymovie/play-Temp.py
+-rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.8.1/src/pymovie/play-introspection.py
+-rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.8.1/src/pymovie/run-pymovie-mac.bat
+-rw-rw-rw-   0        0        0     4271 2023-05-31 13:21:53.000000 pymovie-3.8.1/src/pymovie/selectHotPixelProfile.py
+-rw-rw-rw-   0        0        0     3675 2023-05-31 04:05:11.000000 pymovie-3.8.1/src/pymovie/selectProfile.py
+-rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.8.1/src/pymovie/stacker.py
+-rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.8.1/src/pymovie/starPositionDialog.py
+-rw-rw-rw-   0        0        0       36 2023-07-16 16:32:46.000000 pymovie-3.8.1/src/pymovie/version.py
+-rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.8.1/src/pymovie/wcs_helper_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:55:25.888417 pymovie-3.8.1/src/pymovie.egg-info/
+-rw-rw-rw-   0        0        0     1474 2023-07-16 16:55:25.000000 pymovie-3.8.1/src/pymovie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-07-16 16:55:25.000000 pymovie-3.8.1/src/pymovie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:55:25.000000 pymovie-3.8.1/src/pymovie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.8.1/src/pymovie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      247 2023-07-16 16:55:25.000000 pymovie-3.8.1/src/pymovie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 16:55:25.000000 pymovie-3.8.1/src/pymovie.egg-info/top_level.txt
```

### Comparing `pymovie-3.8.0/LICENSE` & `pymovie-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/PKG-INFO` & `pymovie-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.8.0
+Version: 3.8.1
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.8.0/setup.py` & `pymovie-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/PyMovie-doc.pdf` & `pymovie-3.8.1/src/pymovie/PyMovie-doc.pdf`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/PyMovie-info.pdf` & `pymovie-3.8.1/src/pymovie/PyMovie-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -3,14 +3,18 @@
 For general information about the program (with usage tips), click on the
 Documentation button that is in the Help tab panel. A pdf will be launched – it
 is out-of-date, but still a bit useful.
 Note: there is a series of (grossly out-of-date and nearly useless and possibly
 confusing) YouTube tutorials available. Go to
 http://occultations.org/observing/software/pymovie for access to these videos.
 PyMovie version history
+Version 3.8.1
+16 July 2023
+• Moved finder frames, ocr data, and aperture groups into sub-directories within the
+observation folder to tidy things up a bit.
 Version 3.8.0
 13 July 2023
 • If data was already gathered, then an aperture was renamed to psf-star, the NRE
 analysis would not run UNLESS the user manually cleared the already gathered data.
 This version detects that case and starts the psf gathering process as expected.
 •
 
@@ -34,17 +38,17 @@
 30 June 2023
 • Changed the centering/tracking of fixed radius masks (in static apertures) from
 centering on the single brightest pixel (introduced in version 3.7.0) to a mass centroid
 calculated using the nThBrightPixel algorithm conceived and tested by A. G. Basden
 (reported in Centroids using Brightest Pixel Algorithm by A. G. Basden, et al, MNRAS,
 2011)
 This operates by finding the n brightest pixels in the mask, setting all other pixel values
-to zero, and calculating the x,y centroid of the remaining ‘mass’.
 
-•
+to zero, and calculating the x,y centroid of the remaining ‘mass’.
+•
 
 Optimal extraction for imaging photometry was introduced by Tim Naylor in his 1998
 paper titled: An optimal extraction algorithm for imaging photometry.[ Mon. Not.
 R. Astron. Soc. 296, 339-346 (1998)].
 Naylor's algorithm utilizes a two-dimensional gaussian as an approximation to the psf
 of stars in the image and demonstrates that this is an effective approximation in practice. Using this analytic psf, the paper describes how to calculate a weighted mask that
 lowers the noise in a star intensity measurement by giving a larger weight to those
@@ -80,18 +84,18 @@
 problem in the past and recently, my tests using their data (but NOT their aperture
 placement) consistently found ‘no problem’. My tests were unlucky enough to have had
 an aperture placement that ‘worked’ so I found no problem.
 It is also the case that the problem is only visually identifiable for very short events that
 have a good snr, so it is easily overlooked.
 I believe that this bug has always been present – just undetected and confirmed until
 now.
-Version 3.7.3 11 February 2023
-• Restored the font size of the text box (lower left) that had inadvertently been increased
 
-to 13 back to 9
+Version 3.7.3 11 February 2023
+• Restored the font size of the text box (lower left) that had inadvertently been increased
+to 13 back to 9
 •
 
 Restored use of pyqtgraph 0.12.4
 
 Version 3.7.0 7 February 2023
 • Added an additional tracking feature to static apertures. In previous versions, the fixed
 radius circular sampling mask was always centered inside a static aperture. Tracking
@@ -123,18 +127,18 @@
 Thumbnail source.
 Version 3.6.6 7 September 2022
 • Removed instructions for pipenv installations (we have killed that project before it is
 actually born)
 Version 3.6.5 5 September 2022
 • No code changes. Added ‘wheel’ to required packages to better support pure Python
 installations (no Anaconda3).
-Version 3.6.3 7 August 2022
-• Added messages upon app closing indicating normal program shutdown with advice to
 
-user to ignore any subsequent messages about QBasic timers as they are harmless.
+Version 3.6.3 7 August 2022
+• Added messages upon app closing indicating normal program shutdown with advice to
+user to ignore any subsequent messages about QBasic timers as they are harmless.
 Version 3.6.2 7 August 2022
 • At one point in time (see version 3.2.0 and 3.2.1 discussion) a ‘hack’ was introduced to
 get Windows to preserve any image scaling and positioning during frame changes. The
 hack was to expand and contract the width of the image by 1 pixel. This ‘dance’ is
 sometime apparent. This version removes that ‘hack’ as it appears no longer
 necessary on Win10 or Win11.
 Version 3.6.1 7 August 2022
@@ -161,19 +165,19 @@
 • we no longer write a run-pymovie icon to the desktop. This required an Anaconda3
 installation (with Anaconda3 installed in a specific location) which we are working hard
 to avoid.
 Version 3.4.3 21 July 2022
 • removed option to download new version when found. This was done in part to remove
 a sometimes-annoying nag and to pave the way for a new installation procedure that
 does not require an Anaconda3 installation.
-The usual pip install pymovie==x.y.z remains available for the user to install any new
+
+The usual pip install pymovie==x.y.z remains available for the user to install any new
 version at a time of her choosing for the current installation procedure. For the new
 installation procedure, a batch file is provided that prompts for the new version number
-
-– one no longer hs to remember the magic incantation.
+– one no longer hs to remember the magic incantation.
 Version 3.4.2 9Jul2022
 • fixes QMenu() reference issue (created by Qt programmers changing where the
 QMenu() item is found
 Version 3.4.1 22Jun2022
 • cleans up some issues involving the color scale for the thumbnails.
 Version 3.4.0 18Jun2022
 • For some reason, I thought that 16 bit FITS file images should be scaled (divided by)
@@ -205,22 +209,19 @@
 Version 3.3.1
 • adds (in the Image/Plot tab) a checkbox that requests that a Night Eagle 3 video,
 assumed recorded with gamma 0.75, be linearized. When this box is checked, the
 'gamma' response curve of the Night Eagle 3 will be inverted so that the response
 becomes very close to linear.
 Version 3.3.0
 • removes the requirement for a specific version of opencv-python – this was causing
-problems with new Anaconda installs of Python 3.9
-Version 3.2.9
-
-•
 
-fixes bug where meta-data from adv file was being placed in csv file without leading #
+problems with new Anaconda installs of Python 3.9
+Version 3.2.9
+• fixes bug where meta-data from adv file was being placed in csv file without leading #
 character
-
 Version 3.2.7
 • The CMOS Pixels Tool tab is now fully functional.
 There is too much in this tab to explain in this forum – start your education with the
 Click me for help/info button. Then do right clicks on the other controls, starting at the upper
 left and procedding down the column, then move to the upper right.
 •
 
@@ -252,26 +253,23 @@
 uncomfortably.
 Version 3.2.3
 • version 3.2.2 broke the 3d display of Thumbnail One and the robust mean demo. This
 version fixes that issue.
 Version 3.2.2
 • fixed issue where contrast level settings were not being preserved when an analysis
 was started
-•
+
+•
 
 reduced 'blinking' of thumbnail One image during image changes.
 
 Version 3.2.1
-
-•
-
-added an ugly hack to the Windows version in order to make what worked so easily in
+• added an ugly hack to the Windows version in order to make what worked so easily in
 version 3.2.0 on Mac hardware also work on Windows machine – it took me two full
 days to find this 'hack' and still I hate that it's necessary.
-
 Version 3.2.0
 • has changed so that Zoom/Pan state of main image is preserved when switching back
 and forth between a 'finder' image and a frame image
 Version 3.1.6
 • fixes a bug that kept the use of yellow aperture mask (for windshake files) from
 displaying properly in Thumbnail Two
 Version 3.1.5
@@ -297,19 +295,22 @@
 comments
 Version 3.1.0
 • changed GUI layout for Misc tab
 • changed median filter to adjust all horizontal lines to have a median equal the median
 of the row-by-row medians (previously I was adjusting all lines to the maximum of the
 row-by-row medians). This will make the brightness adjustments less radical.
 Version 3.0.9
-• adds options for the user when she starts an analysis and there is already data
+
+•
+
+adds options for the user when she starts an analysis and there is already data
 present: she can ignore the warning and continue because her settings will not
 produce duplicate frames; she clear the data and proceed into the analysis; she can
+stop the analysis.
 
-stop the analysis.
 Version 3.0.8
 • adds clearing of line filter checkbox when new file is loaded. The display of the median
 plot is now a one-time event, as there was a need to clear that data in preparation of a
 new 'run'. This avoids duplicated and overlaid data in that array.
 Version 3.0.7
 • adds a median filter to reduce/eliminate 'line pattern noise' that some cameras exhibit.
 Such 'patterning' appears as row to row differences in brightness – streaks – that are
@@ -337,19 +338,19 @@
 Version 3.0.1
 • Solves a 'type' problem that occurs when input data (FITS) is 64 bit float.
 Version 3.0.0
 • same as version 2.9.8 but the new scrollable area now scales with the size of the main
 window as it always did before.
 Version 2.9.8
 • changes the routine that looks for the latest version of PyMovie to one provided by Kia
-Getrost. His version contacts the PyPI repository via a json query and is the officially
+
+Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
 a special feature of pip (the loader that get programs from the PyPI repository) that
-
-was marked as 'unsupported'. That worked for many years until the pip programmers
+was marked as 'unsupported'. That worked for many years until the pip programmers
 removed the 'special feature' as was their right (and promise, I guess). This caused
 several users to always get a message that they were not running the most recent
 version of PyMovie, even though they were. Again: thanks to Kia Getrost for
 researching the problem and even supplying correct code (worked first time!) for me to
 use.
 •
 
@@ -387,20 +388,20 @@
 
 With this new change, if you open an avi file and then create a folder for it, that new
 folder will be populated with the last OCR profile you worked with by copying the
 relevant files from your home directory into the newly created folder directory. For
 most people, with a single VTI, this is a good default behavior: when a folder is
 created, OCR will be ready to go.
 
-◦
+◦
 
 If you have a need for more than one OCR profile, you can still use the save/load
 OCR profile mechanism, which remains untouched.
 
-Version 2.9.3
+Version 2.9.3
 • changed the handling of ‘sticky values’ (like folder paths) to force the update of the
 ‘sticky file’ whenever a new folder is opened (to solve the issue where ‘save dialogs’
 sometimes have a previous folder path rather than the current folder path and so
 tricking the unwary user into storing a file unintentionally into the wrong folder)
 Version 2.9.2
 • added forced install of version 4.1.2.30 of opencv-python to (hopefully) eliminate the qt
 plugin errors that occur on Mac installations.
@@ -428,19 +429,19 @@
 • fixed bug that was causing all QHY FITS files to erroneously report detection of one or
 more frames with a GPS status of PartialData
 Version 2.8.6
 • changed the meta-tag that is examined for the QHY174M GPS status from GPS_STAT
 to GPSSTAT
 Version 2.8.5
 • adds special detection for FITS files from QHY174M cameras that have a GPS status
-of PartialData. In this case the normal timestamp meta-data tag (DATE-OBS) is invalid,
+
+of PartialData. In this case the normal timestamp meta-data tag (DATE-OBS) is invalid,
 but there is a belief that a timestamp can be computed from two other meta-data tags
 that do get filled in: GPS_ST and GPS_SU. Such a timestamp will almost certainly
-
-contain errors, but the observer may be able to figure out a common offset to apply to
+contain errors, but the observer may be able to figure out a common offset to apply to
 make them correct, so we are outputting GPS_ST + (GPS_SU / 1,000,000) in this
 special case. This change will be completely transparent – it will not affect QHY frames
 that have a GPS Locked status.
 Version 2.8.4
 • fixed issue that caused the initial display of a help message that was too big for the
 panel to be scrolled to the bottom (obscuring the first few lines) rather than the top.
 Version 2.8.3
@@ -470,19 +471,19 @@
 • adds aperture name to thumbnailOne image
 • adds explanation of aperture color meanings to aperture edit table
 • improves help messages surrounding two-point tracking setup
 Version 2.7.9
 • changes the way the WCS procedure submits a request to nova.astrometry.net. Where
 previously, the submission to nova deliberately restricted the search to a 1 degree
 radius around the target star location, I now allow a full blind-search.
-Restricting the search to a small region was done to give nova.astrometry.net a much
+
+Restricting the search to a small region was done to give nova.astrometry.net a much
 more limited selection of catalogs to search in the interest of speed. In my latest test
 case, a restricted search took 0.43 seconds of computer time at nova, while a blind
-
-search took 4.5 seconds of computer time.
+search took 4.5 seconds of computer time.
 The problem with a restricted search however is that if an error is made such that the
 target star is actually not in the image submitted, the search will simply fail quietly (and
 use a lot of computer time at nova to reach this conclusion!) without giving the user any
 clue as to why no solution could be found.
 With this version, I do a blind-search and if a solution is returned, I check to see if the
 target star is within the image and alert the user if the target star is not visible in the
 image.
@@ -512,24 +513,20 @@
 • The algorithm introduced in version 2.6.8 fails to perform adequately when the pixel
 histogram is insufficiently contiguous with too many missing values. A new algorithm
 has been introduced which seems to perform well no matter what the pixel histogram
 shape may be.
 •
 
 Changed the default threshold for static aperture from 9999 to 99999 to better
-accommodate 12 and 16 bit videos.
 
+accommodate 12 and 16 bit videos.
 Version 2.7.0
-
-•
-
-A small change to the Robust Mean algorithm so that it can be used on “finder” images
+• A small change to the Robust Mean algorithm so that it can be used on “finder” images
 (which have floating point values) as well as single-frame images (which have only
 integer values).
-
 Version 2.6.9
 • Changed the 'help/info' for the Plot Robust Mean button to better explain the algorithm.
 Version 2.6.8
 • Changed the algorithm for calculating the average value of background pixels. This
 new algorithm replaced one that was excellent when background noise had a gaussian
 distribution, but had about a 1% error (too small by 1%) when the noise distribution
 was skewed. The histogram of a skewed distribution has a longer tail on one side than
@@ -555,19 +552,19 @@
 Version 2.6.5
 • This version allows AAV Version 2 files to be read and processed.
 Version 2.6.4
 • With this version, the case of a non-version 2 ADV file is treated more gracefully --- just
 printing a message in the text box rather than a session-ending exception.
 Version 2.6.2
 • Added requirement that top/bottom redact values be entered (in the “finder” tab panel)
-before hot-pixel suppression via median filter will take place. This is needed for the
+
+before hot-pixel suppression via median filter will take place. This is needed for the
 case where a timestamp overlay is present that requires OCR. The median filter
 process has to bypass the region where such timestamps are located, otherwise poor
-
-OCR will be a result.
+OCR will be a result.
 Version 2.6.1
 • Working with Hristo Pavlov, I have added support for reading Version 2 ADV files (Astro
 Digital Video files) to PyMovie.
 A side effect of our collaborative effort is that there is now a publicly available Python
 package on PyPI.org for reading .adv files (Version 2) --- the package is called Adv2
 and is available to any Python programmer by the usual pip install Adv2. The
 project and its documentation can be viewed at https://pypi.org/project/Adv2/
@@ -599,20 +596,21 @@
 and the timestamp calculated by PyMovie. Thanks to Hiroyuki Watanabe for pressing
 the issue.
 Version 2.5.7
 • In the “finder” image generation panel, we have removed the option to use the Fourier=
 transform-based image correlation computations as a stacking/image aligning
 mechanism. It was finicky, had no benefits over the simple to use and understand
 stacking using a single tracking star, and fails on images without dominant features.
-•
+
+•
 
 Also made the name of the aperture to be used for stacking case-insensitive. It must
 still start with the character string 'stack', but 'StAcK' will work just as well.
 
-Version 2.5.6
+Version 2.5.6
 • In version 2.5.4 we switched to using a filename dialog that provided a list of alreadyused .csv file names, a useful convenience on occassion. Unfortunately, another
 characteristic of that file dialog is that it allowed the user to specify a filename that did
 not have a .csv extension. This version adds code to append a .csv extension to any
 filename the user provides that does not already have such an extension.
 Version 2.5.5
 • Squashed bug that kept avi files recorded with a dvsd codec from being read.
 Version 2.5.4
@@ -644,27 +642,28 @@
 
 Version 2.5.3
 • Fixed: during preparation of image for submission to nova.astrometry.net, I was forcing
 conversion of the image to uint16 for display purposes --- normally this would be ok,
 but FITS files can be float64 (signed) and cannot always be converted to uint16. I
 doubt any users will have noticed this, but one of my test data sets is a video of the
 Pluto occultation that was greatly 'massaged' and as a result came to me as a signed
-float64 file.
+
+float64 file.
 •
 
 Fixed: memory leak associated with plots --- some users (and me during testing) found
-
-that pymovie memory usage increased with time, eventually crashing --- I have traced
+that pymovie memory usage increased with time, eventually crashing --- I have traced
 that behavior down to the plot lightcurves function and eliminated the problem. A side
 effect of the 'fix' is that plots from a previous will no longer persist but rather will be
 automatically deleted, closed, and replaced by new plots. For some users, this may
 affect your workflow if you were in the habit of running an analysis, plotting the results,
 and running a changed analysis expecting to be able to generate another set of plots
 without losing the first set. If this was your practice, now you will be required to
 explicitly save plots that you want to use for comparison studies.
+
 Version 2.5.1
 • Fixed: SER file folder selection was not enabling ‘save aperture group’ button.
 • Fixed: Initial ‘save’ of aperture group was not enabling ‘restore aperture group’ button
 • Changed: default aperture name from app00 to ap00
 Version 2.5.0
 • Removed asinh scaling and normalization to 0...255 range in “finder” images. This will
 preserve star intensities and (hopefully) make “finder” images look more like the star
@@ -689,18 +688,18 @@
 • Changed the extraction of timestamps in SER files to use my SharpCap timestamp
 extraction routine. Previously, in a SER.py module that was available on the Internet
 and used by me for reading SER files, timestamp conversion involved first converting
 to Julian date and then to an ISO timestamp. For some reason, the Julian date version
 was always exactly one day earlier than the value from my SharpCap routine. Since
 the SharpCap interpretation matches what is shown visually, I’m electing to use that
 method of timestamp calculation.
-Version 2.4.4
-• Solves a problem extracting SharpCap embedded timestamps on some Win10
 
-systems, which can have a default 32 bit integer rather than the 64 bit integer on Mac
+Version 2.4.4
+• Solves a problem extracting SharpCap embedded timestamps on some Win10
+systems, which can have a default 32 bit integer rather than the 64 bit integer on Mac
 computers.
 Version 2.4.3
 • Solves another problem reading large SER files --- again unique to Win10
 environment.
 Version 2.4.2
 • Solves problem reading large SER files that was unique to Win10 --- reading large
 SER files on Mac was no problem.
@@ -734,20 +733,24 @@
 aperture. And (of course) the settings will be sticky between sessions.
 
 Version 2.3.4
 • Implemented the Preferences tab. An aperture size and a threshold sigma level (1, 2,
 or 3) can be specified. They will be ‘saved’ when PyMovie is closed and applied when
 next PyMovie is started up.
 Version 2.3.3
-• Major rearranging of GUI elements to reduce clutter. Uses Tabs.
+
+•
+
+Major rearranging of GUI elements to reduce clutter. Uses Tabs.
+
 •
 
 Note: the tabs can be dragged to rearrange (but won’t be sticky --- I may do that when I
+implement ‘preferences’)
 
-implement ‘preferences’)
 •
 
 Changed to use of 2 sigma(std) in automatic setting of threshold in snap-to-blob
 apertures.
 
 Version 2.3.1
 • Added test for astrometry.net failing to accept upload of image --- a failed upload
@@ -787,18 +790,18 @@
 can be tracked by a snap-to-blob aperture to provide the needed frame shift
 information.
 To activate this type of stacking, place a snap-to-blob aperture with a name that starts
 with stack That’s the only change needed. This is the easiest and most reliable stack
 alignment algorithm and will follow windshake (which 2 point tracking does not).
 The priority of frame stacking algorithms is:
 1. ‘stack’ aperture
-2. 2 point tracking path
-3. Fourier Correlation
 
-Version 2.2.7
+2. 2 point tracking path
+3. Fourier Correlation
+Version 2.2.7
 • Adds the ability to save multiple sets of apertures (and any associated tracking path).
 When the Save aperture group button is clicked, a dialog will appear requesting that a
 ‘tag’ be supplied to give the 2 or 3 files that are used to record a saved aperture group
 a unique name. The tag is appended to a root name and when the Restore aperture
 group button is clicked, a list of available aperture groups will be presented for
 selection.
 Version 2.2.6
@@ -829,22 +832,23 @@
 defined (they now show up a streaks on the finder image, so you may still want to
 create a hot pixel list).
 Version 2.2.5
 • When a new aperture is added, the new default state is that jogging with the arrow
 keys is enabled. At the same time, jogging is disabled on all apertures. This change
 was made to make the process of positioning apertures on hot-pixels easier.
 It is still possible to individually enable/disable jogging on more than one aperture. The
-only change is when an aperture is first created.
+
+only change is when an aperture is first created.
 •
 
 Added hot-pixel removal from finder images. This is a user guided process --- the user
-
-must place small apertures on hot-pixel groups, set a threshold for identifying hotpixels, and clicking on a button that invokes a program looks through all of the
+must place small apertures on hot-pixel groups, set a threshold for identifying hotpixels, and clicking on a button that invokes a program looks through all of the
 apertures, prepares a list of the coordinates of all hot-pixels, and substitutes the
 average background for all hot-pixels.
+
 Version 2.2.4
 • On lightcurve plots: the composite light curve is back on top. I didn’t like it on the
 bottom so it is back to the top where it will stay. I did ensure that the order of adding
 curves to the composite lightcurve plot is based on the column order. In this way, if the
 target lightcurve is the first column in the csv plot, it will be the last added to the
 composite plot so its ‘dots’ will be on top.
 Version 2.2.3
@@ -875,28 +879,25 @@
 In addition, now when ‘Restore aperture group’ is clicked, any apertures saved by a
 ‘Mark’ will be erased before the saved aperture group is loaded. This is a cleaner ‘start
 over’ and, without this change, if you click Restore aperture group, then Mark, then
 Restore aperture group again you got a duplicate set of apertures.
 
 Version 2.2.0
 • Made the ‘help’ text come up whenever the lunar box is checked. It serves as a
-warning.
-Version 2.1.9
-
-•
 
-Added a ‘lunar’ checkbox which should ONLY be used when an aperture is placed on a
+warning.
+Version 2.1.9
+• Added a ‘lunar’ checkbox which should ONLY be used when an aperture is placed on a
 sunlit lunar limb for a lunar occultation.
 This is experimental: until this point, PyMovie has focussed on asteroid occultations
 only --- this is a deviation from that focus.
 When this box is checked, it signals the Robust Mean extraction routine to statistically
 separate sky pixels from lunar limb and star pixels for use in background calculations.
 This emulates what Limovie does when a properly oriented ‘Avoid Sunlit Face’ aperture
 is utilized and so should produce comparable lightcurves. Time will tell.
-
 Version 2.1.8
 • I now save tracking path data when an aperture group is saved.
 Version 2.1.7
 • Added the ability to set a ‘tracking path’ by specifying two points, one early in the video
 and one late in the video. This feature is primarily useful in processing difficult driftthrough videos where no other good options for tracking are present.
 To learn a bit more, right-click on a non-yellow aperture and then click one of the menu
 items involving ‘track path’. That will cause a help panel to appear.
@@ -916,18 +917,18 @@
 • To simply setting up an OCR profile: added ability to retrain/resample any digit(s) after
 all digits have been initially sampled/trained. When there are missing sample digits,
 the menu of characters to record will show those that remain to be sampled, as it was
 before this version --- that feature speeds up the initial sampling of the digits. The
 change made in this version is that, if all digits have been sampled, a complete menu
 of digits to record will be produced when a digit is right-clicked so that any poorly
 sampled digit can be re-recorded without the need to start over from scratch.
-version 2.1.2
-• Added ability to correct pixel response curve for non-unity gamma setting of camera
 
-version 2.1.1
+version 2.1.2
+• Added ability to correct pixel response curve for non-unity gamma setting of camera
+version 2.1.1
 • Modified the robust mean estimator to deal with videos that have ‘clipped’
 backgrounds, a situation that is surprisingly common.
 
 Here is a ‘normal’ RobustMean plot:
 It shows the usual gaussian background noise in a 51x51 pixel aperture with some stars in
 the aperture as well.
 But sometimes we see that somewhere in the processing chain (could be a camera setting --could be in the recording software) that some sort of 'clipping' has occurred. It exhibits as a
```

### Comparing `pymovie-3.8.0/src/pymovie/SER.py` & `pymovie-3.8.1/src/pymovie/SER.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/alias_lnk_resolver.py` & `pymovie-3.8.1/src/pymovie/alias_lnk_resolver.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/aperture.py` & `pymovie-3.8.1/src/pymovie/aperture.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/apertureEdit.py` & `pymovie-3.8.1/src/pymovie/apertureEdit.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/apertureEditDialog.py` & `pymovie-3.8.1/src/pymovie/apertureEditDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/apertureNameDialog.py` & `pymovie-3.8.1/src/pymovie/apertureNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/aperturesFileTagDialog.py` & `pymovie-3.8.1/src/pymovie/aperturesFileTagDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/astrometry_client.py` & `pymovie-3.8.1/src/pymovie/astrometry_client.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/checkForNewerVersion.py` & `pymovie-3.8.1/src/pymovie/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/gammaUtils.py` & `pymovie-3.8.1/src/pymovie/gammaUtils.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/gui.py` & `pymovie-3.8.1/src/pymovie/gui.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/helpDialog.py` & `pymovie-3.8.1/src/pymovie/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/hotPixelDialog.py` & `pymovie-3.8.1/src/pymovie/hotPixelDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/main.py` & `pymovie-3.8.1/src/pymovie/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,14 +938,17 @@
 
         self.plot_symbol_size = 1
 
         self.fits_folder_in_use = False
         self.avi_wcs_folder_in_use = False
         self.folder_dir = None
 
+        self.aperturesDir = None
+        self.finderFramesDir = None
+
         self.timer = QTimer(self)
         self.timer.timeout.connect(self.setDoTestFlag)  # noqa
         self.do_test = False
 
         # self.filename is set to the full path of the selected image file (or folder) once
         # the user has made a valid selection
         self.filename = None
@@ -2579,17 +2582,20 @@
         self.gammaSettingOfCamera.setValue(1.00)
         self.currentGamma = 1.00
 
     def deleteOcrFiles(self):
         self.deleteModelDigits()
         self.deleteOcrBoxes()
 
-        f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        # TODO Check that this works
+        # f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        f_path = os.path.join(self.ocrDigitsDir, 'formatter.txt')
         if os.path.exists(f_path):
             os.remove(f_path)
+            # os.removedirs(self.ocrDigitsDir)
 
         f_path = os.path.join(self.homeDir, 'formatter.txt')
         if os.path.exists(f_path):
             os.remove(f_path)
 
         self.timestampReadingEnabled = False
         self.vtiSelectComboBox.setEnabled(True)
@@ -2727,34 +2733,34 @@
         # Because an average background was not supplied as an argument in the following call,
         # it will automatically extract one from the center of the current image
         # self.applyHotPixelErasure()
 
     def restoreApertureGroup(self):
 
         # Check the form of saved aperture filenames to see if we need to deal with legacy filenames
-        saved_aperture_groups = glob.glob(self.folder_dir + '/savedApertures*.p')
+        saved_aperture_groups = glob.glob(self.aperturesDir + '/savedApertures*.p')
 
         if not saved_aperture_groups:
 
             # We have no new format aperture groups, so process as old
-            frameFn = self.folder_dir + '/markedFrameNumber.p'
+            frameFn = self.aperturesDir + '/markedFrameNumber.p'
             if os.path.exists(frameFn):
                 savedFrameNumber = pickle.load(open(frameFn, 'rb'))
                 self.showMsg(f'Saved frame number is: {savedFrameNumber}')
                 self.currentFrameSpinBox.setValue(savedFrameNumber)
             else:
                 return
 
             # Erase state saved by a 'Mark'
             self.savedStateApertures = []
             self.transportReturnToMark.setEnabled(False)
 
             self.clearApertures()
 
-            tpathFilename = self.folder_dir + '/trackingPath.p'
+            tpathFilename = self.aperturesDir + '/trackingPath.p'
             if os.path.exists(tpathFilename):
                 tpath_tuple = pickle.load(open(tpathFilename, 'rb'))
 
                 self.tpathEarlyX = tpath_tuple[0]
                 self.tpathEarlyY = tpath_tuple[1]
                 self.tpathEarlyFrame = tpath_tuple[2]
                 self.tpathLateX = tpath_tuple[3]
@@ -2770,30 +2776,30 @@
             # Force frame view
             self.viewFieldsCheckBox.setChecked(False)
 
             # Remove all apertures that have been already placed (particularly the target
             # aperture that is automatically placed when a WCS solution was present)
             self.clearApertures()
 
-            aperturesFn = self.folder_dir + '/markedApertures.p'
+            aperturesFn = self.aperturesDir + '/markedApertures.p'
             if os.path.exists(aperturesFn):
                 savedApertureDicts = pickle.load(open(aperturesFn, "rb"))
                 self.showMsg(f'Num saved apertures: {len(savedApertureDicts)}')
             else:
                 self.showMsg(f'Failed to find markedApertures.p file.')
                 return
         else:
             # Show file select dialog for selection of appropriate saved aperture group
             options = QFileDialog.Options()
             options |= QFileDialog.DontUseNativeDialog
 
             filename, _ = QFileDialog.getOpenFileName(
                 self,  # parent
                 "Select aperture group",  # title for dialog
-                self.folder_dir,  # starting directory
+                self.aperturesDir,  # starting directory
                 "saved aperture groups (savedApertures*.p)",
                 options=options
             )
 
             QtGui.QGuiApplication.processEvents()
 
             if not filename:
@@ -2814,21 +2820,21 @@
 
             if app_group_id == 'savedApertures':
                 app_group_id = '<none found>'
 
             self.showMsg(f'file selected: {basefn}  aperture group id: {app_group_id}')
 
             if app_group_id == '<none found>':
-                frameFn = self.folder_dir + '/savedFrameNumber.p'
-                tpathFilename = self.folder_dir + '/trackingPath.p'
-                aperturesFn = self.folder_dir + '/savedApertures.p'
-            else:
-                frameFn = self.folder_dir + f'/savedFrameNumber-{app_group_id}.p'
-                tpathFilename = self.folder_dir + f'/trackingPath-{app_group_id}.p'
-                aperturesFn = self.folder_dir + f'/savedApertures-{app_group_id}.p'
+                frameFn = self.aperturesDir + '/savedFrameNumber.p'
+                tpathFilename = self.aperturesDir + '/trackingPath.p'
+                aperturesFn = self.aperturesDir + '/savedApertures.p'
+            else:
+                frameFn = self.aperturesDir + f'/savedFrameNumber-{app_group_id}.p'
+                tpathFilename = self.aperturesDir + f'/trackingPath-{app_group_id}.p'
+                aperturesFn = self.aperturesDir + f'/savedApertures-{app_group_id}.p'
 
             if not os.path.exists(frameFn):
                 self.showMsg(f'Failed to find {frameFn} file.')
                 return
 
             if not os.path.exists(aperturesFn):
                 self.showMsg(f'Failed to find {aperturesFn} file.')
@@ -2952,15 +2958,15 @@
         if not self.savedStateApertures:
             self.showMsg(f'There are no apertures to save.')
             return
 
         # Get list of already used aperture group tags
         # Do a grep/glob lookup on self.folder_dir + f'/savedApertures-*.p' and then
         # parse out the tag aided by the guarantee that there be only one - and one . in the file name.
-        tags_in_use_files = glob.glob(self.folder_dir + f'/savedApertures-*.p')
+        tags_in_use_files = glob.glob(self.aperturesDir + f'/savedApertures-*.p')
         tags_in_use = []
         for fn in tags_in_use_files:
             p = pathlib.PurePath(fn)
             parts = p.parts
             file_name = parts[-1]
             tag_with_ext = file_name.split('-')[-1]
             tag = tag_with_ext.split('.')[0]
@@ -2995,38 +3001,38 @@
                                   f'version 3.7.4.\n\n'
                                   f'You will need to redefine them so that the new fields are added.\n\n'
                                   f'You will not be able to save the apertures currently showing.')
                 return
             savedApertureDicts.append(my_dict)
 
         # Pickle the saved aperture dictionaries for use during opening of file/folder
-        pickle.dump(savedApertureDicts, open(self.folder_dir + f'/savedApertures-{tag}.p', "wb"))
+        pickle.dump(savedApertureDicts, open(self.aperturesDir + f'/savedApertures-{tag}.p', "wb"))
 
         self.savedStateFrameNumber = self.currentFrameSpinBox.value()
-        pickle.dump(self.savedStateFrameNumber, open(self.folder_dir + f'/savedFrameNumber-{tag}.p', "wb"))
+        pickle.dump(self.savedStateFrameNumber, open(self.aperturesDir + f'/savedFrameNumber-{tag}.p', "wb"))
 
         if self.tpathSpecified:
             tpath_tuple = (
                 self.tpathEarlyX,
                 self.tpathEarlyY,
                 self.tpathEarlyFrame,
                 self.tpathLateX,
                 self.tpathLateY,
                 self.tpathLateFrame,
                 self.tpathXa,
                 self.tpathXb,
                 self.tpathYa,
                 self.tpathYb
             )
-            pickle.dump(tpath_tuple, open(self.folder_dir + f'/trackingPath-{tag}.p', "wb"))
+            pickle.dump(tpath_tuple, open(self.aperturesDir + f'/trackingPath-{tag}.p', "wb"))
             self.showMsg(f'Current aperture group, frame number, and tracking path saved.')
         else:
             # noinspection PyBroadException
             try:
-                os.remove(self.folder_dir + f'/trackingPath-{tag}.p')
+                os.remove(self.aperturesDir + f'/trackingPath-{tag}.p')
             except Exception:
                 pass
             self.showMsg(f'Current aperture group and frame number saved.')
 
         self.restoreApertureState.setEnabled(True)
 
     def saveCurrentState(self):
@@ -3871,15 +3877,17 @@
                     self.topFieldFirstRadioButton.setChecked(True)
                 self.detectFieldTimeOrder = False
 
         return upper_timestamp, upper_time, upper_scores, upper_cum_score, \
             lower_timestamp, lower_time, lower_scores, lower_cum_score
 
     def writeFormatTypeFile(self, format_type):
-        f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        # TODO Check that this works
+        # f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        f_path = os.path.join(self.ocrDigitsDir, 'formatter.txt')
         with open(f_path, 'w') as f:
             f.writelines(f'{format_type}')
 
         # Write a duplicate to the home directory
         f_path = os.path.join(self.homeDir, 'formatter.txt')
         with open(f_path, 'w') as f:
             f.writelines(f'{format_type}')
@@ -4555,15 +4563,15 @@
         last_frame = first_frame + num_frames_to_stack - 1
         last_frame = min(last_frame, self.stopAtFrameSpinBox.maximum())
 
         enhanced_filename_with_frame_num = f'/enhanced-image-{first_frame}.fit'
 
         # Remove an enhanced image with a matching frame number
         try:
-            os.remove(self.folder_dir + enhanced_filename_with_frame_num)
+            os.remove(self.finderFramesDir + enhanced_filename_with_frame_num)
         except FileNotFoundError:
             pass
 
         if self.fits_folder_in_use:
             fitsReader = self.getFitsFrame
         else:
             fitsReader = None
@@ -4640,25 +4648,25 @@
             self.showMsg, self.stackerProgressBar, QtGui.QGuiApplication.processEvents,
             first_frame=first_frame, last_frame=last_frame,
             timestamp_trim_top=num_top,
             timestamp_trim_bottom=num_bottom,
             fitsReader=fitsReader,
             serReader=serReader,
             advReader=advReader,
-            avi_location=self.avi_location, out_dir_path=self.folder_dir, bkg_threshold=None,
+            avi_location=self.avi_location, out_dir_path=self.finderFramesDir, bkg_threshold=None,
             hot_pixel_erase=self.applyHotPixelErasureToImg,
             delta_x=dx_dframe,
             delta_y=dy_dframe,
             shift_dict=shift_dict
         )
 
         self.finderMethodEdit.setText('')
 
         # Now that we're back, if we got a new enhanced-image.fit, display it.
-        fullpath = self.folder_dir + enhanced_filename_with_frame_num
+        fullpath = self.finderFramesDir + enhanced_filename_with_frame_num
         if os.path.isfile(fullpath):
             self.clearApertureData()
             self.clearApertures()
             self.openFitsImageFile(fullpath)
             self.finderFrameBeingDisplayed = True
             self.restoreSavedState()
             if self.levels:
@@ -7617,14 +7625,23 @@
             self.showMsg(f'Opened FITS folder: {dir_path}', blankLine=False)
             self.settings.setValue('fitsdir', dir_path)  # Make dir 'sticky'"
             self.settings.sync()
 
             self.folder_dir = dir_path
             self.fits_filenames = sorted(glob.glob(dir_path + '/*.fits'))
 
+            self.aperturesDir = os.path.join(self.folder_dir, 'ApertureGroups')
+            if not os.path.exists(self.aperturesDir):
+                os.mkdir(self.aperturesDir)
+
+            # Initialize finder frames directory
+            self.finderFramesDir = os.path.join(self.folder_dir, 'FinderFrames')
+            if not os.path.exists(self.finderFramesDir):
+                os.mkdir(self.finderFramesDir)
+
             if os.path.exists(self.folder_dir + '/pixel-dimensions.p'):
                 self.readPixelDimensions()
             else:
                 self.pixelAspectRatio = 1.0
                 self.pixelWidthEdit.setText('1.00')
                 self.pixelHeightEdit.setText('1.00')
 
@@ -7660,21 +7677,41 @@
 
             self.processTargetAperturePlacementFiles()
 
             self.checkForSavedApertureGroups()
 
     def checkForSavedApertureGroups(self):
 
-        saved_aperture_groups = glob.glob(self.folder_dir + '/savedApertures*.p')
+        # Check for legacy file structure - aperture group info in self.folder_dir
+        old_saved_aperture_group_files = glob.glob(self.folder_dir + '/savedApertures*.p')
+        if old_saved_aperture_group_files:
+            for fpath in old_saved_aperture_group_files:
+                head, tail = os.path.split(fpath)
+                Path(fpath).rename(os.path.join(head, 'ApertureGroups', tail))
+
+        old_saved_aperture_frame_num_files = glob.glob(self.folder_dir + '/savedFrameNumber*.p')
+        if old_saved_aperture_frame_num_files:
+            for fpath in old_saved_aperture_frame_num_files:
+                head, tail = os.path.split(fpath)
+                Path(fpath).rename(os.path.join(head, 'ApertureGroups', tail))
+
+        old_saved_finder_frame_files = glob.glob(self.folder_dir + '/enhanced-image-*.fit')
+        if old_saved_finder_frame_files:
+            for fpath in old_saved_finder_frame_files:
+                head, tail = os.path.split(fpath)
+                Path(fpath).rename(os.path.join(head, 'FinderFrames', tail))
+
+
+        saved_aperture_groups = glob.glob(self.aperturesDir + '/savedApertures*.p')
 
         if saved_aperture_groups:
             self.restoreApertureState.setEnabled(True)
             return
 
-        saved_aperture_groups = glob.glob(self.folder_dir + '/markedApertures.p')
+        saved_aperture_groups = glob.glob(self.aperturesDir + '/markedApertures.p')
 
         if saved_aperture_groups:
             self.restoreApertureState.setEnabled(True)
             return
 
     @staticmethod
     def showMsgDialog(msg):
@@ -7712,15 +7749,15 @@
 
         options = QFileDialog.Options()
         # options |= QFileDialog.DontUseNativeDialog
 
         self.filename, _ = QFileDialog.getOpenFileName(
             self,  # parent
             "Select enhanced image",  # title for dialog
-            self.folder_dir,  # starting directory
+            self.finderFramesDir,  # starting directory
             "finder images (*.bmp enhanced*.fit);; all files (*.*)",
             options=options
         )
 
         QtGui.QGuiApplication.processEvents()
 
         if self.filename:
@@ -8079,22 +8116,26 @@
         elif self.formatterCode == 'SharpCap8':
             self.sharpCapTimestampPresent = True
         else:
             self.showMsg(f'Unknown timestamp formatter code: {self.formatterCode}.  Defaulting to Iota')
             self.timestampFormatter = format_iota_timestamp
 
     def readFormatTypeFile(self):
-        f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        # TODO Check that this works
+        # f_path = os.path.join(self.folder_dir, 'formatter.txt')
+        f_path = os.path.join(self.ocrDigitsDir, 'formatter.txt')
         if not os.path.exists(f_path):
             f_path = os.path.join(self.homeDir, 'formatter.txt')
             if not os.path.exists(f_path):
                 return None
         with open(f_path, 'r') as f:
             code = f.readline()
-            f_path = os.path.join(self.folder_dir, 'formatter.txt')
+            # TODO Check that this works
+            # f_path = os.path.join(self.folder_dir, 'formatter.txt')
+            f_path = os.path.join(self.ocrDigitsDir, 'formatter.txt')
             with open(f_path, 'w') as g:
                 g.write(code)
             return code
 
     def selectAviSerAdvAavFolder(self):
 
         self.lineNoiseFilterCheckBox.setChecked(False)
@@ -8346,16 +8387,29 @@
                         self.changeNavButtonTitles()
 
                     # This will get our image display initialized with default pan/zoom state
                     self.initialFrame = True
                     self.showFrame()
 
                     # Initialize ocr related directories
-                    self.ocrDigitsDir = self.folder_dir
-                    self.ocrBoxesDir = self.folder_dir
+                    self.ocrDigitsDir = os.path.join(self.folder_dir, 'OCR')
+                    if not os.path.exists(self.ocrDigitsDir):
+                        os.mkdir(self.ocrDigitsDir)
+
+                    # Initialize apertures directory
+                    self.aperturesDir = os.path.join(self.folder_dir, 'ApertureGroups')
+                    if not os.path.exists(self.aperturesDir):
+                        os.mkdir(self.aperturesDir)
+                    self.ocrBoxesDir = self.ocrDigitsDir
+
+                    # Initialize finder frames directory
+                    self.finderFramesDir = os.path.join(self.folder_dir, 'FinderFrames')
+                    if not os.path.exists(self.finderFramesDir):
+                        os.mkdir(self.finderFramesDir)
+
                     self.currentOcrBox = None
                     self.clearOcrBoxes()  # From any previous ocr setup
 
                     self.modelDigitsFilename = 'custom-digits.p'
                     self.ocrboxBasePath = 'custom-boxes'
 
                     self.processTargetAperturePlacementFiles()
```

### Comparing `pymovie-3.8.0/src/pymovie/ocr.py` & `pymovie-3.8.1/src/pymovie/ocr.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/ocrCharacterBox.py` & `pymovie-3.8.1/src/pymovie/ocrCharacterBox.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/ocrProfileNameDialog.py` & `pymovie-3.8.1/src/pymovie/ocrProfileNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/play-Temp.py` & `pymovie-3.8.1/src/pymovie/play-Temp.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/play-introspection.py` & `pymovie-3.8.1/src/pymovie/play-introspection.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/selectHotPixelProfile.py` & `pymovie-3.8.1/src/pymovie/selectHotPixelProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/selectProfile.py` & `pymovie-3.8.1/src/pymovie/selectProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/stacker.py` & `pymovie-3.8.1/src/pymovie/stacker.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/starPositionDialog.py` & `pymovie-3.8.1/src/pymovie/starPositionDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie/wcs_helper_functions.py` & `pymovie-3.8.1/src/pymovie/wcs_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.8.0/src/pymovie.egg-info/PKG-INFO` & `pymovie-3.8.1/src/pymovie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.8.0
+Version: 3.8.1
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.8.0/src/pymovie.egg-info/SOURCES.txt` & `pymovie-3.8.1/src/pymovie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

