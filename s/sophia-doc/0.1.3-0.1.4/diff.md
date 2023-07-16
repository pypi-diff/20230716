# Comparing `tmp/sophia_doc-0.1.3.tar.gz` & `tmp/sophia_doc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophia_doc-0.1.3.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sophia_doc-0.1.3.tar` & `sophia_doc-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1072 2022-04-15 12:34:39.951484 sophia_doc-0.1.3/LICENSE
--rw-r--r--   0        0        0     1684 2022-11-25 07:57:44.698203 sophia_doc-0.1.3/README.md
--rw-r--r--   0        0        0     1140 2022-11-25 08:33:48.991387 sophia_doc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    15072 2022-11-25 08:18:43.928032 sophia_doc-0.1.3/sophia_doc/__init__.py
--rw-r--r--   0        0        0     3524 2022-08-19 12:48:53.082769 sophia_doc-0.1.3/sophia_doc/__main__.py
--rw-r--r--   0        0        0     2427 2022-08-19 12:45:24.424181 sophia_doc-0.1.3/sophia_doc/builders/__init__.py
--rw-r--r--   0        0        0    15860 2022-11-25 08:29:26.304365 sophia_doc-0.1.3/sophia_doc/builders/markdown.py
--rw-r--r--   0        0        0     4894 2022-08-19 12:46:47.654485 sophia_doc-0.1.3/sophia_doc/utils.py
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 sophia_doc-0.1.3/setup.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 sophia_doc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/.DS_Store
+-rw-r--r--   0        0        0    15629 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/__init__.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/py.typed
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/utils.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/builders/__init__.py
+-rw-r--r--   0        0        0    16468 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/builders/markdown.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/PKG-INFO
```

### Comparing `sophia_doc-0.1.3/LICENSE` & `sophia_doc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.3/README.md` & `sophia_doc-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 
 ## Introduction
 
 Sophia is a python package to automatically generate API documents for Python modules.
 
 It's a lot like sphinx, but it only focuses on generating markdown documentation.
 
-It does not support PEP 224 attribute docstrings, because the PEP was rejected, and have to use ast module to support
-it, which brings additional complexity to this project.
+It does not support PEP 224 attribute docstring, because the PEP was rejected, and have to use ast module to support it, which brings additional complexity to this project.
 
-# Install
+## Install
 
 ```shell
 pip install sophia-doc
 ```
 
-# Quickstart
+## Quickstart
 
 ```shell
 sophia_doc "sophia_doc" -o ./doc
 ```
 
 ## Usage
 
@@ -49,8 +48,8 @@
                         Overwrite any file in output directory. (default: False)
   --exclude-module-name, --no-exclude-module-name
                         Write file to path which exclude module name. (default: False)
 ```
 
 ## License
 
-MIT © st1020
+MIT © st1020
```

