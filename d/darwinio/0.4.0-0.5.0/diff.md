# Comparing `tmp/darwinio-0.4.0.tar.gz` & `tmp/darwinio-0.5.0.tar.gz`

## Comparing `darwinio-0.4.0.tar` & `darwinio-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.4.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.4.0/keke
--rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.4.0/keke2
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.4.0/requirements.txt
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.4.0/todo.org
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/characteristics.ods
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/doc.md
--rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/doc.pdf
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.4.0/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    15229 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    20840 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.4.0/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.4.0/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.4.0/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.4.0/README.md
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 darwinio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.5.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.5.0/keke
+-rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.5.0/keke2
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.5.0/requirements.txt
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.5.0/todo.org
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.5.0/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    15229 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    21588 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1787 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/stats.py
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/test.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.5.0/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.5.0/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.5.0/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.5.0/README.md
+-rwxr-xr-x   0        0        0      867 2020-02-02 00:00:00.000000 darwinio-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 darwinio-0.5.0/PKG-INFO
```

### Comparing `darwinio-0.4.0/CONTRIBUTING.md` & `darwinio-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/keke` & `darwinio-0.5.0/keke`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/keke2` & `darwinio-0.5.0/keke2`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/todo.org` & `darwinio-0.5.0/todo.org`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/characteristics.ods` & `darwinio-0.5.0/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/doc.md` & `darwinio-0.5.0/documentation/doc.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/doc.pdf` & `darwinio-0.5.0/documentation/doc.pdf`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/earlystages.md` & `darwinio-0.5.0/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/implementation.md` & `darwinio-0.5.0/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/graphical_interface/empty_window.png` & `darwinio-0.5.0/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/graphical_interface/main_game.png` & `darwinio-0.5.0/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/graphical_interface/starting_window.png` & `darwinio-0.5.0/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/screenshot/main_game_play.png` & `darwinio-0.5.0/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/documentation/screenshot/titlescreen.png` & `darwinio-0.5.0/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/__main__.py` & `darwinio-0.5.0/src/darwinio/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 import pygame as pg
 import darwinio.graphical_sim as gsim
 import darwinio.constants as constants
+import darwinio.stats as statistics
 from importlib.metadata import version
 
 
 def main(resolution: tuple[int, int], fps: int, world_size: tuple[int, int]):
     """
     The main function that runs the game.
 
@@ -47,28 +48,31 @@
     music_playing = True
     with gsim.get_asset_path("audio", "Darwinio.mp3") as path:
         pg.mixer.music.load(path)
     pg.mixer.music.set_volume(1)
     pg.mixer.music.play()
 
     world = gsim.World(world_size, initial_temp_avg=45)
+    stats = statistics.StatisticsCollector(
+        ["Population", "Food", "Temperature"]
+    )
 
     # Create the states
     title = gsim.TitleScreen(
         screen, constants.TITLE_ASCII_ART, f'v{version("darwinio")}', 1
     )
     disclaimer = gsim.Heading_TextScreen(
         screen, "DISCLAIMER", constants.DISCLAIMER, 2
     )
     license_notice = gsim.TextScreen(screen, constants.LICENSE_NOTICE, 3)
     world_build = gsim.Organism_selection(screen, world, 5)
     init_help_screen = gsim.TextScreen(screen, constants.HELP, 4)
     help_screen = gsim.TextScreen(screen, constants.HELP, 6)
     with gsim.get_asset_path("art", "archaebacteria_halophile.png") as path:
-        main_game = gsim.Simulation(screen, world, path)
+        main_game = gsim.Simulation(screen, world, stats, path)
 
     # Create the state machine
     statemachine = gsim.StateMachine(
         [
             title,
             disclaimer,
             license_notice,
```

### Comparing `darwinio-0.4.0/src/darwinio/brain.py` & `darwinio-0.5.0/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/constants.py` & `darwinio-0.5.0/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/distribution.py` & `darwinio-0.5.0/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/genome.py` & `darwinio-0.5.0/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/graphical_sim.py` & `darwinio-0.5.0/src/darwinio/graphical_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
 from __future__ import annotations
 from typing import Union
 import pygame as pg
 import pygame_gui as pgui
 import darwinio.distribution as dist
 import darwinio.genome as gn
-from importlib.resources import as_file, files
+from importlib.resources import files
 import threading
 import copy
+import darwinio.stats as statistics
 
 
 class World(dist.World):
     def render(self, surface: pg.Surface, image: pg.Surface):
         """
         Renders the organisms on the given surface using the provided image.
 
@@ -273,22 +274,30 @@
         self.manager.update(time_delta)
         return None
 
 
 class Simulation(State):
     """Represents the main screen state of the game."""
 
