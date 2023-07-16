# Comparing `tmp/lambdamoo_db-0.1.8.tar.gz` & `tmp/lambdamoo_db-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdamoo_db-0.1.8.tar", max compression
+gzip compressed data, was "lambdamoo_db-0.1.9.tar", max compression
```

## Comparing `lambdamoo_db-0.1.8.tar` & `lambdamoo_db-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      100 2023-01-30 05:46:32.188231 lambdamoo_db-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/__init__.py
--rw-r--r--   0        0        0      242 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/cli.py
--rw-r--r--   0        0        0     1769 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/database.py
--rw-r--r--   0        0        0     1701 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/enums.py
--rw-r--r--   0        0        0     2378 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/exporter.py
--rw-r--r--   0        0        0    18970 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/lambdamoo_db/reader.py
--rw-r--r--   0        0        0      548 2023-01-30 05:46:32.192231 lambdamoo_db-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 lambdamoo_db-0.1.8/setup.py
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 lambdamoo_db-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/cli.py
+-rw-r--r--   0        0        0     2427 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/database.py
+-rw-r--r--   0        0        0     1701 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/enums.py
+-rw-r--r--   0        0        0     2498 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/exporter.py
+-rw-r--r--   0        0        0    19590 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/reader.py
+-rw-r--r--   0        0        0      777 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/templates.py
+-rw-r--r--   0        0        0     5077 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/lambdamoo_db/writer.py
+-rw-r--r--   0        0        0      598 2023-06-24 04:23:50.945178 lambdamoo_db-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 lambdamoo_db-0.1.9/PKG-INFO
```

### Comparing `lambdamoo_db-0.1.8/lambdamoo_db/database.py` & `lambdamoo_db-0.1.9/lambdamoo_db/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from typing import Any
+from typing import Any, Generator
 import attrs
 
 
 class ObjNum(int):
     pass
 
 
+class Anon(int):
+    pass
+
+
 @attrs.define()
 class Verb:
     name: str
     owner: int
     perms: int
     preps: int
-
+    object: int
     code: list[str] = attrs.field(init=False, factory=list)
 
 
 @attrs.define()
 class Property:
     propertyName: str
     value: Any
@@ -27,18 +31,27 @@
 @attrs.define()
 class MooObject:
     id: int
     name: str
     flags: int
     owner: int
     location: int
-    parent: int
-
+    parents: list[int] = attrs.field(factory=list)
+    children: list[int] = attrs.field(init=False, factory=list)
+    last_move: int = attrs.field(init=False, default=-1)
+    contents: list[int] = attrs.field(init=False, factory=list)
     verbs: list[Verb] = attrs.field(init=False, factory=list)
     properties: list[Property] = attrs.field(init=False, factory=list)
+    anon: bool = attrs.field(default=False)
+
+    @property
+    def parent(self) -> int:
+        if len(self.parents) > 1:
+            raise Exception("Object has multiple parents")
+        return self.parents[0]
 
 
 @attrs.define()
 class Waif:
     waif_class: int
     owner: int
     props: list[Any]
@@ -67,39 +80,40 @@
 
 
 @attrs.define()
 class QueuedTask:
     firstLineno: int
     id: int
     st: int
-
     value: Any = attrs.field(init=False, default=None)
-
     activation: Activation | None = attrs.field(init=False)
     rtEnv: dict[str, Any] = attrs.field(init=False)
     code: list[str] = attrs.field(init=False, factory=list)
 
 
 @attrs.define()
 class SuspendedTask:
     firstLineno: int
     id: int
     st: int
-
     value: Any = attrs.field(init=False, default=None)
     vm: VM = attrs.field(init=False, default=None)
 
 
 @attrs.define(init=False)
 class MooDatabase:
     versionstring: str
     version: int
-
     total_objects: int
     total_verbs: int
     total_players: int
-
     players: list[int]
+    clocks: list
     objects: dict[int, MooObject]
     queuedTasks: list[QueuedTask]
     suspendedTasks: list[SuspendedTask]
     waifs: dict[int, Waif]
+
+    def all_verbs(self) -> Generator[Verb, None, None]:
+        for obj in self.objects.values():
+            for verb in obj.verbs:
+                yield verb
```

### Comparing `lambdamoo_db-0.1.8/lambdamoo_db/enums.py` & `lambdamoo_db-0.1.9/lambdamoo_db/enums.py`

 * *Files identical despite different names*

### Comparing `lambdamoo_db-0.1.8/lambdamoo_db/exporter.py` & `lambdamoo_db-0.1.9/lambdamoo_db/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,15 @@
     return name
 
 
 def to_json(db: MooDatabase) -> str:
     return json.dumps(cattrs.unstructure(db), indent=2, default=converter)
 
 
