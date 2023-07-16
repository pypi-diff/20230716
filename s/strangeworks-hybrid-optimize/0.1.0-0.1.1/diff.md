# Comparing `tmp/strangeworks_hybrid_optimize-0.1.0.tar.gz` & `tmp/strangeworks_hybrid_optimize-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_hybrid_optimize-0.1.0.tar", max compression
+gzip compressed data, was "strangeworks_hybrid_optimize-0.1.1.tar", max compression
```

## Comparing `strangeworks_hybrid_optimize-0.1.0.tar` & `strangeworks_hybrid_optimize-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       61 2023-06-20 11:44:57.192452 strangeworks_hybrid_optimize-0.1.0/README.md
--rw-r--r--   0        0        0      831 2023-06-20 11:45:11.108618 strangeworks_hybrid_optimize-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-06-20 11:44:57.196452 strangeworks_hybrid_optimize-0.1.0/strangeworks_hybrid_optimize/__init__.py
--rw-r--r--   0        0        0    20458 2023-06-20 11:44:57.196452 strangeworks_hybrid_optimize-0.1.0/strangeworks_hybrid_optimize/sdk.py
--rw-r--r--   0        0        0    12428 2023-06-20 11:44:57.196452 strangeworks_hybrid_optimize-0.1.0/strangeworks_hybrid_optimize/utils.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-16 11:08:20.398575 strangeworks_hybrid_optimize-0.1.1/README.md
+-rw-r--r--   0        0        0      831 2023-07-16 11:08:33.614679 strangeworks_hybrid_optimize-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/__init__.py
+-rw-r--r--   0        0        0    23978 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/sdk.py
+-rw-r--r--   0        0        0    12428 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/utils.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.1/PKG-INFO
```

### Comparing `strangeworks_hybrid_optimize-0.1.0/pyproject.toml` & `strangeworks_hybrid_optimize-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-hybrid-optimize"
-version = "0.1.0"
+version = "0.1.1"
 description = "Extension to strangeworks sdk to allow user to run the hybrid optimization service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_hybrid_optimize"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_hybrid_optimize-0.1.0/strangeworks_hybrid_optimize/sdk.py` & `strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,95 @@
 import json
-from typing import Optional
+from typing import List, Optional
 
 import dimod
 import networkx as nx
 import numpy as np
 import qiskit
 import strangeworks
+from dimod import BinaryQuadraticModel
 from strangeworks.core.errors.error import StrangeworksError
 
 import strangeworks_hybrid_optimize.utils as utils
 
 
+class OptimizationParams:
+    def __init__(
+        self,
+        solver: dict,
+        bqm: Optional[BinaryQuadraticModel] | None = None,
+        var_type: Optional[str] = "BINARY",
+        lagrange_multiplier: Optional[float] = 0.0,
+    ) -> None:
+        self.bqm = json.dumps(bqm.to_serializable()) if bqm else None
+        self.var_type = var_type
+        self.lagrange_multiplier = lagrange_multiplier
+        self.solver = solver
+
+
+class QAOAParams:
+    def __init__(
+        self,
+        maxiter: int,
+        shotsin: int,
+        theta0: Optional[List[float]] | None = None,
+        p: Optional[int] | None = None,
+        alpha: Optional[float] | None = None,
+        optimizer: Optional[str] | None = None,
+        ansatz: Optional[str] | None = None,
+        ising: Optional[bool] | None = None,
+        warm_start: Optional[bool] | None = None,
+        problem_type: Optional[str] = "Classical",
+        optimization_level: Optional[int] = 1,
+        resilience_level: Optional[int] = 1,
+    ) -> None:
+        self.maxiter = maxiter
+        self.shotsin = shotsin
+        self.theta0 = theta0
+        self.p = p
+        self.alpha = alpha
+        self.optimizer = optimizer
+        self.ansatz = ansatz
+        self.ising = ising
+        self.warm_start = warm_start
+        self.problem_type = problem_type
+        self.optimization_level = optimization_level
+        self.resilience_level = resilience_level
+
+
+class HybridParams:
+    def __init__(
+        self,
+        Nf: int,
+        Ns: int,
+        Ng: int,
+        problem_size: int,
+        maxiter: int,
+        shotsin: int,
+        type_subsystem: Optional[str] | None = None,
+        theta0: Optional[List[float]] | None = None,
+        optimizer: Optional[str] | None = None,
+        ansatz: Optional[str] | None = None,
+        optimization_level: Optional[int] = 1,
+        resilience_level: Optional[int] = 1,
+    ) -> None:
+        self.Nf = Nf
+        self.Ns = Ns
+        self.Ng = Ng
+        self.problem_size = problem_size
+        self.type_subsystem = type_subsystem
+        self.maxiter = maxiter
+        self.shotsin = shotsin
+        self.theta0 = theta0
+        self.optimizer = optimizer
+        self.ansatz = ansatz
+        self.optimization_level = optimization_level
+        self.resilience_level = resilience_level
+
+
 class StrangeworksHybrid:
     """Strangeworks client object."""
 
     def __init__(self, resource_slug: Optional[str] = " ") -> None:
         self.product_slug = "77a5lhukf"
 
         try:
