# Comparing `tmp/picaso-3.1.tar.gz` & `tmp/picaso-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picaso-3.1.tar", last modified: Tue Apr  4 23:18:52 2023, max compression
+gzip compressed data, was "picaso-3.1.1.tar", last modified: Sun Jul 16 21:41:48 2023, max compression
```

## Comparing `picaso-3.1.tar` & `picaso-3.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-04-04 23:18:52.236286 picaso-3.1/
--rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.1/LICENSE
--rw-r--r--   0 nbatalh1   (503) staff       (20)      734 2023-04-04 23:18:52.236485 picaso-3.1/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)     9222 2023-03-24 18:45:38.000000 picaso-3.1/README.md
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-04-04 23:18:52.232735 picaso-3.1/picaso/
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.1/picaso/__init__.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    41567 2023-03-24 18:45:38.000000 picaso-3.1/picaso/analyze.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    26790 2023-03-24 18:45:38.000000 picaso-3.1/picaso/atmsetup.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.1/picaso/build_3d_input.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.1/picaso/cia_interpolate.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    50616 2023-03-24 18:45:38.000000 picaso-3.1/picaso/climate.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21239 2022-10-25 17:12:52.000000 picaso-3.1/picaso/deq_chem.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2022-10-25 17:12:52.000000 picaso-3.1/picaso/disco.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123112 2022-08-17 14:23:43.000000 picaso-3.1/picaso/elements.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)   169414 2023-03-24 18:45:38.000000 picaso-3.1/picaso/fluxes.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.1/picaso/io_utils.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   288143 2023-03-24 18:45:38.000000 picaso-3.1/picaso/justdoit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    79849 2023-03-24 18:45:38.000000 picaso-3.1/picaso/justplotit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65344 2023-03-24 18:45:38.000000 picaso-3.1/picaso/opacity_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   119834 2023-03-24 18:45:38.000000 picaso-3.1/picaso/optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.1/picaso/phasecurves.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.1/picaso/rayleigh.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     4174 2022-10-25 17:12:52.000000 picaso-3.1/picaso/references.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.1/picaso/run_opa_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10516 2023-03-24 18:45:38.000000 picaso-3.1/picaso/test.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.1/picaso/test_optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     4880 2022-10-25 17:12:52.000000 picaso-3.1/picaso/vulcan.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2523 2022-10-25 17:12:52.000000 picaso-3.1/picaso/wavelength.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-04-04 23:18:52.235868 picaso-3.1/picaso.egg-info/
--rw-r--r--   0 nbatalh1   (503) staff       (20)      734 2023-04-04 23:18:52.000000 picaso-3.1/picaso.egg-info/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)      675 2023-04-04 23:18:52.000000 picaso-3.1/picaso.egg-info/SOURCES.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-04-04 23:18:52.000000 picaso-3.1/picaso.egg-info/dependency_links.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.1/picaso.egg-info/not-zip-safe
--rw-r--r--   0 nbatalh1   (503) staff       (20)      150 2023-04-04 23:18:52.000000 picaso-3.1/picaso.egg-info/requires.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2023-04-04 23:18:52.000000 picaso-3.1/picaso.egg-info/top_level.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2023-04-04 23:18:52.237525 picaso-3.1/setup.cfg
--rw-r--r--   0 nbatalh1   (503) staff       (20)     3193 2023-04-04 23:17:13.000000 picaso-3.1/setup.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.145520 picaso-3.1.1/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.1.1/LICENSE
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      736 2023-07-16 21:41:48.145635 picaso-3.1.1/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     9222 2023-03-24 18:45:38.000000 picaso-3.1.1/README.md
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.142881 picaso-3.1.1/picaso/
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.1.1/picaso/__init__.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    41567 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/analyze.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28434 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/atmsetup.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/build_3d_input.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/cia_interpolate.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    50616 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/climate.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21239 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/deq_chem.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/disco.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123112 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/elements.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)   169414 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/fluxes.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/io_utils.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   288719 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/justdoit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    80150 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/justplotit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65867 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/opacity_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   118894 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.1.1/picaso/phasecurves.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.1.1/picaso/rayleigh.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     4174 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/references.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/run_opa_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10516 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/test.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/test_optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     4880 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/vulcan.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2523 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/wavelength.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.145268 picaso-3.1.1/picaso.egg-info/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      736 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      675 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/SOURCES.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/dependency_links.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.1.1/picaso.egg-info/not-zip-safe
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      158 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/requires.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/top_level.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2023-07-16 21:41:48.146178 picaso-3.1.1/setup.cfg
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3216 2023-07-16 21:34:56.000000 picaso-3.1.1/setup.py
```

### Comparing `picaso-3.1/LICENSE` & `picaso-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picaso-3.1/PKG-INFO` & `picaso-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picaso
-Version: 3.1
+Version: 3.1.1
 Summary: planetary intesity code for atmospheric scattering observations
 Home-page: https://natashabatalha.github.io/picaso
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
 Download-URL: https://github.com/natashabatalha/picaso
 Platform: UNKNOWN
```

### Comparing `picaso-3.1/README.md` & `picaso-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/analyze.py` & `picaso-3.1.1/picaso/analyze.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/atmsetup.py` & `picaso-3.1.1/picaso/atmsetup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .elements import ELEMENTS as ele 
 import json 
 import os
+import re
 from .io_utils import read_json
 import astropy.units as u
 import astropy.constants as c
 import pandas as pd
 import warnings 
 import numpy as np
 from .wavelength import get_cld_input_grid
