# Comparing `tmp/qtgql-0.128.0.tar.gz` & `tmp/qtgql-0.129.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.128.0.tar", max compression
+gzip compressed data, was "qtgql-0.129.0.tar", max compression
```

## Comparing `qtgql-0.128.0.tar` & `qtgql-0.129.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-10 07:23:29.319740 qtgql-0.128.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-10 07:23:29.319740 qtgql-0.128.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-10 07:23:46.475887 qtgql-0.128.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1939 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1685 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3091 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3366 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    14789 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      864 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4237 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3629 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2985 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1060 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4706 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4137 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5049 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5220 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18250 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1147 2023-07-10 07:23:29.331740 qtgql-0.128.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.128.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-16 14:43:36.502313 qtgql-0.129.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-16 14:43:36.502313 qtgql-0.129.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-16 14:43:56.890223 qtgql-0.129.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3302 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16149 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4458 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2195 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4600 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3629 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2985 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1060 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4706 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4137 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5052 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5221 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18386 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1570 2023-07-16 14:43:36.514313 qtgql-0.129.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.129.0/PKG-INFO
```

### Comparing `qtgql-0.128.0/LICENSE` & `qtgql-0.129.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/README.md` & `qtgql-0.129.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/pyproject.toml` & `qtgql-0.129.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.128.0"
+version = "0.129.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/cli.py` & `qtgql-0.129.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/config.py` & `qtgql-0.129.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.129.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.129.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 from typing import Callable, TypeVar
 
 from graphql import language as gql_lang
 from graphql.type import definition as gql_def
 
 T_AST_Node = TypeVar("T_AST_Node", bound=gql_lang.Node)
+SelectionsSet = tuple[gql_lang.SelectionNode, ...]
 
 
 def ast_identifier_factory(
     expected: type[T_AST_Node],
 ) -> Callable[[gql_lang.Node], T_AST_Node | None]:
     def type_guarder(node: gql_lang.ast.Node) -> T_AST_Node | None:
         if isinstance(node, expected):
             return node
 
     return type_guarder
 
 
 is_selection_set = ast_identifier_factory(gql_lang.ast.SelectionSetNode)
 is_inline_fragment = ast_identifier_factory(gql_lang.InlineFragmentNode)
+is_fragment_spread_node = ast_identifier_factory(gql_lang.FragmentSpreadNode)
+is_fragment_definition_node = ast_identifier_factory(gql_def.FragmentDefinitionNode)
 is_operation_def_node = ast_identifier_factory(gql_def.OperationDefinitionNode)
 is_field_node = ast_identifier_factory(gql_def.FieldNode)
 is_nonnull_node = ast_identifier_factory(gql_lang.NonNullTypeNode)
 is_named_type_node = ast_identifier_factory(gql_lang.NamedTypeNode)
 
 
 T_Definition = TypeVar("T_Definition", bound=gql_def.GraphQLType)
@@ -70,17 +73,19 @@
 inject_id_selection = inject_selection_factory(ID_SELECTION_NODE)
 inject_typename_selection = inject_selection_factory(TYPENAME_SELECTION_NODE)
 
 
 def selection_set_search_factory(
     selection_name: str,
 ) -> Callable[[gql_lang.SelectionSetNode], bool]:
-    def factory(selection_set: gql_lang.SelectionSetNode):
-        for field_or_frag in selection_set.selections:
-            if field := is_field_node(field_or_frag):
+    def factory(
+        selection_set: gql_lang.SelectionSetNode,
+    ):
+        for node in selection_set.selections:
+            if field := is_field_node(node):
                 if field.name.value == selection_name:
                     return True
         return False
 
     return factory
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/core/template.py` & `qtgql-0.129.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/generator.py` & `qtgql-0.129.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.129.0/qtgqlcodegen/operation/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 import attrs
 import graphql
 from attr import define
 
+from qtgqlcodegen.utils import HashAbleDict
+
 if TYPE_CHECKING:
+    from graphql.language import ast as gql_lang
     from graphql.type import definition as gql_def
 
     from qtgqlcodegen.schema.definitions import (
         QtGqlArgumentDefinition,
         QtGqlFieldDefinition,
         QtGqlVariableDefinition,
         SchemaTypeInfo,
@@ -20,20 +23,24 @@
         QtGqlObjectType,
         QtGqlQueriedInterface,
         QtGqlQueriedObjectType,
         QtGqlTypeABC,
     )
 
 