@@ -132,15 +207,15 @@
         return self.backend_list
 
     def run(
         self,
         backend,
         problem,
         hybrid_params,
-        problem_params,
+        problem_params: QAOAParams | OptimizationParams,
         backend_sub: Optional[str] = None,
     ):
         """
         Method to submit QAOA problem to backend.
 
         Parameters:
             backend (str): Backend name for the final QAOA optimization step. Must be a
@@ -227,71 +302,76 @@
         """
 
         if self.backend_list == " ":
             self.backends()
 
         aws = False
         ibm = False
+        aws_sub = False
+        ibm_sub = False
+        if backend_sub is None:
+            backend_sub = backend
         backend_sub_id = backend_sub  # For the optimzers
+        channel_sub = None
         for nn in range(len(self.backend_list["AWS"])):
             if (
                 self.backend_list["AWS"][nn]["name"] == backend
                 or self.backend_list["AWS"][nn]["arn"] == backend
             ):
                 aws = True
                 backend_id = self.backend_list["AWS"][nn]["arn"]
             if (
                 self.backend_list["AWS"][nn]["name"] == backend_sub
                 or self.backend_list["AWS"][nn]["arn"] == backend_sub
             ):
-                aws = True
+                aws_sub = True
                 backend_sub_id = self.backend_list["AWS"][nn]["arn"]
 
         for nn in range(len(self.backend_list["IBMQ"])):
             if self.backend_list["IBMQ"][nn]["backend_name"] == backend:
                 ibm = True
                 channel = "ibm_quantum"
                 backend_id = self.backend_list["IBMQ"][nn]["backend_name"]
             if self.backend_list["IBMQ"][nn]["backend_name"] == backend_sub:
-                ibm = True
-                channel = "ibm_quantum"
+                ibm_sub = True
+                channel_sub = "ibm_quantum"
                 backend_sub_id = self.backend_list["IBMQ"][nn]["backend_name"]
 
         for nn in range(len(self.backend_list["IBM_Cloud"])):
             if self.backend_list["IBM_Cloud"][nn]["backend_name"] == backend:
                 ibm = True
                 channel = "ibm_cloud"
                 backend_id = self.backend_list["IBM_Cloud"][nn]["backend_name"]
             if self.backend_list["IBM_Cloud"][nn]["backend_name"] == backend_sub:
-                ibm = True
-                channel = "ibm_cloud"
+                ibm_sub = True
+                channel_sub = "ibm_cloud"
                 backend_sub_id = self.backend_list["IBM_Cloud"][nn]["backend_name"]
 
         for nn in range(len(self.backend_list["AWS_Sim"])):
             if (
                 self.backend_list["AWS_Sim"][nn]["name"] == backend
                 or self.backend_list["AWS_Sim"][nn]["arn"] == backend
             ):
                 aws = True
                 backend_id = self.backend_list["AWS_Sim"][nn]["arn"]
             if (
                 self.backend_list["AWS_Sim"][nn]["name"] == backend_sub
                 or self.backend_list["AWS_Sim"][nn]["arn"] == backend_sub
             ):
