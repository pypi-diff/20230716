# Comparing `tmp/presentpy-0.5.0.tar.gz` & `tmp/presentpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presentpy-0.5.0.tar", max compression
+gzip compressed data, was "presentpy-0.8.0.tar", max compression
```

## Comparing `presentpy-0.5.0.tar` & `presentpy-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      907 2023-07-11 19:21:00.917271 presentpy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       58 2023-07-11 19:21:00.917271 presentpy-0.5.0/readme.md
--rw-r--r--   0        0        0       22 2023-07-11 19:21:00.917271 presentpy-0.5.0/src/presentpy/__init__.py
--rw-r--r--   0        0        0      704 2023-07-11 19:21:00.917271 presentpy-0.5.0/src/presentpy/__main__.py
--rw-r--r--   0        0        0     1866 2023-07-11 19:21:00.921271 presentpy-0.5.0/src/presentpy/code_slide_source.py
--rw-r--r--   0        0        0      564 2023-07-11 19:21:00.921271 presentpy-0.5.0/src/presentpy/notebook_processor.py
--rw-r--r--   0        0        0   132043 2023-07-11 19:21:30.317594 presentpy-0.5.0/src/presentpy/slide_templates/template-dark.pptx
--rw-r--r--   0        0        0   131814 2023-07-11 19:21:30.313594 presentpy-0.5.0/src/presentpy/slide_templates/template-light.pptx
--rw-r--r--   0        0        0        0 2023-07-11 19:21:00.925271 presentpy-0.5.0/src/presentpy/writers/__init__.py
--rw-r--r--   0        0        0     3658 2023-07-11 19:21:00.925271 presentpy-0.5.0/src/presentpy/writers/pptx_writer.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 presentpy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      908 2023-07-16 14:48:52.371460 presentpy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-16 14:48:52.371460 presentpy-0.8.0/readme.md
+-rw-r--r--   0        0        0       22 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/__init__.py
+-rw-r--r--   0        0        0      786 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/__main__.py
+-rw-r--r--   0        0        0     1866 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/code_slide_source.py
+-rw-r--r--   0        0        0     1121 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/config/__init__.py
+-rw-r--r--   0        0        0      855 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/config/read_only_dot_dict.py
+-rw-r--r--   0        0        0      564 2023-07-16 14:48:52.371460 presentpy-0.8.0/src/presentpy/notebook_processor.py
+-rw-r--r--   0        0        0   132043 2023-07-16 14:49:30.595578 presentpy-0.8.0/src/presentpy/slide_templates/template-dark.pptx
+-rw-r--r--   0        0        0   131814 2023-07-16 14:49:30.587578 presentpy-0.8.0/src/presentpy/slide_templates/template-light.pptx
+-rw-r--r--   0        0        0        0 2023-07-16 14:48:52.379460 presentpy-0.8.0/src/presentpy/writers/__init__.py
+-rw-r--r--   0        0        0     3901 2023-07-16 14:48:52.379460 presentpy-0.8.0/src/presentpy/writers/pptx_writer.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 presentpy-0.8.0/PKG-INFO
```

### Comparing `presentpy-0.5.0/pyproject.toml` & `presentpy-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "presentpy"
-version = "0.5.0"
+version = "0.8.0"
 description = "Create slides from Jupyter Notebooks"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 include = ["src/presentpy/**/*"]
 
 [tool.poetry.scripts]
@@ -19,15 +19,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 bump2version = "^1.0.1"
 isort = "^5.12.0"
 mkdocs-material = "^9.1.18"
 pytest = "^7.3.2"
-ruff = "^0.0.272"
+tomli-w = "^1.0.0"
 
 [tool.poetry.group.juptyter.dependencies]
 jupyter = "^1.0.0"
 jupyterlab = "^4.0.2"
 
 [tool.ruff]
 select = ["E", "F", "I","C90", "N"]
