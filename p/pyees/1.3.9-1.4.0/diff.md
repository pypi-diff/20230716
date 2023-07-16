# Comparing `tmp/pyees-1.3.9.tar.gz` & `tmp/pyees-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.9.tar", last modified: Fri Jul 14 10:43:20 2023, max compression
+gzip compressed data, was "pyees-1.4.0.tar", last modified: Sun Jul 16 07:04:10 2023, max compression
```

## Comparing `pyees-1.3.9.tar` & `pyees-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.067441 pyees-1.3.9/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-14 10:43:20.596026 pyees-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.463382 pyees-1.3.9/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.9/pyees/__init__.py
--rw-rw-rw-   0        0        0    14848 2023-07-14 10:40:42.000000 pyees-1.3.9/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.3.9/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.9/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.9/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.9/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.9/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.9/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-07-14 10:43:20.288849 pyees-1.3.9/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.9/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.9/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.9/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.9/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.9/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.9/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.9/pyees/unit.py
--rw-rw-rw-   0        0        0    34114 2023-07-14 10:43:20.478343 pyees-1.3.9/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.576083 pyees-1.3.9/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-14 10:43:20.623952 pyees-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-14 10:43:18.000000 pyees-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:04:09.433721 pyees-1.4.0/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-16 07:04:10.172283 pyees-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 07:04:09.983787 pyees-1.4.0/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.0/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.0/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.0/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.0/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.0/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.0/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.0/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.0/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-16 06:54:08.000000 pyees-1.4.0/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.0/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.4.0/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.0/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.0/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-16 07:04:09.908988 pyees-1.4.0/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.4.0/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.0/pyees/unit.py
+-rw-rw-rw-   0        0        0    34114 2023-07-16 07:04:10.000740 pyees-1.4.0/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:04:10.142365 pyees-1.4.0/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-16 07:04:09.000000 pyees-1.4.0/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-16 07:04:08.000000 pyees-1.4.0/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 07:04:10.156326 pyees-1.4.0/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-16 07:04:10.202201 pyees-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-16 07:04:00.000000 pyees-1.4.0/setup.py
```

### Comparing `pyees-1.3.9/LICENSE.txt` & `pyees-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/PKG-INFO` & `pyees-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.9
+Version: 1.4.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.9/README.md` & `pyees-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/fit.py` & `pyees-1.4.0/pyees/fit.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,28 +10,40 @@
     from pyees.variable import variable, arrayVariable, scalarVariable
     from pyees.unit import unit
 
 
 
     
 class _fit():
-    def __init__(self, func, x, y, p0) -> None:
+    def __init__(self, func, x, y, p0 = None, useParameters = None) -> None:
+
+        if p0 is None:
+            p0 = [0] * self._nParameters
+        if len(p0) != self._nParameters:
+            raise ValueError(f'The input "p0" has to be None or have a length of {self._nParameters}')
+
+        if useParameters is None:
+            useParameters = [True] * self._nParameters   
+        if len(useParameters) != self._nParameters:
+            raise ValueError(f'The input "useParameters" has to have a length of {self._nParameters}')
+        
         self.func = func
+        self.p0 = p0
+        self.useParameters = useParameters
 
         if not (isinstance(x, arrayVariable) and isinstance(y, arrayVariable)):
             raise ValueError('The inputs has to be variables')
 
         self.xVal = x.value
         self.yVal = y.value
         self.xUnit = x._unitObject
         self.yUnit = y._unitObject
         self.xUncert = x.uncert
         self.yUncert = y.uncert
 
-
         indexesNotToUse = []
         for i in range(len(self.xVal)):
             if np.isnan(self.xVal[i]):
                 indexesNotToUse.append(i)
                 continue
             if np.isnan(self.xUncert[i]):
                 indexesNotToUse.append(i)
@@ -48,34 +60,28 @@
             indexesToUse = [i for i in range(len(self.xVal)) if not i in indexesNotToUse]
             self.xVal = self.xVal[indexesToUse]
             self.xUncert = self.xUncert[indexesToUse]
             self.yVal = self.yVal[indexesToUse]
             self.yUncert = self.yUncert[indexesToUse]
 
         # uncertanties can not be 0