@@ -233,90 +234,111 @@
         available_ray_mol : list of str
             list of available rayleigh molecules 
         available_continuum : list of str
             list of available continuum molecules 
         """
         self.rayleigh_molecules = []
         self.continuum_molecules = []
-        if "H2" in self.molecules:
+
+        simple_names = [convert_to_simple(i) for i in self.molecules]
+        
+        if "H2" in simple_names:
             self.continuum_molecules += [['H2','H2']]
-        if ("H2" in self.molecules) and ("He" in self.molecules):
+        if ("H2" in simple_names) and ("He" in simple_names):
             self.continuum_molecules += [['H2','He']]
-        if ("H2" in self.molecules) and ("N2" in self.molecules):
+        if ("H2" in simple_names) and ("N2" in simple_names):
             self.continuum_molecules += [['H2','N2']]   
-        if  ("H2" in self.molecules) and ("H" in self.molecules):
+        if  ("H2" in simple_names) and ("H" in simple_names):
             self.continuum_molecules += [['H2','H']]
-        if  ("H2" in self.molecules) and ("CH4" in self.molecules):
+        if  ("H2" in simple_names) and ("CH4" in simple_names):
             self.continuum_molecules += [['H2','CH4']]
-        if  ("N2" in self.molecules):
+        if  ("N2" in simple_names):
             self.continuum_molecules += [['N2','N2']]
-        if  ("CO2" in self.molecules):
+        if  ("CO2" in simple_names):
             self.continuum_molecules += [['CO2','CO2']]      
-        if  ("O2" in self.molecules):
+        if  ("O2" in simple_names):
             self.continuum_molecules += [['O2','O2']]    
 
-        if ("H-" in self.molecules):
+        if ("H-" in simple_names):
             self.continuum_molecules += [['H-','bf']]
-        if ("H" in self.molecules) and ("electrons" in self.level.keys()):
+        if ("H" in simple_names) and ("electrons" in self.level.keys()):
             self.continuum_molecules += [['H-','ff']]
-        if ("H2" in self.molecules) and ("electrons" in self.level.keys()):
+        if ("H2" in simple_names) and ("electrons" in self.level.keys()):
             self.continuum_molecules += [['H2-','']]
         #now we can remove continuum molecules from self.molecules to keep them separate 
         if 'H+' in ['H','H2-','H2','H-','He','N2']: self.add_warnings('No H+ continuum opacity included')
 
         #remove anything not in opacity file
         cm =[]
         for i in self.continuum_molecules: 
             if ''.join(i) in available_continuum: cm += [i]
         self.continuum_molecules = cm
 
         #and rayleigh opacity
-        for i in self.molecules: 
+        for i in simple_names: 
             if i in available_ray_mol : self.rayleigh_molecules += [i]
 
+        
         #self.molecules = np.array([ x for x in self.molecules if x not in ['H','H2-','H2','H-','He','N2', 'H+'] ])
 
     def get_weights(self, molecule):
         """
         Automatically gets mean molecular weights of any molecule. Requires that 
         user inputs case sensitive molecules i.e. TiO instead of TIO. 
 
         Parameters
         ----------
         molecule : str or list
             any molecule string e.g. "H2O", "CH4" etc "TiO" or ["H2O", 'CH4']
+            Isotopologues should be specified with a dash separating the 
+            elemtents. E.g. 12C-16O2 or 13C-16O2. If you only want to specify one 
+            then you would have 12C-O2. 
 
         Returns
         -------
         dict 
             molecule as keys with molecular weights as value
-        """
+        """    
         weights = {}
+        separator='_' #e.g. C_16O2 NOT C-16O2
         if not isinstance(molecule,list):
-            molecule = [molecule]
-
-        for i in molecule:
-            molecule_list = []
-            for j in range(0,len(i)):
-                try:
-                    molecule_list += [float(i[j])]
-                except: 
-                    if i[j].isupper(): molecule_list += [i[j]] 
-                    elif i[j].islower(): molecule_list[-1] =  molecule_list[-1] + i[j]
-            totmass=0
-            for j in range(0,len(molecule_list)): 
+                molecule = [molecule]
                 
-                if isinstance(molecule_list[j],str):
-                    elem = ele[molecule_list[j]]
-                    try:
-                        num = float(molecule_list[j+1])
-                    except: 
-                        num = 1 
-                    totmass += elem.mass * num
-            weights[i] = totmass
+        for i in molecule:
+            totmass = 0
+            #this indicates the user has specified the isotope
+            if separator in i: 
+                elements = [separate_molecule_name(j) for j in i.split(separator)]
+            else:    
+                elements = separate_molecule_name(i)
+
+            for iele in elements:
+                if isinstance(iele,list):
+                    #this is the user's specified isotope
+                    if len(iele)==1:
+                        iele = iele[0]
+                        iso_num = 'main'
+                    else:
+                        iso_num = int(iele[0])
+                        iele = iele[1]
+                else: 
+                    iso_num = 'main'
+
+                sep = separate_string_number(iele)
+                if len(sep)==1:
+                    el, num = sep[0], 1
+                else: 
+                    el, num = sep
+                #default isotope
+                if iso_num=='main':
+                    iso_num = list(ele[el].isotopes.keys())[0] 
+                totmass += ele[el].isotopes[iso_num].mass*float(num)
+
+            weights[i]=totmass
+        
         return weights
 
 
     def get_mmw(self):
         """
         Returns the mean molecular weight of the atmosphere 
         """
@@ -625,14 +647,44 @@
             x = self.flux_at_top
             df['thermal_unit'] = 'erg/cm2/s/cm'
             df['thermal_3d'] = x
         except:
             pass
 
         return df
+
+def convert_to_simple(iso_name):
+    """
+    Converts iso name (e.g. 13C-16O2 to CO2)
+    Returns same name if not (e.g. CO2 gives CO2)
+    """
+    separator = '_'
+    if separator not in iso_name: return iso_name
+    separate = [separate_molecule_name(j) for j in iso_name.split('-')]
+    mol=''
+    for i in separate: 
+        if len(i)>1:
+            mol+=i[1]
+        else: 
+            mol += i[0]
+    return mol
+
+def separate_molecule_name(molecule_name):
+    """used for separating molecules
+    For example, CO2 becomes "C" "O2"
+    """
+    elements = re.findall('[A-Z][a-z]?\d*|\d+', molecule_name)
+    return elements
+def separate_string_number(string):
+    """used for separating numbers from molecules
+    For example, CO2 becomes "C" "O2" in `separate_molecule_name` 
+    then this function turns it into [['C'],['O','2']]
+    """
+    elements = re.findall('[A-Za-z]+|\d+', string)
+    return elements
 """
 ## not using this for now.
 def hunt(xx , n , x, jlow):
     flag1 = 0
     if ((jlow <= 0) or (jlow > n-1)): # for py
         jlow = 0
         jhigh= n+1 -1 # for py
```

### Comparing `picaso-3.1/picaso/build_3d_input.py` & `picaso-3.1.1/picaso/build_3d_input.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/cia_interpolate.py` & `picaso-3.1.1/picaso/cia_interpolate.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/climate.py` & `picaso-3.1.1/picaso/climate.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/deq_chem.py` & `picaso-3.1.1/picaso/deq_chem.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/disco.py` & `picaso-3.1.1/picaso/disco.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/elements.py` & `picaso-3.1.1/picaso/elements.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/fluxes.py` & `picaso-3.1.1/picaso/fluxes.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/io_utils.py` & `picaso-3.1.1/picaso/io_utils.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/justdoit.py` & `picaso-3.1.1/picaso/justdoit.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     Returns
     -------
     xarray.Dataset
         this xarray dataset can be easily passed to justdoit.input_xarray to run a spectrum 
         
     """
         
-    full_output = df['full_output']
+    full_output = df['full_output'] if 'full_output' in df.keys() else  df['spectrum_output']['full_output']
     df_atmo = picaso_class.inputs['atmosphere']['profile']
     molecules_included = full_output['weights']
     
     #start with simple layer T
     data_vars=dict(temperature = (["pressure"], 
                                   df_atmo['temperature'],
                                   {'units': 'Kelvin'}))