```

### Comparing `presentpy-0.5.0/src/presentpy/code_slide_source.py` & `presentpy-0.8.0/src/presentpy/code_slide_source.py`

 * *Files identical despite different names*

### Comparing `presentpy-0.5.0/src/presentpy/notebook_processor.py` & `presentpy-0.8.0/src/presentpy/notebook_processor.py`

 * *Files identical despite different names*

### Comparing `presentpy-0.5.0/src/presentpy/slide_templates/template-dark.pptx` & `presentpy-0.8.0/src/presentpy/slide_templates/template-light.pptx`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,52 +1,52 @@
-Zip file size: 132043 bytes, number of entries: 50
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 _rels/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 docProps/
--rw-r--r--  2.0 unx     3307 b- stor 23-Jul-11 19:21 [Content_Types].xml
--rw-r--r--  2.0 unx      714 b- stor 23-Jul-11 19:21 _rels/.rels
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideLayouts/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slides/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/_rels/
--rw-r--r--  2.0 unx      834 b- stor 23-Jul-11 19:21 ppt/viewProps.xml
--rw-r--r--  2.0 unx      149 b- stor 23-Jul-11 19:21 ppt/tableStyles.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/theme/
--rw-r--r--  2.0 unx     3824 b- stor 23-Jul-11 19:21 ppt/presentation.xml
--rw-r--r--  2.0 unx      820 b- stor 23-Jul-11 19:21 ppt/presProps.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideMasters/
--rw-r--r--  2.0 unx     5129 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout2.xml
--rw-r--r--  2.0 unx    10634 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout6.xml
--rw-r--r--  2.0 unx     7702 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout10.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/
--rw-r--r--  2.0 unx     3134 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout8.xml
--rw-r--r--  2.0 unx     6050 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout1.xml
--rw-r--r--  2.0 unx     6660 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout5.xml
--rw-r--r--  2.0 unx     7298 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout4.xml
--rw-r--r--  2.0 unx     7945 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout9.xml
--rw-r--r--  2.0 unx     7068 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout3.xml
--rw-r--r--  2.0 unx     3859 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout7.xml
--rw-r--r--  2.0 unx     5471 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout12.xml
--rw-r--r--  2.0 unx     5185 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout11.xml
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout12.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout2.xml.rels
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slides/_rels/
--rw-r--r--  2.0 unx     2065 b- stor 23-Jul-11 19:21 ppt/slides/slide1.xml
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slides/_rels/slide1.xml.rels
--rw-r--r--  2.0 unx      956 b- stor 23-Jul-11 19:21 ppt/_rels/presentation.xml.rels
--rw-r--r--  2.0 unx    10001 b- stor 23-Jul-11 19:21 ppt/theme/theme1.xml
--rw-r--r--  2.0 unx    17210 b- stor 23-Jul-11 19:21 ppt/slideMasters/slideMaster1.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideMasters/_rels/
--rw-r--r--  2.0 unx     2141 b- stor 23-Jul-11 19:21 ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-r--r--  2.0 unx     1442 b- stor 23-Jul-11 19:21 docProps/app.xml
--rw-r--r--  2.0 unx     1441 b- stor 23-Jul-11 19:21 docProps/thumbnail.jpeg
--rw-r--r--  2.0 unx      695 b- stor 23-Jul-11 19:21 docProps/core.xml
-50 files, 125387 bytes uncompressed, 125387 bytes compressed:  0.0%
+Zip file size: 131814 bytes, number of entries: 50
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 _rels/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 docProps/
+-rw-r--r--  2.0 unx     3307 b- stor 23-Jul-16 14:48 [Content_Types].xml
+-rw-r--r--  2.0 unx      714 b- stor 23-Jul-16 14:48 _rels/.rels
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideLayouts/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slides/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/_rels/
+-rw-r--r--  2.0 unx      834 b- stor 23-Jul-16 14:48 ppt/viewProps.xml
+-rw-r--r--  2.0 unx      149 b- stor 23-Jul-16 14:48 ppt/tableStyles.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/theme/
+-rw-r--r--  2.0 unx     3642 b- stor 23-Jul-16 14:48 ppt/presentation.xml
+-rw-r--r--  2.0 unx      820 b- stor 23-Jul-16 14:48 ppt/presProps.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideMasters/
+-rw-r--r--  2.0 unx     5130 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout2.xml
+-rw-r--r--  2.0 unx    10635 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout6.xml
+-rw-r--r--  2.0 unx     7703 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout10.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/
+-rw-r--r--  2.0 unx     3135 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout8.xml
+-rw-r--r--  2.0 unx     6051 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout1.xml
+-rw-r--r--  2.0 unx     6661 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout5.xml
+-rw-r--r--  2.0 unx     7299 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout4.xml
+-rw-r--r--  2.0 unx     7946 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout9.xml
+-rw-r--r--  2.0 unx     7009 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout3.xml
+-rw-r--r--  2.0 unx     3860 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout7.xml
+-rw-r--r--  2.0 unx     5472 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout12.xml
+-rw-r--r--  2.0 unx     5186 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout11.xml
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout12.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout2.xml.rels
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slides/_rels/
+-rw-r--r--  2.0 unx     2065 b- stor 23-Jul-16 14:48 ppt/slides/slide1.xml
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slides/_rels/slide1.xml.rels
+-rw-r--r--  2.0 unx      956 b- stor 23-Jul-16 14:48 ppt/_rels/presentation.xml.rels
+-rw-r--r--  2.0 unx    10001 b- stor 23-Jul-16 14:48 ppt/theme/theme1.xml
+-rw-r--r--  2.0 unx    17211 b- stor 23-Jul-16 14:48 ppt/slideMasters/slideMaster1.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideMasters/_rels/
+-rw-r--r--  2.0 unx     2141 b- stor 23-Jul-16 14:48 ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-r--r--  2.0 unx     1442 b- stor 23-Jul-16 14:48 docProps/app.xml
+-rw-r--r--  2.0 unx     1441 b- stor 23-Jul-16 14:48 docProps/thumbnail.jpeg
+-rw-r--r--  2.0 unx      695 b- stor 23-Jul-16 14:48 docProps/core.xml
+50 files, 125158 bytes uncompressed, 125158 bytes compressed:  0.0%
```