-        if len(self.xVal) == 1:
-            self._sx = self.xUncert if self.xUncert != 0 else 1e-10
-        else:
-            self._sx = [elem if elem != 0 else 1e-10 for elem in self.xUncert]
-        if len(self.yVal) == 1:
-            self._sy = self.yUncert if self.yUncert != 0 else 1e-10
-        else:
-            self._sy = [elem if elem != 0 else 1e-10 for elem in self.yUncert]
+        self._sx = [elem if elem != 0 else 1e-10 for elem in self.xUncert]
+        self._sy = [elem if elem != 0 else 1e-10 for elem in self.yUncert]
 
         # create the regression
         np.seterr('ignore')
         data = odr.RealData(self.xVal, self.yVal, sx=self._sx, sy=self._sy)
-        regression = odr.ODR(data, odr.Model(self._func), beta0=p0)
+        regression = odr.ODR(data, odr.Model(self._func), beta0=self.p0)
         regression = regression.run()
         popt = regression.beta
         popt = [0.9 * elem for elem in popt]
         regression = odr.ODR(data, odr.Model(self._func), beta0=popt)
         regression = regression.run()
+        # regression = regression.restart()        
         
-
         ## create a list of coefficients
         self.coefficients = []
         units = self.getVariableUnits()
         for i in range(len(regression.beta)):
             var = variable(regression.beta[i], units[i], np.sqrt(regression.cov_beta[i,i]))
             self.coefficients.append(var)
         
@@ -94,21 +100,24 @@
         self._residuals = np.array([yi - pi for yi, pi in zip(self.yVal, self._predict(regression.beta, self.xVal))])# y.value - self._predict(x.value)
         ss_res = sum(self._residuals**2)
         ss_tot = sum((self.yVal - np.mean(self.yVal))**2)
         if ss_tot != 0:
             self.r_squared = variable(1 - (ss_res / ss_tot))
         else:
             self.r_squared = variable(1)
-        np.seterr('warn')
-
+        
+        
+    def getOnlyUsedTerms(self, B):
+        for i in range(len(B)):
+            if not self.useParameters[i]:
+                B[i] = self.p0[i]
+        return B
+        
     def __str__(self):
-        return self.func_name() + ',  ' + self._r2_name()
-
-    def _r2_name(self):
-        return f'$R^2 = {self.r_squared.value:.5f}$'
+        return self.func_name() + f', $R^2 = {self.r_squared.value:.5f}$'
 
     def scatter(self, ax, label=True, showUncert=True, **kwargs):
 
         if all(self.xUncert == 0) and all(self.yUncert == 0):
             showUncert = False
 
         # parse label
@@ -274,160 +283,217 @@
         
         if r < 0.68:
             warnings.warn(f'{(1-r)*100:.2f}% of the datapoints were more than 1 standard deviation away from the regression. This might indicate that the regression is poor', category=Warning, stacklevel=1)
             
 
 
 class dummy_fit(_fit):
-    def __init__(self, x, y):
+    """Create a dummy fit of the input data. No regression is performed when creating a dummy fit. The dummy fit object is onely used to easily plot the data
+    
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    """
+    def __init__(self, x : variable,  y : variable):
         
         if not (isinstance(x, arrayVariable) and isinstance(y, arrayVariable)):
             raise ValueError('The inputs has to be variables')
 
         self.xVal = x.value
         self.yVal = y.value
         self.xUnit = x.unit
         self.yUnit = y.unit
         self.xUncert = x.uncert
         self.yUncert = y.uncert
 
-        self.r_squared = 0
+        self.r_squared = variable(1)
 
     def _func(self, x):
         return 1
 
     def func_name(self):
-        return f'{self.popt[0]}'
+        return '1'
 
 class exp_fit(_fit):