@@ -895,18 +895,14 @@
 
 
     #pressure assumption
     p_reference =  inputs['approx']['p_reference']
 
     ############# DEFINE ALL GEOMETRY USED IN CALCULATION #############
     #see class `inputs` attribute `phase_angle`
-    
-
-    #phase angle 
-    phase_angle = inputs['phase_angle']
     #get geometry
     geom = inputs['disco']
 
     ng, nt = geom['num_gangle'], geom['num_tangle']
     gangle,gweight,tangle,tweight = geom['gangle'], geom['gweight'],geom['tangle'], geom['tweight']
     lat, lon = geom['latitude'], geom['longitude']
     cos_theta = geom['cos_theta']
@@ -1547,15 +1543,15 @@
         self.inputs['star']['radius_unit'] = 'nostar' 
         self.inputs['star']['flux'] = 'nostar' 
         self.inputs['star']['wno'] = 'nostar' 
         self.inputs['star']['semi_major'] = 'nostar' 
         self.inputs['star']['semi_major_unit'] = 'nostar' 
 
     def star(self, opannection,temp=None, metal=None, logg=None ,radius = None, radius_unit=None,
-        semi_major=None, semi_major_unit = None, deq = False, 
+        semi_major=None, semi_major_unit = None, #deq = False, 
         database='ck04models',filename=None, w_unit=None, f_unit=None):
         """
         Get the stellar spectrum using pysynphot and interpolate onto a much finer grid than the 
         planet grid. 
 
         Parameters
         ----------
@@ -1719,17 +1715,20 @@
         self.inputs['star']['radius'] = r 
         self.inputs['star']['radius_unit'] = radius_unit 
         self.inputs['star']['flux'] = bin_flux_star
         self.inputs['star']['wno'] = wno_planet
         self.inputs['star']['semi_major'] = semi_major 
         self.inputs['star']['semi_major_unit'] = semi_major_unit         
 
+        """
+        return not needed anymore
         if deq == True :
             FOPI = fine_flux_star * ((r/semi_major)**2)
             return FOPI
+        """
 
     def atmosphere(self, df=None, filename=None, exclude_mol=None, verbose=True, **pd_kwargs):
         """
         Builds a dataframe and makes sure that minimum necessary parameters have been suplied.
         Sets number of layers in model.  
 
         Parameters
@@ -2057,14 +2056,17 @@
         try: 
             g = self.inputs['planet']['gravity']/100 #m/s2 for sonora
         except AttributeError : 
             raise Exception('Oops! Looks like gravity has not been set. Can you please \
                 run the gravity function to set gravity')
 
         flist = os.listdir(os.path.join(sonora_path))
+        #ignore hidden drive files 
+        flist = [i for i in flist if '._' != i[0:2]]
+
 
         if ('cmp.gz' in str(flist)):
 
             flist = [i.split('/')[-1] for i in flist if 'gz' in i]
             ts = [i.split('g')[0][1:] for i in flist if 'gz' in i]
             gs = [i.split('g')[1].split('nc')[0] for i in flist]
 
@@ -3720,15 +3722,16 @@
         self.inputs['climate']['r_star'] = r_star # solar
         self.inputs['climate']['logg'] = logg # cgs
         self.inputs['climate']['metal'] = metal # solar
         self.inputs['climate']['semi_major'] = semi_major # au
         self.inputs['climate']['r_planet'] = r_planet # jupiter radii
 
     def climate(self, opacityclass, save_all_profiles = False, as_dict=True,with_spec=False,
-        save_all_kzz = False, diseq_chem = False, self_consistent_kzz =False, kz = None):#,
+        save_all_kzz = False, diseq_chem = False, self_consistent_kzz =False, kz = None, 
+        on_fly=False,gases_fly=None, chemeq_first=True):#,
         #vulcan_run = False, photochem=False,on_fly=False,gases_fly=None,mhdeq=None,CtoOdeq=None ):
         """
         Top Function to run the Climate Model
 
         Parameters
         -----------
         opacityclass : class
@@ -3750,15 +3753,15 @@
         photochem : bool
             (beta, contact developers)If you want to run photochemistry in vulcan on the fly (takes much longer),True/False
         
         """
         #save to user 
         all_out = {}
 
-        vulcan_run=False;photochem=False;on_fly=False;gases_fly=None;mhdeq=None;CtoOdeq=None
+        vulcan_run=False;photochem=False;#on_fly=False;gases_fly=None;mhdeq=None;CtoOdeq=None
         if (vulcan_run or photochem): 
             raise Exception("Vulcan and photochemistry is not yet a live feature. If you are interesting in helping the development team, contact us.")
         
         #get necessary parameters from opacity ck-tables 
         wno = opacityclass.wno
         delta_wno = opacityclass.delta_wno
         nwno = opacityclass.nwno
@@ -3791,16 +3794,14 @@
         #otherwise assume that there is stellar irradiation 
         else:
             rfacv = self.inputs['climate']['rfacv']
             r_star = self.inputs['star']['radius'] 
             r_star_unit = self.inputs['star']['radius_unit'] 
             semi_major = self.inputs['star']['semi_major']
             semi_major_unit = self.inputs['star']['semi_major_unit'] 
-            
-
             fine_flux_star  = self.inputs['star']['flux']  # erg/s/cm^2
             FOPI = fine_flux_star * ((r_star/semi_major)**2)
 
         all_profiles= []
         if save_all_profiles:
             save_profile = 1
         else :
@@ -3843,37 +3844,41 @@
         x_max_mult=7.0
         
 
         final = False
         flag_hack = False
 
         
-        pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
             TEMP1,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
             rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , cloudy, cld_species,mh,fsed,flag_hack, save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,first_call_ever=True)
 
         # second convergence call
         it_max= 7
         itmx= 5
         conv = 5.0
         convt=4.0
         x_max_mult=7.0
 
         
         final = False
-        pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
                     temperature,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
                     rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack,save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop )   
 