#### ppt/presentation.xml

##### ppt/presentation.xml

```diff
@@ -99,13 +99,8 @@
         </a:solidFill>
         <a:latin typeface="+mn-lt"/>
         <a:ea typeface="+mn-ea"/>
         <a:cs typeface="+mn-cs"/>
       </a:defRPr>
     </a:lvl9pPr>
   </p:defaultTextStyle>
-  <p:extLst>
-    <p:ext uri="{EFAFB233-063F-42B5-8137-9DF3F51BA10A}">
-      <p15:sldGuideLst xmlns:p15="http://schemas.microsoft.com/office/powerpoint/2012/main"/>
-    </p:ext>
-  </p:extLst>
 </p:presentation>
```

#### ppt/slideLayouts/slideLayout2.xml

##### ppt/slideLayouts/slideLayout2.xml

```diff
@@ -121,15 +121,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout6.xml

##### ppt/slideLayouts/slideLayout6.xml

```diff
@@ -336,15 +336,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout10.xml

##### ppt/slideLayouts/slideLayout10.xml

```diff
@@ -210,15 +210,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout8.xml

##### ppt/slideLayouts/slideLayout8.xml

```diff
@@ -34,15 +34,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout1.xml

##### ppt/slideLayouts/slideLayout1.xml

```diff
@@ -143,15 +143,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout5.xml

##### ppt/slideLayouts/slideLayout5.xml

```diff
@@ -189,15 +189,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout4.xml

##### ppt/slideLayouts/slideLayout4.xml

```diff
@@ -197,15 +197,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout9.xml

##### ppt/slideLayouts/slideLayout9.xml

```diff
@@ -234,15 +234,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout3.xml

##### ppt/slideLayouts/slideLayout3.xml

```diff
@@ -114,46 +114,46 @@
                 <a:cs typeface="Consolas" panose="020B0609020204030204" pitchFamily="49" charset="0"/>
               </a:defRPr>
             </a:lvl5pPr>
           </a:lstStyle>
           <a:p>
             <a:pPr lvl="0"/>
             <a:r>
-              <a:rPr lang="en-GB" dirty="0"/>
+              <a:rPr lang="en-GB"/>
               <a:t>Click to edit Master text styles</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="1"/>
             <a:r>
-              <a:rPr lang="en-GB" dirty="0"/>
+              <a:rPr lang="en-GB"/>
               <a:t>Second level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="2"/>
             <a:r>
-              <a:rPr lang="en-GB" dirty="0"/>
+              <a:rPr lang="en-GB"/>
               <a:t>Third level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="3"/>
             <a:r>
-              <a:rPr lang="en-GB" dirty="0"/>
+              <a:rPr lang="en-GB"/>
               <a:t>Fourth level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="4"/>
             <a:r>
-              <a:rPr lang="en-GB" dirty="0"/>
+              <a:rPr lang="en-GB"/>
               <a:t>Fifth level</a:t>
             </a:r>
-            <a:endParaRPr lang="en-US" dirty="0"/>
+            <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
           <p:cNvPr id="4" name="Date Placeholder 3">
             <a:extLst>
@@ -172,15 +172,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout7.xml

##### ppt/slideLayouts/slideLayout7.xml

```diff
@@ -63,15 +63,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout12.xml