-                aws = True
+                aws_sub = True
                 backend_sub_id = self.backend_list["AWS_Sim"][nn]["arn"]
 
         for nn in range(len(self.backend_list["IBM_Sim"])):
             if self.backend_list["IBM_Sim"][nn]["backend_name"] == backend:
                 ibm = True
                 channel = "ibm_quantum"
                 backend_id = self.backend_list["IBM_Sim"][nn]["backend_name"]
             if self.backend_list["IBM_Sim"][nn]["backend_name"] == backend_sub:
-                ibm = True
-                channel = "ibm_quantum"
+                ibm_sub = True
+                channel_sub = "ibm_quantum"
                 backend_sub_id = self.backend_list["IBM_Sim"][nn]["backend_name"]
 
         if ibm is False and aws is False:
             raise StrangeworksError("Unable to Find Backend")
 
         # Check which format the problem is specified in and convert to the form which
         # our QUBO solver can accept.
@@ -310,53 +390,78 @@
             QUBO = problem["BQM"].to_numpy_matrix(
                 variable_order=problem.get("variable_order")
             )
             H = utils.get_Ham_from_QUBO(QUBO)
         else:
             raise StrangeworksError("Problem not in currently supported format")
 
+        hybrid_params = hybrid_params.__dict__
+        problem_params = problem_params.__dict__
+
         for _, y in H:
             if type(y) is tuple:
                 for n in y:
                     if n > (hybrid_params["problem_size"] - 1):
                         raise StrangeworksError(
                             "Specified qubit number is smaller than problem"
                         )
             else:
                 if y > (hybrid_params["problem_size"] - 1):
                     raise StrangeworksError(
                         "Specified qubit number is smaller than problem"
                     )
 
+        if type(problem_params) == OptimizationParams and (
+            ibm_sub is True or aws_sub is True
+        ):
+            raise StrangeworksError("Input params do not match sub-problem backend")
+        if type(problem_params) == QAOAParams and not (
+            ibm_sub is True or aws_sub is True
+        ):
+            raise StrangeworksError("Input params do not match sub-problem backend")
+
         hybrid_params["H"] = json.dumps(H)
         problem_params["ising"] = (
             json.dumps(problem_params["ising"])
             if problem_params.get("ising")
             else json.dumps(False)
         )
         problem_params["warm_start"] = (
             json.dumps(problem_params["warm_start"])
             if problem_params.get("warm_start")
             else json.dumps(False)
         )
 
+        if aws_sub is True:
+            provider_sub = "aws"
+        elif ibm_sub is True:
+            provider_sub = "ibm"
+        else:
+            provider_sub = None
+
         if aws is True:
+            # Final optimization is on aws backend
             input_params = {
                 "provider": "aws",
+                "provider_sub": provider_sub,
+                "channel_sub": channel_sub,
                 "backend": backend_id,
                 "backend_sub": backend_sub_id,
                 "hyperparams": json.dumps(problem_params),
                 "hybrid_params": json.dumps(hybrid_params),
                 "resource_slug": self.sub_rsc.slug,
                 "product_slug": self.sub_rsc.product.slug,
             }
         elif ibm is True:
+            # Final optimization is on ibm backend
             input_params = {
                 "provider": "ibm",
+                "provider_sub": provider_sub,
                 "channel": channel,
+                "channel_sub": channel_sub,
                 "backend": backend_id,
                 "backend_sub": backend_sub_id,
                 "hyperparams": json.dumps(problem_params),
                 "hybrid_params": json.dumps(hybrid_params),
                 "resource_slug": self.sub_rsc.slug,
                 "product_slug": self.sub_rsc.product.slug,
             }
```

### Comparing `strangeworks_hybrid_optimize-0.1.0/strangeworks_hybrid_optimize/utils.py` & `strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_hybrid_optimize-0.1.0/PKG-INFO` & `strangeworks_hybrid_optimize-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-hybrid-optimize
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension to strangeworks sdk to allow user to run the hybrid optimization service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

