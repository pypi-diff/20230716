# Comparing `tmp/pymcabc-0.8.0.tar.gz` & `tmp/pymcabc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.8.0.tar", last modified: Thu Jul 13 05:10:39 2023, max compression
+gzip compressed data, was "pymcabc-0.9.0.tar", last modified: Sun Jul 16 12:28:14 2023, max compression
```

## Comparing `pymcabc-0.8.0.tar` & `pymcabc-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.023323 pymcabc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 05:10:27.000000 pymcabc-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 05:10:27.000000 pymcabc-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 05:10:39.019322 pymcabc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 05:10:27.000000 pymcabc-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:10:39.023323 pymcabc-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 05:10:27.000000 pymcabc-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_crosssection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_evengen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:28:14.162724 pymcabc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 12:28:03.000000 pymcabc-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-16 12:28:03.000000 pymcabc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-16 12:28:14.162724 pymcabc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-16 12:28:03.000000 pymcabc-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:28:14.158724 pymcabc-0.9.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-16 12:28:03.000000 pymcabc-0.9.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:28:14.158724 pymcabc-0.9.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-16 12:28:14.000000 pymcabc-0.9.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-16 12:28:14.000000 pymcabc-0.9.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:28:14.000000 pymcabc-0.9.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 12:28:14.000000 pymcabc-0.9.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 12:28:14.000000 pymcabc-0.9.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:28:14.162724 pymcabc-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-16 12:28:03.000000 pymcabc-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:28:14.162724 pymcabc-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 12:28:03.000000 pymcabc-0.9.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-16 12:28:03.000000 pymcabc-0.9.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-16 12:28:03.000000 pymcabc-0.9.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-16 12:28:03.000000 pymcabc-0.9.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-16 12:28:03.000000 pymcabc-0.9.0/tests/test_plot.py
```

### Comparing `pymcabc-0.8.0/LICENSE` & `pymcabc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/PKG-INFO` & `pymcabc-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.8.0
+Version: 0.9.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.8.0/README.md` & `pymcabc-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/cross_section.py` & `pymcabc-0.9.0/pymcabc/cross_section.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,22 +76,23 @@
         self.m2 = library["m2"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.process = library["process_type"][0]
         self.p_f = library["outgoing_p"][0]
         self.p_i = library["pi"][0]  
         self.channel = library["channel"][0]
+        self.seed = library["seed"][0]
         # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
         #self.E1 = library["E1"][0]
         #self.E2 = library["E2"][0]
         #self.E1 + self.E2
         #self.p1 = math.sqrt(self.E1**2 - self.m1**2) 
         #self.p2 = math.sqrt(self.E2**2 - self.m2**2) 
         #self.phase_factor = math.sqrt( (self.E1*self.E2 + self.p1*self.p2)**2 - (self.m1*self.m2)**2)
-        #self.p_f = pymcabc.constants.outgoing_p(self.Ecm, self.m3, self.m4)
+        #self.p_f = pymcabc.constants._lambda(self.Ecm, self.m3, self.m4)
 
     def dsigma_st(self, costh):
         if self.channel == "s":
             ME = MatrixElement().s_channel()
         elif self.channel == "t":
             ME = MatrixElement().t_channel(costh, self.p_f)
         else:
@@ -108,43 +109,52 @@
             ME = MatrixElement().u_channel(costh, self.p_f)
         else:
             ME = MatrixElement().t_channel(costh, self.p_f) + MatrixElement().u_channel(costh, self.p_f)
         ME = abs(ME)
         dsigma_tu = 0.5 / ((self.Ecm* 8 * math.pi) ** 2)
         dsigma_tu = dsigma_tu * abs(self.p_f / self.p_i) * ME**2
         return dsigma_tu
-
-    def xsection(self, w_max):
-        costh = -1 + random.random() * 2
+    
+    """
+    def xsection(self, costh, w_max):
         if self.process == "st":
             w_i = CrossSection().dsigma_st(costh) * 2 * 2 * math.pi  
         elif self.process == "tu":
             w_i = CrossSection().dsigma_tu(costh) * 2 * 2 * math.pi 
         if w_max < w_i:
             w_max = w_i
         return w_i, w_max
+    """
 
-    def integrate_xsec(self, N=40000):
+    def integrate_xsec(self, N=10000):
         w_sum = 0
         w_max = 0
         w_square = 0
+        random.seed(self.seed)
         for _i in range(N):
-            w_i, w_max = CrossSection().xsection(w_max)
+            costh = -1 + random.random() * 2
+            if self.process == "st":
+                w_i = CrossSection().dsigma_st(costh) * 2 * 2 * math.pi  
+            elif self.process == "tu":
+                w_i = CrossSection().dsigma_tu(costh) * 2 * 2 * math.pi 
+            if w_max < w_i:
+                w_max = w_i
+            #w_i, w_max = CrossSection().xsection(w_max, costh)
             w_sum += w_i
             w_square += w_i * w_i
         with open("library.json", "r") as f:
             library = json.load(f)
         library["w_max"].append(w_max)
         library["w_square"].append(w_square)
         library["w_sum"].append(w_sum)
         with open("library.json", "w") as f:
             json.dump(library, f)
         return None
 
-    def calc_xsection(self, N: int = 40000):
+    def calc_xsection(self, N: int=10000):
         self.integrate_xsec(N)
         with open("library.json", "r") as f:
             library = json.load(f)
         w_sum = library["w_sum"][0]
         w_square = library["w_square"][0]
         w_max = library["w_max"][0]
         sigma_x = w_sum * pymcabc.constants.convert/ (N * 1e12)  # result in barn unit
```

### Comparing `pymcabc-0.8.0/pymcabc/decay_particle.py` & `pymcabc-0.9.0/pymcabc/decay_particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/detector.py` & `pymcabc-0.9.0/pymcabc/detector.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/feynman_diagram.py` & `pymcabc-0.9.0/pymcabc/feynman_diagram.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/generate_event.py` & `pymcabc-0.9.0/pymcabc/generate_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,29 @@
             library = json.load(f)
         self.w_max = library["w_max"][0]
         self.Ecm = library["Ecm"][0] #+ library["E2"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.process = library["process_type"][0]
         self.out_p = library["outgoing_p"][0]
+        self.seed = library["seed"][0]
 
     def gen_events(self):
         i = 0
         prob = 0
         m_costh = np.zeros(self.Nevent)
         p1_px = np.zeros(self.Nevent)
         p1_py = np.zeros(self.Nevent)
         p1_pz = np.zeros(self.Nevent)
         p1_e = np.zeros(self.Nevent)
         p2_px = np.zeros(self.Nevent)
         p2_py = np.zeros(self.Nevent)
         p2_pz = np.zeros(self.Nevent)
         p2_e = np.zeros(self.Nevent)
+        random.seed(self.seed)
         while i < self.Nevent:
             costh = -1 + (random.random() * 2)
             phi = 2 * math.pi * random.random()  # * self.delta
             if self.process == "st":
                 w_ii = CrossSection().dsigma_st(costh) *  2 * 2 * math.pi 
             elif self.process == "tu":
                 w_ii = CrossSection().dsigma_tu(costh) *  2 * 2 * math.pi
```

### Comparing `pymcabc-0.8.0/pymcabc/identify_process.py` & `pymcabc-0.9.0/pymcabc/identify_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         "mB": [],
         "mC": [],
         "m1": [],
         "m2": [],
         "m3": [],
         "m4": [],
         "mx": [],
+        "_lambda": [],
         "outgoing_p": [],
         "bw": [],
         "massive": [],
         "massive_mass": [],
         "decay_process": [],
         "decay1_mass": [],
         "decay2_mass": [],
@@ -25,14 +26,15 @@
         "Ecm": [],
         "process": [],
         "process_type": [],
         "channel": [],
         "w_max": [],
         "w_sum": [],
         "w_square": [],
+        "seed":[],
     }
     jsonString = json.dumps(library, indent=2)
 
     with open("library.json", "w") as f:
         json.dump(library, f)
 
 
