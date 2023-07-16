# Comparing `tmp/heimdallm-0.2.1.tar.gz` & `tmp/heimdallm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdallm-0.2.1.tar", max compression
+gzip compressed data, was "heimdallm-0.3.0.tar", max compression
```

## Comparing `heimdallm-0.2.1.tar` & `heimdallm-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      750 2023-07-10 22:01:58.825056 heimdallm-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-07-10 22:01:58.825056 heimdallm-0.2.1/LICENSE
--rw-r--r--   0        0        0     6958 2023-07-10 22:01:58.825056 heimdallm-0.2.1/README.md
--rw-r--r--   0        0        0       81 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/__init__.py
--rw-r--r--   0        0        0     6583 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrost.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/__init__.py
--rw-r--r--   0        0        0     5293 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/bifrost.py
--rw-r--r--   0        0        0     5688 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/common.py
--rw-r--r--   0        0        0     6014 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelope.py
--rw-r--r--   0        0        0     1234 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2
--rw-r--r--   0        0        0     1331 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/test.j2
--rw-r--r--   0        0        0     6668 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/exc.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/__init__.py
--rw-r--r--   0        0        0    15919 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/presets.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/__init__.py
--rw-r--r--   0        0        0     1545 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/bifrost.py
--rw-r--r--   0        0        0      563 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/envelope.py
--rw-r--r--   0        0        0     6391 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/grammar.lark
--rw-r--r--   0        0        0      685 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/validator.py
--rw-r--r--   0        0        0     5029 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/reconstruct.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/presets.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/__init__.py
--rw-r--r--   0        0        0     1971 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
--rw-r--r--   0        0        0      564 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py
--rw-r--r--   0        0        0     6737 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/grammar.lark
--rw-r--r--   0        0        0      685 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/validator.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/identifier.py
--rw-r--r--   0        0        0    11519 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/validator.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/__Init__.py
--rw-r--r--   0        0        0     3005 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/aliases.py
--rw-r--r--   0        0        0     2947 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/ambiguity.py
--rw-r--r--   0        0        0    14153 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/facets.py
--rw-r--r--   0        0        0     1451 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/constraints.py
--rw-r--r--   0        0        0     1643 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/envelope.py
--rw-r--r--   0        0        0      734 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/__init__.py
--rw-r--r--   0        0        0      793 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/mock.py
--rw-r--r--   0        0        0     2433 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/openai.py
--rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/support/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/support/github.py
--rw-r--r--   0        0        0     1621 2023-07-10 22:01:58.865057 heimdallm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 heimdallm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-07-16 05:51:54.322255 heimdallm-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-16 05:51:54.322255 heimdallm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6958 2023-07-16 05:51:54.322255 heimdallm-0.3.0/README.md
+-rw-r--r--   0        0        0       81 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrost.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/__init__.py
+-rw-r--r--   0        0        0     6624 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/bifrost.py
+-rw-r--r--   0        0        0     5688 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/common.py
+-rw-r--r--   0        0        0     6014 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/envelope.py
+-rw-r--r--   0        0        0     1351 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2
+-rw-r--r--   0        0        0     1331 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.326254 heimdallm-0.3.0/heimdallm/bifrosts/sql/envelopes/sql/test.j2
+-rw-r--r--   0        0        0     6668 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/__init__.py
+-rw-r--r--   0        0        0    15919 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/presets.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/__init__.py
+-rw-r--r--   0        0        0     1678 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/bifrost.py
+-rw-r--r--   0        0        0      563 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/envelope.py
+-rw-r--r--   0        0        0     6673 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/validator.py
+-rw-r--r--   0        0        0     6902 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/reconstruct.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/presets.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/__init__.py
+-rw-r--r--   0        0        0     2013 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
+-rw-r--r--   0        0        0      564 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/envelope.py
+-rw-r--r--   0        0        0     6946 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/validator.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/utils/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/utils/identifier.py
+-rw-r--r--   0        0        0    11616 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/validator.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/__Init__.py
+-rw-r--r--   0        0        0     4707 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/aliases.py
+-rw-r--r--   0        0        0     2947 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/ambiguity.py
+-rw-r--r--   0        0        0    15624 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/facets.py
+-rw-r--r--   0        0        0     1451 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/constraints.py
+-rw-r--r--   0        0        0     1643 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/envelope.py
+-rw-r--r--   0        0        0      734 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/llm.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/llm_providers/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/llm_providers/mock.py
+-rw-r--r--   0        0        0     2433 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/llm_providers/openai.py
+-rw-r--r--   0        0        0        0 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/support/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-16 05:51:54.330255 heimdallm-0.3.0/heimdallm/support/github.py
+-rw-r--r--   0        0        0     1621 2023-07-16 05:51:54.370255 heimdallm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 heimdallm-0.3.0/PKG-INFO
```

### Comparing `heimdallm-0.2.1/CONTRIBUTING.md` & `heimdallm-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/LICENSE` & `heimdallm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/README.md` & `heimdallm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrost.py` & `heimdallm-0.3.0/heimdallm/bifrost.py`

 * *Files 16% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         validation_exc = None
         for validator in self.constraint_validators:
             log.info(
                 "Trying constraint validator",
                 validator=validator.__class__.__name__,
             )
             try:
-                trusted_llm_output = self._try_validator(
+                trusted_llm_output, tree = self._try_validator(
                     log,
                     validator,
                     autofix,
                     untrusted_llm_output,
                     tree,
                 )
             except Exception as e:
@@ -127,24 +127,26 @@
             except Exception as e:
                 log.exception("Validation failed")
                 raise e
 
         log = log.bind(trusted=untrusted_llm_output)
         log.info("Validation succeeded")
 
+        trusted_llm_output = self.post_transform(trusted_llm_output, tree)
+
         return trusted_llm_output
 
     def _try_validator(
         self,
         log: structlog.BoundLogger,
         validator: "heimdallm.constraints.ConstraintValidator",
         autofix: bool,
         untrusted_llm_output: str,
         tree: ParseTree,
-    ) -> str:
+    ) -> tuple[str, ParseTree]:
         """Attempt validation with an individual constraint validator."""
 
         if autofix:
             log.info("Autofixing parse tree and reconstructing the input")
             try:
                 untrusted_llm_output = validator.fix(self, self.grammar, tree)
             except Exception as e:
@@ -159,15 +161,30 @@
             log.info("Reconstruction succeeded")
 
         # throws a bifrost-specific exception
         log.info("Validating parse tree")
         validator.validate(self, untrusted_llm_output, tree)
         log.info("Validation succeeded")
 
-        return untrusted_llm_output
+        return untrusted_llm_output, tree
+
+    def post_transform(self, trusted_llm_output: str, tree: ParseTree) -> str:
+        """
+        A hook for subclasses to perform post-transformations on the trusted output.
+        This is useful for making adjustments that cannot be made during
+        :doc:`/reconstruction` because they would produce an output that is incompatible
+        with the grammar.
+
+        For example, replacing the generic ``:placeholder`` with the SQL-specific
+        placeholder fields (e.g. ``%(placeholder)s``) cannot be done in reconstruction
+        because it would conflict with the grammar. It needs to be done in a separate
+        step, after the input has been reconstruction and the constraint validators have
+        been satisfied.
+        """
+        return trusted_llm_output
 
     def parse(self, untrusted_llm_output: str) -> ParseTree:
         """Converts the :term:`LLM` output into a parse tree. Override it in a subclass
         to throw custom exceptions based on the grammar and parse state.
 
         :param untrusted_llm_output: The unwrapped output from the LLM.
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/bifrost.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/bifrost.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, Sequence, Union
+from typing import TYPE_CHECKING, Callable, Sequence, Union, cast
 
 import lark
-from lark import Lark, ParseTree
+from lark import Lark, ParseTree, Token
 from lark.exceptions import VisitError
 
 from heimdallm.bifrost import Bifrost as _BaseBifrost
 from heimdallm.bifrosts.sql import exc
 from heimdallm.llm import LLMIntegration
 from heimdallm.llm_providers.mock import EchoMockLLM
 
@@ -113,14 +113,48 @@
                 if isinstance(e.orig_exc, exc.BaseException):
                     raise e.orig_exc
                 raise e
             return final_tree
 
         return parse
 
+    @classmethod
+    def placeholder(cls, name: str) -> str:
+        """
+        For a given database and library, produce a placeholder for a named parameter.
+        This is needed because different databases and libraries have different formats
+        for their placeholder params. For example, sqlite is ``:param`` while mysql is
+        ``%(param)s``.
+
+        :param name: The name of the placeholder to be replaced.
+        :return: The db-specific placeholder.
+        :meta private:
+        """
+        return ":" + name
+
+    def post_transform(self, trusted_llm_output: str, tree: ParseTree) -> str:
+        placeholders = list(tree.find_data("placeholder"))
+
+        # reverse=True so we work backwords so we don't mess up the indices
+        placeholders.sort(key=lambda x: x.meta.start_pos, reverse=True)
+
+        def replace_slice(input_str, start, end, replacement):
+            return input_str[:start] + replacement + input_str[end:]
+
+        for placeholder in placeholders:
+            m = placeholder.meta
+            name = cast(Token, placeholder.children[0]).value
+            trusted_llm_output = replace_slice(
+                trusted_llm_output,
+                m.start_pos,
+                m.end_pos,
+                self.placeholder(name),
+            )
+        return trusted_llm_output
+
     @staticmethod
     @abstractmethod
     def build_grammar() -> Lark:
         """
         Produces the grammar that will be used to parse the dialect of SQL. Must be
         implemented in a subclass.
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/common.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/common.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelope.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 Consider the following Mysql 8.0 SQL schema:
 ```
 {{db_schema}}
 ```
 {%- endblock %}
 
 {% block requester_context -%}
-A requester has written a free-form query that they want translated into a SQL query, compatible with sqlite that operates on the above database schema.
+A requester has written a free-form query that they want translated into a SQL query, compatible with Mysql 8.0 that operates on the above database schema.
 {%- endblock %}
 
 {% block requester_identities -%}
     {%- if id_constraints -%}
 If possible, constrain the query to the data that the requester has access to by using one of the following conditions: {{id_constraints}}.
     {%- else -%}
 Assume that the requester that wrote the query has unrestricted access to all data.
     {%- endif -%}
 {%- endblock %}
 
 {% block current_time -%}
-If the current time is needed, assume that the placeholder `:timestamp` holds the current unix timestamp.
+If the current time is needed, assume that the placeholder `:timestamp` holds the current unix timestamp as an integer. Use the necessary functions to convert it to a datetime in order to compare it to datetime columns.
 {%- endblock %}
 
 {% block delimiters -%}
 Only respond with the SQL query. Delimit the query in the response with "```"
 {%- endblock %}
 
 {% block general_constraints -%}
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/exc.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/exc.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/presets.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/bifrost.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/bifrost.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         Outer joins are unsafe because the join constraint is not applied to the
         rows that would be considered "outer."
         """
         with open(_GRAMMAR_PATH, "r") as h:
             grammar = Lark(
                 ambiguity="explicit",
                 maybe_placeholders=False,
+                propagate_positions=True,
                 grammar=h,
             )
         return grammar
 
     @classmethod
     def reserved_keywords(self) -> set[str]:
         return presets.reserved_keywords
+
+    @classmethod
+    def placeholder(cls, name: str) -> str:
+        return f"%({name})s"
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/envelope.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/grammar.lark` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/grammar.lark`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ?start : full_query
 full_query : select_statement unions?
 
 unions : union+
 union : UNION (ALL | DISTINCT)? select_statement
 
 select_statement : \
-    SELECT DISTINCT? selected_columns \
-    FROM selected_table \
-    joins? \
-    where_clause? \
-    group_by_clause? \
-    having_clause? \
-    order_by_clause? \
+    SELECT _WS DISTINCT? selected_columns \
+    _WS FROM selected_table \
+    (_WS joins)? \
+    (_WS where_clause)? \
+    (_WS group_by_clause)? \
+    (_WS having_clause)? \
+    (_WS order_by_clause)? \
     limit_placeholder \
     SEMICOLON?
 
 // we use a placeholder for the limit clause because we need to be able to insert one
 // automatically in the case of reconstruction. if we didn't have a placeholder, we'd
 // have to examine ever clause child in `select_statement` to try to figure out where
 // to insert our new limit. having a placeholder simplifies this greatly.
@@ -33,79 +33,81 @@
 table_name : quoted_identifier | unquoted_identifier
 table_alias : generic_alias
 
 selected_columns : selected_column ("," selected_column)*
 // a selected column can be a value, not just a column name. a value encapsulates
 // fully qualified column names, and also functions that use column names
 selected_column : aliased_column | COUNT_STAR | value | ALL_COLUMNS
-aliased_column : (value | COUNT_STAR) as column_alias
+aliased_column : (value | COUNT_STAR) as generic_alias
 // this is a "fully-qualified" column name, meaning it just has a table name prefixing
 // it. keep in mind that the table may be an alias.
 fq_column : table_name "." column_name
 column_name : quoted_identifier | unquoted_identifier
 column_alias : generic_alias
 
 // having one generic alias rule makes it easier to check for reserved keywords
 generic_alias : quoted_identifier | unquoted_identifier
 
 joins : join+
-join : join_type joined_table "on"i join_condition ("and"i join_condition)*
+join : join_type _WS joined_table _WS "on"i join_condition (_WS "and"i join_condition)*
 // note we do not allow outer joins. this is because we cannot control
 // the rows that are returned by the outer join, and we cannot depend on the
 // join conditions to restrict the returned rows.
 // https://www.sqlite.org/syntax/join-operator.html
 join_type : legal_join | illegal_join
 legal_join : INNER_JOIN
 illegal_join : CROSS_JOIN | NATURAL_JOIN | OUTER_JOIN | NATURAL_OUTER_JOIN
 join_condition : connecting_join_condition | required_comparison
 // one side can be any value, but the other side must be a column
 connecting_join_condition : fq_column EQUI_JOIN value
 joined_table : aliased_table | table_name
 
-group_by_clause : GROUP_BY group_by_column ("," group_by_column)*
+group_by_clause : GROUP_BY _WS group_by_column ("," group_by_column)*
 group_by_column : value
 
-having_clause : HAVING having_condition
+having_clause : HAVING _WS having_condition
 having_condition : value comparison value
 
-order_by_clause : ORDER_BY order_column ("," order_column)*
-order_column : (COUNT_STAR | value) SORT_ORDER?
+order_by_clause : ORDER_BY _WS order_column ("," order_column)*
+order_column : (COUNT_STAR | value) (_WS SORT_ORDER)?
 SORT_ORDER : ASC | DESC
 
-limit_clause : LIMIT (((offset ",")? limit) | (limit OFFSET offset))
+limit_clause : LIMIT (_WS ((offset ",")? limit) | (limit _WS OFFSET _WS offset))
 limit : NUMBER
 offset : NUMBER
 
-where_clause : WHERE where_conditions
-where_conditions : where_condition (WHERE_TYPE where_condition)*
+where_clause : WHERE _WS where_conditions
+where_conditions : where_condition (_WS WHERE_TYPE _WS where_condition)*
 where_condition : \
     | required_comparison
     | relational_comparison
     | in_comparison
     | between_comparison
     | "(" where_conditions ")"
 
 // a required comparison is a parameterized, equality-based comparison that
 // enforces a constraint on the returned rows.
-required_comparison.1 : (fq_column | column_alias) "=" placeholder
+required_comparison.1 : lhs_req_comparison | rhs_req_comparison
+lhs_req_comparison : (fq_column | column_alias) "=" placeholder
+rhs_req_comparison : placeholder "=" (fq_column | column_alias)
 relational_comparison : value comparison value
 comparison : \
     EQ
     | NEQ
     | LT
     | GT
     | LTE
     | GTE
     | NOT? LIKE
     | IS NOT?
     | SOUNDS_LIKE
     | NOT? (REGEXP | RLIKE)
-in_comparison : value NOT? IN in_list
+in_comparison : value _WS NOT? _WS IN _WS in_list
 in_list : "(" value ("," value)* ")"
-between_comparison : value NOT? BETWEEN value AND value
+between_comparison : value _WS NOT? _WS BETWEEN _WS value _WS AND _WS value
 
 // for everywhere but the SELECT clause, because that's where column aliases
 // are declared, so we cannot use this there
 ?value : NUMBER
     | string
     | boolean
     | NULL
@@ -116,50 +118,49 @@
     | NUMBER_PREFIX? wrapped_value
 wrapped_value : LPAREN value RPAREN
 ?value_expr : function | arith_expr
 ?arith_expr : value ARITH_OP value (ARITH_OP value)*
 
 // a function with any number of arguments
 function : function_name "(" \
-        AGG_FN_MODIFIER? (value ("," value)*)? \
+        (AGG_FN_MODIFIER _WS)? (value ("," value)*)? \
     ")"
 function_name : /[a-zA-Z_]+/
 
 ?boolean : TRUE | FALSE
 ?string : ESCAPED_STRING
 
 // a placeholder for a value passed in as a parameter at query execution time
 placeholder: ":" IDENTIFIER
 
-
 SELECT : "select"i
 FROM : "from"i
 DISTINCT : "distinct"i
 ALL : "all"i
 UNION : "union"i
 SEMICOLON : ";"
 ALL_COLUMNS : "*"
 WHERE : "where"i
 WHERE_TYPE : AND | OR
-ORDER_BY : "order"i WS "by"i
+ORDER_BY : "order"i _WS "by"i
 LIMIT : "limit"i
 OFFSET : "offset"i
-GROUP_BY : "group"i WS "by"i
+GROUP_BY : "group"i _WS "by"i
 HAVING : "having"i
 
 // this is the only way that a query can have a "*" column spec, because it
 // doesn't reveal any information that would be restricted.
-COUNT_STAR : "count"i "(" AGG_FN_MODIFIER? ("*" | "1") ")"
+COUNT_STAR : "count"i "(" (AGG_FN_MODIFIER _WS)? ("*" | "1") ")"
 AGG_FN_MODIFIER : DISTINCT | ALL
 
-INNER_JOIN : ("inner"i WS)? "join"i
-CROSS_JOIN : "cross"i WS "join"i
-NATURAL_JOIN : "natural"i WS (("left"i | "right"i | "full"i | "inner"i) WS)? "join"i
-OUTER_JOIN : ("left"i | "right"i | "full"i) WS ("outer"i WS)? "join"i
-NATURAL_OUTER_JOIN : "natural"i WS (("left"i | "right"i | "full"i) WS)? "outer"i WS "join"i
+INNER_JOIN : ("inner"i _WS)? "join"i
+CROSS_JOIN : "cross"i _WS "join"i
+NATURAL_JOIN : "natural"i _WS (("left"i | "right"i | "full"i | "inner"i) _WS)? "join"i
+OUTER_JOIN : ("left"i | "right"i | "full"i) _WS ("outer"i _WS)? "join"i
+NATURAL_OUTER_JOIN : "natural"i _WS (("left"i | "right"i | "full"i) _WS)? "outer"i _WS "join"i
 
 ASC : "asc"i
 DESC : "desc"i
 
 AND : "and"i
 OR : "or"i
 
@@ -177,15 +178,15 @@
 LT : "<"
 GT : ">"
 LTE : "<="
 GTE : ">="
 IS : "is"i
 BETWEEN : "between"i
 IN : "in"i
-SOUNDS_LIKE : "sounds"i WS "like"i
+SOUNDS_LIKE : "sounds"i _WS "like"i
 LIKE : "like"i
 NOT : "not"i
 REGEXP : "regexp"i
 RLIKE : "rlike"i
 
 TRUE : "true"i
 FALSE : "false"i
@@ -207,14 +208,15 @@
     | "&"
     | "|"
     | "div"i
     | "mod"i
 
 // NOTE this is dialect specific
 ESCAPED_STRING : "'" _STRING_ESC_INNER "'" | "\"" _STRING_ESC_INNER "\""
+_WS : WS
 
 %import common.NUMBER
 %import common.DIGIT
 %import common.WORD
 %import common.WS
 %import common._STRING_ESC_INNER
 %ignore WS
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/validator.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/mysql/select/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/reconstruct.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/reconstruct.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import cast
+from typing import Generator, Iterable, cast
 
 from lark import Discard, Token
 from lark import Transformer as _Transformer
 from lark import Tree
 
 from . import exc
 from .common import FqColumn
@@ -55,14 +55,42 @@
 
     # adding a limit? just append it
     else:
         limit_tree = _build_limit_tree(max_limit)
         limit_placeholder.children.append(limit_tree)
 
 
+def qualify_column(fq_column: FqColumn) -> Tree:
+    """Replaces an alias node with a fully qualified column node."""
+    tree = Tree(
+        "fq_column",
+        [
+            Tree(
+                Token("RULE", "table_name"),
+                [
+                    Tree(
+                        Token("RULE", "unquoted_identifier"),
+                        [Token("IDENTIFIER", fq_column.table)],
+                    )
+                ],
+            ),
+            Tree(
+                Token("RULE", "column_name"),
+                [
+                    Tree(
+                        Token("RULE", "unquoted_identifier"),
+                        [Token("IDENTIFIER", fq_column.column)],
+                    )
+                ],
+            ),
+        ],
+    )
+    return tree
+
+
 class ReconstructTransformer(_Transformer):
     """makes some alterations to a query if it does not meet some basic validation
     constraints, but could with those alterations. currently, these are just the
     following:
 
         - adding or lowering a limit on the number of rows
         - removing illegal selected columns