##### ppt/slideLayouts/slideLayout12.xml

```diff
@@ -131,15 +131,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout11.xml

##### ppt/slideLayouts/slideLayout11.xml

```diff
@@ -121,15 +121,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideMasters/slideMaster1.xml

##### ppt/slideMasters/slideMaster1.xml

```diff
@@ -164,15 +164,15 @@
                 </a:solidFill>
               </a:defRPr>
             </a:lvl1pPr>
           </a:lstStyle>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>7/6/23</a:t>
+              <a:t>6/11/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
@@ -267,15 +267,15 @@
     </p:spTree>
     <p:extLst>
       <p:ext uri="{BB962C8B-B14F-4D97-AF65-F5344CB8AC3E}">
         <p14:creationId xmlns:p14="http://schemas.microsoft.com/office/powerpoint/2010/main" val="3861594154"/>
       </p:ext>
     </p:extLst>
   </p:cSld>
-  <p:clrMap bg1="dk1" tx1="lt1" bg2="dk2" tx2="lt2" accent1="accent1" accent2="accent2" accent3="accent3" accent4="accent4" accent5="accent5" accent6="accent6" hlink="hlink" folHlink="folHlink"/>
+  <p:clrMap bg1="lt1" tx1="dk1" bg2="lt2" tx2="dk2" accent1="accent1" accent2="accent2" accent3="accent3" accent4="accent4" accent5="accent5" accent6="accent6" hlink="hlink" folHlink="folHlink"/>
   <p:sldLayoutIdLst>
     <p:sldLayoutId id="2147483649" r:id="rId1"/>
     <p:sldLayoutId id="2147483650" r:id="rId2"/>
     <p:sldLayoutId id="2147483660" r:id="rId3"/>
     <p:sldLayoutId id="2147483651" r:id="rId4"/>
     <p:sldLayoutId id="2147483652" r:id="rId5"/>
     <p:sldLayoutId id="2147483653" r:id="rId6"/>
```

#### docProps/thumbnail.jpeg

##### Image content

```diff
@@ -1,20 +1,20 @@
                                                             
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
-                                                            
+  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  . 
+   .       .       .       .       .       .       .        
+     .  .    .  .    .  .    .  .    .  .    .  .    .  . . 
+ .       .       .       .       .       .       .          
+   .  .    .  .    .  .    .  .    .  .    .  .    .  . .  .
+  .    .  .    .  .    .  .    .  .    .  .    .  .         
+    .       .       .       .       .       .       . .  .  
+  .   . .    .  .    .  .    .  .    .  .    .  .       .  .
+    .     .    .  .    .  .    .  .    .  .    .  . .       
+  .    .   .       .       .       .       .          .  .  
+     .   .   .  .    .  .    .  .    .  .    .  .  .   .   .
+  .    .      .   .   .   .   .   .   .   .   .   .  .   .  
+    .     . .   .   .   .   .   .   .   .   .   .           
+  .   .           .       .       .       .        .  . .  .
+    .   . .  . .     . .     . .     . .     . .  .         
+  .         .    .       .       .       .          . .  .  
+     . .  .    .   . .     . .     . .     . .  .       .  .
+  .          .         . .     . .     . .     .  . .       
+    .  . . .    . .  .     .       .       .          .  .
```

#### docProps/core.xml

##### docProps/core.xml

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <cp:coreProperties xmlns:cp="http://schemas.openxmlformats.org/package/2006/metadata/core-properties" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:dcmitype="http://purl.org/dc/dcmitype/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <dc:title>PowerPoint Presentation</dc:title>
   <dc:creator>Antonio Feregrino Bolanos</dc:creator>
   <cp:lastModifiedBy>Antonio Feregrino Bolanos</cp:lastModifiedBy>