@@ -55,46 +57,51 @@
         mA: float,
         mB: float,
         mC: float,
         pi: float,
         #E1: float,
         #E2: float,
         channel: str = "none",
+        seed: float = 5,
     ):
 
         build_json()
         with open("library.json", "r") as f:
             self.library = json.load(f)
         self.input_string = input_string
         self.mA = mA
         self.mB = mB
         self.mC = mC
         self.p_i = pi
-        #self.E1 = E1
-        #self.E2 = E2
+        self.E1 = 0
+        self.E2 = 0
+        self.Ecm = 0
+        self._width = 0
         if self.mA < 0 or self.mB < 0 or self.mC < 0:
             raise Exception("Negative masses not accepted")
         #if self.E1 < 0:
         #    raise Exception("Negative Energy not accepted")
         if self.p_i <= 0:
             raise Exception("Negative or Zero absolute momentum not accepted")
         self.library["mA"].append(mA)
         self.library["mB"].append(mB)
         self.library["mC"].append(mC)
         self.library["pi"].append(pi)
+        self.library["seed"].append(seed)
         #self.library["E2"].append(self.E2)
         self.library["channel"].append(channel)
         self.process()
         self.channel()
         self.masses()
         self.identify_mediator()
         self.identify_decay()
         self._ECM()
         self.final_momenta()