@@ -98,14 +126,51 @@
         # if there's no children, it means we discarded every column selected, meaning
         # that they were all illegal columns. since we can't proceed without a column,
         # go ahead and raise an exception about illegal column.
         if not children:
             raise exc.IllegalSelectedColumn(column=self._last_discarded_column.name)
         return Tree("selected_columns", children)
 
+    def column_alias(self, children: list[Tree | Token]):
+        alias_name = get_identifier(children[0], self._reserved_keywords)
+
+        # if we can't find the actual table where this column alias comes from, assume
+        # the selected table.
+        fq_columns = self._collector._aliased_columns[alias_name]
+
+        # None means the alias is not based on any column (it's an expression of some
+        # kind), so we leave this node alone
+        if fq_columns is None:
+            tree = Tree("column_alias", children)
+
+        # if we haven't found any columns associated with this alias, it means that the
+        # query is implicitly using the selected table, so we can fully qualify it based
+        # on that information.
+        elif len(fq_columns) == 0:
+            tree = qualify_column(
+                FqColumn(
+                    table=cast(str, self._collector._selected_table),
+                    column=alias_name,
+                )
+            )
+
+        # if there's only one fq column associated with this alias, then we know it's
+        # not a composite alias, so we can fully qualify it.
+        elif len(fq_columns) == 1:
+            tree = qualify_column(next(iter(fq_columns)))
+
+        # if it's a composite alias, we can't fully qualify it, so we leave it alone.
+        elif len(fq_columns) > 1:
+            tree = Tree("column_alias", children)
+
+        else:
+            assert False, "Unreachable"
+
+        return tree
+
     def selected_column(self, children: list[Tree | Token]):
         """ensures that every selected column is allowed"""
         selected = children[0]
         if is_count_function(selected):
             pass
 
         elif isinstance(selected, Tree):
