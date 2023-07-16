# Comparing `tmp/t8s-0.1.8.tar.gz` & `tmp/t8s-0.1.9.tar.gz`

## Comparing `t8s-0.1.8.tar` & `t8s-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 t8s-0.1.8/.dockerignore
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 t8s-0.1.8/Dockerfile
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 t8s-0.1.8/constraints.txt
--rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 t8s-0.1.8/dockerize.sh
--rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 t8s-0.1.8/main.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.8/publish-to-pypi.md
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 t8s-0.1.8/smoke.py
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 t8s-0.1.8/test-all.sh
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 t8s-0.1.8/ts_01.csv
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 t8s-0.1.8/wfw-dev.sh
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 t8s-0.1.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.8/.vscode/launch.json
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-composite.md
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-singleton.md
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-strategy.md
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/composite-pattern.png
--rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/singleton-pattern.png
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/strategy-pattern.png
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/chain.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/composite.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 t8s-0.1.8/src/stubs/.gitkeep
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/__about__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/__init__.py
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/io.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/log_config.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts.py
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts_builder.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts_writer.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/test_build_from_file.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/test_to_parquet.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 t8s-0.1.8/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 t8s-0.1.8/README.md
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 t8s-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 t8s-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 t8s-0.1.9/.dockerignore
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 t8s-0.1.9/Dockerfile
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 t8s-0.1.9/constraints.txt
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 t8s-0.1.9/dockerize.sh
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 t8s-0.1.9/main.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.9/publish-to-pypi.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 t8s-0.1.9/pyrightconfig.json
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 t8s-0.1.9/smoke.py
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 t8s-0.1.9/test-all.sh
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 t8s-0.1.9/test-requirements.txt
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 t8s-0.1.9/wfw-dev.sh
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 t8s-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 t8s-0.1.9/.vscode/launch.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 t8s-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/dp-composite.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/dp-singleton.md
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/dp-strategy.md
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/img/composite-pattern.png
+-rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/img/singleton-pattern.png
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.9/docs/img/strategy-pattern.png
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 t8s-0.1.9/husky/README.md
+-rw-r--r--   0        0        0    64464 2020-02-02 00:00:00.000000 t8s-0.1.9/husky/add-commit.png
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 t8s-0.1.9/src/patterns/chain.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 t8s-0.1.9/src/patterns/composite.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 t8s-0.1.9/src/patterns/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 t8s-0.1.9/src/stubs/.gitkeep
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/__about__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/__init__.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/io.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/log_config.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/ts.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/ts_builder.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 t8s-0.1.9/src/t8s/ts_writer.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 t8s-0.1.9/tests/test_build_from_file.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 t8s-0.1.9/tests/test_to_parquet.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 t8s-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 t8s-0.1.9/README.md
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 t8s-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 t8s-0.1.9/PKG-INFO
```

### Comparing `t8s-0.1.8/Dockerfile` & `t8s-0.1.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/constraints.txt` & `t8s-0.1.9/constraints.txt`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/dockerize.sh` & `t8s-0.1.9/dockerize.sh`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/main.py` & `t8s-0.1.9/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     print(df_whith_nans)
     print('Tipos das colunas no Dataframe da Série Temporal:')
     for col in df_whith_nans.columns:
         for value in df_whith_nans[col]:
             print(col, '\t', value, type(value))
 
     # --------------------------------------------------------------------------------
-    
+
     # Verifica se a conversão para tipo Number das colunas é trivial ou se é necessário
     # fazer mapeamento de valores não numéricos, tais como, 'Bad', 'Missing', etc.
     numeric_columns: list[str] = list(df_whith_nans.columns[1:])
     all_problems = IO.check_convertion_to_float(numeric_columns, df_whith_nans)
     print('all_problems:', all_problems)
 
     # --------------------------------------------------------------------------------
@@ -178,13 +178,13 @@
     print('df_whith_nans:\n', df_whith_nans)
     print('Tipos das colunas no Dataframe da Série Temporal:')
     for col in df_whith_nans.columns:
         for value in df_whith_nans[col]:
             print(col, '\t', value, type(value))
 
     # --------------------------------------------------------------------------------
-    
+
 
 
     # --------------------------------------------------------------------------------
 
     # --------------------------------------------------------------------------------
