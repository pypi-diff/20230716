# Comparing `tmp/j2config-0.0.5.tar.gz` & `tmp/j2config-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "j2config-0.0.5.tar", last modified: Thu Mar 23 06:30:04 2023, max compression
+gzip compressed data, was "j2config-0.0.6.tar", last modified: Sun Jul 16 04:52:06 2023, max compression
```

## Comparing `j2config-0.0.5.tar` & `j2config-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 06:30:04.911743 j2config-0.0.5/
--rw-rw-rw-   0        0        0     1091 2022-07-10 12:41:56.000000 j2config-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      544 2023-03-23 06:30:04.910747 j2config-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-01-27 13:07:32.000000 j2config-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 06:30:04.854692 j2config-0.0.5/j2config/
--rw-rw-rw-   0        0        0      365 2023-03-23 06:28:12.000000 j2config-0.0.5/j2config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:30:04.906414 j2config-0.0.5/j2config/cmn/
--rw-rw-rw-   0        0        0        0 2023-03-22 08:13:35.000000 j2config-0.0.5/j2config/cmn/__init__.py
--rw-rw-rw-   0        0        0     3989 2023-02-25 08:17:25.000000 j2config-0.0.5/j2config/cmn/common_fn.py
--rw-rw-rw-   0        0        0     4457 2023-02-25 08:07:49.000000 j2config-0.0.5/j2config/data_collect.py
--rw-rw-rw-   0        0        0     8669 2023-03-23 06:27:18.000000 j2config-0.0.5/j2config/func.py
--rw-rw-rw-   0        0        0      489 2023-02-25 08:05:30.000000 j2config-0.0.5/j2config/general.py
--rw-rw-rw-   0        0        0     3423 2023-02-25 08:13:26.000000 j2config-0.0.5/j2config/j2.py
--rw-rw-rw-   0        0        0     1331 2023-02-25 08:13:43.000000 j2config-0.0.5/j2config/read_conditions.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:30:04.878482 j2config-0.0.5/j2config.egg-info/
--rw-rw-rw-   0        0        0      544 2023-03-23 06:30:04.000000 j2config-0.0.5/j2config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-03-23 06:30:04.000000 j2config-0.0.5/j2config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 06:30:04.000000 j2config-0.0.5/j2config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-23 06:30:04.000000 j2config-0.0.5/j2config.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-23 06:30:04.000000 j2config-0.0.5/j2config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 06:30:04.911743 j2config-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-03-23 06:27:55.000000 j2config-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:52:06.762962 j2config-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2022-07-10 12:41:56.000000 j2config-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-07-16 04:52:06.761965 j2config-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2023-01-27 13:07:32.000000 j2config-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 04:52:06.726062 j2config-0.0.6/j2config/
+-rw-rw-rw-   0        0        0      417 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:52:06.760000 j2config-0.0.6/j2config/cmn/
+-rw-rw-rw-   0        0        0        0 2023-03-22 08:13:35.000000 j2config-0.0.6/j2config/cmn/__init__.py
+-rw-rw-rw-   0        0        0     6045 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/cmn/common_fn.py
+-rw-rw-rw-   0        0        0     5085 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/data_collect.py
+-rw-rw-rw-   0        0        0     9398 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/func.py
+-rw-rw-rw-   0        0        0      617 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/general.py
+-rw-rw-rw-   0        0        0     4020 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/j2.py
+-rw-rw-rw-   0        0        0     1502 2023-07-16 03:38:37.000000 j2config-0.0.6/j2config/read_conditions.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:52:06.748034 j2config-0.0.6/j2config.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-07-16 04:52:06.000000 j2config-0.0.6/j2config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-07-16 04:52:06.000000 j2config-0.0.6/j2config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 04:52:06.000000 j2config-0.0.6/j2config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 04:52:06.000000 j2config-0.0.6/j2config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 04:52:06.000000 j2config-0.0.6/j2config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 04:52:06.762962 j2config-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-07-16 03:38:37.000000 j2config-0.0.6/setup.py
```

### Comparing `j2config-0.0.5/LICENSE` & `j2config-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `j2config-0.0.5/PKG-INFO` & `j2config-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2config
-Version: 0.0.5
+Version: 0.0.6
 Summary: configuration generation using jinja2 - for Networking Geeks
 Home-page: https://github.com/aliasgar1978/j2config
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `j2config-0.0.5/j2config/func.py` & `j2config-0.0.6/j2config/func.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 
 
 
 
 class Vrf():
 	"""device vrf/instances
 
+	Args:
+		table (dict): dataframe dictionary
+
 	Returns:
 		Vrf: Instance of VRF
 
 	Yields:
 		Vrf: Instance of VRF
 	"""	
 
 	def __init__(self, table):