@@ -122,31 +187,16 @@
                 if not self._validator.select_column_allowed(column):
                     self._last_discarded_column = column
                     return Discard
 
         return Tree("selected_column", children)
 
 
-def postproc(items):
-    """helps format our reconstructed query so it's not all on one line"""
-    for item in items:
-        if isinstance(item, Token):
-            if item.type in {
-                "FROM",
-                "GROUP_BY",
-                "HAVING",
-                "INNER_JOIN",
-                "LIMIT",
-                "OFFSET",
-                "ORDER_BY",
-                "WHERE",
-                "WHERE_TYPE",
-            }:
-                yield "\n"
-            else:
-                pass
-
-        yield item
-
-        if isinstance(item, Token):
-            if item.type in {}:
-                yield " "
+PostProcToken = Token | str
+
+
+def postproc(items: Iterable[PostProcToken]) -> Generator[PostProcToken, None, None]:
+    for token in items:
+        if token == "_WS":
+            yield " "
+            continue
+        yield token
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/presets.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/bifrost.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         Outer joins are unsafe because the join constraint is not applied to the
         rows that would be considered "outer."
         """
         with open(_GRAMMAR_PATH, "r") as h:
             grammar = Lark(
                 ambiguity="explicit",
                 maybe_placeholders=False,
+                propagate_positions=True,
                 grammar=h,
             )
         return grammar
 
     @classmethod
     def reserved_keywords(self) -> set[str]:
         return presets.reserved_keywords
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/grammar.lark` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/grammar.lark`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ?start : full_query
 full_query : select_statement unions?
 
 unions : union+
 union : UNION (ALL | DISTINCT)? select_statement
 
 select_statement : \
-    SELECT DISTINCT? selected_columns \
-    FROM selected_table \
-    joins? \
-    where_clause? \
-    group_by_clause? \
-    having_clause? \
-    order_by_clause? \
+    SELECT _WS DISTINCT? selected_columns \
+    _WS FROM selected_table \
+    (_WS joins)? \
+    (_WS where_clause)? \
+    (_WS group_by_clause)? \
+    (_WS having_clause)? \
+    (_WS order_by_clause)? \
     limit_placeholder \
     SEMICOLON?
 
 // we use a placeholder for the limit clause because we need to be able to insert one
 // automatically in the case of reconstruction. if we didn't have a placeholder, we'd
 // have to examine ever clause child in `select_statement` to try to figure out where
 // to insert our new limit. having a placeholder simplifies this greatly.
@@ -35,79 +35,81 @@
 table_name : quoted_identifier | unquoted_identifier
 table_alias : generic_alias
 
 selected_columns : selected_column ("," selected_column)*
 // a selected column can be a value, not just a column name. a value encapsulates
 // fully qualified column names, and also functions that use column names
 selected_column : aliased_column | COUNT_STAR | value | ALL_COLUMNS
-aliased_column : (value | COUNT_STAR) as column_alias
+aliased_column : (value | COUNT_STAR) as generic_alias
 // this is a "fully-qualified" column name, meaning it just has a table name prefixing
 // it. keep in mind that the table may be an alias.
 fq_column : table_name "." column_name
 column_name : quoted_identifier | unquoted_identifier
 column_alias : generic_alias
 
 // having one generic alias rule makes it easier to check for reserved keywords
 generic_alias : quoted_identifier | unquoted_identifier
 
 joins : join+
-join : join_type joined_table "on"i join_condition ("and"i join_condition)*
+join : join_type _WS joined_table _WS "on"i join_condition (_WS "and"i join_condition)*
 // note we do not allow outer joins. this is because we cannot control
 // the rows that are returned by the outer join, and we cannot depend on the
 // join conditions to restrict the returned rows.
 // https://www.sqlite.org/syntax/join-operator.html
 join_type : legal_join | illegal_join
 legal_join : INNER_JOIN
 illegal_join : CROSS_JOIN | NATURAL_JOIN | OUTER_JOIN | NATURAL_OUTER_JOIN
 join_condition : connecting_join_condition | required_comparison
 // one side can be any value, but the other side must be a column
 connecting_join_condition : fq_column EQUI_JOIN value
 joined_table : aliased_table | table_name
 
-group_by_clause : GROUP_BY group_by_column ("," group_by_column)*
+group_by_clause : GROUP_BY _WS group_by_column ("," group_by_column)*
 group_by_column : value
 
-having_clause : HAVING having_condition
+having_clause : HAVING _WS having_condition
 having_condition : value comparison value
 
-order_by_clause : ORDER_BY order_column ("," order_column)*
-order_column : (COUNT_STAR | value) SORT_ORDER?
+order_by_clause : ORDER_BY _WS order_column ("," order_column)*
+order_column : (COUNT_STAR | value) (_WS SORT_ORDER)?
 SORT_ORDER : ASC | DESC
 
-limit_clause : LIMIT (((offset ",")? limit) | (limit OFFSET offset))
+limit_clause : LIMIT (_WS ((offset ",")? limit) | (limit _WS OFFSET _WS offset))
 limit : NUMBER
 offset : NUMBER
 
-where_clause : WHERE where_conditions
-where_conditions : where_condition (WHERE_TYPE where_condition)*
+where_clause : WHERE _WS where_conditions
+where_conditions : where_condition (_WS WHERE_TYPE _WS where_condition)*
 where_condition : \
     | required_comparison
     | relational_comparison
     | in_comparison
     | between_comparison
     | "(" where_conditions ")"
 
 // a required comparison is a parameterized, equality-based comparison that
 // enforces a constraint on the returned rows.
-required_comparison.1 : (fq_column | column_alias) "=" placeholder
+required_comparison.1 : lhs_req_comparison | rhs_req_comparison
+lhs_req_comparison : (fq_column | column_alias) "=" placeholder
+rhs_req_comparison : placeholder "=" (fq_column | column_alias)
 relational_comparison : value comparison value
 comparison : \
     EQ
     | NEQ
     | LT
     | GT
     | LTE
     | GTE
     | NOT? LIKE
     | IS NOT?
     | SOUNDS_LIKE
     | NOT? (REGEXP | RLIKE)
-in_comparison : value NOT? IN in_list
+in_comparison : value _WS NOT? _WS IN _WS in_list
 in_list : "(" value ("," value)* ")"
-between_comparison : value NOT? BETWEEN value AND value
+between_comparison : value _WS NOT? _WS BETWEEN _WS value _WS AND _WS value
 
 // for everywhere but the SELECT clause, because that's where column aliases
 // are declared, so we cannot use this there
 ?value : NUMBER
     | string
     | boolean
     | NULL
@@ -118,51 +120,49 @@
     | NUMBER_PREFIX? wrapped_value
 wrapped_value : LPAREN value RPAREN
 ?value_expr : function | arith_expr
 ?arith_expr : value ARITH_OP value (ARITH_OP value)*
 
 // a function with any number of arguments
 function : function_name "(" \
-        AGG_FN_MODIFIER? (value ("," value)*)? \
+        (AGG_FN_MODIFIER _WS)? (value ("," value)*)? \
     ")"
 function_name : /[a-zA-Z_]+/
 
 ?boolean : TRUE | FALSE
 ?string : ESCAPED_STRING
 
 // a placeholder for a value passed in as a parameter at query execution time
-// https://docs.python.org/2/library/sqlite3.html#sqlite3.Cursor.execute
 placeholder: ":" IDENTIFIER
 
-
 SELECT : "select"i
 FROM : "from"i
 DISTINCT : "distinct"i
 ALL : "all"i
 UNION : "union"i
 SEMICOLON : ";"
 ALL_COLUMNS : "*"
 WHERE : "where"i
 WHERE_TYPE : AND | OR
-ORDER_BY : "order"i WS "by"i
+ORDER_BY : "order"i _WS "by"i
 LIMIT : "limit"i
 OFFSET : "offset"i
-GROUP_BY : "group"i WS "by"i
+GROUP_BY : "group"i _WS "by"i
 HAVING : "having"i
 
 // this is the only way that a query can have a "*" column spec, because it
 // doesn't reveal any information that would be restricted.
-COUNT_STAR : "count"i "(" AGG_FN_MODIFIER? ("*" | "1") ")"
+COUNT_STAR : "count"i "(" (AGG_FN_MODIFIER _WS)? ("*" | "1") ")"
 AGG_FN_MODIFIER : DISTINCT | ALL
 
-INNER_JOIN : ("inner"i WS)? "join"i
-CROSS_JOIN : "cross"i WS "join"i
-NATURAL_JOIN : "natural"i WS (("left"i | "right"i | "full"i | "inner"i) WS)? "join"i
-OUTER_JOIN : ("left"i | "right"i | "full"i) WS ("outer"i WS)? "join"i
-NATURAL_OUTER_JOIN : "natural"i WS (("left"i | "right"i | "full"i) WS)? "outer"i WS "join"i
+INNER_JOIN : ("inner"i _WS)? "join"i
+CROSS_JOIN : "cross"i _WS "join"i
+NATURAL_JOIN : "natural"i _WS (("left"i | "right"i | "full"i | "inner"i) _WS)? "join"i
+OUTER_JOIN : ("left"i | "right"i | "full"i) _WS ("outer"i _WS)? "join"i
+NATURAL_OUTER_JOIN : "natural"i _WS (("left"i | "right"i | "full"i) _WS)? "outer"i _WS "join"i
 
 ASC : "asc"i
 DESC : "desc"i
 
 AND : "and"i
 OR : "or"i
 
@@ -180,15 +180,15 @@
 LT : "<"
 GT : ">"
 LTE : "<="
 GTE : ">="
 IS : "is"i
 BETWEEN : "between"i
 IN : "in"i
-SOUNDS_LIKE : "sounds"i WS "like"i
+SOUNDS_LIKE : "sounds"i _WS "like"i
 LIKE : "like"i
 NOT : "not"i
 REGEXP : "regexp"i
 RLIKE : "rlike"i
 
 TRUE : "true"i
 FALSE : "false"i
@@ -213,13 +213,14 @@
     | "mod"i
 
 // in sqlite, double quotes are used for quoting identifiers, single quotes for quoting
 // strings. also, a single quote can be escaped by doubling it, and there are no other
 // escape sequences. https://www.sqlite.org/faq.html#q14 the below inner regex says "any
 // character except a single quote, unless it is doubled"
 ESCAPED_STRING : "'" /([^']|'')*/ "'"
+_WS : WS
 
 %import common.NUMBER
 %import common.DIGIT
 %import common.WORD
 %import common.WS
 %ignore WS
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/validator.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/sqlite/select/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/identifier.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/utils/identifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,16 +29,21 @@
 
 def is_count_function(node: Tree | Token) -> bool:
     """
     A helper for determining if a node is a *safe* aggregate function. We allow safe
     aggregate functions in the SELECT clause, because they don't reveal extra
     information.
     """
+    # count(*) or count(1)
+    if isinstance(node, Token) and node.type == "COUNT_STAR":
+        return True
+
     if isinstance(node, Tree):
         if node.data == "aliased_column":
             node = node.children[0]
 
+    # count(column) or count(some_other_expression)
     if isinstance(node, Tree) and node.data == "function":
         fn_name = cast(Token, node.children[0].children[0]).value.lower()
         if fn_name == "count":
             return True
     return False
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/validator.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from itertools import chain
 from typing import Optional, Sequence, cast
 
-from lark import Lark, ParseTree
+from lark import Lark, ParseTree, Token
 from lark.exceptions import VisitError
 from lark.reconstruct import Reconstructor
 
 from heimdallm.bifrost import Bifrost
 from heimdallm.bifrosts.sql import exc
 from heimdallm.bifrosts.sql.bifrost import Bifrost as _SQLBifrost
 from heimdallm.constraints import ConstraintValidator as _BaseConstraintValidator
@@ -163,15 +163,18 @@
         try:
             fixed_tree = transform.transform(tree)
         except VisitError as e:
             if isinstance(e.orig_exc, exc.BaseException):
                 raise e.orig_exc
             raise e
 
-        output = Reconstructor(grammar).reconstruct(
+        def special(sym):
+            return Token("IGNORE", sym.name)
+
+        output = Reconstructor(grammar, {"_WS": special}).reconstruct(
             fixed_tree,
             postproc=reconstruct.postproc,
         )
         return output
 
     def validate(self, bifrost: Bifrost, untrusted_input: str, tree: ParseTree):
         """Analyze the parsed tree and validate it against our SQL constraints
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/aliases.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/aliases.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,91 @@
-from lark import Token, Tree, Visitor
+from collections import defaultdict as dd
+from typing import cast
 