-@attrs.define(slots=False)
+@attrs.define(slots=False, repr=False)
 class OperationTypeInfo:
     schema_type_info: SchemaTypeInfo
     narrowed_types_map: dict[str, QtGqlQueriedObjectType] = attrs.Factory(dict)
     narrowed_interfaces_map: dict[str, QtGqlQueriedInterface] = attrs.Factory(dict)
     variables: list[QtGqlVariableDefinition] = attrs.Factory(list)
+    used_fragments: HashAbleDict[str, gql_lang.FragmentDefinitionNode] = attrs.Factory(HashAbleDict)
+    available_fragments: HashAbleDict[str, gql_lang.FragmentDefinitionNode] = attrs.Factory(
+        HashAbleDict,
+    )
 
 
 @attrs.define(frozen=True, slots=False, repr=False)
 class QtGqlQueriedField:
     type: QtGqlTypeABC
     type_info: OperationTypeInfo
     origin: QtGqlObjectType
@@ -82,30 +89,35 @@
 
 
 @define(slots=False, repr=False)
 class QtGqlOperationDefinition:
     operation_def: gql_def.OperationDefinitionNode
     root_type: QtGqlQueriedObjectType
     root_field: QtGqlQueriedField
-    fragments: list[str] = attrs.Factory(list)
     variables: list[QtGqlVariableDefinition] = attrs.Factory(list)
     narrowed_types: tuple[QtGqlQueriedObjectType, ...] = attrs.Factory(tuple)
     interfaces: tuple[QtGqlQueriedInterface, ...] = attrs.Factory(tuple)
+    used_fragments: tuple[gql_lang.FragmentDefinitionNode, ...] = attrs.Factory(tuple)
 
     @property
     def generated_variables_type(self) -> str:
         return self.name + "Variables"
 
     @property
     def name(self) -> str:
         assert self.operation_def.name
         return self.operation_def.name.value
 
     @property
     def query(self) -> str:
-        return graphql.print_ast(self.operation_def)
+        return "\n".join(
+            [
+                graphql.print_ast(self.operation_def),
+                *[graphql.print_ast(frag) for frag in self.used_fragments],
+            ],
+        )
 
 
 @define(slots=False, repr=False)
 class QtGqlVariableUse:
     argument: tuple[int, QtGqlArgumentDefinition]
     variable: QtGqlVariableDefinition
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.129.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import TYPE_CHECKING
 
 import graphql
 from graphql import OperationDefinitionNode, OperationType, language as gql_lang
 from graphql.language import visitor
 
 from qtgqlcodegen.core.graphql_ref import (
-    has_id_selection,
-    has_typename_selection,
-    inject_id_selection,
-    inject_typename_selection,
+    SelectionsSet,
     is_field_node,
+    is_fragment_definition_node,
     is_inline_fragment,
     is_named_type_node,
     is_nonnull_node,
     is_operation_def_node,
 )
 from qtgqlcodegen.operation.definitions import (
     OperationTypeInfo,
     QtGqlOperationDefinition,
     QtGqlQueriedField,
     QtGqlVariableUse,
 )
+from qtgqlcodegen.operation.selections_injection import inject_required_selections
+from qtgqlcodegen.operation.utils import unwrap_frag_spreads
 from qtgqlcodegen.schema.definitions import (
     QtGqlFieldDefinition,
     QtGqlVariableDefinition,
     SchemaTypeInfo,
 )
 from qtgqlcodegen.schema.evaluation import evaluate_graphql_type
 from qtgqlcodegen.types import (
@@ -34,15 +34,15 @@
     QtGqlList,
     QtGqlOptional,
     QtGqlQueriedInterface,
     QtGqlQueriedObjectType,
     QtGqlQueriedUnion,
     QtGqlUnion,
 )
-from qtgqlcodegen.utils import require
+from qtgqlcodegen.utils import HashAbleDict, require
 
 if TYPE_CHECKING:
     from qtgqlcodegen.types import QtGqlObjectType, QtGqlTypeABC
 
 
 def is_type_name_selection(field_node: gql_lang.FieldNode):
     # typename is not a 'real' selection and is handled with special care.