-    def __init__(self, x, y, p0=[1, 1, 1, 1]):
-        if len(p0) != 4:
-            raise ValueError('You have to provide initial guesses for 4 parameters')
+    """Create an exponential fit of the input data and easily plot the regression.
+    
+    f(x) = a * exp(b * x) + c
+
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    p0 : List(float) = None
+        The initial guesses in order (a,b,c). If p0 is set to None, then all parameters are initialized to 0.
+    useParameters : List(double) = None
+        Wheater or not to use the parameters in order (a,b,c). If an element is set to "False", then the parameter is fixed to the initial guess
+    """
+    
+    def __init__(self, x : variable, y: variable, p0 : list[float] = None, useParameters : list[bool] = [True, True, False]):
+        self._nParameters = 3
         if x.unit != '1':
             raise ValueError('The variable "x" cannot have a unit')
-        _fit.__init__(self, self.func, x, y, p0=p0)
+        _fit.__init__(self, self.func, x, y, p0=p0, useParameters = useParameters)
 
     def getVariableUnits(self):
-        return [self.yUnit, '', '', self.yUnit]
+        return [self.yUnit, '', self.yUnit]
 
     def _func(self, B, x):
-        a,b,c,d = B
-        return a * b**(x-c) + d
+        a,b,c = self.getOnlyUsedTerms(B)
+        return a * np.exp(b * x) + c
 
     def func_name(self):
-        a,b,c,d = self.coefficients
-        return f'$a\cdot b^(x-c)+d,\quad a={a.__str__(pretty = True)}, \quad b={b.__str__(pretty = True)}, \quad c={c.__str__(pretty = True)}, \quad d={d.__str__(pretty = True)}$'
+        a,b,c = self.coefficients
+        return f'$a\cdot b^(b\cdot x)+d,\quad a={a.__str__(pretty = True)}, \quad b={b.__str__(pretty = True)}, \quad c={c.__str__(pretty = True)}$'
 
 
 class pow_fit(_fit):
-    def __init__(self, x, y, p0=[1, 1]):
+    """Create a power fit of the input data and easily plot the regression.
+    
+    f(x) = a * b**x + c
+
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    p0 : List(float) = None
+        The initial guesses in order (a,b,c). If p0 is set to None, then all parameters are initialized to 0.
+    useParameters : List(double) = None
+        Wheater or not to use the parameters in order (a,b,c). If an element is set to "False", then the parameter is fixed to the initial guess
+    """
+    def __init__(self, x : variable, y: variable, p0 : list[float] = None, useParameters : list[bool] = [True,True,False]):
+        self._nParameters = 3
         
-        if len(p0) != 2:
-            raise ValueError('You have to provide initial guesses for 2 parameters')
         if x.unit != '1':
             raise ValueError('The variable "x" cannot have a unit')
-        _fit.__init__(self, self.func, x, y, p0=p0)
+        
+        _fit.__init__(self, self.func, x, y, p0=p0, useParameters=useParameters)
 
     def getVariableUnits(self):
-        return [self.yUnit, '1']
+        return [self.yUnit, '1', self.yUnit]
 
     def _func(self, B, x):
-        a = B[0]
-        b = B[1]
-        return a * x**b
+        a,b,c = self.getOnlyUsedTerms(B)
+        return a * x**b+c
 
     def func_name(self):
-        return f'$a x^b,\quad a={self.coefficients[0].__str__(pretty = True)}, \quad b={self.coefficients[1].__str__(pretty = True)}$'
+        return f'$a x^b+c,\quad a={self.coefficients[0].__str__(pretty = True)}, \quad b={self.coefficients[1].__str__(pretty = True)}, \quad b={self.coefficients[1].__str__(pretty = True)}$'
 
 
-def lin_fit(x, y, terms = None, p0=None):
-    return pol_fit(x, y, deg=1, terms = terms, p0=p0)
+def lin_fit(x : variable, y: variable, p0 : list[float] = None, useParameters : list[bool] = None):
+    """Create a linear fit of the input data and easily plot the regression.
+    
+    f(x) = a*x + b
 
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    p0 : List(float) = None
+        The initial guesses in order (a,b). If p0 is set to None, then all parameters are initialized to 0.
+    useParameters : List(double) = None
+        Wheater or not to use the parameters in order (a,b). If an element is set to "False", then the parameter is fixed to the initial guess
+    """
+    return pol_fit(x, y, deg=1, p0=p0, useParameters=useParameters)
 