-        self.bw()
+        self._lambda_store()
+        self._bw()
 
     def process(self):
         """identify the physics process"""
         self.library["process"].append(self.input_string)
         string = self.input_string.replace(" > ", " ")
         string = string.split(" ")
         initial_1 = string[0]
@@ -120,14 +127,20 @@
                 raise Exception(
                     "Channel "
                     + channel
                     + " not available for process type "
                     + process_type
                 )
         return None
+    
+    def final_momenta(self):
+        p_f = pymcabc.constants.outgoing_p(self.library["Ecm"][0], self.library["m3"][0], self.library["m4"][0])
+        self.library["outgoing_p"].append(p_f)
+        with open("library.json", "w") as f:
+            json.dump(self.library, f)
 
     def masses(self):
         """assign masses to m1, m2, m3, m4 and mediator"""
         string = self.input_string.replace(" > ", " ")
         string = string.split(" ")
         pmass = [0, 0, 0, 0]
         for i in range(4):
@@ -149,41 +162,31 @@
     
     def _ECM(self):
         #center of mass energy
         with open("library.json", "r") as f:
             library = json.load(f)
         m1 = library["m1"][0]
         m2 = library["m2"][0]
-        E1 = math.sqrt(m1**2 + self.p_i**2)
-        E2 = math.sqrt(m2**2 + self.p_i**2)
-        Ecm = E1 + E2
-        self.library["Ecm"].append(Ecm)
+        self.E1 = math.sqrt(m1**2 + self.p_i**2)
+        self.E2 = math.sqrt(m2**2 + self.p_i**2)
+        self.Ecm = self.E1 + self.E2
+        self.library["Ecm"].append(self.Ecm)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
-        return E1, E2, Ecm
     
     def ECM(self):
-        with open("library.json", "r") as f:
-            library = json.load(f)
-        m1 = library["m1"][0]
-        m2 = library["m2"][0]
-        E1 = math.sqrt(m1**2 + self.p_i**2)
-        E2 = math.sqrt(m2**2 + self.p_i**2)
-        Ecm = E1 + E2
         print(
               "\n",
-            "Energy Beam 1 : ", E1,
+            "Energy Beam 1 : ", self.E1,
               "\n",
-            "Energy Beam 2 : ", E2,
+            "Energy Beam 2 : ", self.E2,
               "\n",
-            "Energy CM : ", Ecm,
+            "Energy CM : ", self.Ecm,
               )
