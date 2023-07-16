# Comparing `tmp/dataclass_mapper-1.7.2.tar.gz` & `tmp/dataclass_mapper-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_mapper-1.7.2.tar", max compression
+gzip compressed data, was "dataclass_mapper-1.8.0.tar", max compression
```

## Comparing `dataclass_mapper-1.7.2.tar` & `dataclass_mapper-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
--rw-r--r--   0        0        0     1052 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/LICENSE.md
--rw-r--r--   0        0        0     5722 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/README.rst
--rw-r--r--   0        0        0      490 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/__init__.py
--rw-r--r--   0        0        0      501 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/__init__.py
--rw-r--r--   0        0        0      487 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/assignment.py
--rw-r--r--   0        0        0     1183 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/function.py
--rw-r--r--   0        0        0      752 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/list.py
--rw-r--r--   0        0        0      780 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/recursive.py
--rw-r--r--   0        0        0      272 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/simple.py
--rw-r--r--   0        0        0      559 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/assignments/utils.py
--rw-r--r--   0        0        0     3962 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/classmeta.py
--rw-r--r--   0        0        0     2285 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/enum.py
--rw-r--r--   0        0        0     2581 2023-05-28 13:19:19.836317 dataclass_mapper-1.7.2/dataclass_mapper/fieldmeta.py
--rw-r--r--   0        0        0    12764 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/mapper.py
--rw-r--r--   0        0        0     7876 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/mapping_method.py
--rw-r--r--   0        0        0      391 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/namespace.py
--rw-r--r--   0        0        0        0 2023-05-28 13:19:19.840317 dataclass_mapper-1.7.2/dataclass_mapper/py.typed
--rw-r--r--   0        0        0     1683 2023-05-28 13:20:19.245045 dataclass_mapper-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     6593 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.2/setup.py
--rw-r--r--   0        0        0     6664 1970-01-01 00:00:00.000000 dataclass_mapper-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/LICENSE.md
+-rw-r--r--   0        0        0     5857 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/README.rst
+-rw-r--r--   0        0        0      490 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/__init__.py
+-rw-r--r--   0        0        0      498 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/assignment.py
+-rw-r--r--   0        0        0     1194 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/function.py
+-rw-r--r--   0        0        0      750 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/list.py
+-rw-r--r--   0        0        0      806 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/recursive.py
+-rw-r--r--   0        0        0      319 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/simple.py
+-rw-r--r--   0        0        0      570 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/utils.py
+-rw-r--r--   0        0        0      604 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/classmeta.py
+-rw-r--r--   0        0        0     2134 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/code_generator.py
+-rw-r--r--   0        0        0     2285 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/enum.py
+-rw-r--r--   0        0        0      400 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/__init__.py
+-rw-r--r--   0        0        0     3008 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/base.py
+-rw-r--r--   0        0        0     1565 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/dataclasses.py
+-rw-r--r--   0        0        0     3545 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v1.py
+-rw-r--r--   0        0        0     3652 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v2.py
+-rw-r--r--   0        0        0      238 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/utils.py
+-rw-r--r--   0        0        0    12792 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/mapper.py
+-rw-r--r--   0        0        0     7410 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/mapping_method.py
+-rw-r--r--   0        0        0      391 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/namespace.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/py.typed
+-rw-r--r--   0        0        0     1187 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/utils.py
+-rw-r--r--   0        0        0     1747 2023-07-16 19:32:13.874320 dataclass_mapper-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6764 1970-01-01 00:00:00.000000 dataclass_mapper-1.8.0/setup.py
+-rw-r--r--   0        0        0     6792 1970-01-01 00:00:00.000000 dataclass_mapper-1.8.0/PKG-INFO
```

### Comparing `dataclass_mapper-1.7.2/LICENSE.md` & `dataclass_mapper-1.8.0/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Jakob Kogler
+Copyright 2022-2023 Jakob Kogler
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `dataclass_mapper-1.7.2/README.rst` & `dataclass_mapper-1.8.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,19 @@
 Features
 --------
 
 The current version has support for:
 
 * Python's ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples
 * Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_
-* Pydantic models:  see `Pydanitc support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
+* Pydantic models:  see `Pydantic support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
 * Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_
 
+Contributing
+------------
+
+See `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/CONTRIBUTING.rst>`_.
+
 License
 -------
 
 The project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.
```

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/assignments/function.py` & `dataclass_mapper-1.8.0/dataclass_mapper/assignments/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inspect import signature
 from typing import Any, Callable, Dict, Union, cast
 from uuid import uuid4
 