-from ..utils.identifier import get_identifier
+from lark import Tree, Visitor
+
+from ..common import FqColumn
+from ..utils.identifier import get_identifier, is_count_function
 
 
 class AliasCollector(Visitor):
     """collects all of our table and column aliases and maps them back to the
     authoritative name. we have to do this pass first, before any other passes,
     because the tree may not evaluate in the order that would allow us to
     resolve aliases."""
 
     def __init__(self, reserved_keywords: set[str]):
         # aliased table names from the FROM clause, as well as JOIN clauses.
         # they map from the alias name to the table name.
         self._aliased_tables: dict[str, str] = {}
-        # aliased column names from the SELECT clause. they map from the alias
-        # name to the (table, column) tuple
-        self._aliased_columns: dict[str, tuple[str | None, str | None]] = {}
+        # aliased column names from the SELECT clause. they map from the alias name to
+        # the a collection of fully qualified column names. the reason why it's a
+        # collection is because a single alias can be a composite alias consisting of
+        # multiple columns, for example, ``(a + b) as c``.
+        #
+        # a None value means that the alias cannot have any associated columns, which
+        # can happen for aliases based on an expression, and not columns.
+        self._aliased_columns: dict[str, set[FqColumn] | None] = dd(set)
         self._reserved_keywords = reserved_keywords
