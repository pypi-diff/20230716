# Comparing `tmp/poslq_simple-0.1.2.tar.gz` & `tmp/poslq_simple-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poslq_simple-0.1.2.tar", last modified: Wed Jul 12 20:29:10 2023, max compression
+gzip compressed data, was "poslq_simple-0.1.3.tar", last modified: Sun Jul 16 19:26:35 2023, max compression
```

## Comparing `poslq_simple-0.1.2.tar` & `poslq_simple-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.569218 poslq_simple-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3302 2023-07-12 20:29:10.568218 poslq_simple-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2778 2023-07-12 18:48:23.000000 poslq_simple-0.1.2/README.md
--rw-rw-rw-   0        0        0      611 2023-07-12 20:27:46.000000 poslq_simple-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 20:29:10.569218 poslq_simple-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.554550 poslq_simple-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.565143 poslq_simple-0.1.2/src/poslq_simple.egg-info/
--rw-rw-rw-   0        0        0     3302 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 20:29:10.000000 poslq_simple-0.1.2/src/poslq_simple.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 20:29:10.567216 poslq_simple-0.1.2/src/posql_simple/
--rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.2/src/posql_simple/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-07-12 18:19:47.000000 poslq_simple-0.1.2/src/posql_simple/cypher.py
--rw-rw-rw-   0        0        0     5954 2023-07-12 20:19:04.000000 poslq_simple-0.1.2/src/posql_simple/w_out_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.064342 poslq_simple-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3399 2023-07-16 19:26:35.064342 poslq_simple-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2875 2023-07-16 19:23:58.000000 poslq_simple-0.1.3/README.md
+-rw-rw-rw-   0        0        0      611 2023-07-16 19:25:58.000000 poslq_simple-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 19:26:35.065345 poslq_simple-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.036795 poslq_simple-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.061831 poslq_simple-0.1.3/src/poslq_simple.egg-info/
+-rw-rw-rw-   0        0        0     3399 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 19:26:35.000000 poslq_simple-0.1.3/src/poslq_simple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 19:26:35.063336 poslq_simple-0.1.3/src/posql_simple/
+-rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.3/src/posql_simple/__init__.py
+-rw-rw-rw-   0        0        0     5339 2023-07-16 19:22:32.000000 poslq_simple-0.1.3/src/posql_simple/w_out_sql.py
```

### Comparing `poslq_simple-0.1.2/LICENSE` & `poslq_simple-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.2/PKG-INFO` & `poslq_simple-0.1.3/src/poslq_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: poslq_simple
-Version: 0.1.2
+Name: poslq-simple
+Version: 0.1.3
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # project
 
+Looking for contributions.
+
 ## What ?
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
@@ -48,14 +50,15 @@
 
 ``load`` returns a Database object. The arguments are path ( the path of the file ) and the decrypt_pass.
 Throws FileNotFoundError err if the file doesn't exist and ( or ) InvalidFileExtensionError ( if the file extension doesn't match  the .pst ).
 
 ``bind_new_collection`` binds the collection to the database object ( for data persistence ). Takes a collection as Param.
 
 ``get_collection`` returns a collection object. Args : coll_name ( name of the collection ).
+``get_collections`` returns a dict with all the collections. 
 
 ## Collection
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
@@ -71,8 +74,8 @@
 returning a bool.
 
 ``search_by`` : takes two positional args : slot_name which is the name of the entry you want ( for instance the "name" entry of,
 each dict ) and the slot_value. Returns None if not found.
 
 ``get_all_slot`` : returns a list of all the entries.
 
-**this lib supports multithreading env by using synchronization.**
+**this lib supports multithreading queries by using synchronization.**
```

### Comparing `poslq_simple-0.1.2/README.md` & `poslq_simple-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # project
 
+Looking for contributions.
+
 ## What ?
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
@@ -34,14 +36,15 @@
 
 ``load`` returns a Database object. The arguments are path ( the path of the file ) and the decrypt_pass.
 Throws FileNotFoundError err if the file doesn't exist and ( or ) InvalidFileExtensionError ( if the file extension doesn't match  the .pst ).
 
 ``bind_new_collection`` binds the collection to the database object ( for data persistence ). Takes a collection as Param.
 
 ``get_collection`` returns a collection object. Args : coll_name ( name of the collection ).
+``get_collections`` returns a dict with all the collections. 
 
 ## Collection
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
@@ -57,8 +60,8 @@
 returning a bool.
 
 ``search_by`` : takes two positional args : slot_name which is the name of the entry you want ( for instance the "name" entry of,
 each dict ) and the slot_value. Returns None if not found.
 
 ``get_all_slot`` : returns a list of all the entries.
 
-**this lib supports multithreading env by using synchronization.**
+**this lib supports multithreading queries by using synchronization.**
```

### Comparing `poslq_simple-0.1.2/pyproject.toml` & `poslq_simple-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "poslq_simple"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="enyos", email="lebedevhh@outlook.fr" },
 ]
 description = "A simple nosql json storage for small projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `poslq_simple-0.1.2/src/poslq_simple.egg-info/PKG-INFO` & `poslq_simple-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: poslq-simple
-Version: 0.1.2
+Name: poslq_simple
+Version: 0.1.3
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # project
 
+Looking for contributions.
+
 ## What ?
 really simple no-sql database ( for small projects ) using json.
 
 ## Documentation
 read the docs.md file.
 
 ## Quickstart ( simple example )