-        pressure, temp, dtdp, nstr_new, flux_plus_final, df, all_profiles, opd_now,w0_now,g0_now =find_strat(pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
+        if chemeq_first: pressure, temp, dtdp, nstr_new, flux_plus_final, df, all_profiles, opd_now,w0_now,g0_now =find_strat(pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
                              t_table, p_table, grad, cp, opacityclass, grav, 
                              rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed, flag_hack, save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
 
         
         if diseq_chem:
+            #Starting with user's guess since there was no request to converge a chemeq profile first 
+            if not chemeq_first: 
+                temp = TEMP1
+
             wv196 = 1e4/wno
 
             # first change the nstr vector because need to check if they grow or not
             # delete upper convective zone if one develops
             
             del_zone =4 # move 4 levels deeper
             if (nstr[1] > 0) & (nstr[4] > 0) & (nstr[3] > 0) :
@@ -3892,17 +3897,16 @@
             if nstr[1] >= nlevel -2 : # making sure we haven't pushed zones too deep
                 nstr[1] = nlevel -4
             if nstr[4] >= nlevel -2:
                 nstr[4] = nlevel -3
             
             print("New NSTR status is ", nstr)
 
-            #was for check SM 
-            #pressure,temp =np.loadtxt("/data/users/samukher/Disequilibrium-picaso/picaso/tstart_800_562.dat",usecols=[1,2],unpack=True) 
-            #temp+=300            
+            
+
             bundle = inputs(calculation='brown')
 
             bundle.phase_angle(0)
             bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
             bundle.add_pt( temp, pressure)
             bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
             DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
@@ -3914,75 +3918,79 @@
             if save_all_kzz == True :
                 save_kzz = 1
             else :
                 save_kzz = 0
             
             #here begins the self consistent Kzz calculation 
             # MLT plus some prescription in radiative zone
-            if self_consistent_kzz: 
-
+            if self_consistent_kzz or (not chemeq_first): 
+                
                 flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, delta_wno, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
                 COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
                 ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
                 wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,True, True)#True for reflected, True for thermal
 
                 flux_net_ir_layer = flux_net_ir_layer_full[:]
                 flux_plus_ir_attop = flux_plus_ir_full[0,:] 
                 calc_type = 0
+                
                 # use mixing length theory to calculate Kzz profile
-                kz = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
+                if self_consistent_kzz: 
+                    kz = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
             
             
             
             
             # shift everything to the 661 grid now.
             #mh = '+0.0'  #don't change these as the opacities you are using are based on these 
             #CtoO = '1.0' # don't change these as the opacities you are using are based on these #
             filename_db=os.path.join(__refdata__, 'climate_INPUTS/ck_cx_cont_opacities_661.db')
             
             if on_fly:
                 print("From now I will mix "+str(gases_fly)+" only on--the--fly")
                 #mhdeq and ctodeq will be auto by opannection
                 #NO Background, just CIA + whatever in gases_fly
-                ck_db=os.path.join(__refdata__, 'climate_INPUTS/sonora_2020_feh'+mhdeq+'_co_'+CtoOdeq+'.data.196')
-                opacityclass = opannection(ck=True, ck_db=ck_db,filename_db=filename_db,deq = True,on_fly=True,gases_fly=gases_fly)
+                #ck_db=os.path.join(__refdata__, 'climate_INPUTS/sonora_2020_feh'+mhdeq+'_co_'+CtoOdeq+'.data.196')
+                opacityclass = opannection(ck=True, 
+                    ck_db=opacityclass.ck_filename,filename_db=filename_db,
+                    deq = True,on_fly=True,gases_fly=gases_fly)
             else:
                 #phillips comparison (discontinued) 
                 #background + gases 
                 #ck_db=os.path.join(__refdata__, 'climate_INPUTS/m+0.0_co1.0.data.196')
                 opacityclass = opannection(ck=True, ck_db=opacityclass.ck_filename,
                     filename_db=filename_db,deq = True,on_fly=False)
 
         
             
             
             if cloudy == 1:    
                 wv661 = 1e4/opacityclass.wno
                 opd_cld_climate,g0_cld_climate,w0_cld_climate = initiate_cld_matrices(opd_cld_climate,g0_cld_climate,w0_cld_climate,wv196,wv661)
                 print(np.shape(opd_cld_climate))
+            
+            #Rerun star so that F0PI can now be on the 
+            #661 grid 
             if 'nostar' in self.inputs['star'].values():
-                rfacv=0.0 
                 FOPI = np.zeros(opacityclass.nwno) + 1.0
-                T_star = None
-                r_star = None
-                logg = None
-                metal = None
-                semi_major = None
-                r_planet = None
-            #otherwise assume that there is stellar irradiation 
             else:
-                rfacv = self.inputs['climate']['rfacv']
-                T_star = self.inputs['climate']['T_star']
-                r_star = self.inputs['climate']['r_star']
-                logg = self.inputs['climate']['logg']
-                metal = self.inputs['climate']['metal']
-                semi_major = self.inputs['climate']['semi_major']
-                r_planet = self.inputs['climate']['r_planet']
-                FOPI = self.star(opacityclass, temp =T_star,metal =metal, logg =logg, radius = r_star, radius_unit=u.R_sun,semi_major= semi_major , semi_major_unit = u.AU, deq= True)
-
+                T_star = self.inputs['star']['temp']
+                r_star = self.inputs['star']['radius']
+                r_star_unit = self.inputs['star']['radius_unit']
+                logg = self.inputs['star']['logg']
+                metal =  self.inputs['star']['metal']
+                semi_major = self.inputs['star']['semi_major']
+                sm_unit = self.inputs['star']['semi_major_unit']
+                database = self.inputs['star']['database']
+                self.star(opacityclass, database=database,temp =T_star,metal =metal, logg =logg, 
+                    radius = r_star, radius_unit=u.Unit(r_star_unit),semi_major= semi_major , 
+                    semi_major_unit = u.Unit(sm_unit))
+                fine_flux_star  = self.inputs['star']['flux']  # erg/s/cm^2
+                FOPI = fine_flux_star * ((r_star/semi_major)**2)
+            
             if not vulcan_run:
                 quench_levels, t_mix = quench_level(pressure, temp, kz ,mmw, grav, return_mix_timescale= True) # determine quench levels
 
                 all_kzz = np.append(all_kzz, t_mix) # save kzz
 
                 print("Quench Levels are CO, CO2, NH3, HCN, PH3 ", quench_levels) # print quench levels
                 
@@ -4470,15 +4478,18 @@
 def toon_phase_coefficients(printout=True):
     """Retrieve options for coefficients used in Toon calculation
     """
     return ["quadrature","eddington"]
 
 def profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
             temp,pressure,FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh,fsed,flag_hack, save_profile, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer=None, flux_plus_ir_attop=None,first_call_ever=False):
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+             cloudy, cld_species,mh,fsed,flag_hack, save_profile, 
+             all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,
+             flux_net_ir_layer=None, flux_plus_ir_attop=None,first_call_ever=False):
     """
     Function iterating on the TP profile by calling tstart and changing opacities as well
     Parameters
     ----------
     it_max : int
         Maximum iterations allowed in the inner no opa change loop
     itmx : int
@@ -5402,15 +5413,19 @@
         kz = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
     
     ## begin bigger loop which gets opacities
     for iii in range(itmx):
         
         temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(nofczns,nstr,it_max,conv,x_max_mult, 
             rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
-            grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
+            grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, 
+            COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, 
+            W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, 
+            single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+            tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
         '''
         if (temp <= min(opacityclass.cia_temps)).any():
             wh = np.where(temp <= min(opacityclass.cia_temps))
             if len(wh[0]) <= 30 :
                 print(len(wh[0])," points went off the opacity grid. Correcting those.")
                 temp = correct_profile(temp,pressure,wh,min(opacityclass.cia_temps))
             else :
```

### Comparing `picaso-3.1/picaso/justplotit.py` & `picaso-3.1.1/picaso/justplotit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1838,15 +1838,16 @@
         plt.legend(fontsize=10)        
     
         return T_B , f
     else: 
         return T_B
 
 
-def animate_convergence(clima_out, picaso_bundle, opacity, wave_range=[0.3,6],
+def animate_convergence(clima_out, picaso_bundle, opacity, calculation='thermal',
+    wave_range=[0.3,6],
     molecules=['H2O','CH4','CO','NH3']):
     """
     Function to animate climate convergence given all profiles that were 
     computed throughout the climate run 
     Animates from the first guess through to the final converged state. 
     Runs spectra for each of those cases. 
     