@@ -97,15 +97,15 @@
         type=_evaluate_variable_node_type(type_info, var.type),
     )
 
 
 def _evaluate_selection_set_type(
     type_info: OperationTypeInfo,
     concrete_type: QtGqlTypeABC,
-    selection_set_node: gql_lang.SelectionSetNode | None,
+    selection_set_node: SelectionsSet | None,
     path: str,
 ) -> QtGqlTypeABC:
     ret: QtGqlTypeABC | None = None
     if not selection_set_node:
         # these types have no selections
         assert (
             concrete_type.is_builtin_scalar
@@ -154,32 +154,33 @@
     type_info: OperationTypeInfo,
     concrete_field: QtGqlFieldDefinition,
     field_node: gql_lang.FieldNode,
     path: str,
     origin: QtGqlObjectType,
 ) -> QtGqlQueriedField:
     path += concrete_field.name
+    selection_set = None if not field_node.selection_set else field_node.selection_set.selections
     return QtGqlQueriedField(
         type=_evaluate_selection_set_type(
             type_info,
             concrete_field.type,
-            field_node.selection_set,
+            selection_set,
             path,
         ),
         concrete=concrete_field,
         variable_uses=_evaluate_variable_uses(type_info, concrete_field, field_node.arguments),
         origin=origin,
         type_info=type_info,
     )
 
 
 def _evaluate_list(
     type_info: OperationTypeInfo,
     concrete: QtGqlList,
-    selection_set: gql_lang.SelectionSetNode,
+    selection_set: SelectionsSet,
     path: str,
 ) -> QtGqlList:
     return QtGqlList(
         of_type=_evaluate_selection_set_type(
             type_info,
             concrete_type=concrete.of_type,
             selection_set_node=selection_set,
@@ -187,181 +188,185 @@
         ),
     )
 
 
 def _evaluate_union(
     type_info: OperationTypeInfo,
     concrete: QtGqlUnion,
-    selection_set: gql_lang.SelectionSetNode,
+    selection_set: SelectionsSet,
     path: str,
 ) -> QtGqlQueriedUnion:
     choices: dict[str, QtGqlQueriedObjectType] = {}
-    if not has_typename_selection(selection_set):
-        inject_typename_selection(selection_set)
-    for selection in selection_set.selections:
+
+    for selection in selection_set:
         if is_field_node(selection):
             continue  # __typename selection
         fragment = is_inline_fragment(selection)
         assert fragment
         type_name = fragment.type_condition.name.value
         # unions support only object types http://spec.graphql.org/October2021/#sec-Unions
         resolved_type = require(concrete.get_by_name(type_name))
         choices[type_name] = _evaluate_object_type(
             type_info=type_info,
             concrete=resolved_type,
-            selection_set=fragment.selection_set,
+            selection_set=fragment.selection_set.selections,
             path=path,
         )
 
     return QtGqlQueriedUnion(
         concrete=concrete,
         choices=tuple(choices.values()),
     )
 
 