-class pol_fit(_fit):
-    def __init__(self, x, y, deg=2, terms=None, p0=None):
-        if terms is None:
-            terms = [True] * (deg + 1)
-        else:
-            for term in terms:
-                if not str(type(term)) == "<class 'bool'>":
-                    raise ValueError('All elements in "terms" has to be booleans')
-            if len(terms) > deg + 1:
-                raise ValueError(f'You have specified to use {len(terms)} terms, but you can only use {deg+1} using a polynomial of degree {deg}')
-        self.terms = terms
 
-        if p0 is None:
-            p0 = [1] * sum(1 for elem in self.terms if elem)
+class pol_fit(_fit):
+    """Create a polynomial fit of the input data and easily plot the regression.
+    
+    f(x) = sum_0^n ( a_i * x**(n-i) )
 
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    p0 : List(float) = None
+        The initial guesses in order (a_n, ..., a_1, a_0). If p0 is set to None, then all parameters are initialized to 0.
+    useParameters : List(double) = None
+        Wheater or not to use the parameters in order (a_n, ..., a_1, a_0). If an element is set to "False", then the parameter is fixed to the initial guess
+    deg: int
+        The degree of the polynomial
+    """
+    def __init__(self, x : variable, y: variable, p0 : list[float] = None, useParameters : list[bool] = None, deg :int = 2):
+        self._nParameters = deg + 1
         self.deg = deg
 
-        _fit.__init__(self, self.func, x, y, p0=p0)
+        _fit.__init__(self, self.func, x, y, p0=p0, useParameters=useParameters)
 
     def getVariableUnits(self):
         units = []
         n = self.deg
-        index = 0
         for i in range(n + 1):
-            if self.terms[i]:
-                u = self.yUnit
-                if i != n:
-                    ui = self.xUnit ** (n - i)
-                    u /= ui
-                units.append(u)
-                index += 1
+            u = self.yUnit
+            if i != n:
+                ui = self.xUnit ** (n - i)
+                u /= ui
+            units.append(u)
         return units
 
     def _func(self, B, x):
+        B = self.getOnlyUsedTerms(B)
         out = 0
-        n = self.deg
-        index = 0
-        for i in range(n + 1):
-            if self.terms[i]:
-                out +=  B[index] * x**(n - i)
-                index += 1
+        for i,b in enumerate(B):
+            out +=  b * x**(self.deg - i)
         return out
 
     def func_name(self):
         out = '$'
         n = self.deg
         for i in range(n + 1):
-            if self.terms[i]:
-                exponent = n - i
-                if i == 0:
-                    out += f'{string.ascii_lowercase[i]}'
-                else:
-                    out += f'+{string.ascii_lowercase[i]}'
-                if exponent != 0:
-                    out += f'x'
-                if exponent > 1:
+            exponent = n - i
+            if i == 0:
+                out += f'{string.ascii_lowercase[i]}'
+            else:
+                out += f'+{string.ascii_lowercase[i]}'
+            if exponent != 0:
+                out += f'x'
+            if exponent > 1:
                     out += f'^{exponent}'
-        index = 0
+       
         for i in range(n + 1):
-            if self.terms[i]:
-                out += f', {string.ascii_lowercase[i]}={self.coefficients[index].__str__(pretty = True)}'
-                index += 1
+            out += f', {string.ascii_lowercase[i]}={self.coefficients[i].__str__(pretty = True)}'
         out += '$'
         return out
 
 
 class logistic_fit(_fit):
-    def __init__(self, x, y, p0=[1, 1, 1]):
-        if len(p0) != 3:
-            raise ValueError('You have to provide initial guesses for 3 parameters')
+    """Create a logistic fit of the input data and easily plot the regression.
+    
+    f(x) = L / (1 + exp(-k * (x - x0)))
+
+    Parameters:
+    x : variable
+        The independent variable
+    y : variable
+        The dependents variable
+    p0 : List(float) = None
+        The initial guesses in order (L,k,x0). If p0 is set to None, then all parameters are initialized to 0.
+    useParameters : List(double) = None
+        Wheater or not to use the parameters in order (L,k,x0). If an element is set to "False", then the parameter is fixed to the initial guess
+    """
+    def __init__(self, x : variable, y: variable, p0 : list[float] = None, useParameters : list[bool] = None):
+
+        self._nParameters = 3
+
         if x.unit != '1':
             raise ValueError('The variable "x" cannot have a unit')