@@ -1864,14 +1865,15 @@
     molecules : list 
         list of strings for what molecules to animate
     
     Returns
     -------
     matplotlib.animation
     """
+    map_calc = {'thermal':'thermal','reflected':'albedo','transmission':'transit_depth'}
     t_eq,p_eq,all_profiles_eq = (
                 np.copy(clima_out['temperature']), 
                 np.copy(clima_out['pressure']), 
                 np.copy(clima_out['all_profiles']))
     
     nlevel = len(t_eq)
     mols_to_plot = {i:np.zeros(len(all_profiles_eq)) for i in molecules}
@@ -1880,16 +1882,16 @@
     for i in range(int(len(all_profiles_eq)/nlevel)):
         
         picaso_bundle.add_pt(all_profiles_eq[i*nlevel:(i+1)*nlevel], 
                              p_eq)
 
         picaso_bundle.premix_atmosphere(opacity,picaso_bundle.inputs['atmosphere']['profile'])
 
-        df_spec = picaso_bundle.spectrum(opacity,full_output=True)
-        spec[i,:] = df_spec['thermal']
+        df_spec = picaso_bundle.spectrum(opacity,calculation=calculation,full_output=True)
+        spec[i,:] = df_spec[map_calc[calculation]]
         for imol in molecules:
             mols_to_plot[imol][i*nlevel:(i+1)*nlevel] = picaso_bundle.inputs['atmosphere']['profile'][imol]
     
     wh = np.where( (1e4/df_spec['wavenumber'] > wave_range[0]) & (1e4/df_spec['wavenumber'] < wave_range[1]))
     wv = 1e4/df_spec['wavenumber'][wh]    
 
 
@@ -1912,32 +1914,35 @@
 
     temp = all_profiles_eq[0*nlevel:(0+1)*nlevel]
     lines = {}
     for imol,col in zip(molecules,Colorblind8):
         lines[imol], = ax['B'].loglog(mols_to_plot[imol][0:nlevel], p_eq,linewidth=3,color=col, label=imol)
 
     lines['temp'], = ax['A'].semilogy(temp, p_eq,linewidth=3,color='k')
-    lines['spec'], = ax['C'].semilogy(1e4/df_spec['wavenumber'], spec[0,:],linewidth=3,color="k")
+    if calculation=='thermal':
+        lines['spec'], = ax['C'].semilogy(1e4/df_spec['wavenumber'], spec[0,:],linewidth=3,color="k")
+    else: 
+        lines['spec'], = ax['C'].plot(1e4/df_spec['wavenumber'], spec[0,:],linewidth=3,color="k")
 
     def init():
         #line.set_ydata(np.ma.array(x, mask=True))
 
         ax['A'].set_xlabel('Temperature [K]',fontsize=30)
         ax['A'].set_ylabel('Pressure [Bars]',fontsize=30)
         ax['A'].set_xlim(200,2900)
         ax['A'].set_ylim(205,1.8e-4)
         ax['B'].set_xlabel('Abundance [V/V]',fontsize=30)
         ax['B'].set_ylabel('Pressure [Bars]',fontsize=30)
         ax['B'].set_xlim(1e-6,1e-2)
         ax['B'].set_ylim(205,1.8e-4)
         ax['B'].legend(fontsize=20)
         ax['C'].set_xlabel('Wavelength [$\mu$m]',fontsize=30)
-        ax['C'].set_ylabel('Flux',fontsize=30)
+        ax['C'].set_ylabel('Spectrum',fontsize=30)
         ax['C'].set_xlim(0,6)
-        ax['C'].set_ylim(1e7,1e14)
+        #ax['C'].set_ylim(1e7,1e14)
         ax['A'].minorticks_on()
         ax['A'].tick_params(axis='both',which='major',length =30, width=2,direction='in',labelsize=30)
         ax['A'].tick_params(axis='both',which='minor',length =10, width=2,direction='in',labelsize=30)
         ax['B'].minorticks_on()
         ax['B'].tick_params(axis='both',which='major',length =30, width=2,direction='in',labelsize=30)
         ax['B'].tick_params(axis='both',which='minor',length =10, width=2,direction='in',labelsize=30)
         ax['C'].minorticks_on()
```

### Comparing `picaso-3.1/picaso/opacity_factory.py` & `picaso-3.1.1/picaso/opacity_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,15 +767,15 @@
         #path to richard's data
         fdata = os.path.join(og_directory,molecule,'p_'+str(int(i)))
 
 
         #Grab 1060 in various format data
         if molecule in ['Cs','K','Li','Na','Rb']:
             openf=FortranFile(fdata,'r')
-            dset = openf.read_ints(dtype=np.float)
+            dset = openf.read_ints(dtype=float)
             og_wvno_grid=np.arange(numw[i-1])*delwn[i-1]+start[i-1] 
         elif molecule =='CH3D':
             df = pd.read_csv(os.path.join(og_directory,molecule,'fort.{0}.bz2'.format(int(i)))
                              ,delim_whitespace=True, skiprows=23,header=None)
             dset=df[1].values
             og_wvno_grid=df[0].values
         else: 
@@ -896,24 +896,26 @@
     else:
         mol_dir = os.path.join(og_directory,molecule)
     
     #determine file type
     find_p_files = glob.glob(os.path.join(mol_dir,'*p_*'))
     find_npy_files = glob.glob(os.path.join(mol_dir,'*npy*'))
     find_txt_files =  glob.glob(os.path.join(mol_dir,'*txt*'))
+    find_fort_files =  glob.glob(os.path.join(mol_dir,'fort.*'))
 
     if len(find_p_files)>1000:
         ftype = 'fortran_binary'
     elif len(find_npy_files)>1000: 
         ftype = 'python'
     elif len(find_txt_files)>1000:
         ftype='lupu_txt'
+    elif len(find_fort_files)>1000:
+        ftype='rfree_fort'
     else: 
         raise Exception('Could not find npy or p_ files. npy are assumed to be read via np.load, where as p_ files are assumed to be unformatted binary or alkali files')
-        
     read_fits = os.path.join(mol_dir,'readomni.fits' )
     lupu_wave= os.path.join(mol_dir,'wavelengths.txt' )
     if os.path.exists(read_fits):
         # Get Richard's READ ME information
         hdulist = fits.open(read_fits)
         sfits = hdulist[1].data
         numw = sfits['Valid rows'] #defines number of wavelength points for each 1060 layer
@@ -924,38 +926,45 @@
     else: 
         #ehsan makes his opacities on uniform 
         numw = s1460['number_wave_pts'].values.astype(int)
         delwn = s1460['delta_wavenumber'].values.astype(float)
         start = s1460['start_wavenumber'].values.astype(float)
         
 
-
+    
     for i,p,t in zip(ifile,pres,temp):  
         #path to data
         if 'fortran' in ftype:
             fdata = os.path.join(mol_dir, 'p_'+str(int(i)))
+        elif 'rfree_fort' in ftype: 
+            fdata = os.path.join(mol_dir, 'fort.'+str(int(i)))
         elif 'python' in ftype: 
             fdata = os.path.join(mol_dir, str(int(i))+'.npy')
         elif 'lupu' in ftype: 
             mbar = p*1e3
             fdata = os.path.join(mol_dir,f'{molecule}_{mbar:.2e}mbar_{t:.0f}K.txt') 
+        
         #Grab 1460 in various format data
         if 'lupu' in ftype: 
             dset =  pd.read_csv(fdata,skiprows=2,header=None).values[:,0]
             og_wvno_grid = 1e4/pd.read_csv(lupu_wave).iloc[:,0].values
         elif molecule in alks:
             dset = pd.read_csv(fdata)
             og_wvno_grid = dset['wno'].values.astype(float)
             dset = dset[molecule].values.astype(float)
         elif 'fortran' in ftype: 
             dset = np.fromfile(fdata, dtype=float) 
             og_wvno_grid=np.arange(numw[i-1])*delwn[i-1]+start[i-1]
         elif 'python' in ftype: 
             dset = np.load(open(fdata,'rb'))
-            og_wvno_grid=np.arange(numw[i-1])*delwn[i-1]+start[i-1]            
+            og_wvno_grid=np.arange(numw[i-1])*delwn[i-1]+start[i-1]  
+        elif 'rfree_fort' in ftype: 
+            df = pd.read_csv(fdata,delim_whitespace=True, skiprows=27, header=None, names=['wno','cx'])
+            dset=df.loc[:,'cx'].values
+            og_wvno_grid=df.loc[:,'wno'].values           
 
         if not insert_direct:
             #interp on high res grid
             #basic interpolation here onto a new wavegrid that 
             dset = np.interp(interp_wvno_grid,og_wvno_grid, dset,right=1e-50, left=1e-50)
             dset[dset<1e-200] = 1e-200 
             #resample evenly
@@ -1216,15 +1225,15 @@
     temp=s['temperature'].values.astype(float)
 
     for i,p,t in zip(list(range(1,1061)),pres,temp):  
         #path to richard's data
         fdata = os.path.join(og_directory,molecule,'p_'+str(int(i)))
 
         #Grab 1060 format data
-        dset = np.fromfile(fdata, dtype=float)   #openf.read_ints(dtype=np.float)
+        dset = np.fromfile(fdata, dtype=float)   #openf.read_ints(dtype=float)
         og_wvno_grid=np.arange(numw[i-1])*delwn[i-1]+start[i-1]      
 
         #interp on high res grid
         dset = np.interp(interp_wvno_grid,og_wvno_grid, dset,right=1e-33, left=1e-33)
 
         #vectorize grab median from sample
         y = vectorize_rebin_median(BINS,dset)
@@ -1385,17 +1394,16 @@
                     FROM molecular
                     WHERE molecule in {}
                     AND ptid in {}""".format(str(tuple(species)), str(tuple(ind_pt))))
 
 
     data= cur.fetchall()
 