-  <cp:revision>2</cp:revision>
+  <cp:revision>1</cp:revision>
   <dcterms:created xsi:type="dcterms:W3CDTF">2023-06-11T16:06:38Z</dcterms:created>
-  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-07-06T15:57:40Z</dcterms:modified>
+  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-06-11T16:09:08Z</dcterms:modified>
 </cp:coreProperties>
```

### Comparing `presentpy-0.5.0/src/presentpy/slide_templates/template-light.pptx` & `presentpy-0.8.0/src/presentpy/slide_templates/template-dark.pptx`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,52 +1,52 @@
-Zip file size: 131814 bytes, number of entries: 50
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 _rels/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 docProps/
--rw-r--r--  2.0 unx     3307 b- stor 23-Jul-11 19:21 [Content_Types].xml
--rw-r--r--  2.0 unx      714 b- stor 23-Jul-11 19:21 _rels/.rels
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideLayouts/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slides/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/_rels/
--rw-r--r--  2.0 unx      834 b- stor 23-Jul-11 19:21 ppt/viewProps.xml
--rw-r--r--  2.0 unx      149 b- stor 23-Jul-11 19:21 ppt/tableStyles.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/theme/
--rw-r--r--  2.0 unx     3642 b- stor 23-Jul-11 19:21 ppt/presentation.xml
--rw-r--r--  2.0 unx      820 b- stor 23-Jul-11 19:21 ppt/presProps.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideMasters/
--rw-r--r--  2.0 unx     5130 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout2.xml
--rw-r--r--  2.0 unx    10635 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout6.xml
--rw-r--r--  2.0 unx     7703 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout10.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/
--rw-r--r--  2.0 unx     3135 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout8.xml
--rw-r--r--  2.0 unx     6051 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout1.xml
--rw-r--r--  2.0 unx     6661 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout5.xml
--rw-r--r--  2.0 unx     7299 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout4.xml
--rw-r--r--  2.0 unx     7946 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout9.xml
--rw-r--r--  2.0 unx     7009 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout3.xml
--rw-r--r--  2.0 unx     3860 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout7.xml
--rw-r--r--  2.0 unx     5472 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout12.xml
--rw-r--r--  2.0 unx     5186 b- stor 23-Jul-11 19:21 ppt/slideLayouts/slideLayout11.xml
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout12.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slideLayouts/_rels/slideLayout2.xml.rels
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slides/_rels/
--rw-r--r--  2.0 unx     2065 b- stor 23-Jul-11 19:21 ppt/slides/slide1.xml
--rw-r--r--  2.0 unx      281 b- stor 23-Jul-11 19:21 ppt/slides/_rels/slide1.xml.rels
--rw-r--r--  2.0 unx      956 b- stor 23-Jul-11 19:21 ppt/_rels/presentation.xml.rels
--rw-r--r--  2.0 unx    10001 b- stor 23-Jul-11 19:21 ppt/theme/theme1.xml
--rw-r--r--  2.0 unx    17211 b- stor 23-Jul-11 19:21 ppt/slideMasters/slideMaster1.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-11 19:21 ppt/slideMasters/_rels/
--rw-r--r--  2.0 unx     2141 b- stor 23-Jul-11 19:21 ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-r--r--  2.0 unx     1442 b- stor 23-Jul-11 19:21 docProps/app.xml
--rw-r--r--  2.0 unx     1441 b- stor 23-Jul-11 19:21 docProps/thumbnail.jpeg
--rw-r--r--  2.0 unx      695 b- stor 23-Jul-11 19:21 docProps/core.xml
-50 files, 125158 bytes uncompressed, 125158 bytes compressed:  0.0%
+Zip file size: 132043 bytes, number of entries: 50
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 _rels/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 docProps/
+-rw-r--r--  2.0 unx     3307 b- stor 23-Jul-16 14:48 [Content_Types].xml
+-rw-r--r--  2.0 unx      714 b- stor 23-Jul-16 14:48 _rels/.rels
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideLayouts/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slides/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/_rels/
+-rw-r--r--  2.0 unx      834 b- stor 23-Jul-16 14:48 ppt/viewProps.xml
+-rw-r--r--  2.0 unx      149 b- stor 23-Jul-16 14:48 ppt/tableStyles.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/theme/
+-rw-r--r--  2.0 unx     3824 b- stor 23-Jul-16 14:48 ppt/presentation.xml
+-rw-r--r--  2.0 unx      820 b- stor 23-Jul-16 14:48 ppt/presProps.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideMasters/
+-rw-r--r--  2.0 unx     5129 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout2.xml
+-rw-r--r--  2.0 unx    10634 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout6.xml
+-rw-r--r--  2.0 unx     7702 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout10.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/
+-rw-r--r--  2.0 unx     3134 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout8.xml
+-rw-r--r--  2.0 unx     6050 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout1.xml
+-rw-r--r--  2.0 unx     6660 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout5.xml
+-rw-r--r--  2.0 unx     7298 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout4.xml
+-rw-r--r--  2.0 unx     7945 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout9.xml
+-rw-r--r--  2.0 unx     7068 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout3.xml
+-rw-r--r--  2.0 unx     3859 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout7.xml
+-rw-r--r--  2.0 unx     5471 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout12.xml
+-rw-r--r--  2.0 unx     5185 b- stor 23-Jul-16 14:48 ppt/slideLayouts/slideLayout11.xml
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout12.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slideLayouts/_rels/slideLayout2.xml.rels
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slides/_rels/
+-rw-r--r--  2.0 unx     2065 b- stor 23-Jul-16 14:48 ppt/slides/slide1.xml
+-rw-r--r--  2.0 unx      281 b- stor 23-Jul-16 14:48 ppt/slides/_rels/slide1.xml.rels
+-rw-r--r--  2.0 unx      956 b- stor 23-Jul-16 14:48 ppt/_rels/presentation.xml.rels
+-rw-r--r--  2.0 unx    10001 b- stor 23-Jul-16 14:48 ppt/theme/theme1.xml
+-rw-r--r--  2.0 unx    17210 b- stor 23-Jul-16 14:48 ppt/slideMasters/slideMaster1.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-16 14:48 ppt/slideMasters/_rels/
+-rw-r--r--  2.0 unx     2141 b- stor 23-Jul-16 14:48 ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-r--r--  2.0 unx     1442 b- stor 23-Jul-16 14:48 docProps/app.xml
+-rw-r--r--  2.0 unx     1441 b- stor 23-Jul-16 14:48 docProps/thumbnail.jpeg
+-rw-r--r--  2.0 unx      695 b- stor 23-Jul-16 14:48 docProps/core.xml
+50 files, 125387 bytes uncompressed, 125387 bytes compressed:  0.0%
```