```

### Comparing `t8s-0.1.8/publish-to-pypi.md` & `t8s-0.1.9/publish-to-pypi.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/smoke.py` & `t8s-0.1.9/smoke.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/.github/workflows/test.yml` & `t8s-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/dp-composite.md` & `t8s-0.1.9/docs/dp-composite.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/dp-singleton.md` & `t8s-0.1.9/docs/dp-singleton.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/dp-strategy.md` & `t8s-0.1.9/docs/dp-strategy.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/img/composite-pattern.png` & `t8s-0.1.9/docs/img/composite-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/img/singleton-pattern.png` & `t8s-0.1.9/docs/img/singleton-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/docs/img/strategy-pattern.png` & `t8s-0.1.9/docs/img/strategy-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/src/patterns/chain.py` & `t8s-0.1.9/src/patterns/chain.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/src/patterns/composite.py` & `t8s-0.1.9/src/patterns/composite.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/src/t8s/io.py` & `t8s-0.1.9/src/t8s/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         IO.__check_csv_schema(csv_file_list)
         result = True
 
         return result
 
     # Quando estamos lendo de arquivos CSV podem aparecer valores que não tem uma
     # representação valida para NaN e portanto atrapalha o processo de inferência
-    # de tipo do Pandas. Assim tokens como  'Configure', 'Bad' e 'NotNamber', 
+    # de tipo do Pandas. Assim tokens como  'Configure', 'Bad' e 'NotNamber',
     # por exemplo, devem ser substituidos por NaN (np.na do numpy) para que possamos
-    # fazer a conversão para float. O método check_convertion_to_float() faz isso.  
+    # fazer a conversão para float. O método check_convertion_to_float() faz isso.
     @staticmethod
     def __check_convertion_to_float(col_name:str, cols: pd.Series) -> tuple[str, list[str]]:
         assert isinstance(cols, pd.Series)
         not_float_values = []
         # Definindo a expressão regular para identificar números de ponto flutuante
         # padrao = r'[+-]?(\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?'
         padrao = get_numeric_regex()
         # Use o método items() para iterar sobre os itens da série
         for idx, valor in cols.items():
             print(idx, valor)
             if (not re.match(padrao, str(valor))) and (not pd.isna(valor)):
                 if isinstance(valor, str):