-    temp_nearest = [pt_pairs[i][2] for i in ind_pt]
-    pres_nearest = [pt_pairs[i][1] for i in ind_pt]
-
+    temp_nearest = [pt_pairs[i-1][2] for i in ind_pt]
+    pres_nearest = [pt_pairs[i-1][1] for i in ind_pt]
     restruct = {i:{} for i in species}
     for i in restruct.keys():
         for t in temp_nearest:
             restruct[i][t] = {}
     for im, iid,ip,it, dat in data : restruct[im][it][ip] = dat
 
     cur.execute('SELECT wavenumber_grid FROM header')
@@ -1507,14 +1515,17 @@
     alkali_dir : str 
         (Optional) Directory of alkalis or "individual_file" which is the method to use for Roxana Lupus data. 
     verbose: bool 
         (Optional) prints out status of which p,t, point the code is at 
 
     """
     grid_file = os.path.join(og_directory,'grid1460.csv')
+    npres = 20 
+    ntemp = 73 
+    ngauss = order*2 
 
     s1460 = pd.read_csv(grid_file,dtype=str)
     #all pressures
     pres=s1460['pressure_bar'].values.astype(float)
     #all temperatures
     temp=s1460['temperature_K'].values.astype(float)
 
@@ -1569,15 +1580,15 @@
     
     gi,wi = g_w_2gauss(order,gfrac)
     
     if not isinstance(wv_file_name,type(None)):
         wvno_low,wvno_high = get_wvno_grid(wv_file_name)
     else: 
         wvno_low,wvno_high = get_wvno_grid(None, min_wavelength, max_wavelength, R)
-    k_coeff_arr = np.zeros(shape=(20,73,len(wvno_low),8))
+    k_coeff_arr = np.zeros(shape=(npres,ntemp,len(wvno_low),ngauss))
     ctp,ctt = 0,0
     for i,p,t in zip(ifile,pres,temp):  
         #path to data
         if 'fortran' in ftype:
             fdata = os.path.join(mol_dir, 'p_'+str(int(i)))
         elif 'python' in ftype: 
             fdata = os.path.join(mol_dir, str(int(i))+'.npy')
```

### Comparing `picaso-3.1/picaso/optics.py` & `picaso-3.1.1/picaso/optics.py`

 * *Files 2% similar despite different names*

```diff
@@ -642,15 +642,16 @@
         This should be in the references directory on Github. This has all the continuum opacity 
         that you need (e.g. H2H2). It also has some extra cross sections that you may want to add 
         in like Karkoschka methane and the optical ozone band. 
     wave_range : list 
         NOT FUNCTIONAL YET. 
         Wavelength range to compuate in the format [min micron, max micron]
     """