+		
 		self.table = table
 
 	def __iter__(self):
 		for key, data in self.table.items():
 			if self.is_vrf(data): yield data
 
 	@staticmethod
@@ -105,14 +109,23 @@
 				yield data
 
 
 
 
 class Vlan():
 	"""device Vlan/instances
+
+	Args:
+		table (dict): dataframe dictionary
+
+	Returns:
+		Vlan: Instance of Vlan
+
+	Yields:
+		Vlan: Instance of Vlan
 	"""	
 	def __init__(self, table):
 		self.table = table
 
 	def __iter__(self):
 		for key, data in self.table.items():
 			if self.is_vlan(data): yield data
@@ -181,14 +194,23 @@
 		"""		
 		for data in self:
 			if data and data['intvrf'] == vrf: yield data
 
 
 class Bgp():
 	"""device Bgp/instances
+
+	Args:
+		table (dict): dataframe dictionary
+
+	Returns:
+		Bgp: Instance of Bgp
+
+	Yields:
+		Bgp: Instance of Bgp
 	"""	
 
 	def __init__(self, table):
 		self.table = table
 
 	def __iter__(self):
 		for key, data in self.table.items():
@@ -228,14 +250,23 @@
 		for data in self:
 			if data['bgp_vrf'] == vrf:
 				yield data
 
 
 class Physical():
 	"""device Physical/instances
+
+	Args:
+		table (dict): dataframe dictionary
+
+	Returns:
+		Physical: Instance of Physical
+
+	Yields:
+		Physical: Instance of Physical
 	"""	
 	def __init__(self, table):
 		self.table = table
 
 	@staticmethod
 	def is_physical(data):
 		"""Condition: Checks if provided data is Physical Interface data
@@ -322,14 +353,23 @@
 			bool: result of condition
 		"""		
 		return data['int_filter'].lower().endswith(x)
 
 
 class Aggregated():
 	"""device Aggregated/instances
+
+	Args:
+		table (dict): dataframe dictionary
+
+	Returns:
+		Aggregated: Instance of Aggregated
+
+	Yields:
+		Aggregated: Instance of Aggregated
 	"""	
 	def __init__(self, table):
 		self.table = table
 
 	def __iter__(self):
 		for key, data in self.table.items():
 			if self.is_aggregated(data): yield data
@@ -345,14 +385,23 @@
 			bool: result of condition
 		"""			
 		return data['filter'].lower() == 'aggregated'
 
 
 class Loopback():
 	"""device Loopback/instances
+
+	Args:
+		table (dict): dataframe dictionary
+
+	Returns:
+		Loopback: Instance of Loopback
+
+	Yields:
+		Loopback: Instance of Loopback
 	"""	
 	def __init__(self, table):
 		self.table = table
 
 	def __iter__(self):
 		for key, data in self.table.items():
 			if self.is_loopback(data): yield data
```

### Comparing `j2config-0.0.5/j2config/j2.py` & `j2config-0.0.6/j2config/j2.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,26 @@
 from . import func as func
 from .func import Vrf, Vlan, Physical, Bgp, Aggregated, Loopback
 from .general import *
 
 
 class PrepareConfig():
 	"""boiler plate code class for start configuration preparation
-	"""
+
+	Args:
+		data_file (str): Excel database
+		jtemplate_file (str): Jinja Template
+		output_folder (str, optional): output path. Defaults to ".".
+		regional_file (str, optional): custom static regional variable file. Defaults to None. (overrides device var)
+		regional_class (class, optional): custom class returning frames to be merge with device var . Defaults to None.
+
+	Raises:
+		Exception: Raise for Custom class insertion
+		Exception: Raise for Custom module insertion
+	"""	
 
 	# -----------------------------------------
 	# IMPORT FILTERS FOR JINJA VARIABLES
 	# -----------------------------------------
 	filters = {}
 	filters.update({'Vrf': Vrf, 'Bgp': Bgp,
 		'Vlan': Vlan, 'Physical': Physical, 'Aggregated': Aggregated, 'Loopback': Loopback, 		
@@ -28,51 +39,59 @@
 	filters.update(dict(getmembers(Loopback, lambda x:not(isroutine(x))))['__dict__'] )
 	filters.update(dict(getmembers(func, isfunction)))
 
 	def __init__(self,
 		data_file,
 		jtemplate_file,
 		output_folder=".",
-		global_variables_file=None,	
+		regional_file=None,
+		regional_class=None,
 		):
+		"""Object Initializer
+		"""		
 		self.data_file = data_file
 		self.jtemplate_file = jtemplate_file.replace("\\", '/')
 		self.output_folder = output_folder
-		self.global_variables_file = global_variables_file
+		self.regional_file = regional_file
+		self.regional_class = regional_class
 
 	def custom_class_add_to_filter(self, **kwargs):
 		"""add custom classes and its methods as jinja filters. External callable.
 		"""
 		for filtername, _cls in kwargs.items():
 			try:
-				# if not self.filters.get(filtername):
 				self.filters.update({filtername: _cls})
 				pre = self.filters.keys()
 				self.filters.update(dict(getmembers(_cls, lambda x:not(isroutine(x))))['__dict__'] )
 				post = self.filters.keys()
-				# print(pre==post)
-				# print(getmembers(_cls, lambda x:not(isroutine(x))))
 			except Exception as e:
 				raise Exception(f"Class Insertion Failed for filter {filtername}\n{e}")
 
 	def custom_module_methods_add_to_filter(self, *modules):
 		"""add custom methods from module(s) as jinja filters. External callable.
 		"""
 		for module in modules:
 			try:
 				self.filters.update(dict(getmembers(module, isfunction)))
 			except Exception as e:
 				raise Exception(f"Module Insertion Failed {module}\n{e}")
 
-
 	def start(self):
-		"""kicks generation
+		"""kick start generation
 		"""
 		# ## LOAD - DATA