-        _fit.__init__(self, self.func, x, y, p0=p0)
+        _fit.__init__(self, self.func, x, y, p0=p0, useParameters=useParameters)
 
     def getVariableUnits(self):
         return [self.yUnit,'1','1']
     
     def _func(self, B, x):
-        L = B[0]
-        k = B[1]
-        x0 = B[2]
+        L,k,x0 = self.getOnlyUsedTerms(B)
         return L / (1 + np.exp(-k * (x - x0)))
 
     def func_name(self):
         L = self.coefficients[0].__str__(pretty=True)
         k = self.coefficients[1].__str__(pretty=True)
         x0 = self.coefficients[2].__str__(pretty=True)
 
@@ -437,8 +503,21 @@
         out += f'\quad x_0={x0}$'
         return out
 
 
 
 ## TODO fit - få det til at virke som i bogen - brug tests - mangler solutions
 
-## TODO fit - lås parametre
+
+
+if __name__ == "__main__":
+    import matplotlib.pyplot as plt
+    x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100])
+    y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
+    f = exp_fit(x,y)
+    print(f)
+    fig, ax = plt.subplots()
+    f.scatter(ax)
+    f.plot(ax)
+    plt.show()
+    
+
```

### Comparing `pyees-1.3.9/pyees/profileFit.py` & `pyees-1.4.0/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/profilePyees.py` & `pyees-1.4.0/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/prop.py` & `pyees-1.4.0/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/sheet.py` & `pyees-1.4.0/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/solve.py` & `pyees-1.4.0/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/stackOverflowODR.py` & `pyees-1.4.0/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testFit.py` & `pyees-1.4.0/pyees/testFit.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,123 +63,115 @@
 
         F = lin_fit(x, y)
         Fa = F.coefficients[0]
         Fb = F.coefficients[1]
 
         self.assertAlmostEqual(Fa.value, 2)
         self.assertEqual(str(Fa.unit), 'DELTAC/m')
-        self.assertAlmostEqual(Fa.uncert, 0)
 
         self.assertAlmostEqual(Fb.value, 10)
         self.assertEqual(str(Fb.unit), 'C')
-        self.assertAlmostEqual(Fb.uncert, 0)
 
         self.assertAlmostEqual(F.r_squared, 1)
 
     def testPolFit2(self):
         a = 2
         b = 10
         c = 15
         n = 100
         x = np.linspace(0, 100, n)
         y = a * x**2 + b * x + c
-        # y += 10 * np.random.rand(n)
 
         x = variable(x, 'm')
         y = variable(y, 'C')
 
         F = pol_fit(x, y)
         Fa = F.coefficients[0]
         Fb = F.coefficients[1]
         Fc = F.coefficients[2]
 
         self.assertAlmostEqual(Fa.value, 2)
         self.assertEqual(str(Fa.unit), 'DELTAC/m2')
-        self.assertAlmostEqual(Fa.uncert, 0)
 
         self.assertAlmostEqual(Fb.value, 10)
         self.assertEqual(str(Fb.unit), 'DELTAC/m')
-        self.assertAlmostEqual(Fb.uncert, 0)
 
         self.assertAlmostEqual(Fc.value, 15)
         self.assertEqual(str(Fc.unit), 'C')
-        self.assertAlmostEqual(Fc.uncert, 0)
 
         self.assertAlmostEqual(F.r_squared, 1)
 
     def testPolFit3(self):
         a = 2
         b = 10
         c = 15
         d = 50
         n = 100
         x = np.linspace(0, 100, n)
         y = a * x**3 + b * x**2 + c * x + d