-                    if valor not in ['NaN', '-NaN', '-nan', 'nan', '<NA>', 'N/A', 
+                    if valor not in ['NaN', '-NaN', '-nan', 'nan', '<NA>', 'N/A',
                                      'NA', 'NULL', 'None', 'n/a', 'null']:
                         # print(idx, '\t', valor, 'não é uma representação valida para NaN')
                         not_float_values.append(valor)
                 else:
                     # print(idx, '\t', valor, 'não e um número valido e nem uma representação valida para NaN')
                     not_float_values.append(valor)
         if len(not_float_values) > 0:
@@ -129,26 +129,26 @@
     # ser obrigatoriamente '.csv' (em minusculo). Isto é uma convenção.
     # Além disso o arquivo deve existir e possuir na primira linha a lista
     # de nomes das colunas / campos (schema). A quintidade de elementos na
     # lista 'column_types' deve ser igual a quntidade de colunas no arquivo,
     # ou seja, deve ser igual ao tamanho da lista de nomes especificada na
     # primeira coluna do arquivo CSV.
     @staticmethod
-    def read_csv_file(path: Path, column_types: list[type], 
-            nan_values:list[str] = [], parse_dates: list[int] = [1], 
+    def read_csv_file(path: Path, column_types: list[type],
+            nan_values:list[str] = [], parse_dates: list[int] = [1],
             date_format:str = 'AAAA-MM-DD HH:MM:SS') -> pd.DataFrame:
         for value in column_types:
             assert isinstance(value, type), f'Erro: {value} não é um tipo válido'
 
         # Define o conversor para cada tipo de coluna
         # Crio um dicionário com os conversores e tipos de colunas
         converters_tmp = {
             f'{i}': column_types[i] for i in range(len(column_types))
         }
-        
+
         # print('converters:', converters_tmp, type(converters_tmp))
         result = pd.read_csv(filepath_or_buffer = path, sep=',', delimiter=None,
             header='infer', dtype=None, engine='c', converters=converters_tmp,
             na_values=nan_values, keep_default_na=True, na_filter=True, verbose=True,
             skip_blank_lines=True, parse_dates=parse_dates, date_format=date_format,
             dayfirst=False, cache_dates=False, compression='infer', thousands=None,
             decimal='.', quotechar='"', # Not Supported: lineterminator=os.linesep
@@ -157,15 +157,15 @@
             low_memory=True, memory_map=False, dtype_backend='numpy_nullable')
         converters =  {}
         if len(converters_tmp) > 0:
             # TODO: Verificar como converter a primeira coluna que é Timestamp e é index.
             for idx, col in enumerate(result.columns[1:]):
                 converters[col] = converters_tmp[str(idx)]
             print('converters:', converters, type(converters))
-        
+
         numeric_columns = list(result.columns[1:])
         all_problems_on_data = IO.check_convertion_to_float(numeric_columns, result)
         for key, value in converters.items():
             assert isinstance(value, type), f'Erro: {value} não é um tipo válido para coluna {key}'
             # Mapeia os tokens inválidos para NaN
             if (key in all_problems_on_data.keys()):
                 result[key] = result[key].replace(to_replace=all_problems_on_data[key], value=np.nan)
@@ -189,19 +189,20 @@
         # como "AAAA-MM-DDTHH:MM:SS", onde "AAAA" representa o ano com quatro dígitos,
         # "MM" representa o mês com dois dígitos, "DD" representa o dia com dois dígitos,
         # "T" é o separador entre a data e a hora, "HH" representa a hora com dois dígitos,
         # "MM" representa os minutos com dois dígitos e "SS" representa os segundos com
         # dois dígitos. No formato "2022-11-29 10:40:55", a data e a hora são separadas
         # por um espaço em vez do caractere "T", mas ainda segue o padrão ISO 8601
         # para representação de datas e horas.
-        df.to_csv(path, sep=',', na_rep='NaN', float_format=None, 
-            header=True, index=True, index_label=None, mode='w', 
-            encoding='utf-8', compression=None, quoting=csv.QUOTE_MINIMAL, 
-            quotechar='"', lineterminator=os.linesep, chunksize=None, 
-            date_format=None, doublequote=True, escapechar=None, 
+        # Veja: https://www.w3.org/TR/NOTE-datetime
+        df.to_csv(path, sep=',', na_rep='NaN', float_format=None,
+            header=True, index=True, index_label=None, mode='w',
+            encoding='utf-8', compression=None, quoting=csv.QUOTE_MINIMAL,
+            quotechar='"', lineterminator=os.linesep, chunksize=None,
+            date_format=None, doublequote=True, escapechar=None,
             decimal='.', errors='strict', storage_options=None)
 
 
 if __name__ == "__main__":
     # Lê o arquivo CSV e gera um Dataframe com os tipos de dados corretos informados
     # na lista column_types que deve corresponder na mesma ordem com as colunas.
     path = Path('ts_01.csv')
@@ -209,8 +210,8 @@
     column_types: list[type] = [np.float32, np.float32]
     df_whith_nans = IO.read_csv_file(path, column_types)
     print('df_whith_nans:\n', df_whith_nans)
     print('Tipos das colunas no Dataframe da Série Temporal:')
     for col in df_whith_nans.columns:
         for value in df_whith_nans[col]:
             print(col, '\t', value, type(value))
-        print('-----------------------------------------------')
+        print('-----------------------------------------------')
```

### Comparing `t8s-0.1.8/src/t8s/log_config.py` & `t8s-0.1.9/src/t8s/log_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 
 class LogConfig(metaclass=LogConfigMeta):
     def __init__(self) -> None:
         self.logger = None
         self.initialize_logger(level=logging.DEBUG)
 
-    def initialize_logger(self, level=logging.DEBUG):
+    def initialize_logger(self, level=logging.DEBUG, log_file: str = 'logs/timeseries.log'):
         my_global_logger = logging.getLogger(__name__)
         my_global_logger.setLevel(level)
         # logger_handler = RotatingFileHandler('timeseries.log', maxBytes=1_000_000, backupCount=10)
-        logger_handler = logging.FileHandler('timeseries.log', mode='w')
+        logger_handler = logging.FileHandler(log_file, mode='w')
         # logger_handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(filename)s - %(funcName)s | %(message)s")) #"%(asctime)s - %(name)s - %(levelname)s - %(filename)s:%(funcName)s(%(lineno)d) - %(message)s"
         logger_handler.setFormatter(
             logging.Formatter("%(levelname)s - %(filename)s - %(funcName)s | %(message)s")
         )  # "%(asctime)s - %(name)s - %(levelname)s - %(filename)s:%(funcName)s(%(lineno)d) - %(message)s"
         my_global_logger.handlers.clear()
         my_global_logger.addHandler(logger_handler)
         self.logger = my_global_logger
```

### Comparing `t8s-0.1.8/src/t8s/ts.py` & `t8s-0.1.9/src/t8s/ts.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/src/t8s/ts_builder.py` & `t8s-0.1.9/src/t8s/ts_builder.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/src/t8s/ts_writer.py` & `t8s-0.1.9/src/t8s/ts_writer.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/tests/test_build_from_file.py` & `t8s-0.1.9/tests/test_build_from_file.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/tests/test_to_parquet.py` & `t8s-0.1.9/tests/test_to_parquet.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/LICENSE.txt` & `t8s-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/README.md` & `t8s-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/pyproject.toml` & `t8s-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `t8s-0.1.8/PKG-INFO` & `t8s-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t8s
-Version: 0.1.8
+Version: 0.1.9
 Project-URL: Documentation, https://github.com/joao-parana/t8s#README.md
 Project-URL: Issues, https://github.com/joao-parana/t8s/issues
 Project-URL: Source, https://github.com/joao-parana/t8s
 Author-email: João Antonio Ferreira <joao.parana@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

