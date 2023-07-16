# Comparing `tmp/somtodaypython-0.0.3.tar.gz` & `tmp/somtodaypython-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somtodaypython-0.0.3.tar", last modified: Sun Mar 19 14:15:27 2023, max compression
+gzip compressed data, was "somtodaypython-0.0.4.tar", last modified: Sun Jul 16 10:24:33 2023, max compression
```

## Comparing `somtodaypython-0.0.3.tar` & `somtodaypython-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-19 14:15:27.527488 somtodaypython-0.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     3590 2023-03-19 14:15:27.527488 somtodaypython-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3295 2023-03-19 14:09:53.000000 somtodaypython-0.0.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-03-19 14:15:27.527488 somtodaypython-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      746 2023-03-19 14:13:13.000000 somtodaypython-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-19 14:15:27.523488 somtodaypython-0.0.3/somtodaypython/
--rw-r--r--   0 runner    (1000) runner    (1000)      122 2023-03-19 14:09:53.000000 somtodaypython-0.0.3/somtodaypython/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17232 2023-03-19 14:09:53.000000 somtodaypython-0.0.3/somtodaypython/asynchronous_somtoday.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17856 2023-03-19 14:09:53.000000 somtodaypython-0.0.3/somtodaypython/nonasyncsomtoday.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-19 14:15:27.527488 somtodaypython-0.0.3/somtodaypython.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3590 2023-03-19 14:15:27.000000 somtodaypython-0.0.3/somtodaypython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      319 2023-03-19 14:15:27.000000 somtodaypython-0.0.3/somtodaypython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-19 14:15:27.000000 somtodaypython-0.0.3/somtodaypython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2023-03-19 14:15:27.000000 somtodaypython-0.0.3/somtodaypython.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2023-03-19 14:15:27.000000 somtodaypython-0.0.3/somtodaypython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 10:24:33.794596 somtodaypython-0.0.4/
+-rw-rw-rw-   0        0        0     4346 2023-07-16 10:24:33.793595 somtodaypython-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2023-07-13 20:24:28.000000 somtodaypython-0.0.4/README.md
+-rw-rw-rw-   0        0        0      369 2023-07-16 10:18:05.000000 somtodaypython-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:24:33.794596 somtodaypython-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-07-16 10:16:46.000000 somtodaypython-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:24:33.771656 somtodaypython-0.0.4/somtodaypython/
+-rw-rw-rw-   0        0        0      127 2023-07-09 16:34:09.000000 somtodaypython-0.0.4/somtodaypython/__init__.py
+-rw-rw-rw-   0        0        0    18271 2023-07-13 20:24:28.000000 somtodaypython-0.0.4/somtodaypython/asynchronous_somtoday.py
+-rw-rw-rw-   0        0        0    20387 2023-07-13 20:24:28.000000 somtodaypython-0.0.4/somtodaypython/nonasyncsomtoday.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:24:33.789598 somtodaypython-0.0.4/somtodaypython.egg-info/
+-rw-rw-rw-   0        0        0     4346 2023-07-16 10:24:33.000000 somtodaypython-0.0.4/somtodaypython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-16 10:24:33.000000 somtodaypython-0.0.4/somtodaypython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:24:33.000000 somtodaypython-0.0.4/somtodaypython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 10:24:33.000000 somtodaypython-0.0.4/somtodaypython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 10:24:33.000000 somtodaypython-0.0.4/somtodaypython.egg-info/top_level.txt
```

### Comparing `somtodaypython-0.0.3/PKG-INFO` & `somtodaypython-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-Metadata-Version: 2.1
-Name: somtodaypython
-Version: 0.0.3
-Summary: Python package for interacting & fetching somtoday's data.
-Home-page: https://github.com/luxkatana/somtodayapi_python
-Author: luxkatana/TheTrojanHorse
-Author-email: taseen.bibi@gmail.com
-Description-Content-Type: text/markdown
-
-***Somtoday Python, the interactor***
-
-***changes in 0.0.3***
-<ul>
-<li>added PasFoto feature to get the PasFoto/Photo of the student.</li>
-<li>added new attribute: student.identifier for student's account's ID</li>
-<li>old student.identifier has been moved to student.leerlingnummer </li>
-</ul>
-
-
-> What the f**ck is this?
-
-this(somtoday python) is a package that fetches and interacts with somtoday API using https requests.
-
-**installation**
-
-*for macos & linux*
-```
-python3 -m pip3 install somtodaypython 
-```
-*for windows*
-```
-python3 -m pip install somtodaypython 
-```
-OR
-```
-python -m pip install somtodaypython
-```
-
-if neither above works then you can always do this
-```
-pip3 install git+https://github.com/luxkatana/somtodayapi_python
-```
-***examples***
-
-*basic interacting with a student(getting data from the student)*
-```py
-
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
-```
-*basic interacting with the timetable of a student*
-```py
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-from datetime import timedelta, datetime as dt
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-today = dt.now()
-tomorrow = today + timedelta(days=2)
-timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
-for day in timetable:
-    for day_subject in day:
-        print(day_subect.subject_name)
-```
-
-**Asynchronous suppport**
-
-We also support asynchronous for somtodaypython.
-
-*Basic interacting with a student(asynchronous)*
-```py
-import somtodaypython.asynchronous_somtoday as async_somtoday
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    print(student.full_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-*Basic interacting with a student's timetable(asynchronous)*
-
-```py
-
-import somtodaypython.asynchronous_somtoday as async_somtoday
-from datetime import timedelta,datetime as dt
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    now = dt.now()
-    tomorrow = now + timedelta(days=2)
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
-    for day in timetable:
-        for  subject in day:
-            print(subject.subject_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-
-**Ending**
-
-
-New features are always welcome! email taseen.bibi@gmail.com
-
-
-**Huizengek#6623**
-Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
-
-github: https://github.com/25huizengek1
-
-
-**elisaado**
-
-Special thanks to **elisaado** for making important API endpoints visible to other users.
-
-github: https://github.com/elisaado/somtoday-api-docs
+***Somtoday Python, the interactor***
+
+***changes in 0.0.4***
+<ul>
+<li> I got more lazier so I wanted to announce this in Dutch </li>
+<li> Gefixt dat Student.fetch_schedule(group_by_day=True) dat het weer werkt(zat blijkbaar een bug in) </li>
+<li> Documentatie verbetert </li>
+<li> Er zat een probleem met Union types, gefixt </li>
+<li> Je kan 2 studenten vergelijken als Student.full_name en Student.school_name allebei gelijk zijn
+<li> Vergelijkingen met Cijfers(kijken als cijfers zijn hoger of lager) Cijfers worden bepaald door Cijfers.resultaat
+<li>beter __repr__ en __str__ voor Cijfer en Subject</li>
+<li>Cijfers resultaat yielden is mogelijk door Student.yield_fetch_cijfers() te doen (ook met asynchronous)</li>
+<li>Rooster vakken yielden is mogelijk door Student.yield_fetch_schedule() te doen (ook met asynchronous)</li>
+</ul>
+
+
+somtodaypython is a package that fetches and interacts with Somtoday API using https requests.
+
+**installation**
+
+*for macos & linux*
+```
+python3 -m pip3 install somtodaypython 
+```
+*for windows*
+```
+python3 -m pip install somtodaypython 
+```
+OR
+```
+python -m pip install somtodaypython
+```
+
+if neither above works then you can always do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python
+```
+
+If you want to try beta versions do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python/dev
+```
+***examples***
+
+*basic interacting with a student(getting data from the student)*
+```py
+
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
+```
+*basic interacting with the timetable of a student*
+```py
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+from datetime import timedelta, datetime as dt
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+today = dt.now()
+tomorrow = today + timedelta(days=2)
+timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
+for day in timetable:
+    for day_subject in day:
+        print(day_subject.subject_name)
+```
+
+**Asynchronous support**
+
+We also support asynchronous for somtodaypython.
+
+*Basic interacting with a student(asynchronous)*
+```py
+import somtodaypython.asynchronous_somtoday as async_somtoday
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    print(student.full_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+*Basic interacting with a student's timetable(asynchronous)*
+
+```py
+
+import somtodaypython.asynchronous_somtoday as async_somtoday
+from datetime import timedelta,datetime as dt
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    now = dt.now()
+    tomorrow = now + timedelta(days=2)
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
+    for day in timetable:
+        for  subject in day:
+            print(subject.subject_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+
+**Ending**
+
+
+New features are always welcome! email taseen.bibi@gmail.com
+
+
+**Huizengek#6623**
+Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
+
+github: https://github.com/25huizengek1
+
+
+**elisaado**
+
+Special thanks to **elisaado** for making important API endpoints visible to other users.
+
+github: https://github.com/elisaado/somtoday-api-docs
```

### Comparing `somtodaypython-0.0.3/README.md` & `somtodaypython-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,127 @@
-***Somtoday Python, the interactor***
-
-***changes in 0.0.3***
-<ul>
-<li>added PasFoto feature to get the PasFoto/Photo of the student.</li>
-<li>added new attribute: student.identifier for student's account's ID</li>
-<li>old student.identifier has been moved to student.leerlingnummer </li>
-</ul>
-
-
-> What the f**ck is this?
-
-this(somtoday python) is a package that fetches and interacts with somtoday API using https requests.
-
-**installation**
-
-*for macos & linux*
-```
-python3 -m pip3 install somtodaypython 
-```
-*for windows*
-```
-python3 -m pip install somtodaypython 
-```
-OR
-```
-python -m pip install somtodaypython
-```
-
-if neither above works then you can always do this
-```
-pip3 install git+https://github.com/luxkatana/somtodayapi_python
-```
-***examples***
-
-*basic interacting with a student(getting data from the student)*
-```py
-
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
-```
-*basic interacting with the timetable of a student*
-```py
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-from datetime import timedelta, datetime as dt
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-today = dt.now()
-tomorrow = today + timedelta(days=2)
-timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
-for day in timetable:
-    for day_subject in day:
-        print(day_subect.subject_name)
-```
-
-**Asynchronous suppport**
-
-We also support asynchronous for somtodaypython.
-
-*Basic interacting with a student(asynchronous)*
-```py
-import somtodaypython.asynchronous_somtoday as async_somtoday
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    print(student.full_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-*Basic interacting with a student's timetable(asynchronous)*
-
-```py
-
-import somtodaypython.asynchronous_somtoday as async_somtoday
-from datetime import timedelta,datetime as dt
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    now = dt.now()
-    tomorrow = now + timedelta(days=2)
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
-    for day in timetable:
-        for  subject in day:
-            print(subject.subject_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-
-**Ending**
-
-
-New features are always welcome! email taseen.bibi@gmail.com
-
-
-**Huizengek#6623**
-Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
-
-github: https://github.com/25huizengek1
-
-
-**elisaado**
-
-Special thanks to **elisaado** for making important API endpoints visible to other users.
-
-github: https://github.com/elisaado/somtoday-api-docs
+Metadata-Version: 2.1
+Name: somtodaypython
+Version: 0.0.4
+Summary: Python package for interacting & fetching somtoday's data.
+Home-page: https://github.com/luxkatana/somtodayapi_python
+Author: luxkatana/TheTrojanHorse
+Author-email: taseen.bibi@gmail.com
+Description-Content-Type: text/markdown
+
+***Somtoday Python, the interactor***
+
+***changes in 0.0.4***
+<ul>
+<li> I got more lazier so I wanted to announce this in Dutch </li>
+<li> Gefixt dat Student.fetch_schedule(group_by_day=True) dat het weer werkt(zat blijkbaar een bug in) </li>
+<li> Documentatie verbetert </li>
+<li> Er zat een probleem met Union types, gefixt </li>
+<li> Je kan 2 studenten vergelijken als Student.full_name en Student.school_name allebei gelijk zijn
+<li> Vergelijkingen met Cijfers(kijken als cijfers zijn hoger of lager) Cijfers worden bepaald door Cijfers.resultaat
+<li>beter __repr__ en __str__ voor Cijfer en Subject</li>
+<li>Cijfers resultaat yielden is mogelijk door Student.yield_fetch_cijfers() te doen (ook met asynchronous)</li>
+<li>Rooster vakken yielden is mogelijk door Student.yield_fetch_schedule() te doen (ook met asynchronous)</li>
+</ul>
+
+
+somtodaypython is a package that fetches and interacts with Somtoday API using https requests.
+
+**installation**
+
+*for macos & linux*
+```
+python3 -m pip3 install somtodaypython 
+```
+*for windows*
+```
+python3 -m pip install somtodaypython 
+```
+OR
+```
+python -m pip install somtodaypython
+```
+
+if neither above works then you can always do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python
+```
+
+If you want to try beta versions do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python/dev
+```
+***examples***
+
+*basic interacting with a student(getting data from the student)*
+```py
+
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
+```
+*basic interacting with the timetable of a student*
+```py
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+from datetime import timedelta, datetime as dt
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+today = dt.now()
+tomorrow = today + timedelta(days=2)
+timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
+for day in timetable:
+    for day_subject in day:
+        print(day_subject.subject_name)
+```
+
+**Asynchronous support**
+
+We also support asynchronous for somtodaypython.
+
+*Basic interacting with a student(asynchronous)*
+```py
+import somtodaypython.asynchronous_somtoday as async_somtoday
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    print(student.full_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+*Basic interacting with a student's timetable(asynchronous)*
+
+```py
+
+import somtodaypython.asynchronous_somtoday as async_somtoday
+from datetime import timedelta,datetime as dt
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    now = dt.now()
+    tomorrow = now + timedelta(days=2)
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
+    for day in timetable:
+        for  subject in day:
+            print(subject.subject_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+
+**Ending**
+
+
+New features are always welcome! email taseen.bibi@gmail.com
+
+
+**Huizengek#6623**
+Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
+
+github: https://github.com/25huizengek1
+
+
+**elisaado**
+
+Special thanks to **elisaado** for making important API endpoints visible to other users.
+
+github: https://github.com/elisaado/somtoday-api-docs
```

### Comparing `somtodaypython-0.0.3/setup.py` & `somtodaypython-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-'''
-setup.py for installing this package do python3 setup.py install.
-'''
-from setuptools import setup, find_packages
-
-VERSION = '0.0.3'
-DESCRIPTION = 'Python package for interacting & fetching somtoday\'s data.'
-
-with open("./README.md", "r", encoding="utf-8")as file:
-    data = file.read()
-setup(
-        name="somtodaypython",
-        version=VERSION,
-        long_description_content_type="text/markdown",
-        long_description=data,
-        author="luxkatana/TheTrojanHorse",
-        author_email="taseen.bibi@gmail.com",
-        description=DESCRIPTION,
-        packages=find_packages(),
-        install_requires=["requests", "httpx"], # add any additional packages that
-        url="https://github.com/luxkatana/somtodayapi_python",
-)
+'''
+setup.py for installing this package do python3 setup.py install.
+'''
+from setuptools import setup, find_packages
+
+VERSION = '0.0.4'
+DESCRIPTION = 'Python package for interacting & fetching somtoday\'s data.'
+
+with open("./README.md", "r", encoding="utf-8")as file:
+    data = file.read()
+setup(
+        name="somtodaypython",
+        version=VERSION,
+        long_description_content_type="text/markdown",
+        long_description=data,
+        author="luxkatana/TheTrojanHorse",
+        author_email="taseen.bibi@gmail.com",
+        description=DESCRIPTION,
+        packages=find_packages(),
+        install_requires=["requests", "httpx"], # add any additional packages that
+        url="https://github.com/luxkatana/somtodayapi_python",
+)
```

### Comparing `somtodaypython-0.0.3/somtodaypython/nonasyncsomtoday.py` & `somtodaypython-0.0.4/somtodaypython/asynchronous_somtoday.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,433 +1,412 @@
-'''
-Module that provide non-asynchronous functions for using the somtoday API
-
-'''
-import base64
-from typing import Any
-from pathlib import Path
-from datetime import datetime
-import hashlib
-import os
-import random
-import string
-from urllib.parse import urlparse, parse_qs
-import requests
-class PasFoto:
-    def __init__(self, b64url: str) -> None:
-        self.base64url: bytes = b64url[21::].encode()
-    def save(self,  save_to: Path) -> bool | Exception:
-        """save the PasFoto as file
-
-        Args:
-            save_to (Path): file where it should save the PasFoto
-
-        Returns:
-            bool | Exception: returns True if everything was gone successfully otherwise it'll return an Exception when an error occurs
-        """        
-        try:
-            with open(save_to, "wb")as f:
-                f.write(base64.decodebytes(self.base64url))
-                return True
-        except Exception as e:
-            return e
-class Cijfer:
-    def __init__(self, **kwargs) -> None:
-        self.vak: str = kwargs.get("vak")
-        self.datum_invoer: datetime = kwargs.get("datum")
-        self.leerjaar: int = kwargs.get("leerjaar")
-        self.resultaat: str = kwargs.get("resultaat")
-class Subject:
-    '''
-    Subject:
-    a model what represents a single school subject/hour from timetable
-    THIS IS NOT MEANT TO BE CREATED BY THE USER
-    '''
-
-    def __init__(self, **kwargs: dict[str, Any]) -> None:
-        self.subject_name: str = kwargs.get("subject")
-        self.begin_time: datetime = kwargs.get("begindt")
-        self.end_time: datetime = kwargs.get("enddt")
-        self.subject_short: str = kwargs.get("subject_short")
-        self.begin_hour: int = kwargs.get("beginhour")
-        self.end_hour:  int = kwargs.get("endhour")
-        self.location: str = kwargs.get("location")
-        self.teacher_short: str = kwargs.get("teacher_shortcut")
-
-    def __repr__(self):
-        return f"{self.subject_name}"
-
-    def __str__(self):
-        return self.__repr__()
-
-
-class Student:
-    '''
-    Student:
-        Model that represents a Student
-        THIS IS NOT MEANT TO BE CREATED BY THE USER
-    '''
-    def __init__(self, **kwargs) -> None:
-        self.name: str = kwargs.get("name")
-        self.password: str = kwargs.get("password")
-        self.school_uuid: str = kwargs.get("uuid")
-        self.school_name: str = kwargs.get("literal_school")
-        self.auth_code: str = kwargs.get("auth_code")
-        self.access_token: str = kwargs.get("access")
-        self.refresh_token: str = kwargs.get("refresh")
-        self.school_subjects: list[Subject] | list[list[Subject]] = []
-        self.email: str
-        self.full_name: str
-        self.gender: str
-        self.cijfers: list[Cijfer]
-        self.leerlingnummer: int
-        self.indentifier: int
-        self.birth_datetime: datetime
-        self.endpoint = "https://api.somtoday.nl"
-        self.pasfoto: PasFoto
-        self.dump_cache: dict[str]
-        self.load_more_data()
-    def fetch_cijfers(self, lower_bound_range: int, upper_bound_range: int) -> list[Cijfer]:
-        """fetches the cijfers and saves it to self.cijfers
-
-        Args:
-            lower_bound_range (int): minimum to return must be greater than 0  and fewer than 100
-            upper_bound_range (int): maximum to return(must be fewer than 100)
-        Raises:
-            ValueError: lower_boung_range or upper_boung_range is negative or more than 100
-            ExceptionGroup: status code is not what is expected
-
-        Returns:
-            list[Cijfer]: list of Cijfers
-        """        
-        if lower_bound_range >= 100 or lower_bound_range <= 0:
-            raise ValueError("lower_bound_range can't be negative or more than 100")
-        elif  upper_bound_range >= 100 or upper_bound_range <= 0:
-            raise ValueError("upper_bound_range can't be negative or more than 100")
-        headers ={
-            "Accept": "Application/json",
-            "Authorization": f"Bearer {self.access_token}",
-            "Range": f"items={lower_bound_range}-{upper_bound_range}"
-        }
-        params = {
-            "additional": ['berekendRapportCijfer']
-        }
-        response = requests.get(f"{self.endpoint}/rest/v1/resultaten/huidigVoorLeerling/{self.indentifier}", params=params, headers=headers)
-        if response.status_code >= 200 and response.status_code < 300:
-            to_dict = response.json()
-            items: list[dict] = to_dict["items"]
-            self.cijfers = []
-            for item in items:
-                tijd_nagekeken = datetime.fromisoformat(item["datumInvoer"])
-                resultaat = item.get("resultaat", "0")
-                leerjaar = item['leerjaar']
-                vak = item["vak"]["naam"]
-                self.cijfers.append(Cijfer(vak=vak, datum=tijd_nagekeken, leerjaar=leerjaar, resultaat=resultaat))
-            self.dump_cache = to_dict
-            return self.cijfers
-        else:
-            raise ExceptionGroup("error", [
-                [
-                    f"response returned status code {response.status_code} from {self.endpoint}/rest/v1/resultaten/huidigVoorLeerling/{self.indentifier}"
-                ]
-            ])
-    def fetch_schedule(self,
-                        begindt: datetime,
-                       enddt: datetime,
-                       group_by_day: bool = False) -> list[Subject] | list[list[Subject]]:
-        """description: fetches the timetable and saves it to self.school_subjects
-        Args:
-            begindt (datetime): starting date to fetch
-            enddt (datetime):   ending date to fetch
-            group_by_day (bool, optional): to group it  by day. Defaults to False.
-
-        Returns:
-            list[Subject]  | list[list[Subject]]:  list what contains Subjects or a grouped Subjects
-        """
-        params_payload = {
-            "begindatum": f"{begindt.year}-{begindt.month}-{begindt.day}",
-            "einddatum": f"{enddt.year}-{enddt.month}-{enddt.day}",
-            "additional": ["vak", "docentAfkortingen"],
-            "sort": "asc-beginDatumTijd"
-        }
-        with requests.get(f"{self.endpoint}/rest/v1/afspraken",
-                          headers={"Accept": "application/json",
-                                   "Authorization": f"Bearer {self.access_token}"},
-                          params=params_payload,
-                          timeout=30) as response:
-            as_json = response.json()
-            items: list[dict] = as_json["items"]
-            self.school_subjects = []
-            groups: dict[str, list[Subject]] = {}
-            for item in items:
-                school_object_dict: dict = item.get(
-                    "additionalObjects").get("vak")
-                afkorting = school_object_dict.get("afkorting")
-                subject_name: str = school_object_dict.get("naam")
-                locatie: str = item.get("locatie")
-                begin_lesuur: int = item.get("beginLesuur")
-                eind_lesuur: int = item.get("eindLesuur")
-                docent_afkorting: str = item.get(
-                    "additionalObjects").get("docentAfkortingen")
-                begin_time: datetime = datetime.fromisoformat(
-                    item.get("beginDatumTijd"))
-                end_time: datetime = datetime.fromisoformat(
-                    item.get("eindDatumTijd"))
-                target_object = Subject(subject=subject_name,
-                                        begindt=begin_time,
-                                        enddt=end_time,
-                                        subject_short=afkorting,
-                                        beginhour=begin_lesuur,
-                                        endhour=eind_lesuur,
-                                        location=locatie,
-                                        teacher_shortcut=docent_afkorting)
-                if group_by_day and begin_time.strftime("%Y-%m-%d") in groups:
-                    group = groups.get(
-                        f"{begin_time.year}-{begin_time.month}-{begin_time.day}")
-                    group.append(target_object)
-                elif group_by_day and begin_time.strftime("%Y-%m-%d")  not in groups:
-                    new_group = {
-                        f"{begin_time.year}-{begin_time.month}-{begin_time.day}": [target_object,]
-                    }
-                    groups.update(new_group)
-                else:
-                    self.school_subjects.append(target_object)
-            if group_by_day:
-                self.school_subjects = [groups.get(x) for x in groups]
-            return self.school_subjects
-
-    def __repr__(self):
-        return f"{self.full_name}, {self.school_name}"
-
-    def __str__(self):
-        return self.__repr__()
-
-    def load_more_data(self) -> bool:
-        """description: generates data(not meant to be called)
-
-        Returns:
-            bool: if it fetched and loaded data by success.
-        """
-        if hasattr(self, "full_name"):
-            return False
-        else:
-            with requests.get(f"{self.endpoint}/rest/v1/leerlingen",
-                              headers={
-                                  "Authorization":
-                                      f"Bearer {self.access_token}",
-                                      "Accept": "application/json"},
-                                      params={"additional": ["pasfoto", "leerlingen"]},
-                                      
-                              timeout=30)as name_response:
-                to_dict = name_response.json()["items"][0]
-                self.pasfoto  = PasFoto(to_dict["additionalObjects"]["pasfoto"]["datauri"])
-                self.full_name = to_dict.get(
-                    "roepnaam") + " " + to_dict.get("achternaam")
-                self.indentifier= to_dict.get("links")[0]["id"]
-                self.email = to_dict.get("email")
-                self.leerlingnummer= to_dict.get("leerlingnummer")
-                self.gender = "Male" if to_dict.get(
-                    "geslacht") == "Man" else "Female"
-                year, month, day = to_dict.get("geboortedatum").split("-")
-                self.birth_datetime = datetime(int(year), int(month), int(day))
-        return True
-
-    @property
-    def school_object(self) -> "School":
-        """description: The school object self(School)
-
-        Returns:
-            School: The School where the student has been fetched.
-        """
-        return School(self.school_name, self.school_uuid)
-
-
-class School:
-    '''
-    Model that represents a school.
-    NOT MEANT TO BE CREATED BY THE USER
-    '''
-
-    def __init__(self, school_name: str, uuid: str) -> None:
-        self.school_name = school_name
-        self.school_uuid = uuid
-        self.__failed_time = 0
-
-    @staticmethod
-    def from_school_uuid(uuid: str) -> "School":
-        """description: Creates a School object from a tenant_uuid(uuid)
-        Args:
-            uuid (str):  The uuid from the school
-
-        Raises:
-            ValueError: uuid is incorrect
-
-        Returns:
-            School: The school what it found
-        """
-        with requests.get("https://servers.somtoday.nl/organisaties.json",
-                          timeout=30)as school_response:
-            as_dict = school_response.json()
-            instellingen = as_dict[0]["instellingen"]
-            exists = tuple(filter(lambda school_: school_[
-                           "uuid"] == uuid, instellingen))
-            if exists:
-                return School(exists[0]["naam"], uuid)
-            else:
-                raise ValueError(f"Invalid  uuid: {uuid}")
-
-    @staticmethod
-    def from_school_name(name: str) -> "School":
-        """description: Alternative to find_school()
-
-        Args:
-            name (str): The school's name
-        Returns:
-            School: The School self
-        """
-        return find_school(name)
-
-    def get_student(self, name: str, password: str) -> Student:
-        """description: Get's the student by name and password(currently the only method)
-        Args:
-            name (str):  The student's name
-            password (str):  The student's password
-
-        Raises:
-            ValueError: Credentials are incorrect.
-            requests.exceptions.RequestException: Error at  last https request. Rarely happens.
-
-        Returns:
-            Student: The student self.
-        """
-        if self.__failed_time > 10:
-            raise ValueError("Credentials might be invalid. Please check")
-        cookies_saved: list | str = []
-        token = base64.urlsafe_b64encode(os.urandom(32)).rstrip(b'=').decode()
-        hashed = base64.urlsafe_b64encode(hashlib.sha256(
-            token.encode()).digest()).rstrip(b'=').decode()
-        payload = {
-            "response_type": "code",
-            "redirect_uri": "somtodayleerling://oauth/callback",
-            "code_challenge": hashed,
-            "tenant_uuid": self.school_uuid,
-            "code_challenge_method": "S256",
-            "state": "".join(random.choices(string.ascii_letters, k=20)),
-            "scope": "openid",
-            "client_id": "D50E0C06-32D1-4B41-A137-A9A850C892C2",
-            "session": "no_session"
-
-        }
-        response = requests.get(
-            "https://inloggen.somtoday.nl/oauth2/authorize",
-            params=payload,
-            allow_redirects=False,
-            timeout=30)
-        cookies_saved = response.cookies
-        parsed = urlparse(response.headers.get("location"))
-        auth_token = parse_qs(parsed.query).get("auth")[0]
-
-        post_headers = {
-            "content-type": "application/x-www-form-urlencoded",
-            "origin": "https://inloggen.somtoday.nl"
-        }
-        firstpos = requests.post("https://inloggen.somtoday.nl/", data={
-            "loginLink": "x",
-            "usernameFieldPanel:usernameFieldPanel_body:usernameField": name
-        }, params={"-1.-panel-signInForm": "",
-                   "auth": auth_token},
-            headers=post_headers, allow_redirects=False, cookies=cookies_saved, timeout=30)
-
-        cookies_saved = firstpos.cookies
-        secondpos = requests.post(
-            "https://inloggen.somtoday.nl/login",
-            data={
-                "loginLink": "x",
-                "passwordFieldPanel:passwordFieldPanel_body:passwordField": password
-            },
-            headers=post_headers,
-            params={
-                "1-1.-passwordForm": "",
-                "auth": auth_token
-            },
-            cookies=cookies_saved,
-            allow_redirects=False,
-            timeout=30
-        )
-        location2 = secondpos.headers.get('location')
-        code_as_return: str = None
-        if location2.startswith("somtodayleerling:"):
-            parsed_url = urlparse(location2)
-            code_as_return: str = parse_qs(parsed_url.query).get("code")[0]
-        else:
-            thirdpost = requests.post(
-                "https://inloggen.somtoday.nl/login",
-                data={
-                    "loginLink": "x",
-                    "passwordFieldPanel:passwordFieldPanel_body:passwordField": password
-                },
-                headers=post_headers,
-                params={
-                    "1-1.-passwordForm": "",
-                    "auth": auth_token
-                },
-                cookies=cookies_saved,
-                allow_redirects=False,
-                timeout=30
-            )
-            location3 = thirdpost.headers.get("location")
-            if location3.startswith("somtodayleerling:"):
-                parsed_url = urlparse(location3)
-                code_as_return: str = parse_qs(parsed_url.query).get("code")[0]
-            else:
-                self.__failed_time += 1
-                return self.get_student(name, password)
-        last_response_payload = {
-            "grant_type":  "authorization_code",
-            "scope": "openid",
-            "client_id": "D50E0C06-32D1-4B41-A137-A9A850C892C2",
-            "tenant_uuid": self.school_uuid,
-            "session": "no_session",
-            "code": code_as_return,
-            "code_verifier":  token
-        }
-        last_response_headers = {
-            "content-type": "application/x-www-form-urlencoded"
-        }
-        last_response_final_response_ara_ara = requests.post(
-            "https://inloggen.somtoday.nl/oauth2/token", data=last_response_payload,
-            headers=last_response_headers,
-            timeout=30)
-        if last_response_final_response_ara_ara.status_code == 200:
-            to_dict = last_response_final_response_ara_ara.json()
-            return Student(name=name,
-                           password=password,
-                           uuid=self.school_uuid,
-                           literal_school=self.school_name,
-                           auth_code=auth_token,
-                           access=to_dict["access_token"],
-                           refresh=to_dict["refresh_token"])
-        else:
-            raise requests.exceptions.RequestException(
-                f"request failed. request code {last_response_final_response_ara_ara.status_code}")
-
-
-def find_school(school_name: str) -> School | None:
-    """description: Function that returns a school by name
-
-    Args:
-        school_name (str): The school's name
-
-    Raises:
-        ValueError: The school's name is incorrect.
-
-    Returns:
-        School | None: The school  itself
-    """
-    with requests.get("https://servers.somtoday.nl/organisaties.json", timeout=30)as schoolresponse:
-        response_as_dict = schoolresponse.json()
-        final_result = tuple(filter(lambda school_dict: school_dict["naam"].lower(
-        ) == school_name.lower(), response_as_dict[0]["instellingen"]))
-        if final_result:
-            return School(school_name, final_result[0]["uuid"])
-        else:
-            raise ValueError(f"{school_name} does not exist")
+'''
+asynchronous support for somtoday API
+'''
+import asyncio
+import base64
+import os
+import string
+from . import nonasyncsomtoday as nonasync_smtd
+from urllib.parse import urlparse, parse_qs
+from datetime import datetime
+from dataclasses import dataclass
+import hashlib
+import random
+import httpx
+from typing import Union
+
+
+class PasFoto(nonasync_smtd.PasFoto):
+    def __init__(self, b64url: str) -> None:
+        super().__init__(b64url)
+
+
+@dataclass
+
+class Cijfer(nonasync_smtd.Cijfer):
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+
+@dataclass
+
+class Subject(nonasync_smtd.Subject):
+
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+
+class Student(nonasync_smtd.Student):
+    '''
+    Model that presents a Student
+    NOT MEANT TO BE CREATED BY USER
+    '''
+
+    def __init__(self, **kwargs) -> None:
+        self.name: str = kwargs.get("name")
+        self.password: str = kwargs.get("password")
+        self.school_uuid: str = kwargs.get("uuid")
+        self.school_name: str = kwargs.get("literal_school")
+        self.auth_code: str = kwargs.get("auth_code")
+        self.access_token: str = kwargs.get("access")
+        self.refresh_token: str = kwargs.get("refresh")
+        self.school_subjects: list[Union[Subject, list[Subject]]] = []
+        self.email: str
+        self.full_name: str
+        self.gender: str
+        self.cijfers: list[Cijfer]
+        self.leerlingnummer: int
+        self.indentifier: int
+        self.birth_datetime: datetime
+        self.endpoint = "https://api.somtoday.nl"
+        self.pasfoto: PasFoto
+        self.dump_cache: dict[str]
+
+    async def yield_fetch_cijfers(self, lower_bound_range: int, upper_bound_range: int):
+        """yields the cijfers by calling self.fetch_cijfers() and yielding it results
+
+        Args:
+            lower_bound_range (int):  minimum to return (must be greater than 0 and fewer than 100)
+            upper_bound_range (int):  maximum to return (must be fewer than 100)
+
+        Yields:
+            cijfer: Cijfer object
+        """        
+        
+        cijfers = await self.fetch_cijfers(lower_bound_range, upper_bound_range)
+        for cijfer in cijfers:
+            yield cijfer
+
+
+    async def fetch_cijfers(self, lower_bound_range: int, upper_bound_range: int) -> list[Cijfer]:
+        """fetches the cijfers and saves it to self.cijfers
+
+        Args:
+            lower_bound_range (int): minimum to return must be greater than 0  and fewer than 100
+            upper_bound_range (int): maximum to return(must be fewer than 100)
+        Raises:
+            ValueError: lower_boung_range or upper_boung_range is negative or more than 100
+            ExceptionGroup: status code is not what is expected
+
+        Returns:
+            list[Cijfer]: list of Cijfers
+        """
+        if lower_bound_range >= 100 or lower_bound_range <= 0:
+            raise ValueError("lower_bound_range can't be negative or more than 100")
+        elif upper_bound_range >= 100 or upper_bound_range <= 0:
+            raise ValueError("upper_bound_range can't be negative or more than 100")
+        headers = {
+            "Accept": "Application/json",
+            "Authorization": f"Bearer {self.access_token}",
+            "Range": f"items={lower_bound_range}-{upper_bound_range}"
+        }
+        params = {
+            "additional": ['berekendRapportCijfer']
+        }
+        async with httpx.AsyncClient() as session:
+            response = await session.get(f"{self.endpoint}/rest/v1/resultaten/huidigVoorLeerling/{self.identifier}",
+                                         params=params, headers=headers)
+            if response.status_code >= 200 and response.status_code < 300:
+                to_dict = response.json()
+                items: list[dict] = to_dict["items"]
+                self.cijfers = []
+                for item in items:
+                    tijd_nagekeken = datetime.fromisoformat(item["datumInvoer"])
+                    resultaat = item.get("resultaat", "0")
+                    leerjaar = item['leerjaar']
+                    vak = item["vak"]["naam"]
+                    self.cijfers.append(Cijfer(vak=vak, datum=tijd_nagekeken, leerjaar=leerjaar, resultaat=resultaat))
+                self.dump_cache = to_dict
+                return self.cijfers
+            else:
+                raise ExceptionGroup("error", [
+                    [
+                        f"response returned status code {response.status_code} from {self.endpoint}/rest/v1/resultaten/huidigVoorLeerling/{self.identifier}"
+                    ]
+                ])
+
+    async def yield_fetch_schedule(self,
+                             begindt: datetime,
+                             enddt: datetime,
+                             group_by_day: bool = False):
+        """Yielding each ``Subject`` object 
+
+        Args:
+            begindt (datetime): starting date to fetch
+            enddt (datetime): ending date to fetch
+            group_by_day (bool, optional): to group it by day. Defaults to False.
+
+        """        
+        schedule = await self.fetch_schedule(begindt, enddt, group_by_day)
+        for subject in schedule:
+            yield subject
+    async def fetch_schedule(self,
+                             begindt: datetime,
+                             enddt: datetime,
+                             group_by_day: bool = False) -> list[Union[list[Subject], Subject]]:
+        """description: fetches the timetable and saves it to self.school_subjects
+        Args:
+            begindt (datetime): starting date to fetch
+            enddt (datetime):   ending date to fetch
+            group_by_day (bool, optional): to group it  by day. Defaults to False.
+
+        Returns:
+            list[Subject]  | list[list[Subject]]:  list that contains Subjects or a grouped Subjects
+        """
+        params_payload = {
+            "begindatum": f"{begindt.year}-{begindt.month}-{begindt.day}",
+            "einddatum": f"{enddt.year}-{enddt.month}-{enddt.day}",
+            "additional": ["vak", "docentAfkortingen"],
+            "sort": "asc-beginDatumTijd"
+        }
+        async with httpx.AsyncClient() as client:
+            response = await client.get(f"{self.endpoint}/rest/v1/afspraken",
+                                        headers={"Accept": "application/json",
+                                                 "Authorization": f"Bearer {self.access_token}"},
+                                        params=params_payload)
+            as_json = response.json()
+            items: list[dict] = as_json["items"]
+            self.school_subjects = []
+            groups: dict[str, list[Subject]] = {}
+            for item in items:
+                school_object_dict: dict = item.get("additionalObjects").get("vak")
+                afkorting = school_object_dict.get("afkorting")
+                subject_name: str = school_object_dict.get("naam")
+                locatie: str = item.get("locatie")
+                begin_lesuur: int = item.get("beginLesuur")
+                eind_lesuur: int = item.get("eindLesuur")
+                docent_afkorting: str = item.get("additionalObjects").get("docentAfkortingen")
+                begin_time: datetime = datetime.fromisoformat(item.get("beginDatumTijd"))
+                end_time: datetime = datetime.fromisoformat(item.get("eindDatumTijd"))
+                target_object = Subject(subject=subject_name,
+                                        begindt=begin_time,
+                                        enddt=end_time,
+                                        subject_short=afkorting,
+                                        beginhour=begin_lesuur,
+                                        endhour=eind_lesuur,
+                                        location=locatie,
+                                        teacher_shortcut=docent_afkorting)
+                if group_by_day and begin_time.strftime("%Y-%m-%d") in groups:
+                    group = groups.get(begin_time.strftime("%Y-%m-%d"))
+                    group.append(target_object)
+                elif group_by_day and begin_time.strftime("%Y-%m-%d") not in groups:
+                    new_group = {
+                        begin_time.strftime("%Y-%m-%d"): [target_object]
+                    }
+                    groups.update(new_group)
+                else:
+                    self.school_subjects.append(target_object)
+            if group_by_day:
+                self.school_subjects = [groups.get(x) for x in groups]
+            return self.school_subjects
+
+
+    async def load_more_data(self) -> bool:
+        '''
+        function that loads data what will be saved by the self object.
+        '''
+        if hasattr(self, "full_name"):
+            return False
+        else:
+            async with httpx.AsyncClient() as client:
+                name_response = await client.get(f"{self.endpoint}/rest/v1/leerlingen",
+                                                 headers={
+                                                     "Authorization": f"Bearer {self.access_token}",
+                                                     "Accept": "application/json"},
+                                                 params={"additional": ["pasfoto", "leerlingen"]})
+                to_dict = name_response.json()
+                to_dict = to_dict["items"][0]
+                self.pasfoto = PasFoto(to_dict["additionalObjects"]["pasfoto"]["datauri"])
+                self.full_name = to_dict.get("roepnaam") + " " + to_dict.get("achternaam")
+                self.identifier = to_dict.get("links")[0]["id"]
+                self.email = to_dict.get("email")
+                self.leerlingnummer = to_dict.get("leerlingnummer")
+                self.gender = "Male" if to_dict.get("geslacht") == "Man" else "Female"
+                year, month, day = to_dict.get("geboortedatum").split("-")
+                self.birth_datetime = datetime(int(year), int(month), int(day))
+            return True
+
+
+class School(nonasync_smtd.School):
+    '''
+    Model that represents a school
+    NOT  MEANT TO BE CREATED BY USER
+    '''
+
+    def __init__(self, *args) -> None:
+        super().__init__(*args)
+
+    @staticmethod
+    async def from_school_uuid(uuid: str) -> "School":
+        """Gets a school by school uuid
+
+        Args:
+            uuid (str): the school uuid
+
+        Raises:
+            ValueError: school does not exist
+
+        Returns:
+            School: object that represents the School
+        """
+        async with httpx.AsyncClient() as session:
+            school_response = await session.get("https://servers.somtoday.nl/organisaties.json")
+            as_dict = school_response.json()
+            instellingen = as_dict[0]["instellingen"]
+            exists = tuple(filter(lambda school_: school_["uuid"] == uuid, instellingen))
+            if exists:
+                return School(exists[0]["naam"], uuid)
+            raise ValueError(f"Invalid  uuid: {uuid}")
+
+    @staticmethod
+    async def from_school_name(name: str) -> "School":
+        '''
+        get the School from_school name, alternative to find_school(name)
+        '''
+        return await find_school(name)
+
+    async def get_student(self, name: str, password: str) -> Student:
+        """description: Gets the student by name and password(without SSO)
+        Args:
+            name (str):  The student's name - The login name you use to login at inloggen.somtoday.nl
+            password (str):  The student's password
+
+        Raises:
+            ValueError: Credentials are incorrect.
+            requests.exceptions.RequestException: Error at  last https request. Rarely happens.
+
+        Returns:
+            Student: The student self.
+        """
+
+        if self.__failed_time > 10:
+            raise ValueError("Credentials might be invalid. Please check")
+        cookies_saved = []
+        token = base64.urlsafe_b64encode(os.urandom(32)).rstrip(b'=').decode()
+        hashed = base64.urlsafe_b64encode(hashlib.sha256(token.encode()).digest()).rstrip(b'=') \
+            .decode()
+        payload = {
+            "response_type": "code",
+            "redirect_uri": "somtodayleerling://oauth/callback",
+            "code_challenge": hashed,
+            "tenant_uuid": self.school_uuid,
+            "code_challenge_method": "S256",
+            "state": "".join(random.choices(string.ascii_letters, k=20)),
+            "scope": "openid",
+            "client_id": "D50E0C06-32D1-4B41-A137-A9A850C892C2",
+            "session": "no_session"
+
+        }
+        async with httpx.AsyncClient() as client:
+            response = await client.get("https://inloggen.somtoday.nl/oauth2/authorize",
+                                        params=payload,
+                                        follow_redirects=False)
+            cookies_saved = response.cookies
+            parsed = urlparse(response.headers.get("location"))
+            auth_token = parse_qs(parsed.query).get("auth")[0]
+
+            post_headers = {
+                "content-type": "application/x-www-form-urlencoded",
+                "origin": "https://inloggen.somtoday.nl"
+            }
+            firstpos = await client.post("https://inloggen.somtoday.nl/", data={
+                "loginLink": "x",
+                "usernameFieldPanel:usernameFieldPanel_body:usernameField": name
+            }, params={"-1.-panel-signInForm": "",
+                       "auth": auth_token},
+                                         headers=post_headers,
+                                         follow_redirects=False,
+                                         cookies=cookies_saved)
+
+            cookies_saved = firstpos.cookies
+            secondpos = await client.post(
+                "https://inloggen.somtoday.nl/login",
+                data={
+                    "loginLink": "x",
+                    "passwordFieldPanel:passwordFieldPanel_body:passwordField": password
+                },
+                headers=post_headers,
+                params={
+                    "1-1.-passwordForm": "",
+                    "auth": auth_token
+                },
+                cookies=cookies_saved,
+                follow_redirects=False
+            )
+            location2 = secondpos.headers.get('location')
+            code_as_return: str = None
+            if location2.startswith("somtodayleerling:"):
+                parsed_url = urlparse(location2)
+                code_as_return: str = parse_qs(parsed_url.query).get("code")[0]
+            else:
+                thirdpost = await client.post(
+                    "https://inloggen.somtoday.nl/login",
+                    data={
+                        "loginLink": "x",
+                        "passwordFieldPanel:passwordFieldPanel_body:passwordField": password
+                    },
+                    headers=post_headers,
+                    params={
+                        "1-1.-passwordForm": "",
+                        "auth": auth_token
+                    },
+                    cookies=cookies_saved,
+                    allow_redirects=False
+                )
+                location3 = thirdpost.headers.get("location")
+                if location3.startswith("somtodayleerling:"):
+                    parsed_url = urlparse(location3)
+                    code_as_return: str = parse_qs(parsed_url.query).get("code")[0]
+                else:
+                    self.__failed_time += 1
+                    return await self.get_student(name, password)
+            last_response_payload = {
+                "grant_type": "authorization_code",
+                "scope": "openid",
+                "client_id": "D50E0C06-32D1-4B41-A137-A9A850C892C2",
+                "tenant_uuid": self.school_uuid,
+                "session": "no_session",
+                "code": code_as_return,
+                "code_verifier": token
+            }
+            last_response_headers = {
+                "content-type": "application/x-www-form-urlencoded"
+            }
+            final_response = await client.post("https://inloggen.somtoday.nl/oauth2/token",
+                                               data=last_response_payload,
+                                               headers=last_response_headers)
+            if final_response.status_code == 200:
+                to_dict = final_response.json()
+                new_student_created = Student(name=name,
+                                              password=password,
+                                              uuid=self.school_uuid,
+                                              literal_school=self.school_name,
+                                              auth_code=auth_token,
+                                              access=to_dict["access_token"],
+                                              refresh=to_dict["refresh_token"])
+                await new_student_created.load_more_data()
+                return new_student_created
+
+            else:
+                raise ValueError(f"request failed: code {final_response.status_code}")
+
+
+async def find_school(school_name: str) -> School:
+    """gets & returns a School object, alternative to School.from_school_name(name)
+    Args:
+        school_name (str): name of the school
+
+    Raises:
+        ValueError: School is not registered by somtoday or school_name invalid
+
+    Returns:
+        School: The School model  representation
+    """
+    async with httpx.AsyncClient() as client:
+        schoolresponse = await client.get("https://servers.somtoday.nl/organisaties.json")
+        response_as_dict = schoolresponse.json()
+        final_result = tuple(filter(
+            lambda school_dict: school_dict["naam"].lower() == school_name.lower(),
+            response_as_dict[0]["instellingen"]))
+        if final_result:
+            return School(school_name, final_result[0]["uuid"])
+        else:
+            raise ValueError(f"{school_name} does not exist")
```

### Comparing `somtodaypython-0.0.3/somtodaypython.egg-info/PKG-INFO` & `somtodaypython-0.0.4/somtodaypython.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,127 @@
-Metadata-Version: 2.1
-Name: somtodaypython
-Version: 0.0.3
-Summary: Python package for interacting & fetching somtoday's data.
-Home-page: https://github.com/luxkatana/somtodayapi_python
-Author: luxkatana/TheTrojanHorse
-Author-email: taseen.bibi@gmail.com
-Description-Content-Type: text/markdown
-
-***Somtoday Python, the interactor***
-
-***changes in 0.0.3***
-<ul>
-<li>added PasFoto feature to get the PasFoto/Photo of the student.</li>
-<li>added new attribute: student.identifier for student's account's ID</li>
-<li>old student.identifier has been moved to student.leerlingnummer </li>
-</ul>
-
-
-> What the f**ck is this?
-
-this(somtoday python) is a package that fetches and interacts with somtoday API using https requests.
-
-**installation**
-
-*for macos & linux*
-```
-python3 -m pip3 install somtodaypython 
-```
-*for windows*
-```
-python3 -m pip install somtodaypython 
-```
-OR
-```
-python -m pip install somtodaypython
-```
-
-if neither above works then you can always do this
-```
-pip3 install git+https://github.com/luxkatana/somtodayapi_python
-```
-***examples***
-
-*basic interacting with a student(getting data from the student)*
-```py
-
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
-```
-*basic interacting with the timetable of a student*
-```py
-import somtodaypython.nonasyncsomtoday as nonasync_somtoday
-from datetime import timedelta, datetime as dt
-school = nonasync_somtoday.find_school("SchoolName")
-student = school.get_student("NAME", "password")
-today = dt.now()
-tomorrow = today + timedelta(days=2)
-timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
-for day in timetable:
-    for day_subject in day:
-        print(day_subect.subject_name)
-```
-
-**Asynchronous suppport**
-
-We also support asynchronous for somtodaypython.
-
-*Basic interacting with a student(asynchronous)*
-```py
-import somtodaypython.asynchronous_somtoday as async_somtoday
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    print(student.full_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-*Basic interacting with a student's timetable(asynchronous)*
-
-```py
-
-import somtodaypython.asynchronous_somtoday as async_somtoday
-from datetime import timedelta,datetime as dt
-import  asyncio # builtin library for asynchronous execution
-async def main() -> None:
-    now = dt.now()
-    tomorrow = now + timedelta(days=2)
-    school = await async_somtoday.find_school("SCHOOLNAME")
-    student = await school.get_student("NAME", "PASSWORD")
-    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
-    for day in timetable:
-        for  subject in day:
-            print(subject.subject_name)
-asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
-```
-
-
-**Ending**
-
-
-New features are always welcome! email taseen.bibi@gmail.com
-
-
-**Huizengek#6623**
-Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
-
-github: https://github.com/25huizengek1
-
-
-**elisaado**
-
-Special thanks to **elisaado** for making important API endpoints visible to other users.
-
-github: https://github.com/elisaado/somtoday-api-docs
+Metadata-Version: 2.1
+Name: somtodaypython
+Version: 0.0.4
+Summary: Python package for interacting & fetching somtoday's data.
+Home-page: https://github.com/luxkatana/somtodayapi_python
+Author: luxkatana/TheTrojanHorse
+Author-email: taseen.bibi@gmail.com
+Description-Content-Type: text/markdown
+
+***Somtoday Python, the interactor***
+
+***changes in 0.0.4***
+<ul>
+<li> I got more lazier so I wanted to announce this in Dutch </li>
+<li> Gefixt dat Student.fetch_schedule(group_by_day=True) dat het weer werkt(zat blijkbaar een bug in) </li>
+<li> Documentatie verbetert </li>
+<li> Er zat een probleem met Union types, gefixt </li>
+<li> Je kan 2 studenten vergelijken als Student.full_name en Student.school_name allebei gelijk zijn
+<li> Vergelijkingen met Cijfers(kijken als cijfers zijn hoger of lager) Cijfers worden bepaald door Cijfers.resultaat
+<li>beter __repr__ en __str__ voor Cijfer en Subject</li>
+<li>Cijfers resultaat yielden is mogelijk door Student.yield_fetch_cijfers() te doen (ook met asynchronous)</li>
+<li>Rooster vakken yielden is mogelijk door Student.yield_fetch_schedule() te doen (ook met asynchronous)</li>
+</ul>
+
+
+somtodaypython is a package that fetches and interacts with Somtoday API using https requests.
+
+**installation**
+
+*for macos & linux*
+```
+python3 -m pip3 install somtodaypython 
+```
+*for windows*
+```
+python3 -m pip install somtodaypython 
+```
+OR
+```
+python -m pip install somtodaypython
+```
+
+if neither above works then you can always do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python
+```
+
+If you want to try beta versions do this
+```
+pip3 install git+https://github.com/luxkatana/somtodayapi_python/dev
+```
+***examples***
+
+*basic interacting with a student(getting data from the student)*
+```py
+
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+print(f"email : {student.email}\tname: {student.full_name}\tgender: {student.gender}")
+```
+*basic interacting with the timetable of a student*
+```py
+import somtodaypython.nonasyncsomtoday as nonasync_somtoday
+from datetime import timedelta, datetime as dt
+school = nonasync_somtoday.find_school("SchoolName")
+student = school.get_student("NAME", "password")
+today = dt.now()
+tomorrow = today + timedelta(days=2)
+timetable: list[list[nonasync_somtoday.Subject]] = student.fetch_schedule(today, tomorrow, group_by_day=True)
+for day in timetable:
+    for day_subject in day:
+        print(day_subject.subject_name)
+```
+
+**Asynchronous support**
+
+We also support asynchronous for somtodaypython.
+
+*Basic interacting with a student(asynchronous)*
+```py
+import somtodaypython.asynchronous_somtoday as async_somtoday
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    print(student.full_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+*Basic interacting with a student's timetable(asynchronous)*
+
+```py
+
+import somtodaypython.asynchronous_somtoday as async_somtoday
+from datetime import timedelta,datetime as dt
+import  asyncio # builtin library for asynchronous execution
+async def main() -> None:
+    now = dt.now()
+    tomorrow = now + timedelta(days=2)
+    school = await async_somtoday.find_school("SCHOOLNAME")
+    student = await school.get_student("NAME", "PASSWORD")
+    timetable: list[list[async_somtoday.Subject]] = await student.fetch_schedule(now, tomorrow, group_by_day=True)
+    for day in timetable:
+        for  subject in day:
+            print(subject.subject_name)
+asyncio.get_event_loop().run_until_complete(main()) # executing the main() function
+```
+
+
+**Ending**
+
+
+New features are always welcome! email taseen.bibi@gmail.com
+
+
+**Huizengek#6623**
+Special thanks to **Huizengek#6623** for showing the method of getting the access token & interacting with the somtoday API.
+
+github: https://github.com/25huizengek1
+
+
+**elisaado**
+
+Special thanks to **elisaado** for making important API endpoints visible to other users.
+
+github: https://github.com/elisaado/somtoday-api-docs
```