-    def __init__(self, surface: pg.Surface, world: World, image_path: str):
+    def __init__(
+        self,
+        surface: pg.Surface,
+        world: World,
+        stats: statistics.StatisticsCollector,
+        image_path: str,
+    ):
         """
         Args:
         -----
         surface: The surface on which the state will be rendered.
 
         world: The world object containing the simulation data.
 
+        stats: The stats object for collecting data and plotting.
+
         image_path: The path of the image which will be used for the organism.
         """
 
         surface_size = width, height = surface.get_size()
         super().__init__(surface, surface_size, None)
 
         # Simulation Interface
@@ -322,14 +331,17 @@
         # User Interface
         self.start_button = pgui.elements.UIButton(
             pg.Rect(width - 100, height - 30, 100, 30), "start", self.manager
         )
         self.restart_button = pgui.elements.UIButton(
             pg.Rect(width - 100, height - 60, 100, 30), "restart", self.manager
         )
+        self.graph_viz_button = pgui.elements.UIButton(
+            pg.Rect(0, 40, -1, -1), "graph", self.manager
+        )
         self.population_label = pgui.elements.UITextBox(
             "0", pg.Rect(0, 0, -1, -1), self.manager
         )
         self.temp_slider = Slider(
             "adjust temperature",
             (width - 500, height - 60),
             45,
@@ -340,14 +352,17 @@
             "adjust the food content",
             (width - 950, height - 60),
             500,
             (0, 1200),
             self.manager,
         )
 
+        # Stats
+        self.stats: statistics.StatisticsCollector = stats
+
     def render(self) -> None:
         """render the main screen state."""
         self.sim_surface.fill("black")
         self.world_surface.fill("#5498C6")
         self.world_buffer.render(self.world_surface, self.image)
         self.sim_surface.blit(self.scaled_world_surface, self.world_rect)
         self.surface.blit(self.sim_surface, self.sim_rect)
@@ -383,14 +398,17 @@
                     )
                     self.world.food_distribution = (
                         self.world.generate_distribution(
                             int(new_avg_food_content), 100
                         )
                     )
                     self.food_slider.update()
+            if event.type == pgui.UI_BUTTON_PRESSED:
+                if event.ui_element == self.graph_viz_button:
+                    self.stats.plot(["Population", "Food", "Temperature"])
             self.manager.process_events(event)
 
         keys_pressed = pg.key.get_pressed()
         # moving
         step_size: int = 500
         if keys_pressed[pg.K_UP] or keys_pressed[pg.K_k]:
             self.world_rect.centery += step_size * time_delta
@@ -454,14 +472,21 @@
             and self.running
             and not self.thread.is_alive()
         ):
             self.world_buffer = copy.deepcopy(self.world)
             self.thread = threading.Thread(target=self.world.update_state)
             self.last_time = current_time
             self.thread.start()
+            self.stats.add(
+                (
+                    self.world.get_population(),
+                    self.world.food_distribution.mean(),
+                    self.world.temp_distribution.mean(),
+                )
+            )
 
 
 class TitleScreen(State):
     """
     Represents the title screen state of the game.
 
     Attributes:
@@ -646,14 +671,14 @@
 def tint(surface: pg.Surface, color: pg.Color) -> pg.Surface:
     """create a tinted surface from the given color"""
     new_surface = surface.copy()
     new_surface.fill(color, special_flags=pg.BLEND_RGB_ADD)
     return new_surface
 
 
-def get_asset_path(*paths: str, is_as_file: bool = True):
+def get_asset_path(*paths: str):
     """Gets the path for an asset"""
     file_path = files("darwinio")
     file_path = file_path.joinpath("assets")
     for path in paths:
         file_path = file_path.joinpath(path)
-    return as_file(file_path) if is_as_file else file_path
+    return file_path
```

### Comparing `darwinio-0.4.0/src/darwinio/organism.py` & `darwinio-0.5.0/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/text_sim.py` & `darwinio-0.5.0/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.5.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.5.0/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.5.0/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.5.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.5.0/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.5.0/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.5.0/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.5.0/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.5.0/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.5.0/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.5.0/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.5.0/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.5.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.5.0/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.5.0/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.5.0/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.5.0/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/art/theme.json` & `darwinio-0.5.0/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.5.0/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/LICENSE.md` & `darwinio-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/README.md` & `darwinio-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.4.0/pyproject.toml` & `darwinio-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 "numpy",
+"pandas"    ,
 "pygame-ce>=2.2.1",
 "pygame-gui>=0.6.9",
 "nilsimsa>=0.3.8",
 ]
 scripts = { darwinio = "darwinio.__main__:cli" }
 
 [project.urls]
```

### Comparing `darwinio-0.4.0/PKG-INFO` & `darwinio-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.4.0
+Version: 0.5.0
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Requires-Dist: nilsimsa>=0.3.8
 Requires-Dist: numpy
+Requires-Dist: pandas
 Requires-Dist: pygame-ce>=2.2.1
 Requires-Dist: pygame-gui>=0.6.9
 Description-Content-Type: text/markdown
 
 # Darwinio
 
  ```ascii
```

