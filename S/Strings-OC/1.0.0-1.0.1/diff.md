# Comparing `tmp/Strings-OC-1.0.0.tar.gz` & `tmp/Strings-OC-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Strings-OC-1.0.0.tar", last modified: Sat Jun 24 19:32:27 2023, max compression
+gzip compressed data, was "Strings-OC-1.0.1.tar", last modified: Sun Jul 16 11:52:41 2023, max compression
```

## Comparing `Strings-OC-1.0.0.tar` & `Strings-OC-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-24 19:32:27.376234 Strings-OC-1.0.0/
--rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-03-17 16:32:23.000000 Strings-OC-1.0.0/LICENSE
--rw-rw-r--   0 bast      (1000) bast      (1000)     5978 2023-06-24 19:32:27.376234 Strings-OC-1.0.0/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)     5335 2023-06-24 19:29:50.000000 Strings-OC-1.0.0/README.md
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-24 19:32:27.376234 Strings-OC-1.0.0/Strings_OC.egg-info/
--rw-rw-r--   0 bast      (1000) bast      (1000)     5978 2023-06-24 19:32:27.000000 Strings-OC-1.0.0/Strings_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)      241 2023-06-24 19:32:27.000000 Strings-OC-1.0.0/Strings_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-06-24 19:32:27.000000 Strings-OC-1.0.0/Strings_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        8 2023-06-24 19:32:27.000000 Strings-OC-1.0.0/Strings_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-03-17 17:15:13.000000 Strings-OC-1.0.0/Strings_OC.egg-info/zip-safe
--rw-rw-r--   0 bast      (1000) bast      (1000)       79 2023-06-24 19:32:27.380234 Strings-OC-1.0.0/setup.cfg
--rw-rw-r--   0 bast      (1000) bast      (1000)      796 2023-06-24 19:31:09.000000 Strings-OC-1.0.0/setup.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-24 19:32:27.376234 Strings-OC-1.0.0/strings/
--rw-rw-r--   0 bast      (1000) bast      (1000)    17099 2023-06-24 17:29:49.000000 Strings-OC-1.0.0/strings/__init__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)       48 2023-03-19 23:23:18.000000 Strings-OC-1.0.0/strings/__main__.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-07-16 11:52:41.933702 Strings-OC-1.0.1/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-03-17 16:32:23.000000 Strings-OC-1.0.1/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)     6990 2023-07-16 11:52:41.933702 Strings-OC-1.0.1/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)     6347 2023-07-16 11:52:07.000000 Strings-OC-1.0.1/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-07-16 11:52:41.933702 Strings-OC-1.0.1/Strings_OC.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     6990 2023-07-16 11:52:41.000000 Strings-OC-1.0.1/Strings_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      241 2023-07-16 11:52:41.000000 Strings-OC-1.0.1/Strings_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-07-16 11:52:41.000000 Strings-OC-1.0.1/Strings_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        8 2023-07-16 11:52:41.000000 Strings-OC-1.0.1/Strings_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-03-17 17:15:13.000000 Strings-OC-1.0.1/Strings_OC.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2023-07-16 11:52:41.933702 Strings-OC-1.0.1/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)      796 2023-07-12 14:20:06.000000 Strings-OC-1.0.1/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-07-16 11:52:41.933702 Strings-OC-1.0.1/strings/
+-rw-rw-r--   0 bast      (1000) bast      (1000)    19062 2023-07-16 11:32:31.000000 Strings-OC-1.0.1/strings/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)       48 2023-06-24 19:32:49.000000 Strings-OC-1.0.1/strings/__main__.py
```

### Comparing `Strings-OC-1.0.0/LICENSE` & `Strings-OC-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Strings-OC-1.0.0/PKG-INFO` & `Strings-OC-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: Strings-OC
-Version: 1.0.0
-Summary: Generic functions for dealing with and generating strings
-Home-page: https://ouroboroscoding.com/strings/
-Author: Chris Nasr - Ouroboros Coding Inc.
-Author-email: chris@ouroboroscoding.com
-License: MIT
-Project-URL: Documentation, https://ouroboroscoding.com/strings/
-Project-URL: Source, https://github.com/ouroboroscoding/strings-python
-Project-URL: Tracker, https://github.com/ouroboroscoding/strings-python/issues
-Keywords: strings,string manipulation,string generation
-Platform: UNKNOWN
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Ouroboros Coding Strings
+# Strings by Ouroboros Coding
 [![pypi version](https://img.shields.io/pypi/v/Strings-OC.svg)](https://pypi.org/project/Strings-OC) ![MIT License](https://img.shields.io/pypi/l/Strings-OC.svg)
 
 Generic functions for dealing with and generating strings
 
 ## Requires
-Config-OC requires python 3.10 or higher
+Strings-OC requires python 3.10 or higher
 
 ## Installation
 ```bash
 pip install Strings-OC
 ```
 
 ## Functions
@@ -52,14 +35,38 @@
 '1234'
 >>> digits('3.1415')
 '31415'
 >>> digits('1e+7')
 '17'
 ```
 
+### from_file
+Returns the entire file as a string
+
+```python
+>>> from strings import from_file
+>>> from_file('version.dat')
+'1.0.1\n'
+```
+
+Assuming `version.dat` contained the following
+
+```
+1.0.1
+
+```
+
+If the file doesn't exist, `from_file` returns `None`. This can be changed by passing a second argument to be the default value.
+
+```python
+>>> from strings import from_file
+>>> from_file('doesnotexist', '1.0.0')
+'1.0.0'
+```
+
 ### normalize
 Returns, as well as possible, a normalized string converted from another string containing characters with special accents. It does this by finding special characters and converting them into their simpler, single character, versions. This is useful for things like automaticlaly generating urls, or for generating from unicode into ascii.
 ```python
 >>> from strings import normalize
 >>> normalize('Ȟěƚľỡ, Ẉợɽḷᶁ!')
 'Hello, World!'
 >>> normalize('ﬃǲǼĳ')
@@ -151,14 +158,26 @@
 True
 >>> to_bool('F')
 False
 >>> to_bool('2')
 ValueError: "2" is not a valid boolean representation in to_bool
 ```
 
+### to_file
+Stores a string in a file, overwriting the existing contents, or creating the file if it didn't exist.
+```python
+>>> from strings import to_file
+>>> to_file('version.dat', '1.1.0')
+True
+```
+The `version.dat` file will now contain the following
+```
+1.1.0
+```
+
 ### uuid_add_dashes
 Used to add dashes "-" to a string representation of a UUID that has none.
 ```python
 >>> from strings import uuid_add_dashes
 >>> uuid_add_dashes('b22eb45ac98311eca05a80fa5b0d7c77')
 'b22eb45a-c983-11ec-a05a-80fa5b0d7c77'
 ```
@@ -167,7 +186,18 @@
 Used to strip dashes "-" from a string representation of a UUID that has them.
 ```python
 >>> from strings import uuid_strip_dashes
 >>> uuid_strip_dashes('b22eb45a-c983-11ec-a05a-80fa5b0d7c77')
 'b22eb45ac98311eca05a80fa5b0d7c77'
 ```
 
+### version_compare
+Compares to version strings and returns if the first is less than (-1), equal to (0) or greater than (1) the second
+```python
+>>> from strings import version_compare
+>>> version_compare('1.0.1', '1.0')
+1
+>>> version_compare('1.0.1', '1.0.1')
+0
+>>> version_compare('1.0.1', '1.1')
+-1
+```
```

### Comparing `Strings-OC-1.0.0/README.md` & `Strings-OC-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,31 @@
-# Ouroboros Coding Strings
+Metadata-Version: 2.1
+Name: Strings-OC
+Version: 1.0.1
+Summary: Generic functions for dealing with and generating strings
+Home-page: https://ouroboroscoding.com/strings/
+Author: Chris Nasr - Ouroboros Coding Inc.
+Author-email: chris@ouroboroscoding.com
+License: MIT
+Project-URL: Documentation, https://ouroboroscoding.com/strings/
+Project-URL: Source, https://github.com/ouroboroscoding/strings-python
+Project-URL: Tracker, https://github.com/ouroboroscoding/strings-python/issues
+Keywords: strings,string manipulation,string generation
+Platform: UNKNOWN
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Strings by Ouroboros Coding
 [![pypi version](https://img.shields.io/pypi/v/Strings-OC.svg)](https://pypi.org/project/Strings-OC) ![MIT License](https://img.shields.io/pypi/l/Strings-OC.svg)
 
 Generic functions for dealing with and generating strings
 
 ## Requires
-Config-OC requires python 3.10 or higher
+Strings-OC requires python 3.10 or higher
 
 ## Installation
 ```bash
 pip install Strings-OC
 ```
 
 ## Functions
@@ -35,14 +52,38 @@
 '1234'
 >>> digits('3.1415')
 '31415'
 >>> digits('1e+7')
 '17'
 ```
 
+### from_file
+Returns the entire file as a string
+
+```python
+>>> from strings import from_file
+>>> from_file('version.dat')
+'1.0.1\n'
+```
+
+Assuming `version.dat` contained the following
+
+```
+1.0.1
+
+```
+
+If the file doesn't exist, `from_file` returns `None`. This can be changed by passing a second argument to be the default value.
+
+```python
+>>> from strings import from_file
+>>> from_file('doesnotexist', '1.0.0')
+'1.0.0'
+```
+
 ### normalize
 Returns, as well as possible, a normalized string converted from another string containing characters with special accents. It does this by finding special characters and converting them into their simpler, single character, versions. This is useful for things like automaticlaly generating urls, or for generating from unicode into ascii.
 ```python
 >>> from strings import normalize
 >>> normalize('Ȟěƚľỡ, Ẉợɽḷᶁ!')
 'Hello, World!'
 >>> normalize('ﬃǲǼĳ')
@@ -134,22 +175,47 @@
 True
 >>> to_bool('F')
 False
 >>> to_bool('2')
 ValueError: "2" is not a valid boolean representation in to_bool
 ```
 
+### to_file
+Stores a string in a file, overwriting the existing contents, or creating the file if it didn't exist.
+```python
+>>> from strings import to_file
+>>> to_file('version.dat', '1.1.0')
+True
+```
+The `version.dat` file will now contain the following
+```
+1.1.0
+```
+
 ### uuid_add_dashes
 Used to add dashes "-" to a string representation of a UUID that has none.
 ```python
 >>> from strings import uuid_add_dashes
 >>> uuid_add_dashes('b22eb45ac98311eca05a80fa5b0d7c77')
 'b22eb45a-c983-11ec-a05a-80fa5b0d7c77'
 ```
 
 ### uuid_strip_dashes
 Used to strip dashes "-" from a string representation of a UUID that has them.
 ```python
 >>> from strings import uuid_strip_dashes
 >>> uuid_strip_dashes('b22eb45a-c983-11ec-a05a-80fa5b0d7c77')
 'b22eb45ac98311eca05a80fa5b0d7c77'
-```
+```
+
+### version_compare
+Compares to version strings and returns if the first is less than (-1), equal to (0) or greater than (1) the second
+```python
+>>> from strings import version_compare
+>>> version_compare('1.0.1', '1.0')
+1
+>>> version_compare('1.0.1', '1.0.1')
+0
+>>> version_compare('1.0.1', '1.1')
+-1
+```
+
```

### Comparing `Strings-OC-1.0.0/Strings_OC.egg-info/PKG-INFO` & `Strings-OC-1.0.1/Strings_OC.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: Strings-OC
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generic functions for dealing with and generating strings
 Home-page: https://ouroboroscoding.com/strings/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/strings/
 Project-URL: Source, https://github.com/ouroboroscoding/strings-python
 Project-URL: Tracker, https://github.com/ouroboroscoding/strings-python/issues
 Keywords: strings,string manipulation,string generation
 Platform: UNKNOWN
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ouroboros Coding Strings
+# Strings by Ouroboros Coding
 [![pypi version](https://img.shields.io/pypi/v/Strings-OC.svg)](https://pypi.org/project/Strings-OC) ![MIT License](https://img.shields.io/pypi/l/Strings-OC.svg)
 
 Generic functions for dealing with and generating strings
 
 ## Requires
-Config-OC requires python 3.10 or higher
+Strings-OC requires python 3.10 or higher
 
 ## Installation
 ```bash
 pip install Strings-OC
 ```
 
 ## Functions
@@ -52,14 +52,38 @@
 '1234'
 >>> digits('3.1415')
 '31415'
 >>> digits('1e+7')
 '17'
 ```
 
+### from_file
+Returns the entire file as a string
+
+```python
+>>> from strings import from_file
+>>> from_file('version.dat')
+'1.0.1\n'
+```
+
+Assuming `version.dat` contained the following
+
+```
+1.0.1
+
+```
+
+If the file doesn't exist, `from_file` returns `None`. This can be changed by passing a second argument to be the default value.
+
+```python
+>>> from strings import from_file
+>>> from_file('doesnotexist', '1.0.0')
+'1.0.0'
+```
+
 ### normalize
 Returns, as well as possible, a normalized string converted from another string containing characters with special accents. It does this by finding special characters and converting them into their simpler, single character, versions. This is useful for things like automaticlaly generating urls, or for generating from unicode into ascii.
 ```python
 >>> from strings import normalize
 >>> normalize('Ȟěƚľỡ, Ẉợɽḷᶁ!')
 'Hello, World!'
 >>> normalize('ﬃǲǼĳ')
@@ -151,14 +175,26 @@
 True
 >>> to_bool('F')
 False
 >>> to_bool('2')
 ValueError: "2" is not a valid boolean representation in to_bool
 ```
 
+### to_file
+Stores a string in a file, overwriting the existing contents, or creating the file if it didn't exist.
+```python
+>>> from strings import to_file
+>>> to_file('version.dat', '1.1.0')
+True
+```
+The `version.dat` file will now contain the following
+```
+1.1.0
+```
+
 ### uuid_add_dashes
 Used to add dashes "-" to a string representation of a UUID that has none.
 ```python
 >>> from strings import uuid_add_dashes
 >>> uuid_add_dashes('b22eb45ac98311eca05a80fa5b0d7c77')
 'b22eb45a-c983-11ec-a05a-80fa5b0d7c77'
 ```
@@ -167,7 +203,19 @@
 Used to strip dashes "-" from a string representation of a UUID that has them.
 ```python
 >>> from strings import uuid_strip_dashes
 >>> uuid_strip_dashes('b22eb45a-c983-11ec-a05a-80fa5b0d7c77')
 'b22eb45ac98311eca05a80fa5b0d7c77'
 ```
 
+### version_compare
+Compares to version strings and returns if the first is less than (-1), equal to (0) or greater than (1) the second
+```python
+>>> from strings import version_compare
+>>> version_compare('1.0.1', '1.0')
+1
+>>> version_compare('1.0.1', '1.0.1')
+0
+>>> version_compare('1.0.1', '1.1')
+-1
+```
+
```

### Comparing `Strings-OC-1.0.0/setup.py` & `Strings-OC-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Strings-OC',
-	version='1.0.0',
+	version='1.0.1',
 	description='Generic functions for dealing with and generating strings',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/strings/',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/strings/',
 		'Source': 'https://github.com/ouroboroscoding/strings-python',
```

### Comparing `Strings-OC-1.0.0/strings/__init__.py` & `Strings-OC-1.0.1/strings/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 __author__		= "Chris Nasr"
 __copyright__	= "Ouroboros Coding Inc."
 __email__		= "chris@ouroboroscoding.com"
 __created__		= "2018-11-11"
 
 # Limit exports
 __all__ = [
-	'bytes_human', 'digits', 'normalize', 'random', 'strtr', 'to_bool',
-	'uuid_add_dashes', 'uuid_strip_dashes'
+	'bytes_human', 'digits', 'from_file', 'normalize', 'random', 'strtr',
+	'to_bool', 'to_file', 'uuid_add_dashes', 'uuid_strip_dashes',
+	'version_compare'
 ]
 
 # Python imports
+import os as _os
 from random import randint as _randint
 import sys as _sys
+from typing import Literal
 
 def bytes_human(num):
 	"""Bytes Human
 
 	Returns the size of bytes in the closest binary prefix so that they are
 	clearly understood by humans
 
@@ -60,14 +63,36 @@
 	for c in val:
 		if c.isdigit():
 			lRet.append(c)
 
 	# Return the new string
 	return ''.join(lRet)
 
+def from_file(
+	filepath: str,
+	_default: str | None = None
+) -> str | None:
+	"""From File
+
+	Returns an entire file as a single string, returns None if the file doesn't
+	exist
+
+	Arguments:
+		filepath (str): The path to the file to load
+
+	Returns:
+		str | None
+	"""
+
+	try:
+		with open(filepath, 'r') as oF:
+			return oF.read()
+	except FileNotFoundError as e:
+		return _default
+
 def normalize(val):
 	"""Normalize
 
 	Replaces all special alpha characters with their ascii equivalent
 
 	Arguments:
 		val (str): The text to normalize
@@ -357,15 +382,15 @@
 	elif isinstance(characters, list):
 
 		# Init the characters
 		sChars = ''
 
 		# If it's empty
 		if len(characters) == 0:
-			raise ValueError('characters must contain at least one set name in %s' % sys._getframe().f_code.co_name)
+			raise ValueError('characters must contain at least one set name in %s' % _sys._getframe().f_code.co_name)
 
 		# Go through the list of passed characters
 		for s in characters:
 
 			# If s is not a string
 			if not isinstance(s, str):
 				raise ValueError('%s is not a string' % s)
@@ -470,14 +495,43 @@
 
 	# Raise an exception
 	raise ValueError('"%s" is not a valid boolean representation in %s' % (
 		t,
 		_sys._getframe().f_code.co_name
 	))
 
+def to_file(
+	filepath: str,
+	text: str,
+	create_path: bool = False
+) -> bool:
+	"""To File
+
+	Stores a string to a file, overwriting the contents
+
+	Arguments:
+		filepath (str): The path to the file to store the string in
+		text (str): The text to write to the file
+		create (bool): Optional, if true, path is created if it doesn't exist
+
+	Returns:
+		bool
+	"""
+
+	try:
+		with open(filepath, 'w') as oF:
+			oF.write(text)
+	except FileNotFoundError as e:
+		_os.makedirs(_os.path.dirname(filepath), exist_ok=True)
+		with open(filepath, 'w') as oF:
+			oF.write(text)
+
+	# return OK
+	return True
+
 def uuid_add_dashes(uuid):
 	"""UUID Add Dashes
 
 	Adds dashes back to a UUID that had them removed
 
 	Arguments:
 		uuid (str): The UUID to transform
@@ -506,8 +560,56 @@
 	"""
 	return '%s%s%s%s%s' % (
 		uuid[0:8],
 		uuid[9:13],
 		uuid[14:18],
 		uuid[19:23],
 		uuid[24:36]
-	)
+	)
+
+def version_compare(
+	a: str,
+	b: str
+) -> Literal[-1] | Literal[0] | Literal[1]:
+	"""Version Compare
+
+	Compares two version strings and returns whether the first one is less \
+	than (-1), equal (0), or greater than (1)
+
+	Arguments:
+		a (str): The first version
+		b (str): The second version
+
+	Returns:
+		-1 | 0 | 1
+	"""
+
+	# First, convert both strings to int lists
+	lA = [int(s) for s in a.split('.')]
+	lB = [int(s) for s in b.split('.')]
+
+	# Get the lengths of each
+	iA = len(lA)
+	iB = len(lB)
+	iLength = iA
+
+	# Make sure the lists are equal in length
+	if iA < iB:
+		for i in range(iB - iA):
+			lA.append(0)
+		iLength = iB
+	elif iA > iB:
+		for i in range(iA - iB):
+			lB.append(0)
+
+	# Go through the range
+	for i in range(iLength):
+
+		# If the values are the same
+		if lA[i] == lB[i]:
+			continue
+
+		# Return if A is less than or greater than
+		return lA[i] < lB[i] and -1 or 1
+
+	# No difference
+	return 0
```

