# Comparing `tmp/slab-1.1.3.tar.gz` & `tmp/slab-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slab-1.1.3.tar", last modified: Thu Apr  6 09:58:08 2023, max compression
+gzip compressed data, was "slab-1.1.4.tar", last modified: Sun Jul 16 11:42:46 2023, max compression
```

## Comparing `slab-1.1.3.tar` & `slab-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:58:08.539773 slab-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-06 09:57:50.000000 slab-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-06 09:57:50.000000 slab-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-04-06 09:58:08.535773 slab-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-06 09:57:50.000000 slab-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 09:58:08.539773 slab-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-06 09:57:50.000000 slab-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:58:08.531772 slab-1.1.3/slab/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-06 09:57:50.000000 slab-1.1.3/slab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28795 2023-04-06 09:57:50.000000 slab-1.1.3/slab/binaural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:58:08.535773 slab-1.1.3/slab/data/
--rw-r--r--   0 runner    (1001) docker     (123)   670746 2023-04-06 09:57:50.000000 slab-1.1.3/slab/data/mit_kemar_normal_pinna.bz2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:58:08.535773 slab-1.1.3/slab/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 09:57:50.000000 slab-1.1.3/slab/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-04-06 09:57:50.000000 slab-1.1.3/slab/experiments/motion_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-06 09:57:50.000000 slab-1.1.3/slab/experiments/room_voice_interference.py
--rw-r--r--   0 runner    (1001) docker     (123)    29833 2023-04-06 09:57:50.000000 slab-1.1.3/slab/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51148 2023-04-06 09:57:50.000000 slab-1.1.3/slab/hrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)    58181 2023-04-06 09:57:50.000000 slab-1.1.3/slab/psychoacoustics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-04-06 09:57:50.000000 slab-1.1.3/slab/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)    72711 2023-04-06 09:57:50.000000 slab-1.1.3/slab/sound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:58:08.535773 slab-1.1.3/slab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 09:58:08.000000 slab-1.1.3/slab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-16 11:42:36.000000 slab-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-16 11:42:36.000000 slab-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 11:42:46.724534 slab-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-16 11:42:36.000000 slab-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:42:46.724534 slab-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-16 11:42:36.000000 slab-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-16 11:42:36.000000 slab-1.1.4/slab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28795 2023-07-16 11:42:36.000000 slab-1.1.4/slab/binaural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   670746 2023-07-16 11:42:36.000000 slab-1.1.4/slab/data/mit_kemar_normal_pinna.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/motion_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-16 11:42:36.000000 slab-1.1.4/slab/experiments/room_voice_interference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29833 2023-07-16 11:42:36.000000 slab-1.1.4/slab/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51148 2023-07-16 11:42:36.000000 slab-1.1.4/slab/hrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58405 2023-07-16 11:42:36.000000 slab-1.1.4/slab/psychoacoustics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-07-16 11:42:36.000000 slab-1.1.4/slab/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72821 2023-07-16 11:42:36.000000 slab-1.1.4/slab/sound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:42:46.724534 slab-1.1.4/slab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 11:42:46.000000 slab-1.1.4/slab.egg-info/top_level.txt
```

### Comparing `slab-1.1.3/LICENSE` & `slab-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/PKG-INFO` & `slab-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slab
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tools for generating and manipulating digital signals, particularly sounds.
 Home-page: http://github.com/DrMarc/slab.git
 Author: Marc Schoenwiesner
 Author-email: marc.schoenwiesner@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Provides-Extra: docs
 Provides-Extra: hrtf
 License-File: LICENSE
 
 ![Package](https://github.com/DrMarc/slab/workflows/Python%20package/badge.svg)
 [![PyPI](https://github.com/DrMarc/slab/workflows/PyPi/badge.svg)](https://pypi.org/project/slab/)
 [![Documentation Status](https://readthedocs.org/projects/slab/badge/?version=latest)](https://slab.readthedocs.io/en/latest/?badge=latest)
+[![Tutorial](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg)](https://github.com/DrMarc/slab/graphs/commit-activity)
 ![PyPI pyversions](https://img.shields.io/badge/python-%3E%3D3.6-blue)
 ![PyPI license](https://img.shields.io/badge/license-MIT-brightgreen)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03284/status.svg)](https://doi.org/10.21105/joss.03284)
 
 **slab**: easy manipulation of sounds and psychoacoustic experiments in Python
 ======================
@@ -191,14 +192,16 @@
 The releases use [semantic versioning](https://semver.org): major.minor.patch, where `major` increments for changes that break backwards compatibility, `minor` increments for added functionality, and `patch` increments for internal bug fixes.
 ```slab.__version__``` prints the installed version.
 
 Documentation
 -------------
 
 Read the tutorial-style documentation on [ReadTheDocs](https://slab.readthedocs.io/).
+For an interactive tutorial without installing anything, try the Colab notebook:
+[![Open tutorial in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 
 Citing slab
 -----------
 
 Schönwiesner et al., (2021). s(ound)lab: An easy to learn Python package for designing and running psychoacoustic experiments. Journal of Open Source Software, 6(62), 3284, https://doi.org/10.21105/joss.03284
 
 ```
```

### Comparing `slab-1.1.3/README.md` & `slab-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![Package](https://github.com/DrMarc/slab/workflows/Python%20package/badge.svg)
 [![PyPI](https://github.com/DrMarc/slab/workflows/PyPi/badge.svg)](https://pypi.org/project/slab/)
 [![Documentation Status](https://readthedocs.org/projects/slab/badge/?version=latest)](https://slab.readthedocs.io/en/latest/?badge=latest)
+[![Tutorial](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg)](https://github.com/DrMarc/slab/graphs/commit-activity)
 ![PyPI pyversions](https://img.shields.io/badge/python-%3E%3D3.6-blue)
 ![PyPI license](https://img.shields.io/badge/license-MIT-brightgreen)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03284/status.svg)](https://doi.org/10.21105/joss.03284)
 
 **slab**: easy manipulation of sounds and psychoacoustic experiments in Python
 ======================
@@ -176,14 +177,16 @@
 The releases use [semantic versioning](https://semver.org): major.minor.patch, where `major` increments for changes that break backwards compatibility, `minor` increments for added functionality, and `patch` increments for internal bug fixes.
 ```slab.__version__``` prints the installed version.
 
 Documentation
 -------------
 
 Read the tutorial-style documentation on [ReadTheDocs](https://slab.readthedocs.io/).
+For an interactive tutorial without installing anything, try the Colab notebook:
+[![Open tutorial in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 
 Citing slab
 -----------
 
 Schönwiesner et al., (2021). s(ound)lab: An easy to learn Python package for designing and running psychoacoustic experiments. Journal of Open Source Software, 6(62), 3284, https://doi.org/10.21105/joss.03284
 
 ```
```

### Comparing `slab-1.1.3/setup.py` & `slab-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/binaural.py` & `slab-1.1.4/slab/binaural.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/data/mit_kemar_normal_pinna.bz2` & `slab-1.1.4/slab/data/mit_kemar_normal_pinna.bz2`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/experiments/motion_speed.py` & `slab-1.1.4/slab/experiments/motion_speed.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/experiments/room_voice_interference.py` & `slab-1.1.4/slab/experiments/room_voice_interference.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/filter.py` & `slab-1.1.4/slab/filter.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/hrtf.py` & `slab-1.1.4/slab/hrtf.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/psychoacoustics.py` & `slab-1.1.4/slab/psychoacoustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 try:
     import matplotlib.pyplot as plt
 except ImportError:
     plt = None
 import slab
 
 results_folder = 'Results'
-input_method = 'keyboard'  #: sets the input for the Key context manager to 'keyboard 'or 'buttonbox'
+input_method = 'keyboard'  #: sets the input for the Key context manager to 'keyboard', 'buttonbox', or 'prompt'
 
 
 class _Buttonbox:
     """
-    Adapter class to allow easy switching between input from the keyboard via curses and from the custom buttonbox
-    adapter (custom arduino device that sends a keystroke followed by a return keystroke when pressing a button on
-    the arduino).
+    Adapter class to allow easy switching between input from the keyboard via curses (no ENTER keypress needed after
+    single button press) to the Python input prompt, which can be used with an external button box (custom arduino device
+    that sends keystrokes) or when running from a Jupiter or Colab notebook.
     """
     @staticmethod
     def getch():
-        input_key = input()  # buttonbox adapter has to return the keycode of intended keys!
+        input_key = input()  # buttonbox has to return the key followed by ENTER!
         if input_key:
-            return int(input_key)
-
+            return ord(input_key)
 
 class _FigChar:
     """
     Adapter class to allow easy switching to input via the current_character attribute of stairs figure.
     Set slab.psychoacoustics.input_method = 'figure' to use. A figure with the name 'stairs' will be opened if it is not
     already present. If used together with the plot method of the Staircase class, input is acquired through the stairs
     plot. Depending on the operating system, you may have to click once into the figure to give it focus.
@@ -63,17 +62,18 @@
         return ord(fig_key)
 
 
 @contextmanager
 def key(mesg=None):
     """
     Wrapper for curses module to simplify getting a single keypress from the terminal (default), a buttonbox, or a
-    figure. Set slab.psychoacoustics.input_method = 'buttonbox' to use a custom USB buttonbox or to 'figure' to open
-    a figure called 'stairs' (if not already opened by the `slab.Staricase.plot` method). Optianally takes a string
-    argument which is printed in the terminal for conveying instructions to the participant.
+    figure. Set slab.psychoacoustics.input_method = 'buttonbox' to use a custom USB buttonbox, to 'figure' to open
+    a figure called 'stairs' (if not already opened by the `slab.Staricase.plot` method), or to 'prompt' for a
+    simple Python prompt (requires pressing Enter/Return after the response). Optionally takes a string argument
+    which is printed in the terminal for conveying instructions to the participant.
 
     Example::
 
         with slab.key('Waiting for buttons 1 (yes) or 2 (no).') as key:
         response = key.getch()
     """
 
@@ -89,15 +89,15 @@
         stdscr.refresh()
         if mesg is not None:
             stdscr.addstr(str(mesg))
         yield stdscr
         curses.nocbreak()
         curses.echo()
         curses.endwin()
-    elif input_method == 'buttonbox':
+    elif input_method == 'buttonbox' or input_method == 'prompt':
         if mesg is not None:
             print(mesg)
         yield _Buttonbox
     elif input_method == 'figure':
         if mesg is not None:
             print(mesg)
         yield _FigChar
@@ -422,26 +422,27 @@
             raise StopIteration
         if self.trials[self.this_n] == 0:
             self.this_trial = 0
         else:
             self.this_trial = self.conditions[self.trials[self.this_n]-1]  # fetch the trial info
         return self.this_trial
 
-    def add_response(self, response):
+    def add_response(self, *response):
         """
-        Append response to the list in the `data` attribute belonging to the current trial (see Trialsequence doc).
+        Append response(s) to the list in the `data` attribute belonging to the current trial (see Trialsequence doc).
 
         Attributes:
              response (any): data to append to the list. Can be anything but save_json method won't be available if
                 the content of `response` is not JSON serializable (if it's an object for example).
         """
         if self.this_n < 0:
             print("Can't add response because trial hasn't started yet!")
         else:
-            self.data[self.this_n].append(response)
+            for r in response:
+                self.data[self.this_n].append(r)
 
     def print_trial_info(self):
         """ Convenience method for printing current trial information. """
         print(f'{self.label} | trial # {self.this_n} of {"inf" if self.kind=="infinite" else self.n_trials} '
               f'({"inf" if self.kind=="infinite" else self.n_remaining} remaining): condition {self.this_trial}, '
               f'last response: {self.data[self.this_n-1]}')
```

### Comparing `slab-1.1.3/slab/signal.py` & `slab-1.1.4/slab/signal.py`

 * *Files identical despite different names*

### Comparing `slab-1.1.3/slab/sound.py` & `slab-1.1.4/slab/sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 _system = platform.system()
 if _system == 'Windows':
     import winsound
 
 import slab.signal
 from slab.signal import Signal
 from slab.filter import Filter
+from slab import _in_notebook
+
+if _in_notebook:
+    from IPython.display import Audio, display
 
 _tmpdir = pathlib.Path(tempfile.gettempdir())  # get a temporary directory for writing intermediate files
 _calibration_intensity = 0  # difference between rms intensity and measured output intensity in dB
 _default_level = 70  # the default level for generated Sounds in dB
 _in_notebook = False # are we in a Jupiter notebook (then use IPython object to play audio)
 
 def set_default_level(level):
@@ -937,16 +941,16 @@
     def play(self):
         """
         Plays the sound through the default device. If the soundcard module is installed it is used
         to play the sound. Otherwise the sound is saved as .wav to a temporary directory and is played via the
         `play_file` method.
         """
         if _in_notebook:
-            from IPython.display import Audio, display
             display(Audio(self.data.T, rate=self.samplerate, autoplay=True))
+            time.sleep(self.duration)  # playing in Jupiter/Colab notebook is non_blocking, thus busy-wait for stim duration
         elif soundcard is not False:
             soundcard.default_speaker().play(self.data, samplerate=self.samplerate)
         else:
             filename = hashlib.sha256(self.data).hexdigest() + '.wav'  # make unique name
             filename = _tmpdir / filename
             if not filename.is_file():
                 self.write(filename, normalise=False)
@@ -959,15 +963,14 @@
 
         Arguments:
              filename (str | pathlib.Path): full path to the .wav file to be played.
         """
         if isinstance(filename, pathlib.Path):
             filename = str(filename)
         if _in_notebook:
-            from IPython.display import Audio, display
             display(Audio(filename, autoplay=True))
         elif _system == 'Windows':
             winsound.PlaySound(filename, winsound.SND_FILENAME)
         elif _system == 'Darwin':  # MacOS
             subprocess.call(['afplay', filename], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
         else:  # Linux
             try:
```

### Comparing `slab-1.1.3/slab.egg-info/PKG-INFO` & `slab-1.1.4/slab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slab
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tools for generating and manipulating digital signals, particularly sounds.
 Home-page: http://github.com/DrMarc/slab.git
 Author: Marc Schoenwiesner
 Author-email: marc.schoenwiesner@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Provides-Extra: docs
 Provides-Extra: hrtf
 License-File: LICENSE
 
 ![Package](https://github.com/DrMarc/slab/workflows/Python%20package/badge.svg)
 [![PyPI](https://github.com/DrMarc/slab/workflows/PyPi/badge.svg)](https://pypi.org/project/slab/)
 [![Documentation Status](https://readthedocs.org/projects/slab/badge/?version=latest)](https://slab.readthedocs.io/en/latest/?badge=latest)
+[![Tutorial](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg)](https://github.com/DrMarc/slab/graphs/commit-activity)
 ![PyPI pyversions](https://img.shields.io/badge/python-%3E%3D3.6-blue)
 ![PyPI license](https://img.shields.io/badge/license-MIT-brightgreen)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03284/status.svg)](https://doi.org/10.21105/joss.03284)
 
 **slab**: easy manipulation of sounds and psychoacoustic experiments in Python
 ======================
@@ -191,14 +192,16 @@
 The releases use [semantic versioning](https://semver.org): major.minor.patch, where `major` increments for changes that break backwards compatibility, `minor` increments for added functionality, and `patch` increments for internal bug fixes.
 ```slab.__version__``` prints the installed version.
 
 Documentation
 -------------
 
 Read the tutorial-style documentation on [ReadTheDocs](https://slab.readthedocs.io/).
+For an interactive tutorial without installing anything, try the Colab notebook:
+[![Open tutorial in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/DrMarc/slab/blob/master/slab_tutorial.ipynb)
 
 Citing slab
 -----------
 
 Schönwiesner et al., (2021). s(ound)lab: An easy to learn Python package for designing and running psychoacoustic experiments. Journal of Open Source Software, 6(62), 3284, https://doi.org/10.21105/joss.03284
 
 ```
```

