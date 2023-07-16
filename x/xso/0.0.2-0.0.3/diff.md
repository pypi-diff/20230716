# Comparing `tmp/xso-0.0.2.tar.gz` & `tmp/xso-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xso-0.0.2.tar", max compression
+gzip compressed data, was "xso-0.0.3.tar", max compression
```

## Comparing `xso-0.0.2.tar` & `xso-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1514 2023-03-03 22:41:01.663778 xso-0.0.2/LICENSE
--rw-r--r--   0        0        0     3048 2023-03-03 22:41:01.663882 xso-0.0.2/README.md
--rw-r--r--   0        0        0      673 2023-07-11 13:40:05.620809 xso-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-09 14:16:37.934652 xso-0.0.2/src/xso/__init__.py
--rw-r--r--   0        0        0     7702 2023-07-10 19:15:07.487130 xso-0.0.2/src/xso/backendcomps.py
--rw-r--r--   0        0        0    23120 2023-07-09 19:41:12.784520 xso-0.0.2/src/xso/component.py
--rw-r--r--   0        0        0     5132 2023-03-03 22:41:01.666823 xso-0.0.2/src/xso/core.py
--rw-r--r--   0        0        0     7344 2023-07-10 21:29:49.567155 xso-0.0.2/src/xso/model.py
--rw-r--r--   0        0        0    16340 2023-07-10 21:55:30.098011 xso-0.0.2/src/xso/solvers.py
--rw-r--r--   0        0        0     9027 2023-07-09 14:26:51.963518 xso-0.0.2/src/xso/variables.py
--rw-r--r--   0        0        0     6227 2023-07-09 21:12:25.451042 xso-0.0.2/src/xso/xsimlabwrappers.py
--rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 xso-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1514 2023-03-03 22:41:01.663778 xso-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3290 2023-07-13 13:11:23.771983 xso-0.0.3/README.md
+-rw-r--r--   0        0        0      693 2023-07-16 15:33:37.590527 xso-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-09 14:16:37.934652 xso-0.0.3/src/xso/__init__.py
+-rw-r--r--   0        0        0     7702 2023-07-12 21:12:02.882760 xso-0.0.3/src/xso/backendcomps.py
+-rw-r--r--   0        0        0    23120 2023-07-09 19:41:12.784520 xso-0.0.3/src/xso/component.py
+-rw-r--r--   0        0        0     5297 2023-07-12 21:20:47.997816 xso-0.0.3/src/xso/core.py
+-rw-r--r--   0        0        0     7215 2023-07-12 20:43:16.541879 xso-0.0.3/src/xso/model.py
+-rw-r--r--   0        0        0    14371 2023-07-12 20:41:43.354334 xso-0.0.3/src/xso/solvers.py
+-rw-r--r--   0        0        0     9027 2023-07-09 14:26:51.963518 xso-0.0.3/src/xso/variables.py
+-rw-r--r--   0        0        0     6757 2023-07-12 21:12:02.875376 xso-0.0.3/src/xso/xsimlabwrappers.py
+-rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 xso-0.0.3/PKG-INFO
```

### Comparing `xso-0.0.2/LICENSE` & `xso-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xso-0.0.2/README.md` & `xso-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # xarray-simlab-ode
 