-        # y += 10 * np.random.rand(n)
 
         x = variable(x, 'm')
         y = variable(y, 'C')
 
         F = pol_fit(x, y, deg=3)
         Fa = F.coefficients[0]
         Fb = F.coefficients[1]
         Fc = F.coefficients[2]
         Fd = F.coefficients[3]
 
         self.assertAlmostEqual(Fa.value, 2)
         self.assertEqual(str(Fa.unit), 'DELTAC/m3')
-        self.assertAlmostEqual(Fa.uncert, 0)
 
         self.assertAlmostEqual(Fb.value, 10)
         self.assertEqual(str(Fb.unit), 'DELTAC/m2')
-        self.assertAlmostEqual(Fb.uncert, 0)
 
         self.assertAlmostEqual(Fc.value, 15)
         self.assertEqual(str(Fc.unit), 'DELTAC/m')
-        self.assertAlmostEqual(Fc.uncert, 0)
 
         self.assertAlmostEqual(Fd.value, 50)
         self.assertEqual(str(Fd.unit), 'C')
-        self.assertAlmostEqual(Fd.uncert, 0)
 
         self.assertAlmostEqual(F.r_squared, 1)
 
     def testExpFit(self):   
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100])
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
         f = exp_fit(x,y)
         
-        a,b,c,d  = f.coefficients
-
+        a,b,c  = f.coefficients
         self.assertEqual(b.unit, '1')
         self.assertEqual(a.unit, y.unit)
+        self.assertEqual(c.unit, y.unit)
         self.assertRelativeDifference(a.value, 0.9875635849080608, 5e-2)
-        self.assertRelativeDifference(b.value, 1.0515901240689571, 1e-3)
+        self.assertRelativeDifference(b.value, 0.04932224945938845, 1e-3)
+        self.assertEqual(c.value,0)
         
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100], 'C')
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
 
         with self.assertRaises(Exception) as context:
-            f = exp_fit(x,y)
+            f = exp_fit(x,y, p0 = [1,1,1,1])
         self.assertTrue('The variable "x" cannot have a unit' in str(context.exception))
        
         
     
 
     def testPowFit(self):    
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100])
         y = variable([2735.968626, 5013.971519, 6501.553987, 10229.42877, 10745.50817, 14982.43969, 17657.04326, 20032.85742, 23085.80822], 'kg/m3') 
-        f = pow_fit(x,y)
+        f = pow_fit(x,y, p0 = [1,1,0])
         
-        a,b  = f.coefficients
-
+        a,b,c  = f.coefficients
         self.assertEqual(b.unit, '1')
         self.assertEqual(a.unit, y.unit)
+        self.assertEqual(c.unit, y.unit)
         self.assertRelativeDifference(a.value, 54.1146149130, 5e-2)
         self.assertRelativeDifference(b.value, 1.3161605224, 1e-2)
+        self.assertEqual(c.value, 0)
+        
         
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100], 'C')
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
 
         with self.assertRaises(Exception) as context:
             f = pow_fit(x,y)
         self.assertTrue('The variable "x" cannot have a unit' in str(context.exception))
@@ -203,15 +195,15 @@
         self.assertRelativeDifference(c.value, 60, 1e-1)
         
     
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100], 'C')
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
 
         with self.assertRaises(Exception) as context:
-            f = logistic_fit(x,y)
+            f = logistic_fit(x,y, p0 = [1,1,1])
         self.assertTrue('The variable "x" cannot have a unit' in str(context.exception))
     
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `pyees-1.3.9/pyees/testProp.py` & `pyees-1.4.0/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testPyees.py` & `pyees-1.4.0/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testSheet.py` & `pyees-1.4.0/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testSolve.py` & `pyees-1.4.0/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testUnit.py` & `pyees-1.4.0/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/testVariable.py` & `pyees-1.4.0/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/unit.py` & `pyees-1.4.0/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees/variable.py` & `pyees-1.4.0/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.9/pyees.egg-info/PKG-INFO` & `pyees-1.4.0/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.9
+Version: 1.4.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.9/setup.py` & `pyees-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.9',
+    version='1.4.0',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