+        self._selected_table: str | None = None
 
     def _resolve_table(self, table):
         return self._aliased_tables.get(table, table)
 
+    def selected_table(self, node: Tree):
+        self._selected_table = get_identifier(node, self._reserved_keywords)
+
     # tables are aliased in the FROM clause of a SELECT statement, or when a
     # table is JOINed. it's here that we know the authoritative table name and
-    # its aliased, which may be used in other parts of the query
+    # its alias, which may be used in other parts of the query
     def aliased_table(self, node: Tree):
         table_node, _as, alias_node = node.children
         table_name = get_identifier(table_node, self._reserved_keywords)
         alias = get_identifier(alias_node, self._reserved_keywords)
         self._aliased_tables[alias] = table_name
 
-        # inefficient, but backfill the correct table alias for any columns
-        for key, (tn, cn) in list(self._aliased_columns.items()):
-            if tn == alias:
-                self._aliased_columns[key] = (table_name, cn)
+        # inefficient, but backfill the correct table alias for any columns. we must do
+        # some form of this because we may have recorded a column alias, e.g. ``r.amt as
+        # amt``, before knowing the table alias, e.g. ``rental as r``. so for each
+        # aliased table that we resolve, we need to make sure the column aliases reflect
+        # that table alias correctly. this could be more efficient.
+        for fq_columns in self._aliased_columns.values():
+            if fq_columns:
+                for fq_column in fq_columns:
+                    if fq_column.table == alias:
+                        fq_column.table = table_name
 
     # columns are aliased in the column list of a SELECT statement. we assume
     # that all aliased columns are fully qualified by table name. note, however,
     # that the table name may be an alias itself.
     def aliased_column(self, node: Tree):
         value_node, _as, alias_node = node.children
         alias_name = get_identifier(alias_node, self._reserved_keywords)
 