+[![Documentation Status](https://readthedocs.org/projects/xarray-simlab-ode/badge/?version=latest)](https://xarray-simlab-ode.readthedocs.io/en/latest/?badge=latest)
+
 The `xso` framework for building and solving models based on ordinary differential equations (ODEs), an extension of [xarray-simlab](https://github.com/xarray-contrib/xarray-simlab).
 
 Xarray-simlab provides a generic framework for building computational models in a modular fashion and an [xarray](http://xarray.pydata.org/) extension for setting and running simulations using xarray's `Dataset` structure.
 
 Xarray-simlab-ode (XSO) extends the framework with a set of variables, processes and a solver backend, suited towards ODE-based models. It is designed for flexible, interactive and reproducible modeling workflows.
 
 ## Installation
@@ -16,39 +18,40 @@
 A highly simplified model based on ordinary differential equations is shown below.
 1. Create new model components by writing compact Python classes:
 ```python
 import xso
 
 @xso.component
 class Variable:
-    var = xso.variable(description='basic state variable')
+    var = xso.variable(description='basic state variable', attrs={'units':'µM'})
 
 @xso.component
 class LinearGrowth:
     var_ext = xso.variable(foreign=True, flux='growth', description='external state variable')
-    rate = xso.parameter(description='linear growth rate')
+    rate = xso.parameter(description='linear growth rate', attrs={'units':'$d^{-1}$'})
+
     @xso.flux
     def growth(self, var_ext, rate):
         return var_ext * rate
 ```
 2. Create a new model just by providing a dictionary of model components:
 
 ```python
-model = xso.create({'Var':Variable,'Growth':LinearGrowth})
+model = xso.create({'Var':Variable,'Growth':LinearGrowth}, time_unit='d')
 ```
 3. Create an input xarray.Dataset, run the model and get an output xarray.Dataset:
 
 ```python
 import numpy as np
 
-input_ds = xso.setup(solver='stepwise',
+input_ds = xso.setup(solver='solve_ivp',
                      model=model,
-                     time=np.arange(1,10),
+                     time=np.arange(1,10,.1),
                      input_vars={
-                         'Var':{'var_label':'X', 'var_init':1},
+                         'Var':{'value_label':'X', 'value_init':1},
                          'Growth':{'var_ext':'X', 'rate':1.},
                      })
 
 with model:
     output_ds = input_ds.xsimlab.run()
 ```
 4.Perform model setup, pre-processing, run, post-processing and visualization in a functional style, using method chaining:
```

### Comparing `xso-0.0.2/pyproject.toml` & `xso-0.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "xso"
-version = "0.0.2"
+version = "0.0.3"
 description = "Framework for building and solving ODE-based models, an extension of xarray-simlab"
 authors = ["Benjamin Post"]
 license = "BSD 3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.5"
 xarray-simlab = "^0.5.0"
-scipy = "^1.9.1"
-dask = {extras = ["distributed"], version = "^2022.10.0"}
-jupyter = "^1.0.0"
-numpy = "^1.25.1"
+scipy = ">=1.9.1"
+dask = {extras = ["distributed"], version = ">=2022.10.0"}
+zarr = ">= 2.3.0"
+xarray = ">=0.10.0"
+numpy = "*"
+tqdm = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 myst-nb = {version = "^0.16.0", python = "^3.9"}
 sphinx-autoapi = "^2.0.0"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `xso-0.0.2/src/xso/backendcomps.py` & `xso-0.0.3/src/xso/backendcomps.py`

 * *Files identical despite different names*

### Comparing `xso-0.0.2/src/xso/component.py` & `xso-0.0.3/src/xso/component.py`

 * *Files identical despite different names*

### Comparing `xso-0.0.2/src/xso/core.py` & `xso-0.0.3/src/xso/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time as tm
 
 from xso.model import Model
-from xso.solvers import SolverABC, ODEINTSolver, StepwiseSolver
+from xso.solvers import SolverABC, IVPSolver, StepwiseSolver
 
-_built_in_solvers = {'odeint': ODEINTSolver, 'stepwise': StepwiseSolver}
+_built_in_solvers = {'solve_ivp': IVPSolver, 'stepwise': StepwiseSolver}
 
 
 class XSOCore:
     """Backend core class that initializes solver and model, and
     translates between the two for model construction and solving.
 
     This core class is necessary to allow an abstract model based on differential equations
@@ -21,23 +21,26 @@
 
     def __init__(self, solver):
         """
         Initializes XSO Model and XSO Solver, and stores solve start and end for diagnostics.
 
         Parameters
         ----------
-        solver : {'stepwise', 'odeint'} or subclass of SolverABC
+        solver : {'stepwise', 'solve_ivp'} or subclass of SolverABC
            Solver name as str, has to be built into xso.
            Alternatively can be passed a custom subclass of xso.solver.SolverABC.
         """
         self.solve_start = None
         self.solve_end = None
 
         if isinstance(solver, str):
-            self.solver = _built_in_solvers[solver]()
+            try:
+                self.solver = _built_in_solvers[solver]()
+            except KeyError:
+                raise KeyError("Solver name passed is not built-in. Please choose from: 'stepwise', 'solve_ivp'.")
         elif isinstance(solver, SolverABC):
             self.solver = solver
         else:
             raise Exception("Solver argument passed to model is not built-in or subclass of SolverABC.")
 
         self.model = Model()
```

### Comparing `xso-0.0.2/src/xso/model.py` & `xso-0.0.3/src/xso/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from collections import defaultdict
 
 import numpy as np
 
-from xso.solvers import ODEINTSolver, StepwiseSolver
-
-_built_in_solvers = {'odeint': ODEINTSolver, 'stepwise': StepwiseSolver}
-
 
 def return_dim_ndarray(value):
     """Helper function to always have at least 1d numpy array returned."""
     if isinstance(value, list):
         return np.array(value)
     elif isinstance(value, np.ndarray):
         return value
@@ -71,15 +67,15 @@
                 index += dims
             else:
                 _length = np.prod(dims)
                 state_dict[key] = flat_state[index:index + _length].reshape(dims)
                 index += _length
         return state_dict
 
-    def model_function(self, time=None, current_state=None,  forcing=None):
+    def model_function(self, time=None, current_state=None, forcing=None):
         """ General model function that computes forcings and fluxes.
         Is called within solve function of Solver.
 
         Parameters
         __________
         current_state : numpy array
            Large array containing all current values for model.
```

### Comparing `xso-0.0.2/src/xso/solvers.py` & `xso-0.0.3/src/xso/solvers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 
 import numpy as np
 import math
 
-from scipy.integrate import odeint, solve_ivp
+from scipy.integrate import solve_ivp
 
 
 def to_ndarray(value):
     """Helper function to always have at least 1d numpy array returned."""
     if isinstance(value, list):
         return np.array(value)
     elif isinstance(value, np.ndarray):
@@ -107,19 +107,21 @@
             return np.abs(x)
 
         def sin(x):
             """ Sine function """
             return np.sin(x)
 
 
-class ODEINTSolver(SolverABC):
-    """Solver that can handle ODEINT solving of Model.
+class IVPSolver(SolverABC):
+    """Solver backend using scipy.integrate.solve_ivp to solve model.
 
-    ODEINT is an adaptive step-size solver for ordinary differential equations,
+    SOLVE_IVP is a variable step-size solver for ordinary differential equations,
     included in the SciPy Python package.
+
+    By default, it utilizes an explicit Runge-Kutta method of order 5(4).
     """
 
     def __init__(self):
         self.var_init = defaultdict()
         self.flux_init = defaultdict()
 
     @staticmethod
@@ -200,84 +202,32 @@
             model.full_model_dims[flx_key] = dim
 
         # TODO: diagnostic print here
         # print model repr for diagnostic purposes:
         # print("Model is assembled!")
         # print(model)
 
-    def xxxsolvexxx(self, model, time_step):
-        """Solve model using ODEINT, passing model_function, initial values and model.time.
-        The model output is then assigned to the previously initialized storage arrays within xsimlab backend.
-        """
-
-        full_init = np.concatenate([[v for val in self.var_init.values() for v in val.ravel()],
-                                    [v for val in self.flux_init.values() for v in val.ravel()]], axis=None)
-
-        # solving model here:
-        full_model_out = odeint(model.model_function, full_init, model.time)  # , mxstep=5000, rtol=1e-10, atol=1e-10)
-
-        state_rows = [row for row in full_model_out.T]
-
-        state_dict = defaultdict()
-        index = 0
-        for key, dims in model.full_model_dims.items():
-            if dims is None:
-                state_dict[key] = state_rows[index]
-                index += 1
-            elif isinstance(dims, int):
-                val_list = []
-                for i in range(dims):
-                    val_list.append(state_rows[index])
-                    index += 1
-                state_dict[key] = np.array(val_list)
-            else:
-                full_dims = (*dims, np.size(model.time))
-                _length = int(np.prod(dims))
-                val_list = []
-                for i in range(_length):
-                    val_list.append(state_rows[index])
-                    index += 1
-
-                state_dict[key] = np.array(val_list).reshape(full_dims)
-
-        # assign solved model state to value storage in xsimlab framework:
-        for var_key, val in model.variables.items():
-            val[...] = state_dict[var_key]
-
-        for flux_key, val in model.flux_values.items():
-            state = state_dict[flux_key]
-            dims = model.full_model_dims[flux_key]
-
-            difference = np.diff(state) / time_step
-
-            if dims:
-                if isinstance(dims, tuple):
-                    val[...] = np.concatenate((difference[..., 0][..., np.newaxis], difference), axis=len(dims))
-                else:
-                    val[...] = np.hstack((difference[..., 0][:, None], difference))
-            else:
-                val[...] = np.hstack((difference[0], difference))
-
     def solve(self, model, time_step):
-        """Solve model using ODEINT, passing model_function, initial values and model.time.
+        """Solve model using scipy.integrate.solve_ivp, passing model_function, initial values and model.time.
         The model output is then assigned to the previously initialized storage arrays within xsimlab backend.
         """
-
+        # convert all initial values to a 1D array:
         full_init = np.concatenate([[v for val in self.var_init.values() for v in val.ravel()],
                                     [v for val in self.flux_init.values() for v in val.ravel()]], axis=None)
 
         # solving model here:
         full_model_out = solve_ivp(model.model_function,
-                                   t_span=[model.time[0],model.time[-1]],
+                                   t_span=[model.time[0], model.time[-1]],
                                    y0=full_init,
                                    t_eval=model.time)
 
-        # rounding to remove floating point errors
-        state_rows = [row for row in np.around(full_model_out.y, decimals=100)]
+        # round off 1e150-th decimal to remove floating point numerical errors
+        state_rows = [row for row in np.around(full_model_out.y, decimals=150)]
 
+        # unpack and reshape state array to appropriate dimensions:
         state_dict = defaultdict()
         index = 0
         for key, dims in model.full_model_dims.items():
             if dims is None:
                 state_dict[key] = state_rows[index]
                 index += 1
             elif isinstance(dims, int):
@@ -439,15 +389,15 @@
                 model_state.append(val[..., self.time_index - 1])
             else:
                 model_state.append(val[self.time_index - 1])
 
         # flatten list for model function:
         flat_model_state = np.concatenate(model_state, axis=None)
 
-        state_out = model.model_function(flat_model_state, forcing=model_forcing)
+        state_out = model.model_function(current_state=flat_model_state, forcing=model_forcing)
 
         # unpack flat state:
         state_dict = model.unpack_flat_state(state_out)
 
         for key, val in model.variables.items():
             if model.full_model_dims[key]:
                 val[..., self.time_index] = val[..., self.time_index - 1] + state_dict[key] * time_step
```

### Comparing `xso-0.0.2/src/xso/variables.py` & `xso-0.0.3/src/xso/variables.py`

 * *Files identical despite different names*

### Comparing `xso-0.0.2/src/xso/xsimlabwrappers.py` & `xso-0.0.3/src/xso/xsimlabwrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,21 +11,25 @@
     automatically adding the necessary model backend, solver and time components.
 
     Parameters
     ----------
     components : dict
         Dictionary with component names as keys and classes (decorated with
         :func:`component`) as values.
+    time_unit : str, optional
+        Unit of time to be used in the model. Default is 'd' for days. This has to be
+        supplied at model creation, since the time unit is written to the immutable
+        metadata of the model object.
     """
 
     components.update({'Core': Backend, 'Solver': RunSolver, 'Time': create_time_component(time_unit)})
     return xs.Model(components)
 
 
-def setup(solver, model, input_vars, output_vars=None, time=None):
+def setup(solver, model, input_vars, output_vars=None, time=None, solver_kwargs=None):
     """Create a specific setup for model runs.
 
     This function wraps xsimlab's create_setup and adds a dummy clock parameter
     necessary for model execution. This convenient function creates a new
     :class:`xarray.Dataset` object with everything needed to run a model
     (i.e., input values, time steps, output variables to save at given times)
     as data variables, coordinates and attributes.
@@ -54,14 +58,18 @@
         Dictionary with model variable names to save as simulation output.
         Entries of the dictionary look similar than for ``input_vars``
         (see here above), except that here ``value`` must correspond
         to the dimension of a clock coordinate (i.e., new output values will
         be saved at each time given by the coordinate labels) or
         ``None`` (i.e., only one value will be saved at the end
         of the simulation).
+    solver_kwargs : dict, optional
+        Additional keyword arguments to pass to the solver backend. This is
+        directly passed to the solving function and can be used to adjust parameters
+        for solver backends that allow this, such as the IVPSolver backend.
 
     Returns
     -------
     dataset : :class:`xarray.Dataset`
         A new Dataset object with model inputs as data variables or coordinates
         (depending on their given value) and clock coordinates.
         The names of the input variables also include the name of their process
```

### Comparing `xso-0.0.2/PKG-INFO` & `xso-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: xso
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for building and solving ODE-based models, an extension of xarray-simlab
 License: BSD 3-Clause
 Author: Benjamin Post
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.5
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dask[distributed] (>=2022.10.0,<2023.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: scipy (>=1.9.1,<2.0.0)
+Requires-Dist: dask[distributed] (>=2022.10.0)
+Requires-Dist: numpy
+Requires-Dist: scipy (>=1.9.1)
+Requires-Dist: tqdm
+Requires-Dist: xarray (>=0.10.0)
 Requires-Dist: xarray-simlab (>=0.5.0,<0.6.0)
+Requires-Dist: zarr (>=2.3.0)
 Description-Content-Type: text/markdown
 
 # xarray-simlab-ode
 
+[![Documentation Status](https://readthedocs.org/projects/xarray-simlab-ode/badge/?version=latest)](https://xarray-simlab-ode.readthedocs.io/en/latest/?badge=latest)
+
 The `xso` framework for building and solving models based on ordinary differential equations (ODEs), an extension of [xarray-simlab](https://github.com/xarray-contrib/xarray-simlab).
 
 Xarray-simlab provides a generic framework for building computational models in a modular fashion and an [xarray](http://xarray.pydata.org/) extension for setting and running simulations using xarray's `Dataset` structure.
 
 Xarray-simlab-ode (XSO) extends the framework with a set of variables, processes and a solver backend, suited towards ODE-based models. It is designed for flexible, interactive and reproducible modeling workflows.
 
 ## Installation
@@ -35,39 +43,40 @@
 A highly simplified model based on ordinary differential equations is shown below.
 1. Create new model components by writing compact Python classes:
 ```python
 import xso
 
 @xso.component
 class Variable:
-    var = xso.variable(description='basic state variable')
+    var = xso.variable(description='basic state variable', attrs={'units':'µM'})
 
 @xso.component
 class LinearGrowth:
     var_ext = xso.variable(foreign=True, flux='growth', description='external state variable')
-    rate = xso.parameter(description='linear growth rate')
+    rate = xso.parameter(description='linear growth rate', attrs={'units':'$d^{-1}$'})
+
     @xso.flux
     def growth(self, var_ext, rate):
         return var_ext * rate
 ```
 2. Create a new model just by providing a dictionary of model components:
 
 ```python
-model = xso.create({'Var':Variable,'Growth':LinearGrowth})
+model = xso.create({'Var':Variable,'Growth':LinearGrowth}, time_unit='d')
 ```
 3. Create an input xarray.Dataset, run the model and get an output xarray.Dataset:
 
 ```python
 import numpy as np
 
-input_ds = xso.setup(solver='stepwise',
+input_ds = xso.setup(solver='solve_ivp',
                      model=model,
-                     time=np.arange(1,10),
+                     time=np.arange(1,10,.1),
                      input_vars={
-                         'Var':{'var_label':'X', 'var_init':1},
+                         'Var':{'value_label':'X', 'value_init':1},
                          'Growth':{'var_ext':'X', 'rate':1.},
                      })
 
 with model:
     output_ds = input_ds.xsimlab.run()
 ```
 4.Perform model setup, pre-processing, run, post-processing and visualization in a functional style, using method chaining:
```

