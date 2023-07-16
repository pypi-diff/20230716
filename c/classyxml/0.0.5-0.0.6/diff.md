# Comparing `tmp/classyxml-0.0.5.tar.gz` & `tmp/classyxml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classyxml-0.0.5.tar", last modified: Tue Mar 28 20:48:27 2023, max compression
+gzip compressed data, was "classyxml-0.0.6.tar", last modified: Sun Jul 16 21:32:01 2023, max compression
```

## Comparing `classyxml-0.0.5.tar` & `classyxml-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 20:48:27.125791 classyxml-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-03-26 23:03:55.000000 classyxml-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4529 2023-03-28 20:48:27.126249 classyxml-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3914 2023-03-28 18:14:07.000000 classyxml-0.0.5/README.md
--rw-rw-rw-   0        0        0      183 2023-03-27 05:44:47.000000 classyxml-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      752 2023-03-28 20:48:27.133231 classyxml-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-28 20:48:27.079855 classyxml-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-28 20:48:27.099957 classyxml-0.0.5/src/classy_xml/
--rw-rw-rw-   0        0        0       47 2023-03-27 17:21:17.000000 classyxml-0.0.5/src/classy_xml/__init__.py
--rw-rw-rw-   0        0        0     5727 2023-03-28 20:45:02.000000 classyxml-0.0.5/src/classy_xml/classy_xml.py
-drwxrwxrwx   0        0        0        0 2023-03-28 20:48:27.121878 classyxml-0.0.5/src/classyxml.egg-info/
--rw-rw-rw-   0        0        0     4529 2023-03-28 20:48:27.000000 classyxml-0.0.5/src/classyxml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-03-28 20:48:27.000000 classyxml-0.0.5/src/classyxml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 20:48:27.000000 classyxml-0.0.5/src/classyxml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-28 20:48:27.000000 classyxml-0.0.5/src/classyxml.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-28 20:48:27.123713 classyxml-0.0.5/tests/
--rw-rw-rw-   0        0        0    29867 2023-03-28 17:04:04.000000 classyxml-0.0.5/tests/test_classy_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:32:01.231902 classyxml-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-03-26 23:03:55.000000 classyxml-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4529 2023-07-16 21:32:01.232900 classyxml-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3914 2023-03-28 18:14:07.000000 classyxml-0.0.6/README.md
+-rw-rw-rw-   0        0        0      183 2023-03-27 05:44:47.000000 classyxml-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      752 2023-07-16 21:32:01.234898 classyxml-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 21:32:01.180804 classyxml-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 21:32:01.202261 classyxml-0.0.6/src/classy_xml/
+-rw-rw-rw-   0        0        0       47 2023-03-27 17:21:17.000000 classyxml-0.0.6/src/classy_xml/__init__.py
+-rw-rw-rw-   0        0        0     5964 2023-07-16 21:23:20.000000 classyxml-0.0.6/src/classy_xml/classy_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:32:01.228894 classyxml-0.0.6/src/classyxml.egg-info/
+-rw-rw-rw-   0        0        0     4529 2023-07-16 21:32:01.000000 classyxml-0.0.6/src/classyxml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-16 21:32:01.000000 classyxml-0.0.6/src/classyxml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:32:01.000000 classyxml-0.0.6/src/classyxml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 21:32:01.000000 classyxml-0.0.6/src/classyxml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 21:32:01.230939 classyxml-0.0.6/tests/
+-rw-rw-rw-   0        0        0    34641 2023-07-16 21:23:20.000000 classyxml-0.0.6/tests/test_classy_xml.py
```

### Comparing `classyxml-0.0.5/LICENSE` & `classyxml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `classyxml-0.0.5/PKG-INFO` & `classyxml-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classyxml
-Version: 0.0.5
+Version: 0.0.6
 Summary: An xml file parser that makes the element text and attributes of an xml file accessible as ClassyXml class attributes.
 Home-page: https://github.com/thatdspguy/classy_xml
 Author: Keaton Scheible
 Author-email: thatdspguy@gmail.com
 Project-URL: Bug Tracker, https://github.com/thatdspguy/classy_xml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classyxml-0.0.5/README.md` & `classyxml-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `classyxml-0.0.5/setup.cfg` & `classyxml-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6c61 7373 7978 6d6c 0d0a 7665   = classyxml..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 350d 0a61  rsion = 0.0.5..a
+00000020: 7273 696f 6e20 3d20 302e 302e 360d 0a61  rsion = 0.0.6..a
 00000030: 7574 686f 7220 3d20 4b65 6174 6f6e 2053  uthor = Keaton S
 00000040: 6368 6569 626c 650d 0a61 7574 686f 725f  cheible..author_
 00000050: 656d 6169 6c20 3d20 7468 6174 6473 7067  email = thatdspg
 00000060: 7579 4067 6d61 696c 2e63 6f6d 0d0a 6465  uy@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 416e 2078  scription = An x
 00000080: 6d6c 2066 696c 6520 7061 7273 6572 2074  ml file parser t
 00000090: 6861 7420 6d61 6b65 7320 7468 6520 656c  hat makes the el
```

### Comparing `classyxml-0.0.5/src/classy_xml/classy_xml.py` & `classyxml-0.0.6/src/classy_xml/classy_xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,112 @@
 from __future__ import annotations
 import os
 import xml.etree.ElementTree as ET
 from collections import defaultdict
 
 
 class ClassyXml:
-    def __init__(self, xml_file: str = None, root_xml_element_name:str ='root'):
+    def __init__(self, xml_info: str = None, root_xml_element_name: str = "root"):
         """ClassyXml Class
-        An xml file parser that makes the element text and attributes of an
-        xml file accessible as ClassyXml class attributes.
+        An xml parser that makes the element text and attributes of an xml
+        file or xml string accessible as ClassyXml class attributes.
 
         Args:
-            xml_file (str): xml file to parse
+            xml_info (str): xml file or xml string to parse
         """
         self._elements = defaultdict(list)
 
-        self.xml_file = xml_file
-        if xml_file is not None and os.path.isfile(xml_file):
-            root = ET.parse(xml_file).getroot()
+        if xml_info is not None:
+            if os.path.isfile(xml_info):
+                self.xml_file = xml_info
+                root = ET.parse(xml_info).getroot()
+            else:
+                root = ET.fromstring(xml_info)
             self.root_xml_element_name = root.tag
             self.parse_xml(root)
         else:
+            self.xml_file = None
             self.root_xml_element_name = root_xml_element_name
 
     def __setattr__(self, name, value):
         if isinstance(value, XmlElement):
             self._elements[name].append(value)
             super().__setattr__(name, self._elements[name])
         else:
             super().__setattr__(name, value)
 
     def __getattribute__(self, name):
         attr = super().__getattribute__(name)
-        if isinstance(attr, list) and isinstance(attr[0], XmlElement) and len(attr) == 1:
+        if (
+            isinstance(attr, list)
+            and isinstance(attr[0], XmlElement)
+            and len(attr) == 1
+        ):
             return attr[0]
         else:
-            return attr    
+            return attr
 
     def parse_xml(self, root: ET.Element, element: XmlElement = None):
         """Parse the xml file and create class attributes for the elements and
         attributes defined in the xml file.
         """
         for attr_name, attr_value in root.attrib.items():
             setattr(element, attr_name, attr_value)
-        children = root.findall('*')
+        children = root.findall("*")
         for child in children:
             child_element = self.parse_xml(child, XmlElement())
             if element is None:
                 setattr(self, child.tag, child_element)
             else:
                 setattr(element, child.tag, child_element)
             child_element.text = child.text
-        
+
         return element
 
     def save(self):
         if self.xml_file is None:
-            raise ValueError('XML file is not defined. Use the save_as(xml_file) method instead')
+            raise ValueError(
+                "XML file is not defined. Use the save_as(xml_file) method instead"
+            )
         self.save_as(self.xml_file)
 
     def save_as(self, xml_file):
         self.xml_file = xml_file
-        with open(xml_file, 'w') as file_handle:
-            file_handle.write(f'<{self.root_xml_element_name}>\n')
+        with open(xml_file, "w") as file_handle:
+            file_handle.write(f"<{self.root_xml_element_name}>\n")
             for element_name, elements in self._elements.items():
                 for element in elements:
                     self._write_xml(file_handle, element, element_name)
-            file_handle.write(f'</{self.root_xml_element_name}>\n')
+            file_handle.write(f"</{self.root_xml_element_name}>\n")
 
     def _write_xml(self, file_handle, element: XmlElement, element_name: str, level=1):
         file_handle.write(f'{"  "*level}<{element_name}')
 
         for attribute_name, attribute_value in element._attributes.items():
             file_handle.write(f' {attribute_name}="{attribute_value}"')
 
         if len(element._elements) == 0:
             needs_end_tag = False
             if element.text:
-                file_handle.write(f'>{element.text}</{element_name}>\n')
+                file_handle.write(f">{element.text}</{element_name}>\n")
             else:
-                file_handle.write('/>\n')
+                file_handle.write("/>\n")
         else:
             needs_end_tag = True
-            file_handle.write('>\n')
+            file_handle.write(">\n")
 
         for child_name, child_elements in element._elements.items():
             for child_element in child_elements:
-                self._write_xml(file_handle, child_element, child_name, level+1)
+                self._write_xml(file_handle, child_element, child_name, level + 1)
 
         if needs_end_tag:
             file_handle.write(f'{"  "*level}</{element_name}>\n')
 
 
 class XmlElement:
-
     def __init__(self, text: str = None, attributes: dict = {}):
         """Helper class with the ClassyXml class
 
         Args:
             text (str, optional): xml element text field. Defaults to None
             attributes (dict, optional): xml element attributes. Defaults to {}.
         """
@@ -105,66 +114,67 @@
         self._attributes = {}
         self._text = text
         self._iterated = False
 
         for name, value in attributes.items():
             setattr(self, name, value)
 
-
     def __setattr__(self, name, value):
         if isinstance(value, XmlElement):
             self._elements[name].append(value)
             super().__setattr__(name, self._elements[name])
         else:
-            if name[0] != '_' and name != 'text':
+            if name[0] != "_" and name != "text":
                 value = str(value)
                 self._attributes[name] = value
             super().__setattr__(name, value)
 
     def __getattribute__(self, name):
         attr = super().__getattribute__(name)
-        if isinstance(attr, list) and isinstance(attr[0], XmlElement) and len(attr) == 1:
+        if (
+            isinstance(attr, list)
+            and isinstance(attr[0], XmlElement)
+            and len(attr) == 1
+        ):
             return attr[0]
         else:
             return attr
-    
+
     def __iter__(self):
         return self
-    
+
     def __next__(self):
         if self._iterated:
             self._iterated = False
             raise StopIteration
         else:
             self._iterated = True
             return self
-    
+
     def __len__(self):
         return 1
-    
+
     def __getitem__(self, index: int):
         if index == 0 or index == -1:
             return self
         else:
             raise ValueError()
-        
+
     @property
     def text(self):
         return self._text
 
     @text.setter
     def text(self, value):
-        if isinstance(value, str): 
-            value = value.replace('\n', '').strip()
-            if value == '':
+        if isinstance(value, str):
+            value = value.replace("\n", "").strip()
+            if value == "":
                 value = None
         elif value == None:
             pass
-        else: 
+        else:
             value = str(value)
         self._text = value
 
     @text.deleter
     def text(self):
         self._text = None
-    
-
```

### Comparing `classyxml-0.0.5/src/classyxml.egg-info/PKG-INFO` & `classyxml-0.0.6/src/classyxml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classyxml
-Version: 0.0.5
+Version: 0.0.6
 Summary: An xml file parser that makes the element text and attributes of an xml file accessible as ClassyXml class attributes.
 Home-page: https://github.com/thatdspguy/classy_xml
 Author: Keaton Scheible
 Author-email: thatdspguy@gmail.com
 Project-URL: Bug Tracker, https://github.com/thatdspguy/classy_xml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classyxml-0.0.5/tests/test_classy_xml.py` & `classyxml-0.0.6/tests/test_classy_xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1867 +1,2166 @@