-    def __init__(self, ck_dir, cont_dir, wave_range=None, deq=False, on_fly=False,gases_fly=None):
+    def __init__(self, ck_dir, cont_dir, wave_range=None, 
+        deq=False, on_fly=False,gases_fly=None):
         self.ck_filename = ck_dir
         #read in the full abundance file sot hat we can check the number of kcoefficient layers 
         #this should either be 1460 or 1060
         self.full_abunds =  pd.read_csv(os.path.join(self.ck_filename,'full_abunds'),
             delim_whitespace=True)
         self.kcoeff_layers = self.full_abunds.shape[0]
 
@@ -667,27 +668,31 @@
             
             self.get_available_continuum()
             self.get_available_rayleigh()
             self.run_cia_spline()
             
         
         elif (deq == True) and (on_fly == False) :
-            #self.get_gauss_pts_661()#Discontinuing to delete repetetive code
+            #this option follows the old method where we used 
+            #661 fortran files computed by T.Karidali
+            #this is why we have to use the 1060 files instead 
+            #of the 1460 files
             self.get_legacy_data_1060(wave_range,deq=deq)
             self.get_new_wvno_grid_661()
             
             opa_filepath  = os.path.join(__refdata__, 'climate_INPUTS/661')
             self.load_kcoeff_arrays(opa_filepath)
             self.db_filename = cont_dir
             self.get_available_continuum()
             self.get_available_rayleigh()
             self.run_cia_spline_661()
         
         elif (deq == True) and (on_fly== True) :
-            self.get_gauss_pts_661_1460()
+            #self.get_gauss_pts_661_1460() repetetive code function
+            self.get_legacy_data_1460(wave_range)
             self.get_new_wvno_grid_661()
             
             opa_filepath  = os.path.join(__refdata__, 'climate_INPUTS/661')
             self.load_kcoeff_arrays_first(opa_filepath,gases_fly)
             self.db_filename = cont_dir
             self.get_available_continuum()
             self.get_available_rayleigh()
@@ -812,15 +817,15 @@
             abunds = abunds + last
             abunds = np.reshape(abunds,(self.max_pc,self.max_tc,max_ele),order='F')
             
             self.nwno = int(data.iloc[end_abunds,1])
             
             end_window = int(max_windows/3)
             self.wno = (data.iloc[end_abunds:end_abunds+end_window,0:3].astype(float)).values.ravel()[2:]
-            if np.float(data.iloc[end_abunds+end_window+1,2]) == 0.0: # for >+1.0 metallicity tables
+            if float(data.iloc[end_abunds+end_window+1,2]) == 0.0: # for >+1.0 metallicity tables
                 max_windows=1000
                 offset_new=267
                 self.delta_wno = (data.iloc[end_abunds+end_window+1+offset_new:1+end_abunds+2*end_window+offset_new,0:3].astype(float)).values.ravel()[:-2]
                 end_windows =1+end_abunds+2*end_window+2*(offset_new)
                 
                 nc_t=int(data.iloc[end_windows,1])
                 
@@ -952,15 +957,15 @@
 
             self.nwno = int(data.iloc[end_abunds,0])
             
 
             end_window = int(max_windows/3)
             
             self.wno = (data.iloc[end_abunds:end_abunds+end_window,0:3].astype(float)).values.ravel()[1:-1]
-            if np.float(data.iloc[end_abunds+end_window+1,2]) == 0.0: # for >+1.0 metallicity tables
+            if float(data.iloc[end_abunds+end_window+1,2]) == 0.0: # for >+1.0 metallicity tables
                 max_windows=1000
                 offset_new=266
                 self.delta_wno = (data.iloc[end_abunds+end_window+1+offset_new:1+end_abunds+2*end_window+offset_new,0:3].astype(float)).values.ravel()[2:]
                 end_windows =1+end_abunds+2*end_window+2*(offset_new+1)
                 
                 nc_t=int(data.iloc[end_windows,0])
                 
@@ -1070,16 +1075,16 @@
             
             #finally add pressure/temperature scale to abundances
                 self.full_abunds['pressure']= self.pressures[self.pressures>0]
                 self.full_abunds['temperature'] = np.concatenate([[i]*max(self.nc_p) for i in self.temps])[self.pressures>0]
  
 
 
