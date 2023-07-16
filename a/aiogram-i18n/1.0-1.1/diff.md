# Comparing `tmp/aiogram_i18n-1.0.tar.gz` & `tmp/aiogram_i18n-1.1.tar.gz`

## Comparing `aiogram_i18n-1.0.tar` & `aiogram_i18n-1.1.tar`

### file list

```diff
@@ -1,28 +1,42 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/py.typed
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/.github/workflows/python-package-tests.yml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/__main__.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/context.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/lazy_proxy.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/cores/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/cores/babel_core.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/cores/base.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/cores/fluent_compile_core.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/cores/fluent_runtime_core.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/managers/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/managers/base.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/managers/const.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/managers/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/utils/__init__.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/utils/fluent_stub.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/aiogram_i18n/utils/keyboard.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/examples/mre.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/examples/locales/en/LC_MESSAGES/mybot.ftl
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/examples/locales/uk/LC_MESSAGES/mybot.ftl
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/.gitignore
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/README.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/pyproject.toml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 aiogram_i18n-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/.github/workflows/python-package-tests.yml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/__main__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/context.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/exceptions.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/py.typed
+-rw-r--r--   0        0        0    22198 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/types.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/cores/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/cores/base.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/cores/fluent_compile_core.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/cores/fluent_runtime_core.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/cores/gnu_text_core.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/lazy/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/lazy/factory.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/lazy/proxy.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/managers/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/managers/base.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/managers/const.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/managers/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/fluent_extract/__init__.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/fluent_extract/models.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/fluent_extract/parser.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/fluent_stub/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/aiogram_i18n/utils/fluent_stub/visitor.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/examples/mre.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/examples/stub.pyi
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/examples/locales/en/LC_MESSAGES/mybot.ftl
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/examples/locales/uk/LC_MESSAGES/mybot.ftl
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/conftest.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/test_cores.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/data/locales/en/LC_MESSAGES/mybot.ftl
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/data/locales/en/LC_MESSAGES/mybot.mo
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/data/locales/uk/LC_MESSAGES/mybot.ftl
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/tests/data/locales/uk/LC_MESSAGES/mybot.mo
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/.gitignore
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/pyproject.toml
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aiogram_i18n-1.1/PKG-INFO
```

### Comparing `aiogram_i18n-1.0/.github/workflows/python-package-tests.yml` & `aiogram_i18n-1.1/.github/workflows/python-package-tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Python package
+name: Test
 
 on:
   push:
-    branches: [ "master" ]
+    branches: [ "master" , "dev" ]
   pull_request:
-    branches: [ "master" ]
+    branches: [ "master" , "dev" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
+
+    - name: Upgrade pip
+      run: python -m pip install --upgrade pip
     - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+      run: pip install .[test]
+
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
```

### Comparing `aiogram_i18n-1.0/.github/workflows/python-publish.yml` & `aiogram_i18n-1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiogram_i18n-1.0/aiogram_i18n/context.py` & `aiogram_i18n-1.1/aiogram_i18n/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from contextlib import contextmanager
 from functools import partial
-from typing import Dict, Any, Generator
+from typing import Dict, Any, Generator, Callable
 
 from aiogram.utils.mixins import ContextInstanceMixin
 
 from aiogram_i18n.cores.base import BaseCore
 from aiogram_i18n.managers.base import BaseManager
 
 
 class I18nContext(ContextInstanceMixin["I18nContext"]):
     locale: str
     core: BaseCore[Any]
     manager: BaseManager
     data: Dict[str, Any]
-    key_sep: str
+    key_separator: str
 
     def __init__(
-            self,
-            locale: str, core: BaseCore[Any],
-            manager: BaseManager, data: Dict[str, Any],
-            key_sep: str = "-"
+        self,
+        locale: str, core: BaseCore[Any],
+        manager: BaseManager, data: Dict[str, Any],
+        key_separator: str = "-"
     ) -> None:
         self.locale = locale
         self.core = core
         self.manager = manager
         self.data = data
-        self.key_sep = key_sep
+        self.key_separator = key_separator
 
-    def get(self, key: str, **kwargs: Any) -> str:
-        return self.core.get(locale=self.locale, key=key, **kwargs)
+    def get(self, key: str, /, **kwargs: Any) -> str:
+        return self.core.get(key, locale=self.locale, **kwargs)
 
-    async def set_locale(self, locale: str) -> None:
-        await self.manager.set_locale(
-            locale=locale,
+    async def set_locale(self, locale: str, **kwargs: Any) -> None:
+        await self.manager.set_locale_mixin.call(
+            locale,
             core=self.core,
             manager=self.manager,
-            data=self.data
+            **self.data, **kwargs
         )
         self.locale = locale
 
-    def __getattr__(self, item: str) -> partial:
-        return partial(self.get, key=item.replace("_", self.key_sep))
+    def __getattr__(self, item: str) -> Callable[..., str]:
+        return partial(self.get, item.replace("_", self.key_separator))
 
     @contextmanager
-    def with_locale(self, locale: str) -> Generator["I18nContext", None, None]:
+    def use_locale(self, locale: str) -> Generator["I18nContext", None, None]:
         old_locale = self.locale
         self.locale = locale
         try:
             yield self
         finally:
             self.locale = old_locale
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/middleware.py` & `aiogram_i18n-1.1/aiogram_i18n/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,62 @@
-from collections import UserString
-from json import dumps, JSONEncoder
-from typing import Callable, Dict, Any, Awaitable, Optional, Sequence
+from typing import Callable, Dict, Any, Awaitable, Optional
 
-from aiogram import Dispatcher, BaseMiddleware, Bot
+from aiogram import Dispatcher, BaseMiddleware
 from aiogram.types import TelegramObject
 
 from aiogram_i18n.context import I18nContext
 from aiogram_i18n.cores.base import BaseCore
 from aiogram_i18n.managers.base import BaseManager
 from aiogram_i18n.managers.fsm import FSMManager
 
 
-def default(default_dump: Callable[..., str]) -> Callable[..., str]:
-    def serialize_lazy(obj: Any) -> str:
-        if isinstance(obj, UserString):
-            return obj.data
-        return default_dump(obj)
-
-    return serialize_lazy
-
-
-def on_startup(bots: Sequence[Bot]) -> None:
-    def_enc = JSONEncoder(default=default(dumps))
-    for bot in bots:
-        if bot.session.json_dumps is dumps:
-            bot.session.json_dumps = def_enc.encode
-        else:
-            bot.session.json_dumps = default(bot.session.json_dumps)
-
-
 class I18nMiddleware(BaseMiddleware):
     core: BaseCore[Any]
     manager: BaseManager
     context_key: str
     locale_key: str
     middleware_key: str
     default_locale: str
-    key_sep: str
+    key_separator: str
 
     def __init__(
         self,
         core: BaseCore[Any],
         manager: Optional[BaseManager] = None,
         context_key: str = "i18n",
         locale_key: str = "locale",
         middleware_key: str = "i18n_middleware",
         default_locale: str = "en",
-        key_sep: str = "-"
+        key_separator: str = "-"
     ) -> None:
         self.core = core
-        if manager is None:
-            manager = FSMManager(default_locale=default_locale, key=locale_key)
-        self.manager = manager
+        self.manager = manager or FSMManager(default_locale=default_locale, key=locale_key)
         self.context_key = context_key
         self.locale_key = locale_key
         self.middleware_key = middleware_key
         self.default_locale = default_locale
-        self.key_sep = key_sep
+        self.key_separator = key_separator
 
     def setup(self, dispatcher: Dispatcher) -> None:
         dispatcher.update.outer_middleware.register(self)
         dispatcher.startup.register(self.core.startup)
         dispatcher.shutdown.register(self.core.shutdown)
-        dispatcher.startup.register(on_startup)
 
     async def __call__(
         self,
         handler: Callable[[TelegramObject, Dict[str, Any]], Awaitable[Any]],
         event: TelegramObject,
         data: Dict[str, Any]
     ) -> Any:
         locale = await self.manager.get_locale(event=event, data=data)
-
-        data[self.context_key] = I18nContext(
+        data[self.context_key] = context = I18nContext(
             locale=locale,
             core=self.core,
             manager=self.manager,
             data=data,
-            key_sep=self.key_sep
+            key_separator=self.key_separator
         )
         data[self.locale_key] = locale
         data[self.middleware_key] = self
 
-        I18nContext.set_current(data[self.context_key])
+        I18nContext.set_current(context)
         return await handler(event, data)
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/cores/babel_core.py` & `aiogram_i18n-1.1/aiogram_i18n/cores/gnu_text_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from gettext import GNUTranslations
 from typing import Dict, Any
 
 from aiogram_i18n.cores.base import BaseCore
 
 
-class BabelCore(BaseCore[GNUTranslations]):
+class GNUTextCore(BaseCore[GNUTranslations]):
     def __init__(
         self, *,
         path: str,
         default_locale: str = "en"
     ) -> None:
         super().__init__()
         self.path = path
@@ -26,10 +26,10 @@
             trans = translations[locale] = GNUTranslations()
             for path in paths:
                 with open(path, "rb") as fp:
                     trans._parse(fp=fp) # noqa
 
         return translations
 
-    def get(self, locale: str, key: str, *args: Any, **kwargs: Any) -> str:
+    def get(self, key: str, /, locale: str, **kwargs: Any) -> str:
         translator = self.get_translator(locale=locale)
-        return translator.gettext(key).format(*args, **kwargs)
+        return translator.gettext(key).format(**kwargs)
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/cores/base.py` & `aiogram_i18n-1.1/aiogram_i18n/cores/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 import os
 from abc import abstractmethod, ABC
 from typing import List, Dict, Optional, Any, Tuple, TypeVar, Generic
+from aiogram_i18n.exceptions import NoTranslateFileExistsError, NoLocalesFoundError, NoLocalesError
 
 
 Translator = TypeVar("Translator")
 
 
 class BaseCore(Generic[Translator], ABC):
     default_locale: str
     locales: Dict[str, Translator]
 
     def __init__(self) -> None:
         self.locales = {}
 
     @abstractmethod
-    def get(self, locale: str, key: str, *args: Any, **kwargs: Any) -> str:
+    def get(self, key: str, /, locale: str, **kwargs: Any) -> str:
         ...
 
     def get_translator(self, locale: str) -> Translator:
         if locale not in self.locales:
             locale = self.default_locale
         return self.locales[locale]
 
     async def startup(self) -> None:
         self.locales.update(self.find_locales())
 
     async def shutdown(self, *args: Any, **kwargs: Any) -> None:
-        ...
+        self.locales.clear()
 
     @staticmethod
     def _extract_locales(path: str) -> List[str]:
         if "{locale}" in path:
             path = path.split("{locale}")[0]
-        return [p for p in os.listdir(path) if os.path.isdir(os.path.join(path, p))]
+        locales: List[str] = []
+        for file_path in os.listdir(path):
+            if os.path.isdir(os.path.join(path, file_path)):
+                locales.append(file_path)
+        if not locales:
+            raise NoLocalesFoundError(locales=["..."], path=path)
+        return locales
 
     @staticmethod
     def _find_locales(path: str, locales: List[str], ext: Optional[str] = None) -> Dict[str, List[str]]:
+        if not locales:
+            raise NoLocalesError
         paths: Dict[str, List[str]] = {}
         if "{locale}" not in path:
             path = os.path.join(path, "{locale}")
         for locale in locales:
             paths[locale] = []
             locale_path = path.format(locale=locale)
             for obj in os.listdir(locale_path):
                 if ext is not None:
                     if not obj.endswith(ext):
                         continue
                 obj_path = os.path.join(locale_path, obj)
                 if not os.path.isfile(obj_path):
                     continue
                 paths[locale].append(obj_path)
+            if not paths[locale]:
+                raise NoTranslateFileExistsError(ext=ext, locale_path=locale_path)
+        if not paths:
+            raise NoLocalesFoundError(locales=locales, path=path)
         return paths
 
     @abstractmethod
     def find_locales(self) -> Dict[str, Translator]:
         ...
 
     @property
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/cores/fluent_compile_core.py` & `aiogram_i18n-1.1/aiogram_i18n/cores/fluent_compile_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from typing import Dict, Callable, Optional, Any, cast
 
+from aiogram_i18n.exceptions import NoModuleError, KeyNotFound
+
 try:
     from fluent_compiler.bundle import FluentBundle  # type: ignore[import]
 except ImportError:
-    raise ImportError(
-        "FluentCompileCore can be used only when fluent_compiler installed\n"
-        "Just install fluent_compiler (`pip install fluent_compiler`)"
-    )
+    raise NoModuleError(name="FluentCompileCore", module_name="fluent_compiler")
 
 from aiogram_i18n.cores.base import BaseCore
 
 
 class FluentCompileCore(BaseCore[FluentBundle]):
     def __init__(
-        self,
-        path: str,
-        default_locale: str = "en",
-        use_isolating: bool = True,
-        functions: Optional[Dict[str, Callable[..., Any]]] = None
+            self,
+            path: str,
+            default_locale: str = "en",
+            use_isolating: bool = True,
+            functions: Optional[Dict[str, Callable[..., Any]]] = None,
+            raise_key_error: bool = True
     ) -> None:
         super().__init__()
         self.path = path
         self.use_isolating = use_isolating
         self.functions = functions
         self.default_locale = default_locale
+        self.raise_key_error = raise_key_error
 
-    def get(self, locale: str, key: str, **kwargs: Any) -> str:  # type: ignore[override]
+    def get(self, key: str, /, locale: str, **kwargs: Any) -> str:
         translator: FluentBundle = self.get_translator(locale=locale)
-        text, errors = translator.format(message_id=key, args=kwargs)
+        try:
+            text, errors = translator.format(message_id=key, args=kwargs)
+        except KeyError:
+            if self.raise_key_error:
+                raise KeyNotFound(key)
+            return key
         if errors:
             raise ValueError("\n".join(errors))
         return cast(str, text)  # 'cause fluent_compiler type-ignored
 
     def find_locales(self) -> Dict[str, FluentBundle]:
         """
         Load all compiled locales from path
 
         :return: dict with locales
         """
         translations: Dict[str, FluentBundle] = {}
         locales = self._extract_locales(self.path)
-        for locale, paths in self._find_locales(self.path, locales, ".flt").items():
+        for locale, paths in self._find_locales(self.path, locales, ".ftl").items():
             texts = []
             for path in paths:
                 with open(path, "r", encoding="utf8") as fp:
                     texts.append(fp.read())
             translations[locale] = FluentBundle.from_string(
                 text="\n".join(texts), locale=locale,
                 use_isolating=self.use_isolating,
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/cores/fluent_runtime_core.py` & `aiogram_i18n-1.1/aiogram_i18n/cores/fluent_runtime_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from typing import Dict, Callable, Optional, Any, cast
 
+from aiogram_i18n.exceptions import NoModuleError, KeyNotFound
+
 try:
     from fluent.runtime import FluentBundle, FluentResource
 except ImportError:
-    raise ImportError(
-        "FluentRuntimeCore can be used only when fluent.runtime installed\n"
-        "Just install fluent.runtime (`pip install fluent.runtime`)"
-    )
+    raise NoModuleError(name="FluentRuntimeCore", module_name="fluent.runtime")
 
 from aiogram_i18n.cores.base import BaseCore
 
 
 class FluentRuntimeCore(BaseCore[FluentBundle]):
     def __init__(
         self,
         path: str, default_locale: str = "en",
         use_isolating: bool = True,
         functions: Optional[Dict[str, Callable[..., Any]]] = None,
-        pre_compile: bool = True
+        pre_compile: bool = True,
+        raise_key_error: bool = True
     ) -> None:
         super().__init__()
         self.path = path
         self.use_isolating = use_isolating
         self.functions = functions
         self.default_locale = default_locale
-        self.pre_compile = pre_compile
+        self.pre_compile = pre_compile,
+        self.raise_key_error = raise_key_error
 
-    def get(self, locale: str, key: str, **kwargs: Any) -> str:  # type: ignore[override]
+    def get(self, key: str, /, locale: str, **kwargs: Any) -> str:
         translator: FluentBundle = self.get_translator(locale=locale)
         message = translator.get_message(message_id=key)
         if message.value is None:
-            raise ValueError("key", key, "not find")
+            if self.raise_key_error:
+                raise KeyNotFound(key)
+            return key
         text, errors = translator.format_pattern(
             pattern=message.value,
             args=kwargs
         )
         if errors:
             raise errors[0]
         return cast(str, text)
```

### Comparing `aiogram_i18n-1.0/aiogram_i18n/managers/fsm.py` & `aiogram_i18n-1.1/aiogram_i18n/managers/fsm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict, Any, Optional
+
 from aiogram.fsm.context import FSMContext
 from aiogram.types import TelegramObject
 
 from aiogram_i18n.managers.base import BaseManager
 
 
 class FSMManager(BaseManager):
@@ -20,10 +21,9 @@
             locale = fsm_data.get(self.key, None)
         if locale is None:
             locale = self.default_locale
             if state:
                 await state.update_data(data={self.key: locale})
         return locale
 
-    async def set_locale(self, locale: str, *args: Any, **kwargs: Any) -> None:
-        state: FSMContext = kwargs["data"].get("state")
+    async def set_locale(self, locale: str, state: FSMContext) -> None:
         await state.update_data(data={self.key: locale})
```

### Comparing `aiogram_i18n-1.0/examples/mre.py` & `aiogram_i18n-1.1/examples/mre.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,53 +2,58 @@
 from contextlib import suppress
 from logging import basicConfig, INFO
 from typing import Any
 
 from aiogram import Router, Dispatcher, F, Bot
 from aiogram.enums import ParseMode
 from aiogram.filters import CommandStart
-from aiogram.types import ReplyKeyboardMarkup, Message
+from aiogram.types import Message
 
 from aiogram_i18n import I18nContext, LazyProxy, I18nMiddleware
 from aiogram_i18n.cores.fluent_runtime_core import FluentRuntimeCore
-from aiogram_i18n.utils.keyboard import KeyboardButton  # you should import the keyboard from here if you want to use LazyProxy
+from aiogram_i18n.types import (
+    ReplyKeyboardMarkup, KeyboardButton
+    # you should import mutable objects from here if you want to use LazyProxy in them
+)
+
 
 router = Router(name=__name__)
 rkb = ReplyKeyboardMarkup(
     keyboard=[
-        [KeyboardButton(text=LazyProxy(key="help"))]
+        [KeyboardButton(text=LazyProxy("help"))]  # or L.help()
     ], resize_keyboard=True
 )
 
 
 @router.message(CommandStart())
 async def cmd_start(message: Message, i18n: I18nContext) -> Any:
+    name = message.from_user.mention_html()
     return message.reply(
-        text=i18n.get("hello", user=message.from_user.full_name),
+        text=i18n.get("hello", user=name),  # or i18n.hello(user=name)
         reply_markup=rkb
     )
 
 
-@router.message(F.text == LazyProxy(key="help"))
+@router.message(F.text == LazyProxy("help"))
 async def cmd_help(message: Message) -> Any:
     return message.reply(text="-- " + message.text + " --")
 
 
 async def main() -> None:
     basicConfig(level=INFO)
     bot = Bot("42:ABC", parse_mode=ParseMode.HTML)
-    i18n = I18nMiddleware(
+    i18n_middleware = I18nMiddleware(
         core=FluentRuntimeCore(
             path="locales/{locale}/LC_MESSAGES"
         )
     )
 
     dp = Dispatcher()
     dp.include_router(router)
-    i18n.setup(dispatcher=dp)
+    i18n_middleware.setup(dispatcher=dp)
 
     await dp.start_polling(bot)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
```

### Comparing `aiogram_i18n-1.0/README.md` & `aiogram_i18n-1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 # aiogram_i18n
 
-FluentCompileCore:
+Installation:
+```pip install aiogram_i18n```
+
+To use FluentCompileCore:
 ```pip install fluent_compiler```
 
-FluentRuntimeCore:
+To use FluentRuntimeCore:
 ```pip install fluent.runtime```
 
 
 ```python
 import asyncio
 from contextlib import suppress
 from logging import basicConfig, INFO
 from typing import Any
 
 from aiogram import Router, Dispatcher, F, Bot
 from aiogram.enums import ParseMode
 from aiogram.filters import CommandStart
-from aiogram.types import ReplyKeyboardMarkup, Message
+from aiogram.types import Message
 
 from aiogram_i18n import I18nContext, LazyProxy, I18nMiddleware
 from aiogram_i18n.cores.fluent_runtime_core import FluentRuntimeCore
-from aiogram_i18n.utils.keyboard import KeyboardButton  # you should import the keyboard from here if you want to use LazyProxy
+from aiogram_i18n.types import (
+    ReplyKeyboardMarkup, KeyboardButton
+    # you should import mutable objects from here if you want to use LazyProxy in them
+)
 
 
 router = Router(name=__name__)
 rkb = ReplyKeyboardMarkup(
     keyboard=[
-        [KeyboardButton(text=LazyProxy(key="help"))]
+        [KeyboardButton(text=LazyProxy("help"))]  # or L.help()
     ], resize_keyboard=True
 )
 
 
 @router.message(CommandStart())
 async def cmd_start(message: Message, i18n: I18nContext) -> Any:
+    name = message.from_user.mention_html()
     return message.reply(
-        text=i18n.get("hello", user=message.from_user.full_name),
+        text=i18n.get("hello", user=name),  # or i18n.hello(user=name)
         reply_markup=rkb
     )
 
 
-@router.message(F.text == LazyProxy(key="help"))
+@router.message(F.text == LazyProxy("help"))
 async def cmd_help(message: Message) -> Any:
     return message.reply(text="-- " + message.text + " --")
 
 
 async def main() -> None:
     basicConfig(level=INFO)
     bot = Bot("42:ABC", parse_mode=ParseMode.HTML)
-    i18n = I18nMiddleware(
+    i18n_middleware = I18nMiddleware(
         core=FluentRuntimeCore(
             path="locales/{locale}/LC_MESSAGES"
         )
     )
 
     dp = Dispatcher()
     dp.include_router(router)
-    i18n.setup(dispatcher=dp)
+    i18n_middleware.setup(dispatcher=dp)
 
     await dp.start_polling(bot)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
-
 ```
```

### Comparing `aiogram_i18n-1.0/PKG-INFO` & `aiogram_i18n-1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,98 @@
 Metadata-Version: 2.1
 Name: aiogram_i18n
-Version: 1.0
+Version: 1.1
 Summary: small translation tools for aiogram
 Project-URL: Repository, https://github.com/RootShinobi/aiogram_i18n
 Author: RootShinobi
 License: MIT License
-Keywords: aiogram,api,asyncio,bot,fluent,framework,i18n,telegram,wrapper
+Keywords: aiogram,api,asyncio,bot,fluent,framework,gnutext,i18n,telegram,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiogram~=3.0.0b7
+Requires-Dist: click==8.1.4
+Provides-Extra: compiler
+Requires-Dist: fluent-compiler~=1.0; extra == 'compiler'
+Provides-Extra: runtime
+Requires-Dist: fluent-runtime~=0.4.0; extra == 'runtime'
+Provides-Extra: test
+Requires-Dist: flake8~=6.0.0; extra == 'test'
+Requires-Dist: pytest-asyncio~=0.21.1; extra == 'test'
+Requires-Dist: pytest-lazy-fixture~=0.6.3; extra == 'test'
+Requires-Dist: pytest~=7.4.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # aiogram_i18n
 
-FluentCompileCore:
+Installation:
+```pip install aiogram_i18n```
+
+To use FluentCompileCore:
 ```pip install fluent_compiler```
 
-FluentRuntimeCore:
+To use FluentRuntimeCore:
 ```pip install fluent.runtime```
 
 
 ```python
 import asyncio
 from contextlib import suppress
 from logging import basicConfig, INFO
 from typing import Any
 
 from aiogram import Router, Dispatcher, F, Bot
 from aiogram.enums import ParseMode
 from aiogram.filters import CommandStart
-from aiogram.types import ReplyKeyboardMarkup, Message
+from aiogram.types import Message
 
 from aiogram_i18n import I18nContext, LazyProxy, I18nMiddleware
 from aiogram_i18n.cores.fluent_runtime_core import FluentRuntimeCore
-from aiogram_i18n.utils.keyboard import KeyboardButton  # you should import the keyboard from here if you want to use LazyProxy
+from aiogram_i18n.types import (
+    ReplyKeyboardMarkup, KeyboardButton
+    # you should import mutable objects from here if you want to use LazyProxy in them
+)
 
 
 router = Router(name=__name__)
 rkb = ReplyKeyboardMarkup(
     keyboard=[
-        [KeyboardButton(text=LazyProxy(key="help"))]
+        [KeyboardButton(text=LazyProxy("help"))]  # or L.help()
     ], resize_keyboard=True
 )
 
 
 @router.message(CommandStart())
 async def cmd_start(message: Message, i18n: I18nContext) -> Any:
+    name = message.from_user.mention_html()
     return message.reply(
-        text=i18n.get("hello", user=message.from_user.full_name),
+        text=i18n.get("hello", user=name),  # or i18n.hello(user=name)
         reply_markup=rkb
     )
 
 
-@router.message(F.text == LazyProxy(key="help"))
+@router.message(F.text == LazyProxy("help"))
 async def cmd_help(message: Message) -> Any:
     return message.reply(text="-- " + message.text + " --")
 
 
 async def main() -> None:
     basicConfig(level=INFO)
     bot = Bot("42:ABC", parse_mode=ParseMode.HTML)
-    i18n = I18nMiddleware(
+    i18n_middleware = I18nMiddleware(
         core=FluentRuntimeCore(
             path="locales/{locale}/LC_MESSAGES"
         )
     )
 
     dp = Dispatcher()
     dp.include_router(router)
-    i18n.setup(dispatcher=dp)
+    i18n_middleware.setup(dispatcher=dp)
 
     await dp.start_polling(bot)
 
 
 if __name__ == "__main__":
     with suppress(KeyboardInterrupt):
         asyncio.run(main())
-
 ```
```