-00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
-00000010: 6f72 7420 7079 7465 7374 0d0a 6672 6f6d  ort pytest..from
-00000020: 2063 6c61 7373 795f 786d 6c20 696d 706f   classy_xml impo
-00000030: 7274 2043 6c61 7373 7958 6d6c 2c20 586d  rt ClassyXml, Xm
-00000040: 6c45 6c65 6d65 6e74 0d0a 0d0a 0d0a 4070  lElement......@p
-00000050: 7974 6573 742e 6669 7874 7572 650d 0a64  ytest.fixture..d
-00000060: 6566 2063 6c61 7373 795f 786d 6c5f 7465  ef classy_xml_te
-00000070: 7374 5f66 6978 7475 7265 2829 3a0d 0a20  st_fixture():.. 
-00000080: 2020 2066 696c 6570 6174 6820 3d20 6f73     filepath = os
-00000090: 2e70 6174 682e 7370 6c69 7428 5f5f 6669  .path.split(__fi
-000000a0: 6c65 5f5f 295b 305d 0d0a 2020 2020 7465  le__)[0]..    te
-000000b0: 7374 5f78 6d6c 203d 206f 732e 7061 7468  st_xml = os.path
-000000c0: 2e6a 6f69 6e28 6669 6c65 7061 7468 2c20  .join(filepath, 
-000000d0: 2774 6573 742e 786d 6c27 290d 0a20 2020  'test.xml')..   
-000000e0: 2072 6574 7572 6e20 436c 6173 7379 586d   return ClassyXm
-000000f0: 6c28 7465 7374 5f78 6d6c 290d 0a0d 0a0d  l(test_xml).....
-00000100: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
-00000110: 0d0a 6465 6620 636c 6173 7379 5f78 6d6c  ..def classy_xml
-00000120: 5f65 6d70 7479 5f66 6978 7475 7265 2829  _empty_fixture()
-00000130: 3a0d 0a20 2020 2072 6574 7572 6e20 436c  :..    return Cl
-00000140: 6173 7379 586d 6c28 290d 0a0d 0a0d 0a40  assyXml()......@
-00000150: 7079 7465 7374 2e66 6978 7475 7265 0d0a  pytest.fixture..
-00000160: 6465 6620 636c 6173 7379 5f78 6d6c 5f63  def classy_xml_c
-00000170: 6f75 6e74 7269 6573 5f66 6978 7475 7265  ountries_fixture
-00000180: 2829 3a0d 0a20 2020 2066 696c 6570 6174  ():..    filepat
-00000190: 6820 3d20 6f73 2e70 6174 682e 7370 6c69  h = os.path.spli
-000001a0: 7428 5f5f 6669 6c65 5f5f 295b 305d 0d0a  t(__file__)[0]..
-000001b0: 2020 2020 7465 7374 5f78 6d6c 203d 206f      test_xml = o
-000001c0: 732e 7061 7468 2e6a 6f69 6e28 6669 6c65  s.path.join(file
-000001d0: 7061 7468 2c20 2763 6f75 6e74 7269 6573  path, 'countries
-000001e0: 2e78 6d6c 2729 0d0a 2020 2020 7265 7475  .xml')..    retu
-000001f0: 726e 2043 6c61 7373 7958 6d6c 2874 6573  rn ClassyXml(tes
-00000200: 745f 786d 6c29 0d0a 0d0a 0d0a 4070 7974  t_xml)......@pyt
-00000210: 6573 742e 6669 7874 7572 650d 0a64 6566  est.fixture..def
-00000220: 2063 6c61 7373 795f 786d 6c5f 6d6f 6469   classy_xml_modi
-00000230: 6679 5f61 6e64 5f73 6176 655f 6669 7874  fy_and_save_fixt
-00000240: 7572 6528 293a 0d0a 2020 2020 7265 7475  ure():..    retu
-00000250: 726e 2043 6c61 7373 7958 6d6c 2829 0d0a  rn ClassyXml()..
-00000260: 0d0a 0d0a 6465 6620 7465 7374 5f62 6173  ....def test_bas
-00000270: 6963 5f65 6c65 6d65 6e74 5f6c 656e 6774  ic_element_lengt
-00000280: 6828 636c 6173 7379 5f78 6d6c 5f74 6573  h(classy_xml_tes
-00000290: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-000002a0: 2061 7373 6572 7420 6c65 6e28 636c 6173   assert len(clas
-000002b0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
-000002c0: 7572 652e 6261 7369 635f 656c 656d 656e  ure.basic_elemen
-000002d0: 7429 203d 3d20 310d 0a0d 0a0d 0a64 6566  t) == 1......def
-000002e0: 2074 6573 745f 6261 7369 635f 656c 656d   test_basic_elem
-000002f0: 656e 745f 7465 7874 2863 6c61 7373 795f  ent_text(classy_
-00000300: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00000310: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
-00000320: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00000330: 6978 7475 7265 2e62 6173 6963 5f65 6c65  ixture.basic_ele
-00000340: 6d65 6e74 2e74 6578 7420 3d3d 2027 6261  ment.text == 'ba
-00000350: 7369 635f 656c 656d 656e 745f 7465 7874  sic_element_text
-00000360: 270d 0a0d 0a0d 0a64 6566 2074 6573 745f  '......def test_
-00000370: 6d75 6c74 695f 656c 656d 656e 745f 6c65  multi_element_le
-00000380: 6e67 7468 2863 6c61 7373 795f 786d 6c5f  ngth(classy_xml_
-00000390: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
-000003a0: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
-000003b0: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-000003c0: 6978 7475 7265 2e6d 756c 7469 5f65 6c65  ixture.multi_ele
-000003d0: 6d65 6e74 2920 3d3d 2032 0d0a 0d0a 0d0a  ment) == 2......
-000003e0: 6465 6620 7465 7374 5f6d 756c 7469 5f65  def test_multi_e
-000003f0: 6c65 6d65 6e74 5f30 5f74 6578 7428 636c  lement_0_text(cl
-00000400: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00000410: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
-00000420: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00000430: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00000440: 695f 656c 656d 656e 745b 305d 2e74 6578  i_element[0].tex
-00000450: 7420 3d3d 2027 6d75 6c74 695f 656c 656d  t == 'multi_elem
-00000460: 656e 745f 7465 7874 5f30 270d 0a0d 0a0d  ent_text_0'.....
-00000470: 0a64 6566 2074 6573 745f 6d75 6c74 695f  .def test_multi_
-00000480: 656c 656d 656e 745f 315f 7465 7874 2863  element_1_text(c
-00000490: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-000004a0: 6978 7475 7265 293a 0d0a 2020 2020 6173  ixture):..    as
-000004b0: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
-000004c0: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
-000004d0: 7469 5f65 6c65 6d65 6e74 5b31 5d2e 7465  ti_element[1].te
-000004e0: 7874 203d 3d20 276d 756c 7469 5f65 6c65  xt == 'multi_ele
-000004f0: 6d65 6e74 5f74 6578 745f 3127 0d0a 0d0a  ment_text_1'....
-00000500: 0d0a 6465 6620 7465 7374 5f65 6d70 7479  ..def test_empty
-00000510: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
-00000520: 7472 6962 7574 6573 5f6c 656e 6774 6828  tributes_length(
-00000530: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00000540: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
-00000550: 7373 6572 7420 6c65 6e28 636c 6173 7379  ssert len(classy
-00000560: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-00000570: 652e 656d 7074 795f 656c 656d 656e 745f  e.empty_element_
-00000580: 7769 7468 5f61 7474 7269 6275 7465 7329  with_attributes)
-00000590: 203d 3d20 310d 0a0d 0a0d 0a64 6566 2074   == 1......def t
-000005a0: 6573 745f 656d 7074 795f 656c 656d 656e  est_empty_elemen
-000005b0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-000005c0: 735f 7465 7874 2863 6c61 7373 795f 786d  s_text(classy_xm
-000005d0: 6c5f 7465 7374 5f66 6978 7475 7265 293a  l_test_fixture):
-000005e0: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-000005f0: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00000600: 7475 7265 2e65 6d70 7479 5f65 6c65 6d65  ture.empty_eleme
-00000610: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00000620: 6573 2e74 6578 7420 6973 204e 6f6e 650d  es.text is None.
-00000630: 0a0d 0a0d 0a64 6566 2074 6573 745f 656d  .....def test_em
-00000640: 7074 795f 656c 656d 656e 745f 7769 7468  pty_element_with
-00000650: 5f61 7474 7269 6275 7465 735f 6174 7472  _attributes_attr
-00000660: 6962 7574 6573 2863 6c61 7373 795f 786d  ibutes(classy_xm
-00000670: 6c5f 7465 7374 5f66 6978 7475 7265 293a  l_test_fixture):
-00000680: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00000690: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-000006a0: 7475 7265 2e65 6d70 7479 5f65 6c65 6d65  ture.empty_eleme
-000006b0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-000006c0: 6573 2e6e 616d 6520 3d3d 2027 6174 7472  es.name == 'attr
-000006d0: 5f6e 616d 6527 0d0a 2020 2020 6173 7365  _name'..    asse
-000006e0: 7274 2063 6c61 7373 795f 786d 6c5f 7465  rt classy_xml_te
-000006f0: 7374 5f66 6978 7475 7265 2e65 6d70 7479  st_fixture.empty
-00000700: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
-00000710: 7472 6962 7574 6573 2e76 616c 7565 203d  tributes.value =
-00000720: 3d20 2761 7474 725f 7661 6c75 6527 0d0a  = 'attr_value'..
-00000730: 0d0a 0d0a 6465 6620 7465 7374 5f65 6d70  ....def test_emp
-00000740: 7479 5f6d 756c 7469 5f65 6c65 6d65 6e74  ty_multi_element
-00000750: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00000760: 5f6c 656e 6774 6828 636c 6173 7379 5f78  _length(classy_x
-00000770: 6d6c 5f74 6573 745f 6669 7874 7572 6529  ml_test_fixture)
-00000780: 3a0d 0a20 2020 2061 7373 6572 7420 6c65  :..    assert le
-00000790: 6e28 636c 6173 7379 5f78 6d6c 5f74 6573  n(classy_xml_tes
-000007a0: 745f 6669 7874 7572 652e 656d 7074 795f  t_fixture.empty_
-000007b0: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
-000007c0: 7468 5f61 7474 7269 6275 7465 7329 203d  th_attributes) =
-000007d0: 3d20 320d 0a0d 0a0d 0a64 6566 2074 6573  = 2......def tes
-000007e0: 745f 656d 7074 795f 6d75 6c74 695f 656c  t_empty_multi_el
-000007f0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00000800: 6275 7465 735f 7465 7874 2863 6c61 7373  butes_text(class
-00000810: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00000820: 7265 293a 0d0a 2020 2020 6173 7365 7274  re):..    assert
-00000830: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
-00000840: 5f66 6978 7475 7265 2e65 6d70 7479 5f6d  _fixture.empty_m
-00000850: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00000860: 685f 6174 7472 6962 7574 6573 5b30 5d2e  h_attributes[0].
-00000870: 7465 7874 2069 7320 4e6f 6e65 0d0a 2020  text is None..  
-00000880: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-00000890: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-000008a0: 2e65 6d70 7479 5f6d 756c 7469 5f65 6c65  .empty_multi_ele
-000008b0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-000008c0: 7574 6573 5b31 5d2e 7465 7874 2069 7320  utes[1].text is 
-000008d0: 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620 7465  None......def te
-000008e0: 7374 5f65 6d70 7479 5f6d 756c 7469 5f65  st_empty_multi_e
-000008f0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-00000900: 6962 7574 6573 5f61 7474 7269 6275 7465  ibutes_attribute
-00000910: 7328 636c 6173 7379 5f78 6d6c 5f74 6573  s(classy_xml_tes
-00000920: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00000930: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00000940: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00000950: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
-00000960: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00000970: 7465 735b 305d 2e6e 616d 6520 3d3d 2027  tes[0].name == '
-00000980: 6174 7472 5f30 5f6e 616d 6527 0d0a 2020  attr_0_name'..  
-00000990: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-000009a0: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-000009b0: 2e65 6d70 7479 5f6d 756c 7469 5f65 6c65  .empty_multi_ele
-000009c0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-000009d0: 7574 6573 5b0d 0a20 2020 2020 2020 2030  utes[..        0
-000009e0: 5d2e 7661 6c75 6520 3d3d 2027 6174 7472  ].value == 'attr
-000009f0: 5f30 5f76 616c 7565 270d 0a20 2020 2061  _0_value'..    a
-00000a00: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00000a10: 5f74 6573 745f 6669 7874 7572 652e 656d  _test_fixture.em
-00000a20: 7074 795f 6d75 6c74 695f 656c 656d 656e  pty_multi_elemen
-00000a30: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-00000a40: 735b 315d 2e6e 616d 6520 3d3d 2027 6174  s[1].name == 'at
-00000a50: 7472 5f31 5f6e 616d 6527 0d0a 2020 2020  tr_1_name'..    
-00000a60: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
-00000a70: 6c5f 7465 7374 5f66 6978 7475 7265 2e65  l_test_fixture.e
-00000a80: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
-00000a90: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00000aa0: 6573 5b0d 0a20 2020 2020 2020 2031 5d2e  es[..        1].
-00000ab0: 7661 6c75 6520 3d3d 2027 6174 7472 5f31  value == 'attr_1
-00000ac0: 5f76 616c 7565 270d 0a0d 0a0d 0a64 6566  _value'......def
-00000ad0: 2074 6573 745f 6261 7369 635f 656c 656d   test_basic_elem
-00000ae0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00000af0: 7465 735f 6c65 6e67 7468 2863 6c61 7373  tes_length(class
-00000b00: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00000b10: 7265 293a 0d0a 2020 2020 6173 7365 7274  re):..    assert
-00000b20: 206c 656e 2863 6c61 7373 795f 786d 6c5f   len(classy_xml_
-00000b30: 7465 7374 5f66 6978 7475 7265 2e62 6173  test_fixture.bas
-00000b40: 6963 5f65 6c65 6d65 6e74 5f77 6974 685f  ic_element_with_
-00000b50: 6174 7472 6962 7574 6573 2920 3d3d 2031  attributes) == 1
-00000b60: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f62  ......def test_b
-00000b70: 6173 6963 5f65 6c65 6d65 6e74 5f77 6974  asic_element_wit
-00000b80: 685f 6174 7472 6962 7574 6573 5f74 6578  h_attributes_tex
-00000b90: 7428 636c 6173 7379 5f78 6d6c 5f74 6573  t(classy_xml_tes
-00000ba0: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00000bb0: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00000bc0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00000bd0: 6261 7369 635f 656c 656d 656e 745f 7769  basic_element_wi
-00000be0: 7468 5f61 7474 7269 6275 7465 732e 7465  th_attributes.te
-00000bf0: 7874 203d 3d20 2762 6173 6963 5f65 6c65  xt == 'basic_ele
-00000c00: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-00000c10: 7574 6573 5f74 6578 7427 0d0a 0d0a 0d0a  utes_text'......
-00000c20: 6465 6620 7465 7374 5f62 6173 6963 5f65  def test_basic_e
-00000c30: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-00000c40: 6962 7574 6573 5f61 7474 7269 6275 7465  ibutes_attribute
-00000c50: 7328 636c 6173 7379 5f78 6d6c 5f74 6573  s(classy_xml_tes
-00000c60: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00000c70: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00000c80: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00000c90: 6261 7369 635f 656c 656d 656e 745f 7769  basic_element_wi
-00000ca0: 7468 5f61 7474 7269 6275 7465 732e 6e61  th_attributes.na
-00000cb0: 6d65 203d 3d20 2761 7474 725f 6e61 6d65  me == 'attr_name
-00000cc0: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00000cd0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00000ce0: 7874 7572 652e 6261 7369 635f 656c 656d  xture.basic_elem
-00000cf0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00000d00: 7465 732e 7661 6c75 6520 3d3d 2027 6174  tes.value == 'at
-00000d10: 7472 5f76 616c 7565 270d 0a0d 0a0d 0a64  tr_value'......d
-00000d20: 6566 2074 6573 745f 6d75 6c74 695f 656c  ef test_multi_el
-00000d30: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00000d40: 6275 7465 735f 6c65 6e67 7468 2863 6c61  butes_length(cla
-00000d50: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00000d60: 7475 7265 293a 0d0a 2020 2020 6173 7365  ture):..    asse
-00000d70: 7274 206c 656e 2863 6c61 7373 795f 786d  rt len(classy_xm
-00000d80: 6c5f 7465 7374 5f66 6978 7475 7265 2e6d  l_test_fixture.m
-00000d90: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00000da0: 685f 6174 7472 6962 7574 6573 2920 3d3d  h_attributes) ==
-00000db0: 2032 0d0a 0d0a 0d0a 6465 6620 7465 7374   2......def test
-00000dc0: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
-00000dd0: 6974 685f 6174 7472 6962 7574 6573 5f74  ith_attributes_t
-00000de0: 6578 7428 636c 6173 7379 5f78 6d6c 5f74  ext(classy_xml_t
-00000df0: 6573 745f 6669 7874 7572 6529 3a0d 0a20  est_fixture):.. 
-00000e00: 2020 2061 7373 6572 7420 636c 6173 7379     assert classy
-00000e10: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-00000e20: 652e 6d75 6c74 695f 656c 656d 656e 745f  e.multi_element_
-00000e30: 7769 7468 5f61 7474 7269 6275 7465 735b  with_attributes[
-00000e40: 0d0a 2020 2020 2020 2020 305d 2e74 6578  ..        0].tex
-00000e50: 7420 3d3d 2027 6d75 6c74 695f 656c 656d  t == 'multi_elem
-00000e60: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00000e70: 7465 735f 7465 7874 5f30 270d 0a20 2020  tes_text_0'..   
-00000e80: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00000e90: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00000ea0: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
-00000eb0: 7468 5f61 7474 7269 6275 7465 735b 0d0a  th_attributes[..
-00000ec0: 2020 2020 2020 2020 315d 2e74 6578 7420          1].text 
-00000ed0: 3d3d 2027 6d75 6c74 695f 656c 656d 656e  == 'multi_elemen
-00000ee0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-00000ef0: 735f 7465 7874 5f31 270d 0a0d 0a0d 0a64  s_text_1'......d
-00000f00: 6566 2074 6573 745f 6d75 6c74 695f 656c  ef test_multi_el
-00000f10: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00000f20: 6275 7465 735f 6174 7472 6962 7574 6573  butes_attributes
-00000f30: 2863 6c61 7373 795f 786d 6c5f 7465 7374  (classy_xml_test
-00000f40: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-00000f50: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
-00000f60: 6c5f 7465 7374 5f66 6978 7475 7265 2e6d  l_test_fixture.m
-00000f70: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00000f80: 685f 6174 7472 6962 7574 6573 5b30 5d2e  h_attributes[0].
-00000f90: 6e61 6d65 203d 3d20 2761 7474 725f 305f  name == 'attr_0_
-00000fa0: 6e61 6d65 270d 0a20 2020 2061 7373 6572  name'..    asser
-00000fb0: 7420 636c 6173 7379 5f78 6d6c 5f74 6573  t classy_xml_tes
-00000fc0: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
-00000fd0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00000fe0: 7269 6275 7465 735b 305d 2e76 616c 7565  ributes[0].value
-00000ff0: 203d 3d20 2761 7474 725f 305f 7661 6c75   == 'attr_0_valu
-00001000: 6527 0d0a 2020 2020 6173 7365 7274 2063  e'..    assert c
-00001010: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001020: 6978 7475 7265 2e6d 756c 7469 5f65 6c65  ixture.multi_ele
-00001030: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-00001040: 7574 6573 5b31 5d2e 6e61 6d65 203d 3d20  utes[1].name == 
-00001050: 2761 7474 725f 315f 6e61 6d65 270d 0a20  'attr_1_name'.. 
-00001060: 2020 2061 7373 6572 7420 636c 6173 7379     assert classy
-00001070: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-00001080: 652e 6d75 6c74 695f 656c 656d 656e 745f  e.multi_element_
-00001090: 7769 7468 5f61 7474 7269 6275 7465 735b  with_attributes[
-000010a0: 315d 2e76 616c 7565 203d 3d20 2761 7474  1].value == 'att
-000010b0: 725f 315f 7661 6c75 6527 0d0a 0d0a 0d0a  r_1_value'......
-000010c0: 6465 6620 7465 7374 5f62 6173 6963 5f6e  def test_basic_n
-000010d0: 6573 7465 645f 656c 656d 656e 745f 6c65  ested_element_le
-000010e0: 6e67 7468 2863 6c61 7373 795f 786d 6c5f  ngth(classy_xml_
-000010f0: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
-00001100: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
-00001110: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001120: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-00001130: 7465 645f 656c 656d 656e 7429 203d 3d20  ted_element) == 
-00001140: 310d 0a0d 0a0d 0a64 6566 2074 6573 745f  1......def test_
-00001150: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
-00001160: 6d65 6e74 5f5f 6261 7369 635f 656c 656d  ment__basic_elem
-00001170: 656e 745f 6368 696c 645f 6c65 6e67 7468  ent_child_length
-00001180: 2863 6c61 7373 795f 786d 6c5f 7465 7374  (classy_xml_test
-00001190: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-000011a0: 6173 7365 7274 206c 656e 280d 0a20 2020  assert len(..   
-000011b0: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
-000011c0: 7465 7374 5f66 6978 7475 7265 2e62 6173  test_fixture.bas
-000011d0: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
-000011e0: 742e 6261 7369 635f 656c 656d 656e 745f  t.basic_element_
-000011f0: 6368 696c 6429 203d 3d20 310d 0a0d 0a0d  child) == 1.....
-00001200: 0a64 6566 2074 6573 745f 6261 7369 635f  .def test_basic_
-00001210: 6e65 7374 6564 5f65 6c65 6d65 6e74 5f5f  nested_element__
-00001220: 6261 7369 635f 656c 656d 656e 745f 6368  basic_element_ch
-00001230: 696c 645f 7465 7874 2863 6c61 7373 795f  ild_text(classy_
-00001240: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00001250: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
-00001260: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001270: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-00001280: 7465 645f 656c 656d 656e 742e 6261 7369  ted_element.basi
-00001290: 635f 656c 656d 656e 745f 6368 696c 642e  c_element_child.
-000012a0: 7465 7874 203d 3d20 2762 6173 6963 5f65  text == 'basic_e
-000012b0: 6c65 6d65 6e74 5f63 6869 6c64 5f74 6578  lement_child_tex
-000012c0: 7427 0d0a 0d0a 0d0a 6465 6620 7465 7374  t'......def test
-000012d0: 5f62 6173 6963 5f6e 6573 7465 645f 656c  _basic_nested_el
-000012e0: 656d 656e 745f 5f6d 756c 7469 5f65 6c65  ement__multi_ele
-000012f0: 6d65 6e74 5f63 6869 6c64 5f6c 656e 6774  ment_child_lengt
-00001300: 6828 636c 6173 7379 5f78 6d6c 5f74 6573  h(classy_xml_tes
-00001310: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00001320: 2061 7373 6572 7420 6c65 6e28 0d0a 2020   assert len(..  
-00001330: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
-00001340: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
-00001350: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
-00001360: 6e74 2e6d 756c 7469 5f65 6c65 6d65 6e74  nt.multi_element
-00001370: 5f63 6869 6c64 2920 3d3d 2032 0d0a 0d0a  _child) == 2....
-00001380: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
-00001390: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
-000013a0: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f63  _multi_element_c
-000013b0: 6869 6c64 5f74 6578 7428 636c 6173 7379  hild_text(classy
-000013c0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-000013d0: 6529 3a0d 0a20 2020 2061 7373 6572 7420  e):..    assert 
-000013e0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-000013f0: 6669 7874 7572 652e 6261 7369 635f 6e65  fixture.basic_ne
-00001400: 7374 6564 5f65 6c65 6d65 6e74 2e6d 756c  sted_element.mul
-00001410: 7469 5f65 6c65 6d65 6e74 5f63 6869 6c64  ti_element_child
-00001420: 5b0d 0a20 2020 2020 2020 2030 5d2e 7465  [..        0].te
-00001430: 7874 203d 3d20 276d 756c 7469 5f65 6c65  xt == 'multi_ele
-00001440: 6d65 6e74 5f63 6869 6c64 5f74 6578 745f  ment_child_text_
-00001450: 3027 0d0a 2020 2020 6173 7365 7274 2063  0'..    assert c
-00001460: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001470: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-00001480: 7465 645f 656c 656d 656e 742e 6d75 6c74  ted_element.mult
-00001490: 695f 656c 656d 656e 745f 6368 696c 645b  i_element_child[
-000014a0: 0d0a 2020 2020 2020 2020 315d 2e74 6578  ..        1].tex
-000014b0: 7420 3d3d 2027 6d75 6c74 695f 656c 656d  t == 'multi_elem
-000014c0: 656e 745f 6368 696c 645f 7465 7874 5f31  ent_child_text_1
-000014d0: 270d 0a0d 0a0d 0a64 6566 2074 6573 745f  '......def test_
-000014e0: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
-000014f0: 6d65 6e74 5f5f 656d 7074 795f 656c 656d  ment__empty_elem
-00001500: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00001510: 7465 735f 6368 696c 645f 6c65 6e67 7468  tes_child_length
-00001520: 2863 6c61 7373 795f 786d 6c5f 7465 7374  (classy_xml_test
-00001530: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-00001540: 6173 7365 7274 206c 656e 280d 0a20 2020  assert len(..   
-00001550: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
-00001560: 7465 7374 5f66 6978 7475 7265 2e62 6173  test_fixture.bas
-00001570: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
-00001580: 742e 656d 7074 795f 656c 656d 656e 745f  t.empty_element_
-00001590: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-000015a0: 6368 696c 6429 203d 3d20 310d 0a0d 0a0d  child) == 1.....
-000015b0: 0a64 6566 2074 6573 745f 6261 7369 635f  .def test_basic_
-000015c0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5f5f  nested_element__
-000015d0: 656d 7074 795f 656c 656d 656e 745f 7769  empty_element_wi
-000015e0: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-000015f0: 696c 645f 7465 7874 2863 6c61 7373 795f  ild_text(classy_
-00001600: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00001610: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
-00001620: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001630: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-00001640: 7465 645f 656c 656d 656e 742e 656d 7074  ted_element.empt
-00001650: 795f 656c 656d 656e 745f 7769 7468 5f61  y_element_with_a
-00001660: 7474 7269 6275 7465 735f 6368 696c 642e  ttributes_child.
-00001670: 7465 7874 2069 7320 4e6f 6e65 0d0a 0d0a  text is None....
-00001680: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
-00001690: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
-000016a0: 5f65 6d70 7479 5f65 6c65 6d65 6e74 5f77  _empty_element_w
-000016b0: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-000016c0: 6869 6c64 5f61 7474 7269 6275 7465 7328  hild_attributes(
-000016d0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-000016e0: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
-000016f0: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00001700: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
-00001710: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
-00001720: 6e74 2e65 6d70 7479 5f65 6c65 6d65 6e74  nt.empty_element
-00001730: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00001740: 5f63 6869 6c64 2e6e 616d 6520 3d3d 2027  _child.name == '
-00001750: 6368 696c 645f 6174 7472 5f6e 616d 6527  child_attr_name'
-00001760: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00001770: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00001780: 7475 7265 2e62 6173 6963 5f6e 6573 7465  ture.basic_neste
-00001790: 645f 656c 656d 656e 742e 656d 7074 795f  d_element.empty_
-000017a0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-000017b0: 7269 6275 7465 735f 6368 696c 642e 7661  ributes_child.va
-000017c0: 6c75 6520 3d3d 2027 6368 696c 645f 6174  lue == 'child_at
-000017d0: 7472 5f76 616c 7565 270d 0a0d 0a0d 0a64  tr_value'......d
-000017e0: 6566 2074 6573 745f 6261 7369 635f 6e65  ef test_basic_ne
-000017f0: 7374 6564 5f65 6c65 6d65 6e74 5f5f 656d  sted_element__em
-00001800: 7074 795f 6d75 6c74 695f 656c 656d 656e  pty_multi_elemen
-00001810: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-00001820: 735f 6368 696c 645f 6c65 6e67 7468 2863  s_child_length(c
-00001830: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001840: 6978 7475 7265 293a 0d0a 2020 2020 6173  ixture):..    as
-00001850: 7365 7274 206c 656e 280d 0a20 2020 2020  sert len(..     
-00001860: 2020 2063 6c61 7373 795f 786d 6c5f 7465     classy_xml_te
-00001870: 7374 5f66 6978 7475 7265 2e62 6173 6963  st_fixture.basic
-00001880: 5f6e 6573 7465 645f 656c 656d 656e 742e  _nested_element.
-00001890: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
-000018a0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-000018b0: 7465 735f 6368 696c 6429 203d 3d20 320d  tes_child) == 2.
-000018c0: 0a0d 0a0d 0a64 6566 2074 6573 745f 6261  .....def test_ba
-000018d0: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
-000018e0: 6e74 5f5f 656d 7074 795f 6d75 6c74 695f  nt__empty_multi_
-000018f0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00001900: 7269 6275 7465 735f 6368 696c 645f 7465  ributes_child_te
-00001910: 7874 2863 6c61 7373 795f 786d 6c5f 7465  xt(classy_xml_te
-00001920: 7374 5f66 6978 7475 7265 293a 0d0a 2020  st_fixture):..  
-00001930: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-00001940: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00001950: 2e62 6173 6963 5f6e 6573 7465 645f 656c  .basic_nested_el
-00001960: 656d 656e 742e 656d 7074 795f 6d75 6c74  ement.empty_mult
-00001970: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
-00001980: 7474 7269 6275 7465 735f 6368 696c 645b  ttributes_child[
-00001990: 0d0a 2020 2020 2020 2020 305d 2e74 6578  ..        0].tex
-000019a0: 7420 6973 204e 6f6e 650d 0a20 2020 2061  t is None..    a
-000019b0: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-000019c0: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
-000019d0: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
-000019e0: 6e74 2e65 6d70 7479 5f6d 756c 7469 5f65  nt.empty_multi_e
-000019f0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-00001a00: 6962 7574 6573 5f63 6869 6c64 5b0d 0a20  ibutes_child[.. 
-00001a10: 2020 2020 2020 2031 5d2e 7465 7874 2069         1].text i
-00001a20: 7320 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620  s None......def 
-00001a30: 7465 7374 5f62 6173 6963 5f6e 6573 7465  test_basic_neste
-00001a40: 645f 656c 656d 656e 745f 5f65 6d70 7479  d_element__empty
-00001a50: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
-00001a60: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-00001a70: 6869 6c64 5f61 7474 7269 6275 7465 7328  hild_attributes(
-00001a80: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00001a90: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
-00001aa0: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00001ab0: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
-00001ac0: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
-00001ad0: 6e74 2e65 6d70 7479 5f6d 756c 7469 5f65  nt.empty_multi_e
-00001ae0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-00001af0: 6962 7574 6573 5f63 6869 6c64 5b0d 0a20  ibutes_child[.. 
-00001b00: 2020 2020 2020 2030 5d2e 6e61 6d65 203d         0].name =
-00001b10: 3d20 2763 6869 6c64 5f61 7474 725f 305f  = 'child_attr_0_
-00001b20: 6e61 6d65 270d 0a20 2020 2061 7373 6572  name'..    asser
-00001b30: 7420 636c 6173 7379 5f78 6d6c 5f74 6573  t classy_xml_tes
-00001b40: 745f 6669 7874 7572 652e 6261 7369 635f  t_fixture.basic_
-00001b50: 6e65 7374 6564 5f65 6c65 6d65 6e74 2e65  nested_element.e
-00001b60: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
-00001b70: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00001b80: 6573 5f63 6869 6c64 5b0d 0a20 2020 2020  es_child[..     
-00001b90: 2020 2030 5d2e 7661 6c75 6520 3d3d 2027     0].value == '
-00001ba0: 6368 696c 645f 6174 7472 5f30 5f76 616c  child_attr_0_val
-00001bb0: 7565 270d 0a20 2020 2061 7373 6572 7420  ue'..    assert 
-00001bc0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00001bd0: 6669 7874 7572 652e 6261 7369 635f 6e65  fixture.basic_ne
-00001be0: 7374 6564 5f65 6c65 6d65 6e74 2e65 6d70  sted_element.emp
-00001bf0: 7479 5f6d 756c 7469 5f65 6c65 6d65 6e74  ty_multi_element
-00001c00: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00001c10: 5f63 6869 6c64 5b0d 0a20 2020 2020 2020  _child[..       
-00001c20: 2031 5d2e 6e61 6d65 203d 3d20 2763 6869   1].name == 'chi
-00001c30: 6c64 5f61 7474 725f 315f 6e61 6d65 270d  ld_attr_1_name'.
-00001c40: 0a20 2020 2061 7373 6572 7420 636c 6173  .    assert clas
-00001c50: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
-00001c60: 7572 652e 6261 7369 635f 6e65 7374 6564  ure.basic_nested
-00001c70: 5f65 6c65 6d65 6e74 2e65 6d70 7479 5f6d  _element.empty_m
-00001c80: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00001c90: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-00001ca0: 6c64 5b0d 0a20 2020 2020 2020 2031 5d2e  ld[..        1].
-00001cb0: 7661 6c75 6520 3d3d 2027 6368 696c 645f  value == 'child_
-00001cc0: 6174 7472 5f31 5f76 616c 7565 270d 0a0d  attr_1_value'...
-00001cd0: 0a0d 0a64 6566 2074 6573 745f 6261 7369  ...def test_basi
-00001ce0: 635f 6e65 7374 6564 5f65 6c65 6d65 6e74  c_nested_element
-00001cf0: 5f5f 6261 7369 635f 656c 656d 656e 745f  __basic_element_
-00001d00: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00001d10: 6368 696c 645f 6c65 6e67 7468 2863 6c61  child_length(cla
-00001d20: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00001d30: 7475 7265 293a 0d0a 2020 2020 6173 7365  ture):..    asse
-00001d40: 7274 206c 656e 280d 0a20 2020 2020 2020  rt len(..       
-00001d50: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
-00001d60: 5f66 6978 7475 7265 2e62 6173 6963 5f6e  _fixture.basic_n
-00001d70: 6573 7465 645f 656c 656d 656e 742e 6261  ested_element.ba
-00001d80: 7369 635f 656c 656d 656e 745f 7769 7468  sic_element_with
-00001d90: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00001da0: 6429 203d 3d20 310d 0a0d 0a0d 0a64 6566  d) == 1......def
-00001db0: 2074 6573 745f 6261 7369 635f 6e65 7374   test_basic_nest
-00001dc0: 6564 5f65 6c65 6d65 6e74 5f5f 6261 7369  ed_element__basi
-00001dd0: 635f 656c 656d 656e 745f 7769 7468 5f61  c_element_with_a
-00001de0: 7474 7269 6275 7465 735f 6368 696c 645f  ttributes_child_
-00001df0: 7465 7874 2863 6c61 7373 795f 786d 6c5f  text(classy_xml_
-00001e00: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
-00001e10: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-00001e20: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00001e30: 7265 2e62 6173 6963 5f6e 6573 7465 645f  re.basic_nested_
-00001e40: 656c 656d 656e 742e 6261 7369 635f 656c  element.basic_el
-00001e50: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00001e60: 6275 7465 735f 6368 696c 642e 7465 7874  butes_child.text
-00001e70: 203d 3d20 2762 6173 6963 5f65 6c65 6d65   == 'basic_eleme
-00001e80: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00001e90: 6573 5f63 6869 6c64 5f74 6578 7427 0d0a  es_child_text'..
-00001ea0: 0d0a 0d0a 6465 6620 7465 7374 5f62 6173  ....def test_bas
-00001eb0: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
-00001ec0: 745f 5f62 6173 6963 5f65 6c65 6d65 6e74  t__basic_element
-00001ed0: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00001ee0: 5f63 6869 6c64 5f61 7474 7269 6275 7465  _child_attribute
-00001ef0: 7328 636c 6173 7379 5f78 6d6c 5f74 6573  s(classy_xml_tes
-00001f00: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00001f10: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00001f20: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00001f30: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
-00001f40: 6d65 6e74 2e62 6173 6963 5f65 6c65 6d65  ment.basic_eleme
-00001f50: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00001f60: 6573 5f63 6869 6c64 2e6e 616d 6520 3d3d  es_child.name ==
-00001f70: 2027 6368 696c 645f 6174 7472 5f6e 616d   'child_attr_nam
-00001f80: 6527 0d0a 2020 2020 6173 7365 7274 2063  e'..    assert c
-00001f90: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00001fa0: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-00001fb0: 7465 645f 656c 656d 656e 742e 6261 7369  ted_element.basi
-00001fc0: 635f 656c 656d 656e 745f 7769 7468 5f61  c_element_with_a
-00001fd0: 7474 7269 6275 7465 735f 6368 696c 642e  ttributes_child.
-00001fe0: 7661 6c75 6520 3d3d 2027 6368 696c 645f  value == 'child_
-00001ff0: 6174 7472 5f76 616c 7565 270d 0a0d 0a0d  attr_value'.....
-00002000: 0a64 6566 2074 6573 745f 6261 7369 635f  .def test_basic_
-00002010: 6e65 7374 6564 5f65 6c65 6d65 6e74 5f5f  nested_element__
-00002020: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
-00002030: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-00002040: 696c 645f 6c65 6e67 7468 2863 6c61 7373  ild_length(class
-00002050: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00002060: 7265 293a 0d0a 2020 2020 6173 7365 7274  re):..    assert
-00002070: 206c 656e 280d 0a20 2020 2020 2020 2063   len(..        c
-00002080: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00002090: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
-000020a0: 7465 645f 656c 656d 656e 742e 6d75 6c74  ted_element.mult
-000020b0: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
-000020c0: 7474 7269 6275 7465 735f 6368 696c 6429  ttributes_child)
-000020d0: 203d 3d20 320d 0a0d 0a0d 0a64 6566 2074   == 2......def t
-000020e0: 6573 745f 6261 7369 635f 6e65 7374 6564  est_basic_nested
-000020f0: 5f65 6c65 6d65 6e74 5f5f 6d75 6c74 695f  _element__multi_
-00002100: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00002110: 7269 6275 7465 735f 6368 696c 645f 7465  ributes_child_te
-00002120: 7874 2863 6c61 7373 795f 786d 6c5f 7465  xt(classy_xml_te
-00002130: 7374 5f66 6978 7475 7265 293a 0d0a 2020  st_fixture):..  
-00002140: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-00002150: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00002160: 2e62 6173 6963 5f6e 6573 7465 645f 656c  .basic_nested_el
-00002170: 656d 656e 742e 6d75 6c74 695f 656c 656d  ement.multi_elem
-00002180: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00002190: 7465 735f 6368 696c 645b 0d0a 2020 2020  tes_child[..    
-000021a0: 2020 2020 305d 2e74 6578 7420 3d3d 2027      0].text == '
-000021b0: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
-000021c0: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-000021d0: 696c 645f 7465 7874 5f30 270d 0a20 2020  ild_text_0'..   
-000021e0: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-000021f0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00002200: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
-00002210: 6d65 6e74 2e6d 756c 7469 5f65 6c65 6d65  ment.multi_eleme
-00002220: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00002230: 6573 5f63 6869 6c64 5b0d 0a20 2020 2020  es_child[..     
-00002240: 2020 2031 5d2e 7465 7874 203d 3d20 276d     1].text == 'm
-00002250: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00002260: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-00002270: 6c64 5f74 6578 745f 3127 0d0a 0d0a 0d0a  ld_text_1'......
-00002280: 6465 6620 7465 7374 5f62 6173 6963 5f6e  def test_basic_n
-00002290: 6573 7465 645f 656c 656d 656e 745f 5f6d  ested_element__m
-000022a0: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-000022b0: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-000022c0: 6c64 5f61 7474 7269 6275 7465 7328 636c  ld_attributes(cl
-000022d0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-000022e0: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
-000022f0: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00002300: 6573 745f 6669 7874 7572 652e 6261 7369  est_fixture.basi
-00002310: 635f 6e65 7374 6564 5f65 6c65 6d65 6e74  c_nested_element
-00002320: 2e6d 756c 7469 5f65 6c65 6d65 6e74 5f77  .multi_element_w
-00002330: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-00002340: 6869 6c64 5b0d 0a20 2020 2020 2020 2030  hild[..        0
-00002350: 5d2e 6e61 6d65 203d 3d20 2763 6869 6c64  ].name == 'child
-00002360: 5f61 7474 725f 305f 6e61 6d65 270d 0a20  _attr_0_name'.. 
-00002370: 2020 2061 7373 6572 7420 636c 6173 7379     assert classy
-00002380: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-00002390: 652e 6261 7369 635f 6e65 7374 6564 5f65  e.basic_nested_e
-000023a0: 6c65 6d65 6e74 2e6d 756c 7469 5f65 6c65  lement.multi_ele
-000023b0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-000023c0: 7574 6573 5f63 6869 6c64 5b0d 0a20 2020  utes_child[..   
-000023d0: 2020 2020 2030 5d2e 7661 6c75 6520 3d3d       0].value ==
-000023e0: 2027 6368 696c 645f 6174 7472 5f30 5f76   'child_attr_0_v
-000023f0: 616c 7565 270d 0a20 2020 2061 7373 6572  alue'..    asser
-00002400: 7420 636c 6173 7379 5f78 6d6c 5f74 6573  t classy_xml_tes
-00002410: 745f 6669 7874 7572 652e 6261 7369 635f  t_fixture.basic_
-00002420: 6e65 7374 6564 5f65 6c65 6d65 6e74 2e6d  nested_element.m
-00002430: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00002440: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-00002450: 6c64 5b0d 0a20 2020 2020 2020 2031 5d2e  ld[..        1].
-00002460: 6e61 6d65 203d 3d20 2763 6869 6c64 5f61  name == 'child_a
-00002470: 7474 725f 315f 6e61 6d65 270d 0a20 2020  ttr_1_name'..   
-00002480: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00002490: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-000024a0: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
-000024b0: 6d65 6e74 2e6d 756c 7469 5f65 6c65 6d65  ment.multi_eleme
-000024c0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-000024d0: 6573 5f63 6869 6c64 5b0d 0a20 2020 2020  es_child[..     
-000024e0: 2020 2031 5d2e 7661 6c75 6520 3d3d 2027     1].value == '
-000024f0: 6368 696c 645f 6174 7472 5f31 5f76 616c  child_attr_1_val
-00002500: 7565 270d 0a0d 0a0d 0a64 6566 2074 6573  ue'......def tes
-00002510: 745f 6d75 6c74 695f 6e65 7374 6564 5f65  t_multi_nested_e
-00002520: 6c65 6d65 6e74 5f6c 656e 6774 6828 636c  lement_length(cl
-00002530: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00002540: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
-00002550: 6572 7420 6c65 6e28 636c 6173 7379 5f78  ert len(classy_x
-00002560: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00002570: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00002580: 6d65 6e74 2920 3d3d 2032 0d0a 0d0a 0d0a  ment) == 2......
-00002590: 6465 6620 7465 7374 5f6d 756c 7469 5f6e  def test_multi_n
-000025a0: 6573 7465 645f 656c 656d 656e 745f 5f62  ested_element__b
-000025b0: 6173 6963 5f65 6c65 6d65 6e74 5f63 6869  asic_element_chi
-000025c0: 6c64 5f6c 656e 6774 6828 636c 6173 7379  ld_length(classy
-000025d0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-000025e0: 6529 3a0d 0a20 2020 2061 7373 6572 7420  e):..    assert 
-000025f0: 6c65 6e28 0d0a 2020 2020 2020 2020 636c  len(..        cl
-00002600: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00002610: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00002620: 6564 5f65 6c65 6d65 6e74 5b30 5d2e 6261  ed_element[0].ba
-00002630: 7369 635f 656c 656d 656e 745f 6368 696c  sic_element_chil
-00002640: 6429 203d 3d20 310d 0a20 2020 2061 7373  d) == 1..    ass
-00002650: 6572 7420 6c65 6e28 0d0a 2020 2020 2020  ert len(..      
-00002660: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
-00002670: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
-00002680: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b31  nested_element[1
-00002690: 5d2e 6261 7369 635f 656c 656d 656e 745f  ].basic_element_
-000026a0: 6368 696c 6429 203d 3d20 310d 0a0d 0a0d  child) == 1.....
-000026b0: 0a64 6566 2074 6573 745f 6d75 6c74 695f  .def test_multi_
-000026c0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5f5f  nested_element__
-000026d0: 6261 7369 635f 656c 656d 656e 745f 6368  basic_element_ch
-000026e0: 696c 645f 7465 7874 2863 6c61 7373 795f  ild_text(classy_
-000026f0: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00002700: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
-00002710: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00002720: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
-00002730: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
-00002740: 2020 2020 2020 305d 2e62 6173 6963 5f65        0].basic_e
-00002750: 6c65 6d65 6e74 5f63 6869 6c64 2e74 6578  lement_child.tex
-00002760: 7420 3d3d 2027 6261 7369 635f 656c 656d  t == 'basic_elem
-00002770: 656e 745f 6368 696c 645f 305f 7465 7874  ent_child_0_text
-00002780: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00002790: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-000027a0: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-000027b0: 6564 5f65 6c65 6d65 6e74 5b0d 0a20 2020  ed_element[..   
-000027c0: 2020 2020 2031 5d2e 6261 7369 635f 656c       1].basic_el
-000027d0: 656d 656e 745f 6368 696c 642e 7465 7874  ement_child.text
-000027e0: 203d 3d20 2762 6173 6963 5f65 6c65 6d65   == 'basic_eleme
-000027f0: 6e74 5f63 6869 6c64 5f31 5f74 6578 7427  nt_child_1_text'
-00002800: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f6d  ......def test_m
-00002810: 756c 7469 5f6e 6573 7465 645f 656c 656d  ulti_nested_elem
-00002820: 656e 745f 5f6d 756c 7469 5f65 6c65 6d65  ent__multi_eleme
-00002830: 6e74 5f63 6869 6c64 5f6c 656e 6774 6828  nt_child_length(
-00002840: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00002850: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
-00002860: 7373 6572 7420 6c65 6e28 0d0a 2020 2020  ssert len(..    
-00002870: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
-00002880: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00002890: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-000028a0: 5b30 5d2e 6d75 6c74 695f 656c 656d 656e  [0].multi_elemen
-000028b0: 745f 6368 696c 6429 203d 3d20 320d 0a20  t_child) == 2.. 
-000028c0: 2020 2061 7373 6572 7420 6c65 6e28 0d0a     assert len(..
-000028d0: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
-000028e0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-000028f0: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00002900: 6d65 6e74 5b31 5d2e 6d75 6c74 695f 656c  ment[1].multi_el
-00002910: 656d 656e 745f 6368 696c 6429 203d 3d20  ement_child) == 
-00002920: 320d 0a0d 0a0d 0a64 6566 2074 6573 745f  2......def test_
-00002930: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00002940: 6d65 6e74 5f5f 6d75 6c74 695f 656c 656d  ment__multi_elem
-00002950: 656e 745f 6368 696c 645f 7465 7874 2863  ent_child_text(c
-00002960: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00002970: 6978 7475 7265 293a 0d0a 2020 2020 6173  ixture):..    as
-00002980: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
-00002990: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
-000029a0: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
-000029b0: 745b 0d0a 2020 2020 2020 2020 305d 2e6d  t[..        0].m
-000029c0: 756c 7469 5f65 6c65 6d65 6e74 5f63 6869  ulti_element_chi
-000029d0: 6c64 5b30 5d2e 7465 7874 203d 3d20 276d  ld[0].text == 'm
-000029e0: 756c 7469 5f65 6c65 6d65 6e74 5f63 6869  ulti_element_chi
-000029f0: 6c64 5f30 5f74 6578 745f 3027 0d0a 2020  ld_0_text_0'..  
-00002a00: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-00002a10: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00002a20: 2e6d 756c 7469 5f6e 6573 7465 645f 656c  .multi_nested_el
-00002a30: 656d 656e 745b 0d0a 2020 2020 2020 2020  ement[..        
-00002a40: 305d 2e6d 756c 7469 5f65 6c65 6d65 6e74  0].multi_element
-00002a50: 5f63 6869 6c64 5b31 5d2e 7465 7874 203d  _child[1].text =
-00002a60: 3d20 276d 756c 7469 5f65 6c65 6d65 6e74  = 'multi_element
-00002a70: 5f63 6869 6c64 5f30 5f74 6578 745f 3127  _child_0_text_1'
-00002a80: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00002a90: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00002aa0: 7475 7265 2e6d 756c 7469 5f6e 6573 7465  ture.multi_neste
-00002ab0: 645f 656c 656d 656e 745b 0d0a 2020 2020  d_element[..    
-00002ac0: 2020 2020 315d 2e6d 756c 7469 5f65 6c65      1].multi_ele
-00002ad0: 6d65 6e74 5f63 6869 6c64 5b30 5d2e 7465  ment_child[0].te
-00002ae0: 7874 203d 3d20 276d 756c 7469 5f65 6c65  xt == 'multi_ele
-00002af0: 6d65 6e74 5f63 6869 6c64 5f31 5f74 6578  ment_child_1_tex
-00002b00: 745f 3027 0d0a 2020 2020 6173 7365 7274  t_0'..    assert
-00002b10: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
-00002b20: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
-00002b30: 6573 7465 645f 656c 656d 656e 745b 0d0a  ested_element[..
-00002b40: 2020 2020 2020 2020 315d 2e6d 756c 7469          1].multi
-00002b50: 5f65 6c65 6d65 6e74 5f63 6869 6c64 5b31  _element_child[1
-00002b60: 5d2e 7465 7874 203d 3d20 276d 756c 7469  ].text == 'multi
-00002b70: 5f65 6c65 6d65 6e74 5f63 6869 6c64 5f31  _element_child_1
-00002b80: 5f74 6578 745f 3127 0d0a 0d0a 0d0a 6465  _text_1'......de
-00002b90: 6620 7465 7374 5f6d 756c 7469 5f6e 6573  f test_multi_nes
-00002ba0: 7465 645f 656c 656d 656e 745f 5f65 6d70  ted_element__emp
-00002bb0: 7479 5f65 6c65 6d65 6e74 5f77 6974 685f  ty_element_with_
-00002bc0: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
-00002bd0: 5f6c 656e 6774 6828 636c 6173 7379 5f78  _length(classy_x
-00002be0: 6d6c 5f74 6573 745f 6669 7874 7572 6529  ml_test_fixture)
-00002bf0: 3a0d 0a20 2020 2061 7373 6572 7420 6c65  :..    assert le
-00002c00: 6e28 0d0a 2020 2020 2020 2020 636c 6173  n(..        clas
-00002c10: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
-00002c20: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
-00002c30: 5f65 6c65 6d65 6e74 5b30 5d2e 656d 7074  _element[0].empt
-00002c40: 795f 656c 656d 656e 745f 7769 7468 5f61  y_element_with_a
-00002c50: 7474 7269 6275 7465 735f 6368 696c 6429  ttributes_child)
-00002c60: 203d 3d20 310d 0a20 2020 2061 7373 6572   == 1..    asser
-00002c70: 7420 6c65 6e28 0d0a 2020 2020 2020 2020  t len(..        
-00002c80: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00002c90: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
-00002ca0: 7374 6564 5f65 6c65 6d65 6e74 5b31 5d2e  sted_element[1].
-00002cb0: 656d 7074 795f 656c 656d 656e 745f 7769  empty_element_wi
-00002cc0: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-00002cd0: 696c 6429 203d 3d20 310d 0a0d 0a0d 0a64  ild) == 1......d
-00002ce0: 6566 2074 6573 745f 6d75 6c74 695f 6e65  ef test_multi_ne
-00002cf0: 7374 6564 5f65 6c65 6d65 6e74 5f5f 656d  sted_element__em
-00002d00: 7074 795f 656c 656d 656e 745f 7769 7468  pty_element_with
-00002d10: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00002d20: 645f 7465 7874 2863 6c61 7373 795f 786d  d_text(classy_xm
-00002d30: 6c5f 7465 7374 5f66 6978 7475 7265 293a  l_test_fixture):
-00002d40: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00002d50: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00002d60: 7475 7265 2e6d 756c 7469 5f6e 6573 7465  ture.multi_neste
-00002d70: 645f 656c 656d 656e 745b 0d0a 2020 2020  d_element[..    
-00002d80: 2020 2020 305d 2e65 6d70 7479 5f65 6c65      0].empty_ele
-00002d90: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-00002da0: 7574 6573 5f63 6869 6c64 2e74 6578 7420  utes_child.text 
-00002db0: 6973 204e 6f6e 650d 0a20 2020 2061 7373  is None..    ass
-00002dc0: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00002dd0: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00002de0: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-00002df0: 5b0d 0a20 2020 2020 2020 2031 5d2e 656d  [..        1].em
-00002e00: 7074 795f 656c 656d 656e 745f 7769 7468  pty_element_with
-00002e10: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00002e20: 642e 7465 7874 2069 7320 4e6f 6e65 0d0a  d.text is None..
-00002e30: 0d0a 0d0a 6465 6620 7465 7374 5f6d 756c  ....def test_mul
-00002e40: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
-00002e50: 745f 5f65 6d70 7479 5f65 6c65 6d65 6e74  t__empty_element
-00002e60: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00002e70: 5f63 6869 6c64 5f61 7474 7269 6275 7465  _child_attribute
-00002e80: 7328 636c 6173 7379 5f78 6d6c 5f74 6573  s(classy_xml_tes
-00002e90: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00002ea0: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00002eb0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00002ec0: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00002ed0: 6d65 6e74 5b0d 0a20 2020 2020 2020 2030  ment[..        0
-00002ee0: 5d2e 656d 7074 795f 656c 656d 656e 745f  ].empty_element_
-00002ef0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00002f00: 6368 696c 642e 6e61 6d65 203d 3d20 2763  child.name == 'c
-00002f10: 6869 6c64 5f30 5f61 7474 725f 6e61 6d65  hild_0_attr_name
-00002f20: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00002f30: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00002f40: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00002f50: 6564 5f65 6c65 6d65 6e74 5b0d 0a20 2020  ed_element[..   
-00002f60: 2020 2020 2030 5d2e 656d 7074 795f 656c       0].empty_el
-00002f70: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00002f80: 6275 7465 735f 6368 696c 642e 7661 6c75  butes_child.valu
-00002f90: 6520 3d3d 2027 6368 696c 645f 305f 6174  e == 'child_0_at
-00002fa0: 7472 5f76 616c 7565 270d 0a20 2020 2061  tr_value'..    a
-00002fb0: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00002fc0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
-00002fd0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
-00002fe0: 6e74 5b0d 0a20 2020 2020 2020 2031 5d2e  nt[..        1].
-00002ff0: 656d 7074 795f 656c 656d 656e 745f 7769  empty_element_wi
-00003000: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-00003010: 696c 642e 6e61 6d65 203d 3d20 2763 6869  ild.name == 'chi
-00003020: 6c64 5f31 5f61 7474 725f 6e61 6d65 270d  ld_1_attr_name'.
-00003030: 0a20 2020 2061 7373 6572 7420 636c 6173  .    assert clas
-00003040: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
-00003050: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
-00003060: 5f65 6c65 6d65 6e74 5b0d 0a20 2020 2020  _element[..     
-00003070: 2020 2031 5d2e 656d 7074 795f 656c 656d     1].empty_elem
-00003080: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00003090: 7465 735f 6368 696c 642e 7661 6c75 6520  tes_child.value 
-000030a0: 3d3d 2027 6368 696c 645f 315f 6174 7472  == 'child_1_attr
-000030b0: 5f76 616c 7565 270d 0a0d 0a0d 0a64 6566  _value'......def
-000030c0: 2074 6573 745f 6d75 6c74 695f 6e65 7374   test_multi_nest
-000030d0: 6564 5f65 6c65 6d65 6e74 5f5f 656d 7074  ed_element__empt
-000030e0: 795f 6d75 6c74 695f 656c 656d 656e 745f  y_multi_element_
-000030f0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00003100: 6368 696c 645f 6c65 6e67 7468 2863 6c61  child_length(cla
-00003110: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00003120: 7475 7265 293a 0d0a 2020 2020 6173 7365  ture):..    asse
-00003130: 7274 206c 656e 280d 0a20 2020 2020 2020  rt len(..       
-00003140: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
-00003150: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
-00003160: 6573 7465 645f 656c 656d 656e 745b 305d  ested_element[0]
-00003170: 2e65 6d70 7479 5f6d 756c 7469 5f65 6c65  .empty_multi_ele
-00003180: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
-00003190: 7574 6573 5f63 6869 6c64 2920 3d3d 2032  utes_child) == 2
-000031a0: 0d0a 2020 2020 6173 7365 7274 206c 656e  ..    assert len
-000031b0: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
-000031c0: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-000031d0: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
-000031e0: 656c 656d 656e 745b 315d 2e65 6d70 7479  element[1].empty
-000031f0: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
-00003200: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-00003210: 6869 6c64 2920 3d3d 2032 0d0a 0d0a 0d0a  hild) == 2......
-00003220: 6465 6620 7465 7374 5f6d 756c 7469 5f6e  def test_multi_n
-00003230: 6573 7465 645f 656c 656d 656e 745f 5f65  ested_element__e
-00003240: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
-00003250: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00003260: 6573 5f63 6869 6c64 5f74 6578 7428 636c  es_child_text(cl
-00003270: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00003280: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
-00003290: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-000032a0: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-000032b0: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-000032c0: 5b30 5d2e 656d 7074 795f 6d75 6c74 695f  [0].empty_multi_
-000032d0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-000032e0: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-000032f0: 2020 2020 2020 2020 305d 2e74 6578 7420          0].text 
-00003300: 6973 204e 6f6e 650d 0a20 2020 2061 7373  is None..    ass
-00003310: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00003320: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00003330: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-00003340: 5b30 5d2e 656d 7074 795f 6d75 6c74 695f  [0].empty_multi_
-00003350: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00003360: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-00003370: 2020 2020 2020 2020 315d 2e74 6578 7420          1].text 
-00003380: 6973 204e 6f6e 650d 0a20 2020 2061 7373  is None..    ass
-00003390: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-000033a0: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-000033b0: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-000033c0: 5b31 5d2e 656d 7074 795f 6d75 6c74 695f  [1].empty_multi_
-000033d0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-000033e0: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-000033f0: 2020 2020 2020 2020 305d 2e74 6578 7420          0].text 
-00003400: 6973 204e 6f6e 650d 0a20 2020 2061 7373  is None..    ass
-00003410: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00003420: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00003430: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-00003440: 5b31 5d2e 656d 7074 795f 6d75 6c74 695f  [1].empty_multi_
-00003450: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00003460: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-00003470: 2020 2020 2020 2020 315d 2e74 6578 7420          1].text 
-00003480: 6973 204e 6f6e 650d 0a0d 0a0d 0a64 6566  is None......def
-00003490: 2074 6573 745f 6d75 6c74 695f 6e65 7374   test_multi_nest
-000034a0: 6564 5f65 6c65 6d65 6e74 5f5f 656d 7074  ed_element__empt
-000034b0: 795f 6d75 6c74 695f 656c 656d 656e 745f  y_multi_element_
-000034c0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-000034d0: 6368 696c 645f 6174 7472 6962 7574 6573  child_attributes
-000034e0: 2863 6c61 7373 795f 786d 6c5f 7465 7374  (classy_xml_test
-000034f0: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-00003500: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
-00003510: 6c5f 7465 7374 5f66 6978 7475 7265 2e6d  l_test_fixture.m
-00003520: 756c 7469 5f6e 6573 7465 645f 656c 656d  ulti_nested_elem
-00003530: 656e 745b 305d 2e65 6d70 7479 5f6d 756c  ent[0].empty_mul
-00003540: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
-00003550: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
-00003560: 5b0d 0a20 2020 2020 2020 2030 5d2e 6e61  [..        0].na
-00003570: 6d65 203d 3d20 2763 6869 6c64 5f30 5f61  me == 'child_0_a
-00003580: 7474 725f 305f 6e61 6d65 270d 0a20 2020  ttr_0_name'..   
-00003590: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-000035a0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-000035b0: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-000035c0: 6d65 6e74 5b30 5d2e 656d 7074 795f 6d75  ment[0].empty_mu
-000035d0: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
-000035e0: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-000035f0: 645b 0d0a 2020 2020 2020 2020 305d 2e76  d[..        0].v
-00003600: 616c 7565 203d 3d20 2763 6869 6c64 5f30  alue == 'child_0
-00003610: 5f61 7474 725f 305f 7661 6c75 6527 0d0a  _attr_0_value'..
-00003620: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-00003630: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00003640: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
-00003650: 656c 656d 656e 745b 305d 2e65 6d70 7479  element[0].empty
-00003660: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
-00003670: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-00003680: 6869 6c64 5b0d 0a20 2020 2020 2020 2031  hild[..        1
-00003690: 5d2e 6e61 6d65 203d 3d20 2763 6869 6c64  ].name == 'child
-000036a0: 5f30 5f61 7474 725f 315f 6e61 6d65 270d  _0_attr_1_name'.
-000036b0: 0a20 2020 2061 7373 6572 7420 636c 6173  .    assert clas
-000036c0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
-000036d0: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
-000036e0: 5f65 6c65 6d65 6e74 5b30 5d2e 656d 7074  _element[0].empt
-000036f0: 795f 6d75 6c74 695f 656c 656d 656e 745f  y_multi_element_
-00003700: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00003710: 6368 696c 645b 0d0a 2020 2020 2020 2020  child[..        
-00003720: 315d 2e76 616c 7565 203d 3d20 2763 6869  1].value == 'chi
-00003730: 6c64 5f30 5f61 7474 725f 315f 7661 6c75  ld_0_attr_1_valu
-00003740: 6527 0d0a 2020 2020 6173 7365 7274 2063  e'..    assert c
-00003750: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00003760: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
-00003770: 7465 645f 656c 656d 656e 745b 315d 2e65  ted_element[1].e
-00003780: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
-00003790: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-000037a0: 6573 5f63 6869 6c64 5b0d 0a20 2020 2020  es_child[..     
-000037b0: 2020 2030 5d2e 6e61 6d65 203d 3d20 2763     0].name == 'c
-000037c0: 6869 6c64 5f31 5f61 7474 725f 305f 6e61  hild_1_attr_0_na
-000037d0: 6d65 270d 0a20 2020 2061 7373 6572 7420  me'..    assert 
-000037e0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-000037f0: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
-00003800: 7374 6564 5f65 6c65 6d65 6e74 5b31 5d2e  sted_element[1].
-00003810: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
-00003820: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00003830: 7465 735f 6368 696c 645b 0d0a 2020 2020  tes_child[..    
-00003840: 2020 2020 305d 2e76 616c 7565 203d 3d20      0].value == 
-00003850: 2763 6869 6c64 5f31 5f61 7474 725f 305f  'child_1_attr_0_
-00003860: 7661 6c75 6527 0d0a 2020 2020 6173 7365  value'..    asse
-00003870: 7274 2063 6c61 7373 795f 786d 6c5f 7465  rt classy_xml_te
-00003880: 7374 5f66 6978 7475 7265 2e6d 756c 7469  st_fixture.multi
-00003890: 5f6e 6573 7465 645f 656c 656d 656e 745b  _nested_element[
-000038a0: 315d 2e65 6d70 7479 5f6d 756c 7469 5f65  1].empty_multi_e
-000038b0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-000038c0: 6962 7574 6573 5f63 6869 6c64 5b0d 0a20  ibutes_child[.. 
-000038d0: 2020 2020 2020 2031 5d2e 6e61 6d65 203d         1].name =
-000038e0: 3d20 2763 6869 6c64 5f31 5f61 7474 725f  = 'child_1_attr_
-000038f0: 315f 6e61 6d65 270d 0a20 2020 2061 7373  1_name'..    ass
-00003900: 6572 7420 636c 6173 7379 5f78 6d6c 5f74  ert classy_xml_t
-00003910: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
-00003920: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
-00003930: 5b31 5d2e 656d 7074 795f 6d75 6c74 695f  [1].empty_multi_
-00003940: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00003950: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-00003960: 2020 2020 2020 2020 315d 2e76 616c 7565          1].value
-00003970: 203d 3d20 2763 6869 6c64 5f31 5f61 7474   == 'child_1_att
-00003980: 725f 315f 7661 6c75 6527 0d0a 0d0a 0d0a  r_1_value'......
-00003990: 6465 6620 7465 7374 5f6d 756c 7469 5f6e  def test_multi_n
-000039a0: 6573 7465 645f 656c 656d 656e 745f 5f62  ested_element__b
-000039b0: 6173 6963 5f65 6c65 6d65 6e74 5f77 6974  asic_element_wit
-000039c0: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-000039d0: 6c64 5f6c 656e 6774 6828 636c 6173 7379  ld_length(classy
-000039e0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-000039f0: 6529 3a0d 0a20 2020 2061 7373 6572 7420  e):..    assert 
-00003a00: 6c65 6e28 0d0a 2020 2020 2020 2020 636c  len(..        cl
-00003a10: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00003a20: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00003a30: 6564 5f65 6c65 6d65 6e74 5b30 5d2e 6261  ed_element[0].ba
-00003a40: 7369 635f 656c 656d 656e 745f 7769 7468  sic_element_with
-00003a50: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00003a60: 6429 203d 3d20 310d 0a20 2020 2061 7373  d) == 1..    ass
-00003a70: 6572 7420 6c65 6e28 0d0a 2020 2020 2020  ert len(..      
-00003a80: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
-00003a90: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
-00003aa0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b31  nested_element[1
-00003ab0: 5d2e 6261 7369 635f 656c 656d 656e 745f  ].basic_element_
-00003ac0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00003ad0: 6368 696c 6429 203d 3d20 310d 0a0d 0a0d  child) == 1.....
-00003ae0: 0a64 6566 2074 6573 745f 6d75 6c74 695f  .def test_multi_
-00003af0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5f5f  nested_element__
-00003b00: 6261 7369 635f 656c 656d 656e 745f 7769  basic_element_wi
-00003b10: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-00003b20: 696c 645f 7465 7874 2863 6c61 7373 795f  ild_text(classy_
-00003b30: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00003b40: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
-00003b50: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
-00003b60: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
-00003b70: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
-00003b80: 2020 2020 2020 305d 2e62 6173 6963 5f65        0].basic_e
-00003b90: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
-00003ba0: 6962 7574 6573 5f63 6869 6c64 2e74 6578  ibutes_child.tex
-00003bb0: 7420 3d3d 2027 6261 7369 635f 656c 656d  t == 'basic_elem
-00003bc0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00003bd0: 7465 735f 6368 696c 645f 305f 7465 7874  tes_child_0_text
-00003be0: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00003bf0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00003c00: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00003c10: 6564 5f65 6c65 6d65 6e74 5b0d 0a20 2020  ed_element[..   
-00003c20: 2020 2020 2031 5d2e 6261 7369 635f 656c       1].basic_el
-00003c30: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00003c40: 6275 7465 735f 6368 696c 642e 7465 7874  butes_child.text
-00003c50: 203d 3d20 2762 6173 6963 5f65 6c65 6d65   == 'basic_eleme
-00003c60: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00003c70: 6573 5f63 6869 6c64 5f31 5f74 6578 7427  es_child_1_text'
-00003c80: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f6d  ......def test_m
-00003c90: 756c 7469 5f6e 6573 7465 645f 656c 656d  ulti_nested_elem
-00003ca0: 656e 745f 5f62 6173 6963 5f65 6c65 6d65  ent__basic_eleme
-00003cb0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
-00003cc0: 6573 5f63 6869 6c64 5f61 7474 7269 6275  es_child_attribu
-00003cd0: 7465 7328 636c 6173 7379 5f78 6d6c 5f74  tes(classy_xml_t
-00003ce0: 6573 745f 6669 7874 7572 6529 3a0d 0a20  est_fixture):.. 
-00003cf0: 2020 2061 7373 6572 7420 636c 6173 7379     assert classy
-00003d00: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-00003d10: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
-00003d20: 6c65 6d65 6e74 5b0d 0a20 2020 2020 2020  lement[..       
-00003d30: 2030 5d2e 6261 7369 635f 656c 656d 656e   0].basic_elemen
-00003d40: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-00003d50: 735f 6368 696c 642e 6e61 6d65 203d 3d20  s_child.name == 
-00003d60: 2763 6869 6c64 5f30 5f61 7474 725f 6e61  'child_0_attr_na
-00003d70: 6d65 270d 0a20 2020 2061 7373 6572 7420  me'..    assert 
-00003d80: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
-00003d90: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
-00003da0: 7374 6564 5f65 6c65 6d65 6e74 5b0d 0a20  sted_element[.. 
-00003db0: 2020 2020 2020 2030 5d2e 6261 7369 635f         0].basic_
-00003dc0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00003dd0: 7269 6275 7465 735f 6368 696c 642e 7661  ributes_child.va
-00003de0: 6c75 6520 3d3d 2027 6368 696c 645f 305f  lue == 'child_0_
-00003df0: 6174 7472 5f76 616c 7565 270d 0a20 2020  attr_value'..   
-00003e00: 2061 7373 6572 7420 636c 6173 7379 5f78   assert classy_x
-00003e10: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
-00003e20: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00003e30: 6d65 6e74 5b0d 0a20 2020 2020 2020 2031  ment[..        1
-00003e40: 5d2e 6261 7369 635f 656c 656d 656e 745f  ].basic_element_
-00003e50: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-00003e60: 6368 696c 642e 6e61 6d65 203d 3d20 2763  child.name == 'c
-00003e70: 6869 6c64 5f31 5f61 7474 725f 6e61 6d65  hild_1_attr_name
-00003e80: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00003e90: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00003ea0: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00003eb0: 6564 5f65 6c65 6d65 6e74 5b0d 0a20 2020  ed_element[..   
-00003ec0: 2020 2020 2031 5d2e 6261 7369 635f 656c       1].basic_el
-00003ed0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00003ee0: 6275 7465 735f 6368 696c 642e 7661 6c75  butes_child.valu
-00003ef0: 6520 3d3d 2027 6368 696c 645f 315f 6174  e == 'child_1_at
-00003f00: 7472 5f76 616c 7565 270d 0a0d 0a0d 0a64  tr_value'......d
-00003f10: 6566 2074 6573 745f 6d75 6c74 695f 6e65  ef test_multi_ne
-00003f20: 7374 6564 5f65 6c65 6d65 6e74 5f5f 6d75  sted_element__mu
-00003f30: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
-00003f40: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00003f50: 645f 6c65 6e67 7468 2863 6c61 7373 795f  d_length(classy_
-00003f60: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
-00003f70: 293a 0d0a 2020 2020 6173 7365 7274 206c  ):..    assert l
-00003f80: 656e 280d 0a20 2020 2020 2020 2063 6c61  en(..        cla
-00003f90: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
-00003fa0: 7475 7265 2e6d 756c 7469 5f6e 6573 7465  ture.multi_neste
-00003fb0: 645f 656c 656d 656e 745b 305d 2e6d 756c  d_element[0].mul
-00003fc0: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
-00003fd0: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
-00003fe0: 2920 3d3d 2032 0d0a 2020 2020 6173 7365  ) == 2..    asse
-00003ff0: 7274 206c 656e 280d 0a20 2020 2020 2020  rt len(..       
-00004000: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
-00004010: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
-00004020: 6573 7465 645f 656c 656d 656e 745b 315d  ested_element[1]
-00004030: 2e6d 756c 7469 5f65 6c65 6d65 6e74 5f77  .multi_element_w
-00004040: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
-00004050: 6869 6c64 2920 3d3d 2032 0d0a 0d0a 0d0a  hild) == 2......
-00004060: 6465 6620 7465 7374 5f6d 756c 7469 5f6e  def test_multi_n
-00004070: 6573 7465 645f 656c 656d 656e 745f 5f6d  ested_element__m
-00004080: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
-00004090: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
-000040a0: 6c64 5f74 6578 7428 636c 6173 7379 5f78  ld_text(classy_x
-000040b0: 6d6c 5f74 6573 745f 6669 7874 7572 6529  ml_test_fixture)
-000040c0: 3a0d 0a20 2020 2061 7373 6572 7420 636c  :..    assert cl
-000040d0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-000040e0: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-000040f0: 6564 5f65 6c65 6d65 6e74 5b30 5d2e 6d75  ed_element[0].mu
-00004100: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
-00004110: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-00004120: 645b 0d0a 2020 2020 2020 2020 305d 2e74  d[..        0].t
-00004130: 6578 7420 3d3d 2027 6d75 6c74 695f 656c  ext == 'multi_el
-00004140: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
-00004150: 6275 7465 735f 6368 696c 645f 305f 7465  butes_child_0_te
-00004160: 7874 5f30 270d 0a20 2020 2061 7373 6572  xt_0'..    asser
-00004170: 7420 636c 6173 7379 5f78 6d6c 5f74 6573  t classy_xml_tes
-00004180: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
-00004190: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b30  nested_element[0
-000041a0: 5d2e 6d75 6c74 695f 656c 656d 656e 745f  ].multi_element_
-000041b0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
-000041c0: 6368 696c 645b 0d0a 2020 2020 2020 2020  child[..        
-000041d0: 315d 2e74 6578 7420 3d3d 2027 6d75 6c74  1].text == 'mult
-000041e0: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
-000041f0: 7474 7269 6275 7465 735f 6368 696c 645f  ttributes_child_
-00004200: 305f 7465 7874 5f31 270d 0a20 2020 2061  0_text_1'..    a
-00004210: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00004220: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
-00004230: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
-00004240: 6e74 5b31 5d2e 6d75 6c74 695f 656c 656d  nt[1].multi_elem
-00004250: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00004260: 7465 735f 6368 696c 645b 0d0a 2020 2020  tes_child[..    
-00004270: 2020 2020 305d 2e74 6578 7420 3d3d 2027      0].text == '
-00004280: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
-00004290: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
-000042a0: 696c 645f 315f 7465 7874 5f30 270d 0a20  ild_1_text_0'.. 
-000042b0: 2020 2061 7373 6572 7420 636c 6173 7379     assert classy
-000042c0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-000042d0: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
-000042e0: 6c65 6d65 6e74 5b31 5d2e 6d75 6c74 695f  lement[1].multi_
-000042f0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
-00004300: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
-00004310: 2020 2020 2020 2020 315d 2e74 6578 7420          1].text 
-00004320: 3d3d 2027 6d75 6c74 695f 656c 656d 656e  == 'multi_elemen
-00004330: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
-00004340: 735f 6368 696c 645f 315f 7465 7874 5f31  s_child_1_text_1
-00004350: 270d 0a0d 0a0d 0a64 6566 2074 6573 745f  '......def test_
-00004360: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
-00004370: 6d65 6e74 5f5f 6d75 6c74 695f 656c 656d  ment__multi_elem
-00004380: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-00004390: 7465 735f 6368 696c 645f 6174 7472 6962  tes_child_attrib
-000043a0: 7574 6573 2863 6c61 7373 795f 786d 6c5f  utes(classy_xml_
-000043b0: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
-000043c0: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-000043d0: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-000043e0: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
-000043f0: 656c 656d 656e 745b 305d 2e6d 756c 7469  element[0].multi
-00004400: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
-00004410: 7472 6962 7574 6573 5f63 6869 6c64 5b0d  tributes_child[.
-00004420: 0a20 2020 2020 2020 2030 5d2e 6e61 6d65  .        0].name
-00004430: 203d 3d20 2763 6869 6c64 5f30 5f61 7474   == 'child_0_att
-00004440: 725f 305f 6e61 6d65 270d 0a20 2020 2061  r_0_name'..    a
-00004450: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00004460: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
-00004470: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
-00004480: 6e74 5b30 5d2e 6d75 6c74 695f 656c 656d  nt[0].multi_elem
-00004490: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-000044a0: 7465 735f 6368 696c 645b 0d0a 2020 2020  tes_child[..    
-000044b0: 2020 2020 305d 2e76 616c 7565 203d 3d20      0].value == 
-000044c0: 2763 6869 6c64 5f30 5f61 7474 725f 305f  'child_0_attr_0_
-000044d0: 7661 6c75 6527 0d0a 2020 2020 6173 7365  value'..    asse
-000044e0: 7274 2063 6c61 7373 795f 786d 6c5f 7465  rt classy_xml_te
-000044f0: 7374 5f66 6978 7475 7265 2e6d 756c 7469  st_fixture.multi
-00004500: 5f6e 6573 7465 645f 656c 656d 656e 745b  _nested_element[
-00004510: 305d 2e6d 756c 7469 5f65 6c65 6d65 6e74  0].multi_element
-00004520: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00004530: 5f63 6869 6c64 5b0d 0a20 2020 2020 2020  _child[..       
-00004540: 2031 5d2e 6e61 6d65 203d 3d20 2763 6869   1].name == 'chi
-00004550: 6c64 5f30 5f61 7474 725f 315f 6e61 6d65  ld_0_attr_1_name
-00004560: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-00004570: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-00004580: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-00004590: 6564 5f65 6c65 6d65 6e74 5b30 5d2e 6d75  ed_element[0].mu
-000045a0: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
-000045b0: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-000045c0: 645b 0d0a 2020 2020 2020 2020 315d 2e76  d[..        1].v
-000045d0: 616c 7565 203d 3d20 2763 6869 6c64 5f30  alue == 'child_0
-000045e0: 5f61 7474 725f 315f 7661 6c75 6527 0d0a  _attr_1_value'..
-000045f0: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-00004600: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
-00004610: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
-00004620: 656c 656d 656e 745b 315d 2e6d 756c 7469  element[1].multi
-00004630: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
-00004640: 7472 6962 7574 6573 5f63 6869 6c64 5b0d  tributes_child[.
-00004650: 0a20 2020 2020 2020 2030 5d2e 6e61 6d65  .        0].name
-00004660: 203d 3d20 2763 6869 6c64 5f31 5f61 7474   == 'child_1_att
-00004670: 725f 305f 6e61 6d65 270d 0a20 2020 2061  r_0_name'..    a
-00004680: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00004690: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
-000046a0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
-000046b0: 6e74 5b31 5d2e 6d75 6c74 695f 656c 656d  nt[1].multi_elem
-000046c0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
-000046d0: 7465 735f 6368 696c 645b 0d0a 2020 2020  tes_child[..    
-000046e0: 2020 2020 305d 2e76 616c 7565 203d 3d20      0].value == 
-000046f0: 2763 6869 6c64 5f31 5f61 7474 725f 305f  'child_1_attr_0_
-00004700: 7661 6c75 6527 0d0a 2020 2020 6173 7365  value'..    asse
-00004710: 7274 2063 6c61 7373 795f 786d 6c5f 7465  rt classy_xml_te
-00004720: 7374 5f66 6978 7475 7265 2e6d 756c 7469  st_fixture.multi
-00004730: 5f6e 6573 7465 645f 656c 656d 656e 745b  _nested_element[
-00004740: 315d 2e6d 756c 7469 5f65 6c65 6d65 6e74  1].multi_element
-00004750: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
-00004760: 5f63 6869 6c64 5b0d 0a20 2020 2020 2020  _child[..       
-00004770: 2031 5d2e 6e61 6d65 203d 3d20 2763 6869   1].name == 'chi
-00004780: 6c64 5f31 5f61 7474 725f 315f 6e61 6d65  ld_1_attr_1_name
-00004790: 270d 0a20 2020 2061 7373 6572 7420 636c  '..    assert cl
-000047a0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
-000047b0: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
-000047c0: 6564 5f65 6c65 6d65 6e74 5b31 5d2e 6d75  ed_element[1].mu
-000047d0: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
-000047e0: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
-000047f0: 645b 0d0a 2020 2020 2020 2020 315d 2e76  d[..        1].v
-00004800: 616c 7565 203d 3d20 2763 6869 6c64 5f31  alue == 'child_1
-00004810: 5f61 7474 725f 315f 7661 6c75 6527 0d0a  _attr_1_value'..
-00004820: 0d0a 0d0a 6465 6620 7465 7374 5f6d 756c  ....def test_mul
-00004830: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
-00004840: 745f 5f75 6e69 7175 655f 656c 656d 656e  t__unique_elemen
-00004850: 745f 6368 696c 645f 6578 6973 7465 6e63  t_child_existenc
-00004860: 6528 636c 6173 7379 5f78 6d6c 5f74 6573  e(classy_xml_tes
-00004870: 745f 6669 7874 7572 6529 3a0d 0a20 2020  t_fixture):..   
-00004880: 2061 7373 6572 7420 6861 7361 7474 7228   assert hasattr(
-00004890: 0d0a 2020 2020 2020 2020 636c 6173 7379  ..        classy
-000048a0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
-000048b0: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
-000048c0: 6c65 6d65 6e74 5b30 5d2c 2027 756e 6971  lement[0], 'uniq
-000048d0: 7565 5f65 6c65 6d65 6e74 5f63 6869 6c64  ue_element_child
-000048e0: 2729 0d0a 2020 2020 6173 7365 7274 206e  ')..    assert n
-000048f0: 6f74 2068 6173 6174 7472 280d 0a20 2020  ot hasattr(..   
-00004900: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
-00004910: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
-00004920: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
-00004930: 745b 315d 2c20 2775 6e69 7175 655f 656c  t[1], 'unique_el
-00004940: 656d 656e 745f 6368 696c 6427 290d 0a0d  ement_child')...
-00004950: 0a0d 0a64 6566 2074 6573 745f 636c 6173  ...def test_clas
-00004960: 7379 5f78 6d6c 5f61 6464 5f65 6c65 6d65  sy_xml_add_eleme
-00004970: 6e74 2863 6c61 7373 795f 786d 6c5f 656d  nt(classy_xml_em
-00004980: 7074 795f 6669 7874 7572 6529 3a0d 0a20  pty_fixture):.. 
-00004990: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-000049a0: 7074 795f 6669 7874 7572 652e 7465 7374  pty_fixture.test
-000049b0: 5f65 6c65 6d65 6e74 203d 2058 6d6c 456c  _element = XmlEl
-000049c0: 656d 656e 7428 290d 0a20 2020 2061 7373  ement()..    ass
-000049d0: 6572 7420 6973 696e 7374 616e 6365 2863  ert isinstance(c
-000049e0: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-000049f0: 6669 7874 7572 652e 7465 7374 5f65 6c65  fixture.test_ele
-00004a00: 6d65 6e74 2c20 586d 6c45 6c65 6d65 6e74  ment, XmlElement
-00004a10: 290d 0a0d 0a0d 0a64 6566 2074 6573 745f  )......def test_
-00004a20: 636c 6173 7379 5f78 6d6c 5f72 656d 6f76  classy_xml_remov
-00004a30: 655f 656c 656d 656e 7428 636c 6173 7379  e_element(classy
-00004a40: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00004a50: 7265 293a 0d0a 2020 2020 636c 6173 7379  re):..    classy
-00004a60: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00004a70: 7265 2e74 6573 745f 656c 656d 656e 7420  re.test_element 
-00004a80: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
-00004a90: 2020 2020 6465 6c20 636c 6173 7379 5f78      del classy_x
-00004aa0: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
-00004ab0: 2e74 6573 745f 656c 656d 656e 740d 0a20  .test_element.. 
-00004ac0: 2020 2061 7373 6572 7420 6e6f 7420 6861     assert not ha
-00004ad0: 7361 7474 7228 636c 6173 7379 5f78 6d6c  sattr(classy_xml
-00004ae0: 5f65 6d70 7479 5f66 6978 7475 7265 2c20  _empty_fixture, 
-00004af0: 2774 6573 745f 656c 656d 656e 7427 290d  'test_element').
-00004b00: 0a0d 0a0d 0a64 6566 2074 6573 745f 636c  .....def test_cl
-00004b10: 6173 7379 5f78 6d6c 5f61 6464 5f65 6c65  assy_xml_add_ele
-00004b20: 6d65 6e74 5f61 7272 6179 2863 6c61 7373  ment_array(class
-00004b30: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004b40: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
-00004b50: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004b60: 7572 652e 7465 7374 5f65 6c65 6d65 6e74  ure.test_element
-00004b70: 5f61 7272 6179 203d 2058 6d6c 456c 656d  _array = XmlElem
-00004b80: 656e 7428 290d 0a20 2020 2063 6c61 7373  ent()..    class
-00004b90: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004ba0: 7572 652e 7465 7374 5f65 6c65 6d65 6e74  ure.test_element
-00004bb0: 5f61 7272 6179 203d 2058 6d6c 456c 656d  _array = XmlElem
-00004bc0: 656e 7428 290d 0a20 2020 2061 7373 6572  ent()..    asser
-00004bd0: 7420 6973 696e 7374 616e 6365 280d 0a20  t isinstance(.. 
-00004be0: 2020 2020 2020 2063 6c61 7373 795f 786d         classy_xm
-00004bf0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00004c00: 7465 7374 5f65 6c65 6d65 6e74 5f61 7272  test_element_arr
-00004c10: 6179 5b30 5d2c 2058 6d6c 456c 656d 656e  ay[0], XmlElemen
-00004c20: 7429 0d0a 2020 2020 6173 7365 7274 2069  t)..    assert i
-00004c30: 7369 6e73 7461 6e63 6528 0d0a 2020 2020  sinstance(..    
-00004c40: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-00004c50: 6d70 7479 5f66 6978 7475 7265 2e74 6573  mpty_fixture.tes
-00004c60: 745f 656c 656d 656e 745f 6172 7261 795b  t_element_array[
-00004c70: 315d 2c20 586d 6c45 6c65 6d65 6e74 290d  1], XmlElement).
-00004c80: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
-00004c90: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00004ca0: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
-00004cb0: 656d 656e 745f 6172 7261 7929 203d 3d20  ement_array) == 
-00004cc0: 320d 0a0d 0a0d 0a64 6566 2074 6573 745f  2......def test_
-00004cd0: 636c 6173 7379 5f78 6d6c 5f72 656d 6f76  classy_xml_remov
-00004ce0: 655f 656c 656d 656e 745f 6172 7261 7928  e_element_array(
-00004cf0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00004d00: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-00004d10: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00004d20: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
-00004d30: 656d 656e 745f 6172 7261 7920 3d20 586d  ement_array = Xm
-00004d40: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
-00004d50: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00004d60: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
-00004d70: 656d 656e 745f 6172 7261 7920 3d20 586d  ement_array = Xm
-00004d80: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
-00004d90: 6465 6c20 636c 6173 7379 5f78 6d6c 5f65  del classy_xml_e
-00004da0: 6d70 7479 5f66 6978 7475 7265 2e74 6573  mpty_fixture.tes
-00004db0: 745f 656c 656d 656e 745f 6172 7261 795b  t_element_array[
-00004dc0: 305d 0d0a 2020 2020 6173 7365 7274 2069  0]..    assert i
-00004dd0: 7369 6e73 7461 6e63 6528 636c 6173 7379  sinstance(classy
-00004de0: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00004df0: 7265 2e74 6573 745f 656c 656d 656e 745f  re.test_element_
-00004e00: 6172 7261 792c 2058 6d6c 456c 656d 656e  array, XmlElemen
-00004e10: 7429 0d0a 2020 2020 6173 7365 7274 206c  t)..    assert l
-00004e20: 656e 2863 6c61 7373 795f 786d 6c5f 656d  en(classy_xml_em
-00004e30: 7074 795f 6669 7874 7572 652e 7465 7374  pty_fixture.test
-00004e40: 5f65 6c65 6d65 6e74 5f61 7272 6179 2920  _element_array) 
-00004e50: 3d3d 2031 0d0a 0d0a 0d0a 6465 6620 7465  == 1......def te
-00004e60: 7374 5f78 6d6c 5f65 6c65 6d65 6e74 5f61  st_xml_element_a
-00004e70: 6464 5f65 6c65 6d65 6e74 2863 6c61 7373  dd_element(class
-00004e80: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004e90: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
-00004ea0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004eb0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00004ec0: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
-00004ed0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-00004ee0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00004ef0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-00004f00: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
-00004f10: 456c 656d 656e 7428 290d 0a20 2020 2061  Element()..    a
-00004f20: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-00004f30: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
-00004f40: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00004f50: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00004f60: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 2c20  nt.xml_element, 
-00004f70: 586d 6c45 6c65 6d65 6e74 290d 0a0d 0a0d  XmlElement).....
-00004f80: 0a64 6566 2074 6573 745f 786d 6c5f 656c  .def test_xml_el
-00004f90: 656d 656e 745f 7265 6d6f 7665 5f65 6c65  ement_remove_ele
-00004fa0: 6d65 6e74 2863 6c61 7373 795f 786d 6c5f  ment(classy_xml_
-00004fb0: 656d 7074 795f 6669 7874 7572 6529 3a0d  empty_fixture):.
-00004fc0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-00004fd0: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-00004fe0: 6173 7379 5f65 6c65 6d65 6e74 203d 2058  assy_element = X
-00004ff0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
-00005000: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-00005010: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-00005020: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-00005030: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005040: 7428 290d 0a20 2020 2064 656c 2063 6c61  t()..    del cla
-00005050: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005060: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005070: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-00005080: 0d0a 2020 2020 6173 7365 7274 206e 6f74  ..    assert not
-00005090: 2068 6173 6174 7472 2863 6c61 7373 795f   hasattr(classy_
-000050a0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-000050b0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-000050c0: 2c20 2778 6d6c 5f65 6c65 6d65 6e74 2729  , 'xml_element')
-000050d0: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f78  ......def test_x
-000050e0: 6d6c 5f65 6c65 6d65 6e74 5f61 6464 5f65  ml_element_add_e
-000050f0: 6c65 6d65 6e74 5f61 7272 6179 2863 6c61  lement_array(cla
-00005100: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005110: 7874 7572 6529 3a0d 0a20 2020 2063 6c61  xture):..    cla
-00005120: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005130: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005140: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005150: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
-00005160: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-00005170: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-00005180: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
-00005190: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
-000051a0: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-000051b0: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-000051c0: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-000051d0: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-000051e0: 7428 290d 0a20 2020 2061 7373 6572 7420  t()..    assert 
-000051f0: 6973 696e 7374 616e 6365 280d 0a20 2020  isinstance(..   
-00005200: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
-00005210: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-00005220: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
-00005230: 5f65 6c65 6d65 6e74 5b30 5d2c 2058 6d6c  _element[0], Xml
-00005240: 456c 656d 656e 7429 0d0a 2020 2020 6173  Element)..    as
-00005250: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+00000000: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
+00000010: 7420 7079 7465 7374 0d0a 6672 6f6d 2063  t pytest..from c
+00000020: 6c61 7373 795f 786d 6c20 696d 706f 7274  lassy_xml import
+00000030: 2043 6c61 7373 7958 6d6c 2c20 586d 6c45   ClassyXml, XmlE
+00000040: 6c65 6d65 6e74 0d0a 0d0a 0d0a 4070 7974  lement......@pyt
+00000050: 6573 742e 6669 7874 7572 650d 0a64 6566  est.fixture..def
+00000060: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00000070: 5f66 6978 7475 7265 2829 3a0d 0a20 2020  _fixture():..   
+00000080: 2066 696c 6570 6174 6820 3d20 6f73 2e70   filepath = os.p
+00000090: 6174 682e 7370 6c69 7428 5f5f 6669 6c65  ath.split(__file
+000000a0: 5f5f 295b 305d 0d0a 2020 2020 7465 7374  __)[0]..    test
+000000b0: 5f78 6d6c 203d 206f 732e 7061 7468 2e6a  _xml = os.path.j
+000000c0: 6f69 6e28 6669 6c65 7061 7468 2c20 2274  oin(filepath, "t
+000000d0: 6573 742e 786d 6c22 290d 0a20 2020 2072  est.xml")..    r
+000000e0: 6574 7572 6e20 436c 6173 7379 586d 6c28  eturn ClassyXml(
+000000f0: 7465 7374 5f78 6d6c 290d 0a0d 0a0d 0a40  test_xml)......@
+00000100: 7079 7465 7374 2e66 6978 7475 7265 0d0a  pytest.fixture..
+00000110: 6465 6620 636c 6173 7379 5f78 6d6c 5f65  def classy_xml_e
+00000120: 6d70 7479 5f66 6978 7475 7265 2829 3a0d  mpty_fixture():.
+00000130: 0a20 2020 2072 6574 7572 6e20 436c 6173  .    return Clas
+00000140: 7379 586d 6c28 290d 0a0d 0a0d 0a40 7079  syXml()......@py
+00000150: 7465 7374 2e66 6978 7475 7265 0d0a 6465  test.fixture..de
+00000160: 6620 636c 6173 7379 5f78 6d6c 5f63 6f75  f classy_xml_cou
+00000170: 6e74 7269 6573 5f66 6978 7475 7265 2829  ntries_fixture()
+00000180: 3a0d 0a20 2020 2066 696c 6570 6174 6820  :..    filepath 
+00000190: 3d20 6f73 2e70 6174 682e 7370 6c69 7428  = os.path.split(
+000001a0: 5f5f 6669 6c65 5f5f 295b 305d 0d0a 2020  __file__)[0]..  
+000001b0: 2020 7465 7374 5f78 6d6c 203d 206f 732e    test_xml = os.
+000001c0: 7061 7468 2e6a 6f69 6e28 6669 6c65 7061  path.join(filepa
+000001d0: 7468 2c20 2263 6f75 6e74 7269 6573 2e78  th, "countries.x
+000001e0: 6d6c 2229 0d0a 2020 2020 7265 7475 726e  ml")..    return
+000001f0: 2043 6c61 7373 7958 6d6c 2874 6573 745f   ClassyXml(test_
+00000200: 786d 6c29 0d0a 0d0a 0d0a 4070 7974 6573  xml)......@pytes
+00000210: 742e 6669 7874 7572 650d 0a64 6566 2063  t.fixture..def c
+00000220: 6c61 7373 795f 786d 6c5f 6d6f 6469 6679  lassy_xml_modify
+00000230: 5f61 6e64 5f73 6176 655f 6669 7874 7572  _and_save_fixtur
+00000240: 6528 293a 0d0a 2020 2020 7265 7475 726e  e():..    return
+00000250: 2043 6c61 7373 7958 6d6c 2829 0d0a 0d0a   ClassyXml()....
+00000260: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
+00000270: 5f65 6c65 6d65 6e74 5f6c 656e 6774 6828  _element_length(
+00000280: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00000290: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
+000002a0: 7373 6572 7420 6c65 6e28 636c 6173 7379  ssert len(classy
+000002b0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+000002c0: 652e 6261 7369 635f 656c 656d 656e 7429  e.basic_element)
+000002d0: 203d 3d20 310d 0a0d 0a0d 0a64 6566 2074   == 1......def t
+000002e0: 6573 745f 6261 7369 635f 656c 656d 656e  est_basic_elemen
+000002f0: 745f 7465 7874 2863 6c61 7373 795f 786d  t_text(classy_xm
+00000300: 6c5f 7465 7374 5f66 6978 7475 7265 293a  l_test_fixture):
+00000310: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
+00000320: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+00000330: 7475 7265 2e62 6173 6963 5f65 6c65 6d65  ture.basic_eleme
+00000340: 6e74 2e74 6578 7420 3d3d 2022 6261 7369  nt.text == "basi
+00000350: 635f 656c 656d 656e 745f 7465 7874 220d  c_element_text".
+00000360: 0a0d 0a0d 0a64 6566 2074 6573 745f 6d75  .....def test_mu
+00000370: 6c74 695f 656c 656d 656e 745f 6c65 6e67  lti_element_leng
+00000380: 7468 2863 6c61 7373 795f 786d 6c5f 7465  th(classy_xml_te
+00000390: 7374 5f66 6978 7475 7265 293a 0d0a 2020  st_fixture):..  
+000003a0: 2020 6173 7365 7274 206c 656e 2863 6c61    assert len(cla
+000003b0: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+000003c0: 7475 7265 2e6d 756c 7469 5f65 6c65 6d65  ture.multi_eleme
+000003d0: 6e74 2920 3d3d 2032 0d0a 0d0a 0d0a 6465  nt) == 2......de
+000003e0: 6620 7465 7374 5f6d 756c 7469 5f65 6c65  f test_multi_ele
+000003f0: 6d65 6e74 5f30 5f74 6578 7428 636c 6173  ment_0_text(clas
+00000400: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00000410: 7572 6529 3a0d 0a20 2020 2061 7373 6572  ure):..    asser
+00000420: 7420 636c 6173 7379 5f78 6d6c 5f74 6573  t classy_xml_tes
+00000430: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+00000440: 656c 656d 656e 745b 305d 2e74 6578 7420  element[0].text 
+00000450: 3d3d 2022 6d75 6c74 695f 656c 656d 656e  == "multi_elemen
+00000460: 745f 7465 7874 5f30 220d 0a0d 0a0d 0a64  t_text_0"......d
+00000470: 6566 2074 6573 745f 6d75 6c74 695f 656c  ef test_multi_el
+00000480: 656d 656e 745f 315f 7465 7874 2863 6c61  ement_1_text(cla
+00000490: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+000004a0: 7475 7265 293a 0d0a 2020 2020 6173 7365  ture):..    asse
+000004b0: 7274 2063 6c61 7373 795f 786d 6c5f 7465  rt classy_xml_te
+000004c0: 7374 5f66 6978 7475 7265 2e6d 756c 7469  st_fixture.multi
+000004d0: 5f65 6c65 6d65 6e74 5b31 5d2e 7465 7874  _element[1].text
+000004e0: 203d 3d20 226d 756c 7469 5f65 6c65 6d65   == "multi_eleme
+000004f0: 6e74 5f74 6578 745f 3122 0d0a 0d0a 0d0a  nt_text_1"......
+00000500: 6465 6620 7465 7374 5f65 6d70 7479 5f65  def test_empty_e
+00000510: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00000520: 6962 7574 6573 5f6c 656e 6774 6828 636c  ibutes_length(cl
+00000530: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00000540: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
+00000550: 6572 7420 6c65 6e28 636c 6173 7379 5f78  ert len(classy_x
+00000560: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00000570: 656d 7074 795f 656c 656d 656e 745f 7769  empty_element_wi
+00000580: 7468 5f61 7474 7269 6275 7465 7329 203d  th_attributes) =
+00000590: 3d20 310d 0a0d 0a0d 0a64 6566 2074 6573  = 1......def tes
+000005a0: 745f 656d 7074 795f 656c 656d 656e 745f  t_empty_element_
+000005b0: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+000005c0: 7465 7874 2863 6c61 7373 795f 786d 6c5f  text(classy_xml_
+000005d0: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
+000005e0: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
+000005f0: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00000600: 7265 2e65 6d70 7479 5f65 6c65 6d65 6e74  re.empty_element
+00000610: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+00000620: 2e74 6578 7420 6973 204e 6f6e 650d 0a0d  .text is None...
+00000630: 0a0d 0a64 6566 2074 6573 745f 656d 7074  ...def test_empt
+00000640: 795f 656c 656d 656e 745f 7769 7468 5f61  y_element_with_a
+00000650: 7474 7269 6275 7465 735f 6174 7472 6962  ttributes_attrib
+00000660: 7574 6573 2863 6c61 7373 795f 786d 6c5f  utes(classy_xml_
+00000670: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
+00000680: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
+00000690: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+000006a0: 7265 2e65 6d70 7479 5f65 6c65 6d65 6e74  re.empty_element
+000006b0: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+000006c0: 2e6e 616d 6520 3d3d 2022 6174 7472 5f6e  .name == "attr_n
+000006d0: 616d 6522 0d0a 2020 2020 6173 7365 7274  ame"..    assert
+000006e0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+000006f0: 5f66 6978 7475 7265 2e65 6d70 7479 5f65  _fixture.empty_e
+00000700: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00000710: 6962 7574 6573 2e76 616c 7565 203d 3d20  ibutes.value == 
+00000720: 2261 7474 725f 7661 6c75 6522 0d0a 0d0a  "attr_value"....
+00000730: 0d0a 6465 6620 7465 7374 5f65 6d70 7479  ..def test_empty
+00000740: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
+00000750: 6974 685f 6174 7472 6962 7574 6573 5f6c  ith_attributes_l
+00000760: 656e 6774 6828 636c 6173 7379 5f78 6d6c  ength(classy_xml
+00000770: 5f74 6573 745f 6669 7874 7572 6529 3a0d  _test_fixture):.
+00000780: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00000790: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+000007a0: 6669 7874 7572 652e 656d 7074 795f 6d75  fixture.empty_mu
+000007b0: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
+000007c0: 5f61 7474 7269 6275 7465 7329 203d 3d20  _attributes) == 
+000007d0: 320d 0a0d 0a0d 0a64 6566 2074 6573 745f  2......def test_
+000007e0: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
+000007f0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00000800: 7465 735f 7465 7874 2863 6c61 7373 795f  tes_text(classy_
+00000810: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+00000820: 293a 0d0a 2020 2020 6173 7365 7274 2063  ):..    assert c
+00000830: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+00000840: 6978 7475 7265 2e65 6d70 7479 5f6d 756c  ixture.empty_mul
+00000850: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00000860: 6174 7472 6962 7574 6573 5b30 5d2e 7465  attributes[0].te
+00000870: 7874 2069 7320 4e6f 6e65 0d0a 2020 2020  xt is None..    
+00000880: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
+00000890: 6c5f 7465 7374 5f66 6978 7475 7265 2e65  l_test_fixture.e
+000008a0: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+000008b0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+000008c0: 6573 5b31 5d2e 7465 7874 2069 7320 4e6f  es[1].text is No
+000008d0: 6e65 0d0a 0d0a 0d0a 6465 6620 7465 7374  ne......def test
+000008e0: 5f65 6d70 7479 5f6d 756c 7469 5f65 6c65  _empty_multi_ele
+000008f0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00000900: 7574 6573 5f61 7474 7269 6275 7465 7328  utes_attributes(
+00000910: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00000920: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
+00000930: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+00000940: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00000950: 5f66 6978 7475 7265 2e65 6d70 7479 5f6d  _fixture.empty_m
+00000960: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
+00000970: 685f 6174 7472 6962 7574 6573 5b30 5d2e  h_attributes[0].
+00000980: 6e61 6d65 0d0a 2020 2020 2020 2020 3d3d  name..        ==
+00000990: 2022 6174 7472 5f30 5f6e 616d 6522 0d0a   "attr_0_name"..
+000009a0: 2020 2020 290d 0a20 2020 2061 7373 6572      )..    asser
+000009b0: 7420 280d 0a20 2020 2020 2020 2063 6c61  t (..        cla
+000009c0: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+000009d0: 7475 7265 2e65 6d70 7479 5f6d 756c 7469  ture.empty_multi
+000009e0: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+000009f0: 7472 6962 7574 6573 5b30 5d2e 7661 6c75  tributes[0].valu
+00000a00: 650d 0a20 2020 2020 2020 203d 3d20 2261  e..        == "a
+00000a10: 7474 725f 305f 7661 6c75 6522 0d0a 2020  ttr_0_value"..  
+00000a20: 2020 290d 0a20 2020 2061 7373 6572 7420    )..    assert 
+00000a30: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
+00000a40: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00000a50: 7265 2e65 6d70 7479 5f6d 756c 7469 5f65  re.empty_multi_e
+00000a60: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00000a70: 6962 7574 6573 5b31 5d2e 6e61 6d65 0d0a  ibutes[1].name..
+00000a80: 2020 2020 2020 2020 3d3d 2022 6174 7472          == "attr
+00000a90: 5f31 5f6e 616d 6522 0d0a 2020 2020 290d  _1_name"..    ).
+00000aa0: 0a20 2020 2061 7373 6572 7420 280d 0a20  .    assert (.. 
+00000ab0: 2020 2020 2020 2063 6c61 7373 795f 786d         classy_xm
+00000ac0: 6c5f 7465 7374 5f66 6978 7475 7265 2e65  l_test_fixture.e
+00000ad0: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+00000ae0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00000af0: 6573 5b31 5d2e 7661 6c75 650d 0a20 2020  es[1].value..   
+00000b00: 2020 2020 203d 3d20 2261 7474 725f 315f       == "attr_1_
+00000b10: 7661 6c75 6522 0d0a 2020 2020 290d 0a0d  value"..    )...
+00000b20: 0a0d 0a64 6566 2074 6573 745f 6261 7369  ...def test_basi
+00000b30: 635f 656c 656d 656e 745f 7769 7468 5f61  c_element_with_a
+00000b40: 7474 7269 6275 7465 735f 6c65 6e67 7468  ttributes_length
+00000b50: 2863 6c61 7373 795f 786d 6c5f 7465 7374  (classy_xml_test
+00000b60: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
+00000b70: 6173 7365 7274 206c 656e 2863 6c61 7373  assert len(class
+00000b80: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00000b90: 7265 2e62 6173 6963 5f65 6c65 6d65 6e74  re.basic_element
+00000ba0: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+00000bb0: 2920 3d3d 2031 0d0a 0d0a 0d0a 6465 6620  ) == 1......def 
+00000bc0: 7465 7374 5f62 6173 6963 5f65 6c65 6d65  test_basic_eleme
+00000bd0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00000be0: 6573 5f74 6578 7428 636c 6173 7379 5f78  es_text(classy_x
+00000bf0: 6d6c 5f74 6573 745f 6669 7874 7572 6529  ml_test_fixture)
+00000c00: 3a0d 0a20 2020 2061 7373 6572 7420 280d  :..    assert (.
+00000c10: 0a20 2020 2020 2020 2063 6c61 7373 795f  .        classy_
+00000c20: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+00000c30: 2e62 6173 6963 5f65 6c65 6d65 6e74 5f77  .basic_element_w
+00000c40: 6974 685f 6174 7472 6962 7574 6573 2e74  ith_attributes.t
+00000c50: 6578 740d 0a20 2020 2020 2020 203d 3d20  ext..        == 
+00000c60: 2262 6173 6963 5f65 6c65 6d65 6e74 5f77  "basic_element_w
+00000c70: 6974 685f 6174 7472 6962 7574 6573 5f74  ith_attributes_t
+00000c80: 6578 7422 0d0a 2020 2020 290d 0a0d 0a0d  ext"..    ).....
+00000c90: 0a64 6566 2074 6573 745f 6261 7369 635f  .def test_basic_
+00000ca0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00000cb0: 7269 6275 7465 735f 6174 7472 6962 7574  ributes_attribut
+00000cc0: 6573 2863 6c61 7373 795f 786d 6c5f 7465  es(classy_xml_te
+00000cd0: 7374 5f66 6978 7475 7265 293a 0d0a 2020  st_fixture):..  
+00000ce0: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
+00000cf0: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+00000d00: 2e62 6173 6963 5f65 6c65 6d65 6e74 5f77  .basic_element_w
+00000d10: 6974 685f 6174 7472 6962 7574 6573 2e6e  ith_attributes.n
+00000d20: 616d 6520 3d3d 2022 6174 7472 5f6e 616d  ame == "attr_nam
+00000d30: 6522 0d0a 2020 2020 6173 7365 7274 2063  e"..    assert c
+00000d40: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+00000d50: 6978 7475 7265 2e62 6173 6963 5f65 6c65  ixture.basic_ele
+00000d60: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00000d70: 7574 6573 2e76 616c 7565 203d 3d20 2261  utes.value == "a
+00000d80: 7474 725f 7661 6c75 6522 0d0a 0d0a 0d0a  ttr_value"......
+00000d90: 6465 6620 7465 7374 5f6d 756c 7469 5f65  def test_multi_e
+00000da0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00000db0: 6962 7574 6573 5f6c 656e 6774 6828 636c  ibutes_length(cl
+00000dc0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00000dd0: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
+00000de0: 6572 7420 6c65 6e28 636c 6173 7379 5f78  ert len(classy_x
+00000df0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00000e00: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+00000e10: 7468 5f61 7474 7269 6275 7465 7329 203d  th_attributes) =
+00000e20: 3d20 320d 0a0d 0a0d 0a64 6566 2074 6573  = 2......def tes
+00000e30: 745f 6d75 6c74 695f 656c 656d 656e 745f  t_multi_element_
+00000e40: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00000e50: 7465 7874 2863 6c61 7373 795f 786d 6c5f  text(classy_xml_
+00000e60: 7465 7374 5f66 6978 7475 7265 293a 0d0a  test_fixture):..
+00000e70: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+00000e80: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00000e90: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00000ea0: 6c74 695f 656c 656d 656e 745f 7769 7468  lti_element_with
+00000eb0: 5f61 7474 7269 6275 7465 735b 305d 2e74  _attributes[0].t
+00000ec0: 6578 740d 0a20 2020 2020 2020 203d 3d20  ext..        == 
+00000ed0: 226d 756c 7469 5f65 6c65 6d65 6e74 5f77  "multi_element_w
+00000ee0: 6974 685f 6174 7472 6962 7574 6573 5f74  ith_attributes_t
+00000ef0: 6578 745f 3022 0d0a 2020 2020 290d 0a20  ext_0"..    ).. 
+00000f00: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00000f10: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00000f20: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
+00000f30: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00000f40: 6174 7472 6962 7574 6573 5b31 5d2e 7465  attributes[1].te
+00000f50: 7874 0d0a 2020 2020 2020 2020 3d3d 2022  xt..        == "
+00000f60: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+00000f70: 7468 5f61 7474 7269 6275 7465 735f 7465  th_attributes_te
+00000f80: 7874 5f31 220d 0a20 2020 2029 0d0a 0d0a  xt_1"..    )....
+00000f90: 0d0a 6465 6620 7465 7374 5f6d 756c 7469  ..def test_multi
+00000fa0: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+00000fb0: 7472 6962 7574 6573 5f61 7474 7269 6275  tributes_attribu
+00000fc0: 7465 7328 636c 6173 7379 5f78 6d6c 5f74  tes(classy_xml_t
+00000fd0: 6573 745f 6669 7874 7572 6529 3a0d 0a20  est_fixture):.. 
+00000fe0: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00000ff0: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00001000: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
+00001010: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00001020: 6174 7472 6962 7574 6573 5b30 5d2e 6e61  attributes[0].na
+00001030: 6d65 203d 3d20 2261 7474 725f 305f 6e61  me == "attr_0_na
+00001040: 6d65 220d 0a20 2020 2029 0d0a 2020 2020  me"..    )..    
+00001050: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+00001060: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00001070: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+00001080: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00001090: 7269 6275 7465 735b 305d 2e76 616c 7565  ributes[0].value
+000010a0: 203d 3d20 2261 7474 725f 305f 7661 6c75   == "attr_0_valu
+000010b0: 6522 0d0a 2020 2020 290d 0a20 2020 2061  e"..    )..    a
+000010c0: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+000010d0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+000010e0: 5f66 6978 7475 7265 2e6d 756c 7469 5f65  _fixture.multi_e
+000010f0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00001100: 6962 7574 6573 5b31 5d2e 6e61 6d65 203d  ibutes[1].name =
+00001110: 3d20 2261 7474 725f 315f 6e61 6d65 220d  = "attr_1_name".
+00001120: 0a20 2020 2029 0d0a 2020 2020 6173 7365  .    )..    asse
+00001130: 7274 2028 0d0a 2020 2020 2020 2020 636c  rt (..        cl
+00001140: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00001150: 7874 7572 652e 6d75 6c74 695f 656c 656d  xture.multi_elem
+00001160: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00001170: 7465 735b 315d 2e76 616c 7565 203d 3d20  tes[1].value == 
+00001180: 2261 7474 725f 315f 7661 6c75 6522 0d0a  "attr_1_value"..
+00001190: 2020 2020 290d 0a0d 0a0d 0a64 6566 2074      )......def t
+000011a0: 6573 745f 6261 7369 635f 6e65 7374 6564  est_basic_nested
+000011b0: 5f65 6c65 6d65 6e74 5f6c 656e 6774 6828  _element_length(
+000011c0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+000011d0: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
+000011e0: 7373 6572 7420 6c65 6e28 636c 6173 7379  ssert len(classy
+000011f0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00001200: 652e 6261 7369 635f 6e65 7374 6564 5f65  e.basic_nested_e
+00001210: 6c65 6d65 6e74 2920 3d3d 2031 0d0a 0d0a  lement) == 1....
+00001220: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
+00001230: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
+00001240: 5f62 6173 6963 5f65 6c65 6d65 6e74 5f63  _basic_element_c
+00001250: 6869 6c64 5f6c 656e 6774 6828 636c 6173  hild_length(clas
+00001260: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00001270: 7572 6529 3a0d 0a20 2020 2061 7373 6572  ure):..    asser
+00001280: 7420 6c65 6e28 636c 6173 7379 5f78 6d6c  t len(classy_xml
+00001290: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
+000012a0: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
+000012b0: 6e74 2e62 6173 6963 5f65 6c65 6d65 6e74  nt.basic_element
+000012c0: 5f63 6869 6c64 2920 3d3d 2031 0d0a 0d0a  _child) == 1....
+000012d0: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
+000012e0: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
+000012f0: 5f62 6173 6963 5f65 6c65 6d65 6e74 5f63  _basic_element_c
+00001300: 6869 6c64 5f74 6578 7428 636c 6173 7379  hild_text(classy
+00001310: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00001320: 6529 3a0d 0a20 2020 2061 7373 6572 7420  e):..    assert 
+00001330: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
+00001340: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00001350: 7265 2e62 6173 6963 5f6e 6573 7465 645f  re.basic_nested_
+00001360: 656c 656d 656e 742e 6261 7369 635f 656c  element.basic_el
+00001370: 656d 656e 745f 6368 696c 642e 7465 7874  ement_child.text
+00001380: 0d0a 2020 2020 2020 2020 3d3d 2022 6261  ..        == "ba
+00001390: 7369 635f 656c 656d 656e 745f 6368 696c  sic_element_chil
+000013a0: 645f 7465 7874 220d 0a20 2020 2029 0d0a  d_text"..    )..
+000013b0: 0d0a 0d0a 6465 6620 7465 7374 5f62 6173  ....def test_bas
+000013c0: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
+000013d0: 745f 5f6d 756c 7469 5f65 6c65 6d65 6e74  t__multi_element
+000013e0: 5f63 6869 6c64 5f6c 656e 6774 6828 636c  _child_length(cl
+000013f0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00001400: 7874 7572 6529 3a0d 0a20 2020 2061 7373  xture):..    ass
+00001410: 6572 7420 6c65 6e28 636c 6173 7379 5f78  ert len(classy_x
+00001420: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00001430: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
+00001440: 6d65 6e74 2e6d 756c 7469 5f65 6c65 6d65  ment.multi_eleme
+00001450: 6e74 5f63 6869 6c64 2920 3d3d 2032 0d0a  nt_child) == 2..
+00001460: 0d0a 0d0a 6465 6620 7465 7374 5f62 6173  ....def test_bas
+00001470: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
+00001480: 745f 5f6d 756c 7469 5f65 6c65 6d65 6e74  t__multi_element
+00001490: 5f63 6869 6c64 5f74 6578 7428 636c 6173  _child_text(clas
+000014a0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000014b0: 7572 6529 3a0d 0a20 2020 2061 7373 6572  ure):..    asser
+000014c0: 7420 280d 0a20 2020 2020 2020 2063 6c61  t (..        cla
+000014d0: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+000014e0: 7475 7265 2e62 6173 6963 5f6e 6573 7465  ture.basic_neste
+000014f0: 645f 656c 656d 656e 742e 6d75 6c74 695f  d_element.multi_
+00001500: 656c 656d 656e 745f 6368 696c 645b 305d  element_child[0]
+00001510: 2e74 6578 740d 0a20 2020 2020 2020 203d  .text..        =
+00001520: 3d20 226d 756c 7469 5f65 6c65 6d65 6e74  = "multi_element
+00001530: 5f63 6869 6c64 5f74 6578 745f 3022 0d0a  _child_text_0"..
+00001540: 2020 2020 290d 0a20 2020 2061 7373 6572      )..    asser
+00001550: 7420 280d 0a20 2020 2020 2020 2063 6c61  t (..        cla
+00001560: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+00001570: 7475 7265 2e62 6173 6963 5f6e 6573 7465  ture.basic_neste
+00001580: 645f 656c 656d 656e 742e 6d75 6c74 695f  d_element.multi_
+00001590: 656c 656d 656e 745f 6368 696c 645b 315d  element_child[1]
+000015a0: 2e74 6578 740d 0a20 2020 2020 2020 203d  .text..        =
+000015b0: 3d20 226d 756c 7469 5f65 6c65 6d65 6e74  = "multi_element
+000015c0: 5f63 6869 6c64 5f74 6578 745f 3122 0d0a  _child_text_1"..
+000015d0: 2020 2020 290d 0a0d 0a0d 0a64 6566 2074      )......def t
+000015e0: 6573 745f 6261 7369 635f 6e65 7374 6564  est_basic_nested
+000015f0: 5f65 6c65 6d65 6e74 5f5f 656d 7074 795f  _element__empty_
+00001600: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00001610: 7269 6275 7465 735f 6368 696c 645f 6c65  ributes_child_le
+00001620: 6e67 7468 280d 0a20 2020 2063 6c61 7373  ngth(..    class
+00001630: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00001640: 7265 2c0d 0a29 3a0d 0a20 2020 2061 7373  re,..):..    ass
+00001650: 6572 7420 280d 0a20 2020 2020 2020 206c  ert (..        l
+00001660: 656e 280d 0a20 2020 2020 2020 2020 2020  en(..           
+00001670: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00001680: 5f66 6978 7475 7265 2e62 6173 6963 5f6e  _fixture.basic_n
+00001690: 6573 7465 645f 656c 656d 656e 742e 656d  ested_element.em
+000016a0: 7074 795f 656c 656d 656e 745f 7769 7468  pty_element_with
+000016b0: 5f61 7474 7269 6275 7465 735f 6368 696c  _attributes_chil
+000016c0: 640d 0a20 2020 2020 2020 2029 0d0a 2020  d..        )..  
+000016d0: 2020 2020 2020 3d3d 2031 0d0a 2020 2020        == 1..    
+000016e0: 290d 0a0d 0a0d 0a64 6566 2074 6573 745f  )......def test_
+000016f0: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
+00001700: 6d65 6e74 5f5f 656d 7074 795f 656c 656d  ment__empty_elem
+00001710: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00001720: 7465 735f 6368 696c 645f 7465 7874 280d  tes_child_text(.
+00001730: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00001740: 7465 7374 5f66 6978 7475 7265 2c0d 0a29  test_fixture,..)
+00001750: 3a0d 0a20 2020 2061 7373 6572 7420 280d  :..    assert (.
+00001760: 0a20 2020 2020 2020 2063 6c61 7373 795f  .        classy_
+00001770: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+00001780: 2e62 6173 6963 5f6e 6573 7465 645f 656c  .basic_nested_el
+00001790: 656d 656e 742e 656d 7074 795f 656c 656d  ement.empty_elem
+000017a0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+000017b0: 7465 735f 6368 696c 642e 7465 7874 0d0a  tes_child.text..
+000017c0: 2020 2020 2020 2020 6973 204e 6f6e 650d          is None.
+000017d0: 0a20 2020 2029 0d0a 0d0a 0d0a 6465 6620  .    )......def 
+000017e0: 7465 7374 5f62 6173 6963 5f6e 6573 7465  test_basic_neste
+000017f0: 645f 656c 656d 656e 745f 5f65 6d70 7479  d_element__empty
+00001800: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+00001810: 7472 6962 7574 6573 5f63 6869 6c64 5f61  tributes_child_a
+00001820: 7474 7269 6275 7465 7328 0d0a 2020 2020  ttributes(..    
+00001830: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00001840: 6669 7874 7572 652c 0d0a 293a 0d0a 2020  fixture,..):..  
+00001850: 2020 6173 7365 7274 2028 0d0a 2020 2020    assert (..    
+00001860: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00001870: 6573 745f 6669 7874 7572 652e 6261 7369  est_fixture.basi
+00001880: 635f 6e65 7374 6564 5f65 6c65 6d65 6e74  c_nested_element
+00001890: 2e65 6d70 7479 5f65 6c65 6d65 6e74 5f77  .empty_element_w
+000018a0: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+000018b0: 6869 6c64 2e6e 616d 650d 0a20 2020 2020  hild.name..     
+000018c0: 2020 203d 3d20 2263 6869 6c64 5f61 7474     == "child_att
+000018d0: 725f 6e61 6d65 220d 0a20 2020 2029 0d0a  r_name"..    )..
+000018e0: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+000018f0: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00001900: 5f74 6573 745f 6669 7874 7572 652e 6261  _test_fixture.ba
+00001910: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
+00001920: 6e74 2e65 6d70 7479 5f65 6c65 6d65 6e74  nt.empty_element
+00001930: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+00001940: 5f63 6869 6c64 2e76 616c 7565 0d0a 2020  _child.value..  
+00001950: 2020 2020 2020 3d3d 2022 6368 696c 645f        == "child_
+00001960: 6174 7472 5f76 616c 7565 220d 0a20 2020  attr_value"..   
+00001970: 2029 0d0a 0d0a 0d0a 6465 6620 7465 7374   )......def test
+00001980: 5f62 6173 6963 5f6e 6573 7465 645f 656c  _basic_nested_el
+00001990: 656d 656e 745f 5f65 6d70 7479 5f6d 756c  ement__empty_mul
+000019a0: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+000019b0: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+000019c0: 5f6c 656e 6774 6828 0d0a 2020 2020 636c  _length(..    cl
+000019d0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+000019e0: 7874 7572 652c 0d0a 293a 0d0a 2020 2020  xture,..):..    
+000019f0: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+00001a00: 2020 6c65 6e28 0d0a 2020 2020 2020 2020    len(..        
+00001a10: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00001a20: 6573 745f 6669 7874 7572 652e 6261 7369  est_fixture.basi
+00001a30: 635f 6e65 7374 6564 5f65 6c65 6d65 6e74  c_nested_element
+00001a40: 2e65 6d70 7479 5f6d 756c 7469 5f65 6c65  .empty_multi_ele
+00001a50: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00001a60: 7574 6573 5f63 6869 6c64 0d0a 2020 2020  utes_child..    
+00001a70: 2020 2020 290d 0a20 2020 2020 2020 203d      )..        =
+00001a80: 3d20 320d 0a20 2020 2029 0d0a 0d0a 0d0a  = 2..    )......
+00001a90: 6465 6620 7465 7374 5f62 6173 6963 5f6e  def test_basic_n
+00001aa0: 6573 7465 645f 656c 656d 656e 745f 5f65  ested_element__e
+00001ab0: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+00001ac0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00001ad0: 6573 5f63 6869 6c64 5f74 6578 7428 0d0a  es_child_text(..
+00001ae0: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00001af0: 6573 745f 6669 7874 7572 652c 0d0a 293a  est_fixture,..):
+00001b00: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+00001b10: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+00001b20: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00001b30: 6261 7369 635f 6e65 7374 6564 5f65 6c65  basic_nested_ele
+00001b40: 6d65 6e74 2e65 6d70 7479 5f6d 756c 7469  ment.empty_multi
+00001b50: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+00001b60: 7472 6962 7574 6573 5f63 6869 6c64 5b0d  tributes_child[.
+00001b70: 0a20 2020 2020 2020 2020 2020 2030 0d0a  .            0..
+00001b80: 2020 2020 2020 2020 5d2e 7465 7874 0d0a          ].text..
+00001b90: 2020 2020 2020 2020 6973 204e 6f6e 650d          is None.
+00001ba0: 0a20 2020 2029 0d0a 2020 2020 6173 7365  .    )..    asse
+00001bb0: 7274 2028 0d0a 2020 2020 2020 2020 636c  rt (..        cl
+00001bc0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00001bd0: 7874 7572 652e 6261 7369 635f 6e65 7374  xture.basic_nest
+00001be0: 6564 5f65 6c65 6d65 6e74 2e65 6d70 7479  ed_element.empty
+00001bf0: 5f6d 756c 7469 5f65 6c65 6d65 6e74 5f77  _multi_element_w
+00001c00: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+00001c10: 6869 6c64 5b0d 0a20 2020 2020 2020 2020  hild[..         
+00001c20: 2020 2031 0d0a 2020 2020 2020 2020 5d2e     1..        ].
+00001c30: 7465 7874 0d0a 2020 2020 2020 2020 6973  text..        is
+00001c40: 204e 6f6e 650d 0a20 2020 2029 0d0a 0d0a   None..    )....
+00001c50: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
+00001c60: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
+00001c70: 5f65 6d70 7479 5f6d 756c 7469 5f65 6c65  _empty_multi_ele
+00001c80: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00001c90: 7574 6573 5f63 6869 6c64 5f61 7474 7269  utes_child_attri
+00001ca0: 6275 7465 7328 0d0a 2020 2020 636c 6173  butes(..    clas
+00001cb0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00001cc0: 7572 652c 0d0a 293a 0d0a 2020 2020 6173  ure,..):..    as
+00001cd0: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+00001ce0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00001cf0: 6669 7874 7572 652e 6261 7369 635f 6e65  fixture.basic_ne
+00001d00: 7374 6564 5f65 6c65 6d65 6e74 2e65 6d70  sted_element.emp
+00001d10: 7479 5f6d 756c 7469 5f65 6c65 6d65 6e74  ty_multi_element
+00001d20: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+00001d30: 5f63 6869 6c64 5b0d 0a20 2020 2020 2020  _child[..       
+00001d40: 2020 2020 2030 0d0a 2020 2020 2020 2020       0..        
+00001d50: 5d2e 6e61 6d65 0d0a 2020 2020 2020 2020  ].name..        
+00001d60: 3d3d 2022 6368 696c 645f 6174 7472 5f30  == "child_attr_0
+00001d70: 5f6e 616d 6522 0d0a 2020 2020 290d 0a20  _name"..    ).. 
+00001d80: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00001d90: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00001da0: 7465 7374 5f66 6978 7475 7265 2e62 6173  test_fixture.bas
+00001db0: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
+00001dc0: 742e 656d 7074 795f 6d75 6c74 695f 656c  t.empty_multi_el
+00001dd0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+00001de0: 6275 7465 735f 6368 696c 645b 0d0a 2020  butes_child[..  
+00001df0: 2020 2020 2020 2020 2020 300d 0a20 2020            0..   
+00001e00: 2020 2020 205d 2e76 616c 7565 0d0a 2020       ].value..  
+00001e10: 2020 2020 2020 3d3d 2022 6368 696c 645f        == "child_
+00001e20: 6174 7472 5f30 5f76 616c 7565 220d 0a20  attr_0_value".. 
+00001e30: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00001e40: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00001e50: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00001e60: 7572 652e 6261 7369 635f 6e65 7374 6564  ure.basic_nested
+00001e70: 5f65 6c65 6d65 6e74 2e65 6d70 7479 5f6d  _element.empty_m
+00001e80: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
+00001e90: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
+00001ea0: 6c64 5b0d 0a20 2020 2020 2020 2020 2020  ld[..           
+00001eb0: 2031 0d0a 2020 2020 2020 2020 5d2e 6e61   1..        ].na
+00001ec0: 6d65 0d0a 2020 2020 2020 2020 3d3d 2022  me..        == "
+00001ed0: 6368 696c 645f 6174 7472 5f31 5f6e 616d  child_attr_1_nam
+00001ee0: 6522 0d0a 2020 2020 290d 0a20 2020 2061  e"..    )..    a
+00001ef0: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+00001f00: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00001f10: 5f66 6978 7475 7265 2e62 6173 6963 5f6e  _fixture.basic_n
+00001f20: 6573 7465 645f 656c 656d 656e 742e 656d  ested_element.em
+00001f30: 7074 795f 6d75 6c74 695f 656c 656d 656e  pty_multi_elemen
+00001f40: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00001f50: 735f 6368 696c 645b 0d0a 2020 2020 2020  s_child[..      
+00001f60: 2020 2020 2020 310d 0a20 2020 2020 2020        1..       
+00001f70: 205d 2e76 616c 7565 0d0a 2020 2020 2020   ].value..      
+00001f80: 2020 3d3d 2022 6368 696c 645f 6174 7472    == "child_attr
+00001f90: 5f31 5f76 616c 7565 220d 0a20 2020 2029  _1_value"..    )
+00001fa0: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f62  ......def test_b
+00001fb0: 6173 6963 5f6e 6573 7465 645f 656c 656d  asic_nested_elem
+00001fc0: 656e 745f 5f62 6173 6963 5f65 6c65 6d65  ent__basic_eleme
+00001fd0: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00001fe0: 6573 5f63 6869 6c64 5f6c 656e 6774 6828  es_child_length(
+00001ff0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+00002000: 5f74 6573 745f 6669 7874 7572 652c 0d0a  _test_fixture,..
+00002010: 293a 0d0a 2020 2020 6173 7365 7274 2028  ):..    assert (
+00002020: 0d0a 2020 2020 2020 2020 6c65 6e28 0d0a  ..        len(..
+00002030: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+00002040: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00002050: 7572 652e 6261 7369 635f 6e65 7374 6564  ure.basic_nested
+00002060: 5f65 6c65 6d65 6e74 2e62 6173 6963 5f65  _element.basic_e
+00002070: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00002080: 6962 7574 6573 5f63 6869 6c64 0d0a 2020  ibutes_child..  
+00002090: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000020a0: 203d 3d20 310d 0a20 2020 2029 0d0a 0d0a   == 1..    )....
+000020b0: 0d0a 6465 6620 7465 7374 5f62 6173 6963  ..def test_basic
+000020c0: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
+000020d0: 5f62 6173 6963 5f65 6c65 6d65 6e74 5f77  _basic_element_w
+000020e0: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+000020f0: 6869 6c64 5f74 6578 7428 0d0a 2020 2020  hild_text(..    
+00002100: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00002110: 6669 7874 7572 652c 0d0a 293a 0d0a 2020  fixture,..):..  
+00002120: 2020 6173 7365 7274 2028 0d0a 2020 2020    assert (..    
+00002130: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00002140: 6573 745f 6669 7874 7572 652e 6261 7369  est_fixture.basi
+00002150: 635f 6e65 7374 6564 5f65 6c65 6d65 6e74  c_nested_element
+00002160: 2e62 6173 6963 5f65 6c65 6d65 6e74 5f77  .basic_element_w
+00002170: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+00002180: 6869 6c64 2e74 6578 740d 0a20 2020 2020  hild.text..     
+00002190: 2020 203d 3d20 2262 6173 6963 5f65 6c65     == "basic_ele
+000021a0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+000021b0: 7574 6573 5f63 6869 6c64 5f74 6578 7422  utes_child_text"
+000021c0: 0d0a 2020 2020 290d 0a0d 0a0d 0a64 6566  ..    )......def
+000021d0: 2074 6573 745f 6261 7369 635f 6e65 7374   test_basic_nest
+000021e0: 6564 5f65 6c65 6d65 6e74 5f5f 6261 7369  ed_element__basi
+000021f0: 635f 656c 656d 656e 745f 7769 7468 5f61  c_element_with_a
+00002200: 7474 7269 6275 7465 735f 6368 696c 645f  ttributes_child_
+00002210: 6174 7472 6962 7574 6573 280d 0a20 2020  attributes(..   
+00002220: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00002230: 5f66 6978 7475 7265 2c0d 0a29 3a0d 0a20  _fixture,..):.. 
+00002240: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00002250: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00002260: 7465 7374 5f66 6978 7475 7265 2e62 6173  test_fixture.bas
+00002270: 6963 5f6e 6573 7465 645f 656c 656d 656e  ic_nested_elemen
+00002280: 742e 6261 7369 635f 656c 656d 656e 745f  t.basic_element_
+00002290: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+000022a0: 6368 696c 642e 6e61 6d65 0d0a 2020 2020  child.name..    
+000022b0: 2020 2020 3d3d 2022 6368 696c 645f 6174      == "child_at
+000022c0: 7472 5f6e 616d 6522 0d0a 2020 2020 290d  tr_name"..    ).
+000022d0: 0a20 2020 2061 7373 6572 7420 280d 0a20  .    assert (.. 
+000022e0: 2020 2020 2020 2063 6c61 7373 795f 786d         classy_xm
+000022f0: 6c5f 7465 7374 5f66 6978 7475 7265 2e62  l_test_fixture.b
+00002300: 6173 6963 5f6e 6573 7465 645f 656c 656d  asic_nested_elem
+00002310: 656e 742e 6261 7369 635f 656c 656d 656e  ent.basic_elemen
+00002320: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00002330: 735f 6368 696c 642e 7661 6c75 650d 0a20  s_child.value.. 
+00002340: 2020 2020 2020 203d 3d20 2263 6869 6c64         == "child
+00002350: 5f61 7474 725f 7661 6c75 6522 0d0a 2020  _attr_value"..  
+00002360: 2020 290d 0a0d 0a0d 0a64 6566 2074 6573    )......def tes
+00002370: 745f 6261 7369 635f 6e65 7374 6564 5f65  t_basic_nested_e
+00002380: 6c65 6d65 6e74 5f5f 6d75 6c74 695f 656c  lement__multi_el
+00002390: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+000023a0: 6275 7465 735f 6368 696c 645f 6c65 6e67  butes_child_leng
+000023b0: 7468 280d 0a20 2020 2063 6c61 7373 795f  th(..    classy_
+000023c0: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+000023d0: 2c0d 0a29 3a0d 0a20 2020 2061 7373 6572  ,..):..    asser
+000023e0: 7420 280d 0a20 2020 2020 2020 206c 656e  t (..        len
+000023f0: 280d 0a20 2020 2020 2020 2020 2020 2063  (..            c
+00002400: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+00002410: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
+00002420: 7465 645f 656c 656d 656e 742e 6d75 6c74  ted_element.mult
+00002430: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
+00002440: 7474 7269 6275 7465 735f 6368 696c 640d  ttributes_child.
+00002450: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+00002460: 2020 2020 3d3d 2032 0d0a 2020 2020 290d      == 2..    ).
+00002470: 0a0d 0a0d 0a64 6566 2074 6573 745f 6261  .....def test_ba
+00002480: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
+00002490: 6e74 5f5f 6d75 6c74 695f 656c 656d 656e  nt__multi_elemen
+000024a0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+000024b0: 735f 6368 696c 645f 7465 7874 280d 0a20  s_child_text(.. 
+000024c0: 2020 2063 6c61 7373 795f 786d 6c5f 7465     classy_xml_te
+000024d0: 7374 5f66 6978 7475 7265 2c0d 0a29 3a0d  st_fixture,..):.
+000024e0: 0a20 2020 2061 7373 6572 7420 280d 0a20  .    assert (.. 
+000024f0: 2020 2020 2020 2063 6c61 7373 795f 786d         classy_xm
+00002500: 6c5f 7465 7374 5f66 6978 7475 7265 2e62  l_test_fixture.b
+00002510: 6173 6963 5f6e 6573 7465 645f 656c 656d  asic_nested_elem
+00002520: 656e 742e 6d75 6c74 695f 656c 656d 656e  ent.multi_elemen
+00002530: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00002540: 735f 6368 696c 645b 0d0a 2020 2020 2020  s_child[..      
+00002550: 2020 2020 2020 300d 0a20 2020 2020 2020        0..       
+00002560: 205d 2e74 6578 740d 0a20 2020 2020 2020   ].text..       
+00002570: 203d 3d20 226d 756c 7469 5f65 6c65 6d65   == "multi_eleme
+00002580: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00002590: 6573 5f63 6869 6c64 5f74 6578 745f 3022  es_child_text_0"
+000025a0: 0d0a 2020 2020 290d 0a20 2020 2061 7373  ..    )..    ass
+000025b0: 6572 7420 280d 0a20 2020 2020 2020 2063  ert (..        c
+000025c0: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+000025d0: 6978 7475 7265 2e62 6173 6963 5f6e 6573  ixture.basic_nes
+000025e0: 7465 645f 656c 656d 656e 742e 6d75 6c74  ted_element.mult
+000025f0: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
+00002600: 7474 7269 6275 7465 735f 6368 696c 645b  ttributes_child[
+00002610: 0d0a 2020 2020 2020 2020 2020 2020 310d  ..            1.
+00002620: 0a20 2020 2020 2020 205d 2e74 6578 740d  .        ].text.
+00002630: 0a20 2020 2020 2020 203d 3d20 226d 756c  .        == "mul
+00002640: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00002650: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+00002660: 5f74 6578 745f 3122 0d0a 2020 2020 290d  _text_1"..    ).
+00002670: 0a0d 0a0d 0a64 6566 2074 6573 745f 6261  .....def test_ba
+00002680: 7369 635f 6e65 7374 6564 5f65 6c65 6d65  sic_nested_eleme
+00002690: 6e74 5f5f 6d75 6c74 695f 656c 656d 656e  nt__multi_elemen
+000026a0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+000026b0: 735f 6368 696c 645f 6174 7472 6962 7574  s_child_attribut
+000026c0: 6573 280d 0a20 2020 2063 6c61 7373 795f  es(..    classy_
+000026d0: 786d 6c5f 7465 7374 5f66 6978 7475 7265  xml_test_fixture
+000026e0: 2c0d 0a29 3a0d 0a20 2020 2061 7373 6572  ,..):..    asser
+000026f0: 7420 280d 0a20 2020 2020 2020 2063 6c61  t (..        cla
+00002700: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+00002710: 7475 7265 2e62 6173 6963 5f6e 6573 7465  ture.basic_neste
+00002720: 645f 656c 656d 656e 742e 6d75 6c74 695f  d_element.multi_
+00002730: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00002740: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
+00002750: 2020 2020 2020 2020 2020 2020 300d 0a20              0.. 
+00002760: 2020 2020 2020 205d 2e6e 616d 650d 0a20         ].name.. 
+00002770: 2020 2020 2020 203d 3d20 2263 6869 6c64         == "child
+00002780: 5f61 7474 725f 305f 6e61 6d65 220d 0a20  _attr_0_name".. 
+00002790: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+000027a0: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+000027b0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000027c0: 7572 652e 6261 7369 635f 6e65 7374 6564  ure.basic_nested
+000027d0: 5f65 6c65 6d65 6e74 2e6d 756c 7469 5f65  _element.multi_e
+000027e0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+000027f0: 6962 7574 6573 5f63 6869 6c64 5b0d 0a20  ibutes_child[.. 
+00002800: 2020 2020 2020 2020 2020 2030 0d0a 2020             0..  
+00002810: 2020 2020 2020 5d2e 7661 6c75 650d 0a20        ].value.. 
+00002820: 2020 2020 2020 203d 3d20 2263 6869 6c64         == "child
+00002830: 5f61 7474 725f 305f 7661 6c75 6522 0d0a  _attr_0_value"..
+00002840: 2020 2020 290d 0a20 2020 2061 7373 6572      )..    asser
+00002850: 7420 280d 0a20 2020 2020 2020 2063 6c61  t (..        cla
+00002860: 7373 795f 786d 6c5f 7465 7374 5f66 6978  ssy_xml_test_fix
+00002870: 7475 7265 2e62 6173 6963 5f6e 6573 7465  ture.basic_neste
+00002880: 645f 656c 656d 656e 742e 6d75 6c74 695f  d_element.multi_
+00002890: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+000028a0: 7269 6275 7465 735f 6368 696c 645b 0d0a  ributes_child[..
+000028b0: 2020 2020 2020 2020 2020 2020 310d 0a20              1.. 
+000028c0: 2020 2020 2020 205d 2e6e 616d 650d 0a20         ].name.. 
+000028d0: 2020 2020 2020 203d 3d20 2263 6869 6c64         == "child
+000028e0: 5f61 7474 725f 315f 6e61 6d65 220d 0a20  _attr_1_name".. 
+000028f0: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00002900: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00002910: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00002920: 7572 652e 6261 7369 635f 6e65 7374 6564  ure.basic_nested
+00002930: 5f65 6c65 6d65 6e74 2e6d 756c 7469 5f65  _element.multi_e
+00002940: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00002950: 6962 7574 6573 5f63 6869 6c64 5b0d 0a20  ibutes_child[.. 
+00002960: 2020 2020 2020 2020 2020 2031 0d0a 2020             1..  
+00002970: 2020 2020 2020 5d2e 7661 6c75 650d 0a20        ].value.. 
+00002980: 2020 2020 2020 203d 3d20 2263 6869 6c64         == "child
+00002990: 5f61 7474 725f 315f 7661 6c75 6522 0d0a  _attr_1_value"..
+000029a0: 2020 2020 290d 0a0d 0a0d 0a64 6566 2074      )......def t
+000029b0: 6573 745f 6d75 6c74 695f 6e65 7374 6564  est_multi_nested
+000029c0: 5f65 6c65 6d65 6e74 5f6c 656e 6774 6828  _element_length(
+000029d0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+000029e0: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
+000029f0: 7373 6572 7420 6c65 6e28 636c 6173 7379  ssert len(classy
+00002a00: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00002a10: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00002a20: 6c65 6d65 6e74 2920 3d3d 2032 0d0a 0d0a  lement) == 2....
+00002a30: 0d0a 6465 6620 7465 7374 5f6d 756c 7469  ..def test_multi
+00002a40: 5f6e 6573 7465 645f 656c 656d 656e 745f  _nested_element_
+00002a50: 5f62 6173 6963 5f65 6c65 6d65 6e74 5f63  _basic_element_c
+00002a60: 6869 6c64 5f6c 656e 6774 6828 636c 6173  hild_length(clas
+00002a70: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00002a80: 7572 6529 3a0d 0a20 2020 2061 7373 6572  ure):..    asser
+00002a90: 7420 6c65 6e28 636c 6173 7379 5f78 6d6c  t len(classy_xml
+00002aa0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00002ab0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00002ac0: 6e74 5b30 5d2e 6261 7369 635f 656c 656d  nt[0].basic_elem
+00002ad0: 656e 745f 6368 696c 6429 203d 3d20 310d  ent_child) == 1.
+00002ae0: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00002af0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00002b00: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
+00002b10: 7374 6564 5f65 6c65 6d65 6e74 5b31 5d2e  sted_element[1].
+00002b20: 6261 7369 635f 656c 656d 656e 745f 6368  basic_element_ch
+00002b30: 696c 6429 203d 3d20 310d 0a0d 0a0d 0a64  ild) == 1......d
+00002b40: 6566 2074 6573 745f 6d75 6c74 695f 6e65  ef test_multi_ne
+00002b50: 7374 6564 5f65 6c65 6d65 6e74 5f5f 6261  sted_element__ba
+00002b60: 7369 635f 656c 656d 656e 745f 6368 696c  sic_element_chil
+00002b70: 645f 7465 7874 2863 6c61 7373 795f 786d  d_text(classy_xm
+00002b80: 6c5f 7465 7374 5f66 6978 7475 7265 293a  l_test_fixture):
+00002b90: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+00002ba0: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+00002bb0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00002bc0: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
+00002bd0: 6d65 6e74 5b30 5d2e 6261 7369 635f 656c  ment[0].basic_el
+00002be0: 656d 656e 745f 6368 696c 642e 7465 7874  ement_child.text
+00002bf0: 0d0a 2020 2020 2020 2020 3d3d 2022 6261  ..        == "ba
+00002c00: 7369 635f 656c 656d 656e 745f 6368 696c  sic_element_chil
+00002c10: 645f 305f 7465 7874 220d 0a20 2020 2029  d_0_text"..    )
+00002c20: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+00002c30: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+00002c40: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00002c50: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
+00002c60: 6d65 6e74 5b31 5d2e 6261 7369 635f 656c  ment[1].basic_el
+00002c70: 656d 656e 745f 6368 696c 642e 7465 7874  ement_child.text
+00002c80: 0d0a 2020 2020 2020 2020 3d3d 2022 6261  ..        == "ba
+00002c90: 7369 635f 656c 656d 656e 745f 6368 696c  sic_element_chil
+00002ca0: 645f 315f 7465 7874 220d 0a20 2020 2029  d_1_text"..    )
+00002cb0: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f6d  ......def test_m
+00002cc0: 756c 7469 5f6e 6573 7465 645f 656c 656d  ulti_nested_elem
+00002cd0: 656e 745f 5f6d 756c 7469 5f65 6c65 6d65  ent__multi_eleme
+00002ce0: 6e74 5f63 6869 6c64 5f6c 656e 6774 6828  nt_child_length(
+00002cf0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00002d00: 6669 7874 7572 6529 3a0d 0a20 2020 2061  fixture):..    a
+00002d10: 7373 6572 7420 6c65 6e28 636c 6173 7379  ssert len(classy
+00002d20: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00002d30: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00002d40: 6c65 6d65 6e74 5b30 5d2e 6d75 6c74 695f  lement[0].multi_
+00002d50: 656c 656d 656e 745f 6368 696c 6429 203d  element_child) =
+00002d60: 3d20 320d 0a20 2020 2061 7373 6572 7420  = 2..    assert 
+00002d70: 6c65 6e28 636c 6173 7379 5f78 6d6c 5f74  len(classy_xml_t
+00002d80: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
+00002d90: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
+00002da0: 5b31 5d2e 6d75 6c74 695f 656c 656d 656e  [1].multi_elemen
+00002db0: 745f 6368 696c 6429 203d 3d20 320d 0a0d  t_child) == 2...
+00002dc0: 0a0d 0a64 6566 2074 6573 745f 6d75 6c74  ...def test_mult
+00002dd0: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
+00002de0: 5f5f 6d75 6c74 695f 656c 656d 656e 745f  __multi_element_
+00002df0: 6368 696c 645f 7465 7874 2863 6c61 7373  child_text(class
+00002e00: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00002e10: 7265 293a 0d0a 2020 2020 6173 7365 7274  re):..    assert
+00002e20: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00002e30: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00002e40: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+00002e50: 5f65 6c65 6d65 6e74 5b30 5d2e 6d75 6c74  _element[0].mult
+00002e60: 695f 656c 656d 656e 745f 6368 696c 645b  i_element_child[
+00002e70: 305d 2e74 6578 740d 0a20 2020 2020 2020  0].text..       
+00002e80: 203d 3d20 226d 756c 7469 5f65 6c65 6d65   == "multi_eleme
+00002e90: 6e74 5f63 6869 6c64 5f30 5f74 6578 745f  nt_child_0_text_
+00002ea0: 3022 0d0a 2020 2020 290d 0a20 2020 2061  0"..    )..    a
+00002eb0: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+00002ec0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00002ed0: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
+00002ee0: 6573 7465 645f 656c 656d 656e 745b 305d  ested_element[0]
+00002ef0: 2e6d 756c 7469 5f65 6c65 6d65 6e74 5f63  .multi_element_c
+00002f00: 6869 6c64 5b31 5d2e 7465 7874 0d0a 2020  hild[1].text..  
+00002f10: 2020 2020 2020 3d3d 2022 6d75 6c74 695f        == "multi_
+00002f20: 656c 656d 656e 745f 6368 696c 645f 305f  element_child_0_
+00002f30: 7465 7874 5f31 220d 0a20 2020 2029 0d0a  text_1"..    )..
+00002f40: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+00002f50: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00002f60: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00002f70: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00002f80: 6e74 5b31 5d2e 6d75 6c74 695f 656c 656d  nt[1].multi_elem
+00002f90: 656e 745f 6368 696c 645b 305d 2e74 6578  ent_child[0].tex
+00002fa0: 740d 0a20 2020 2020 2020 203d 3d20 226d  t..        == "m
+00002fb0: 756c 7469 5f65 6c65 6d65 6e74 5f63 6869  ulti_element_chi
+00002fc0: 6c64 5f31 5f74 6578 745f 3022 0d0a 2020  ld_1_text_0"..  
+00002fd0: 2020 290d 0a20 2020 2061 7373 6572 7420    )..    assert 
+00002fe0: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
+00002ff0: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00003000: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
+00003010: 656c 656d 656e 745b 315d 2e6d 756c 7469  element[1].multi
+00003020: 5f65 6c65 6d65 6e74 5f63 6869 6c64 5b31  _element_child[1
+00003030: 5d2e 7465 7874 0d0a 2020 2020 2020 2020  ].text..        
+00003040: 3d3d 2022 6d75 6c74 695f 656c 656d 656e  == "multi_elemen
+00003050: 745f 6368 696c 645f 315f 7465 7874 5f31  t_child_1_text_1
+00003060: 220d 0a20 2020 2029 0d0a 0d0a 0d0a 6465  "..    )......de
+00003070: 6620 7465 7374 5f6d 756c 7469 5f6e 6573  f test_multi_nes
+00003080: 7465 645f 656c 656d 656e 745f 5f65 6d70  ted_element__emp
+00003090: 7479 5f65 6c65 6d65 6e74 5f77 6974 685f  ty_element_with_
+000030a0: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+000030b0: 5f6c 656e 6774 6828 0d0a 2020 2020 636c  _length(..    cl
+000030c0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+000030d0: 7874 7572 652c 0d0a 293a 0d0a 2020 2020  xture,..):..    
+000030e0: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+000030f0: 2020 6c65 6e28 0d0a 2020 2020 2020 2020    len(..        
+00003100: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00003110: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
+00003120: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
+00003130: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00003140: 2020 2030 0d0a 2020 2020 2020 2020 2020     0..          
+00003150: 2020 5d2e 656d 7074 795f 656c 656d 656e    ].empty_elemen
+00003160: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00003170: 735f 6368 696c 640d 0a20 2020 2020 2020  s_child..       
+00003180: 2029 0d0a 2020 2020 2020 2020 3d3d 2031   )..        == 1
+00003190: 0d0a 2020 2020 290d 0a20 2020 2061 7373  ..    )..    ass
+000031a0: 6572 7420 280d 0a20 2020 2020 2020 206c  ert (..        l
+000031b0: 656e 280d 0a20 2020 2020 2020 2020 2020  en(..           
+000031c0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+000031d0: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
+000031e0: 6573 7465 645f 656c 656d 656e 745b 0d0a  ested_element[..
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 310d 0a20 2020 2020 2020 2020 2020 205d  1..            ]
+00003210: 2e65 6d70 7479 5f65 6c65 6d65 6e74 5f77  .empty_element_w
+00003220: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+00003230: 6869 6c64 0d0a 2020 2020 2020 2020 290d  hild..        ).
+00003240: 0a20 2020 2020 2020 203d 3d20 310d 0a20  .        == 1.. 
+00003250: 2020 2029 0d0a 0d0a 0d0a 6465 6620 7465     )......def te
+00003260: 7374 5f6d 756c 7469 5f6e 6573 7465 645f  st_multi_nested_
+00003270: 656c 656d 656e 745f 5f65 6d70 7479 5f65  element__empty_e
+00003280: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00003290: 6962 7574 6573 5f63 6869 6c64 5f74 6578  ibutes_child_tex
+000032a0: 7428 0d0a 2020 2020 636c 6173 7379 5f78  t(..    classy_x
+000032b0: 6d6c 5f74 6573 745f 6669 7874 7572 652c  ml_test_fixture,
+000032c0: 0d0a 293a 0d0a 2020 2020 6173 7365 7274  ..):..    assert
+000032d0: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+000032e0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000032f0: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+00003300: 5f65 6c65 6d65 6e74 5b0d 0a20 2020 2020  _element[..     
+00003310: 2020 2020 2020 2030 0d0a 2020 2020 2020         0..      
+00003320: 2020 5d2e 656d 7074 795f 656c 656d 656e    ].empty_elemen
+00003330: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00003340: 735f 6368 696c 642e 7465 7874 0d0a 2020  s_child.text..  
+00003350: 2020 2020 2020 6973 204e 6f6e 650d 0a20        is None.. 
+00003360: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00003370: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00003380: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00003390: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+000033a0: 5f65 6c65 6d65 6e74 5b0d 0a20 2020 2020  _element[..     
+000033b0: 2020 2020 2020 2031 0d0a 2020 2020 2020         1..      
+000033c0: 2020 5d2e 656d 7074 795f 656c 656d 656e    ].empty_elemen
+000033d0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+000033e0: 735f 6368 696c 642e 7465 7874 0d0a 2020  s_child.text..  
+000033f0: 2020 2020 2020 6973 204e 6f6e 650d 0a20        is None.. 
+00003400: 2020 2029 0d0a 0d0a 0d0a 6465 6620 7465     )......def te
+00003410: 7374 5f6d 756c 7469 5f6e 6573 7465 645f  st_multi_nested_
+00003420: 656c 656d 656e 745f 5f65 6d70 7479 5f65  element__empty_e
+00003430: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00003440: 6962 7574 6573 5f63 6869 6c64 5f61 7474  ibutes_child_att
+00003450: 7269 6275 7465 7328 0d0a 2020 2020 636c  ributes(..    cl
+00003460: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00003470: 7874 7572 652c 0d0a 293a 0d0a 2020 2020  xture,..):..    
+00003480: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+00003490: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+000034a0: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+000034b0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b0d  nested_element[.
+000034c0: 0a20 2020 2020 2020 2020 2020 2030 0d0a  .            0..
+000034d0: 2020 2020 2020 2020 5d2e 656d 7074 795f          ].empty_
+000034e0: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+000034f0: 7269 6275 7465 735f 6368 696c 642e 6e61  ributes_child.na
+00003500: 6d65 0d0a 2020 2020 2020 2020 3d3d 2022  me..        == "
+00003510: 6368 696c 645f 305f 6174 7472 5f6e 616d  child_0_attr_nam
+00003520: 6522 0d0a 2020 2020 290d 0a20 2020 2061  e"..    )..    a
+00003530: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+00003540: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00003550: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
+00003560: 6573 7465 645f 656c 656d 656e 745b 0d0a  ested_element[..
+00003570: 2020 2020 2020 2020 2020 2020 300d 0a20              0.. 
+00003580: 2020 2020 2020 205d 2e65 6d70 7479 5f65         ].empty_e
+00003590: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+000035a0: 6962 7574 6573 5f63 6869 6c64 2e76 616c  ibutes_child.val
+000035b0: 7565 0d0a 2020 2020 2020 2020 3d3d 2022  ue..        == "
+000035c0: 6368 696c 645f 305f 6174 7472 5f76 616c  child_0_attr_val
+000035d0: 7565 220d 0a20 2020 2029 0d0a 2020 2020  ue"..    )..    
+000035e0: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+000035f0: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00003600: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+00003610: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b0d  nested_element[.
+00003620: 0a20 2020 2020 2020 2020 2020 2031 0d0a  .            1..
+00003630: 2020 2020 2020 2020 5d2e 656d 7074 795f          ].empty_
+00003640: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00003650: 7269 6275 7465 735f 6368 696c 642e 6e61  ributes_child.na
+00003660: 6d65 0d0a 2020 2020 2020 2020 3d3d 2022  me..        == "
+00003670: 6368 696c 645f 315f 6174 7472 5f6e 616d  child_1_attr_nam
+00003680: 6522 0d0a 2020 2020 290d 0a20 2020 2061  e"..    )..    a
+00003690: 7373 6572 7420 280d 0a20 2020 2020 2020  ssert (..       
+000036a0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+000036b0: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
+000036c0: 6573 7465 645f 656c 656d 656e 745b 0d0a  ested_element[..
+000036d0: 2020 2020 2020 2020 2020 2020 310d 0a20              1.. 
+000036e0: 2020 2020 2020 205d 2e65 6d70 7479 5f65         ].empty_e
+000036f0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00003700: 6962 7574 6573 5f63 6869 6c64 2e76 616c  ibutes_child.val
+00003710: 7565 0d0a 2020 2020 2020 2020 3d3d 2022  ue..        == "
+00003720: 6368 696c 645f 315f 6174 7472 5f76 616c  child_1_attr_val
+00003730: 7565 220d 0a20 2020 2029 0d0a 0d0a 0d0a  ue"..    )......
+00003740: 6465 6620 7465 7374 5f6d 756c 7469 5f6e  def test_multi_n
+00003750: 6573 7465 645f 656c 656d 656e 745f 5f65  ested_element__e
+00003760: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+00003770: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00003780: 6573 5f63 6869 6c64 5f6c 656e 6774 6828  es_child_length(
+00003790: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+000037a0: 5f74 6573 745f 6669 7874 7572 652c 0d0a  _test_fixture,..
+000037b0: 293a 0d0a 2020 2020 6173 7365 7274 2028  ):..    assert (
+000037c0: 0d0a 2020 2020 2020 2020 6c65 6e28 0d0a  ..        len(..
+000037d0: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+000037e0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000037f0: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+00003800: 5f65 6c65 6d65 6e74 5b0d 0a20 2020 2020  _element[..     
+00003810: 2020 2020 2020 2020 2020 2030 0d0a 2020             0..  
+00003820: 2020 2020 2020 2020 2020 5d2e 656d 7074            ].empt
+00003830: 795f 6d75 6c74 695f 656c 656d 656e 745f  y_multi_element_
+00003840: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00003850: 6368 696c 640d 0a20 2020 2020 2020 2029  child..        )
+00003860: 0d0a 2020 2020 2020 2020 3d3d 2032 0d0a  ..        == 2..
+00003870: 2020 2020 290d 0a20 2020 2061 7373 6572      )..    asser
+00003880: 7420 280d 0a20 2020 2020 2020 206c 656e  t (..        len
+00003890: 280d 0a20 2020 2020 2020 2020 2020 2063  (..            c
+000038a0: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+000038b0: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
+000038c0: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
+000038d0: 2020 2020 2020 2020 2020 2020 2020 310d                1.
+000038e0: 0a20 2020 2020 2020 2020 2020 205d 2e65  .            ].e
+000038f0: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+00003900: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00003910: 6573 5f63 6869 6c64 0d0a 2020 2020 2020  es_child..      
+00003920: 2020 290d 0a20 2020 2020 2020 203d 3d20    )..        == 
+00003930: 320d 0a20 2020 2029 0d0a 0d0a 0d0a 6465  2..    )......de
+00003940: 6620 7465 7374 5f6d 756c 7469 5f6e 6573  f test_multi_nes
+00003950: 7465 645f 656c 656d 656e 745f 5f65 6d70  ted_element__emp
+00003960: 7479 5f6d 756c 7469 5f65 6c65 6d65 6e74  ty_multi_element
+00003970: 5f77 6974 685f 6174 7472 6962 7574 6573  _with_attributes
+00003980: 5f63 6869 6c64 5f74 6578 7428 0d0a 2020  _child_text(..  
+00003990: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+000039a0: 745f 6669 7874 7572 652c 0d0a 293a 0d0a  t_fixture,..):..
+000039b0: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+000039c0: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+000039d0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+000039e0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+000039f0: 6e74 5b30 5d0d 0a20 2020 2020 2020 202e  nt[0]..        .
+00003a00: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
+00003a10: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00003a20: 7465 735f 6368 696c 645b 305d 0d0a 2020  tes_child[0]..  
+00003a30: 2020 2020 2020 2e74 6578 740d 0a20 2020        .text..   
+00003a40: 2020 2020 2069 7320 4e6f 6e65 0d0a 2020       is None..  
+00003a50: 2020 290d 0a20 2020 2061 7373 6572 7420    )..    assert 
+00003a60: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
+00003a70: 795f 786d 6c5f 7465 7374 5f66 6978 7475  y_xml_test_fixtu
+00003a80: 7265 2e6d 756c 7469 5f6e 6573 7465 645f  re.multi_nested_
+00003a90: 656c 656d 656e 745b 305d 0d0a 2020 2020  element[0]..    
+00003aa0: 2020 2020 2e65 6d70 7479 5f6d 756c 7469      .empty_multi
+00003ab0: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+00003ac0: 7472 6962 7574 6573 5f63 6869 6c64 5b31  tributes_child[1
+00003ad0: 5d0d 0a20 2020 2020 2020 202e 7465 7874  ]..        .text
+00003ae0: 0d0a 2020 2020 2020 2020 6973 204e 6f6e  ..        is Non
+00003af0: 650d 0a20 2020 2029 0d0a 2020 2020 6173  e..    )..    as
+00003b00: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+00003b10: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00003b20: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
+00003b30: 7374 6564 5f65 6c65 6d65 6e74 5b31 5d0d  sted_element[1].
+00003b40: 0a20 2020 2020 2020 202e 656d 7074 795f  .        .empty_
+00003b50: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+00003b60: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
+00003b70: 696c 645b 305d 0d0a 2020 2020 2020 2020  ild[0]..        
+00003b80: 2e74 6578 740d 0a20 2020 2020 2020 2069  .text..        i
+00003b90: 7320 4e6f 6e65 0d0a 2020 2020 290d 0a20  s None..    ).. 
+00003ba0: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00003bb0: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00003bc0: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
+00003bd0: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
+00003be0: 745b 315d 0d0a 2020 2020 2020 2020 2e65  t[1]..        .e
+00003bf0: 6d70 7479 5f6d 756c 7469 5f65 6c65 6d65  mpty_multi_eleme
+00003c00: 6e74 5f77 6974 685f 6174 7472 6962 7574  nt_with_attribut
+00003c10: 6573 5f63 6869 6c64 5b31 5d0d 0a20 2020  es_child[1]..   
+00003c20: 2020 2020 202e 7465 7874 0d0a 2020 2020       .text..    
+00003c30: 2020 2020 6973 204e 6f6e 650d 0a20 2020      is None..   
+00003c40: 2029 0d0a 0d0a 0d0a 6465 6620 7465 7374   )......def test
+00003c50: 5f6d 756c 7469 5f6e 6573 7465 645f 656c  _multi_nested_el
+00003c60: 656d 656e 745f 5f65 6d70 7479 5f6d 756c  ement__empty_mul
+00003c70: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00003c80: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+00003c90: 5f61 7474 7269 6275 7465 7328 0d0a 2020  _attributes(..  
+00003ca0: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00003cb0: 745f 6669 7874 7572 652c 0d0a 293a 0d0a  t_fixture,..):..
+00003cc0: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+00003cd0: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00003ce0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00003cf0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00003d00: 6e74 5b30 5d0d 0a20 2020 2020 2020 202e  nt[0]..        .
+00003d10: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
+00003d20: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00003d30: 7465 735f 6368 696c 645b 305d 0d0a 2020  tes_child[0]..  
+00003d40: 2020 2020 2020 2e6e 616d 650d 0a20 2020        .name..   
+00003d50: 2020 2020 203d 3d20 2263 6869 6c64 5f30       == "child_0
+00003d60: 5f61 7474 725f 305f 6e61 6d65 220d 0a20  _attr_0_name".. 
+00003d70: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00003d80: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00003d90: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00003da0: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+00003db0: 5f65 6c65 6d65 6e74 5b30 5d0d 0a20 2020  _element[0]..   
+00003dc0: 2020 2020 202e 656d 7074 795f 6d75 6c74       .empty_mult
+00003dd0: 695f 656c 656d 656e 745f 7769 7468 5f61  i_element_with_a
+00003de0: 7474 7269 6275 7465 735f 6368 696c 645b  ttributes_child[
+00003df0: 305d 0d0a 2020 2020 2020 2020 2e76 616c  0]..        .val
+00003e00: 7565 0d0a 2020 2020 2020 2020 3d3d 2022  ue..        == "
+00003e10: 6368 696c 645f 305f 6174 7472 5f30 5f76  child_0_attr_0_v
+00003e20: 616c 7565 220d 0a20 2020 2029 0d0a 2020  alue"..    )..  
+00003e30: 2020 6173 7365 7274 2028 0d0a 2020 2020    assert (..    
+00003e40: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00003e50: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
+00003e60: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
+00003e70: 5b30 5d0d 0a20 2020 2020 2020 202e 656d  [0]..        .em
+00003e80: 7074 795f 6d75 6c74 695f 656c 656d 656e  pty_multi_elemen
+00003e90: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00003ea0: 735f 6368 696c 645b 315d 0d0a 2020 2020  s_child[1]..    
+00003eb0: 2020 2020 2e6e 616d 650d 0a20 2020 2020      .name..     
+00003ec0: 2020 203d 3d20 2263 6869 6c64 5f30 5f61     == "child_0_a
+00003ed0: 7474 725f 315f 6e61 6d65 220d 0a20 2020  ttr_1_name"..   
+00003ee0: 2029 0d0a 2020 2020 6173 7365 7274 2028   )..    assert (
+00003ef0: 0d0a 2020 2020 2020 2020 636c 6173 7379  ..        classy
+00003f00: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00003f10: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00003f20: 6c65 6d65 6e74 5b30 5d0d 0a20 2020 2020  lement[0]..     
+00003f30: 2020 202e 656d 7074 795f 6d75 6c74 695f     .empty_multi_
+00003f40: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00003f50: 7269 6275 7465 735f 6368 696c 645b 315d  ributes_child[1]
+00003f60: 0d0a 2020 2020 2020 2020 2e76 616c 7565  ..        .value
+00003f70: 0d0a 2020 2020 2020 2020 3d3d 2022 6368  ..        == "ch
+00003f80: 696c 645f 305f 6174 7472 5f31 5f76 616c  ild_0_attr_1_val
+00003f90: 7565 220d 0a20 2020 2029 0d0a 2020 2020  ue"..    )..    
+00003fa0: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+00003fb0: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00003fc0: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+00003fd0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b31  nested_element[1
+00003fe0: 5d0d 0a20 2020 2020 2020 202e 656d 7074  ]..        .empt
+00003ff0: 795f 6d75 6c74 695f 656c 656d 656e 745f  y_multi_element_
+00004000: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00004010: 6368 696c 645b 305d 0d0a 2020 2020 2020  child[0]..      
+00004020: 2020 2e6e 616d 650d 0a20 2020 2020 2020    .name..       
+00004030: 203d 3d20 2263 6869 6c64 5f31 5f61 7474   == "child_1_att
+00004040: 725f 305f 6e61 6d65 220d 0a20 2020 2029  r_0_name"..    )
+00004050: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+00004060: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+00004070: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00004080: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
+00004090: 6d65 6e74 5b31 5d0d 0a20 2020 2020 2020  ment[1]..       
+000040a0: 202e 656d 7074 795f 6d75 6c74 695f 656c   .empty_multi_el
+000040b0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+000040c0: 6275 7465 735f 6368 696c 645b 305d 0d0a  butes_child[0]..
+000040d0: 2020 2020 2020 2020 2e76 616c 7565 0d0a          .value..
+000040e0: 2020 2020 2020 2020 3d3d 2022 6368 696c          == "chil
+000040f0: 645f 315f 6174 7472 5f30 5f76 616c 7565  d_1_attr_0_value
+00004100: 220d 0a20 2020 2029 0d0a 2020 2020 6173  "..    )..    as
+00004110: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+00004120: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00004130: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
+00004140: 7374 6564 5f65 6c65 6d65 6e74 5b31 5d0d  sted_element[1].
+00004150: 0a20 2020 2020 2020 202e 656d 7074 795f  .        .empty_
+00004160: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+00004170: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
+00004180: 696c 645b 315d 0d0a 2020 2020 2020 2020  ild[1]..        
+00004190: 2e6e 616d 650d 0a20 2020 2020 2020 203d  .name..        =
+000041a0: 3d20 2263 6869 6c64 5f31 5f61 7474 725f  = "child_1_attr_
+000041b0: 315f 6e61 6d65 220d 0a20 2020 2029 0d0a  1_name"..    )..
+000041c0: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+000041d0: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+000041e0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+000041f0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00004200: 6e74 5b31 5d0d 0a20 2020 2020 2020 202e  nt[1]..        .
+00004210: 656d 7074 795f 6d75 6c74 695f 656c 656d  empty_multi_elem
+00004220: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00004230: 7465 735f 6368 696c 645b 315d 0d0a 2020  tes_child[1]..  
+00004240: 2020 2020 2020 2e76 616c 7565 0d0a 2020        .value..  
+00004250: 2020 2020 2020 3d3d 2022 6368 696c 645f        == "child_
+00004260: 315f 6174 7472 5f31 5f76 616c 7565 220d  1_attr_1_value".
+00004270: 0a20 2020 2029 0d0a 0d0a 0d0a 6465 6620  .    )......def 
+00004280: 7465 7374 5f6d 756c 7469 5f6e 6573 7465  test_multi_neste
+00004290: 645f 656c 656d 656e 745f 5f62 6173 6963  d_element__basic
+000042a0: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+000042b0: 7472 6962 7574 6573 5f63 6869 6c64 5f6c  tributes_child_l
+000042c0: 656e 6774 6828 0d0a 2020 2020 636c 6173  ength(..    clas
+000042d0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000042e0: 7572 652c 0d0a 293a 0d0a 2020 2020 6173  ure,..):..    as
+000042f0: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+00004300: 6c65 6e28 0d0a 2020 2020 2020 2020 2020  len(..          
+00004310: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00004320: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+00004330: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b0d  nested_element[.
+00004340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004350: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+00004360: 5d2e 6261 7369 635f 656c 656d 656e 745f  ].basic_element_
+00004370: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00004380: 6368 696c 640d 0a20 2020 2020 2020 2029  child..        )
+00004390: 0d0a 2020 2020 2020 2020 3d3d 2031 0d0a  ..        == 1..
+000043a0: 2020 2020 290d 0a20 2020 2061 7373 6572      )..    asser
+000043b0: 7420 280d 0a20 2020 2020 2020 206c 656e  t (..        len
+000043c0: 280d 0a20 2020 2020 2020 2020 2020 2063  (..            c
+000043d0: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+000043e0: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
+000043f0: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
+00004400: 2020 2020 2020 2020 2020 2020 2020 310d                1.
+00004410: 0a20 2020 2020 2020 2020 2020 205d 2e62  .            ].b
+00004420: 6173 6963 5f65 6c65 6d65 6e74 5f77 6974  asic_element_wit
+00004430: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
+00004440: 6c64 0d0a 2020 2020 2020 2020 290d 0a20  ld..        ).. 
+00004450: 2020 2020 2020 203d 3d20 310d 0a20 2020         == 1..   
+00004460: 2029 0d0a 0d0a 0d0a 6465 6620 7465 7374   )......def test
+00004470: 5f6d 756c 7469 5f6e 6573 7465 645f 656c  _multi_nested_el
+00004480: 656d 656e 745f 5f62 6173 6963 5f65 6c65  ement__basic_ele
+00004490: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+000044a0: 7574 6573 5f63 6869 6c64 5f74 6578 7428  utes_child_text(
+000044b0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+000044c0: 5f74 6573 745f 6669 7874 7572 652c 0d0a  _test_fixture,..
+000044d0: 293a 0d0a 2020 2020 6173 7365 7274 2028  ):..    assert (
+000044e0: 0d0a 2020 2020 2020 2020 636c 6173 7379  ..        classy
+000044f0: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00004500: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00004510: 6c65 6d65 6e74 5b0d 0a20 2020 2020 2020  lement[..       
+00004520: 2020 2020 2030 0d0a 2020 2020 2020 2020       0..        
+00004530: 5d2e 6261 7369 635f 656c 656d 656e 745f  ].basic_element_
+00004540: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00004550: 6368 696c 642e 7465 7874 0d0a 2020 2020  child.text..    
+00004560: 2020 2020 3d3d 2022 6261 7369 635f 656c      == "basic_el
+00004570: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+00004580: 6275 7465 735f 6368 696c 645f 305f 7465  butes_child_0_te
+00004590: 7874 220d 0a20 2020 2029 0d0a 2020 2020  xt"..    )..    
+000045a0: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+000045b0: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+000045c0: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+000045d0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b0d  nested_element[.
+000045e0: 0a20 2020 2020 2020 2020 2020 2031 0d0a  .            1..
+000045f0: 2020 2020 2020 2020 5d2e 6261 7369 635f          ].basic_
+00004600: 656c 656d 656e 745f 7769 7468 5f61 7474  element_with_att
+00004610: 7269 6275 7465 735f 6368 696c 642e 7465  ributes_child.te
+00004620: 7874 0d0a 2020 2020 2020 2020 3d3d 2022  xt..        == "
+00004630: 6261 7369 635f 656c 656d 656e 745f 7769  basic_element_wi
+00004640: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
+00004650: 696c 645f 315f 7465 7874 220d 0a20 2020  ild_1_text"..   
+00004660: 2029 0d0a 0d0a 0d0a 6465 6620 7465 7374   )......def test
+00004670: 5f6d 756c 7469 5f6e 6573 7465 645f 656c  _multi_nested_el
+00004680: 656d 656e 745f 5f62 6173 6963 5f65 6c65  ement__basic_ele
+00004690: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+000046a0: 7574 6573 5f63 6869 6c64 5f61 7474 7269  utes_child_attri
+000046b0: 6275 7465 7328 0d0a 2020 2020 636c 6173  butes(..    clas
+000046c0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000046d0: 7572 652c 0d0a 293a 0d0a 2020 2020 6173  ure,..):..    as
+000046e0: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+000046f0: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00004700: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
+00004710: 7374 6564 5f65 6c65 6d65 6e74 5b0d 0a20  sted_element[.. 
+00004720: 2020 2020 2020 2020 2020 2030 0d0a 2020             0..  
+00004730: 2020 2020 2020 5d2e 6261 7369 635f 656c        ].basic_el
+00004740: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+00004750: 6275 7465 735f 6368 696c 642e 6e61 6d65  butes_child.name
+00004760: 0d0a 2020 2020 2020 2020 3d3d 2022 6368  ..        == "ch
+00004770: 696c 645f 305f 6174 7472 5f6e 616d 6522  ild_0_attr_name"
+00004780: 0d0a 2020 2020 290d 0a20 2020 2061 7373  ..    )..    ass
+00004790: 6572 7420 280d 0a20 2020 2020 2020 2063  ert (..        c
+000047a0: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+000047b0: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
+000047c0: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
+000047d0: 2020 2020 2020 2020 2020 300d 0a20 2020            0..   
+000047e0: 2020 2020 205d 2e62 6173 6963 5f65 6c65       ].basic_ele
+000047f0: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00004800: 7574 6573 5f63 6869 6c64 2e76 616c 7565  utes_child.value
+00004810: 0d0a 2020 2020 2020 2020 3d3d 2022 6368  ..        == "ch
+00004820: 696c 645f 305f 6174 7472 5f76 616c 7565  ild_0_attr_value
+00004830: 220d 0a20 2020 2029 0d0a 2020 2020 6173  "..    )..    as
+00004840: 7365 7274 2028 0d0a 2020 2020 2020 2020  sert (..        
+00004850: 636c 6173 7379 5f78 6d6c 5f74 6573 745f  classy_xml_test_
+00004860: 6669 7874 7572 652e 6d75 6c74 695f 6e65  fixture.multi_ne
+00004870: 7374 6564 5f65 6c65 6d65 6e74 5b0d 0a20  sted_element[.. 
+00004880: 2020 2020 2020 2020 2020 2031 0d0a 2020             1..  
+00004890: 2020 2020 2020 5d2e 6261 7369 635f 656c        ].basic_el
+000048a0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+000048b0: 6275 7465 735f 6368 696c 642e 6e61 6d65  butes_child.name
+000048c0: 0d0a 2020 2020 2020 2020 3d3d 2022 6368  ..        == "ch
+000048d0: 696c 645f 315f 6174 7472 5f6e 616d 6522  ild_1_attr_name"
+000048e0: 0d0a 2020 2020 290d 0a20 2020 2061 7373  ..    )..    ass
+000048f0: 6572 7420 280d 0a20 2020 2020 2020 2063  ert (..        c
+00004900: 6c61 7373 795f 786d 6c5f 7465 7374 5f66  lassy_xml_test_f
+00004910: 6978 7475 7265 2e6d 756c 7469 5f6e 6573  ixture.multi_nes
+00004920: 7465 645f 656c 656d 656e 745b 0d0a 2020  ted_element[..  
+00004930: 2020 2020 2020 2020 2020 310d 0a20 2020            1..   
+00004940: 2020 2020 205d 2e62 6173 6963 5f65 6c65       ].basic_ele
+00004950: 6d65 6e74 5f77 6974 685f 6174 7472 6962  ment_with_attrib
+00004960: 7574 6573 5f63 6869 6c64 2e76 616c 7565  utes_child.value
+00004970: 0d0a 2020 2020 2020 2020 3d3d 2022 6368  ..        == "ch
+00004980: 696c 645f 315f 6174 7472 5f76 616c 7565  ild_1_attr_value
+00004990: 220d 0a20 2020 2029 0d0a 0d0a 0d0a 6465  "..    )......de
+000049a0: 6620 7465 7374 5f6d 756c 7469 5f6e 6573  f test_multi_nes
+000049b0: 7465 645f 656c 656d 656e 745f 5f6d 756c  ted_element__mul
+000049c0: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+000049d0: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+000049e0: 5f6c 656e 6774 6828 0d0a 2020 2020 636c  _length(..    cl
+000049f0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00004a00: 7874 7572 652c 0d0a 293a 0d0a 2020 2020  xture,..):..    
+00004a10: 6173 7365 7274 2028 0d0a 2020 2020 2020  assert (..      
+00004a20: 2020 6c65 6e28 0d0a 2020 2020 2020 2020    len(..        
+00004a30: 2020 2020 636c 6173 7379 5f78 6d6c 5f74      classy_xml_t
+00004a40: 6573 745f 6669 7874 7572 652e 6d75 6c74  est_fixture.mult
+00004a50: 695f 6e65 7374 6564 5f65 6c65 6d65 6e74  i_nested_element
+00004a60: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00004a70: 2020 2030 0d0a 2020 2020 2020 2020 2020     0..          
+00004a80: 2020 5d2e 6d75 6c74 695f 656c 656d 656e    ].multi_elemen
+00004a90: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00004aa0: 735f 6368 696c 640d 0a20 2020 2020 2020  s_child..       
+00004ab0: 2029 0d0a 2020 2020 2020 2020 3d3d 2032   )..        == 2
+00004ac0: 0d0a 2020 2020 290d 0a20 2020 2061 7373  ..    )..    ass
+00004ad0: 6572 7420 280d 0a20 2020 2020 2020 206c  ert (..        l
+00004ae0: 656e 280d 0a20 2020 2020 2020 2020 2020  en(..           
+00004af0: 2063 6c61 7373 795f 786d 6c5f 7465 7374   classy_xml_test
+00004b00: 5f66 6978 7475 7265 2e6d 756c 7469 5f6e  _fixture.multi_n
+00004b10: 6573 7465 645f 656c 656d 656e 745b 0d0a  ested_element[..
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 310d 0a20 2020 2020 2020 2020 2020 205d  1..            ]
+00004b40: 2e6d 756c 7469 5f65 6c65 6d65 6e74 5f77  .multi_element_w
+00004b50: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+00004b60: 6869 6c64 0d0a 2020 2020 2020 2020 290d  hild..        ).
+00004b70: 0a20 2020 2020 2020 203d 3d20 320d 0a20  .        == 2.. 
+00004b80: 2020 2029 0d0a 0d0a 0d0a 6465 6620 7465     )......def te
+00004b90: 7374 5f6d 756c 7469 5f6e 6573 7465 645f  st_multi_nested_
+00004ba0: 656c 656d 656e 745f 5f6d 756c 7469 5f65  element__multi_e
+00004bb0: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00004bc0: 6962 7574 6573 5f63 6869 6c64 5f74 6578  ibutes_child_tex
+00004bd0: 7428 0d0a 2020 2020 636c 6173 7379 5f78  t(..    classy_x
+00004be0: 6d6c 5f74 6573 745f 6669 7874 7572 652c  ml_test_fixture,
+00004bf0: 0d0a 293a 0d0a 2020 2020 6173 7365 7274  ..):..    assert
+00004c00: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00004c10: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00004c20: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+00004c30: 5f65 6c65 6d65 6e74 5b30 5d0d 0a20 2020  _element[0]..   
+00004c40: 2020 2020 202e 6d75 6c74 695f 656c 656d       .multi_elem
+00004c50: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00004c60: 7465 735f 6368 696c 645b 305d 0d0a 2020  tes_child[0]..  
+00004c70: 2020 2020 2020 2e74 6578 740d 0a20 2020        .text..   
+00004c80: 2020 2020 203d 3d20 226d 756c 7469 5f65       == "multi_e
+00004c90: 6c65 6d65 6e74 5f77 6974 685f 6174 7472  lement_with_attr
+00004ca0: 6962 7574 6573 5f63 6869 6c64 5f30 5f74  ibutes_child_0_t
+00004cb0: 6578 745f 3022 0d0a 2020 2020 290d 0a20  ext_0"..    ).. 
+00004cc0: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00004cd0: 2020 2020 2063 6c61 7373 795f 786d 6c5f       classy_xml_
+00004ce0: 7465 7374 5f66 6978 7475 7265 2e6d 756c  test_fixture.mul
+00004cf0: 7469 5f6e 6573 7465 645f 656c 656d 656e  ti_nested_elemen
+00004d00: 745b 305d 0d0a 2020 2020 2020 2020 2e6d  t[0]..        .m
+00004d10: 756c 7469 5f65 6c65 6d65 6e74 5f77 6974  ulti_element_wit
+00004d20: 685f 6174 7472 6962 7574 6573 5f63 6869  h_attributes_chi
+00004d30: 6c64 5b31 5d0d 0a20 2020 2020 2020 202e  ld[1]..        .
+00004d40: 7465 7874 0d0a 2020 2020 2020 2020 3d3d  text..        ==
+00004d50: 2022 6d75 6c74 695f 656c 656d 656e 745f   "multi_element_
+00004d60: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00004d70: 6368 696c 645f 305f 7465 7874 5f31 220d  child_0_text_1".
+00004d80: 0a20 2020 2029 0d0a 2020 2020 6173 7365  .    )..    asse
+00004d90: 7274 2028 0d0a 2020 2020 2020 2020 636c  rt (..        cl
+00004da0: 6173 7379 5f78 6d6c 5f74 6573 745f 6669  assy_xml_test_fi
+00004db0: 7874 7572 652e 6d75 6c74 695f 6e65 7374  xture.multi_nest
+00004dc0: 6564 5f65 6c65 6d65 6e74 5b31 5d0d 0a20  ed_element[1].. 
+00004dd0: 2020 2020 2020 202e 6d75 6c74 695f 656c         .multi_el
+00004de0: 656d 656e 745f 7769 7468 5f61 7474 7269  ement_with_attri
+00004df0: 6275 7465 735f 6368 696c 645b 305d 0d0a  butes_child[0]..
+00004e00: 2020 2020 2020 2020 2e74 6578 740d 0a20          .text.. 
+00004e10: 2020 2020 2020 203d 3d20 226d 756c 7469         == "multi
+00004e20: 5f65 6c65 6d65 6e74 5f77 6974 685f 6174  _element_with_at
+00004e30: 7472 6962 7574 6573 5f63 6869 6c64 5f31  tributes_child_1
+00004e40: 5f74 6578 745f 3022 0d0a 2020 2020 290d  _text_0"..    ).
+00004e50: 0a20 2020 2061 7373 6572 7420 280d 0a20  .    assert (.. 
+00004e60: 2020 2020 2020 2063 6c61 7373 795f 786d         classy_xm
+00004e70: 6c5f 7465 7374 5f66 6978 7475 7265 2e6d  l_test_fixture.m
+00004e80: 756c 7469 5f6e 6573 7465 645f 656c 656d  ulti_nested_elem
+00004e90: 656e 745b 315d 0d0a 2020 2020 2020 2020  ent[1]..        
+00004ea0: 2e6d 756c 7469 5f65 6c65 6d65 6e74 5f77  .multi_element_w
+00004eb0: 6974 685f 6174 7472 6962 7574 6573 5f63  ith_attributes_c
+00004ec0: 6869 6c64 5b31 5d0d 0a20 2020 2020 2020  hild[1]..       
+00004ed0: 202e 7465 7874 0d0a 2020 2020 2020 2020   .text..        
+00004ee0: 3d3d 2022 6d75 6c74 695f 656c 656d 656e  == "multi_elemen
+00004ef0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00004f00: 735f 6368 696c 645f 315f 7465 7874 5f31  s_child_1_text_1
+00004f10: 220d 0a20 2020 2029 0d0a 0d0a 0d0a 6465  "..    )......de
+00004f20: 6620 7465 7374 5f6d 756c 7469 5f6e 6573  f test_multi_nes
+00004f30: 7465 645f 656c 656d 656e 745f 5f6d 756c  ted_element__mul
+00004f40: 7469 5f65 6c65 6d65 6e74 5f77 6974 685f  ti_element_with_
+00004f50: 6174 7472 6962 7574 6573 5f63 6869 6c64  attributes_child
+00004f60: 5f61 7474 7269 6275 7465 7328 0d0a 2020  _attributes(..  
+00004f70: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+00004f80: 745f 6669 7874 7572 652c 0d0a 293a 0d0a  t_fixture,..):..
+00004f90: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+00004fa0: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00004fb0: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00004fc0: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00004fd0: 6e74 5b30 5d0d 0a20 2020 2020 2020 202e  nt[0]..        .
+00004fe0: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+00004ff0: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
+00005000: 696c 645b 305d 0d0a 2020 2020 2020 2020  ild[0]..        
+00005010: 2e6e 616d 650d 0a20 2020 2020 2020 203d  .name..        =
+00005020: 3d20 2263 6869 6c64 5f30 5f61 7474 725f  = "child_0_attr_
+00005030: 305f 6e61 6d65 220d 0a20 2020 2029 0d0a  0_name"..    )..
+00005040: 2020 2020 6173 7365 7274 2028 0d0a 2020      assert (..  
+00005050: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00005060: 5f74 6573 745f 6669 7874 7572 652e 6d75  _test_fixture.mu
+00005070: 6c74 695f 6e65 7374 6564 5f65 6c65 6d65  lti_nested_eleme
+00005080: 6e74 5b30 5d0d 0a20 2020 2020 2020 202e  nt[0]..        .
+00005090: 6d75 6c74 695f 656c 656d 656e 745f 7769  multi_element_wi
+000050a0: 7468 5f61 7474 7269 6275 7465 735f 6368  th_attributes_ch
+000050b0: 696c 645b 305d 0d0a 2020 2020 2020 2020  ild[0]..        
+000050c0: 2e76 616c 7565 0d0a 2020 2020 2020 2020  .value..        
+000050d0: 3d3d 2022 6368 696c 645f 305f 6174 7472  == "child_0_attr
+000050e0: 5f30 5f76 616c 7565 220d 0a20 2020 2029  _0_value"..    )
+000050f0: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+00005100: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+00005110: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+00005120: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
+00005130: 6d65 6e74 5b30 5d0d 0a20 2020 2020 2020  ment[0]..       
+00005140: 202e 6d75 6c74 695f 656c 656d 656e 745f   .multi_element_
+00005150: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00005160: 6368 696c 645b 315d 0d0a 2020 2020 2020  child[1]..      
+00005170: 2020 2e6e 616d 650d 0a20 2020 2020 2020    .name..       
+00005180: 203d 3d20 2263 6869 6c64 5f30 5f61 7474   == "child_0_att
+00005190: 725f 315f 6e61 6d65 220d 0a20 2020 2029  r_1_name"..    )
+000051a0: 0d0a 2020 2020 6173 7365 7274 2028 0d0a  ..    assert (..
+000051b0: 2020 2020 2020 2020 636c 6173 7379 5f78          classy_x
+000051c0: 6d6c 5f74 6573 745f 6669 7874 7572 652e  ml_test_fixture.
+000051d0: 6d75 6c74 695f 6e65 7374 6564 5f65 6c65  multi_nested_ele
+000051e0: 6d65 6e74 5b30 5d0d 0a20 2020 2020 2020  ment[0]..       
+000051f0: 202e 6d75 6c74 695f 656c 656d 656e 745f   .multi_element_
+00005200: 7769 7468 5f61 7474 7269 6275 7465 735f  with_attributes_
+00005210: 6368 696c 645b 315d 0d0a 2020 2020 2020  child[1]..      
+00005220: 2020 2e76 616c 7565 0d0a 2020 2020 2020    .value..      
+00005230: 2020 3d3d 2022 6368 696c 645f 305f 6174    == "child_0_at
+00005240: 7472 5f31 5f76 616c 7565 220d 0a20 2020  tr_1_value"..   
+00005250: 2029 0d0a 2020 2020 6173 7365 7274 2028   )..    assert (
 00005260: 0d0a 2020 2020 2020 2020 636c 6173 7379  ..        classy
-00005270: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00005280: 7265 2e63 6c61 7373 795f 656c 656d 656e  re.classy_elemen
-00005290: 742e 786d 6c5f 656c 656d 656e 745b 315d  t.xml_element[1]
-000052a0: 2c20 586d 6c45 6c65 6d65 6e74 290d 0a20  , XmlElement).. 
-000052b0: 2020 2061 7373 6572 7420 6c65 6e28 636c     assert len(cl
-000052c0: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
-000052d0: 6978 7475 7265 2e63 6c61 7373 795f 656c  ixture.classy_el
-000052e0: 656d 656e 742e 786d 6c5f 656c 656d 656e  ement.xml_elemen
-000052f0: 7429 203d 3d20 320d 0a0d 0a0d 0a64 6566  t) == 2......def
-00005300: 2074 6573 745f 786d 6c5f 656c 656d 656e   test_xml_elemen
-00005310: 745f 7265 6d6f 7665 5f65 6c65 6d65 6e74  t_remove_element
-00005320: 5f61 7272 6179 2863 6c61 7373 795f 786d  _array(classy_xm
-00005330: 6c5f 656d 7074 795f 6669 7874 7572 6529  l_empty_fixture)
-00005340: 3a0d 0a20 2020 2063 6c61 7373 795f 786d  :..    classy_xm
-00005350: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00005360: 636c 6173 7379 5f65 6c65 6d65 6e74 203d  classy_element =
-00005370: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
-00005380: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-00005390: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-000053a0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-000053b0: 6c65 6d65 6e74 203d 2058 6d6c 456c 656d  lement = XmlElem
-000053c0: 656e 7428 290d 0a20 2020 2063 6c61 7373  ent()..    class
-000053d0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-000053e0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-000053f0: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 203d  nt.xml_element =
-00005400: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
-00005410: 2020 2064 656c 2063 6c61 7373 795f 786d     del classy_xm
-00005420: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00005430: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-00005440: 6d6c 5f65 6c65 6d65 6e74 5b30 5d0d 0a20  ml_element[0].. 
-00005450: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00005460: 616e 6365 280d 0a20 2020 2020 2020 2063  ance(..        c
-00005470: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00005480: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00005490: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-000054a0: 6e74 2c20 586d 6c45 6c65 6d65 6e74 290d  nt, XmlElement).
-000054b0: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
-000054c0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-000054d0: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-000054e0: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
-000054f0: 656e 7429 203d 3d20 310d 0a0d 0a0d 0a64  ent) == 1......d
-00005500: 6566 2074 6573 745f 786d 6c5f 656c 656d  ef test_xml_elem
-00005510: 656e 745f 6164 645f 7465 7874 2863 6c61  ent_add_text(cla
-00005520: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005530: 7874 7572 6529 3a0d 0a20 2020 2063 6c61  xture):..    cla
-00005540: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005550: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005560: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005570: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
-00005580: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-00005590: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-000055a0: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
-000055b0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
-000055c0: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-000055d0: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-000055e0: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-000055f0: 6d65 6e74 2e74 6578 7420 3d20 2774 6573  ment.text = 'tes
-00005600: 7427 0d0a 2020 2020 6173 7365 7274 2063  t'..    assert c
-00005610: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00005620: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00005630: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-00005640: 6e74 2e74 6578 7420 3d3d 2027 7465 7374  nt.text == 'test
-00005650: 270d 0a0d 0a0d 0a64 6566 2074 6573 745f  '......def test_
-00005660: 786d 6c5f 656c 656d 656e 745f 6368 616e  xml_element_chan
-00005670: 6765 5f74 6578 7428 636c 6173 7379 5f78  ge_text(classy_x
-00005680: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
-00005690: 293a 0d0a 2020 2020 636c 6173 7379 5f78  ):..    classy_x
-000056a0: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
-000056b0: 2e63 6c61 7373 795f 656c 656d 656e 7420  .classy_element 
-000056c0: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
-000056d0: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-000056e0: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-000056f0: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-00005700: 656c 656d 656e 7420 3d20 586d 6c45 6c65  element = XmlEle
-00005710: 6d65 6e74 2829 0d0a 2020 2020 636c 6173  ment()..    clas
-00005720: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
-00005730: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
-00005740: 656e 742e 786d 6c5f 656c 656d 656e 742e  ent.xml_element.
-00005750: 7465 7874 203d 2027 7465 7374 270d 0a20  text = 'test'.. 
-00005760: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-00005770: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-00005780: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-00005790: 6c65 6d65 6e74 2e74 6578 7420 3d20 2763  lement.text = 'c
-000057a0: 6861 6e67 6564 270d 0a20 2020 2061 7373  hanged'..    ass
-000057b0: 6572 7420 636c 6173 7379 5f78 6d6c 5f65  ert classy_xml_e
-000057c0: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-000057d0: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-000057e0: 656c 656d 656e 742e 7465 7874 203d 3d20  element.text == 
-000057f0: 2763 6861 6e67 6564 270d 0a0d 0a0d 0a64  'changed'......d
-00005800: 6566 2074 6573 745f 786d 6c5f 656c 656d  ef test_xml_elem
-00005810: 656e 745f 7265 6d6f 7665 5f74 6578 7428  ent_remove_text(
-00005820: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00005830: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
-00005840: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00005850: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-00005860: 656c 656d 656e 7420 3d20 586d 6c45 6c65  element = XmlEle
-00005870: 6d65 6e74 2829 0d0a 2020 2020 636c 6173  ment()..    clas
-00005880: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
-00005890: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
-000058a0: 656e 742e 786d 6c5f 656c 656d 656e 7420  ent.xml_element 
-000058b0: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
-000058c0: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-000058d0: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-000058e0: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-000058f0: 656c 656d 656e 742e 7465 7874 203d 2027  element.text = '
-00005900: 7465 7374 270d 0a20 2020 2064 656c 2063  test'..    del c
-00005910: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00005920: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00005930: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-00005940: 6e74 2e74 6578 740d 0a20 2020 2061 7373  nt.text..    ass
-00005950: 6572 7420 636c 6173 7379 5f78 6d6c 5f65  ert classy_xml_e
-00005960: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-00005970: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-00005980: 656c 656d 656e 742e 7465 7874 2069 7320  element.text is 
-00005990: 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620 7465  None......def te
-000059a0: 7374 5f78 6d6c 5f65 6c65 6d65 6e74 5f61  st_xml_element_a
-000059b0: 7272 6179 5f61 6464 5f74 6578 7428 636c  rray_add_text(cl
-000059c0: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
-000059d0: 6978 7475 7265 293a 0d0a 2020 2020 636c  ixture):..    cl
-000059e0: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
-000059f0: 6978 7475 7265 2e63 6c61 7373 795f 656c  ixture.classy_el
-00005a00: 656d 656e 7420 3d20 586d 6c45 6c65 6d65  ement = XmlEleme
-00005a10: 6e74 2829 0d0a 2020 2020 636c 6173 7379  nt()..    classy
-00005a20: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00005a30: 7265 2e63 6c61 7373 795f 656c 656d 656e  re.classy_elemen
-00005a40: 742e 786d 6c5f 656c 656d 656e 7420 3d20  t.xml_element = 
-00005a50: 586d 6c45 6c65 6d65 6e74 2829 0d0a 2020  XmlElement()..  
-00005a60: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
-00005a70: 7479 5f66 6978 7475 7265 2e63 6c61 7373  ty_fixture.class
-00005a80: 795f 656c 656d 656e 742e 786d 6c5f 656c  y_element.xml_el
-00005a90: 656d 656e 7420 3d20 586d 6c45 6c65 6d65  ement = XmlEleme
-00005aa0: 6e74 2829 0d0a 2020 2020 636c 6173 7379  nt()..    classy
-00005ab0: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00005ac0: 7265 2e63 6c61 7373 795f 656c 656d 656e  re.classy_elemen
-00005ad0: 742e 786d 6c5f 656c 656d 656e 745b 305d  t.xml_element[0]
-00005ae0: 2e74 6578 7420 3d20 2774 6573 7427 0d0a  .text = 'test'..
-00005af0: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-00005b00: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00005b10: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00005b20: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 5b30  nt.xml_element[0
-00005b30: 5d2e 7465 7874 203d 3d20 2774 6573 7427  ].text == 'test'
-00005b40: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00005b50: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005b60: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005b70: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-00005b80: 5b31 5d2e 7465 7874 2069 7320 4e6f 6e65  [1].text is None
-00005b90: 0d0a 0d0a 0d0a 6465 6620 7465 7374 5f78  ......def test_x
-00005ba0: 6d6c 5f65 6c65 6d65 6e74 5f61 7272 6179  ml_element_array
-00005bb0: 5f72 656d 6f76 655f 7465 7874 2863 6c61  _remove_text(cla
-00005bc0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005bd0: 7874 7572 6529 3a0d 0a20 2020 2063 6c61  xture):..    cla
-00005be0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005bf0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005c00: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005c10: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
-00005c20: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-00005c30: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-00005c40: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
-00005c50: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
-00005c60: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-00005c70: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-00005c80: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-00005c90: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005ca0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
-00005cb0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-00005cc0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-00005cd0: 2e78 6d6c 5f65 6c65 6d65 6e74 5b30 5d2e  .xml_element[0].
-00005ce0: 7465 7874 203d 2027 7465 7374 5f30 270d  text = 'test_0'.
-00005cf0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-00005d00: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-00005d10: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
-00005d20: 5f65 6c65 6d65 6e74 5b31 5d2e 7465 7874  _element[1].text
-00005d30: 203d 2027 7465 7374 5f31 270d 0a20 2020   = 'test_1'..   
-00005d40: 2064 656c 2063 6c61 7373 795f 786d 6c5f   del classy_xml_
-00005d50: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-00005d60: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
-00005d70: 5f65 6c65 6d65 6e74 5b30 5d2e 7465 7874  _element[0].text
-00005d80: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00005d90: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005da0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005db0: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-00005dc0: 5b30 5d2e 7465 7874 2069 7320 4e6f 6e65  [0].text is None
-00005dd0: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00005de0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005df0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005e00: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-00005e10: 5b31 5d2e 7465 7874 203d 3d20 2774 6573  [1].text == 'tes
-00005e20: 745f 3127 0d0a 0d0a 0d0a 6465 6620 7465  t_1'......def te
-00005e30: 7374 5f78 6d6c 5f65 6c65 6d65 6e74 5f61  st_xml_element_a
-00005e40: 6464 5f61 7474 7269 6275 7465 2863 6c61  dd_attribute(cla
-00005e50: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005e60: 7874 7572 6529 3a0d 0a20 2020 2063 6c61  xture):..    cla
-00005e70: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005e80: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005e90: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
-00005ea0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
-00005eb0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-00005ec0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-00005ed0: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
-00005ee0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
-00005ef0: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-00005f00: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-00005f10: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-00005f20: 6d65 6e74 2e6e 616d 6520 3d20 2774 6573  ment.name = 'tes
-00005f30: 745f 6e61 6d65 270d 0a20 2020 2063 6c61  t_name'..    cla
-00005f40: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00005f50: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-00005f60: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-00005f70: 2e76 616c 7565 203d 2031 0d0a 2020 2020  .value = 1..    
-00005f80: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
-00005f90: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00005fa0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-00005fb0: 6d6c 5f65 6c65 6d65 6e74 2e6e 616d 6520  ml_element.name 
-00005fc0: 3d3d 2027 7465 7374 5f6e 616d 6527 0d0a  == 'test_name'..
-00005fd0: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
-00005fe0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00005ff0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00006000: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 2e76  nt.xml_element.v
-00006010: 616c 7565 203d 3d20 2731 270d 0a0d 0a0d  alue == '1'.....
-00006020: 0a64 6566 2074 6573 745f 786d 6c5f 656c  .def test_xml_el
-00006030: 656d 656e 745f 6368 616e 6765 5f61 7474  ement_change_att
-00006040: 7269 6275 7465 2863 6c61 7373 795f 786d  ribute(classy_xm
-00006050: 6c5f 656d 7074 795f 6669 7874 7572 6529  l_empty_fixture)
-00006060: 3a0d 0a20 2020 2063 6c61 7373 795f 786d  :..    classy_xm
-00006070: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00006080: 636c 6173 7379 5f65 6c65 6d65 6e74 203d  classy_element =
-00006090: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
-000060a0: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-000060b0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-000060c0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-000060d0: 6c65 6d65 6e74 203d 2058 6d6c 456c 656d  lement = XmlElem
-000060e0: 656e 7428 290d 0a20 2020 2063 6c61 7373  ent()..    class
-000060f0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00006100: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00006110: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 2e6e  nt.xml_element.n
-00006120: 616d 6520 3d20 2774 6573 745f 6e61 6d65  ame = 'test_name
-00006130: 270d 0a20 2020 2063 6c61 7373 795f 786d  '..    classy_xm
-00006140: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00006150: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-00006160: 6d6c 5f65 6c65 6d65 6e74 2e6e 616d 6520  ml_element.name 
-00006170: 3d20 2763 6861 6e67 6564 5f6e 616d 6527  = 'changed_name'
-00006180: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
-00006190: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-000061a0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
-000061b0: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
-000061c0: 2e6e 616d 6520 3d3d 2027 6368 616e 6765  .name == 'change
-000061d0: 645f 6e61 6d65 270d 0a0d 0a0d 0a64 6566  d_name'......def
-000061e0: 2074 6573 745f 786d 6c5f 656c 656d 656e   test_xml_elemen
-000061f0: 745f 7265 6d6f 7665 5f61 7474 7269 6275  t_remove_attribu
-00006200: 7465 2863 6c61 7373 795f 786d 6c5f 656d  te(classy_xml_em
-00006210: 7074 795f 6669 7874 7572 6529 3a0d 0a20  pty_fixture):.. 
-00006220: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-00006230: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-00006240: 7379 5f65 6c65 6d65 6e74 203d 2058 6d6c  sy_element = Xml
-00006250: 456c 656d 656e 7428 290d 0a20 2020 2063  Element()..    c
-00006260: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00006270: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00006280: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-00006290: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
-000062a0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-000062b0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-000062c0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-000062d0: 6d6c 5f65 6c65 6d65 6e74 2e76 616c 7565  ml_element.value
-000062e0: 203d 2027 7465 7374 270d 0a20 2020 2064   = 'test'..    d
-000062f0: 656c 2063 6c61 7373 795f 786d 6c5f 656d  el classy_xml_em
-00006300: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-00006310: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-00006320: 6c65 6d65 6e74 2e76 616c 7565 0d0a 2020  lement.value..  
-00006330: 2020 6173 7365 7274 206e 6f74 2068 6173    assert not has
-00006340: 6174 7472 280d 0a20 2020 2020 2020 2063  attr(..        c
-00006350: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00006360: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00006370: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-00006380: 6e74 2c20 2776 616c 7565 2729 0d0a 0d0a  nt, 'value')....
-00006390: 0d0a 6465 6620 7465 7374 5f78 6d6c 5f65  ..def test_xml_e
-000063a0: 6c65 6d65 6e74 5f61 7272 6179 5f61 6464  lement_array_add
-000063b0: 5f61 7474 7269 6275 7465 2863 6c61 7373  _attribute(class
-000063c0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-000063d0: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
-000063e0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-000063f0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-00006400: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
-00006410: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-00006420: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00006430: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-00006440: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
-00006450: 456c 656d 656e 7428 290d 0a20 2020 2063  Element()..    c
-00006460: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00006470: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
-00006480: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
-00006490: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
-000064a0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-000064b0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-000064c0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
-000064d0: 6d6c 5f65 6c65 6d65 6e74 5b30 5d2e 6e61  ml_element[0].na
-000064e0: 6d65 203d 2027 7465 7374 5f6e 616d 655f  me = 'test_name_
-000064f0: 3027 0d0a 2020 2020 636c 6173 7379 5f78  0'..    classy_x
-00006500: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
-00006510: 2e63 6c61 7373 795f 656c 656d 656e 742e  .classy_element.
-00006520: 786d 6c5f 656c 656d 656e 745b 315d 2e6e  xml_element[1].n
-00006530: 616d 6520 3d20 2774 6573 745f 6e61 6d65  ame = 'test_name
-00006540: 5f31 270d 0a20 2020 2061 7373 6572 7420  _1'..    assert 
-00006550: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00006560: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-00006570: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
-00006580: 656e 745b 305d 2e6e 616d 6520 3d3d 2027  ent[0].name == '
-00006590: 7465 7374 5f6e 616d 655f 3027 0d0a 2020  test_name_0'..  
-000065a0: 2020 6173 7365 7274 2063 6c61 7373 795f    assert classy_
-000065b0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
-000065c0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
-000065d0: 2e78 6d6c 5f65 6c65 6d65 6e74 5b31 5d2e  .xml_element[1].
-000065e0: 6e61 6d65 203d 3d20 2774 6573 745f 6e61  name == 'test_na
-000065f0: 6d65 5f31 270d 0a0d 0a0d 0a64 6566 2074  me_1'......def t
-00006600: 6573 745f 786d 6c5f 656c 656d 656e 745f  est_xml_element_
-00006610: 6172 7261 795f 6368 616e 6765 5f61 7474  array_change_att
-00006620: 7269 6275 7465 2863 6c61 7373 795f 786d  ribute(classy_xm
-00006630: 6c5f 656d 7074 795f 6669 7874 7572 6529  l_empty_fixture)
-00006640: 3a0d 0a20 2020 2063 6c61 7373 795f 786d  :..    classy_xm
-00006650: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00006660: 636c 6173 7379 5f65 6c65 6d65 6e74 203d  classy_element =
-00006670: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
-00006680: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-00006690: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-000066a0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-000066b0: 6c65 6d65 6e74 203d 2058 6d6c 456c 656d  lement = XmlElem
-000066c0: 656e 7428 290d 0a20 2020 2063 6c61 7373  ent()..    class
-000066d0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-000066e0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
-000066f0: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 203d  nt.xml_element =
-00006700: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
-00006710: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
-00006720: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
-00006730: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
-00006740: 6c65 6d65 6e74 5b30 5d2e 6e61 6d65 203d  lement[0].name =
-00006750: 2027 7465 7374 5f6e 616d 655f 3027 0d0a   'test_name_0'..
-00006760: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-00006770: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-00006780: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-00006790: 656c 656d 656e 745b 315d 2e6e 616d 6520  element[1].name 
-000067a0: 3d20 2774 6573 745f 6e61 6d65 5f31 270d  = 'test_name_1'.
-000067b0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-000067c0: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-000067d0: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
-000067e0: 5f65 6c65 6d65 6e74 5b30 5d2e 6e61 6d65  _element[0].name
-000067f0: 203d 2027 7465 7374 5f6e 616d 655f 305f   = 'test_name_0_
-00006800: 6368 616e 6765 6427 0d0a 2020 2020 6173  changed'..    as
-00006810: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
-00006820: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
-00006830: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
-00006840: 5f65 6c65 6d65 6e74 5b30 5d2e 6e61 6d65  _element[0].name
-00006850: 203d 3d20 2774 6573 745f 6e61 6d65 5f30   == 'test_name_0
-00006860: 5f63 6861 6e67 6564 270d 0a20 2020 2061  _changed'..    a
-00006870: 7373 6572 7420 636c 6173 7379 5f78 6d6c  ssert classy_xml
-00006880: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
-00006890: 6c61 7373 795f 656c 656d 656e 742e 786d  lassy_element.xm
-000068a0: 6c5f 656c 656d 656e 745b 315d 2e6e 616d  l_element[1].nam
-000068b0: 6520 3d3d 2027 7465 7374 5f6e 616d 655f  e == 'test_name_
-000068c0: 3127 0d0a 0d0a 0d0a 6465 6620 7465 7374  1'......def test
-000068d0: 5f78 6d6c 5f65 6c65 6d65 6e74 5f61 7272  _xml_element_arr
-000068e0: 6179 5f72 656d 6f76 655f 6174 7472 6962  ay_remove_attrib
-000068f0: 7574 6528 636c 6173 7379 5f78 6d6c 5f65  ute(classy_xml_e
-00006900: 6d70 7479 5f66 6978 7475 7265 293a 0d0a  mpty_fixture):..
-00006910: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-00006920: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-00006930: 7373 795f 656c 656d 656e 7420 3d20 586d  ssy_element = Xm
-00006940: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
-00006950: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00006960: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-00006970: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
-00006980: 656e 7420 3d20 586d 6c45 6c65 6d65 6e74  ent = XmlElement
-00006990: 2829 0d0a 2020 2020 636c 6173 7379 5f78  ()..    classy_x
-000069a0: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
-000069b0: 2e63 6c61 7373 795f 656c 656d 656e 742e  .classy_element.
-000069c0: 786d 6c5f 656c 656d 656e 7420 3d20 586d  xml_element = Xm
-000069d0: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
-000069e0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-000069f0: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-00006a00: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
-00006a10: 656e 745b 305d 2e6e 616d 6520 3d20 2774  ent[0].name = 't
-00006a20: 6573 745f 6e61 6d65 5f30 270d 0a20 2020  est_name_0'..   
-00006a30: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-00006a40: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
-00006a50: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
-00006a60: 6d65 6e74 5b31 5d2e 6e61 6d65 203d 2027  ment[1].name = '
-00006a70: 7465 7374 5f6e 616d 655f 3127 0d0a 2020  test_name_1'..  
-00006a80: 2020 6465 6c20 636c 6173 7379 5f78 6d6c    del classy_xml
-00006a90: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
-00006aa0: 6c61 7373 795f 656c 656d 656e 742e 786d  lassy_element.xm
-00006ab0: 6c5f 656c 656d 656e 745b 305d 2e6e 616d  l_element[0].nam
-00006ac0: 650d 0a20 2020 2061 7373 6572 7420 6e6f  e..    assert no
-00006ad0: 7420 6861 7361 7474 7228 0d0a 2020 2020  t hasattr(..    
-00006ae0: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-00006af0: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
-00006b00: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
-00006b10: 656c 656d 656e 745b 305d 2c20 276e 616d  element[0], 'nam
-00006b20: 6527 290d 0a20 2020 2061 7373 6572 7420  e')..    assert 
-00006b30: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00006b40: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
-00006b50: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
-00006b60: 656e 745b 315d 2e6e 616d 6520 3d3d 2027  ent[1].name == '
-00006b70: 7465 7374 5f6e 616d 655f 3127 0d0a 0d0a  test_name_1'....
-00006b80: 0d0a 6465 6620 7465 7374 5f73 6176 655f  ..def test_save_
-00006b90: 6173 2863 6c61 7373 795f 786d 6c5f 636f  as(classy_xml_co
-00006ba0: 756e 7472 6965 735f 6669 7874 7572 6529  untries_fixture)
-00006bb0: 3a0d 0a20 2020 2066 696c 6570 6174 6820  :..    filepath 
-00006bc0: 3d20 6f73 2e70 6174 682e 7370 6c69 7428  = os.path.split(
-00006bd0: 5f5f 6669 6c65 5f5f 295b 305d 0d0a 2020  __file__)[0]..  
-00006be0: 2020 7361 7665 5f61 735f 6669 6c65 6e61    save_as_filena
-00006bf0: 6d65 203d 206f 732e 7061 7468 2e6a 6f69  me = os.path.joi
-00006c00: 6e28 6669 6c65 7061 7468 2c20 2774 656d  n(filepath, 'tem
-00006c10: 705f 636f 756e 7472 6965 732e 786d 6c27  p_countries.xml'
-00006c20: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-00006c30: 6c5f 636f 756e 7472 6965 735f 6669 7874  l_countries_fixt
-00006c40: 7572 652e 7361 7665 5f61 7328 7361 7665  ure.save_as(save
-00006c50: 5f61 735f 6669 6c65 6e61 6d65 290d 0a20  _as_filename).. 
-00006c60: 2020 2077 6974 6820 6f70 656e 2863 6c61     with open(cla
-00006c70: 7373 795f 786d 6c5f 636f 756e 7472 6965  ssy_xml_countrie
-00006c80: 735f 6669 7874 7572 652e 786d 6c5f 6669  s_fixture.xml_fi
-00006c90: 6c65 2920 6173 2066 696c 653a 0d0a 2020  le) as file:..  
-00006ca0: 2020 2020 2020 636f 756e 7472 6965 735f        countries_
-00006cb0: 7465 7874 203d 2066 696c 652e 7265 6164  text = file.read
-00006cc0: 2829 0d0a 2020 2020 7769 7468 206f 7065  ()..    with ope
-00006cd0: 6e28 7361 7665 5f61 735f 6669 6c65 6e61  n(save_as_filena
-00006ce0: 6d65 2920 6173 2066 696c 653a 0d0a 2020  me) as file:..  
-00006cf0: 2020 2020 2020 7465 6d70 5f63 6f75 6e74        temp_count
-00006d00: 7269 6573 5f74 6578 7420 3d20 6669 6c65  ries_text = file
-00006d10: 2e72 6561 6428 290d 0a20 2020 206f 732e  .read()..    os.
-00006d20: 7265 6d6f 7665 2873 6176 655f 6173 5f66  remove(save_as_f
-00006d30: 696c 656e 616d 6529 0d0a 2020 2020 6173  ilename)..    as
-00006d40: 7365 7274 2063 6f75 6e74 7269 6573 5f74  sert countries_t
-00006d50: 6578 7420 3d3d 2074 656d 705f 636f 756e  ext == temp_coun
-00006d60: 7472 6965 735f 7465 7874 0d0a 0d0a 0d0a  tries_text......
-00006d70: 6465 6620 7465 7374 5f6d 6f64 6966 795f  def test_modify_
-00006d80: 616e 645f 7361 7665 5f78 6d6c 2863 6c61  and_save_xml(cla
-00006d90: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
-00006da0: 7874 7572 6529 3a0d 0a0d 0a20 2020 2063  xture):....    c
-00006db0: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00006dc0: 6669 7874 7572 652e 636f 756e 7472 7920  fixture.country 
-00006dd0: 3d20 586d 6c45 6c65 6d65 6e74 280d 0a20  = XmlElement(.. 
-00006de0: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
-00006df0: 733d 7b27 6e61 6d65 273a 2027 4c69 6563  s={'name': 'Liec
-00006e00: 6874 656e 7374 6569 6e27 7d29 0d0a 2020  htenstein'})..  
-00006e10: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
-00006e20: 7479 5f66 6978 7475 7265 2e63 6f75 6e74  ty_fixture.count
-00006e30: 7279 5b30 5d2e 7261 6e6b 203d 2058 6d6c  ry[0].rank = Xml
-00006e40: 456c 656d 656e 7428 7465 7874 3d31 290d  Element(text=1).
-00006e50: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-00006e60: 656d 7074 795f 6669 7874 7572 652e 636f  empty_fixture.co
-00006e70: 756e 7472 795b 305d 2e79 6561 7220 3d20  untry[0].year = 
-00006e80: 586d 6c45 6c65 6d65 6e74 2874 6578 743d  XmlElement(text=
-00006e90: 3230 3038 290d 0a20 2020 2063 6c61 7373  2008)..    class
-00006ea0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
-00006eb0: 7572 652e 636f 756e 7472 795b 305d 2e67  ure.country[0].g
-00006ec0: 6470 7063 203d 2058 6d6c 456c 656d 656e  dppc = XmlElemen
-00006ed0: 7428 7465 7874 3d31 3431 3130 3029 0d0a  t(text=141100)..
-00006ee0: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
-00006ef0: 6d70 7479 5f66 6978 7475 7265 2e63 6f75  mpty_fixture.cou
-00006f00: 6e74 7279 5b30 5d2e 6e65 6967 6862 6f72  ntry[0].neighbor
-00006f10: 203d 2058 6d6c 456c 656d 656e 7428 0d0a   = XmlElement(..
-00006f20: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-00006f30: 6573 3d7b 276e 616d 6527 3a20 2741 7573  es={'name': 'Aus
-00006f40: 7472 6961 272c 2027 6469 7265 6374 696f  tria', 'directio
-00006f50: 6e27 3a20 2745 277d 290d 0a20 2020 2063  n': 'E'})..    c
-00006f60: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
-00006f70: 6669 7874 7572 652e 636f 756e 7472 795b  fixture.country[
-00006f80: 305d 2e6e 6569 6768 626f 7220 3d20 586d  0].neighbor = Xm
-00006f90: 6c45 6c65 6d65 6e74 280d 0a20 2020 2020  lElement(..     
-00006fa0: 2020 2061 7474 7269 6275 7465 733d 7b27     attributes={'
-00006fb0: 6e61 6d65 273a 2027 5377 6974 7a65 726c  name': 'Switzerl
-00006fc0: 616e 6427 2c20 2764 6972 6563 7469 6f6e  and', 'direction
-00006fd0: 273a 2027 5727 7d29 0d0a 0d0a 2020 2020  ': 'W'})....    
-00006fe0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
-00006ff0: 5f66 6978 7475 7265 2e63 6f75 6e74 7279  _fixture.country
-00007000: 203d 2058 6d6c 456c 656d 656e 7428 290d   = XmlElement().
-00007010: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-00007020: 656d 7074 795f 6669 7874 7572 652e 636f  empty_fixture.co
-00007030: 756e 7472 795b 315d 2e6e 616d 6520 3d20  untry[1].name = 
-00007040: 2753 696e 6761 706f 7265 270d 0a20 2020  'Singapore'..   
-00007050: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
-00007060: 795f 6669 7874 7572 652e 636f 756e 7472  y_fixture.countr
-00007070: 795b 315d 2e72 616e 6b20 3d20 586d 6c45  y[1].rank = XmlE
-00007080: 6c65 6d65 6e74 2829 0d0a 2020 2020 636c  lement()..    cl
-00007090: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
-000070a0: 6978 7475 7265 2e63 6f75 6e74 7279 5b31  ixture.country[1
-000070b0: 5d2e 7261 6e6b 2e74 6578 7420 3d20 340d  ].rank.text = 4.
-000070c0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
-000070d0: 656d 7074 795f 6669 7874 7572 652e 636f  empty_fixture.co
-000070e0: 756e 7472 795b 315d 2e79 6561 7220 3d20  untry[1].year = 
-000070f0: 586d 6c45 6c65 6d65 6e74 2829 0d0a 2020  XmlElement()..  
-00007100: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
-00007110: 7479 5f66 6978 7475 7265 2e63 6f75 6e74  ty_fixture.count
-00007120: 7279 5b31 5d2e 7965 6172 2e74 6578 7420  ry[1].year.text 
-00007130: 3d20 3230 3131 0d0a 2020 2020 636c 6173  = 2011..    clas
-00007140: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
-00007150: 7475 7265 2e63 6f75 6e74 7279 5b31 5d2e  ture.country[1].
-00007160: 6764 7070 6320 3d20 586d 6c45 6c65 6d65  gdppc = XmlEleme
-00007170: 6e74 2829 0d0a 2020 2020 636c 6173 7379  nt()..    classy
-00007180: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00007190: 7265 2e63 6f75 6e74 7279 5b31 5d2e 6764  re.country[1].gd
-000071a0: 7070 632e 7465 7874 203d 2035 3939 3030  ppc.text = 59900
-000071b0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
-000071c0: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
-000071d0: 6f75 6e74 7279 5b31 5d2e 6e65 6967 6862  ountry[1].neighb
-000071e0: 6f72 203d 2058 6d6c 456c 656d 656e 7428  or = XmlElement(
-000071f0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
-00007200: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
-00007210: 636f 756e 7472 795b 315d 2e6e 6569 6768  country[1].neigh
-00007220: 626f 725b 305d 2e6e 616d 6520 3d20 274d  bor[0].name = 'M
-00007230: 616c 6179 7369 6127 0d0a 2020 2020 636c  alaysia'..    cl
-00007240: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
-00007250: 6978 7475 7265 2e63 6f75 6e74 7279 5b31  ixture.country[1
-00007260: 5d2e 6e65 6967 6862 6f72 5b30 5d2e 6469  ].neighbor[0].di
-00007270: 7265 6374 696f 6e20 3d20 274e 270d 0a0d  rection = 'N'...
-00007280: 0a20 2020 2066 696c 6570 6174 6820 3d20  .    filepath = 
-00007290: 6f73 2e70 6174 682e 7370 6c69 7428 5f5f  os.path.split(__
-000072a0: 6669 6c65 5f5f 295b 305d 0d0a 2020 2020  file__)[0]..    
-000072b0: 6765 6e5f 636f 756e 7472 6965 735f 6669  gen_countries_fi
-000072c0: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
-000072d0: 2e6a 6f69 6e28 6669 6c65 7061 7468 2c20  .join(filepath, 
-000072e0: 2763 6f75 6e74 7269 6573 5f67 656e 2e78  'countries_gen.x
-000072f0: 6d6c 2729 0d0a 2020 2020 636c 6173 7379  ml')..    classy
-00007300: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
-00007310: 7265 2e73 6176 655f 6173 2867 656e 5f63  re.save_as(gen_c
-00007320: 6f75 6e74 7269 6573 5f66 696c 656e 616d  ountries_filenam
-00007330: 6529 0d0a 0d0a 2020 2020 7769 7468 206f  e)....    with o
-00007340: 7065 6e28 6765 6e5f 636f 756e 7472 6965  pen(gen_countrie
-00007350: 735f 6669 6c65 6e61 6d65 2920 6173 2066  s_filename) as f
-00007360: 696c 653a 0d0a 2020 2020 2020 2020 636f  ile:..        co
-00007370: 756e 7472 6965 735f 6765 6e5f 7465 7874  untries_gen_text
-00007380: 203d 2066 696c 652e 7265 6164 2829 0d0a   = file.read()..
-00007390: 2020 2020 6f73 2e72 656d 6f76 6528 6765      os.remove(ge
-000073a0: 6e5f 636f 756e 7472 6965 735f 6669 6c65  n_countries_file
-000073b0: 6e61 6d65 290d 0a0d 0a20 2020 2066 696c  name)....    fil
-000073c0: 6570 6174 6820 3d20 6f73 2e70 6174 682e  epath = os.path.
-000073d0: 7370 6c69 7428 5f5f 6669 6c65 5f5f 295b  split(__file__)[
-000073e0: 305d 0d0a 2020 2020 636f 756e 7472 6965  0]..    countrie
-000073f0: 735f 6669 6c65 6e61 6d65 203d 206f 732e  s_filename = os.
-00007400: 7061 7468 2e6a 6f69 6e28 6669 6c65 7061  path.join(filepa
-00007410: 7468 2c20 2763 6f75 6e74 7269 6573 2e78  th, 'countries.x
-00007420: 6d6c 2729 0d0a 2020 2020 7769 7468 206f  ml')..    with o
-00007430: 7065 6e28 636f 756e 7472 6965 735f 6669  pen(countries_fi
-00007440: 6c65 6e61 6d65 2920 6173 2066 696c 653a  lename) as file:
-00007450: 0d0a 2020 2020 2020 2020 636f 756e 7472  ..        countr
-00007460: 6965 735f 7465 7874 203d 2066 696c 652e  ies_text = file.
-00007470: 7265 6164 2829 0d0a 0d0a 2020 2020 6173  read()....    as
-00007480: 7365 7274 2063 6f75 6e74 7269 6573 5f67  sert countries_g
-00007490: 656e 5f74 6578 7420 3d3d 2063 6f75 6e74  en_text == count
-000074a0: 7269 6573 5f74 6578 740d 0a              ries_text..
+00005270: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00005280: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00005290: 6c65 6d65 6e74 5b31 5d0d 0a20 2020 2020  lement[1]..     
+000052a0: 2020 202e 6d75 6c74 695f 656c 656d 656e     .multi_elemen
+000052b0: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+000052c0: 735f 6368 696c 645b 305d 0d0a 2020 2020  s_child[0]..    
+000052d0: 2020 2020 2e6e 616d 650d 0a20 2020 2020      .name..     
+000052e0: 2020 203d 3d20 2263 6869 6c64 5f31 5f61     == "child_1_a
+000052f0: 7474 725f 305f 6e61 6d65 220d 0a20 2020  ttr_0_name"..   
+00005300: 2029 0d0a 2020 2020 6173 7365 7274 2028   )..    assert (
+00005310: 0d0a 2020 2020 2020 2020 636c 6173 7379  ..        classy
+00005320: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00005330: 652e 6d75 6c74 695f 6e65 7374 6564 5f65  e.multi_nested_e
+00005340: 6c65 6d65 6e74 5b31 5d0d 0a20 2020 2020  lement[1]..     
+00005350: 2020 202e 6d75 6c74 695f 656c 656d 656e     .multi_elemen
+00005360: 745f 7769 7468 5f61 7474 7269 6275 7465  t_with_attribute
+00005370: 735f 6368 696c 645b 305d 0d0a 2020 2020  s_child[0]..    
+00005380: 2020 2020 2e76 616c 7565 0d0a 2020 2020      .value..    
+00005390: 2020 2020 3d3d 2022 6368 696c 645f 315f      == "child_1_
+000053a0: 6174 7472 5f30 5f76 616c 7565 220d 0a20  attr_0_value".. 
+000053b0: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+000053c0: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+000053d0: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+000053e0: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+000053f0: 5f65 6c65 6d65 6e74 5b31 5d0d 0a20 2020  _element[1]..   
+00005400: 2020 2020 202e 6d75 6c74 695f 656c 656d       .multi_elem
+00005410: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+00005420: 7465 735f 6368 696c 645b 315d 0d0a 2020  tes_child[1]..  
+00005430: 2020 2020 2020 2e6e 616d 650d 0a20 2020        .name..   
+00005440: 2020 2020 203d 3d20 2263 6869 6c64 5f31       == "child_1
+00005450: 5f61 7474 725f 315f 6e61 6d65 220d 0a20  _attr_1_name".. 
+00005460: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00005470: 2028 0d0a 2020 2020 2020 2020 636c 6173   (..        clas
+00005480: 7379 5f78 6d6c 5f74 6573 745f 6669 7874  sy_xml_test_fixt
+00005490: 7572 652e 6d75 6c74 695f 6e65 7374 6564  ure.multi_nested
+000054a0: 5f65 6c65 6d65 6e74 5b31 5d0d 0a20 2020  _element[1]..   
+000054b0: 2020 2020 202e 6d75 6c74 695f 656c 656d       .multi_elem
+000054c0: 656e 745f 7769 7468 5f61 7474 7269 6275  ent_with_attribu
+000054d0: 7465 735f 6368 696c 645b 315d 0d0a 2020  tes_child[1]..  
+000054e0: 2020 2020 2020 2e76 616c 7565 0d0a 2020        .value..  
+000054f0: 2020 2020 2020 3d3d 2022 6368 696c 645f        == "child_
+00005500: 315f 6174 7472 5f31 5f76 616c 7565 220d  1_attr_1_value".
+00005510: 0a20 2020 2029 0d0a 0d0a 0d0a 6465 6620  .    )......def 
+00005520: 7465 7374 5f6d 756c 7469 5f6e 6573 7465  test_multi_neste
+00005530: 645f 656c 656d 656e 745f 5f75 6e69 7175  d_element__uniqu
+00005540: 655f 656c 656d 656e 745f 6368 696c 645f  e_element_child_
+00005550: 6578 6973 7465 6e63 6528 636c 6173 7379  existence(classy
+00005560: 5f78 6d6c 5f74 6573 745f 6669 7874 7572  _xml_test_fixtur
+00005570: 6529 3a0d 0a20 2020 2061 7373 6572 7420  e):..    assert 
+00005580: 6861 7361 7474 7228 0d0a 2020 2020 2020  hasattr(..      
+00005590: 2020 636c 6173 7379 5f78 6d6c 5f74 6573    classy_xml_tes
+000055a0: 745f 6669 7874 7572 652e 6d75 6c74 695f  t_fixture.multi_
+000055b0: 6e65 7374 6564 5f65 6c65 6d65 6e74 5b30  nested_element[0
+000055c0: 5d2c 2022 756e 6971 7565 5f65 6c65 6d65  ], "unique_eleme
+000055d0: 6e74 5f63 6869 6c64 220d 0a20 2020 2029  nt_child"..    )
+000055e0: 0d0a 2020 2020 6173 7365 7274 206e 6f74  ..    assert not
+000055f0: 2068 6173 6174 7472 280d 0a20 2020 2020   hasattr(..     
+00005600: 2020 2063 6c61 7373 795f 786d 6c5f 7465     classy_xml_te
+00005610: 7374 5f66 6978 7475 7265 2e6d 756c 7469  st_fixture.multi
+00005620: 5f6e 6573 7465 645f 656c 656d 656e 745b  _nested_element[
+00005630: 315d 2c20 2275 6e69 7175 655f 656c 656d  1], "unique_elem
+00005640: 656e 745f 6368 696c 6422 0d0a 2020 2020  ent_child"..    
+00005650: 290d 0a0d 0a0d 0a64 6566 2074 6573 745f  )......def test_
+00005660: 636c 6173 7379 5f78 6d6c 5f61 6464 5f65  classy_xml_add_e
+00005670: 6c65 6d65 6e74 2863 6c61 7373 795f 786d  lement(classy_xm
+00005680: 6c5f 656d 7074 795f 6669 7874 7572 6529  l_empty_fixture)
+00005690: 3a0d 0a20 2020 2063 6c61 7373 795f 786d  :..    classy_xm
+000056a0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+000056b0: 7465 7374 5f65 6c65 6d65 6e74 203d 2058  test_element = X
+000056c0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+000056d0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+000056e0: 6365 2863 6c61 7373 795f 786d 6c5f 656d  ce(classy_xml_em
+000056f0: 7074 795f 6669 7874 7572 652e 7465 7374  pty_fixture.test
+00005700: 5f65 6c65 6d65 6e74 2c20 586d 6c45 6c65  _element, XmlEle
+00005710: 6d65 6e74 290d 0a0d 0a0d 0a64 6566 2074  ment)......def t
+00005720: 6573 745f 636c 6173 7379 5f78 6d6c 5f72  est_classy_xml_r
+00005730: 656d 6f76 655f 656c 656d 656e 7428 636c  emove_element(cl
+00005740: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
+00005750: 6978 7475 7265 293a 0d0a 2020 2020 636c  ixture):..    cl
+00005760: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
+00005770: 6978 7475 7265 2e74 6573 745f 656c 656d  ixture.test_elem
+00005780: 656e 7420 3d20 586d 6c45 6c65 6d65 6e74  ent = XmlElement
+00005790: 2829 0d0a 2020 2020 6465 6c20 636c 6173  ()..    del clas
+000057a0: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+000057b0: 7475 7265 2e74 6573 745f 656c 656d 656e  ture.test_elemen
+000057c0: 740d 0a20 2020 2061 7373 6572 7420 6e6f  t..    assert no
+000057d0: 7420 6861 7361 7474 7228 636c 6173 7379  t hasattr(classy
+000057e0: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
+000057f0: 7265 2c20 2274 6573 745f 656c 656d 656e  re, "test_elemen
+00005800: 7422 290d 0a0d 0a0d 0a64 6566 2074 6573  t")......def tes
+00005810: 745f 636c 6173 7379 5f78 6d6c 5f61 6464  t_classy_xml_add
+00005820: 5f65 6c65 6d65 6e74 5f61 7272 6179 2863  _element_array(c
+00005830: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00005840: 6669 7874 7572 6529 3a0d 0a20 2020 2063  fixture):..    c
+00005850: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00005860: 6669 7874 7572 652e 7465 7374 5f65 6c65  fixture.test_ele
+00005870: 6d65 6e74 5f61 7272 6179 203d 2058 6d6c  ment_array = Xml
+00005880: 456c 656d 656e 7428 290d 0a20 2020 2063  Element()..    c
+00005890: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+000058a0: 6669 7874 7572 652e 7465 7374 5f65 6c65  fixture.test_ele
+000058b0: 6d65 6e74 5f61 7272 6179 203d 2058 6d6c  ment_array = Xml
+000058c0: 456c 656d 656e 7428 290d 0a20 2020 2061  Element()..    a
+000058d0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+000058e0: 2863 6c61 7373 795f 786d 6c5f 656d 7074  (classy_xml_empt
+000058f0: 795f 6669 7874 7572 652e 7465 7374 5f65  y_fixture.test_e
+00005900: 6c65 6d65 6e74 5f61 7272 6179 5b30 5d2c  lement_array[0],
+00005910: 2058 6d6c 456c 656d 656e 7429 0d0a 2020   XmlElement)..  
+00005920: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00005930: 6e63 6528 636c 6173 7379 5f78 6d6c 5f65  nce(classy_xml_e
+00005940: 6d70 7479 5f66 6978 7475 7265 2e74 6573  mpty_fixture.tes
+00005950: 745f 656c 656d 656e 745f 6172 7261 795b  t_element_array[
+00005960: 315d 2c20 586d 6c45 6c65 6d65 6e74 290d  1], XmlElement).
+00005970: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00005980: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00005990: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
+000059a0: 656d 656e 745f 6172 7261 7929 203d 3d20  ement_array) == 
+000059b0: 320d 0a0d 0a0d 0a64 6566 2074 6573 745f  2......def test_
+000059c0: 636c 6173 7379 5f78 6d6c 5f72 656d 6f76  classy_xml_remov
+000059d0: 655f 656c 656d 656e 745f 6172 7261 7928  e_element_array(
+000059e0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+000059f0: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
+00005a00: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00005a10: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
+00005a20: 656d 656e 745f 6172 7261 7920 3d20 586d  ement_array = Xm
+00005a30: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
+00005a40: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00005a50: 5f66 6978 7475 7265 2e74 6573 745f 656c  _fixture.test_el
+00005a60: 656d 656e 745f 6172 7261 7920 3d20 586d  ement_array = Xm
+00005a70: 6c45 6c65 6d65 6e74 2829 0d0a 2020 2020  lElement()..    
+00005a80: 6465 6c20 636c 6173 7379 5f78 6d6c 5f65  del classy_xml_e
+00005a90: 6d70 7479 5f66 6978 7475 7265 2e74 6573  mpty_fixture.tes
+00005aa0: 745f 656c 656d 656e 745f 6172 7261 795b  t_element_array[
+00005ab0: 305d 0d0a 2020 2020 6173 7365 7274 2069  0]..    assert i
+00005ac0: 7369 6e73 7461 6e63 6528 636c 6173 7379  sinstance(classy
+00005ad0: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
+00005ae0: 7265 2e74 6573 745f 656c 656d 656e 745f  re.test_element_
+00005af0: 6172 7261 792c 2058 6d6c 456c 656d 656e  array, XmlElemen
+00005b00: 7429 0d0a 2020 2020 6173 7365 7274 206c  t)..    assert l
+00005b10: 656e 2863 6c61 7373 795f 786d 6c5f 656d  en(classy_xml_em
+00005b20: 7074 795f 6669 7874 7572 652e 7465 7374  pty_fixture.test
+00005b30: 5f65 6c65 6d65 6e74 5f61 7272 6179 2920  _element_array) 
+00005b40: 3d3d 2031 0d0a 0d0a 0d0a 6465 6620 7465  == 1......def te
+00005b50: 7374 5f78 6d6c 5f65 6c65 6d65 6e74 5f61  st_xml_element_a
+00005b60: 6464 5f65 6c65 6d65 6e74 2863 6c61 7373  dd_element(class
+00005b70: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00005b80: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
+00005b90: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00005ba0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00005bb0: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
+00005bc0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
+00005bd0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00005be0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00005bf0: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
+00005c00: 456c 656d 656e 7428 290d 0a20 2020 2061  Element()..    a
+00005c10: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00005c20: 2863 6c61 7373 795f 786d 6c5f 656d 7074  (classy_xml_empt
+00005c30: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00005c40: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00005c50: 6d65 6e74 2c20 586d 6c45 6c65 6d65 6e74  ment, XmlElement
+00005c60: 290d 0a0d 0a0d 0a64 6566 2074 6573 745f  )......def test_
+00005c70: 786d 6c5f 656c 656d 656e 745f 7265 6d6f  xml_element_remo
+00005c80: 7665 5f65 6c65 6d65 6e74 2863 6c61 7373  ve_element(class
+00005c90: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00005ca0: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
+00005cb0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00005cc0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00005cd0: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
+00005ce0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
+00005cf0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00005d00: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00005d10: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
+00005d20: 456c 656d 656e 7428 290d 0a20 2020 2064  Element()..    d
+00005d30: 656c 2063 6c61 7373 795f 786d 6c5f 656d  el classy_xml_em
+00005d40: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+00005d50: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+00005d60: 6c65 6d65 6e74 0d0a 2020 2020 6173 7365  lement..    asse
+00005d70: 7274 206e 6f74 2068 6173 6174 7472 2863  rt not hasattr(c
+00005d80: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00005d90: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00005da0: 6c65 6d65 6e74 2c20 2278 6d6c 5f65 6c65  lement, "xml_ele
+00005db0: 6d65 6e74 2229 0d0a 0d0a 0d0a 6465 6620  ment")......def 
+00005dc0: 7465 7374 5f78 6d6c 5f65 6c65 6d65 6e74  test_xml_element
+00005dd0: 5f61 6464 5f65 6c65 6d65 6e74 5f61 7272  _add_element_arr
+00005de0: 6179 2863 6c61 7373 795f 786d 6c5f 656d  ay(classy_xml_em
+00005df0: 7074 795f 6669 7874 7572 6529 3a0d 0a20  pty_fixture):.. 
+00005e00: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
+00005e10: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+00005e20: 7379 5f65 6c65 6d65 6e74 203d 2058 6d6c  sy_element = Xml
+00005e30: 456c 656d 656e 7428 290d 0a20 2020 2063  Element()..    c
+00005e40: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00005e50: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00005e60: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+00005e70: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
+00005e80: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
+00005e90: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00005ea0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00005eb0: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
+00005ec0: 456c 656d 656e 7428 290d 0a20 2020 2061  Element()..    a
+00005ed0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00005ee0: 280d 0a20 2020 2020 2020 2063 6c61 7373  (..        class
+00005ef0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00005f00: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00005f10: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 5b30  nt.xml_element[0
+00005f20: 5d2c 2058 6d6c 456c 656d 656e 740d 0a20  ], XmlElement.. 
+00005f30: 2020 2029 0d0a 2020 2020 6173 7365 7274     )..    assert
+00005f40: 2069 7369 6e73 7461 6e63 6528 0d0a 2020   isinstance(..  
+00005f50: 2020 2020 2020 636c 6173 7379 5f78 6d6c        classy_xml
+00005f60: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
+00005f70: 6c61 7373 795f 656c 656d 656e 742e 786d  lassy_element.xm
+00005f80: 6c5f 656c 656d 656e 745b 315d 2c20 586d  l_element[1], Xm
+00005f90: 6c45 6c65 6d65 6e74 0d0a 2020 2020 290d  lElement..    ).
+00005fa0: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00005fb0: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00005fc0: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
+00005fd0: 656c 656d 656e 742e 786d 6c5f 656c 656d  element.xml_elem
+00005fe0: 656e 7429 203d 3d20 320d 0a0d 0a0d 0a64  ent) == 2......d
+00005ff0: 6566 2074 6573 745f 786d 6c5f 656c 656d  ef test_xml_elem
+00006000: 656e 745f 7265 6d6f 7665 5f65 6c65 6d65  ent_remove_eleme
+00006010: 6e74 5f61 7272 6179 2863 6c61 7373 795f  nt_array(classy_
+00006020: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00006030: 6529 3a0d 0a20 2020 2063 6c61 7373 795f  e):..    classy_
+00006040: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00006050: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00006060: 203d 2058 6d6c 456c 656d 656e 7428 290d   = XmlElement().
+00006070: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00006080: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006090: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+000060a0: 5f65 6c65 6d65 6e74 203d 2058 6d6c 456c  _element = XmlEl
+000060b0: 656d 656e 7428 290d 0a20 2020 2063 6c61  ement()..    cla
+000060c0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+000060d0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+000060e0: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
+000060f0: 203d 2058 6d6c 456c 656d 656e 7428 290d   = XmlElement().
+00006100: 0a20 2020 2064 656c 2063 6c61 7373 795f  .    del classy_
+00006110: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00006120: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00006130: 2e78 6d6c 5f65 6c65 6d65 6e74 5b30 5d0d  .xml_element[0].
+00006140: 0a20 2020 2061 7373 6572 7420 6973 696e  .    assert isin
+00006150: 7374 616e 6365 2863 6c61 7373 795f 786d  stance(classy_xm
+00006160: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00006170: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00006180: 6d6c 5f65 6c65 6d65 6e74 2c20 586d 6c45  ml_element, XmlE
+00006190: 6c65 6d65 6e74 290d 0a20 2020 2061 7373  lement)..    ass
+000061a0: 6572 7420 6c65 6e28 636c 6173 7379 5f78  ert len(classy_x
+000061b0: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
+000061c0: 2e63 6c61 7373 795f 656c 656d 656e 742e  .classy_element.
+000061d0: 786d 6c5f 656c 656d 656e 7429 203d 3d20  xml_element) == 
+000061e0: 310d 0a0d 0a0d 0a64 6566 2074 6573 745f  1......def test_
+000061f0: 786d 6c5f 656c 656d 656e 745f 6164 645f  xml_element_add_
+00006200: 7465 7874 2863 6c61 7373 795f 786d 6c5f  text(classy_xml_
+00006210: 656d 7074 795f 6669 7874 7572 6529 3a0d  empty_fixture):.
+00006220: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00006230: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006240: 6173 7379 5f65 6c65 6d65 6e74 203d 2058  assy_element = X
+00006250: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00006260: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00006270: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00006280: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00006290: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+000062a0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+000062b0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+000062c0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+000062d0: 2e78 6d6c 5f65 6c65 6d65 6e74 2e74 6578  .xml_element.tex
+000062e0: 7420 3d20 2274 6573 7422 0d0a 2020 2020  t = "test"..    
+000062f0: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
+00006300: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00006310: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00006320: 6d6c 5f65 6c65 6d65 6e74 2e74 6578 7420  ml_element.text 
+00006330: 3d3d 2022 7465 7374 220d 0a0d 0a0d 0a64  == "test"......d
+00006340: 6566 2074 6573 745f 786d 6c5f 656c 656d  ef test_xml_elem
+00006350: 656e 745f 6368 616e 6765 5f74 6578 7428  ent_change_text(
+00006360: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00006370: 5f66 6978 7475 7265 293a 0d0a 2020 2020  _fixture):..    
+00006380: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00006390: 5f66 6978 7475 7265 2e63 6c61 7373 795f  _fixture.classy_
+000063a0: 656c 656d 656e 7420 3d20 586d 6c45 6c65  element = XmlEle
+000063b0: 6d65 6e74 2829 0d0a 2020 2020 636c 6173  ment()..    clas
+000063c0: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+000063d0: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
+000063e0: 656e 742e 786d 6c5f 656c 656d 656e 7420  ent.xml_element 
+000063f0: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
+00006400: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
+00006410: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
+00006420: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
+00006430: 656c 656d 656e 742e 7465 7874 203d 2022  element.text = "
+00006440: 7465 7374 220d 0a20 2020 2063 6c61 7373  test"..    class
+00006450: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00006460: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00006470: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 2e74  nt.xml_element.t
+00006480: 6578 7420 3d20 2263 6861 6e67 6564 220d  ext = "changed".
+00006490: 0a20 2020 2061 7373 6572 7420 636c 6173  .    assert clas
+000064a0: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+000064b0: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
+000064c0: 656e 742e 786d 6c5f 656c 656d 656e 742e  ent.xml_element.
+000064d0: 7465 7874 203d 3d20 2263 6861 6e67 6564  text == "changed
+000064e0: 220d 0a0d 0a0d 0a64 6566 2074 6573 745f  "......def test_
+000064f0: 786d 6c5f 656c 656d 656e 745f 7265 6d6f  xml_element_remo
+00006500: 7665 5f74 6578 7428 636c 6173 7379 5f78  ve_text(classy_x
+00006510: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
+00006520: 293a 0d0a 2020 2020 636c 6173 7379 5f78  ):..    classy_x
+00006530: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
+00006540: 2e63 6c61 7373 795f 656c 656d 656e 7420  .classy_element 
+00006550: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
+00006560: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
+00006570: 6d70 7479 5f66 6978 7475 7265 2e63 6c61  mpty_fixture.cla
+00006580: 7373 795f 656c 656d 656e 742e 786d 6c5f  ssy_element.xml_
+00006590: 656c 656d 656e 7420 3d20 586d 6c45 6c65  element = XmlEle
+000065a0: 6d65 6e74 2829 0d0a 2020 2020 636c 6173  ment()..    clas
+000065b0: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+000065c0: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
+000065d0: 656e 742e 786d 6c5f 656c 656d 656e 742e  ent.xml_element.
+000065e0: 7465 7874 203d 2022 7465 7374 220d 0a20  text = "test".. 
+000065f0: 2020 2064 656c 2063 6c61 7373 795f 786d     del classy_xm
+00006600: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00006610: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00006620: 6d6c 5f65 6c65 6d65 6e74 2e74 6578 740d  ml_element.text.
+00006630: 0a20 2020 2061 7373 6572 7420 636c 6173  .    assert clas
+00006640: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+00006650: 7475 7265 2e63 6c61 7373 795f 656c 656d  ture.classy_elem
+00006660: 656e 742e 786d 6c5f 656c 656d 656e 742e  ent.xml_element.
+00006670: 7465 7874 2069 7320 4e6f 6e65 0d0a 0d0a  text is None....
+00006680: 0d0a 6465 6620 7465 7374 5f78 6d6c 5f65  ..def test_xml_e
+00006690: 6c65 6d65 6e74 5f61 7272 6179 5f61 6464  lement_array_add
+000066a0: 5f74 6578 7428 636c 6173 7379 5f78 6d6c  _text(classy_xml
+000066b0: 5f65 6d70 7479 5f66 6978 7475 7265 293a  _empty_fixture):
+000066c0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+000066d0: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
+000066e0: 6c61 7373 795f 656c 656d 656e 7420 3d20  lassy_element = 
+000066f0: 586d 6c45 6c65 6d65 6e74 2829 0d0a 2020  XmlElement()..  
+00006700: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
+00006710: 7479 5f66 6978 7475 7265 2e63 6c61 7373  ty_fixture.class
+00006720: 795f 656c 656d 656e 742e 786d 6c5f 656c  y_element.xml_el
+00006730: 656d 656e 7420 3d20 586d 6c45 6c65 6d65  ement = XmlEleme
+00006740: 6e74 2829 0d0a 2020 2020 636c 6173 7379  nt()..    classy
+00006750: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
+00006760: 7265 2e63 6c61 7373 795f 656c 656d 656e  re.classy_elemen
+00006770: 742e 786d 6c5f 656c 656d 656e 7420 3d20  t.xml_element = 
+00006780: 586d 6c45 6c65 6d65 6e74 2829 0d0a 2020  XmlElement()..  
+00006790: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
+000067a0: 7479 5f66 6978 7475 7265 2e63 6c61 7373  ty_fixture.class
+000067b0: 795f 656c 656d 656e 742e 786d 6c5f 656c  y_element.xml_el
+000067c0: 656d 656e 745b 305d 2e74 6578 7420 3d20  ement[0].text = 
+000067d0: 2274 6573 7422 0d0a 2020 2020 6173 7365  "test"..    asse
+000067e0: 7274 2063 6c61 7373 795f 786d 6c5f 656d  rt classy_xml_em
+000067f0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+00006800: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+00006810: 6c65 6d65 6e74 5b30 5d2e 7465 7874 203d  lement[0].text =
+00006820: 3d20 2274 6573 7422 0d0a 2020 2020 6173  = "test"..    as
+00006830: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
+00006840: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006850: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00006860: 5f65 6c65 6d65 6e74 5b31 5d2e 7465 7874  _element[1].text
+00006870: 2069 7320 4e6f 6e65 0d0a 0d0a 0d0a 6465   is None......de
+00006880: 6620 7465 7374 5f78 6d6c 5f65 6c65 6d65  f test_xml_eleme
+00006890: 6e74 5f61 7272 6179 5f72 656d 6f76 655f  nt_array_remove_
+000068a0: 7465 7874 2863 6c61 7373 795f 786d 6c5f  text(classy_xml_
+000068b0: 656d 7074 795f 6669 7874 7572 6529 3a0d  empty_fixture):.
+000068c0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+000068d0: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+000068e0: 6173 7379 5f65 6c65 6d65 6e74 203d 2058  assy_element = X
+000068f0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00006900: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00006910: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00006920: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00006930: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+00006940: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+00006950: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00006960: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00006970: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
+00006980: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00006990: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+000069a0: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+000069b0: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+000069c0: 6d65 6e74 5b30 5d2e 7465 7874 203d 2022  ment[0].text = "
+000069d0: 7465 7374 5f30 220d 0a20 2020 2063 6c61  test_0"..    cla
+000069e0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+000069f0: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+00006a00: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
+00006a10: 5b31 5d2e 7465 7874 203d 2022 7465 7374  [1].text = "test
+00006a20: 5f31 220d 0a20 2020 2064 656c 2063 6c61  _1"..    del cla
+00006a30: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00006a40: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+00006a50: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
+00006a60: 5b30 5d2e 7465 7874 0d0a 2020 2020 6173  [0].text..    as
+00006a70: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
+00006a80: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006a90: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00006aa0: 5f65 6c65 6d65 6e74 5b30 5d2e 7465 7874  _element[0].text
+00006ab0: 2069 7320 4e6f 6e65 0d0a 2020 2020 6173   is None..    as
+00006ac0: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
+00006ad0: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006ae0: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00006af0: 5f65 6c65 6d65 6e74 5b31 5d2e 7465 7874  _element[1].text
+00006b00: 203d 3d20 2274 6573 745f 3122 0d0a 0d0a   == "test_1"....
+00006b10: 0d0a 6465 6620 7465 7374 5f78 6d6c 5f65  ..def test_xml_e
+00006b20: 6c65 6d65 6e74 5f61 6464 5f61 7474 7269  lement_add_attri
+00006b30: 6275 7465 2863 6c61 7373 795f 786d 6c5f  bute(classy_xml_
+00006b40: 656d 7074 795f 6669 7874 7572 6529 3a0d  empty_fixture):.
+00006b50: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00006b60: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006b70: 6173 7379 5f65 6c65 6d65 6e74 203d 2058  assy_element = X
+00006b80: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00006b90: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00006ba0: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00006bb0: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00006bc0: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+00006bd0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+00006be0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00006bf0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00006c00: 2e78 6d6c 5f65 6c65 6d65 6e74 2e6e 616d  .xml_element.nam
+00006c10: 6520 3d20 2274 6573 745f 6e61 6d65 220d  e = "test_name".
+00006c20: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00006c30: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006c40: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00006c50: 5f65 6c65 6d65 6e74 2e76 616c 7565 203d  _element.value =
+00006c60: 2031 0d0a 2020 2020 6173 7365 7274 2063   1..    assert c
+00006c70: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00006c80: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00006c90: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+00006ca0: 6e74 2e6e 616d 6520 3d3d 2022 7465 7374  nt.name == "test
+00006cb0: 5f6e 616d 6522 0d0a 2020 2020 6173 7365  _name"..    asse
+00006cc0: 7274 2063 6c61 7373 795f 786d 6c5f 656d  rt classy_xml_em
+00006cd0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+00006ce0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+00006cf0: 6c65 6d65 6e74 2e76 616c 7565 203d 3d20  lement.value == 
+00006d00: 2231 220d 0a0d 0a0d 0a64 6566 2074 6573  "1"......def tes
+00006d10: 745f 786d 6c5f 656c 656d 656e 745f 6368  t_xml_element_ch
+00006d20: 616e 6765 5f61 7474 7269 6275 7465 2863  ange_attribute(c
+00006d30: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00006d40: 6669 7874 7572 6529 3a0d 0a20 2020 2063  fixture):..    c
+00006d50: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00006d60: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00006d70: 6c65 6d65 6e74 203d 2058 6d6c 456c 656d  lement = XmlElem
+00006d80: 656e 7428 290d 0a20 2020 2063 6c61 7373  ent()..    class
+00006d90: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00006da0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00006db0: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 203d  nt.xml_element =
+00006dc0: 2058 6d6c 456c 656d 656e 7428 290d 0a20   XmlElement().. 
+00006dd0: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
+00006de0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+00006df0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+00006e00: 6c65 6d65 6e74 2e6e 616d 6520 3d20 2274  lement.name = "t
+00006e10: 6573 745f 6e61 6d65 220d 0a20 2020 2063  est_name"..    c
+00006e20: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00006e30: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00006e40: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+00006e50: 6e74 2e6e 616d 6520 3d20 2263 6861 6e67  nt.name = "chang
+00006e60: 6564 5f6e 616d 6522 0d0a 2020 2020 6173  ed_name"..    as
+00006e70: 7365 7274 2063 6c61 7373 795f 786d 6c5f  sert classy_xml_
+00006e80: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00006e90: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00006ea0: 5f65 6c65 6d65 6e74 2e6e 616d 6520 3d3d  _element.name ==
+00006eb0: 2022 6368 616e 6765 645f 6e61 6d65 220d   "changed_name".
+00006ec0: 0a0d 0a0d 0a64 6566 2074 6573 745f 786d  .....def test_xm
+00006ed0: 6c5f 656c 656d 656e 745f 7265 6d6f 7665  l_element_remove
+00006ee0: 5f61 7474 7269 6275 7465 2863 6c61 7373  _attribute(class
+00006ef0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00006f00: 7572 6529 3a0d 0a20 2020 2063 6c61 7373  ure):..    class
+00006f10: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00006f20: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00006f30: 6e74 203d 2058 6d6c 456c 656d 656e 7428  nt = XmlElement(
+00006f40: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
+00006f50: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00006f60: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+00006f70: 6d6c 5f65 6c65 6d65 6e74 203d 2058 6d6c  ml_element = Xml
+00006f80: 456c 656d 656e 7428 290d 0a20 2020 2063  Element()..    c
+00006f90: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00006fa0: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00006fb0: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+00006fc0: 6e74 2e76 616c 7565 203d 2022 7465 7374  nt.value = "test
+00006fd0: 220d 0a20 2020 2064 656c 2063 6c61 7373  "..    del class
+00006fe0: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00006ff0: 7572 652e 636c 6173 7379 5f65 6c65 6d65  ure.classy_eleme
+00007000: 6e74 2e78 6d6c 5f65 6c65 6d65 6e74 2e76  nt.xml_element.v
+00007010: 616c 7565 0d0a 2020 2020 6173 7365 7274  alue..    assert
+00007020: 206e 6f74 2068 6173 6174 7472 2863 6c61   not hasattr(cla
+00007030: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007040: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+00007050: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
+00007060: 2c20 2276 616c 7565 2229 0d0a 0d0a 0d0a  , "value")......
+00007070: 6465 6620 7465 7374 5f78 6d6c 5f65 6c65  def test_xml_ele
+00007080: 6d65 6e74 5f61 7272 6179 5f61 6464 5f61  ment_array_add_a
+00007090: 7474 7269 6275 7465 2863 6c61 7373 795f  ttribute(classy_
+000070a0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+000070b0: 6529 3a0d 0a20 2020 2063 6c61 7373 795f  e):..    classy_
+000070c0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+000070d0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+000070e0: 203d 2058 6d6c 456c 656d 656e 7428 290d   = XmlElement().
+000070f0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00007100: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00007110: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+00007120: 5f65 6c65 6d65 6e74 203d 2058 6d6c 456c  _element = XmlEl
+00007130: 656d 656e 7428 290d 0a20 2020 2063 6c61  ement()..    cla
+00007140: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007150: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+00007160: 6d65 6e74 2e78 6d6c 5f65 6c65 6d65 6e74  ment.xml_element
+00007170: 203d 2058 6d6c 456c 656d 656e 7428 290d   = XmlElement().
+00007180: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00007190: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+000071a0: 6173 7379 5f65 6c65 6d65 6e74 2e78 6d6c  assy_element.xml
+000071b0: 5f65 6c65 6d65 6e74 5b30 5d2e 6e61 6d65  _element[0].name
+000071c0: 203d 2022 7465 7374 5f6e 616d 655f 3022   = "test_name_0"
+000071d0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+000071e0: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
+000071f0: 6c61 7373 795f 656c 656d 656e 742e 786d  lassy_element.xm
+00007200: 6c5f 656c 656d 656e 745b 315d 2e6e 616d  l_element[1].nam
+00007210: 6520 3d20 2274 6573 745f 6e61 6d65 5f31  e = "test_name_1
+00007220: 220d 0a20 2020 2061 7373 6572 7420 636c  "..    assert cl
+00007230: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
+00007240: 6978 7475 7265 2e63 6c61 7373 795f 656c  ixture.classy_el
+00007250: 656d 656e 742e 786d 6c5f 656c 656d 656e  ement.xml_elemen
+00007260: 745b 305d 2e6e 616d 6520 3d3d 2022 7465  t[0].name == "te
+00007270: 7374 5f6e 616d 655f 3022 0d0a 2020 2020  st_name_0"..    
+00007280: 6173 7365 7274 2063 6c61 7373 795f 786d  assert classy_xm
+00007290: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+000072a0: 636c 6173 7379 5f65 6c65 6d65 6e74 2e78  classy_element.x
+000072b0: 6d6c 5f65 6c65 6d65 6e74 5b31 5d2e 6e61  ml_element[1].na
+000072c0: 6d65 203d 3d20 2274 6573 745f 6e61 6d65  me == "test_name
+000072d0: 5f31 220d 0a0d 0a0d 0a64 6566 2074 6573  _1"......def tes
+000072e0: 745f 786d 6c5f 656c 656d 656e 745f 6172  t_xml_element_ar
+000072f0: 7261 795f 6368 616e 6765 5f61 7474 7269  ray_change_attri
+00007300: 6275 7465 2863 6c61 7373 795f 786d 6c5f  bute(classy_xml_
+00007310: 656d 7074 795f 6669 7874 7572 6529 3a0d  empty_fixture):.
+00007320: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00007330: 656d 7074 795f 6669 7874 7572 652e 636c  empty_fixture.cl
+00007340: 6173 7379 5f65 6c65 6d65 6e74 203d 2058  assy_element = X
+00007350: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00007360: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00007370: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00007380: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00007390: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+000073a0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+000073b0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+000073c0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+000073d0: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
+000073e0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+000073f0: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00007400: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+00007410: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+00007420: 6d65 6e74 5b30 5d2e 6e61 6d65 203d 2022  ment[0].name = "
+00007430: 7465 7374 5f6e 616d 655f 3022 0d0a 2020  test_name_0"..  
+00007440: 2020 636c 6173 7379 5f78 6d6c 5f65 6d70    classy_xml_emp
+00007450: 7479 5f66 6978 7475 7265 2e63 6c61 7373  ty_fixture.class
+00007460: 795f 656c 656d 656e 742e 786d 6c5f 656c  y_element.xml_el
+00007470: 656d 656e 745b 315d 2e6e 616d 6520 3d20  ement[1].name = 
+00007480: 2274 6573 745f 6e61 6d65 5f31 220d 0a20  "test_name_1".. 
+00007490: 2020 2063 6c61 7373 795f 786d 6c5f 656d     classy_xml_em
+000074a0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+000074b0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+000074c0: 6c65 6d65 6e74 5b30 5d2e 6e61 6d65 203d  lement[0].name =
+000074d0: 2022 7465 7374 5f6e 616d 655f 305f 6368   "test_name_0_ch
+000074e0: 616e 6765 6422 0d0a 2020 2020 6173 7365  anged"..    asse
+000074f0: 7274 2028 0d0a 2020 2020 2020 2020 636c  rt (..        cl
+00007500: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
+00007510: 6978 7475 7265 2e63 6c61 7373 795f 656c  ixture.classy_el
+00007520: 656d 656e 742e 786d 6c5f 656c 656d 656e  ement.xml_elemen
+00007530: 745b 305d 2e6e 616d 650d 0a20 2020 2020  t[0].name..     
+00007540: 2020 203d 3d20 2274 6573 745f 6e61 6d65     == "test_name
+00007550: 5f30 5f63 6861 6e67 6564 220d 0a20 2020  _0_changed"..   
+00007560: 2029 0d0a 2020 2020 6173 7365 7274 2063   )..    assert c
+00007570: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00007580: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00007590: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+000075a0: 6e74 5b31 5d2e 6e61 6d65 203d 3d20 2274  nt[1].name == "t
+000075b0: 6573 745f 6e61 6d65 5f31 220d 0a0d 0a0d  est_name_1".....
+000075c0: 0a64 6566 2074 6573 745f 786d 6c5f 656c  .def test_xml_el
+000075d0: 656d 656e 745f 6172 7261 795f 7265 6d6f  ement_array_remo
+000075e0: 7665 5f61 7474 7269 6275 7465 2863 6c61  ve_attribute(cla
+000075f0: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007600: 7874 7572 6529 3a0d 0a20 2020 2063 6c61  xture):..    cla
+00007610: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007620: 7874 7572 652e 636c 6173 7379 5f65 6c65  xture.classy_ele
+00007630: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+00007640: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+00007650: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00007660: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00007670: 2e78 6d6c 5f65 6c65 6d65 6e74 203d 2058  .xml_element = X
+00007680: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00007690: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+000076a0: 795f 6669 7874 7572 652e 636c 6173 7379  y_fixture.classy
+000076b0: 5f65 6c65 6d65 6e74 2e78 6d6c 5f65 6c65  _element.xml_ele
+000076c0: 6d65 6e74 203d 2058 6d6c 456c 656d 656e  ment = XmlElemen
+000076d0: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+000076e0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+000076f0: 652e 636c 6173 7379 5f65 6c65 6d65 6e74  e.classy_element
+00007700: 2e78 6d6c 5f65 6c65 6d65 6e74 5b30 5d2e  .xml_element[0].
+00007710: 6e61 6d65 203d 2022 7465 7374 5f6e 616d  name = "test_nam
+00007720: 655f 3022 0d0a 2020 2020 636c 6173 7379  e_0"..    classy
+00007730: 5f78 6d6c 5f65 6d70 7479 5f66 6978 7475  _xml_empty_fixtu
+00007740: 7265 2e63 6c61 7373 795f 656c 656d 656e  re.classy_elemen
+00007750: 742e 786d 6c5f 656c 656d 656e 745b 315d  t.xml_element[1]
+00007760: 2e6e 616d 6520 3d20 2274 6573 745f 6e61  .name = "test_na
+00007770: 6d65 5f31 220d 0a20 2020 2064 656c 2063  me_1"..    del c
+00007780: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00007790: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+000077a0: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+000077b0: 6e74 5b30 5d2e 6e61 6d65 0d0a 2020 2020  nt[0].name..    
+000077c0: 6173 7365 7274 206e 6f74 2068 6173 6174  assert not hasat
+000077d0: 7472 2863 6c61 7373 795f 786d 6c5f 656d  tr(classy_xml_em
+000077e0: 7074 795f 6669 7874 7572 652e 636c 6173  pty_fixture.clas
+000077f0: 7379 5f65 6c65 6d65 6e74 2e78 6d6c 5f65  sy_element.xml_e
+00007800: 6c65 6d65 6e74 5b30 5d2c 2022 6e61 6d65  lement[0], "name
+00007810: 2229 0d0a 2020 2020 6173 7365 7274 2063  ")..    assert c
+00007820: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00007830: 6669 7874 7572 652e 636c 6173 7379 5f65  fixture.classy_e
+00007840: 6c65 6d65 6e74 2e78 6d6c 5f65 6c65 6d65  lement.xml_eleme
+00007850: 6e74 5b31 5d2e 6e61 6d65 203d 3d20 2274  nt[1].name == "t
+00007860: 6573 745f 6e61 6d65 5f31 220d 0a0d 0a0d  est_name_1".....
+00007870: 0a64 6566 2074 6573 745f 7361 7665 5f61  .def test_save_a
+00007880: 7328 636c 6173 7379 5f78 6d6c 5f63 6f75  s(classy_xml_cou
+00007890: 6e74 7269 6573 5f66 6978 7475 7265 293a  ntries_fixture):
+000078a0: 0d0a 2020 2020 6669 6c65 7061 7468 203d  ..    filepath =
+000078b0: 206f 732e 7061 7468 2e73 706c 6974 285f   os.path.split(_
+000078c0: 5f66 696c 655f 5f29 5b30 5d0d 0a20 2020  _file__)[0]..   
+000078d0: 2073 6176 655f 6173 5f66 696c 656e 616d   save_as_filenam
+000078e0: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
+000078f0: 2866 696c 6570 6174 682c 2022 7465 6d70  (filepath, "temp
+00007900: 5f63 6f75 6e74 7269 6573 2e78 6d6c 2229  _countries.xml")
+00007910: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+00007920: 5f63 6f75 6e74 7269 6573 5f66 6978 7475  _countries_fixtu
+00007930: 7265 2e73 6176 655f 6173 2873 6176 655f  re.save_as(save_
+00007940: 6173 5f66 696c 656e 616d 6529 0d0a 2020  as_filename)..  
+00007950: 2020 7769 7468 206f 7065 6e28 636c 6173    with open(clas
+00007960: 7379 5f78 6d6c 5f63 6f75 6e74 7269 6573  sy_xml_countries
+00007970: 5f66 6978 7475 7265 2e78 6d6c 5f66 696c  _fixture.xml_fil
+00007980: 6529 2061 7320 6669 6c65 3a0d 0a20 2020  e) as file:..   
+00007990: 2020 2020 2063 6f75 6e74 7269 6573 5f74       countries_t
+000079a0: 6578 7420 3d20 6669 6c65 2e72 6561 6428  ext = file.read(
+000079b0: 290d 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
+000079c0: 2873 6176 655f 6173 5f66 696c 656e 616d  (save_as_filenam
+000079d0: 6529 2061 7320 6669 6c65 3a0d 0a20 2020  e) as file:..   
+000079e0: 2020 2020 2074 656d 705f 636f 756e 7472       temp_countr
+000079f0: 6965 735f 7465 7874 203d 2066 696c 652e  ies_text = file.
+00007a00: 7265 6164 2829 0d0a 2020 2020 6f73 2e72  read()..    os.r
+00007a10: 656d 6f76 6528 7361 7665 5f61 735f 6669  emove(save_as_fi
+00007a20: 6c65 6e61 6d65 290d 0a20 2020 2061 7373  lename)..    ass
+00007a30: 6572 7420 636f 756e 7472 6965 735f 7465  ert countries_te
+00007a40: 7874 203d 3d20 7465 6d70 5f63 6f75 6e74  xt == temp_count
+00007a50: 7269 6573 5f74 6578 740d 0a0d 0a0d 0a64  ries_text......d
+00007a60: 6566 2074 6573 745f 6d6f 6469 6679 5f61  ef test_modify_a
+00007a70: 6e64 5f73 6176 655f 786d 6c28 636c 6173  nd_save_xml(clas
+00007a80: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+00007a90: 7475 7265 293a 0d0a 2020 2020 636c 6173  ture):..    clas
+00007aa0: 7379 5f78 6d6c 5f65 6d70 7479 5f66 6978  sy_xml_empty_fix
+00007ab0: 7475 7265 2e63 6f75 6e74 7279 203d 2058  ture.country = X
+00007ac0: 6d6c 456c 656d 656e 7428 6174 7472 6962  mlElement(attrib
+00007ad0: 7574 6573 3d7b 226e 616d 6522 3a20 224c  utes={"name": "L
+00007ae0: 6965 6368 7465 6e73 7465 696e 227d 290d  iechtenstein"}).
+00007af0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00007b00: 656d 7074 795f 6669 7874 7572 652e 636f  empty_fixture.co
+00007b10: 756e 7472 795b 305d 2e72 616e 6b20 3d20  untry[0].rank = 
+00007b20: 586d 6c45 6c65 6d65 6e74 2874 6578 743d  XmlElement(text=
+00007b30: 3129 0d0a 2020 2020 636c 6173 7379 5f78  1)..    classy_x
+00007b40: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
+00007b50: 2e63 6f75 6e74 7279 5b30 5d2e 7965 6172  .country[0].year
+00007b60: 203d 2058 6d6c 456c 656d 656e 7428 7465   = XmlElement(te
+00007b70: 7874 3d32 3030 3829 0d0a 2020 2020 636c  xt=2008)..    cl
+00007b80: 6173 7379 5f78 6d6c 5f65 6d70 7479 5f66  assy_xml_empty_f
+00007b90: 6978 7475 7265 2e63 6f75 6e74 7279 5b30  ixture.country[0
+00007ba0: 5d2e 6764 7070 6320 3d20 586d 6c45 6c65  ].gdppc = XmlEle
+00007bb0: 6d65 6e74 2874 6578 743d 3134 3131 3030  ment(text=141100
+00007bc0: 290d 0a20 2020 2063 6c61 7373 795f 786d  )..    classy_xm
+00007bd0: 6c5f 656d 7074 795f 6669 7874 7572 652e  l_empty_fixture.
+00007be0: 636f 756e 7472 795b 305d 2e6e 6569 6768  country[0].neigh
+00007bf0: 626f 7220 3d20 586d 6c45 6c65 6d65 6e74  bor = XmlElement
+00007c00: 280d 0a20 2020 2020 2020 2061 7474 7269  (..        attri
+00007c10: 6275 7465 733d 7b22 6e61 6d65 223a 2022  butes={"name": "
+00007c20: 4175 7374 7269 6122 2c20 2264 6972 6563  Austria", "direc
+00007c30: 7469 6f6e 223a 2022 4522 7d0d 0a20 2020  tion": "E"}..   
+00007c40: 2029 0d0a 2020 2020 636c 6173 7379 5f78   )..    classy_x
+00007c50: 6d6c 5f65 6d70 7479 5f66 6978 7475 7265  ml_empty_fixture
+00007c60: 2e63 6f75 6e74 7279 5b30 5d2e 6e65 6967  .country[0].neig
+00007c70: 6862 6f72 203d 2058 6d6c 456c 656d 656e  hbor = XmlElemen
+00007c80: 7428 0d0a 2020 2020 2020 2020 6174 7472  t(..        attr
+00007c90: 6962 7574 6573 3d7b 226e 616d 6522 3a20  ibutes={"name": 
+00007ca0: 2253 7769 747a 6572 6c61 6e64 222c 2022  "Switzerland", "
+00007cb0: 6469 7265 6374 696f 6e22 3a20 2257 227d  direction": "W"}
+00007cc0: 0d0a 2020 2020 290d 0a0d 0a20 2020 2063  ..    )....    c
+00007cd0: 6c61 7373 795f 786d 6c5f 656d 7074 795f  lassy_xml_empty_
+00007ce0: 6669 7874 7572 652e 636f 756e 7472 7920  fixture.country 
+00007cf0: 3d20 586d 6c45 6c65 6d65 6e74 2829 0d0a  = XmlElement()..
+00007d00: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
+00007d10: 6d70 7479 5f66 6978 7475 7265 2e63 6f75  mpty_fixture.cou
+00007d20: 6e74 7279 5b31 5d2e 6e61 6d65 203d 2022  ntry[1].name = "
+00007d30: 5369 6e67 6170 6f72 6522 0d0a 2020 2020  Singapore"..    
+00007d40: 636c 6173 7379 5f78 6d6c 5f65 6d70 7479  classy_xml_empty
+00007d50: 5f66 6978 7475 7265 2e63 6f75 6e74 7279  _fixture.country
+00007d60: 5b31 5d2e 7261 6e6b 203d 2058 6d6c 456c  [1].rank = XmlEl
+00007d70: 656d 656e 7428 290d 0a20 2020 2063 6c61  ement()..    cla
+00007d80: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007d90: 7874 7572 652e 636f 756e 7472 795b 315d  xture.country[1]
+00007da0: 2e72 616e 6b2e 7465 7874 203d 2034 0d0a  .rank.text = 4..
+00007db0: 2020 2020 636c 6173 7379 5f78 6d6c 5f65      classy_xml_e
+00007dc0: 6d70 7479 5f66 6978 7475 7265 2e63 6f75  mpty_fixture.cou
+00007dd0: 6e74 7279 5b31 5d2e 7965 6172 203d 2058  ntry[1].year = X
+00007de0: 6d6c 456c 656d 656e 7428 290d 0a20 2020  mlElement()..   
+00007df0: 2063 6c61 7373 795f 786d 6c5f 656d 7074   classy_xml_empt
+00007e00: 795f 6669 7874 7572 652e 636f 756e 7472  y_fixture.countr
+00007e10: 795b 315d 2e79 6561 722e 7465 7874 203d  y[1].year.text =
+00007e20: 2032 3031 310d 0a20 2020 2063 6c61 7373   2011..    class
+00007e30: 795f 786d 6c5f 656d 7074 795f 6669 7874  y_xml_empty_fixt
+00007e40: 7572 652e 636f 756e 7472 795b 315d 2e67  ure.country[1].g
+00007e50: 6470 7063 203d 2058 6d6c 456c 656d 656e  dppc = XmlElemen
+00007e60: 7428 290d 0a20 2020 2063 6c61 7373 795f  t()..    classy_
+00007e70: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00007e80: 652e 636f 756e 7472 795b 315d 2e67 6470  e.country[1].gdp
+00007e90: 7063 2e74 6578 7420 3d20 3539 3930 300d  pc.text = 59900.
+00007ea0: 0a20 2020 2063 6c61 7373 795f 786d 6c5f  .    classy_xml_
+00007eb0: 656d 7074 795f 6669 7874 7572 652e 636f  empty_fixture.co
+00007ec0: 756e 7472 795b 315d 2e6e 6569 6768 626f  untry[1].neighbo
+00007ed0: 7220 3d20 586d 6c45 6c65 6d65 6e74 2829  r = XmlElement()
+00007ee0: 0d0a 2020 2020 636c 6173 7379 5f78 6d6c  ..    classy_xml
+00007ef0: 5f65 6d70 7479 5f66 6978 7475 7265 2e63  _empty_fixture.c
+00007f00: 6f75 6e74 7279 5b31 5d2e 6e65 6967 6862  ountry[1].neighb
+00007f10: 6f72 5b30 5d2e 6e61 6d65 203d 2022 4d61  or[0].name = "Ma
+00007f20: 6c61 7973 6961 220d 0a20 2020 2063 6c61  laysia"..    cla
+00007f30: 7373 795f 786d 6c5f 656d 7074 795f 6669  ssy_xml_empty_fi
+00007f40: 7874 7572 652e 636f 756e 7472 795b 315d  xture.country[1]
+00007f50: 2e6e 6569 6768 626f 725b 305d 2e64 6972  .neighbor[0].dir
+00007f60: 6563 7469 6f6e 203d 2022 4e22 0d0a 0d0a  ection = "N"....
+00007f70: 2020 2020 6669 6c65 7061 7468 203d 206f      filepath = o
+00007f80: 732e 7061 7468 2e73 706c 6974 285f 5f66  s.path.split(__f
+00007f90: 696c 655f 5f29 5b30 5d0d 0a20 2020 2067  ile__)[0]..    g
+00007fa0: 656e 5f63 6f75 6e74 7269 6573 5f66 696c  en_countries_fil
+00007fb0: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
+00007fc0: 6a6f 696e 2866 696c 6570 6174 682c 2022  join(filepath, "
+00007fd0: 636f 756e 7472 6965 735f 6765 6e2e 786d  countries_gen.xm
+00007fe0: 6c22 290d 0a20 2020 2063 6c61 7373 795f  l")..    classy_
+00007ff0: 786d 6c5f 656d 7074 795f 6669 7874 7572  xml_empty_fixtur
+00008000: 652e 7361 7665 5f61 7328 6765 6e5f 636f  e.save_as(gen_co
+00008010: 756e 7472 6965 735f 6669 6c65 6e61 6d65  untries_filename
+00008020: 290d 0a0d 0a20 2020 2077 6974 6820 6f70  )....    with op
+00008030: 656e 2867 656e 5f63 6f75 6e74 7269 6573  en(gen_countries
+00008040: 5f66 696c 656e 616d 6529 2061 7320 6669  _filename) as fi
+00008050: 6c65 3a0d 0a20 2020 2020 2020 2063 6f75  le:..        cou
+00008060: 6e74 7269 6573 5f67 656e 5f74 6578 7420  ntries_gen_text 
+00008070: 3d20 6669 6c65 2e72 6561 6428 290d 0a20  = file.read().. 
+00008080: 2020 206f 732e 7265 6d6f 7665 2867 656e     os.remove(gen
+00008090: 5f63 6f75 6e74 7269 6573 5f66 696c 656e  _countries_filen
+000080a0: 616d 6529 0d0a 0d0a 2020 2020 6669 6c65  ame)....    file
+000080b0: 7061 7468 203d 206f 732e 7061 7468 2e73  path = os.path.s
+000080c0: 706c 6974 285f 5f66 696c 655f 5f29 5b30  plit(__file__)[0
+000080d0: 5d0d 0a20 2020 2063 6f75 6e74 7269 6573  ]..    countries
+000080e0: 5f66 696c 656e 616d 6520 3d20 6f73 2e70  _filename = os.p
+000080f0: 6174 682e 6a6f 696e 2866 696c 6570 6174  ath.join(filepat
+00008100: 682c 2022 636f 756e 7472 6965 732e 786d  h, "countries.xm
+00008110: 6c22 290d 0a20 2020 2077 6974 6820 6f70  l")..    with op
+00008120: 656e 2863 6f75 6e74 7269 6573 5f66 696c  en(countries_fil
+00008130: 656e 616d 6529 2061 7320 6669 6c65 3a0d  ename) as file:.
+00008140: 0a20 2020 2020 2020 2063 6f75 6e74 7269  .        countri
+00008150: 6573 5f74 6578 7420 3d20 6669 6c65 2e72  es_text = file.r
+00008160: 6561 6428 290d 0a0d 0a20 2020 2061 7373  ead()....    ass
+00008170: 6572 7420 636f 756e 7472 6965 735f 6765  ert countries_ge
+00008180: 6e5f 7465 7874 203d 3d20 636f 756e 7472  n_text == countr
+00008190: 6965 735f 7465 7874 0d0a 0d0a 0d0a 6465  ies_text......de
+000081a0: 6620 7465 7374 5f70 6173 7369 6e67 5f78  f test_passing_x
+000081b0: 6d6c 5f61 735f 7374 7269 6e67 2829 3a0d  ml_as_string():.
+000081c0: 0a20 2020 2078 6d6c 5f73 7472 203d 2022  .    xml_str = "
+000081d0: 2222 0d0a 2020 2020 2020 2020 3c72 6f6f  ""..        <roo
+000081e0: 743e 0d0a 2020 2020 2020 2020 2020 2020  t>..            
+000081f0: 3c63 6f75 6e74 7279 206e 616d 653d 224c  <country name="L
+00008200: 6965 6368 7465 6e73 7465 696e 223e 0d0a  iechtenstein">..
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 3c72 616e 6b3e 313c 2f72 616e 6b3e 0d0a  <rank>1</rank>..
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 3c79 6561 723e 3230 3038 3c2f 7965 6172  <year>2008</year
+00008250: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
+00008260: 2020 203c 6764 7070 633e 3134 3131 3030     <gdppc>141100
+00008270: 3c2f 6764 7070 633e 0d0a 2020 2020 2020  </gdppc>..      
+00008280: 2020 2020 2020 2020 2020 3c6e 6569 6768            <neigh
+00008290: 626f 7220 6e61 6d65 3d22 4175 7374 7269  bor name="Austri
+000082a0: 6122 2064 6972 6563 7469 6f6e 3d22 4522  a" direction="E"
+000082b0: 2f3e 0d0a 2020 2020 2020 2020 2020 2020  />..            
+000082c0: 2020 2020 3c6e 6569 6768 626f 7220 6e61      <neighbor na
+000082d0: 6d65 3d22 5377 6974 7a65 726c 616e 6422  me="Switzerland"
+000082e0: 2064 6972 6563 7469 6f6e 3d22 5722 2f3e   direction="W"/>
+000082f0: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
+00008300: 636f 756e 7472 793e 0d0a 2020 2020 2020  country>..      
+00008310: 2020 2020 2020 3c63 6f75 6e74 7279 206e        <country n
+00008320: 616d 653d 2253 696e 6761 706f 7265 223e  ame="Singapore">
+00008330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008340: 2020 3c72 616e 6b3e 343c 2f72 616e 6b3e    <rank>4</rank>
+00008350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008360: 2020 3c79 6561 723e 3230 3131 3c2f 7965    <year>2011</ye
+00008370: 6172 3e0d 0a20 2020 2020 2020 2020 2020  ar>..           
+00008380: 2020 2020 203c 6764 7070 633e 3539 3930       <gdppc>5990
+00008390: 303c 2f67 6470 7063 3e0d 0a20 2020 2020  0</gdppc>..     
+000083a0: 2020 2020 2020 2020 2020 203c 6e65 6967             <neig
+000083b0: 6862 6f72 206e 616d 653d 224d 616c 6179  hbor name="Malay
+000083c0: 7369 6122 2064 6972 6563 7469 6f6e 3d22  sia" direction="
+000083d0: 4e22 2f3e 0d0a 2020 2020 2020 2020 2020  N"/>..          
+000083e0: 2020 3c2f 636f 756e 7472 793e 0d0a 2020    </country>..  
+000083f0: 2020 2020 2020 3c2f 726f 6f74 3e0d 0a20        </root>.. 
+00008400: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00008410: 636c 6173 7379 203d 2043 6c61 7373 7958  classy = ClassyX
+00008420: 6d6c 2878 6d6c 5f73 7472 290d 0a20 2020  ml(xml_str)..   
+00008430: 2061 7373 6572 7420 6861 7361 7474 7228   assert hasattr(
+00008440: 636c 6173 7379 2c20 2263 6f75 6e74 7279  classy, "country
+00008450: 2229 0d0a 2020 2020 6173 7365 7274 2063  ")..    assert c
+00008460: 6c61 7373 792e 636f 756e 7472 795b 305d  lassy.country[0]
+00008470: 2e6e 616d 6520 3d3d 2022 4c69 6563 6874  .name == "Liecht
+00008480: 656e 7374 6569 6e22 0d0a 2020 2020 6173  enstein"..    as
+00008490: 7365 7274 2063 6c61 7373 792e 636f 756e  sert classy.coun
+000084a0: 7472 795b 305d 2e72 616e 6b2e 7465 7874  try[0].rank.text
+000084b0: 203d 3d20 2231 220d 0a20 2020 2061 7373   == "1"..    ass
+000084c0: 6572 7420 636c 6173 7379 2e63 6f75 6e74  ert classy.count
+000084d0: 7279 5b30 5d2e 7965 6172 2e74 6578 7420  ry[0].year.text 
+000084e0: 3d3d 2022 3230 3038 220d 0a20 2020 2061  == "2008"..    a
+000084f0: 7373 6572 7420 636c 6173 7379 2e63 6f75  ssert classy.cou
+00008500: 6e74 7279 5b30 5d2e 6764 7070 632e 7465  ntry[0].gdppc.te
+00008510: 7874 203d 3d20 2231 3431 3130 3022 0d0a  xt == "141100"..
+00008520: 2020 2020 6173 7365 7274 2063 6c61 7373      assert class
+00008530: 792e 636f 756e 7472 795b 305d 2e6e 6569  y.country[0].nei
+00008540: 6768 626f 725b 305d 2e6e 616d 6520 3d3d  ghbor[0].name ==
+00008550: 2022 4175 7374 7269 6122 0d0a 2020 2020   "Austria"..    
+00008560: 6173 7365 7274 2063 6c61 7373 792e 636f  assert classy.co
+00008570: 756e 7472 795b 305d 2e6e 6569 6768 626f  untry[0].neighbo
+00008580: 725b 305d 2e64 6972 6563 7469 6f6e 203d  r[0].direction =
+00008590: 3d20 2245 220d 0a20 2020 2061 7373 6572  = "E"..    asser
+000085a0: 7420 636c 6173 7379 2e63 6f75 6e74 7279  t classy.country
+000085b0: 5b30 5d2e 6e65 6967 6862 6f72 5b31 5d2e  [0].neighbor[1].
+000085c0: 6e61 6d65 203d 3d20 2253 7769 747a 6572  name == "Switzer
+000085d0: 6c61 6e64 220d 0a20 2020 2061 7373 6572  land"..    asser
+000085e0: 7420 636c 6173 7379 2e63 6f75 6e74 7279  t classy.country
+000085f0: 5b30 5d2e 6e65 6967 6862 6f72 5b31 5d2e  [0].neighbor[1].
+00008600: 6469 7265 6374 696f 6e20 3d3d 2022 5722  direction == "W"
+00008610: 0d0a 2020 2020 6173 7365 7274 2063 6c61  ..    assert cla
+00008620: 7373 792e 636f 756e 7472 795b 315d 2e6e  ssy.country[1].n
+00008630: 616d 6520 3d3d 2022 5369 6e67 6170 6f72  ame == "Singapor
+00008640: 6522 0d0a 2020 2020 6173 7365 7274 2063  e"..    assert c
+00008650: 6c61 7373 792e 636f 756e 7472 795b 315d  lassy.country[1]
+00008660: 2e72 616e 6b2e 7465 7874 203d 3d20 2234  .rank.text == "4
+00008670: 220d 0a20 2020 2061 7373 6572 7420 636c  "..    assert cl
+00008680: 6173 7379 2e63 6f75 6e74 7279 5b31 5d2e  assy.country[1].
+00008690: 7965 6172 2e74 6578 7420 3d3d 2022 3230  year.text == "20
+000086a0: 3131 220d 0a20 2020 2061 7373 6572 7420  11"..    assert 
+000086b0: 636c 6173 7379 2e63 6f75 6e74 7279 5b31  classy.country[1
+000086c0: 5d2e 6764 7070 632e 7465 7874 203d 3d20  ].gdppc.text == 
+000086d0: 2235 3939 3030 220d 0a20 2020 2061 7373  "59900"..    ass
+000086e0: 6572 7420 636c 6173 7379 2e63 6f75 6e74  ert classy.count
+000086f0: 7279 5b31 5d2e 6e65 6967 6862 6f72 5b30  ry[1].neighbor[0
+00008700: 5d2e 6e61 6d65 203d 3d20 224d 616c 6179  ].name == "Malay
+00008710: 7369 6122 0d0a 2020 2020 6173 7365 7274  sia"..    assert
+00008720: 2063 6c61 7373 792e 636f 756e 7472 795b   classy.country[
+00008730: 315d 2e6e 6569 6768 626f 725b 305d 2e64  1].neighbor[0].d
+00008740: 6972 6563 7469 6f6e 203d 3d20 224e 220d  irection == "N".
+00008750: 0a                                       .
```

