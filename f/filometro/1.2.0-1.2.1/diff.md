# Comparing `tmp/filometro-1.2.0.tar.gz` & `tmp/filometro-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filometro-1.2.0.tar", last modified: Fri Dec 23 02:02:45 2022, max compression
+gzip compressed data, was "filometro-1.2.1.tar", last modified: Sun Jul 16 21:53:49 2023, max compression
```

## Comparing `filometro-1.2.0.tar` & `filometro-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2022-12-23 02:02:45.609601 filometro-1.2.0/
--rw-r--r--   0 matheus   (1000) matheus   (1000)     1071 2022-03-17 02:44:05.000000 filometro-1.2.0/LICENSE
--rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2022-12-23 02:02:45.609601 filometro-1.2.0/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)     9691 2022-12-23 01:57:30.000000 filometro-1.2.0/README.md
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2022-12-23 02:02:45.609601 filometro-1.2.0/filometro/
--rw-r--r--   0 matheus   (1000) matheus   (1000)      571 2022-12-23 01:57:30.000000 filometro-1.2.0/filometro/__init__.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     3064 2022-12-23 01:57:30.000000 filometro-1.2.0/filometro/dataclasses.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     1880 2022-10-21 23:35:36.000000 filometro-1.2.0/filometro/deolhonafila.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     4161 2022-12-23 01:57:30.000000 filometro-1.2.0/filometro/enums.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     4279 2022-12-23 01:57:30.000000 filometro-1.2.0/filometro/filometro.py
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2022-12-23 02:02:45.609601 filometro-1.2.0/filometro.egg-info/
--rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2022-12-23 02:02:45.000000 filometro-1.2.0/filometro.egg-info/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)      337 2022-12-23 02:02:45.000000 filometro-1.2.0/filometro.egg-info/SOURCES.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2022-12-23 02:02:45.000000 filometro-1.2.0/filometro.egg-info/dependency_links.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2022-03-29 22:27:15.000000 filometro-1.2.0/filometro.egg-info/not-zip-safe
--rw-r--r--   0 matheus   (1000) matheus   (1000)       17 2022-12-23 02:02:45.000000 filometro-1.2.0/filometro.egg-info/requires.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2022-12-23 02:02:45.000000 filometro-1.2.0/filometro.egg-info/top_level.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2022-12-23 02:02:45.609601 filometro-1.2.0/setup.cfg
--rw-r--r--   0 matheus   (1000) matheus   (1000)     3136 2022-10-21 23:35:36.000000 filometro-1.2.0/setup.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.127969 filometro-1.2.1/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     1071 2022-03-17 02:44:05.000000 filometro-1.2.1/LICENSE
+-rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2023-07-16 21:53:49.117969 filometro-1.2.1/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     9691 2022-12-23 01:57:30.000000 filometro-1.2.1/README.md
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.117969 filometro-1.2.1/filometro/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      571 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/__init__.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     3064 2023-07-14 19:28:15.000000 filometro-1.2.1/filometro/dataclasses.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     2383 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/deolhonafila.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     4161 2022-12-23 01:57:30.000000 filometro-1.2.1/filometro/enums.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      212 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/exceptions.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     4299 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/filometro.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.117969 filometro-1.2.1/filometro.egg-info/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      361 2023-07-16 21:53:49.000000 filometro-1.2.1/filometro.egg-info/SOURCES.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/dependency_links.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2022-03-29 22:27:15.000000 filometro-1.2.1/filometro.egg-info/not-zip-safe
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       17 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/requires.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2023-07-16 21:53:49.000000 filometro-1.2.1/filometro.egg-info/top_level.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2023-07-16 21:53:49.127969 filometro-1.2.1/setup.cfg
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     3136 2022-10-21 23:35:36.000000 filometro-1.2.1/setup.py
```

### Comparing `filometro-1.2.0/LICENSE` & `filometro-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `filometro-1.2.0/PKG-INFO` & `filometro-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filometro
-Version: 1.2.0
+Version: 1.2.1
 Summary: Obtenha os dados dos postos de vacinação da covid-19 em São Paulo
 Home-page: https://github.com/matheusfelipeog/filometro
 Author: Matheus Felipe
 Author-email: matheusfelipeog@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/matheusfelipeog/filometro/issues
 Project-URL: Documentation, https://github.com/matheusfelipeog/filometro/tree/master#documentação
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: filometro Version: 1.2.0 Summary: Obtenha os dados
+Metadata-Version: 2.1 Name: filometro Version: 1.2.1 Summary: Obtenha os dados
 dos postos de vacinaÃ§Ã£o da covid-19 em SÃ£o Paulo Home-page: https://
 github.com/matheusfelipeog/filometro Author: Matheus Felipe Author-email:
 matheusfelipeog@protonmail.com License: MIT License Project-URL: Bug Tracker,
 https://github.com/matheusfelipeog/filometro/issues Project-URL: Documentation,
 https://github.com/matheusfelipeog/filometro/tree/master#documentaÃ§Ã£o
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-
```

### Comparing `filometro-1.2.0/README.md` & `filometro-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `filometro-1.2.0/filometro/__init__.py` & `filometro-1.2.1/filometro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'Zone',
     'Modality',
     'Situation',
     'Immunizing',
     'District',
     'Filometro'
 ]
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 __author__ = 'Matheus Felipe'
 
 from filometro.enums import Zone
 from filometro.enums import Modality
 from filometro.enums import Situation
 from filometro.enums import Immunizing
 from filometro.enums import District