-def to_json_file(
-    db: MooDatabase, f: TextIOWrapper, indent: Optional[int] = None
-) -> None:
+def to_json_file(db: MooDatabase, f: TextIOWrapper, indent: Optional[int] = None) -> None:
     json.dump(cattrs.unstructure(db), f, indent=indent, default=converter)
 
 
 def to_moo_files(db: MooDatabase, path: str, corrify: bool) -> None:
     if os.path.exists(path):
         shutil.rmtree(path)
 
@@ -75,21 +73,26 @@
             id = names[i]
         return id
 
     for i, o in db.objects.items():
         id = name(i)
         os.mkdir(os.path.join(path, id))
         with open(os.path.join(path, id, "info.json"), "w") as f:
+
             info = {
                 "name": o.name,
-                "parent": name(o.parent),
+                "parent": None,
+                "parents": [name(p) for p in o.parents],
                 "owner": o.owner,
                 "location": o.location,
                 "verbs": [v.name for v in o.verbs],
             }
+            if len(o.parents) < 2:
+                info["parent"] = o.parent
+
             json.dump(info, f, indent=2)
         with open(os.path.join(path, id, "props.json"), "w") as f:
             json.dump(cattrs.unstructure(o.properties), f, indent=2, default=converter)
 
         for i, v in enumerate(o.verbs):
             filename = (sanitize(v.name) or str(i)).split(" ", 1)[0] + ".moo"
             with open(os.path.join(path, id, filename), "w") as f:
```

### Comparing `lambdamoo_db-0.1.8/lambdamoo_db/reader.py` & `lambdamoo_db-0.1.9/lambdamoo_db/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 from io import TextIOWrapper
 import re