### Comparing `sophia_doc-0.1.3/sophia_doc/__init__.py` & `sophia_doc-0.1.4/sophia_doc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import sophia_doc.builders.markdown
 
 module = sophia_doc.ModuleNode(sophia_doc)
 builder = sophia_doc.builders.markdown.MarkdownBuilder(module)
 builder.write('doc_dir')
 ```
 """
-import sys
 import inspect
 import pkgutil
-import warnings
+import sys
 import traceback
+import types
+import warnings
 from enum import Enum
 from functools import cached_property
-from types import MethodType, ModuleType, FunctionType, MethodDescriptorType
-from typing import Any, Dict, List, Tuple, Union, Generic, TypeVar, Optional, NamedTuple
+from typing import Any, Dict, Generic, List, NamedTuple, Optional, Tuple, TypeVar, Union
 
 from sophia_doc.utils import import_module
 
 _T = TypeVar("_T")
 
 
 def _find_class(func: Any) -> Optional[type]:
@@ -37,19 +37,19 @@
         return None
     return cls
 
 
 def _find_doc(obj: Any) -> Optional[str]:
     # cut from pydoc
     if inspect.ismethod(obj):
-        name = obj.__func__.__name__
+        name = obj.__func__.__name__  # type: ignore
         self = obj.__self__
         if (
             inspect.isclass(self)
-            and getattr(getattr(self, name, None), "__func__") is obj.__func__
+            and getattr(self, name, None).__func__ is obj.__func__  # type: ignore
         ):
             # class method
             cls = self
         else:
             cls = self.__class__
     elif inspect.isfunction(obj):
         name = obj.__name__
@@ -63,43 +63,41 @@
             # class method
             cls = self
         else:
             cls = self.__class__
     # Should be tested before isdatadescriptor().
     elif isinstance(obj, property):
         func = obj.fget
-        name = func.__name__
+        name = func.__name__  # type: ignore
         cls = _find_class(func)
         if cls is None or getattr(cls, name) is not obj:
             return None
     elif inspect.ismethoddescriptor(obj) or inspect.isdatadescriptor(obj):
-        name = obj.__name__
-        cls = obj.__objclass__
+        name = obj.__name__  # type: ignore
+        cls = obj.__objclass__  # type: ignore
         if getattr(cls, name) is not obj:
             return None
         if inspect.ismemberdescriptor(obj):
             slots = getattr(cls, "__slots__", None)
             if isinstance(slots, dict) and name in slots:
                 return slots[name]
     else:
         return None
-    for base in cls.__mro__:
+    for base in cls.__mro__:  # type: ignore
         try:
             doc = _get_own_doc(getattr(base, name))
         except AttributeError:
             continue
         if doc is not None:
             return doc
     return None
 
 
 def _get_own_doc(obj: Any) -> Optional[str]:
-    """Get the documentation string for an object
-    if it is not inherited from its class.
-    """
+    """Get the documentation string for an object if it is not inherited from its class."""
     # cut from pydoc
     try:
         doc = object.__getattribute__(obj, "__doc__")
         if doc is None:
             return None
         if obj is not type:
             typedoc = type(obj).__doc__
@@ -160,28 +158,25 @@
         Show documentation on a variable or not.
     """
     if name == "__init__":
         return True
     # only document that which the programmer exported in __all__
     if _all is not None:
         return name in _all
-    else:
-        return not name.startswith("_")
+    return not name.startswith("_")
 
 
 def get_annotations(obj: Any) -> Dict[str, Any]:
     """Get the annotations dict for an object."""
     # refs: https://docs.python.org/3/howto/annotations.html
     if sys.version_info >= (3, 10):
         return inspect.get_annotations(obj)
-    else:
-        if isinstance(obj, type):
-            return obj.__dict__.get("__annotations__", {})
-        else:
-            return getattr(obj, "__annotations__", {})
+    if isinstance(obj, type):
+        return obj.__dict__.get("__annotations__", {})
+    return getattr(obj, "__annotations__", {})
 
 
 class DocNode(Generic[_T]):
     """The base class of document node.
 
     Attributes:
         obj: An object.
@@ -192,24 +187,24 @@
     __slots__ = ("obj", "name", "module", "_qualname")
     obj: _T
     name: str
     module: "ModuleNode"
     _qualname: str
 
     def __init__(self, obj: _T, name: str, qualname: str, module: "ModuleNode"):
+        """Init DocNode."""
         self.obj = obj
         self.name = name
         self._qualname = qualname
         self.module = module
 
     @cached_property
     def qualname(self) -> str:
-        if hasattr(self.obj, "__qualname__"):
-            return self.obj.__qualname__
-        return self._qualname
+        """The qualname of this object."""
+        return getattr(self.obj, "__qualname__", self._qualname)
 
     @cached_property
     def realname(self) -> str:
         """Real name of this object."""
         return getattr(self.obj, "__name__", self.name)
 
     @cached_property
@@ -237,61 +232,65 @@
         """
         try:
             if inspect.ismodule(obj):
                 return ModuleNode(obj)
             if inspect.isclass(obj):
                 return ClassNode(obj, name, qualname, module)
             if inspect.isroutine(obj):
-                return FunctionNode(obj, name, qualname, module)
+                return FunctionNode(obj, name, qualname, module)  # type: ignore
         except AttributeError:
             pass
         if isdata(obj):
             return DataNode(obj, name, qualname, module)
         return OtherNode(obj, name, qualname, module)
 
     def __repr__(self):
+        """Return the repr of this DocNode."""
         return (
             f"{self.__class__.__name__}:{self.name} "
             f"obj:{self.obj} docstring:{self.docstring}"
         )
 
 
-class ModuleNode(DocNode[ModuleType]):
+class ModuleNode(DocNode[types.ModuleType]):
     """The class of module node."""
 
-    def __init__(self, obj: ModuleType):
+    def __init__(self, obj: types.ModuleType):
+        """Init ModuleNode."""
         super().__init__(obj, obj.__name__, "", self)
 
     @cached_property
     def attributes(self) -> List[DocNode]:
         """A list of attributes of this module."""
         _all = getattr(self.obj, "__all__", None)
         attributes = []
         for key, value in list(getattr(self.obj, "__dict__", {}).items()):
-            if _all is not None or (inspect.getmodule(value) or self.obj) is self.obj:
-                if is_visible_name(key, _all):
-                    attributes.append(self.from_obj(value, key, key, self))
+            if (inspect.getmodule(value) or self.obj) is self.obj and is_visible_name(
+                key, _all
+            ):
+                attributes.append(self.from_obj(value, key, key, self))
         return attributes
 
     @cached_property
     def submodules(self) -> List["ModuleNode"]:
         """A list of submodules of this module."""
         submodules = []
         submodule_names = set()
         if self.is_package:
-            for importer, modname, ispkg in pkgutil.iter_modules(self.obj.__path__):
+            for _importer, modname, _ispkg in pkgutil.iter_modules(self.obj.__path__):
                 if not is_visible_name(modname):
                     continue
                 try:
                     submodule_names.add(modname)
                     module = import_module(self.name + "." + modname)
                     submodules.append(ModuleNode(module))
                 except ImportError:
                     warnings.warn(
-                        f"Can not import {modname}:\n{traceback.format_exc()}"
+                        f"Can not import {modname}:\n{traceback.format_exc()}",
+                        stacklevel=1,
                     )
 
         for key, value in inspect.getmembers(self.obj, inspect.ismodule):
             if (
                 value.__name__.startswith(self.name + ".")
                 and key not in submodule_names
             ):
@@ -348,48 +347,68 @@
         return [i for i in self.attributes if isinstance(i, DataNode)]
 
 
 class ClassNode(DocNode[type]):
     """The class of class node."""
 
     class Attribute(NamedTuple):
+        """The attribute of a class."""
+
         name: str
         kind: str
         node: DocNode
 
     @cached_property
     def attributes(self) -> List["ClassNode.Attribute"]:
         """A list of attributes of this class."""
         attributes = []
-        for name, kind, cls, value in inspect.classify_class_attrs(self.obj):
-            if (is_visible_name(name) and cls is self.obj) or (
-                name == "__init__" and not isinstance(self.obj, Enum)
+        for name in filter(is_visible_name, dir(self.obj)):
+            if isinstance(self.obj, Enum) and name == "__init__":
+                continue
+
+            if (
+                name != "__init__"
+                and name not in self.obj.__dict__
+                and name not in getattr(self.obj, "__slots__", [])
             ):
-                if inspect.isdatadescriptor(value):
-                    # ignore data descriptor create by __slots__
-                    if name in getattr(self.obj, "__slots__", []):
-                        continue
-                    kind = "data descriptor"
-                    if isinstance(value, property) and value.fset is None:
-                        kind = "readonly property"
-                # get original function from class method or static method
-                if kind == "class method" or kind == "static method":
-                    value = value.__func__
-                # functools.cached_property needs special handling
-                if isinstance(value, cached_property):
-                    kind = "cached property"
-                    node = DataNode(
-                        value, name, self.qualname + "." + name, self.module
-                    )
+                continue
+
+            value = getattr(self.obj, name)
+
+            if isinstance(value, (staticmethod, types.BuiltinMethodType)):
+                kind = "static method"
+            elif isinstance(value, (classmethod, types.ClassMethodDescriptorType)):
+                kind = "class method"
+            elif isinstance(value, property):
+                kind = "readonly property" if value.fset is None else "property"
+            elif inspect.isroutine(value):
+                kind = "method"
+            elif inspect.isdatadescriptor(value):
+                # ignore data descriptor create by __slots__
+                if name in getattr(self.obj, "__slots__", []):
+                    continue
+                kind = "data descriptor"
+            else:
+                kind = "data"
+
+            # get original function from class method or static method
+            if kind == "class method" or kind == "static method":
+                value = value.__func__  # type: ignore
+
+            # functools.cached_property needs special handling
+            if isinstance(value, cached_property):
+                kind = "cached property"
+                node = DataNode(value, name, self.qualname + "." + name, self.module)
+            else:
+                node = DocNode.from_obj(
+                    value, name, self.qualname + "." + name, self.module
+                )
+
+            attributes.append(self.Attribute(name, kind, node))
 
-                else:
-                    node = DocNode.from_obj(
-                        value, name, self.qualname + "." + name, self.module
-                    )
-                attributes.append(self.Attribute(name, kind, node))
         return attributes
 
     @cached_property
     def subclasses(self) -> List["ClassNode"]:
         """A list of subclasses of this class."""
         return [
             ClassNode(cls, cls.__name__, cls.__qualname__, self.module)
@@ -397,33 +416,32 @@
             if not (cls.__name__.startswith("_") and cls.__module__ == "builtins")
         ]
 
     @cached_property
     def bases(self) -> Tuple[str, ...]:
         """Base class names of this class."""
         return tuple(
-            map(
-                lambda x: (x.__module__ + "." if x.__module__ != "builtins" else "")
-                + x.__qualname__,
-                self.obj.__bases__,
-            )
+            (x.__module__ + "." if x.__module__ != "builtins" else "") + x.__qualname__
+            for x in self.obj.__bases__
         )
 
     @cached_property
     def mro(self) -> Tuple[type, ...]:
         """The mro of this class."""
         return inspect.getmro(self.obj)
 
     @cached_property
     def is_abstract(self) -> bool:
         """Returns True if this class is an abstract class."""
         return inspect.isabstract(self.obj)
 
 
-class FunctionNode(DocNode[Union[FunctionType, MethodType, MethodDescriptorType]]):
+class FunctionNode(
+    DocNode[Union[types.FunctionType, types.MethodType, types.MethodDescriptorType]]
+):
     """The class of function node."""
 
     @cached_property
     def signature(self) -> Optional[inspect.Signature]:
         """Signature of this function."""
         try:
             return inspect.signature(self.obj)
@@ -464,9 +482,7 @@
         if isinstance(self.obj, cached_property):
             return get_annotations(self.obj.func)
         return get_annotations(self.obj)
 
 
 class OtherNode(DocNode[_T]):
     """The class of other node."""
-
-    pass
```

