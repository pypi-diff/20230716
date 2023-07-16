# Comparing `tmp/adadmire-0.0.9.tar.gz` & `tmp/adadmire-1.0.0.tar.gz`

## Comparing `adadmire-0.0.9.tar` & `adadmire-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,20 @@
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 adadmire-0.0.9/doc/contribute.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 adadmire-0.0.9/src/adadmire/__init__.py
--rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 adadmire-0.0.9/src/adadmire/apgpy.py
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 adadmire-0.0.9/src/adadmire/main.py
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 adadmire-0.0.9/src/adadmire/mgm.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 adadmire-0.0.9/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 adadmire-0.0.9/LICENSE
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 adadmire-0.0.9/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 adadmire-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 adadmire-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/levels.npy
+-rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/pheno.npy
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/pheno_with_stimulations.xlsx
+-rw-r--r--   0        0        0    39328 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0   310332 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/levels.npy
+-rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/pheno.npy
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/pheno.xlsx
+-rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 adadmire-1.0.0/doc/contribute.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/apgpy.py
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/main.py
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/mgm.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adadmire-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 adadmire-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 adadmire-1.0.0/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 adadmire-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 adadmire-1.0.0/PKG-INFO
```

### Comparing `adadmire-0.0.9/doc/contribute.md` & `adadmire-1.0.0/doc/contribute.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-# Contribute
-
-In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
-
-In case you want to **write code** for this package, please also create an [Issue](https://github.com/spang-lab/adadmire/issues) first, in which you describe your planned code contribution. After acceptance of your proposal by an active maintainer of the repository you will get permissions to create branches for this repository. After this, please follow the steps outlined in the following to create new versions of adadmire.
-
-🗒️Note: all following steps are based on <https://packaging.python.org/en/latest/tutorials/packaging-projects/>.
-
-⚠️Important: all commands mentioned in the following should be run from the root folder of this repository.
-
-1. **Make your code changes**
-2. **Increase the version** in [pyproject.toml](../pyproject.toml)
-3. **Build the package**:
-   * Run command `python -m pip install --upgrade build twine` to install modules [build](https://pypi.org/project/build/) and [twine](https://pypi.org/project/twine/) (required for building and uploading of packages) 
-   * Run command `python -m build` to generate pre-built version of your package (`dist/adadmire*.whl`) as well as a source version of your package (`dist/adadmire*.tar.gz`)
-4. **Upload to PyPI Test Server**: this step is optional and only required if you want to try out the upload and following installation.
-   * Run command `python -m twine upload --repository testpypi dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [test.pypi.org](https://test.pypi.org/) first! Please also note, that you need two separate accounts for [test.pypi.org](https://test.pypi.org/) and [pypi.org](https://pypi.org/).
-   * Check that your new version is listed at [test.pypi.org/project/adadmire](https://test.pypi.org/project/adadmire)
-   * Run command `python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire` to check that your new version can be installed via pip
-5. **Upload to PyPI Production Server**
-   * Run command `python -m twine upload dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [pypi.org](https://pypi.org/) first! Please also note, that you need two separate accounts for [pypi.org](https://pypi.org/) and [test.pypi.org](https://test.pypi.org/).
-   * Check that your new version is listed at [pypi.org/project/adadmire](https://pypi.org/project/adadmire)
-   * Run command `python -m pip install --upgrade adadmire` to check that your new version can be installed via pip
-
-All above commands in short
-
-```bash
-python -m pip install --upgrade build twine wheel # Update packages
-rm dist/* # Clean dist folder
-python -m build # Build package
-# IF POWERSHELL
-$whl=$(ls ./dist/adadmire-*-py3-none-any.whl).FullName
-python -m pip install $whl # Test installation locally
-# ELSE
-python -m pip install ./dist/adadmire-*-py3-none-any.whl
-# END IF
-python -m twine upload --repository testpypi dist/* # Upload to test server
-python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire
-python -m twine upload dist/* # Upload to production server
-python -m pip install --upgrade adadmire # Test installation from server
-```
-
-## Tips and Tricks
-
-### Create a .pypirc file
-
-Create a [.pypirc](https://packaging.python.org/en/latest/specifications/pypirc/) file in your local home directory. This way you don't have to type your PyPI username and password each time. Mine looks as follows:
-
-```
-[testpypi]
-repository = https://test.pypi.org/legacy/
-username = <my_test_pypi_username>
-password = <my_test_pypi_password>
-
-[pypi]
-repository = https://upload.pypi.org/legacy/
-username = <my_pypi_username>
-password = <my_pypi_password>
-```
+# Contribute
+
+In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
+
+In case you want to **write code** for this package, please also create an [Issue](https://github.com/spang-lab/adadmire/issues) first, in which you describe your planned code contribution. After acceptance of your proposal by an active maintainer of the repository you will get permissions to create branches for this repository. After this, please follow the steps outlined in the following to create new versions of adadmire.
+
+🗒️Note: all following steps are based on <https://packaging.python.org/en/latest/tutorials/packaging-projects/>.
+
+⚠️Important: all commands mentioned in the following should be run from the root folder of this repository.
+
+1. **Make your code changes**
+2. **Increase the version** in [pyproject.toml](../pyproject.toml)
+3. **Build the package**:
+   * Run command `python -m pip install --upgrade build twine` to install modules [build](https://pypi.org/project/build/) and [twine](https://pypi.org/project/twine/) (required for building and uploading of packages) 
+   * Run command `python -m build` to generate pre-built version of your package (`dist/adadmire*.whl`) as well as a source version of your package (`dist/adadmire*.tar.gz`)
+4. **Upload to PyPI Test Server**: this step is optional and only required if you want to try out the upload and following installation.
+   * Run command `python -m twine upload --repository testpypi dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [test.pypi.org](https://test.pypi.org/) first! Please also note, that you need two separate accounts for [test.pypi.org](https://test.pypi.org/) and [pypi.org](https://pypi.org/).
+   * Check that your new version is listed at [test.pypi.org/project/adadmire](https://test.pypi.org/project/adadmire)
+   * Run command `python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire` to check that your new version can be installed via pip
+5. **Upload to PyPI Production Server**
+   * Run command `python -m twine upload dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [pypi.org](https://pypi.org/) first! Please also note, that you need two separate accounts for [pypi.org](https://pypi.org/) and [test.pypi.org](https://test.pypi.org/).
+   * Check that your new version is listed at [pypi.org/project/adadmire](https://pypi.org/project/adadmire)
+   * Run command `python -m pip install --upgrade adadmire` to check that your new version can be installed via pip
+
+All above commands in short
+
+```bash
+python -m pip install --upgrade build twine wheel # Update packages
+rm dist/* # Clean dist folder
+python -m build # Build package. IMPORTANT: version updated in pyproject.toml?
+# IF POWERSHELL
+$whl=$(ls ./dist/adadmire-*-py3-none-any.whl).FullName
+python -m pip install $whl # Test installation locally
+# ELSE
+python -m pip install ./dist/adadmire-*-py3-none-any.whl
+# END IF
+python -m twine upload --repository testpypi dist/* # Upload to test server
+python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire
+python -m twine upload dist/* # Upload to production server
+python -m pip install --upgrade adadmire # Test installation from server
+# IMPORTANT: do not forget to push your changes to Github as well ;)
+```
+
+## Tips and Tricks
+
+### Create a .pypirc file
+
+Create a [.pypirc](https://packaging.python.org/en/latest/specifications/pypirc/) file in your local home directory. This way you don't have to type your PyPI username and password each time. Mine looks as follows:
+
+```
+[testpypi]
+repository = https://test.pypi.org/legacy/
+username = <my_test_pypi_username>
+password = <my_test_pypi_password>
+
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = <my_pypi_username>
+password = <my_pypi_password>
+```
```

### Comparing `adadmire-0.0.9/src/adadmire/apgpy.py` & `adadmire-1.0.0/src/adadmire/apgpy.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-# Copyright (c) 2012-2013, Brendan O'Donoghue (bodonoghue85@gmail.com)
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions are met:
-#
-# 1. Redistributions of source code must retain the above copyright notice, this
-#    list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright notice,
-#    this list of conditions and the following disclaimer in the documentation
-#    and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
-# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-#
-# The views and conclusions contained in the software and documentation are those
-# of the authors and should not be interpreted as representing official policies,
-# either expressed or implied, of the FreeBSD Project, the Air Force Research
-# Laboratory, or the U.S. Government.
-
-
-# Note from Tobias Schmidt: this file contains source code from the package
-# apgpy (https://github.com/bodono/apgpy). Package apgpy is not available via
-# PyPI (https://pypi.org) and therefore cannot be resolved automatically by
-# pip. We include its source code directly within this package to make
-# installation via pip possible. This is explicictly allowed by the license of
-# apgpy (see above).
-from __future__ import print_function
-import numpy as np
-from functools import partial
-
-class IWrapper:
-    def dot(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __add__(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __sub__(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __mul__(self, scalar):
-        raise NotImplementedError("Implement in subclass")
-
-    def copy(self):
-        raise NotImplementedError("Implement in subclass")
-
-    def norm(self):
-        raise NotImplementedError("Implement in subclass")
-
-    @property
-    def data(self):
-        return self
-
-    __rmul__ = __mul__
-
-
-class NumpyWrapper(IWrapper):
-    def __init__(self, nparray):
-        self._nparray = nparray
-
-    def dot(self, other):
-        return np.inner(self.data, other.data)
-
-    def __add__(self, other):
-        return NumpyWrapper(self.data + other.data)
-
-    def __sub__(self, other):
-        return NumpyWrapper(self.data - other.data)
-
-    def __mul__(self, scalar):
-        return NumpyWrapper(self.data * scalar)
-
-    def copy(self):
-        return NumpyWrapper(np.copy(self.data))
-
-    def norm(self):
-        return np.linalg.norm(self.data)
-
-    @property
-    def data(self):
-        return self._nparray
-
-    __rmul__ = __mul__
-
-
-def npwrap(x):
-    if isinstance(x, np.ndarray):
-        return NumpyWrapper(x)
-    return x
-
-
-def npwrapfunc(f, *args):
-    return npwrap(f(*args))
-
-
-def solve(grad_f, prox_h, x_init,
-          max_iters=2500,
-          eps=1e-6,
-          alpha=1.01,
-          beta=0.5,
-          use_restart=True,
-          gen_plots=False,
-          quiet=False,
-          use_gra=False,
-          step_size=False,
-          fixed_step_size=False,
-          debug=False):
-
-    df = partial(npwrapfunc, grad_f)
-    ph = partial(npwrapfunc, prox_h)
-
-    x_init = npwrap(x_init)
-
-    x = x_init.copy()
-    y = x.copy()
-    g = df(y.data)
-    theta = 1.
-
-    if not step_size:
-        # barzilai-borwein step-size initialization:
-        t = 1. / g.norm()
-        x_hat = x - t * g
-        g_hat = df(x_hat.data)
-        t = abs((x - x_hat).dot(g - g_hat) / (g - g_hat).norm() ** 2)
-    else:
-        t = step_size
-
-    if gen_plots:
-        errs = np.zeros(max_iters)
-
-    k = 0
-    err1 = np.nan
-    iter_str = 'iter num %i, norm(Gk)/(1+norm(xk)): %1.2e, step-size: %1.2e'
-    for k in range(max_iters):
-
-        if not quiet and k % 100 == 0:
-            print(iter_str % (k, err1, t))
-
-        x_old = x.copy()
-        y_old = y.copy()
-
-        x = y - t * g
-
-        if prox_h:
-            x = ph(x.data, t)
-
-        err1 = (y - x).norm() / (1 + x.norm()) / t
-
-        if gen_plots:
-            errs[k] = err1
-
-        if err1 < eps:
-            break
-
-        if not use_gra:
-            theta = 2. / (1 + np.sqrt(1 + 4 / (theta ** 2)))
-        else:
-            theta = 1.
-
-        if not use_gra and use_restart and (y - x).dot(x - x_old) > 0:
-            if debug:
-                print('restart, dg = %1.2e' % (y - x).dot(x - x_old))
-            x = x_old.copy()
-            y = x.copy()
-            theta = 1.
-        else:
-            y = x + (1 - theta) * (x - x_old)
-
-        g_old = g.copy()
-        g = df(y.data)
-
-        # tfocs-style backtracking:
-        if not fixed_step_size:
-            t_old = t
-            t_hat = 0.5 * ((y - y_old).norm() ** 2) / \
-                abs((y - y_old).dot(g_old - g))
-            t = min(alpha * t, max(beta * t, t_hat))
-            if debug:
-                if t_old > t:
-                    print('back-track, t = %1.2e, t_old = %1.2e, t_hat = %1.2e' %
-                          (t, t_old, t_hat))
-
-    if not quiet:
-        print(iter_str % (k, err1, t))
-        print('terminated')
-    if gen_plots:
-        import matplotlib.pyplot as plt
-        errs = errs[1:k]
-        plt.figure()
-        plt.semilogy(errs[1:k])
-        plt.xlabel('iters')
-        plt.title('||Gk||/(1+||xk||)')
-        plt.draw()
-
-    return x.data
+# Copyright (c) 2012-2013, Brendan O'Donoghue (bodonoghue85@gmail.com)
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+#
+# The views and conclusions contained in the software and documentation are those
+# of the authors and should not be interpreted as representing official policies,
+# either expressed or implied, of the FreeBSD Project, the Air Force Research
+# Laboratory, or the U.S. Government.
+
+
+# Note from Tobias Schmidt: this file contains source code from the package
+# apgpy (https://github.com/bodono/apgpy). Package apgpy is not available via
+# PyPI (https://pypi.org) and therefore cannot be resolved automatically by
+# pip. We include its source code directly within this package to make
+# installation via pip possible. This is explicictly allowed by the license of
+# apgpy (see above).
+from __future__ import print_function
+import numpy as np
+from functools import partial
+
+class IWrapper:
+    def dot(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __add__(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __sub__(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __mul__(self, scalar):
+        raise NotImplementedError("Implement in subclass")
+
+    def copy(self):
+        raise NotImplementedError("Implement in subclass")
+
+    def norm(self):
+        raise NotImplementedError("Implement in subclass")
+
+    @property
+    def data(self):
+        return self
+
+    __rmul__ = __mul__
+
+
+class NumpyWrapper(IWrapper):
+    def __init__(self, nparray):
+        self._nparray = nparray
+
+    def dot(self, other):
+        return np.inner(self.data, other.data)
+
+    def __add__(self, other):
+        return NumpyWrapper(self.data + other.data)
+
+    def __sub__(self, other):
+        return NumpyWrapper(self.data - other.data)
+
+    def __mul__(self, scalar):
+        return NumpyWrapper(self.data * scalar)
+
+    def copy(self):
+        return NumpyWrapper(np.copy(self.data))
+
+    def norm(self):
+        return np.linalg.norm(self.data)
+
+    @property
+    def data(self):
+        return self._nparray
+
+    __rmul__ = __mul__
+
+
+def npwrap(x):
+    if isinstance(x, np.ndarray):
+        return NumpyWrapper(x)
+    return x
+
+
+def npwrapfunc(f, *args):
+    return npwrap(f(*args))
+
+
+def solve(grad_f, prox_h, x_init,
+          max_iters=2500,
+          eps=1e-6,
+          alpha=1.01,
+          beta=0.5,
+          use_restart=True,
+          gen_plots=False,
+          quiet=False,
+          use_gra=False,
+          step_size=False,
+          fixed_step_size=False,
+          debug=False):
+
+    df = partial(npwrapfunc, grad_f)
+    ph = partial(npwrapfunc, prox_h)
+
+    x_init = npwrap(x_init)
+
+    x = x_init.copy()
+    y = x.copy()
+    g = df(y.data)
+    theta = 1.
+
+    if not step_size:
+        # barzilai-borwein step-size initialization:
+        t = 1. / g.norm()
+        x_hat = x - t * g
+        g_hat = df(x_hat.data)
+        t = abs((x - x_hat).dot(g - g_hat) / (g - g_hat).norm() ** 2)
+    else:
+        t = step_size
+
+    if gen_plots:
+        errs = np.zeros(max_iters)
+
+    k = 0
+    err1 = np.nan
+    iter_str = 'iter num %i, norm(Gk)/(1+norm(xk)): %1.2e, step-size: %1.2e'
+    for k in range(max_iters):
+
+        if not quiet and k % 100 == 0:
+            print(iter_str % (k, err1, t))
+
+        x_old = x.copy()
+        y_old = y.copy()
+
+        x = y - t * g
+
+        if prox_h:
+            x = ph(x.data, t)
+
+        err1 = (y - x).norm() / (1 + x.norm()) / t
+
+        if gen_plots:
+            errs[k] = err1
+
+        if err1 < eps:
+            break
+
+        if not use_gra:
+            theta = 2. / (1 + np.sqrt(1 + 4 / (theta ** 2)))
+        else:
+            theta = 1.
+
+        if not use_gra and use_restart and (y - x).dot(x - x_old) > 0:
+            if debug:
+                print('restart, dg = %1.2e' % (y - x).dot(x - x_old))
+            x = x_old.copy()
+            y = x.copy()
+            theta = 1.
+        else:
+            y = x + (1 - theta) * (x - x_old)
+
+        g_old = g.copy()
+        g = df(y.data)
+
+        # tfocs-style backtracking:
+        if not fixed_step_size:
+            t_old = t
+            t_hat = 0.5 * ((y - y_old).norm() ** 2) / \
+                abs((y - y_old).dot(g_old - g))
+            t = min(alpha * t, max(beta * t, t_hat))
+            if debug:
+                if t_old > t:
+                    print('back-track, t = %1.2e, t_old = %1.2e, t_hat = %1.2e' %
+                          (t, t_old, t_hat))
+
+    if not quiet:
+        print(iter_str % (k, err1, t))
+        print('terminated')
+    if gen_plots:
+        import matplotlib.pyplot as plt
+        errs = errs[1:k]
+        plt.figure()
+        plt.semilogy(errs[1:k])
+        plt.xlabel('iters')
+        plt.title('||Gk||/(1+||xk||)')
+        plt.draw()
+
+    return x.data
```

### Comparing `adadmire-0.0.9/src/adadmire/mgm.py` & `adadmire-1.0.0/src/adadmire/mgm.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-# MIT License
-# Copyright (c) 2019 Michael Altenbuchinger and Helena Zacharias
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import numpy as np
-import adadmire.apgpy as apg
-
-def grad_neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
-    n = X.shape[0]
-    p = B.shape[0]
-    q = levels.shape[0]
-
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    for r in range(0, q):
-        Phi[int(levelSum[r]):int(levelSum[r]+levels[r]),
-            int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
-
-    Bd = np.diag(B)
-    B = B - np.diag(Bd)
-    B = np.triu(B)
-    B = B + np.transpose(B)
-    DRho = np.dot(D, Rho)
-    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1., p), Bd)))
-    XB = np.dot(X, B)
-    XB = np.dot(XB, np.diag(np.divide(np.repeat(1., p), Bd)))
-    consts = np.tile(alphap, (n, 1))
-    Xt = np.transpose(X)
-    res = consts + DRho + XB + X
-    gradBd = np.repeat(0., p)
-
-    for s in range(0, p):
-        gradBd[s] = - n/(2.*Bd[s]) - .5*np.dot(res[:, s], res[:, s]
-                                              ) + np.dot(res[:, s], XB[:, s] +
-                                                         DRho[:, s])
-
-    gradB = - np.dot(Xt, res)
-    gradB = gradB - np.diag(np.diag(gradB))
-    gradB = np.transpose(np.tril(gradB)) + np.triu(gradB)
-    gradalphap = - np.dot(np.diag(Bd), np.sum(res, axis=0)[:, np.newaxis])
-    gradalphap = gradalphap[:, 0]
-
-    gradRho = - np.dot(np.transpose(D), res)
-
-    Xt = np.transpose(X)
-    RhoX = np.dot(Rho, Xt)
-    Phi = Phi - np.diag(np.diag(Phi))
-    Phi = np.triu(Phi)
-    Phi = Phi + np.transpose(Phi)
-    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
-    PhiD = np.dot(Phi, np.transpose(D))
-    discprod = np.transpose(RhoX+Phirr+PhiD)
-
-    for r in range(0, q):
-        disctemp = discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
-        denominator = np.logaddexp.reduce(disctemp, axis=1)
-        disctemp = disctemp - denominator[:, np.newaxis]
-        disctemp = np.exp(disctemp)
-        temp = disctemp - D[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
-        discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])] = temp
-
-    gradalphaq = np.sum(discprod, axis=0)
-    gradw = np.dot(Xt, discprod)
-    gradRho = gradRho+np.transpose(gradw)
-    gradPhi = np.dot(np.transpose(D), discprod)
-
-    for r in range(0, q):
-        gradPhi[int(levelSum[r]):int(levelSum[r]+levels[r]),
-                int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
-
-    gradPhi = np.transpose(np.tril(gradPhi))+np.triu(gradPhi)
-    gradB.flat[::p+1] = gradBd
-    gradB = gradB/n
-    gradRho = gradRho/n
-    gradPhi = gradPhi/n
-    gradalphap = gradalphap/n
-    gradalphaq = gradalphaq/n
-    return gradB, gradRho, gradPhi, gradalphap, gradalphaq
-
-
-def neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
-    n = X.shape[0]
-    p = B.shape[0]
-    q = levels.shape[0]
-    Bd = np.diag(B)
-    B = B - np.diag(Bd)
-    B = np.triu(B)
-    B = B + np.transpose(B)
-    DRho = np.dot(D, Rho)
-    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1, p), Bd)))
-    XB = np.dot(X, B)
-    XB = np.dot(XB, np.diag(np.divide(np.repeat(1, p), Bd)))
-    Xt = np.transpose(X)
-    RhoX = np.dot(Rho, Xt)
-    Phi = Phi - np.diag(np.diag(Phi))
-    Phi = np.triu(Phi)
-    Phi = Phi + np.transpose(Phi)
-    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
-    PhiD = np.dot(Phi, np.transpose(D))
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    consts = np.tile(alphap, (n, 1))
-    PLcont1 = -n/2.*np.sum(np.log(-Bd)) #here, the constant term is neglected
-    PLcont2 = consts + DRho + XB + X
-    PLcont2 = np.dot(PLcont2, np.diag(np.sqrt(-Bd)))
-    PLcont2 = np.multiply(PLcont2, PLcont2)
-    PLcont2 = 0.5*np.sum(np.sum(PLcont2, axis=0))
-    temp = RhoX+Phirr+PhiD
-    PLdisc = 0
-    for r in range(0, q):
-        temp2 = temp[int(levelSum[r]):int(levelSum[r]+levels[r]), :]
-        denominator = np.sum(
-            np.exp(np.dot(np.identity(int(levels[r])), temp2)), axis=0)
-        numerator = np.sum(np.multiply(D[:, int(levelSum[r]):int(
-            levelSum[r]+levels[r])], np.transpose(temp2)), axis=1)
-        PLdisc = PLdisc-numerator+np.log(denominator)
-    PLdisc = np.sum(PLdisc)
-    return((PLcont1+PLcont2+PLdisc)/n)
-
-
-def neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
-    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
-    x1 = neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
-    return(x1)
-
-
-def B_Rho_Phi_alphap_alphaq(B, Rho, Phi, alphap, alphaq):
-    p = B.shape[0]
-    q = Phi.shape[0]
-    sizes = np.cumsum([p*p, p*q, q*q, p, q])
-    x = np.repeat(0., sizes[4])
-    x[0:sizes[0]] = np.reshape(B, (1, p*p))[0, :]
-    x[sizes[0]:sizes[1]] = np.reshape(Rho, (1, p*q))[0, :]
-    x[sizes[1]:sizes[2]] = np.reshape(Phi, (1, q*q))[0, :]
-    x[sizes[2]:sizes[3]] = alphap
-    x[sizes[3]:sizes[4]] = alphaq
-    return(x)
-
-
-def Inv_B_Rho_Phi_alphap_alphaq(x, p, q):
-    sizes = np.cumsum([p*p, p*q, q*q, p, q])
-    B = np.reshape(x[0:sizes[0]], (p, p))
-    Rho = np.reshape(x[sizes[0]:sizes[1]], (q, p))
-    Phi = np.reshape(x[sizes[1]:sizes[2]], (q, q))
-    alphap = x[sizes[2]:sizes[3]]
-    alphaq = x[sizes[3]:sizes[4]]
-    return(B, Rho, Phi, alphap, alphaq)
-
-
-def grad_neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
-    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
-    x1 = grad_neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
-    return(x1[0], x1[1], x1[2], x1[3], x1[4])
-
-
-def make_starting_parameters(X, D, levels):
-    p = X.shape[1]
-    q = D.shape[1]
-    B = -np.diag(np.repeat(1, p))
-    Rho = np.zeros((q, p))
-    Phi = np.zeros((q, q))
-    alphap = np.zeros(p)
-    alphaq = np.zeros(q)
-    return(B, Rho, Phi, alphap, alphaq, p, q)
-
-
-def grad_f_temp(x, X, D, levels, p, q):
-    x2 = grad_neglogli_plain(x, X, D, levels, p, q)
-    x3 = B_Rho_Phi_alphap_alphaq(x2[0], x2[1], x2[2], x2[3], x2[4])
-    return(x3)
-
-
-def prox_enet(x, l_l1, l_l2, t, pen, p0, tol0):
-    prox_l1 = np.sign(x) * np.maximum(abs(x) - t * l_l1 * pen, 0)
-    return prox_l1 / (1. + t * l_l2 * pen)
-
-
-def make_penalty_factors(X, D, levels):
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    p = X.shape[1]
-    qL = len(levels)
-    q = np.sum(levels)
-    sds = np.reshape(np.std(X, axis=0), (p, 1))
-    ps = np.reshape(np.mean(D, axis=0), (q, 1))
-    B = np.ones((p, p)) - np.diag(np.repeat(1, p))
-    B = np.multiply(B, np.dot(sds, np.transpose(sds)))
-    Rho = np.ones((q, p))
-    Phi = np.ones((q, q))
-    alphap = np.zeros(p)
-    alphaq = np.zeros(q)
-    for r in range(0, qL):
-        Phi[int(levelSum[r]), :] = np.repeat(10, Phi.shape[1])
-        Phi[:, int(levelSum[r])] = np.repeat(10, Phi.shape[1])
-        ps_t = ps[int(levelSum[r]):int(levelSum[r]+levels[r])]
-        ps[int(levelSum[r]):int(levelSum[r]+levels[r])
-           ] = np.sqrt(np.sum(ps_t*(1-ps_t)))
-        Rho[int(levelSum[r]), :] = np.repeat(10, Rho.shape[1])
-    Rho = np.multiply(Rho, np.dot(ps, np.transpose(sds)))
-    Phi = np.multiply(Phi, np.dot(ps, np.transpose(ps)))
-    return(B, Rho, Phi, alphap, alphaq, p, q)
-
-
-def Fit_MGM(X, D, levels, lambda_seq, iterations, eps=1e-6):
-    p = X.shape[1]
-    q = D.shape[1]
-    start = make_starting_parameters(X, D, levels)
-    start = B_Rho_Phi_alphap_alphaq(
-        start[0], start[1], start[2], start[3], start[4])
-    penalty = make_penalty_factors(X, D, levels)
-    penalty = B_Rho_Phi_alphap_alphaq(
-        penalty[0], penalty[1], penalty[2], penalty[3], penalty[4])
-    x_start = np.zeros(penalty.shape[0])
-
-    def grad_f(x): return grad_f_temp(x + x_start, X, D, levels, p, q)
-
-    def fun(x): return neglogli_plain(x + x_start, X, D, levels, p, q)
-    x_list = [None]*lambda_seq.shape[0]
-    xtemp = start
-    for i in range(0, lambda_seq.shape[0]):
-        l_l1 = lambda_seq[i]
-        print("lambda =", l_l1)
-
-        def prox_g(x, l): return prox_enet(
-            x, l_l1, 0, t=l, pen=penalty, p0=p, tol0=eps)
-        x_fista = apg.solve(grad_f, prox_g, xtemp, eps=eps,
-                            max_iters=iterations, gen_plots=False,
-                            debug=False)
-        x_list[i] = Inv_B_Rho_Phi_alphap_alphaq(x_fista, p, q)
-        xtemp = x_fista
-    loss_list = []
-    k = 0
-    for j in range(0, len(x_list)):
-        k = k+1
-        loss_vec = neglogli(
-            x_list[j][0], x_list[j][1], x_list[j][2], x_list[j][3],
-            x_list[j][4], X, D, levels)
-        loss_list = np.append(loss_list, loss_vec)
-    return([x_list, loss_list])
+# MIT License
+# Copyright (c) 2019 Michael Altenbuchinger and Helena Zacharias
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import numpy as np
+import adadmire.apgpy as apg
+
+def grad_neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
+    n = X.shape[0]
+    p = B.shape[0]
+    q = levels.shape[0]
+
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    for r in range(0, q):
+        Phi[int(levelSum[r]):int(levelSum[r]+levels[r]),
+            int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
+
+    Bd = np.diag(B)
+    B = B - np.diag(Bd)
+    B = np.triu(B)
+    B = B + np.transpose(B)
+    DRho = np.dot(D, Rho)
+    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1., p), Bd)))
+    XB = np.dot(X, B)
+    XB = np.dot(XB, np.diag(np.divide(np.repeat(1., p), Bd)))
+    consts = np.tile(alphap, (n, 1))
+    Xt = np.transpose(X)
+    res = consts + DRho + XB + X
+    gradBd = np.repeat(0., p)
+
+    for s in range(0, p):
+        gradBd[s] = - n/(2.*Bd[s]) - .5*np.dot(res[:, s], res[:, s]
+                                              ) + np.dot(res[:, s], XB[:, s] +
+                                                         DRho[:, s])
+
+    gradB = - np.dot(Xt, res)
+    gradB = gradB - np.diag(np.diag(gradB))
+    gradB = np.transpose(np.tril(gradB)) + np.triu(gradB)
+    gradalphap = - np.dot(np.diag(Bd), np.sum(res, axis=0)[:, np.newaxis])
+    gradalphap = gradalphap[:, 0]
+
+    gradRho = - np.dot(np.transpose(D), res)
+
+    Xt = np.transpose(X)
+    RhoX = np.dot(Rho, Xt)
+    Phi = Phi - np.diag(np.diag(Phi))
+    Phi = np.triu(Phi)
+    Phi = Phi + np.transpose(Phi)
+    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
+    PhiD = np.dot(Phi, np.transpose(D))
+    discprod = np.transpose(RhoX+Phirr+PhiD)
+
+    for r in range(0, q):
+        disctemp = discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
+        denominator = np.logaddexp.reduce(disctemp, axis=1)
+        disctemp = disctemp - denominator[:, np.newaxis]
+        disctemp = np.exp(disctemp)
+        temp = disctemp - D[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
+        discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])] = temp
+
+    gradalphaq = np.sum(discprod, axis=0)
+    gradw = np.dot(Xt, discprod)
+    gradRho = gradRho+np.transpose(gradw)
+    gradPhi = np.dot(np.transpose(D), discprod)
+
+    for r in range(0, q):
+        gradPhi[int(levelSum[r]):int(levelSum[r]+levels[r]),
+                int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
+
+    gradPhi = np.transpose(np.tril(gradPhi))+np.triu(gradPhi)
+    gradB.flat[::p+1] = gradBd
+    gradB = gradB/n
+    gradRho = gradRho/n
+    gradPhi = gradPhi/n
+    gradalphap = gradalphap/n
+    gradalphaq = gradalphaq/n
+    return gradB, gradRho, gradPhi, gradalphap, gradalphaq
+
+
+def neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
+    n = X.shape[0]
+    p = B.shape[0]
+    q = levels.shape[0]
+    Bd = np.diag(B)
+    B = B - np.diag(Bd)
+    B = np.triu(B)
+    B = B + np.transpose(B)
+    DRho = np.dot(D, Rho)
+    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1, p), Bd)))
+    XB = np.dot(X, B)
+    XB = np.dot(XB, np.diag(np.divide(np.repeat(1, p), Bd)))
+    Xt = np.transpose(X)
+    RhoX = np.dot(Rho, Xt)
+    Phi = Phi - np.diag(np.diag(Phi))
+    Phi = np.triu(Phi)
+    Phi = Phi + np.transpose(Phi)
+    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
+    PhiD = np.dot(Phi, np.transpose(D))
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    consts = np.tile(alphap, (n, 1))
+    PLcont1 = -n/2.*np.sum(np.log(-Bd)) #here, the constant term is neglected
+    PLcont2 = consts + DRho + XB + X
+    PLcont2 = np.dot(PLcont2, np.diag(np.sqrt(-Bd)))
+    PLcont2 = np.multiply(PLcont2, PLcont2)
+    PLcont2 = 0.5*np.sum(np.sum(PLcont2, axis=0))
+    temp = RhoX+Phirr+PhiD
+    PLdisc = 0
+    for r in range(0, q):
+        temp2 = temp[int(levelSum[r]):int(levelSum[r]+levels[r]), :]
+        denominator = np.sum(
+            np.exp(np.dot(np.identity(int(levels[r])), temp2)), axis=0)
+        numerator = np.sum(np.multiply(D[:, int(levelSum[r]):int(
+            levelSum[r]+levels[r])], np.transpose(temp2)), axis=1)
+        PLdisc = PLdisc-numerator+np.log(denominator)
+    PLdisc = np.sum(PLdisc)
+    return((PLcont1+PLcont2+PLdisc)/n)
+
+
+def neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
+    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
+    x1 = neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
+    return(x1)
+
+
+def B_Rho_Phi_alphap_alphaq(B, Rho, Phi, alphap, alphaq):
+    p = B.shape[0]
+    q = Phi.shape[0]
+    sizes = np.cumsum([p*p, p*q, q*q, p, q])
+    x = np.repeat(0., sizes[4])
+    x[0:sizes[0]] = np.reshape(B, (1, p*p))[0, :]
+    x[sizes[0]:sizes[1]] = np.reshape(Rho, (1, p*q))[0, :]
+    x[sizes[1]:sizes[2]] = np.reshape(Phi, (1, q*q))[0, :]
+    x[sizes[2]:sizes[3]] = alphap
+    x[sizes[3]:sizes[4]] = alphaq
+    return(x)
+
+
+def Inv_B_Rho_Phi_alphap_alphaq(x, p, q):
+    sizes = np.cumsum([p*p, p*q, q*q, p, q])
+    B = np.reshape(x[0:sizes[0]], (p, p))
+    Rho = np.reshape(x[sizes[0]:sizes[1]], (q, p))
+    Phi = np.reshape(x[sizes[1]:sizes[2]], (q, q))
+    alphap = x[sizes[2]:sizes[3]]
+    alphaq = x[sizes[3]:sizes[4]]
+    return(B, Rho, Phi, alphap, alphaq)
+
+
+def grad_neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
+    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
+    x1 = grad_neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
+    return(x1[0], x1[1], x1[2], x1[3], x1[4])
+
+
+def make_starting_parameters(X, D, levels):
+    p = X.shape[1]
+    q = D.shape[1]
+    B = -np.diag(np.repeat(1, p))
+    Rho = np.zeros((q, p))
+    Phi = np.zeros((q, q))
+    alphap = np.zeros(p)
+    alphaq = np.zeros(q)
+    return(B, Rho, Phi, alphap, alphaq, p, q)
+
+
+def grad_f_temp(x, X, D, levels, p, q):
+    x2 = grad_neglogli_plain(x, X, D, levels, p, q)
+    x3 = B_Rho_Phi_alphap_alphaq(x2[0], x2[1], x2[2], x2[3], x2[4])
+    return(x3)
+
+
+def prox_enet(x, l_l1, l_l2, t, pen, p0, tol0):
+    prox_l1 = np.sign(x) * np.maximum(abs(x) - t * l_l1 * pen, 0)
+    return prox_l1 / (1. + t * l_l2 * pen)
+
+
+def make_penalty_factors(X, D, levels):
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    p = X.shape[1]
+    qL = len(levels)
+    q = np.sum(levels)
+    sds = np.reshape(np.std(X, axis=0), (p, 1))
+    ps = np.reshape(np.mean(D, axis=0), (q, 1))
+    B = np.ones((p, p)) - np.diag(np.repeat(1, p))
+    B = np.multiply(B, np.dot(sds, np.transpose(sds)))
+    Rho = np.ones((q, p))
+    Phi = np.ones((q, q))
+    alphap = np.zeros(p)
+    alphaq = np.zeros(q)
+    for r in range(0, qL):
+        Phi[int(levelSum[r]), :] = np.repeat(10, Phi.shape[1])
+        Phi[:, int(levelSum[r])] = np.repeat(10, Phi.shape[1])
+        ps_t = ps[int(levelSum[r]):int(levelSum[r]+levels[r])]
+        ps[int(levelSum[r]):int(levelSum[r]+levels[r])
+           ] = np.sqrt(np.sum(ps_t*(1-ps_t)))
+        Rho[int(levelSum[r]), :] = np.repeat(10, Rho.shape[1])
+    Rho = np.multiply(Rho, np.dot(ps, np.transpose(sds)))
+    Phi = np.multiply(Phi, np.dot(ps, np.transpose(ps)))
+    return(B, Rho, Phi, alphap, alphaq, p, q)
+
+
+def Fit_MGM(X, D, levels, lambda_seq, iterations, eps=1e-6):
+    p = X.shape[1]
+    q = D.shape[1]
+    start = make_starting_parameters(X, D, levels)
+    start = B_Rho_Phi_alphap_alphaq(
+        start[0], start[1], start[2], start[3], start[4])
+    penalty = make_penalty_factors(X, D, levels)
+    penalty = B_Rho_Phi_alphap_alphaq(
+        penalty[0], penalty[1], penalty[2], penalty[3], penalty[4])
+    x_start = np.zeros(penalty.shape[0])
+
+    def grad_f(x): return grad_f_temp(x + x_start, X, D, levels, p, q)
+
+    def fun(x): return neglogli_plain(x + x_start, X, D, levels, p, q)
+    x_list = [None]*lambda_seq.shape[0]
+    xtemp = start
+    for i in range(0, lambda_seq.shape[0]):
+        l_l1 = lambda_seq[i]
+        print("lambda =", l_l1)
+
+        def prox_g(x, l): return prox_enet(
+            x, l_l1, 0, t=l, pen=penalty, p0=p, tol0=eps)
+        x_fista = apg.solve(grad_f, prox_g, xtemp, eps=eps,
+                            max_iters=iterations, gen_plots=False,
+                            debug=False)
+        x_list[i] = Inv_B_Rho_Phi_alphap_alphaq(x_fista, p, q)
+        xtemp = x_fista
+    loss_list = []
+    k = 0
+    for j in range(0, len(x_list)):
+        k = k+1
+        loss_vec = neglogli(
+            x_list[j][0], x_list[j][1], x_list[j][2], x_list[j][3],
+            x_list[j][4], X, D, levels)
+        loss_list = np.append(loss_list, loss_vec)
+    return([x_list, loss_list])
```

### Comparing `adadmire-0.0.9/pyproject.toml` & `adadmire-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "adadmire"
-version = "0.0.9"
-authors = [
-  { name="Lena Buck", email="lena.buck@ukr.de" },
-  { name="Tobias Schmidt", email="tobias2.schmidt@ukr.de" },
-]
-description = "Functions for detecting anomalies in tabular datasets using Mixed Graphical Models."
-dependencies = []
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/spang-lab/adadmire"
-"Bug Tracker" = "https://github.com/spang-lab/adadmire/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "adadmire"
+version = "1.0.0"
+authors = [
+  { name="Lena Buck", email="lena.buck@ukr.de" },
+  { name="Tobias Schmidt", email="tobias2.schmidt@ukr.de" },
+]
+description = "Functions for detecting anomalies in tabular datasets using Mixed Graphical Models."
+dependencies = []
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/spang-lab/adadmire"
+"Bug Tracker" = "https://github.com/spang-lab/adadmire/issues"
```