```

### Comparing `filometro-1.2.0/filometro/dataclasses.py` & `filometro-1.2.1/filometro/dataclasses.py`

 * *Files identical despite different names*

### Comparing `filometro-1.2.0/filometro/deolhonafila.py` & `filometro-1.2.1/filometro/deolhonafila.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 """
 filometro.deolhonafila
 ----------------------
 
-Disponíbiliza formas de ter acesso aos dados do site 'De Olho na Fila'.
+Disponibiliza formas de ter acesso aos dados do site 'De Olho na Fila'.
 """
 
 __all__ = ['APIDeOlhoNaFila']
 
 from typing import List
 
 import requests
 
+from filometro.exceptions import DataCollectionError
+
 
 class APIDeOlhoNaFila():
     """Um wrapper da API do site 'De Olho na Fila'."""
 
     def __init__(self) -> None:
-        self.endpoint = 'https://deolhonafila.prefeitura.sp.gov.br/processadores/dados.php'
+        self.endpoint = (
+            'https://deolhonafila.prefeitura.sp.gov.br'
+            '/processadores/dados.php'
+        )
         self.payload = {'dados': 'dados'}
         self.headers = {
             'User-Agent': (
-                'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)'
-                'Chrome/95.0.4638.69 Safari/537.36'
+                'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36'
+                '(KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36'
             ),
             'Host': 'deolhonafila.prefeitura.sp.gov.br',
             'Connection': 'keep-alive',
             'Content-Length': '11',
-            'sec-ch-ua': '"Google Chrome";v="95", "Chromium";v="95", ";Not A Brand";v="99"',
+            'sec-ch-ua': (
+                '"Google Chrome";v="95", "Chromium";'
+                'v="95", ";Not A Brand";v="99"'
+            ),
             'Accept': 'application/json, text/javascript, */*; q=0.01',
             'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'X-Requested-With': 'XMLHttpRequest',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'Origin': 'https://deolhonafila.prefeitura.sp.gov.br',
             'Sec-Fetch-Site': 'same-origin',
@@ -42,12 +50,26 @@
             'dnt': '1',
             'sec-gpc': '1'
         }
 
     def get_data(self) -> List[dict]:
         """Pegue todos os dados do site 'De Olho na Fila'."""
 
-        response = requests.post(self.endpoint, headers=self.headers, data=self.payload)
-
-        response.raise_for_status()
+        data = []
+        try:
+            response = requests.post(
+                self.endpoint,
+                headers=self.headers,
+                data=self.payload,
+                timeout=15
+            )
+
+            response.raise_for_status()
+
+            data = response.json()
+
+        except (requests.Timeout, requests.HTTPError) as err:
+            raise DataCollectionError(
+                'Não foi possível coletar os dados no site "De Olho na Fila".'
+            ) from err
 
-        return response.json()
+        return data
```

### Comparing `filometro-1.2.0/filometro/enums.py` & `filometro-1.2.1/filometro/enums.py`

 * *Files identical despite different names*

### Comparing `filometro-1.2.0/filometro/filometro.py` & `filometro-1.2.1/filometro/filometro.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 -------------------
 
 Fornece a API pública principal do pacote.
 """
 
 __all__ = ['Filometro']
 
-from typing import List
+from typing import List, Union
 
 from dataclasses import asdict
 
 from filometro.deolhonafila import APIDeOlhoNaFila
 
 from filometro.dataclasses import Posto
 
@@ -59,15 +59,15 @@
 
 class Filometro():
     """Filometro é a API príncipal do pacote.
 
     Fornence os métodos para coletar e filtrar os dados dos postos.
     """
 
-    def __init__(self, _api: APIDeOlhoNaFila = None) -> None:
+    def __init__(self, _api: Union[APIDeOlhoNaFila, None] = None) -> None:
         self._api = _api or APIDeOlhoNaFila()
 
         self._postos = self._load_postos()
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(postos={len(self._postos)})'
```

### Comparing `filometro-1.2.0/filometro.egg-info/PKG-INFO` & `filometro-1.2.1/filometro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filometro
-Version: 1.2.0
+Version: 1.2.1
 Summary: Obtenha os dados dos postos de vacinação da covid-19 em São Paulo
 Home-page: https://github.com/matheusfelipeog/filometro
 Author: Matheus Felipe
 Author-email: matheusfelipeog@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/matheusfelipeog/filometro/issues
 Project-URL: Documentation, https://github.com/matheusfelipeog/filometro/tree/master#documentação
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: filometro Version: 1.2.0 Summary: Obtenha os dados
+Metadata-Version: 2.1 Name: filometro Version: 1.2.1 Summary: Obtenha os dados
 dos postos de vacinaÃ§Ã£o da covid-19 em SÃ£o Paulo Home-page: https://
 github.com/matheusfelipeog/filometro Author: Matheus Felipe Author-email:
 matheusfelipeog@protonmail.com License: MIT License Project-URL: Bug Tracker,
 https://github.com/matheusfelipeog/filometro/issues Project-URL: Documentation,
 https://github.com/matheusfelipeog/filometro/tree/master#documentaÃ§Ã£o
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-
```

### Comparing `filometro-1.2.0/setup.py` & `filometro-1.2.1/setup.py`

 * *Files identical despite different names*

