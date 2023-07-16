# Comparing `tmp/barladb-0.1.4.tar.gz` & `tmp/barladb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barladb-0.1.4.tar", last modified: Sat Jul 15 14:32:44 2023, max compression
+gzip compressed data, was "barladb-0.1.5.tar", last modified: Sun Jul 16 10:49:17 2023, max compression
```

## Comparing `barladb-0.1.4.tar` & `barladb-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.579240 barladb-0.1.4/
--rw-rw-rw-   0        0        0     3312 2023-07-15 14:32:44.580542 barladb-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.575151 barladb-0.1.4/barladb/
--rw-rw-rw-   0        0        0      342 2023-07-15 11:58:29.000000 barladb-0.1.4/barladb/classes.py
--rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.4/barladb/config.py
--rw-rw-rw-   0        0        0     2057 2023-07-15 14:30:46.000000 barladb-0.1.4/barladb/db.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.579240 barladb-0.1.4/barladb.egg-info/
--rw-rw-rw-   0        0        0     3312 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 14:32:44.580542 barladb-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3447 2023-07-15 14:32:21.000000 barladb-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.492751 barladb-0.1.5/
+-rw-rw-rw-   0        0        0     3588 2023-07-16 10:49:17.492751 barladb-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.488686 barladb-0.1.5/barladb/
+-rw-rw-rw-   0        0        0      342 2023-07-15 11:58:29.000000 barladb-0.1.5/barladb/classes.py
+-rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.5/barladb/config.py
+-rw-rw-rw-   0        0        0     2979 2023-07-16 10:29:28.000000 barladb-0.1.5/barladb/db.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:49:17.491694 barladb-0.1.5/barladb.egg-info/
+-rw-rw-rw-   0        0        0     3588 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 14:32:44.000000 barladb-0.1.5/barladb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-16 10:49:17.000000 barladb-0.1.5/barladb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:49:17.493803 barladb-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3723 2023-07-16 10:34:55.000000 barladb-0.1.5/setup.py
```

### Comparing `barladb-0.1.4/PKG-INFO` & `barladb-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-Metadata-Version: 2.1
-Name: barladb
-Version: 0.1.4
-Summary: A very easy local database based on JSON
-Author: barlin41k
-Author-email: sasaigrypocta@gmail.com
-Description-Content-Type: text/markdown
-
+from setuptools import setup
 
+setup(
+    name='barladb',
+    version='0.1.5',
+    description='A very easy local database based on JSON',
+    packages=['barladb'],
+    author_email='sasaigrypocta@gmail.com',
+    author="barlin41k",
+    zip_safe=False,
+    long_description='''
 # Изменения:
-- В классе `Json` я указал неправильную функцию в файле `db.py`. `db.create` будет работать корректно!
+- Добавлена новая тестовая функция:
+```python
+db.search(filepath, key)
+```
+- Она парсит файл БД, и в случае прям точного совпадения (К примеру `age = age`) показывает значение данного столбца
+- В скором добавлю показывание нескольких совпадений (К примеру `age, ages`)
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
@@ -43,8 +50,9 @@
 # Как установить?
 - `pip install barladb`
 
 # Особенности barlaDB
 - Простота в использовании
 - Очень лёгкий интерфейс
 - Базирована на всеми известном `JSON`
-    
+    ''',
+    long_description_content_type="text/markdown",)
```

### Comparing `barladb-0.1.4/barladb/db.py` & `barladb-0.1.5/barladb/db.py`

 * *Files 27% similar despite different names*

```diff
@@ -35,21 +35,39 @@
         if data == None:
             print("BarlaDB: " + Fore.YELLOW + "Переменная с данными пуста." + Style.RESET_ALL)
         else:
             return
     except:
         print("BarlaDB: " + Fore.RED + f"Базы данных {filepath} не существует!" + Style.RESET_ALL)
         return
+#create - создать БД
 def create(filename: str):
     Json.save(filename, data)
     if config.debug:
         print("BarlaDB: " + Fore.GREEN + f"База данных {filepath} была успешно создана!" + Style.RESET_ALL)
-def delete(filename: str):
-  try:
-    os.remove(f"{filename}.json")
-    if config.debug:
-      print("BarlaDB: " + Fore.GREEN + f"База данных {filepath} была успешно удалена!" + Style.RESET_ALL)
-    else:
-       return data
-  except:
-    print("BarlaDB: " + Fore.RED + f"Базы данных {filepath} не существует!" + Style.RESET_ALL)
-    return
+#delete - удалить БД
+def delete(filepath: str):
+    try:
+        os.remove(f"{filename}.json")
+        if config.debug:
+            print("BarlaDB: " + Fore.GREEN + f"База данных {filepath} была успешно удалена!" + Style.RESET_ALL)
+        else:
+            return data
+    except:
+        print("BarlaDB: " + Fore.RED + f"Базы данных {filepath} не существует!" + Style.RESET_ALL)
+        return
+def search(filepath, key):
+    try:
+        with open(filepath + ".json", "r") as file:
+            data = Json.get(filepath)
+            if data == {}:
+                print("BarlaDB: " + Fore.YELLOW + "База данных пустая." + Style.RESET_ALL)
+                return
+            if key in data:
+                print("BarlaDB: " + Fore.GREEN + "Найдено одно совпадение.\n" + Style.RESET_ALL + f'"{key}": {data[key]}')
+                return data[key]
+            else:
+                print("BarlaDB: " + Fore.YELLOW + "Не найдено ни одно совпадение." + Style.RESET_ALL)
+                return None
+    except:
+        print("BarlaDB: " + Fore.RED + f"Базы данных {filepath} не существует!" + Style.RESET_ALL)
+        return
```

### Comparing `barladb-0.1.4/barladb.egg-info/PKG-INFO` & `barladb-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.4
+Version: 0.1.5
 Summary: A very easy local database based on JSON
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 
 # Изменения:
-- В классе `Json` я указал неправильную функцию в файле `db.py`. `db.create` будет работать корректно!
+- Добавлена новая тестовая функция:
+```python
+db.search(filepath, key)
+```
+- Она парсит файл БД, и в случае прям точного совпадения (К примеру `age = age`) показывает значение данного столбца
+- В скором добавлю показывание нескольких совпадений (К примеру `age, ages`)
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
```