-def _unwrap_interface_fragments(
-    type_info: SchemaTypeInfo,
+def _unwrap_interface_inline_fragments(
+    type_info: OperationTypeInfo,
     parent_concrete: QtGqlObjectType | QtGqlInterface,
-    selection_set: gql_lang.SelectionSetNode,
+    selection_set: SelectionsSet,
     initial: dict[str, list[gql_lang.FieldNode]],
-    id_was_selected: bool = False,
 ) -> dict[str, list[gql_lang.FieldNode]]:
     """Fragments can be nested, i.e node{ id.
 
-        ...on SomeFrag{
+    ...on SomeFrag{
             field1
             ...on Obj{
                 name
             }
         }
     }
-    :returns: all of the inline fragments as a flat list.
+    :return: unwrap everything and return the selections mapped to object names.
     """
-    fields_for_concrete: list[gql_lang.FieldNode] = []
-    if (
-        parent_concrete.implements_node
-        and not has_id_selection(selection_set)
-        and not id_was_selected
-    ):
-        id_was_selected = True
-        inject_id_selection(selection_set)
-    for field_or_frag in selection_set.selections:
-        if inline_frag := is_inline_fragment(field_or_frag):
+    concrete_selections: list[gql_lang.FieldNode] = []
+    for node in selection_set:
+        if inline_frag := is_inline_fragment(node):
             type_name = inline_frag.type_condition.name.value
-            # no need to validate inner types are implementation, graphql-core does this.
-            concrete_choice = type_info.get_object_type(
-                type_name,
-            ) or type_info.get_interface(type_name)
-            assert concrete_choice
-            _unwrap_interface_fragments(
+            concrete_choice = type_info.schema_type_info.get_object_or_interface(type_name)
+            _unwrap_interface_inline_fragments(
                 type_info,
                 concrete_choice,
-                inline_frag.selection_set,
+                inline_frag.selection_set.selections,
                 initial,
-                id_was_selected,
             )
         else:
-            field_node = is_field_node(field_or_frag)
-            assert field_node
+            field_node = require(is_field_node(node))
             if field_node.name.value != "__typename":
-                fields_for_concrete.append(field_node)
+                concrete_selections.append(field_node)
 
-    initial[parent_concrete.name] = fields_for_concrete
+    initial[parent_concrete.name] = concrete_selections
     return initial
 
 
+def _create_name_for_path(
+    concrete: QtGqlObjectType | QtGqlInterface,
+    path: str,
+):
+    return f"{concrete.name}__{path}"
+
+
+def _create_objects_for_interface(
+    type_info: OperationTypeInfo,
+    raw_selections_map: dict[str, list[gql_lang.FieldNode]],
+    interface: QtGqlInterface,
+    path: str,
+) -> list[QtGqlQueriedObjectType]:
+    choices: list[QtGqlQueriedObjectType] = []
+    # dispatch fragmented fields where they are needed.
+    for resolve_able in interface.implementations.values():
+        if concrete_choice := resolve_able.is_object_type:
+            selections_for_obj: list[gql_lang.FieldNode] = []
+            # collect selections from parent interfaces.
+            for base in concrete_choice.interfaces_raw:
+                if selections_for_base := raw_selections_map.get(base.name, None):
+                    selections_for_obj.extend(selections_for_base)
+
+            # collect selections from the object itself.
+            if choice_fields := raw_selections_map.get(concrete_choice.name, None):
+                selections_for_obj.extend(choice_fields)
+
+            # This could probably be more optimized though, currently
+            # this would suffice to reduce complexity.
+            obj = _evaluate_object_type(
+                type_info=type_info,
+                concrete=concrete_choice,
+                selection_set=tuple(selections_for_obj),
+                path=path,
+            )
+            choices.append(obj)
+    return choices
+
+
 def _evaluate_interface(
     type_info: OperationTypeInfo,
     concrete: QtGqlInterface,
-    selection_set: gql_lang.SelectionSetNode,
+    selection_set: SelectionsSet,
     path: str,  # current path in the query tree.
 ) -> QtGqlQueriedInterface:
-    choices: list[QtGqlQueriedObjectType] = []
+    unwrapped_selections = unwrap_frag_spreads(type_info.available_fragments, selection_set)
+    type_info.used_fragments.update(unwrapped_selections.used_fragments)
+    selection_set = unwrapped_selections.selection_set
 
-    raw_fields_map = _unwrap_interface_fragments(
-        type_info.schema_type_info,
+    raw_selections_map = _unwrap_interface_inline_fragments(
+        type_info,
         concrete,
         selection_set,
         {},
     )
-    # dispatch fragmented fields where they are needed.
-    for resolve_able in concrete.implementations.values():
-        if concrete_choice := resolve_able.is_object_type:
-            fields_for_obj = []
-            # collect fields from bases.
-            for base in concrete_choice.interfaces_raw:
-                if fields_for_base := raw_fields_map.get(base.name, None):
-                    fields_for_obj.extend(fields_for_base)
-
-            # append fields of the choice itself
-            if choice_fields := raw_fields_map.get(concrete_choice.name, None):
-                fields_for_obj.extend(choice_fields)
-            ss = gql_lang.SelectionSetNode(selections=tuple(fields_for_obj))
-            choices.append(
-                # This could probably be more optimized though, currently
-                # this would suffice to reduce complexity.
-                _evaluate_object_type(
-                    type_info=type_info,
-                    concrete=concrete_choice,
-                    selection_set=ss,
-                    path=path,
-                ),
-            )
+    choices = _create_objects_for_interface(type_info, raw_selections_map, concrete, path)
+    name = _create_name_for_path(concrete, path)
 
-    # inject __type_name selection, we'll use this to deserialize correctly.
-    if not has_typename_selection(selection_set):
-        inject_typename_selection(selection_set)
+    fields_for_interface = {
+        field.name.value: _evaluate_field(
+            type_info=type_info,
+            concrete_field=concrete.fields_dict[field.name.value],
+            path=path,
+            field_node=field,
+            origin=concrete,
+        )
+        for field in raw_selections_map[concrete.name]
+    }
 
-    name = f"{concrete.name}__{path}"
     ret = QtGqlQueriedInterface(
         name=name,
         concrete=concrete,
         choices=choices,
-        fields_dict={
-            field.name.value: _evaluate_field(
-                type_info=type_info,
-                concrete_field=concrete.fields_dict[field.name.value],
-                path=path,
-                field_node=field,
-                origin=concrete,
-            )
-            for field in raw_fields_map[concrete.name]
-        },
+        fields_dict=fields_for_interface,
     )
     for choice in choices:
         choice.base_interface = ret
+
     type_info.narrowed_interfaces_map[name] = ret
     return ret
 
 
 def _evaluate_object_type(
     type_info: OperationTypeInfo,
     concrete: QtGqlObjectType,
-    selection_set: gql_lang.SelectionSetNode,
+    selection_set: SelectionsSet,
     path: str,  # current path in the query tree.
 ) -> QtGqlQueriedObjectType:
-    # inject id selection for node implementors, it is required for caching purposes.
-    if concrete.implements_node and not has_id_selection(selection_set):
-        inject_id_selection(selection_set)
+    assert not type_info.narrowed_types_map.get(concrete.name, None), "object already evaluated"
+    unwrapped_selections = unwrap_frag_spreads(type_info.available_fragments, selection_set)
+    type_info.used_fragments.update(unwrapped_selections.used_fragments)
+    selection_set = unwrapped_selections.selection_set
 
     fields: dict[str, QtGqlQueriedField] = {}
-    for selection in selection_set.selections:
+    for selection in selection_set:
         if f_node := is_field_node(selection):
             if is_type_name_selection(f_node):
                 continue  # __typename selection is handled with special care.
             concrete_field = concrete.fields_dict[f_node.name.value]
             fields[concrete_field.name] = _evaluate_field(
                 type_info=type_info,
                 concrete_field=concrete_field,
                 field_node=f_node,
                 path=path,
                 origin=concrete,
             )
 
-    name = f"{concrete.name}__{path}"
+    name = _create_name_for_path(concrete, path)
     if ret := type_info.narrowed_types_map.get(name, None):
         return ret
 
     ret = QtGqlQueriedObjectType(
         name=name,
         concrete=concrete,
         fields_dict=fields,
@@ -369,73 +374,97 @@
     type_info.narrowed_types_map[name] = ret
     return ret
 
 
 def _evaluate_operation(
     operation: OperationDefinitionNode,
     schema_type_info: SchemaTypeInfo,
+    raw_fragments: HashAbleDict[str, gql_lang.FragmentDefinitionNode],
 ) -> QtGqlOperationDefinition:
     """Each operation generates a whole new "proxy" schema. That schema will
     contain only the fields that are currently queried. The way we do that is
     creating a so-called "proxy objects".
 
     - Each proxy object mirrors a concrete object at schema level.
     - Each proxy object contains only the fields that was queried for this field in the tree.
 
     And because of that, one object type (at the concrete schema) might have many proxy objects.
     """
-    type_info = OperationTypeInfo(schema_type_info)
-
+    type_info = OperationTypeInfo(schema_type_info, available_fragments=raw_fragments)
     # input variables
     if variables_def := operation.variable_definitions:
         for var in variables_def:
             type_info.variables.append(_evaluate_variable(type_info.schema_type_info, var))
 
     selections = operation.selection_set
-    root_type = type_info.schema_type_info.operation_types[operation.operation.value]
-    assert root_type, f"Make sure you have {operation.operation.name} type defined in your schema"
+    root_type = type_info.schema_type_info.get_root_type(operation.operation.value)
+    inject_required_selections(type_info.schema_type_info, selections, root_type)
     root_proxy_type = _evaluate_object_type(
         type_info=type_info,
         concrete=root_type,
-        selection_set=selections,
+        selection_set=selections.selections,
         path="",
     )
     assert len(root_proxy_type.fields) == 1
     root_field = root_proxy_type.fields[0]
     return QtGqlOperationDefinition(
         root_field=root_field,
         root_type=root_proxy_type,
         operation_def=operation,
         variables=type_info.variables,
         narrowed_types=tuple(type_info.narrowed_types_map.values()),
         interfaces=tuple(type_info.narrowed_interfaces_map.values()),
+        used_fragments=tuple(type_info.used_fragments.values()),
     )
 
 
 class _OperationsVisitor(visitor.Visitor):
-    def __init__(self, type_info: SchemaTypeInfo):
+    def __init__(
+        self,
+        type_info: SchemaTypeInfo,
+        fragments: HashAbleDict[str, gql_lang.FragmentDefinitionNode],
+    ):
         super().__init__()
         self.schema_type_info = type_info
+        self.raw_fragments = fragments
         self.operations: dict[str, QtGqlOperationDefinition] = {}
 
-    def enter_operation_definition(self, node, key, parent, path, ancestors) -> None:
+    def enter_operation_definition(self, node: graphql.Node, *args, **kwargs) -> None:
         if operation := is_operation_def_node(node):
             if operation.operation in (
                 OperationType.QUERY,
                 OperationType.MUTATION,
                 OperationType.SUBSCRIPTION,
             ):
                 assert operation.name, "QtGql enforces operations to have names."
                 self.operations[operation.name.value] = _evaluate_operation(
                     operation,
                     self.schema_type_info,
+                    self.raw_fragments,
                 )
 
 
+class _FragmentsVisitor(visitor.Visitor):
+    """Gets all fragments from the operations file."""
+
+    def __init__(self, type_info: SchemaTypeInfo):
+        super().__init__()
+        self.schema_type_info = type_info
+        self.fragments: HashAbleDict[str, gql_lang.FragmentDefinitionNode] = HashAbleDict()
+
+    def enter_fragment_definition(self, node: graphql.Node, *args, **kwargs) -> None:
+        fragment = require(is_fragment_definition_node(node))
+        on = self.schema_type_info.get_object_or_interface(fragment.type_condition.name.value)
+        inject_required_selections(self.schema_type_info, fragment.selection_set, on)
+        self.fragments[fragment.name.value] = fragment
+
+
 def evaluate_operations(
     operations_document: graphql.DocumentNode,
     type_info: SchemaTypeInfo,
 ) -> dict[str, QtGqlOperationDefinition]:
-    operation_visitor = _OperationsVisitor(type_info)
+    fragment_visitor = _FragmentsVisitor(type_info)
+    graphql.visit(operations_document, fragment_visitor)
+    operation_visitor = _OperationsVisitor(type_info, fragment_visitor.fragments)
     graphql.visit(operations_document, operation_visitor)
     assert operation_visitor.operations
     return operation_visitor.operations
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/operation/template.py` & `qtgql-0.129.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.129.0/qtgqlcodegen/schema/definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING
 
 from attr import Factory, define
 from graphql import OperationType
 
+from qtgqlcodegen.utils import require
+
 if TYPE_CHECKING:
     from graphql.type import definition as gql_def
     from typing_extensions import TypeAlias
 
     from qtgqlcodegen.types import (
         CustomScalarDefinition,
         QtGqlEnumDefinition,
@@ -106,35 +108,43 @@
 
 
 @define(slots=False)
 class SchemaTypeInfo:
     schema_definition: gql_def.GraphQLSchema
     custom_scalars: CustomScalarMap
     operation_types: dict[
-        Literal["query", "mutation", "subscription"],
+        str,
         QtGqlObjectType,
     ] = Factory(dict)
     object_types: ObjectTypeMap = Factory(dict)
     enums: EnumMap = Factory(dict)
     input_objects: InputObjectMap = Factory(dict)
     interfaces: InterfacesMap = Factory(dict)
 
     def get_interface(self, name: str) -> QtGqlInterface | None:
         return self.interfaces.get(name, None)
 
     def get_object_type(self, name: str) -> QtGqlObjectType | None:
         return self.object_types.get(name, None)
 
+    def get_object_or_interface(self, name: str) -> QtGqlInterface | QtGqlObjectType:
+        return require(self.get_object_type(name) or self.get_interface(name))
+
     def add_objecttype(self, objecttype: QtGqlObjectType) -> None:
         self.object_types[objecttype.name] = objecttype
 
     @cached_property
     def root_types(self) -> list[gql_def.GraphQLObjectType | None]:
         return [
             self.schema_definition.get_root_type(OperationType.QUERY),
             self.schema_definition.get_root_type(OperationType.MUTATION),
             self.schema_definition.get_root_type(OperationType.SUBSCRIPTION),
         ]
 
     @cached_property
     def root_types_names(self) -> str:
         return " ".join([tp.name for tp in self.root_types if tp])
+
+    def get_root_type(self, name: str) -> QtGqlObjectType:
+        ret = self.operation_types.get(name, None)
+        assert ret, f"Make sure you have {name} type defined in your schema"
+        return ret
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.129.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/schema/template.py` & `qtgql-0.129.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.129.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 : m_inst{inst}, 👉 base_name 👈::👉 base_name 👈(operation)
 {
     {% endif -%}
     m_operation = operation;
     {%- for field in t.fields -%}
     👉 initialize_proxy_field(field) 👈
     {% endfor -%}
-    qtgql_connect_signals();
+    _qtgql_connect_signals();
 }
 
-void 👉 t.name 👈::qtgql_connect_signals(){
+void 👉 t.name 👈::_qtgql_connect_signals(){
 {# connecting signals here, when the concrete changed it will be mirrored here. -#}
 {% if t.concrete.is_root -%}
 auto m_inst_ptr = m_inst;
 {% else %}
 auto m_inst_ptr = m_inst.get();
 {% endif -%}
 Q_ASSERT_X(m_inst_ptr, __FILE__, "Tried to instantiate a proxy object with an empty pointer!");
@@ -123,12 +123,12 @@
     m_inst->disconnect(this);
     {% for field in t.fields -%}
     if(m_inst->👉 field.private_name 👈 != new_inst->👉 field.private_name 👈){
     👉update_proxy_field(field, context.operation)👈
     };
     {% endfor -%}
     m_inst = new_inst;
-    qtgql_connect_signals();
+    _qtgql_connect_signals();
 };
 {% endif -%}
 {% endfor %}
 }
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 {% else -%}
 👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
 {% endif %}
 {% if  not t.concrete.is_root -%}
 void qtgql_replace_concrete(const std::shared_ptr<👉 t.concrete.name 👈> & new_inst);
 {% endif %}
 protected:
-    void qtgql_connect_signals();
+    void _qtgql_connect_signals();
 public:
 {% for f in t.fields -%}
 [[nodiscard]] const 👉 f.type.property_type 👈  👉 f.concrete.getter_name 👈() const;
 {% endfor -%}
 public:
 [[nodiscard]] const QString & __typename() const {% if t.base_interface -%}final{% endif %}{
     return m_inst->__typename();
```

### Comparing `qtgql-0.128.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.129.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.128.0/qtgqlcodegen/types.py` & `qtgql-0.129.0/qtgqlcodegen/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,14 +520,18 @@
     def is_queried_object_type(self) -> QtGqlQueriedObjectType | None:
         return None
 
     @property
     def is_queried_interface(self) -> QtGqlQueriedInterface | None:
         return self
 
+    @property
+    def references(self) -> list[QtGqlQueriedField]:
+        return []  # there is no need for references in interfaces.
+
 
 @define(slots=False, repr=False)
 class QtGqlQueriedUnion(QtGqlQueriedTypeABC, QtGqlTypeABC):
     concrete: QtGqlUnion
     choices: tuple[QtGqlQueriedObjectType, ...]
 
     @property
```

### Comparing `qtgql-0.128.0/PKG-INFO` & `qtgql-0.129.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.128.0
+Version: 0.129.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