-from ..fieldmeta import FieldMeta
+from ..implementations.base import FieldMeta
 
 CallableWithMax1Parameter = Union[Callable[[], Any], Callable[[Any], Any]]
 
 
 class FunctionAssignment:
     def __init__(
         self, function: CallableWithMax1Parameter, target: FieldMeta, methods: Dict[str, Callable], target_cls_name: str
```

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/assignments/recursive.py` & `dataclass_mapper-1.8.0/dataclass_mapper/assignments/recursive.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,13 @@
         return is_mappable_to(self.source.type, self.target.type) and not (
             self.source.allow_none and self.target.disallow_none
         )
 
     def right_side(self) -> str:
         return self._get_map_func(get_var_name(self.source), target_cls=self.target.type, extra_str=self.extra_str())
 
-    def extra_str(self) -> str:
-        return f'extra.get("{self.target.name}", {{}})'
+    def extra_str(self, default: str = "{}") -> str:
+        return f'extra.get("{self.target.name}", {default})'
 
     def _get_map_func(self, name: str, target_cls: Any, extra_str: str) -> str:
         func_name = get_map_to_func_name(target_cls)
         return f"{name}.{func_name}({extra_str})"
```

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/assignments/utils.py` & `dataclass_mapper-1.8.0/dataclass_mapper/assignments/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from ..fieldmeta import FieldMeta
+from ..implementations.base import FieldMeta
 
 
 def get_var_name(fieldmeta: FieldMeta) -> str:
     return f"self.{fieldmeta.name}"
 
 
 def is_mappable_to(SourceCls: Any, TargetCls: Any) -> bool:
```

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/enum.py` & `dataclass_mapper-1.8.0/dataclass_mapper/enum.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/mapper.py` & `dataclass_mapper-1.8.0/dataclass_mapper/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,27 +108,27 @@
     :param mapping: An optional dictionary which which it's possible to describe how each field in the target
         class gets initialized.
         Fields that are not specified will be mapped automatically.
         Every single field in the target class must have some mapping (in order to not forget about a field),
         either a default mapping (if the field names match), or an explicit mapping definition with this
         `mapping` parameter.
 
-        - ``{"x": "y"}`` means, that the field ``x`` of the target object will have the value of the
-          ``y`` fields in the target object.
+        - ``{"x": "y"}`` means, that the field ``x`` of the target object will be initialized with the value of the
+          ``y`` fields in the source object.
         - ``{"x": lambda: 42}`` means, that the field ``x`` will be initialized with the value 42.
         - ``{"x": lambda self: self.x + 1}`` means, that the field ``x`` will be initialized with the
           incremented value ``x`` of the source object.
         - ``{"x": USE_DEFAULT}`` (deprecated) means, nothing is mapped to the field ``x``, it will just be
           initialized with the default value / factory of that field.
         - ``{"x": IGNORE_MISSING_MAPPING}`` (deprecated) means, nothing is mapped to the field ``x``, it will just be
           initialized with the default value / factory of that field.
         - ``{"x": init_with_default()}`` means, nothing is mapped to the field ``x``, it will just be
           initialized with the default value / factory of that field.
-        - ``{"x": assume_not_none("y")}`` means, that the target field ``x`` will have the value of the
-          ``y`` source field, and the library will assume that the source field might be optional.
+        - ``{"x": assume_not_none("y")}`` means, that the target field ``x`` will be initialized with the value of the
+          ``y`` source field, and the library will assume that the source field is not ``None``.
           If no source field name is given, it will additionally assume that the source field is also called ``x``.
         - ``{"x": provide_with_extra()}`` means, that you don't fill this field with any field of the source class,
           but with the extra dictionary given by the `map_to` method.
     """
 
     namespace = get_namespace()
```

### Comparing `dataclass_mapper-1.7.2/dataclass_mapper/mapping_method.py` & `dataclass_mapper-1.8.0/dataclass_mapper/mapping_method.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Callable, Dict, List, Optional, Type, Union
 
+from . import code_generator as cg
 from .assignments import (
     Assignment,
     CallableWithMax1Parameter,
     FunctionAssignment,
     ListRecursiveAssignment,
     RecursiveAssignment,
     SimpleAssignment,
     get_var_name,
 )
-from .classmeta import ClassMeta, DataclassType
-from .fieldmeta import FieldMeta
+from .implementations.base import ClassMeta, FieldMeta
 
 
 class Spezial(Enum):
     USE_DEFAULT = auto()
     IGNORE_MISSING_MAPPING = auto()
 
 
@@ -72,44 +72,32 @@
         (for Optional fields in Pydantic classes)
     :param only_if_not_None: don't assign the right side, if the value is None
         (for Optional -> non-Optional mappings with defaults in target fields)
     :param if_None: only assign the right side if it is not None (for Optional, recursive fields),
         otherwise set it to None
     """
 
-    only_if_set: bool = False
     only_if_not_None: bool = False
     if_None: bool = False
 
     @classmethod
     def from_Metas(
         cls, source_cls: ClassMeta, target_cls: ClassMeta, source: FieldMeta, target: FieldMeta
     ) -> "AssignmentOptions":
-        # maintain Pydantic's unset property
-        only_if_set = (
-            source.allow_none
-            and target.allow_none
-            and not target.required
-            and source_cls._type == target_cls._type == DataclassType.PYDANTIC
-        )
-        # TODO: what if the defaults of source/target are not just None?
-        # How to map `x: Optional[int] = Field(42)` to `x: Optional[int] = Field(15)`?
-
         # handle optional to non-optional mappings
         only_if_not_None = False
         if source.allow_none and target.disallow_none:
             if not target.required:
                 only_if_not_None = True
             else:
                 raise TypeError(f"{source} of '{source_cls.name}' cannot be converted to {target}")
 
         if_None = source.allow_none
 
         return cls(
-            only_if_set=only_if_set,
             only_if_not_None=only_if_not_None,
             if_None=if_None,
         )
 
 
 class MappingMethodSourceCode:
     """Source code of the mapping method"""
@@ -119,74 +107,72 @@
         RecursiveAssignment,
         ListRecursiveAssignment,
     ]
 
     def __init__(self, source_cls: ClassMeta, target_cls: ClassMeta) -> None:
         self.source_cls = source_cls
         self.target_cls = target_cls
-        self.lines = [
-            f'def convert(self, extra: dict) -> "{self.target_cls.name}":',
-            "    d = {}",
-        ]
+        self.function = cg.Function(
+            "convert",
+            args="self, extra: dict",
+            return_type=self.target_cls.name,
+            body=cg.Block(cg.Assignment(name="d", rhs="{}")),
+        )
         self.methods: Dict[str, Callable] = {}
 
     @classmethod
     def _get_asssigment(cls, target: FieldMeta, source: FieldMeta) -> Optional[Assignment]:
         for AssignmentCls in cls.AssignmentClasses:
             if (assignment := AssignmentCls(source=source, target=target)).applicable():
                 return assignment
         return None
 
-    def _assignment_lines(
+    def _field_assignment(
         self,
         source: FieldMeta,
         target: FieldMeta,
         right_side: str,
         options: AssignmentOptions,
-    ) -> List[str]:
+    ) -> cg.Statement:
         """Generate code for setting the target field to the right side.
         Only do it for a couple of conditions.
 
         :param right_side: some expression (code) that will be assigned to the target if conditions allow it
         """
-        lines: List[str] = []
-        indent = 4
-        if options.only_if_not_None:
-            lines.append(f"    if {get_var_name(source)} is not None:")
-            indent = 8
-        if options.only_if_set:
-            lines.append(f"    if '{source.name}' in self.__fields_set__:")
-            indent = 8
-
-        right_side = right_side
         if options.if_None and not options.only_if_not_None:
             right_side = f"None if {get_var_name(source)} is None else {right_side}"
-        lines.append(self._get_assignment_str(target, right_side, indent))
-        return lines
+        code: cg.Statement = self._get_assignment(target, right_side)
+
+        if options.only_if_not_None:
+            code = cg.IfElse(condition=f"{get_var_name(source)} is not None", if_block=code)
+
+        code = self.target_cls.post_process(code, source_cls=self.source_cls, source_field=source, target_field=target)
+        return code
 
-    def _get_assignment_str(self, target: FieldMeta, right_side: str, indent: int = 4) -> str:
+    def _get_assignment(self, target: FieldMeta, right_side: str) -> cg.Assignment:
         variable_name = self.target_cls.get_assignment_name(target)
-        return f'{" "*indent}d["{variable_name}"] = {right_side}'
+        lookup = cg.DictLookup(dict_name="d", key=variable_name)
+        return cg.Assignment(name=lookup, rhs=right_side)
 
     def add_mapping(self, target: FieldMeta, source: Union[FieldMeta, Callable]) -> None:
         if callable(source):
             function_assignment = FunctionAssignment(
                 function=source, target=target, methods=self.methods, target_cls_name=self.target_cls.name
             )
             right_side = function_assignment.right_side()
-            self.lines.append(self._get_assignment_str(target, right_side))
+            self.function.body.append(self._get_assignment(target, right_side))
         else:
             assert isinstance(source, FieldMeta)
 
             options = AssignmentOptions.from_Metas(
                 source_cls=self.source_cls, target_cls=self.target_cls, source=source, target=target
             )
             if assignment := self._get_asssigment(source=source, target=target):
-                self.lines.extend(
-                    self._assignment_lines(
+                self.function.body.append(
+                    self._field_assignment(
                         source=source,
                         target=target,
                         right_side=assignment.right_side(),
                         options=options,
                     )
                 )
             else:  # impossible
@@ -194,20 +180,15 @@
 
     def add_fill_with_extra(self, target: FieldMeta) -> None:
         variable_name = self.target_cls.get_assignment_name(target)
         exception_msg = (
             f"When mapping an object of '{self.source_cls.name}' to '{self.target_cls.name}' "
             f"the field '{variable_name}' needs to be provided in the `extra` dictionary"
         )
-        self.lines.extend(
-            [
-                f'    if "{variable_name}" not in extra:',
-                f'        raise TypeError("{exception_msg}")',
-                self._get_assignment_str(
-                    target=target,
-                    right_side=f'extra["{variable_name}"]',
-                ),
-            ]
+        self.function.body.append(
+            cg.IfElse(condition=f'"{variable_name}" not in extra', if_block=cg.Raise(f'TypeError("{exception_msg}")'))
         )
+        self.function.body.append(self._get_assignment(target=target, right_side=f'extra["{variable_name}"]'))
 
     def __str__(self) -> str:
-        return "\n".join(self.lines + [self.target_cls.return_statement()])
+        self.function.body.append(self.target_cls.return_statement())
+        return self.function.to_string(0)
```

### Comparing `dataclass_mapper-1.7.2/pyproject.toml` & `dataclass_mapper-1.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-mapper"
-version = "1.7.2"
+version = "1.8.0"
 description = "Autogenerate mappings between dataclasses"
 authors = ["Jakob Kogler <jakob.kogler@gmail.com>"]
 
 readme = "README.rst"
 license = "MIT"
 
 repository = "https://github.com/dataclass-mapper/dataclass-mapper"
@@ -13,36 +13,37 @@
 
 keywords = ['dataclass', 'pydantic', 'python', 'automation']
 
 classifiers = ["Topic :: Software Development :: Code Generators"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = { version = "^1.9.0", optional = true }
+pydantic = { version = ">=1.9.0", optional = true }
 
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.0.0"
+pytest = "^7.2.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
-tox = "^3.25.0"
+tox = "^4.5.2"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
-
+sphinxcontrib-plantuml = "^0.25"
+sphinx-autobuild = "^2021.3.14"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.270"
+ruff = "^0.0.276"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `dataclass_mapper-1.7.2/setup.py` & `dataclass_mapper-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['dataclass_mapper', 'dataclass_mapper.assignments']
+['dataclass_mapper',
+ 'dataclass_mapper.assignments',
+ 'dataclass_mapper.implementations']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{'pydantic': ['pydantic>=1.9.0,<2.0.0']}
+{'pydantic': ['pydantic>=1.9.0']}
 
 setup_kwargs = {
     'name': 'dataclass-mapper',
-    'version': '1.7.2',
+    'version': '1.8.0',
     'description': 'Autogenerate mappings between dataclasses',
-    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/main/graphs/badge.svg?branch=main\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=main\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses and Pydantic models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydanitc support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.\n',
+    'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/main/graphs/badge.svg?branch=main\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=main\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses and Pydantic models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydantic support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nContributing\n------------\n\nSee `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/CONTRIBUTING.rst>`_.\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.\n',
     'author': 'Jakob Kogler',
     'author_email': 'jakob.kogler@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dataclass-mapper.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dataclass_mapper-1.7.2/PKG-INFO` & `dataclass_mapper-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-mapper
-Version: 1.7.2
+Version: 1.8.0
 Summary: Autogenerate mappings between dataclasses
 Home-page: https://dataclass-mapper.readthedocs.io
 License: MIT
 Keywords: dataclass,pydantic,python,automation
 Author: Jakob Kogler
 Author-email: jakob.kogler@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Provides-Extra: pydantic
-Requires-Dist: pydantic (>=1.9.0,<2.0.0); extra == "pydantic"
+Requires-Dist: pydantic (>=1.9.0); extra == "pydantic"
 Project-URL: Documentation, https://dataclass-mapper.readthedocs.io
 Project-URL: Repository, https://github.com/dataclass-mapper/dataclass-mapper
 Description-Content-Type: text/x-rst
 
 dataclass-mapper
 ================
 
@@ -146,15 +146,20 @@
 Features
 --------
 
 The current version has support for:
 
 * Python's ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples
 * Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_
-* Pydantic models:  see `Pydanitc support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
+* Pydantic models:  see `Pydantic support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_
 * Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_
 
+Contributing
+------------
+
+See `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/CONTRIBUTING.rst>`_.
+
 License
 -------
 
 The project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.
```