-        return E1, E2, Ecm
-
-
+        return self.E1, self.E2, self.Ecm
 
     def identify_mediator(self):
         """identify the mediator of the process"""
         process = self.library["process"][0]
         process = process.replace(" > ", " ")
         if (
             process == "A A B B"
@@ -211,29 +214,38 @@
             self.library["mediator"].append("A")
         else:
             return None
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
     
-    def final_momenta(self):
-        p_f = pymcabc.constants.outgoing_p(self.library["Ecm"][0], self.library["m3"][0], self.library["m4"][0])
-        self.library["outgoing_p"].append(p_f)
+    def _lambda_store(self):
+        if self.library["mx"][0] > 0:
+            p_f = pymcabc.constants.f_lambda(self.library["mA"][0], self.library["mB"][0], self.library["mC"][0], self.library["mx"][0])
+        else:
+            p_f = 0
+        self.library["_lambda"].append(p_f)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
+        return p_f
 
-    def bw(self):
-        if self.library["mx"][0] > 0:
-            deno  = 8*math.pi*(self.library["mx"][0])**2
-            _bw = (pymcabc.constants.g**2*self.library["outgoing_p"][0])/deno
-        else:
+    def _bw(self):
+        if self.library["mx"][0] == min(self.mA, self.mB, self.mC) or self.library["mx"][0]==0:
             _bw = 0.0
+        else:
+            deno  = 8*math.pi*(self.library["mx"][0])**2
+            _bw = (pymcabc.constants.g**2*self.library["_lambda"][0])/deno
         self.library["bw"].append(_bw)
+        self._width = _bw 
         with open("library.json", "w") as f:
             json.dump(self.library, f)
+        return _bw
+
+    def width(self):
+        return self._width
 
     def identify_decay(self):
         """identify the decay chain associated with the process"""
         mA = self.library["mA"][0]
         mB = self.library["mB"][0]
         mC = self.library["mC"][0]
         if mA > mB + mC:
```

### Comparing `pymcabc-0.8.0/pymcabc/particle.py` & `pymcabc-0.9.0/pymcabc/particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/plotting.py` & `pymcabc-0.9.0/pymcabc/plotting.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/pymcabc/save_events.py` & `pymcabc-0.9.0/pymcabc/save_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # import pandas as pd
 import uproot
+import os
 import json
 import numpy as np
 from pymcabc.generate_event import GENEvents
 from pymcabc.particle import Particle
 from pymcabc.decay_particle import DecayParticle
 from pymcabc.detector import Detector
 
@@ -77,14 +78,19 @@
 
     def to_root(self, name: str = "ABC_events.root"):
         """function to save event as ROOT file
         Parameters:
             name (str): name of root file
 
         """
+
+        check_extension = os.path.splitext(name)
+        if check_extension[1] != ".root":
+            raise ValueError("Output supported with .root extension only") 
+
         if self.boolTruth == True:
             file = uproot.recreate("truth_" + name)
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
```

### Comparing `pymcabc-0.8.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.9.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.8.0
+Version: 0.9.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.8.0/pymcabc.egg-info/SOURCES.txt` & `pymcabc-0.9.0/pymcabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/setup.py` & `pymcabc-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="pymcabc",
-    version="0.8.0",
+    version="0.9.0",
     description="Monte Carlo Event Generator for the ABC theory",
     author="Aman Desai",
     author_email="amanmukeshdesai@gmail.com",
     maintainer="Aman Desai",
     maintainer_email="amanmukeshdesai@gmail.com",
     url="https://github.com/amanmdesai/pymcabc",
     long_description=long_description,
```

### Comparing `pymcabc-0.8.0/tests/test_crosssection.py` & `pymcabc-0.9.0/tests/test_crosssection.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/tests/test_evengen.py` & `pymcabc-0.9.0/tests/test_evengen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pymcabc
 import os
+import pytest
 
 
 # test if the file is prepared
 def test_eventGen_detector_decay():
     pymcabc.DefineProcess("A A > B B", mA=4, mB=10, mC=1, pi=30)
     pymcabc.CrossSection().calc_xsection()
     pymcabc.SaveEvent(100, boolDecay=True, boolDetector=True).to_root(
@@ -15,29 +16,35 @@
 
 def test_eventGen_decay():
     pymcabc.DefineProcess("A A > B B", mA=4, mB=10, mC=1, pi=30)
     pymcabc.CrossSection().calc_xsection()
     pymcabc.SaveEvent(100, boolDecay=True, boolDetector=False).to_root(
         "test_eventGen_decay.root"
     )
-    # pymcabc.PlotData.file('test_eventGen_decay.root')
     assert "test_eventGen_decay.root" in os.listdir(), "file not created"
 
 
 def test_eventGen_detector():
     pymcabc.DefineProcess("A A > B B", mA=4, mB=10, mC=1, pi=30)
     pymcabc.CrossSection().calc_xsection()
     pymcabc.SaveEvent(100, boolDecay=False, boolDetector=True).to_root(
         "test_eventGen_detector.root"
     )
-    # pymcabc.PlotData.file('test_eventGen_detector.root')
     assert "test_eventGen_detector.root" in os.listdir(), "file not created"
 
 
 def test_eventGen():
     pymcabc.DefineProcess("A A > B B", mA=4, mB=10, mC=1, pi=30)
     pymcabc.CrossSection().calc_xsection()
     pymcabc.SaveEvent(100, boolDecay=False, boolDetector=False).to_root(
         "test_eventGen.root"
     )
-    # pymcabc.PlotData.file('test_eventGen.root')
     assert "test_eventGen.root" in os.listdir(), "file not created"
+
+
+def test_csv_output_reject():
+    pymcabc.DefineProcess("A A > B B", mA=4, mB=10, mC=1, pi=30)
+    pymcabc.CrossSection().calc_xsection()
+    with pytest.raises(
+        Exception, match="Output supported with .root extension only"):
+        pymcabc.SaveEvent(100, boolDecay=False, boolDetector=False).to_root("test_eventGen.csv")
+
```

### Comparing `pymcabc-0.8.0/tests/test_identify.py` & `pymcabc-0.9.0/tests/test_identify.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.8.0/tests/test_plot.py` & `pymcabc-0.9.0/tests/test_plot.py`

 * *Files identical despite different names*