-from typing import Any, NoReturn
-from lambdamoo_db.database import (
+import parse
+from typing import Any, NoReturn, Pattern
+from .database import (
     VM,
+    Anon,
     ObjNum,
     Waif,
     Activation,
     MooDatabase,
     MooObject,
     Property,
     QueuedTask,
     SuspendedTask,
     Verb,
     WaifReference,
 )
-from lambdamoo_db.enums import DBVersions, MooTypes
+from .enums import DBVersions, MooTypes
+from . import templates
 
 
 def load(filename: str) -> MooDatabase:
     with open(filename, "r", encoding="latin-1") as f:
         r = Reader(f, filename)
         return r.parse()
 
 
-versionRe = re.compile(r"\*\* LambdaMOO Database, Format Version (?P<version>\d+) \*\*")
-varCountRe = re.compile(r"(?P<count>\d+) variables")
-clockCountRe = re.compile(r"(?P<count>\d+) clocks")
-taskCountRe = re.compile(r"(?P<count>\d+) queued tasks")
-taskHeaderRe = re.compile(r"\d+ (\d+) (\d+) (\d+)")
-activationHeaderRe = re.compile(
-    r"-?(\d+) -?\d+ -?\d+ -?(\d+) -?\d+ -?(\d+) -?(\d+) -?\d+ -?(\d+)"
-)
-pendingValueRe = re.compile(r"(?P<count>\d+) values pending finalization")
-suspendedTaskCountRe = re.compile(r"(?P<count>\d+) suspended tasks")
-suspendedTaskHeaderRe = re.compile(
-    r"(?P<startTime>\d+) (?P<id>\d+)(?P<endchar>| (?P<value>\d+))$"
-)
-interruptedTaskCountRe = re.compile(r"(?P<count>\d+) interrupted tasks")
+def compile(template: str) -> Pattern[str]:
+    compiled = parse.compile(template)
+    if compiled._match_re is None:
+        raise Exception(f"Failed to compile template: {template}")
+    return compiled._match_re
+
+
+versionRe = compile(templates.version)
+varCountRe = compile(templates.var_count)
+clockCountRe = compile(templates.clock_count)
+taskCountRe = compile(templates.task_count)
+taskHeaderRe = compile(templates.task_header)
+activationHeaderRe = compile(templates.activation_header)
+pendingValueRe = compile(templates.pending_values_count)
+suspendedTaskCountRe = compile(templates.suspended_task_count)
+suspendedTaskHeaderRe = compile(templates.suspended_task_header)
+interruptedTaskCountRe = compile(templates.interrupted_task_count)
 interruptedTaskHeaderRe = re.compile(r"(?P<id>\d+) (?P<status>[\w\W]+)")
-vmHeaderRe = re.compile(
-    r"(?P<top>\d+) (?P<vector>-?\d+) (?P<funcId>\d+)(\n| (?P<maxStackframes>\d))"
-)
-connectionCountRe = re.compile(
-    r"(?P<count>\d+) active connections(?P<listener_tag>| with listeners)"
-)
-langverRe = re.compile(r"language version (?P<version>\d+)")
-stackheaderRe = re.compile(r"(?P<slots>\d+) rt_stack slots in use")
-
-pcRe = re.compile(r"(?P<pc>\d+) (?P<bi_func>\d+) (?P<error>\d+)")
-waifHeaderRe = re.compile(r"(?P<flag>[cr]) (?P<index>\d+)")
+vmHeaderRe = compile(templates.vm_header)
+connectionCountRe = re.compile(r"(?P<count>\d+) active connections(?P<listener_tag>| with listeners)")
+langverRe = compile(templates.langver)
+stackheaderRe = compile(templates.stack_header)
+pcRe = compile(templates.pc)
+waifHeaderRe = compile(templates.waif_header)
 
 
 class Reader:
     def __init__(self, fio: TextIOWrapper, filename: str = "") -> None:
         self.filename = filename
         self.file = fio
         self.line = 0
@@ -80,23 +81,23 @@
     def parse_v4(self, db: MooDatabase) -> None:
         db.total_objects = self.readInt()
         db.total_verbs = self.readInt()
         self.readString()  # dummy
         self.readPlayers(db)
         self.readObjects(db)
         self.readVerbs(db)
-        self.readClocks()
+        self.readClocks(db)
         self.readTaskQueue(db)
         self.readSuspendedTasks(db)
         self.readConnections()
 
     def parse_v17(self, db: MooDatabase) -> None:
         self.readPlayers(db)
         self.readPending(db)
-        self.readClocks()
+        self.readClocks(db)
         self.readTaskQueue(db)
         self.readSuspendedTasks(db)
         self.readInterruptedTasks(db)
         self.readConnections()
         db.total_objects = self.readInt()
         self.readObjects(db)
         if db.version >= DBVersions.DBV_Anon:
@@ -111,15 +112,15 @@
             val_type = self.readInt()
         match val_type:
             case MooTypes.STR:
                 return self.readString()
             case MooTypes.OBJ:
                 return self.readObjnum()
             case MooTypes.ANON:
-                return self.readAnon()
+                return self.readAnon(db)
             case MooTypes.INT:
                 return self.readInt()
             case MooTypes.FLOAT:
                 return self.readFloat()
             case MooTypes.ERR:
                 return self.readErr()
             case MooTypes.LIST:
@@ -217,15 +218,22 @@
         owner = self.readObjnum()
         location = self.readObjnum()
         firstContent = self.readInt()
         neighbor = self.readInt()
         parent = self.readObjnum()
         firstChild = self.readInt()
         sibling = self.readInt()
-        obj = MooObject(oid, name, flags, owner, location, parent)
+        obj = MooObject(
+            id=oid,
+            name=name,
+            flags=flags,
+            owner=owner,
+            location=location,
+            parents=[parent],
+        )
         numVerbs = self.readInt()
         for _ in range(numVerbs):
             self.readVerbMetadata(obj)
 
         self.readProperties(db, obj)
         return obj
 
@@ -243,23 +251,32 @@
         owner = self.readObjnum()
         location = self.readValue(db)
         if db.version >= DBVersions.DBV_Last_Move:
             last_move = self.readValue(db)
 
         contents = self.readValue(db)
         parents = self.readValue(db)
+        if not isinstance(parents, list):
+            parents = [parents]
         children = self.readValue(db)
         obj = MooObject(oid, name, flags, owner, location, parents)
         numVerbs = self.readInt()
         for _ in range(numVerbs):
             self.readVerbMetadata(obj)
 
         self.readProperties(db, obj)
         return obj
 
+    def readAnon(self, db: MooDatabase) -> None:
+        oid = self.readInt()
+        if oid == -1:
+            self.parse_error("Not sure what to do with a -1 anon yet")
+        else:
+            return Anon(oid)
+
     def readConnections(self) -> None:
         header = self.readString()
         headerMatch = connectionCountRe.match(header)
         if not headerMatch:
             self.parse_error("Bad active connections header line")
 
         count = int(headerMatch.group("count"))
@@ -284,14 +301,15 @@
         if not obj:
             self.parse_error(f"object {objNumber} not found")
 
         verb = obj.verbs[verbNumber]
         if not verb:
             self.parse_error(f"verb ${verbNumber} not found on object ${objNumber}")
 
+        verb.object = objNumber
         verb.code = code
 
     def readCode(self) -> list[str]:
         code = []
         lastLine = self.readString()
         while lastLine != ".":
             code.append(lastLine)
@@ -304,15 +322,17 @@
         for _ in range(db.total_players):
             db.players.append(self.readObjnum())
         assert db.total_players == len(db.players)
 
     def readAnonObjects(self, db: MooDatabase) -> None:
         num_anon = self.readInt()
         if num_anon > 0:
-            self.parse_error("Anonymous Objects not implemented yet")
+            obj = self.readObject_ng(db)
+            obj.anon = True
+            db.objects[obj.id] = obj
 
     def readObjects(self, db: MooDatabase) -> None:
         db.objects = {}
         for _ in range(db.total_objects):
             if db.version == 4:
                 obj = self.readObject_v4(db)
             else:
@@ -323,31 +343,37 @@
         for o in db.objects.values():
             self.process_propnames(db, o)
 
     def process_propnames(self, db: MooDatabase, obj: MooObject) -> None:
         names = []
         parent = obj
         while parent is not None:
-            names.extend(
-                p.propertyName for p in parent.properties if p.propertyName is not None
-            )
+            names.extend(p.propertyName for p in parent.properties if p.propertyName is not None)
+            if len(parent.parents) > 1:
+                # todo: Identify order of multi-inheritence
+                break
             parent = db.objects.get(parent.parent)
+        i = 1
         for p in obj.properties:
-            n = names.pop(0)
+            try:
+                n = names.pop(0)
+            except IndexError:
+                n = i
             if not p.propertyName:
                 p.propertyName = n
             elif n != p.propertyName:
                 self.parse_error(f"property name mismatch: {n} != {p.propertyName}")
+            i += 1
 
     def readVerbMetadata(self, obj: MooObject) -> None:
         name = self.readString()
         owner = self.readObjnum()
         perms = self.readInt()
         preps = self.readInt()
-        verb = Verb(name, owner, perms, preps)
+        verb = Verb(name, owner, perms, preps, -1)
         obj.verbs.append(verb)
 
     def readProperties(self, db: MooDatabase, obj: MooObject):
         numProperties = self.readInt()
         propertyNames = []
         for _ in range(numProperties):
             propertyNames.append(self.readString())
@@ -368,26 +394,27 @@
         if not valueMatch:
             self.parse_error("Bad pending finalizations")
 
         finalizationCount = int(valueMatch.group("count"))
         for _ in range(finalizationCount):
             self.readValue(db)
 
-    def readClocks(self) -> None:
+    def readClocks(self, db: MooDatabase) -> None:
         clockLine = self.readString()
         clockMatch = clockCountRe.match(clockLine)
         if not clockMatch:
             self.parse_error("Could not find clock definitions")
+        db.clocks = []
         numClocks = int(clockMatch.group("count"))
         for _ in range(numClocks):
-            self.readClock()
+            self.readClock(db)
 
-    def readClock(self) -> None:
+    def readClock(self, db: MooDatabase) -> None:
         """Obsolete"""
-        self.readString()
+        db.clocks.append(self.readString())
 
     def readTaskQueue(self, db: MooDatabase) -> None:
         queuedTasksLine = self.readString()
         queuedTasksMatch = taskCountRe.match(queuedTasksLine)
         if not queuedTasksMatch:
             self.parse_error("Could not find task queue")
 
@@ -496,17 +523,15 @@
         headerLine = self.readString()
         taskMatch = suspendedTaskHeaderRe.match(headerLine)
         if not taskMatch:
             self.parse_error(f"Bad suspended task header: {headerLine}")
 
         id = int(taskMatch.group("id"))
         startTime = int(taskMatch.group("startTime"))
-        task = SuspendedTask(
-            0, id, startTime
-        )  # Set line number to 0 for a suspended task since we don't know it (only opcodes, not text)
+        task = SuspendedTask(0, id, startTime)  # Set line number to 0 for a suspended task since we don't know it (only opcodes, not text)
         if val := taskMatch.group("value"):
             task.value = self.readValue(db, known_type=int(val))
         task.vm = self.readVM(db)
         db.suspendedTasks.append(task)
 
     def readInterruptedTasks(self, db: MooDatabase):
         valueLine = self.readString()
```

### Comparing `lambdamoo_db-0.1.8/pyproject.toml` & `lambdamoo_db-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [tool.poetry]
 name = "lambdamoo-db"
-version = "0.1.8"
+version = "0.1.9"
 description = "Parser for LambdaMOO databases"
 authors = ["Katelyn Gigante <clockwork.singularity@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lambdamoo_db"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 attrs = "^22.2.0"
 cattrs = "^22.2.0"
 click = "^8.1.3"
+parse = "^1.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 moodb2flat = "lambdamoo_db.cli:moodb2flat"
+
+[tool.black]
+line-length = 160
```

### Comparing `lambdamoo_db-0.1.8/PKG-INFO` & `lambdamoo_db-0.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lambdamoo-db
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parser for LambdaMOO databases
 License: MIT
 Author: Katelyn Gigante
 Author-email: clockwork.singularity@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: parse (>=1.19.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # LambdaMOO database reader and exporter
 
 Fill me in!
 
 ## cli commands
```

