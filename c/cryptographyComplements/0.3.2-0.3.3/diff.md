# Comparing `tmp/cryptographyComplements-0.3.2.tar.gz` & `tmp/cryptographyComplements-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.3.2.tar", last modified: Wed Jul 12 17:25:09 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.3.3.tar", last modified: Sun Jul 16 17:35:28 2023, max compression
```

## Comparing `cryptographyComplements-0.3.2.tar` & `cryptographyComplements-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.738794 cryptographyComplements-0.3.2/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-07-12 17:25:09.736615 cryptographyComplements-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.731896 cryptographyComplements-0.3.2/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.2/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-07-12 16:51:45.000000 cryptographyComplements-0.3.2/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    15876 2023-07-12 17:22:44.000000 cryptographyComplements-0.3.2/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2069 2023-07-12 17:15:11.000000 cryptographyComplements-0.3.2/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     3002 2023-07-07 17:40:51.000000 cryptographyComplements-0.3.2/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:25:09.735595 cryptographyComplements-0.3.2/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-07-12 17:25:09.000000 cryptographyComplements-0.3.2/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 17:25:09.739786 cryptographyComplements-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-07-12 16:56:08.000000 cryptographyComplements-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:28.613598 cryptographyComplements-0.3.3/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-07-16 17:35:28.612578 cryptographyComplements-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:28.606845 cryptographyComplements-0.3.3/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.3/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-07-12 16:51:45.000000 cryptographyComplements-0.3.3/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    15189 2023-07-16 17:09:32.000000 cryptographyComplements-0.3.3/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2069 2023-07-12 17:15:11.000000 cryptographyComplements-0.3.3/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3002 2023-07-07 17:40:51.000000 cryptographyComplements-0.3.3/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:35:28.610138 cryptographyComplements-0.3.3/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-16 17:35:28.000000 cryptographyComplements-0.3.3/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 17:35:28.613598 cryptographyComplements-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-07-16 17:35:21.000000 cryptographyComplements-0.3.3/setup.py
```

### Comparing `cryptographyComplements-0.3.2/LICENSE` & `cryptographyComplements-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.2/PKG-INFO` & `cryptographyComplements-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.3.2/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.3.3/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.2/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.3.3/cryptographyComplements/mathFunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,80 +253,62 @@
 
     return steps
 
 def FermatEulerTheorem(a:int, n:int) -> int:
     "From a given two given integers calculate Fermat-Euler Theorem. \n\nNote: a is the number and n is the modulo. Moreover, the function will return 1 if and only if a and are coprime positive."
     return pow(a, EulerTotientFunction(n), n)
 
-def EulerFormulaForPQ(p: int, q: int) -> bool:
-    "The Euler Formula from two given integers p and q returns True if the congruence a^((p-1)(q-1)/g) mod pq is congruent to 1 and False if it's not."
-
-    if p == 2 or q == 2:
-        return FermatEulerTheorem(p, q)
-
-    g = EuclideanAlgorithm(p-1, q-1)
-
-    a = pow(2, (p-1)*(q-1)//g, p*q) # 2 can be set, to the base, because is coprime with p*q if p or q isn't 2
-
-    if EuclideanAlgorithm(a, p*q) != 1:
-        return False
-
-    if pow(a, (p-1)*(q-1)//g, p*q) != 1:
-        return False
-
-    return True
-
 def PrimeNumberTheorem(n: int) -> float:
     "Calculate the Prime Number Theorem for n using n/ln(n). The value returned is an approximation."
 
     import math
 
     if n <= 1:
         return 0.0
     return n / (math.log(n)) # here log is the natural logarithm ln(x)
 
-from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
 class FactorizationMethods:
     "This class contains factorization methods, including special purpose and general purpose ones."
 
-    def TrialDivision(n: int, maxN: int) -> list:
+    def TrialDivision(n:int, maxN: int) -> list:
         "This factorization method uses the trial division and it's a special purpose algorithm, so it's not recommended for numbers that could be possibly be prime, or for large composites.\n\nNote: maxN defines the maximum value for which will be searched primes that factorize n. It has been implemented to avoid large computations. \nIf you want to search up to n, just put maxN=n"
 
-        from cryptographyComplements.tools import Numbers
+        from cryptographyComplements.primalityTests import MillerRabinPrimalityTest
+        import math
 
         if MillerRabinPrimalityTest(n, 100):
-            return [n]        
-
-        primeFactors = []
-        keep = n
-
-        for i in range(2, maxN+1):
+            return [n]
+        
+        factorization = []
+        maxNumber = math.sqrt(n)
 
-            flag = False
+        N = n
 
-            if n / i % 1 == 0:
+        while n % 2 == 0:
+            factorization.append(2)
+            n //= 2
 
-                for prime in primeFactors:
-                    if i/prime % 1 == 0:
-                        flag = True
-                        break
+        for d in range(3, n, 2):
+            if d > maxNumber or d>maxN:
+                break
 
-                if not flag:
-                    primeFactors.append(i)
-                    n /= i
+            while n % d == 0:
+                factorization.append(d)
+                n = n//d
+        
+        if n == 1:
+            return factorization
 
-                    while n/i % 1 == 0:
-                        primeFactors.append(i)
-                        n /= i
+        if maxN == N or maxN > N:
 
+            factorization.append(n)
 
-            if Numbers.listMultiplication(primeFactors) == keep:
-                break
+            return factorization
 
-        return primeFactors
+        return factorization
 
     def PollardRhoFactorizationAlgorithm(n: int) -> int:
         "The Pollard Rho factorization algorithm is a special purpose algorithm \n\n The algorithm returns a prime factor of n."
 
         def gx(x, n):
             return (x**2 + 1) % n
 
@@ -534,8 +516,7 @@
         for n in range(x, y+1, 2):
 
             if MillerRabinPrimalityTest(n, 100) and MillerRabinPrimalityTest(n+2, 100):
                 twinPrimes.append((n, n+2))
 
         return twinPrimes
     
-
```

### Comparing `cryptographyComplements-0.3.2/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.3.3/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.2/cryptographyComplements/tools.py` & `cryptographyComplements-0.3.3/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.2/setup.py` & `cryptographyComplements-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import decimal
 
 setup(
     name='cryptographyComplements',
-    version='0.3.2',
+    version='0.3.3',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