-        if isinstance(value_node, Token):
-            if value_node.type == "COUNT_STAR":
-                self._aliased_columns[alias_name] = (None, None)
+        # if it's a count function, we don't care what it's composed of, because it
+        # doesn't reveal any information about the underlying data. so we don't use it
+        # for resolving aliases
+        if is_count_function(value_node):
+            self._aliased_columns[alias_name] = None
             return
 
         # there may be multiple columns referenced in this alias column, for
         # example if we're running a function on multiple columns and aliasing
         # the result. so we need to look at each fq_column individually
+        inserted_fq_alias = False
         for fq_column_node in value_node.find_data("fq_column"):
             table_node, column_node = fq_column_node.children
             table_name = get_identifier(table_node, self._reserved_keywords)
             column_name = get_identifier(column_node, self._reserved_keywords)
 
             # do we already have a table alias for this column? use that instead for
             # the table name
             table_name = self._resolve_table(table_name)
-            self._aliased_columns[alias_name] = (table_name, column_name)
+            composite_columns = cast(set[FqColumn], self._aliased_columns[alias_name])
+            composite_columns.add(FqColumn(table=table_name, column=column_name))
+            inserted_fq_alias = True
+
+        # if we didn't insert an alias at this point, it means it's an expression that
+        # is being an aliased. something like ``1 + 1 as name``. so we set it to None so
+        # that we don't try to autofix it later to be a fully qualified column.
+        if not inserted_fq_alias:
+            self._aliased_columns[alias_name] = None
```

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/ambiguity.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/ambiguity.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/facets.py` & `heimdallm-0.3.0/heimdallm/bifrosts/sql/visitors/facets.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,18 @@
         collector: AliasCollector,
         reserved_keywords: set[str],
     ):
         self._collector = collector
         self._facets = facets
         self._reserved_keywords = reserved_keywords
 
-    def _resolve_column(self, node: Tree):
+    def _resolve_column(self, node: Tree) -> set[FqColumn] | None:
         if node.data == "column_alias":
             maybe_alias = get_identifier(node, self._reserved_keywords)
-            table, column = self._collector._aliased_columns.get(
-                maybe_alias, (None, maybe_alias)
-            )
-            return table, column
+            return self._collector._aliased_columns[maybe_alias]
 
         # should never happen
         raise RuntimeError(f"unknown column reference type: {type(node)}")
 
     def _resolve_table(self, table_ref: Tree | Token):
         if isinstance(table_ref, Tree):
             if table_ref.data == "aliased_table":
@@ -161,36 +158,36 @@
         # reveal any of the underlying values
         elif is_count_function(child):
             return
 
         elif isinstance(child, Tree):
             # if it's an aliased column, we need to ensure that the thing being aliased
             # isn't a non-fully-qualified column. we do that by looking for
-            # `column_alias`
+            # `generic_alias`
             if child.data == "aliased_column":
                 alias_child = child.children[0]
                 # if we're aliasing COUNT(*), it's safe to ignore, since it doesn't
                 # reveal any of the underlying values
                 if isinstance(alias_child, Token) and alias_child.type == "COUNT_STAR":
                     return
 
-                if list(alias_child.find_data("column_alias")):
+                if list(alias_child.find_data("generic_alias")):
                     alias = get_identifier(alias_child, self._reserved_keywords)
                     raise exc.UnqualifiedColumn(column=alias)
 
             # if the column looks like a column alias (meaning a non-fully-qualified
             # column), then that's an error, because we only work with fully-qualified
             # columns
-            elif child.data == "column_alias":
+            elif child.data == "generic_alias":
                 alias = get_identifier(child, self._reserved_keywords)
                 raise exc.UnqualifiedColumn(column=alias)
 
             # if we're not an aliased column, but we contain a column alias somewhere,
             # that's an error, because we only work with fully-qualified columns
-            elif column_alias := list(child.find_data("column_alias")):
+            elif column_alias := list(child.find_data("generic_alias")):
                 alias = get_identifier(column_alias[0], self._reserved_keywords)
                 raise exc.UnqualifiedColumn(column=alias)
 
             # if we've made it this far, we're sure we're dealing with a fully-qualified
             # column, or a non-column based expression
             try:
                 table_node = next(child.find_data("table_name"))
@@ -212,38 +209,72 @@
                         column=column_name,
                     )
                 )
 
     def _add_required_comparison(self, node: Tree):
         """takes a node representing a required comparison and adds it to the
         facets"""
-        maybe_fq_column_node, placeholder = node.children
+
+        # handle both a forwards (column = :placeholder) and backwards (:placeholder =
+        # column)
+        if list(node.find_data("lhs_req_comparison")):
+            maybe_fq_column_node, placeholder = node.children[0].children
+        else:
+            placeholder, maybe_fq_column_node = node.children[0].children
+
         placeholder_name = cast(Token, placeholder.children[0]).value
 
         if maybe_fq_column_node.data == "column_alias":
-            table_name, column_name = self._resolve_column(maybe_fq_column_node)
+            maybe_fq_columns = self._resolve_column(maybe_fq_column_node)
+
+            # none means the alias is based on an expression, so we don't need to add it
+            # to the required constraints because it's not a column
+            if maybe_fq_columns is None:
+                return
+
+            # multiple columns means the alias is based on a composite expression, so we
+            # cannot determine which column to add to the required constraints, so we
+            # add none of them
+            elif len(maybe_fq_columns) > 1:
+                return
+
+            # no columns means the alias was never resolved. i don't think we should
+            # ever end up down this path
+            elif len(maybe_fq_columns) == 0:
+                assert False, "Unreachable"
+
+            # otherwise we have one column backing the alias, so we add it to the
+            # required constraints that were found.
+            elif len(maybe_fq_columns) == 1:
+                fq_column = next(iter(maybe_fq_columns))
+                self._facets.required_constraints.add(
+                    RequiredConstraint(
+                        column=fq_column.name,
+                        placeholder=placeholder_name,
+                    )
+                )
 
         elif maybe_fq_column_node.data == "fq_column":
             fq_column_node = maybe_fq_column_node
             table_node, column_node = fq_column_node.children
 
             table_name = self._resolve_table(table_node)
             column_name = get_identifier(column_node, self._reserved_keywords)
+
+            self._facets.required_constraints.add(
+                RequiredConstraint(
+                    column=f"{table_name}.{column_name}",
+                    placeholder=placeholder_name,
+                )
+            )
         else:
             raise RuntimeError(
                 f"Unknown required column type {type(maybe_fq_column_node)}"
             )
 
-        self._facets.required_constraints.add(
-            RequiredConstraint(
-                column=f"{table_name}.{column_name}",
-                placeholder=placeholder_name,
-            )
-        )
-
     def where_clause(self, where_node: Tree):
         """here we'll do a breadth-first search on the where clause, going level
         by level. if any level contains an "OR", that means the entire level is
         tainted and can't be used for a required constraint, because the
         required constraint may be optional.
 
         if a level is tainted, then all of its children (WHERE subclauses) are
@@ -287,30 +318,28 @@
                 FqColumn(
                     table=table_name,
                     column=column_name,
                 )
             )
 
         for column_alias_node in node.find_data("column_alias"):
-            table_name, column_name = self._resolve_column(column_alias_node)
-            if not table_name:
-                # no table name AND no column name means the inserted alias is an alias
-                # for a non-column expression, like `COUNT(*) as thing`. this is valid
-                # as it is, so we don't raise, and we don't track it as a condition
-                # column.
-                if not column_name:
-                    pass
-                else:
-                    raise exc.UnqualifiedColumn(column=column_name)
-            self._facets.condition_columns.add(
-                FqColumn(
-                    table=table_name,
-                    column=column_name,
-                )
-            )
+            maybe_fq_columns = self._resolve_column(column_alias_node)
+
+            # a None means this is a non-column expression alias. this is valid as it
+            # is, so we don't raise, and we don't track it as a condition column.
+            if maybe_fq_columns is None:
+                pass
+            # we have a single underlying column, or multiple composite columns. add all
+            # of them to our condition columns.
+            elif len(maybe_fq_columns) > 0:
+                self._facets.condition_columns.update(maybe_fq_columns)
+            # we have no columns that resolve the alias. this is an error.
+            else:
+                column_name = get_identifier(column_alias_node, self._reserved_keywords)
+                raise exc.UnqualifiedColumn(column=column_name)
 
     where_condition = _collect_condition_column
     having_condition = _collect_condition_column
     order_column = _collect_condition_column
 
     def limit(self, node: Tree):
         self._facets.limit = int(cast(Token, node.children[0]).value)
```