#### ppt/presentation.xml

##### ppt/presentation.xml

```diff
@@ -99,8 +99,13 @@
         </a:solidFill>
         <a:latin typeface="+mn-lt"/>
         <a:ea typeface="+mn-ea"/>
         <a:cs typeface="+mn-cs"/>
       </a:defRPr>
     </a:lvl9pPr>
   </p:defaultTextStyle>
+  <p:extLst>
+    <p:ext uri="{EFAFB233-063F-42B5-8137-9DF3F51BA10A}">
+      <p15:sldGuideLst xmlns:p15="http://schemas.microsoft.com/office/powerpoint/2012/main"/>
+    </p:ext>
+  </p:extLst>
 </p:presentation>
```

#### ppt/slideLayouts/slideLayout2.xml

##### ppt/slideLayouts/slideLayout2.xml

```diff
@@ -121,15 +121,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout6.xml

##### ppt/slideLayouts/slideLayout6.xml

```diff
@@ -336,15 +336,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout10.xml

##### ppt/slideLayouts/slideLayout10.xml

```diff
@@ -210,15 +210,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout8.xml

##### ppt/slideLayouts/slideLayout8.xml

```diff
@@ -34,15 +34,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout1.xml

##### ppt/slideLayouts/slideLayout1.xml

```diff
@@ -143,15 +143,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout5.xml

##### ppt/slideLayouts/slideLayout5.xml

```diff
@@ -189,15 +189,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout4.xml

##### ppt/slideLayouts/slideLayout4.xml

```diff
@@ -197,15 +197,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout9.xml

##### ppt/slideLayouts/slideLayout9.xml

```diff
@@ -234,15 +234,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout3.xml

##### ppt/slideLayouts/slideLayout3.xml