### Comparing `sophia_doc-0.1.3/sophia_doc/__main__.py` & `sophia_doc-0.1.4/sophia_doc/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import sys
+"""The Sophia-doc Command-line interface."""
 import argparse
+import sys
 
 from docstring_parser import DocstringStyle
 
 from sophia_doc import ModuleNode
-from sophia_doc.utils import import_module
 from sophia_doc.builders.markdown import MarkdownBuilder
+from sophia_doc.utils import import_module
 
 if sys.version_info >= (3, 9):
     from argparse import BooleanOptionalAction
 else:
     from argparse import Action
 
     class BooleanOptionalAction(Action):
@@ -20,15 +21,14 @@
             default=None,
             type=None,
             choices=None,
             required=False,
             help=None,
             metavar=None,
         ):
-
             _option_strings = []
             for option_string in option_strings:
                 _option_strings.append(option_string)
 
                 if option_string.startswith("--"):
                     option_string = "--no-" + option_string[2:]
                     _option_strings.append(option_string)
@@ -46,23 +46,23 @@
                 required=required,
                 help=help,
                 metavar=metavar,
             )
 
         def __call__(self, parser, namespace, values, option_string=None):
             if option_string in self.option_strings:
-                setattr(namespace, self.dest, not option_string.startswith("--no-"))
+                setattr(namespace, self.dest, not option_string.startswith("--no-"))  # type: ignore
 
         def format_usage(self):
             return " | ".join(self.option_strings)
 
 
 parser = argparse.ArgumentParser(
     description="Sophia_doc is a python package to automatically "
-                "generate API documents for Python modules",
+    "generate API documents for Python modules",
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
 parser.add_argument("module", type=str, help="Python module names.")
 parser.add_argument(
     "-o",
     "--output-dir",
     type=str,
@@ -108,14 +108,15 @@
     type=str,
     default="index.md",
     help="The name of Markdown file from __init__.py, index.md by default.",
 )
 
 
 def cli():
+    """The Sophia-doc Command-line interface."""
     args = parser.parse_args()
     MarkdownBuilder(
         ModuleNode(import_module(args.module)),
         docstring_style=getattr(DocstringStyle, args.docstring_style.upper()),
         anchor_extend=args.anchor_extend,
         ignore_data=args.ignore_data,
     ).write(
```

### Comparing `sophia_doc-0.1.3/sophia_doc/builders/__init__.py` & `sophia_doc-0.1.4/sophia_doc/builders/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Builder is class to build ModuleNode to target formats."""
+from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING
-from abc import ABC, abstractmethod
 
 from docstring_parser import Docstring, DocstringStyle, parse
 
 if TYPE_CHECKING:
     from sophia_doc import DocNode, ModuleNode
 
 
@@ -24,14 +24,20 @@
 
     def __init__(
         self,
         module: "ModuleNode",
         *,
         docstring_style: DocstringStyle = DocstringStyle.AUTO,
     ):
+        """Init Builder.
+
+        Args:
+            module: The Module Node to build.
+            docstring_style: The docstring style. Defaults to DocstringStyle.AUTO.
+        """
         self.module = module
         self.docstring_style = docstring_style
 
     def _new_builder(self, module: "ModuleNode") -> "Builder":
         """Get a new instance of Builder class, is used in write method."""
         return self.__class__(module, docstring_style=self.docstring_style)
 
@@ -59,14 +65,15 @@
     def write(self, output_dir: str, *, overwrite: bool = False, **kwargs) -> None:
         """Write file to output dir.
 
         Args:
             output_dir: The output directory.
             overwrite: If true will overwrite any file in output directory,
                 otherwise raise an Exception when file already exists.
+            **kwargs: Other args.
         """
         filepath = Path(output_dir).resolve() / self.get_path(**kwargs)
         filepath.parent.mkdir(parents=True, exist_ok=True)
         if not self.module.is_namespace:
             filepath.touch(exist_ok=overwrite)
             with open(filepath, "w", encoding="utf-8") as f:
                 f.write(self.text())
```

### Comparing `sophia_doc-0.1.3/sophia_doc/builders/markdown.py` & `sophia_doc-0.1.4/sophia_doc/builders/markdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+"""The Markdown Builder."""
 import inspect
 import warnings
 from pathlib import Path
 from textwrap import indent
-from typing import Dict, List, Tuple, Optional
+from typing import Dict, List, Optional, Tuple
 
 from docstring_parser import Docstring, DocstringParam, DocstringStyle
 
+from sophia_doc import ClassNode, DataNode, DocNode, FunctionNode, ModuleNode
 from sophia_doc.builders import Builder
-from sophia_doc.utils import format_signature, format_annotation
-from sophia_doc import DocNode, DataNode, ClassNode, ModuleNode, FunctionNode
+from sophia_doc.utils import format_annotation, format_signature
 
 
-def get_description(docstring: "Docstring") -> List[str]:
+def get_description(docstring: Docstring) -> List[str]:
     """Get description form a Docstring object.
 
     Args:
         docstring: A Docstring object.
 
     Returns:
         A list of description string.
     """
-    result: List[str] = list()
+    result: List[str] = []
     if docstring.short_description:
         result.append(docstring.short_description)
     if docstring.long_description:
         result.append(docstring.long_description)
     return result
 
 
@@ -45,15 +46,15 @@
     if annotation:
         result += f" ({Markdown.italic(annotation)})"
     if description:
         result += f" - {description}"
     return result
 
 
-def parser_docstring_param(param: "DocstringParam") -> str:
+def parser_docstring_param(param: DocstringParam) -> str:
     """Get formatted string of parameter from a DocstringParam object.
 
     Args:
         param: A DocstringParam object.
 
     Returns:
         Formatted string of parameter.
@@ -62,158 +63,170 @@
 
 
 class Markdown:
     """Markdown format."""
 
     @staticmethod
     def indent(text: str, level: int = 1) -> str:
+        """Indent."""
         return indent(text, prefix=" " * (level * 2))
 
     @staticmethod
     def italic(text: str) -> str:
+        """Italic."""
         return f"*{text}*"
 
     @staticmethod
     def bold(text: str) -> str:
+        """Bold."""
         return f"**{text}**"
 
     @staticmethod
     def title(text: str, level: int = 1) -> str:
+        """Title."""
         return "#" * level + " " + text
 
     @staticmethod
     def inline_code(text: str) -> str:
+        """Inline Code."""
         return f"`{text}`"
 
 
 class MarkdownBuilder(Builder):
-    """
-    Markdown Builder.
+    """Markdown Builder.
 
     Attributes:
         anchor_extend: If true will add anchor extend to title,
             like # Your title {#your-custom-id}
         ignore_data: If true will ignore data in Markdown text.
     """
 
     anchor_extend: bool
     ignore_data: bool
 
     def __init__(
         self,
-        module: "ModuleNode",
+        module: ModuleNode,
         *,
         docstring_style: DocstringStyle = DocstringStyle.AUTO,
         anchor_extend: bool = False,
         ignore_data: bool = False,
     ):
+        """Init Markdown Builder."""
         super().__init__(module, docstring_style=docstring_style)
         self.anchor_extend = anchor_extend
         self.ignore_data = ignore_data
 
-    def _new_builder(self, module: "ModuleNode") -> "Builder":
+    def _new_builder(self, module: ModuleNode) -> "Builder":
         return self.__class__(
             module,
             docstring_style=self.docstring_style,
             anchor_extend=self.anchor_extend,
             ignore_data=self.ignore_data,
         )
 
     def get_path(
         self,
         exclude_module_name: bool = False,
         init_file_name: str = "index.md",
-        **kwargs,
+        **kwargs,  # noqa: ARG002
     ) -> Path:
         """Get the path to write file.
 
         Args:
             exclude_module_name: If true will write file to path
                 which exclude module name, like change output path
                 form `./doc/sophia_doc/index.md` to `./doc/index.md`.
             init_file_name: The name of Markdown file
                 from __init__.py, `index.md` by default.
+            **kwargs: Other args.
         """
         if exclude_module_name:
             path = Path(*self.module.name.split(".")[1:])
         else:
             path = Path(*self.module.name.split(".")[0:])
         return (
             path / init_file_name if self.module.is_package else path.with_suffix(".md")
         )
 
     def text(self) -> str:
-        result: List[str] = list()
+        """Get string of current module documentation."""
+        result: List[str] = []
         result.append(Markdown.title(self.module.name, 1))
 
         docstring = self.get_docstring(self.module)
         result.extend(get_description(docstring))
 
         for node in self.module.attributes:
             result.append(self.build_doc(node))
 
         return self._build_str(result).replace("<", r"\<").replace(">", r"\>")
 
     @staticmethod
     def _build_str(str_list: List[str]) -> str:
         return "\n\n".join(filter(lambda x: x, str_list))
 
-    def build_doc(self, node: "DocNode", *, level: int = 1, **kwargs) -> str:
+    def build_doc(self, node: DocNode, *, level: int = 1, **kwargs) -> str:
         """Build markdown string from a DocNode.
 
         Args:
             node: A DocNode.
             level: The title level.
+            **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if isinstance(node, ClassNode):
             return self.build_class(node, level=level)
-        elif isinstance(node, FunctionNode):
+        if isinstance(node, FunctionNode):
             return self.build_function(node, level=level, **kwargs)
-        elif isinstance(node, DataNode):
+        if isinstance(node, DataNode):
             return self.build_data(node, level=level, **kwargs)
+        raise ValueError
 
-    def _extend_title(self, title: str, node: "DocNode") -> str:
+    def _extend_title(self, title: str, node: DocNode) -> str:
         return title + " {#" + node.qualname + "}" if self.anchor_extend else title
 
     def build_class(self, node: ClassNode, *, level: int = 1) -> str:
         """Build markdown string from a ClassNode.
 
         Args:
             node: A ClassNode.
             level: The title level.
 
         Returns:
             A markdown string.
         """
-        _kind = list()
+        _kind = []
         if node.is_abstract:
             _kind.append("abstract")
         if isinstance(node.obj, Exception):
             _kind.append("exception")
         else:
             _kind.append("class")
         _kind = " ".join(_kind)
 
         init = None
         for attr in node.attributes:
             if attr.name == "__init__":
                 assert isinstance(attr.node, FunctionNode)
                 init = attr.node
 
-        result: List[str] = list()
+        result: List[str] = []
         title = Markdown.title(
             Markdown.italic(_kind) + " " + Markdown.inline_code(node.name), level + 1
         )
         if init and init.signature:
             title += format_signature(init.signature)
         else:
-            warnings.warn(f"Can not get __init__ method signature of class {node.name}")
+            warnings.warn(
+                f"Can not get __init__ method signature of class {node.name}",
+                stacklevel=1,
+            )
         result.append(self._extend_title(title, node))
 
         result.append("Bases: " + ", ".join(map(Markdown.inline_code, node.bases)))
 
         docstring = self.get_docstring(node)
         result.extend(get_description(docstring))
 
@@ -224,15 +237,15 @@
                 )
             )
 
         if docstring.params or node.annotations:
             result.append("- **Attributes**")
 
             parma_dict: Dict[
-                str, Tuple["inspect.Parameter", Optional["DocstringParam"]]
+                str, Tuple[inspect.Parameter, Optional[DocstringParam]]
             ] = {}
             if node.annotations:
                 parma_dict = {
                     key: (annotation, None)
                     for key, annotation in node.annotations.items()
                     if not key.startswith("_")
                 }