### Comparing `heimdallm-0.2.1/heimdallm/constraints.py` & `heimdallm-0.3.0/heimdallm/constraints.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/envelope.py` & `heimdallm-0.3.0/heimdallm/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/llm.py` & `heimdallm-0.3.0/heimdallm/llm.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/llm_providers/mock.py` & `heimdallm-0.3.0/heimdallm/llm_providers/mock.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/llm_providers/openai.py` & `heimdallm-0.3.0/heimdallm/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/heimdallm/support/github.py` & `heimdallm-0.3.0/heimdallm/support/github.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.1/pyproject.toml` & `heimdallm-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heimdallm"
-version = "0.2.1"
+version = "0.3.0"
 description = "Construct trusted SQL queries from untrusted input"
 homepage = "https://github.com/amoffat/HeimdaLLM"
 repository = "https://github.com/amoffat/HeimdaLLM"
 documentation = "https://heimdallm.readthedocs.io/en/latest/"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 maintainers = ["Andrew Moffat <arwmoffat@gmail.com>"]
 keywords = ["sql", "llm", "ai"]
```

### Comparing `heimdallm-0.2.1/PKG-INFO` & `heimdallm-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heimdallm
-Version: 0.2.1
+Version: 0.3.0
 Summary: Construct trusted SQL queries from untrusted input
 Home-page: https://github.com/amoffat/HeimdaLLM
 License: AGPL-3.0
 Keywords: sql,llm,ai
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
```