```diff
@@ -114,46 +114,46 @@
                 <a:cs typeface="Consolas" panose="020B0609020204030204" pitchFamily="49" charset="0"/>
               </a:defRPr>
             </a:lvl5pPr>
           </a:lstStyle>
           <a:p>
             <a:pPr lvl="0"/>
             <a:r>
-              <a:rPr lang="en-GB"/>
+              <a:rPr lang="en-GB" dirty="0"/>
               <a:t>Click to edit Master text styles</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="1"/>
             <a:r>
-              <a:rPr lang="en-GB"/>
+              <a:rPr lang="en-GB" dirty="0"/>
               <a:t>Second level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="2"/>
             <a:r>
-              <a:rPr lang="en-GB"/>
+              <a:rPr lang="en-GB" dirty="0"/>
               <a:t>Third level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="3"/>
             <a:r>
-              <a:rPr lang="en-GB"/>
+              <a:rPr lang="en-GB" dirty="0"/>
               <a:t>Fourth level</a:t>
             </a:r>
           </a:p>
           <a:p>
             <a:pPr lvl="4"/>
             <a:r>
-              <a:rPr lang="en-GB"/>
+              <a:rPr lang="en-GB" dirty="0"/>
               <a:t>Fifth level</a:t>
             </a:r>
-            <a:endParaRPr lang="en-US"/>
+            <a:endParaRPr lang="en-US" dirty="0"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
           <p:cNvPr id="4" name="Date Placeholder 3">
             <a:extLst>
@@ -172,15 +172,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout7.xml

##### ppt/slideLayouts/slideLayout7.xml

```diff
@@ -63,15 +63,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout12.xml

##### ppt/slideLayouts/slideLayout12.xml

```diff
@@ -131,15 +131,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideLayouts/slideLayout11.xml

##### ppt/slideLayouts/slideLayout11.xml

```diff
@@ -121,15 +121,15 @@
         <p:spPr/>
         <p:txBody>
           <a:bodyPr/>
           <a:lstStyle/>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
```

#### ppt/slideMasters/slideMaster1.xml

##### ppt/slideMasters/slideMaster1.xml

```diff
@@ -164,15 +164,15 @@
                 </a:solidFill>
               </a:defRPr>
             </a:lvl1pPr>
           </a:lstStyle>
           <a:p>
             <a:fld id="{3D09BA89-35E8-E347-826C-5826ACFF694D}" type="datetimeFigureOut">
               <a:rPr lang="en-US" smtClean="0"/>
-              <a:t>6/11/23</a:t>
+              <a:t>7/6/23</a:t>
             </a:fld>
             <a:endParaRPr lang="en-US"/>
           </a:p>
         </p:txBody>
       </p:sp>
       <p:sp>
         <p:nvSpPr>
@@ -267,15 +267,15 @@
     </p:spTree>
     <p:extLst>
       <p:ext uri="{BB962C8B-B14F-4D97-AF65-F5344CB8AC3E}">
         <p14:creationId xmlns:p14="http://schemas.microsoft.com/office/powerpoint/2010/main" val="3861594154"/>
       </p:ext>
     </p:extLst>
   </p:cSld>
-  <p:clrMap bg1="lt1" tx1="dk1" bg2="lt2" tx2="dk2" accent1="accent1" accent2="accent2" accent3="accent3" accent4="accent4" accent5="accent5" accent6="accent6" hlink="hlink" folHlink="folHlink"/>
+  <p:clrMap bg1="dk1" tx1="lt1" bg2="dk2" tx2="lt2" accent1="accent1" accent2="accent2" accent3="accent3" accent4="accent4" accent5="accent5" accent6="accent6" hlink="hlink" folHlink="folHlink"/>
   <p:sldLayoutIdLst>
     <p:sldLayoutId id="2147483649" r:id="rId1"/>
     <p:sldLayoutId id="2147483650" r:id="rId2"/>
     <p:sldLayoutId id="2147483660" r:id="rId3"/>
     <p:sldLayoutId id="2147483651" r:id="rId4"/>
     <p:sldLayoutId id="2147483652" r:id="rId5"/>
     <p:sldLayoutId id="2147483653" r:id="rId6"/>
```

#### docProps/thumbnail.jpeg

##### Image content

```diff
@@ -1,20 +1,20 @@
                                                             
