# Comparing `tmp/landingzone_organization-0.5.0.tar.gz` & `tmp/landingzone_organization-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.5.0.tar", max compression
+gzip compressed data, was "landingzone_organization-0.6.1.tar", max compression
```

## Comparing `landingzone_organization-0.5.0.tar` & `landingzone_organization-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      981 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/README.md
--rw-r--r--   0        0        0      636 2023-06-20 08:57:49.282397 landingzone_organization-0.5.0/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      395 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0     1242 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      558 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0     2096 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/profiles.py
--rw-r--r--   0        0        0      707 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1517 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      666 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/groups.py
--rw-r--r--   0        0        0     3220 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      917 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/profile.py
--rw-r--r--   0        0        0     1164 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/profiles.py
--rw-r--r--   0        0        0      887 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1559 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1386 2023-06-20 08:57:49.282397 landingzone_organization-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      981 2023-07-16 14:31:58.411204 landingzone_organization-0.6.1/README.md
+-rw-r--r--   0        0        0      636 2023-07-16 14:31:59.271248 landingzone_organization-0.6.1/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      558 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0     2096 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/profiles.py
+-rw-r--r--   0        0        0      707 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1517 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      955 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1035 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     3220 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      917 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/profile.py
+-rw-r--r--   0        0        0     1164 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/profiles.py
+-rw-r--r--   0        0        0      906 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1559 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1386 2023-07-16 14:31:59.271248 landingzone_organization-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.6.1/PKG-INFO
```

### Comparing `landingzone_organization-0.5.0/README.md` & `landingzone_organization-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/__init__.py` & `landingzone_organization-0.6.1/landingzone_organization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from landingzone_organization.organization_unit import OrganizationUnit
 from landingzone_organization.account import Account
 from landingzone_organization.groups import Groups
 from landingzone_organization.group import Group
 from landingzone_organization.profile import Profile
 from landingzone_organization.profiles import Profiles
 
-__version__ = "0.5.0"
+__version__ = "0.6.1"
 __all__ = [
     AWSOrganization,
     Organization,
     OrganizationUnit,
     Account,
     Groups,
     Group,
```

### Comparing `landingzone_organization-0.5.0/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.6.1/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/commands/account.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/commands/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,21 @@
         click.echo(f"Name        : {account.name}")
         click.echo(f"Environment : {account.environment}")
     else:
         click.echo(f"The {account_id} is not known to this organization.")
 
 
 @cli.command()
-@click.argument('output')
+@click.argument("output")
 @click.pass_obj
 def export(ctx: Context, output: str):
     """List all workloads"""
     perform_export(output, ctx.organization.accounts([]))
 
 
 def perform_export(path: str, accounts: List[Account]) -> None:
     with open(path, "w") as fh:
         writer = csv.writer(fh, delimiter=";", quotechar='"', quoting=csv.QUOTE_ALL)
-        writer.writerow([
-            "AccountId", "Name", "Environment"
-        ])
+        writer.writerow(["AccountId", "Name", "Environment"])
 
     for account in accounts:
         writer.writerow([account.account_id, account.name, account.environment])
```

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/commands/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/commands/profiles.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/commands/workload.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/commands/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/context.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/cli/handler.py` & `landingzone_organization-0.6.1/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/filtering.py` & `landingzone_organization-0.6.1/landingzone_organization/filtering.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from __future__ import annotations
 
 import os
 import re
 from typing import Optional
 
-
 PATTERN_WORKLOAD_NAME = os.environ.get("PATTERN_WORKLOAD_NAME", ".*?-(.*)-.*")
 PATTERN_ENVIRONMENT_NAME = os.environ.get("PATTERN_ENVIRONMENT_NAME", ".*-.*-(.*)")
+ENVIRONMENT_WEIGHT = os.environ.get("ENVIRONMENT_WEIGHT", "dev,test,acc,prod")
 
 
 def match_workload_pattern(name: str) -> bool:
     return bool(re.match(PATTERN_WORKLOAD_NAME, name))
 
 
 def resolve_workload_name(name: str) -> Optional[str]:
     match = re.match(PATTERN_WORKLOAD_NAME, name)
     return match.group(1) if match else None
 
 
 def resolve_account_environment(name: str) -> Optional[str]:
     match = re.match(PATTERN_ENVIRONMENT_NAME, name)
     return match.group(1) if match else None
+
+
+def resolve_account_weight(name: str) -> int:
+    order = ENVIRONMENT_WEIGHT.split(",")
+    item = next(filter(lambda x: name.startswith(x), order), None)
+
+    return order.index(item) if item else len(order)
```

### Comparing `landingzone_organization-0.5.0/landingzone_organization/group.py` & `landingzone_organization-0.6.1/landingzone_organization/group.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/groups.py` & `landingzone_organization-0.6.1/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/organization.py` & `landingzone_organization-0.6.1/landingzone_organization/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/organization_unit.py` & `landingzone_organization-0.6.1/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/profile.py` & `landingzone_organization-0.6.1/landingzone_organization/profile.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/profiles.py` & `landingzone_organization-0.6.1/landingzone_organization/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/landingzone_organization/workload.py` & `landingzone_organization-0.6.1/landingzone_organization/workload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-import re
-from typing import List, Optional, Set
+from typing import List, Optional
 
 from landingzone_organization.account import Account
 
 
 class Workload:
     def __init__(self, name: str, accounts: List[Account]) -> None:
         self.__name = name
@@ -12,19 +11,19 @@
 
     @property
     def name(self) -> str:
         return self.__name
 
     @property
     def accounts(self) -> List[Account]:
-        return self.__accounts
+        return sorted(self.__accounts, key=lambda x: x.weight)
 
     @property
-    def environments(self) -> Set[str]:
-        return set(map(lambda account: str(account.environment), self.accounts))
+    def environments(self) -> List[str]:
+        return list(map(lambda account: str(account.environment), self.accounts))
 
     def by_environment(self, name: str) -> Optional[Account]:
         def match(account: Account):
             return account.environment == name
 
         return next(filter(match, self.accounts), None)  # type: ignore
```

### Comparing `landingzone_organization-0.5.0/landingzone_organization/workloads.py` & `landingzone_organization-0.6.1/landingzone_organization/workloads.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.5.0/pyproject.toml` & `landingzone_organization-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.5.0"
+version = "0.6.1"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 homepage = "https://binxio.github.io/landingzone-organization/"
 documentation = "https://binxio.github.io/landingzone-organization/3-user-documentation/"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
@@ -22,21 +22,21 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.83"
 click = "^8.1.3"
 jsonpickle = "^3.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 black = "^23.1.0"
 radon = "^5.1.0"
 xenon = "^0.9.0"
-mypy = "^1.0.1"
-aws-sam-cli = "^1.78.0"
+mypy = "^1.4.1"
+aws-sam-cli = "^1.90.0"
 
 [tool.poetry.scripts]
 landingzone-organization = "landingzone_organization.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
```

### Comparing `landingzone_organization-0.5.0/PKG-INFO` & `landingzone_organization-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingzone-organization
-Version: 0.5.0
+Version: 0.6.1
 Summary: 
 Home-page: https://binxio.github.io/landingzone-organization/
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