-		DD = DeviceDetails(self.global_variables_file, self.data_file)
+		DD = DeviceDetails(self.data_file)
+		frames = []
+		try:
+			RCD = self.regional_class(DD.device_details, self.regional_file)
+			frames = RCD.frames
+		except:
+			pass
+		DD.merge_with_var_frames(frames)
+		DD.read_table()
 
 		# ## LOAD - JINJA TEMPLATE AND ENVIRONMENT
 		templateLoader = jinja2.FileSystemLoader(searchpath='')
 		templateEnv = jinja2.Environment(loader=templateLoader, 
 			extensions=['jinja2.ext.loopcontrols', 'jinja2.ext.do',])
 		for key, value in self.filters.items():
 			templateEnv.filters[key] = value
```

### Comparing `j2config-0.0.5/j2config/read_conditions.py` & `j2config-0.0.6/j2config/read_conditions.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,42 @@
 import nettoolkit as nt
 
 
 
 
 def get_conditions(jinja_flie):
 	"""get all conditional statements from jinja file
-	--> dict
-	"""
+
+	Args:
+		jinja_flie (str): jinja template file
+
+	Returns:
+		dict: dictionary with list of jinja variables, conditions, and loops.
+	"""	
 	d = {'conditions':set(), 'loops':set(), 'variables': set() }
 	with open(jinja_flie, 'r') as f:
 		lns = f.readlines()
 	for ln in lns:
 		if ln.strip().startswith("{% for "):
 			d['loops'].add(ln)
 		elif ln.strip().startswith("{% if") or ln.strip().startswith("{% elif"):
 			d['conditions'].add(ln)
 		elif ln.strip().startswith("{% set "):
 			d['variables'].add(ln)
 	return d
 
 def get_variables(jinja_flie):
 	"""get all jinja variables defined in jinja file
-	--> set
-	"""
+
+	Args:
+		jinja_flie (str): jinja template file
+
+	Returns:
+		set: set of jinja variables
+	"""	
 	conds = set()
 	with open(jinja_flie, 'r') as f:
 		lns = f.readlines()
 	for ln in lns:
 		starts, ends = [], []
 		for i in range(20):
 			if i == 0: s,e = 0,0
@@ -39,13 +49,11 @@
 			ends.append(end)
 			s = start+2
 			e = end+2
 
 		if starts == []: continue
 		for s, e in zip(starts, ends):
 			cond = ln[s:e+2]
-			# print(cond, end='\t' )
 			conds.add(cond)
-		# print()
 	return conds
 
 # # -----------------------------------------------------------------------------------------
```

### Comparing `j2config-0.0.5/j2config.egg-info/PKG-INFO` & `j2config-0.0.6/j2config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2config
-Version: 0.0.5
+Version: 0.0.6
 Summary: configuration generation using jinja2 - for Networking Geeks
 Home-page: https://github.com/aliasgar1978/j2config
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `j2config-0.0.5/setup.py` & `j2config-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="j2config",
-    version="0.0.5",
+    version="0.0.6",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="configuration generation using jinja2 - for Networking Geeks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aliasgar1978/j2config",
     # package_data={
```