@@ -240,15 +253,18 @@
             if docstring.params:
                 for param_doc in docstring.params:
                     annotation, _ = parma_dict.get(param_doc.arg_name, (None, None))
                     if param_doc.type_name is None and annotation:
                         param_doc.type_name = format_annotation(
                             annotation, base_module=node.module.obj
                         )
-                    parma_dict[param_doc.arg_name] = (annotation, param_doc)
+                    parma_dict[param_doc.arg_name] = (  # type:ignore
+                        annotation,
+                        param_doc,
+                    )
 
             for name, (annotation, param_doc) in parma_dict.items():
                 if param_doc is None:
                     result.append(
                         Markdown.indent(
                             parser_param(
                                 name,
@@ -260,62 +276,63 @@
                         )
                     )
                 else:
                     result.append(Markdown.indent(parser_docstring_param(param_doc)))
 
         if docstring.examples:
             result.append("- **Examples**")
-            result.append(Markdown.indent(docstring.examples[0].description))
+            result.append(Markdown.indent(docstring.examples[0].description or ""))
 
-        for name, kind, node in node.attributes:
+        for name, kind, node_ in node.attributes:
             if name == "__init__":
                 continue
             result.append(
                 self.build_doc(
-                    node,
+                    node_,
                     level=level + 1,
                     kind=kind,
                     ignore_first_arg=kind == "method" or kind == "class method",
                 )
             )
 
         return self._build_str(result)
 
     @staticmethod
     def _build_argument(
-        node: FunctionNode, docstring: "Docstring", *, ignore_first_arg: bool = False
+        node: FunctionNode, docstring: Docstring, *, ignore_first_arg: bool = False
     ) -> List[str]:
         result = []
         if docstring.params or (node.signature and node.signature.parameters):
             parma_dict: Dict[
-                str, Tuple["inspect.Parameter", Optional["DocstringParam"]]
+                str, Tuple[inspect.Parameter, Optional[DocstringParam]]
             ] = {}
             if node.signature and node.signature.parameters:
                 for key, param in node.signature.parameters.items():
                     if param.kind == param.VAR_POSITIONAL:
-                        key = "*" + key
+                        key = "*" + key  # noqa: PLW2901
                     elif param.kind == param.VAR_KEYWORD:
-                        key = "**" + key
+                        key = "**" + key  # noqa: PLW2901
                     parma_dict[key] = (param, None)
 
             if docstring.params:
                 for param_doc in docstring.params:
                     if param_doc.arg_name not in parma_dict and (
                         node.signature and node.signature.parameters
                     ):
                         warnings.warn(
                             f'The argument "{param_doc.arg_name}" '
-                            f"can not find in function signature."
+                            f"can not find in function signature.",
+                            stacklevel=1,
                         )
                     param, _ = parma_dict.get(param_doc.arg_name, (None, None))
                     if param_doc.type_name is None and param:
                         param_doc.type_name = format_annotation(
                             param.annotation, base_module=node.module.obj
                         )
-                    parma_dict[param_doc.arg_name] = (param, param_doc)
+                    parma_dict[param_doc.arg_name] = (param, param_doc)  # type:ignore
 
             if ignore_first_arg and parma_dict:
                 parma_dict.pop(list(parma_dict.keys())[0])
 
             if parma_dict:
                 result.append("- **Arguments**")
 
@@ -340,52 +357,52 @@
     def build_function(
         self,
         node: FunctionNode,
         *,
         level: int = 1,
         kind: str = "function",
         ignore_first_arg: bool = False,
-        **kwargs,  # noqa
+        **kwargs,  # noqa: ARG002
     ) -> str:
         """Build markdown string from a FunctionNode.
 
         Args:
             node: A FunctionNode.
             level: The title level.
             kind: The function kind, like 'function', 'method', 'class method'.
             ignore_first_arg: If True the first argument of the function
                 will be ignored.
+            **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if not node.signature:
             warnings.warn(
-                f"The {node.qualname} ({node.obj}) not have signature, ignored."
+                f"The {node.qualname} ({node.obj}) not have signature, ignored.",
+                stacklevel=1,
             )
             return ""
 
-        _kind = list()
+        _kind = []
         if node.is_async:
             _kind.append("async")
         if node.is_lambda_func:
             _kind.append("lambda")
         _kind.append(kind)
         _kind = " ".join(_kind)
 
-        result: List[str] = list()
+        result: List[str] = []
         result.append(
             self._extend_title(
                 Markdown.title(
                     Markdown.italic(_kind)
                     + " "
                     + Markdown.inline_code(
-                        "{name}{signature}".format(
-                            name=node.name, signature=format_signature(node.signature)
-                        )
+                        f"{node.name}{format_signature(node.signature)}"
                     ),
                     level + 1,
                 ),
                 node,
             )
         )
 
@@ -421,43 +438,49 @@
 
         if docstring.raises:
             result.append("- **Raises**")
             for raise_doc in docstring.raises:
                 result.append(
                     Markdown.indent(
                         "- {type_name} - {description}".format(
-                            type_name=Markdown.bold(raise_doc.type_name),
+                            type_name=Markdown.bold(raise_doc.type_name or ""),
                             description=raise_doc.description,
                         )
                     )
                 )
 
         if docstring.examples:
             result.append("- **Examples**")
-            result.append(Markdown.indent(docstring.examples[0].description))
+            result.append(Markdown.indent(docstring.examples[0].description or ""))
 
         return self._build_str(result)
 
     def build_data(
-        self, node: DataNode, *, level: int = 1, kind: str = "data", **kwargs  # noqa
+        self,
+        node: DataNode,
+        *,
+        level: int = 1,
+        kind: str = "data",
+        **kwargs,  # noqa: ARG002
     ) -> str:
         """Build markdown string from a DataNode.
 
         Args:
             node: A DataNode.
             level: The title level.
             kind: The function kind, like 'data', 'property'.
+            **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if self.ignore_data and kind == "data":
             return ""
 
-        result: List[str] = list()
+        result: List[str] = []
         result.append(
             self._extend_title(
                 Markdown.title(
                     Markdown.italic(kind) + " " + Markdown.inline_code(node.name),
                     level + 1,
                 ),
                 node,
```

### Comparing `sophia_doc-0.1.3/sophia_doc/utils.py` & `sophia_doc-0.1.4/sophia_doc/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utils of sophia_doc."""
-import re
-import inspect
-import warnings
 import importlib
+import inspect
+import re
 import traceback
+import warnings
 from types import ModuleType
 from typing import Any, Optional
 
 
 def import_module(modname: str) -> ModuleType:
     """A wrapper of importlib.import_module, convert exceptions to ImportError.
 
@@ -42,17 +42,17 @@
     """
     if annotation is inspect.Signature.empty:
         return ""
     if isinstance(annotation, str):
         return annotation
     # use regex delete 'ForwardRef' from annotation
     return re.sub(
-        r"\bForwardRef\((?P<quot>[\'\"])(?P<string>.*?)(?P=quot)\)",
-        r"\g<string>",
-        inspect.formatannotation(annotation, base_module),
+        r"\bForwardRef\((?P<quot>[\'\"])(?P<string>.*?)(?P=quot)\)",  # type: ignore
+        r"\g<string>",  # type: ignore
+        inspect.formatannotation(annotation, base_module),  # type: ignore
     )
 
 
 def format_parameter(parameter: inspect.Parameter, type_comments: bool = False) -> str:
     """Format inspect.Parameter object, type comments is optional.
 
     Cut from inspect.Parameter.__str__().
@@ -65,33 +65,32 @@
         The formatted string.
     """
     kind = parameter.kind
     formatted = parameter.name
 
     # Add annotation and default value
     if parameter.annotation is not inspect.Parameter.empty and type_comments:
-        formatted = "{}: {}".format(formatted, format_annotation(parameter.annotation))
+        formatted = f"{formatted}: {format_annotation(parameter.annotation)}"
 
     if parameter.default is not inspect.Parameter.empty:
         if parameter.annotation is not inspect.Parameter.empty:
-            formatted = "{} = {}".format(formatted, repr(parameter.default))
+            formatted = f"{formatted} = {parameter.default!r}"
         else:
-            formatted = "{}={}".format(formatted, repr(parameter.default))
+            formatted = f"{formatted}={parameter.default!r}"
 
     if kind == inspect.Parameter.VAR_POSITIONAL:
         formatted = "*" + formatted
     elif kind == inspect.Parameter.VAR_KEYWORD:
         formatted = "**" + formatted
 
     return formatted
 
 
 def format_signature(signature: inspect.Signature, type_comments: bool = False) -> str:
-    """
-    Format inspect.Signature object, type comments is optional.
+    """Format inspect.Signature object, type comments is optional.
 
     Cut from inspect.Signature.__str__().
 
     Args:
         signature: The inspect.Signature object to be formatted.
         type_comments: If True will include type comments.
 
@@ -137,10 +136,10 @@
         # flag was not reset to 'False'
         result.append("/")
 
     rendered = "({})".format(", ".join(result))
 
     if signature.return_annotation is not inspect.Parameter.empty and type_comments:
         anno = format_annotation(signature.return_annotation)
-        rendered += " -> {}".format(anno)
+        rendered += f" -> {anno}"
 
     return rendered
```

### Comparing `sophia_doc-0.1.3/setup.py` & `sophia_doc-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sophia-doc
+Version: 0.1.4
+Summary: A python package to automatically generate API documents for Python modules.
+Project-URL: Homepage, https://github.com/st1020/sophia-doc
+Project-URL: Source, https://github.com/st1020/sophia-doc
+Author-email: st1020 <stone_1020@qq.com>
+License: MIT
+License-File: LICENSE
+Keywords: doc,documentation,markdown,pydoc,sophia-doc
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Requires-Dist: docstring-parser>=0.15
+Description-Content-Type: text/markdown
+
+# Sophia-doc
+
+**A python package to automatically generate API documents for Python modules.**
+
+## Introduction
+
+Sophia is a python package to automatically generate API documents for Python modules.
+
+It's a lot like sphinx, but it only focuses on generating markdown documentation.
+
+It does not support PEP 224 attribute docstring, because the PEP was rejected, and have to use ast module to support it, which brings additional complexity to this project.
+
+## Install
+
+```shell
+pip install sophia-doc
+```
+
+## Quickstart
+
+```shell
+sophia_doc "sophia_doc" -o ./doc
+```
+
+## Usage
+
+Command line:
+
+```shell
+usage: sophia_doc [-h] [-o OUTPUT_DIR] [--docstring-style DOCSTRING_STYLE] [--anchor-extend | --no-anchor-extend] [--overwrite | --no-overwrite]
+                   [--exclude-module-name | --no-exclude-module-name]
+                   module
+
+Sophia_doc is a python package to automatically generate API documents for Python modules
+
+positional arguments:
+  module                Python module names.
+
+options:
+  -h, --help            show this help message and exit
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        The directory to write document. (default: doc)
+  --docstring-style DOCSTRING_STYLE
+                        Docstring style the python module used. (default: auto)
+  --anchor-extend, --no-anchor-extend
+                        Add anchor to markdown title. (default: False)
+  --overwrite, --no-overwrite
+                        Overwrite any file in output directory. (default: False)
+  --exclude-module-name, --no-exclude-module-name
+                        Write file to path which exclude module name. (default: False)
+```
 
-packages = \
-['sophia_doc', 'sophia_doc.builders']
+## License
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['docstring-parser>=0.15,<0.16']
-
-entry_points = \
-{'console_scripts': ['sophia-doc = sophia_doc.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'sophia-doc',
-    'version': '0.1.3',
-    'description': 'A python package to automatically generate API documents for Python modules.',
-    'long_description': '# Sophia-doc\n\n**A python package to automatically generate API documents for Python modules.**\n\n## Introduction\n\nSophia is a python package to automatically generate API documents for Python modules.\n\nIt\'s a lot like sphinx, but it only focuses on generating markdown documentation.\n\nIt does not support PEP 224 attribute docstrings, because the PEP was rejected, and have to use ast module to support\nit, which brings additional complexity to this project.\n\n# Install\n\n```shell\npip install sophia-doc\n```\n\n# Quickstart\n\n```shell\nsophia_doc "sophia_doc" -o ./doc\n```\n\n## Usage\n\nCommand line:\n\n```shell\nusage: sophia_doc [-h] [-o OUTPUT_DIR] [--docstring-style DOCSTRING_STYLE] [--anchor-extend | --no-anchor-extend] [--overwrite | --no-overwrite]\n                   [--exclude-module-name | --no-exclude-module-name]\n                   module\n\nSophia_doc is a python package to automatically generate API documents for Python modules\n\npositional arguments:\n  module                Python module names.\n\noptions:\n  -h, --help            show this help message and exit\n  -o OUTPUT_DIR, --output-dir OUTPUT_DIR\n                        The directory to write document. (default: doc)\n  --docstring-style DOCSTRING_STYLE\n                        Docstring style the python module used. (default: auto)\n  --anchor-extend, --no-anchor-extend\n                        Add anchor to markdown title. (default: False)\n  --overwrite, --no-overwrite\n                        Overwrite any file in output directory. (default: False)\n  --exclude-module-name, --no-exclude-module-name\n                        Write file to path which exclude module name. (default: False)\n```\n\n## License\n\nMIT © st1020',
-    'author': 'st1020',
-    'author_email': 'stone_1020@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+MIT © st1020
```