@@ -48,14 +50,15 @@
 
 ``load`` returns a Database object. The arguments are path ( the path of the file ) and the decrypt_pass.
 Throws FileNotFoundError err if the file doesn't exist and ( or ) InvalidFileExtensionError ( if the file extension doesn't match  the .pst ).
 
 ``bind_new_collection`` binds the collection to the database object ( for data persistence ). Takes a collection as Param.
 
 ``get_collection`` returns a collection object. Args : coll_name ( name of the collection ).
+``get_collections`` returns a dict with all the collections. 
 
 ## Collection
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
@@ -71,8 +74,8 @@
 returning a bool.
 
 ``search_by`` : takes two positional args : slot_name which is the name of the entry you want ( for instance the "name" entry of,
 each dict ) and the slot_value. Returns None if not found.
 
 ``get_all_slot`` : returns a list of all the entries.
 
-**this lib supports multithreading env by using synchronization.**
+**this lib supports multithreading queries by using synchronization.**
```

### Comparing `poslq_simple-0.1.2/src/posql_simple/w_out_sql.py` & `poslq_simple-0.1.3/src/posql_simple/w_out_sql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,54 @@
 import json
 import threading
 import time
 import uuid
-from os.path import exists, basename
+from os.path import exists, isfile, isfile
 import os
-from cypher import gen_cipher_file, gen_decypher_file
 from pathlib import Path
 
 LOCK = threading.Lock()
 
 # custom error class
 class InvalidFileExtensionError( Exception ):
     "File extension must be .pst"
     pass
 
 class Database:
     # for ezz mig \ you can pass directly the data
     # need to input the password ( for decrypting the file )
-    def __init__(self, __pass : str, __data : dict = {}, path : str = "./default.pst"):
+    def __init__(self, __data : dict = {}, path : str = "./default.pst"):
         self.__data=__data # this holds all the collections
-        self.__pass = __pass # this is the encrypt pass 
-        print ("[INFO] make sure to remember the pass to decrypt the file...")
         self.path = path
-    
+        print ( "thanks for using this library..." )
+          
     # persisting the collect obj 
     # Want to debug ( the message on the console ) -> YES ( leave the debug param to true ) : NO  -> ( make false ) 
     def save(self, debug : bool = True ):
         # try and catch ? 
         obj_serialized = json.dumps( self.__data )
         # issue : always on save we write the whole object ( maybe implement some cache ? )
         with open(self.path , "w") as y:
-            y.write(obj_serialized) # transforms the __data props into a string
+            y.write(obj_serialized)
             length_byte_written = len( obj_serialized ) * 8
             log_message = "data saved on file {fname} [written : {data_length} bytes ]".format(fname=self.path, data_length=length_byte_written)
             if (debug):
                 print (log_message )
             y.close()
 
-        # this is not good ... ( reopening files to much times )        
-        # obviously our lib doesn't take into account synchronized request
-        # maybe create a lock for synchronizing those parallel request...
-
-    # private method ( with the two underscores )
-    @staticmethod
-    def __parse_file_content( filename : str ):
-        with open(filename , "r") as y:
-            str__ = '\n'.join(y.readlines()) # the readlines mehtod returns an array ( so you must polish it first )
-            __data = json.loads( str__ )
-            y.close()
-            return __data
-
     # throws an exception
     @staticmethod
-    def load(path : str, decrypt_pass : str ) :
+    def load(path : str) :
         # we need to check if the file is encrypted ( if yes, then decrypt )
         if (exists( path ) ):
             if path[-4:] == ".pst":
-                __data = parse_file_content( path )
-                return Database(__data , path)
+                with open ( path, "r") as file : 
+                    data = file.readlines()
+                    data = json.loads( data )
+                    return Database(__data = data, path = path )
             else :
                 raise InvalidFileExtensionError
         else:
             raise FileNotFoundError("file {fname} doesn't exist".format( fname = path))
 
     def __repr__( self ):
         return "path : {path_name}, collections : {coll}".format( path_name = self.path, coll = self.__data )
@@ -70,31 +57,35 @@
         self.__data[collection.collect_name] = collection._get_all_slot()
         self.save(debug = False)
 
     def get_collection(self, coll_name : str ):
         if ( col_name in list(self.__data.keys())):
             return Collection( coll_name, self.__data[coll_name])
         else :
+            print ( "[INFO] this is collection doesn't exist")
             print ( "[INFO] created new collection into {db_name}, with name {coll_name}".format(db_name = self.path, coll_name = coll_name))
             result = Collection( coll_name )
             self.bind_new_collection( result )
             return result
+            
+    def get_all_collections(self) -> dict :
+        return self.__data
 
 class Collection:
     def __init__(self, collect_name : str , __container_documents : list = []):
         self.collect_name=collect_name
         self.__container_documents = __container_documents# empty list to stores one all the documents
     
     def add_record(self, record : dict ) -> bool :
         # we need to check / if it has the _id prop
         lock.acquire()
         try : 
             add_thing = record.copy()
             if not ("_id" in list(add_thing.keys())):
-                add_thing['_id'] = generate_random_id()            
+                add_thing['_id'] = Cypher.generate_random_id()            
             self.__container_documents.append(add_thing)
             lock.release() 
             return True 
         except:
             lock.release() 
             return False 
             
@@ -148,11 +139,8 @@
         for  slot in self.__container_documents :
             if ( slot[slot_name] == slot_value ):
                 return slot.copy() 
         return None
 
     # getter
     def _get_all_slot(self):
-        return self.__container_documents
-
-def generate_random_id():
-    return str(uuid.uuid4().fields[-1])[:5]
+        return self.__container_documents
```