-    def get_gauss_pts_661_1460(self):
-        """
+    def get_gauss_pts_661_1460_deprecate(self):
+        """NOT needed anymore, should be replaced with 1460 function
         Function to read the legacy data of the 1060 grid computed by Roxana Lupu. 
         Note
         ----
         This function is **highly** sensitive to the file format. You cannot edit the ascii file and then 
         run this function. Each specific line is accounted for.
         """
         data = pd.read_csv(os.path.join(self.ck_filename,'ascii_data'), 
@@ -1721,17 +1726,19 @@
             log_kappa_interpolated[i,:,:] = (1.-tt[i])*(1.-u[i])*kappa_lowp_lowt[i,:,:] + tt[i]*(1.-u[i])*kappa_lowp_hight[i,:,:] +tt[i]*u[i]*kappa_highp_hight[i,:,:]+ (1.-tt[i])*u[i]*kappa_highp_lowt[i,:,:]
         
         
         self.molecular_opa = np.exp(log_kappa_interpolated)*6.02214086e+23  #avogadro constant!
         #self.molecular_opa = np.exp(self.kappa[ind_p, ind_t, :, :])*6.02214086e+23  #avogadro constant!
         
     def load_kcoeff_arrays(self,path):
- # this loads and returns the kappa tables from Theodora's bin_mol files
- # will have this very hardcoded.
- # use this func only once before run begins
+        """
+        This loads and returns the kappa tables from Theodora's bin_mol files
+        will have this very hardcoded.
+        use this func only once before run begins
+        """
         max_wind = 670 # this can change as well but hopefully not
         n_windows = 661 # wait for 196 , then this is 196
         npres = 18 # max pres grid #
         ntemp = 60 # max temp grid #
 
         f = FortranFile( path+'/bin_CO', 'r' )
 
@@ -1769,37 +1776,15 @@
         dummy1= f.read_record(dtype='float32')
         dummy2 = f.read_reals( dtype='float32' )
         k_h2o = f.read_reals( dtype='float' )
         dummy3 = f.read_reals( dtype='float' )
         dummy4 = f.read_reals( dtype='int16' )
 
         kh2o = np.reshape(k_h2o,(ntemp,npres,16,max_wind))
-        '''
-        f = FortranFile( path+'/bin_CO2', 'r' )
-        dummy1= f.read_record(dtype='float32')
-        dummy2 = f.read_reals( dtype='float32' )
-        k_co2 = f.read_reals( dtype='float' )
-        dummy3 = f.read_reals( dtype='float' )
-        dummy4 = f.read_reals( dtype='int16' )
-        kco2 = np.reshape(k_co2,(ntemp,npres,16,max_wind))
-        f = FortranFile( path+'/bin_HCN', 'r' )
-        dummy1= f.read_record(dtype='float32')
-        dummy2 = f.read_reals( dtype='float32' )
-        k_hcn = f.read_reals( dtype='float' )
-        dummy3 = f.read_reals( dtype='float' )
-        dummy4 = f.read_reals( dtype='int16' )
-        khcn = np.reshape(k_hcn,(ntemp,npres,16,max_wind))
-        f = FortranFile( path+'/bin_N2', 'r' )
-        dummy1= f.read_record(dtype='float32')
-        dummy2 = f.read_reals( dtype='float32' )
-        k_n2 = f.read_reals( dtype='float' )
-        dummy3 = f.read_reals( dtype='float' )
-        dummy4 = f.read_reals( dtype='int16' )
-        kn2 = np.reshape(k_n2,(ntemp,npres,16,max_wind))
-        '''
+
         f = FortranFile( path+'/bin_deq_rst_4', 'r' )
 
         dummy1= f.read_record(dtype='float32')
         dummy2 = f.read_reals( dtype='float32' )
         k_back = f.read_reals( dtype='float' )
         dummy3 = f.read_reals( dtype='float' )
         dummy4 = f.read_reals( dtype='int16' )
@@ -1816,37 +1801,36 @@
         kch4 = kch4.swapaxes(2,3)
 
         knh3 = knh3.swapaxes(0,1)
         knh3 = knh3.swapaxes(2,3)
 
         kco = kco.swapaxes(0,1)
         kco = kco.swapaxes(2,3)
-        '''
-        kco2 = kco2.swapaxes(0,1)
-        kco2 = kco2.swapaxes(2,3)
-        kn2 = kn2.swapaxes(0,1)
-        kn2 = kn2.swapaxes(2,3)
-        khcn = khcn.swapaxes(0,1)
-        khcn = khcn.swapaxes(2,3)
-        '''
+
 
         self.kappa_back = kback[:,:,0:self.nwno,0:self.ngauss]
         self.kappa_h2o = kh2o[:,:,0:self.nwno,0:self.ngauss]
         self.kappa_co = kco[:,:,0:self.nwno,0:self.ngauss]
         self.kappa_nh3 = knh3[:,:,0:self.nwno,0:self.ngauss]
         self.kappa_ch4 = kch4[:,:,0:self.nwno,0:self.ngauss]
-        '''
-        self.kappa_co2 = kco2[:,:,0:self.nwno,0:self.ngauss]
-        self.kappa_n2 = kn2[:,:,0:self.nwno,0:self.ngauss]
-        self.kappa_hcn = khcn[:,:,0:self.nwno,0:self.ngauss]
-        '''
+
+
     def load_kcoeff_arrays_first(self,path,gases_fly):
- # this loads and returns the kappa tables from Theodora's bin_mol files
- # will have this very hardcoded.
- # use this func only once before run begins
+        """
+        This loads and returns the kappa tables from
+        opacity_factory.compute_ck_molecular()
+        Currently we have a single file for each molecule 
+
+        Parameters 
+        ----------
+        path : str 
+            Path to the individual ck files 
+        gases_fly : bool 
+            Specifies what gasses to mix on the fly 
+        """
         if 'H2O' in gases_fly:
             array = np.load(path+'/H2O_1460.npy')
             self.kappa_h2o = array
         else:
             array = np.load(path+'/H2O_1460.npy')
             self.kappa_h2o = array*0-250.0
         
@@ -1941,15 +1925,15 @@
             array = np.load(path+'/VO_1460.npy')
             self.kappa_vo = array*0-250.0
         
         if 'FeH' in gases_fly:
             array = np.load(path+'/FeH_1460.npy')
             self.kappa_feh = array
         else:
-            array = np.load(path+'/Feh_1460.npy')
+            array = np.load(path+'/FeH_1460.npy')
             self.kappa_feh = array*0-250.0
         
     def get_new_wvno_grid_661(self):
         path = os.path.join(__refdata__, 'climate_INPUTS/')#'/Users/sagnickmukherjee/Documents/GitHub/Disequilibrium-Picaso/reference/climate_INPUTS/'
         wvno_new,dwni_new = np.loadtxt(path+"wvno_661",usecols=[0,1],unpack=True)
         self.wno = wvno_new
         self.delta_wno = dwni_new
```

### Comparing `picaso-3.1/picaso/phasecurves.py` & `picaso-3.1.1/picaso/phasecurves.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/rayleigh.py` & `picaso-3.1.1/picaso/rayleigh.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/references.py` & `picaso-3.1.1/picaso/references.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/run_opa_factory.py` & `picaso-3.1.1/picaso/run_opa_factory.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/test.py` & `picaso-3.1.1/picaso/test.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/test_optics.py` & `picaso-3.1.1/picaso/test_optics.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/vulcan.py` & `picaso-3.1.1/picaso/vulcan.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso/wavelength.py` & `picaso-3.1.1/picaso/wavelength.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1/picaso.egg-info/PKG-INFO` & `picaso-3.1.1/picaso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picaso
-Version: 3.1
+Version: 3.1.1
 Summary: planetary intesity code for atmospheric scattering observations
 Home-page: https://natashabatalha.github.io/picaso
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
 Download-URL: https://github.com/natashabatalha/picaso
 Platform: UNKNOWN
```

### Comparing `picaso-3.1/picaso.egg-info/SOURCES.txt` & `picaso-3.1.1/picaso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picaso-3.1/setup.cfg` & `picaso-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `picaso-3.1/setup.py` & `picaso-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # from the setup.cfg file.
 #
 # use_2to3 and zip_safe are common options support by setuptools; these can
 # also be placed in the setup.cfg, as will be demonstrated in a future update
 # to this sample package.
 setup(
     name='picaso', 
-    version = '3.1',
+    version = '3.1.1',
     description = 'planetary intesity code for atmospheric scattering observations',
     long_description = 'README.md',
     author = 'Natasha E. Batalha',
     author_email = 'natasha.e.batalha@gmail.com',
     url = 'https://natashabatalha.github.io/picaso',
     license = 'GPL-3.0',
     download_url = 'https://github.com/natashabatalha/picaso',
@@ -70,11 +70,12 @@
           'astropy>=3.2.3',
           'matplotlib',
           'pysynphot',
           'sphinx',
           'scipy',
           'virga-exo',
           'xarray',
-          'bibtexparser'
+          'bibtexparser',
+          'dynesty'
           ], 
     zip_safe = False,
 )
```