-  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  .  . .  . 
-   .       .       .       .       .       .       .        
-     .  .    .  .    .  .    .  .    .  .    .  .    .  . . 
- .       .       .       .       .       .       .          
-   .  .    .  .    .  .    .  .    .  .    .  .    .  . .  .
-  .    .  .    .  .    .  .    .  .    .  .    .  .         
-    .       .       .       .       .       .       . .  .  
-  .   . .    .  .    .  .    .  .    .  .    .  .       .  .
-    .     .    .  .    .  .    .  .    .  .    .  . .       
-  .    .   .       .       .       .       .          .  .  
-     .   .   .  .    .  .    .  .    .  .    .  .  .   .   .
-  .    .      .   .   .   .   .   .   .   .   .   .  .   .  
-    .     . .   .   .   .   .   .   .   .   .   .           
-  .   .           .       .       .       .        .  . .  .
-    .   . .  . .     . .     . .     . .     . .  .         
-  .         .    .       .       .       .          . .  .  
-     . .  .    .   . .     . .     . .     . .  .       .  .
-  .          .         . .     . .     . .     .  . .       
-    .  . . .    . .  .     .       .       .          .  .  
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+                                                            
+
```

#### docProps/core.xml

##### docProps/core.xml

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <cp:coreProperties xmlns:cp="http://schemas.openxmlformats.org/package/2006/metadata/core-properties" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:dcmitype="http://purl.org/dc/dcmitype/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <dc:title>PowerPoint Presentation</dc:title>
   <dc:creator>Antonio Feregrino Bolanos</dc:creator>
   <cp:lastModifiedBy>Antonio Feregrino Bolanos</cp:lastModifiedBy>
-  <cp:revision>1</cp:revision>
+  <cp:revision>2</cp:revision>
   <dcterms:created xsi:type="dcterms:W3CDTF">2023-06-11T16:06:38Z</dcterms:created>
-  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-06-11T16:09:08Z</dcterms:modified>
+  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-07-06T15:57:40Z</dcterms:modified>
 </cp:coreProperties>
```

### Comparing `presentpy-0.5.0/src/presentpy/writers/pptx_writer.py` & `presentpy-0.8.0/src/presentpy/writers/pptx_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,18 +51,19 @@
 
     return token_colors
 
 
 class PptxWriter:
     TEMPLATE_CODE_SLIDE_INDEX = 2
 
-    def __init__(self, theme: str = "light"):
+    def __init__(self, configuration, theme: str = "light"):
         template = pkg_resources.resource_filename("presentpy", f"slide_templates/template-{theme}.pptx")
         self.presentation = Presentation(template)
         self.theme = get_theme(theme)
+        self.configuration = configuration
 
     def _write_code_slide(self, slide_title, parsed_tokens, lines_to_highlight):
         slide_layout = self.presentation.slide_layouts[PptxWriter.TEMPLATE_CODE_SLIDE_INDEX]
         slide = self.presentation.slides.add_slide(slide_layout)
 
         title = slide.shapes.title
         if slide_title:
@@ -77,19 +78,21 @@
         p.bullet = False
 
         for line_number, line_content in enumerate(parsed_tokens, 1):
             for kind, text in line_content:
                 run = p.add_run()
                 run.text = text
                 font = run.font
-                font.bold = line_number in lines_to_highlight
                 font.color.rgb = self.theme.get(kind, RGBColor(0, 0, 0))
-                font.size = Pt(14)
+                font.size = Pt(self.configuration.font_size)
+                if line_number in lines_to_highlight:
+                    font.size = Pt(self.configuration.highlight.font_size)
+                    font.bold = self.configuration.highlight.bold
             run = p.add_run()
-            run.font.size = Pt(14)
+            run.font.size = Pt(self.configuration.font_size)
             run.text = CARRIAGE_RETURN
 
     def write(self, code_slide_source: CodeSlideSource):
         parsed_lines = get_parsed_lines(code_slide_source.code)
 
         # We need to add this -1 so that there is AT LEAST ONE slide rendered
         # The -1 is because no line number will match, therefore the source code will be rendered without highlighting
```

### Comparing `presentpy-0.5.0/PKG-INFO` & `presentpy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: presentpy
-Version: 0.5.0
+Version: 0.8.0
 Summary: Create slides from Jupyter Notebooks
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

