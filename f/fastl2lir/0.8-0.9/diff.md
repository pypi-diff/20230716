# Comparing `tmp/fastl2lir-0.8-py2.py3-none-any.whl.zip` & `tmp/fastl2lir-0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 6810 bytes, number of entries: 8
+Zip file size: 4527 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       33 b- defN 19-Dec-10 15:49 fastl2lir/__init__.py
--rw-r--r--  2.0 unx     7570 b- defN 22-Jan-16 08:04 fastl2lir/fastl2lir.py
--rw-r--r--  2.0 unx     7612 b- defN 21-Oct-27 16:02 fastl2lir/jax.py
--rw-r--r--  2.0 unx     1069 b- defN 22-Jan-16 08:10 fastl2lir-0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      390 b- defN 22-Jan-16 08:10 fastl2lir-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jan-16 08:10 fastl2lir-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Jan-16 08:10 fastl2lir-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      614 b- defN 22-Jan-16 08:10 fastl2lir-0.8.dist-info/RECORD
-8 files, 17408 bytes uncompressed, 5744 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     7794 b- defN 22-Mar-15 12:01 fastl2lir/fastl2lir.py
+-rw-r--r--  2.0 unx     1069 b- defN 22-Mar-15 12:02 fastl2lir-0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      390 b- defN 22-Mar-15 12:02 fastl2lir-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-Mar-15 12:02 fastl2lir-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 22-Mar-15 12:02 fastl2lir-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      541 b- defN 22-Mar-15 12:02 fastl2lir-0.9.dist-info/RECORD
+7 files, 9947 bytes uncompressed, 3569 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: fastl2lir/__init__.py
 Comment: 
 
 Filename: fastl2lir/fastl2lir.py
 Comment: 
 
-Filename: fastl2lir/jax.py
+Filename: fastl2lir-0.9.dist-info/LICENSE
 Comment: 
 
-Filename: fastl2lir-0.8.dist-info/LICENSE
+Filename: fastl2lir-0.9.dist-info/METADATA
 Comment: 
 
-Filename: fastl2lir-0.8.dist-info/METADATA
+Filename: fastl2lir-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fastl2lir-0.8.dist-info/WHEEL
+Filename: fastl2lir-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fastl2lir-0.8.dist-info/top_level.txt
-Comment: 
-
-Filename: fastl2lir-0.8.dist-info/RECORD
+Filename: fastl2lir-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastl2lir/fastl2lir.py

```diff
@@ -170,27 +170,29 @@
                 with threadpool_limits(limits=1, user_api='blas'):
                     for index_outputDim in tqdm(range(Y.shape[1])):
                         C0 = abs(C[index_outputDim,:])
                         I = np.argsort(C0)
                         I = I[::-1]
                         I = I[0:n_feat]
                         I = np.hstack((I, X.shape[1]-1))
-                        Wb = np.linalg.solve(W0[I][:, I], W1[index_outputDim][I].reshape(-1,1))
+                        W0_sub = (W0.ravel()[(I + (I * W0.shape[1]).reshape((-1,1))).ravel()]).reshape(I.size, I.size)
+                        Wb = np.linalg.solve(W0_sub, W1[index_outputDim][I].reshape(-1,1))
                         for index_selectedDim in range(n_feat):
                             W[index_outputDim, I[index_selectedDim]] = Wb[index_selectedDim]
                         b[0, index_outputDim] = Wb[-1]
                     W = W.T
             else:
                 for index_outputDim in tqdm(range(Y.shape[1])):
                     C0 = abs(C[index_outputDim,:])
                     I = np.argsort(C0)
                     I = I[::-1]
                     I = I[0:n_feat]
                     I = np.hstack((I, X.shape[1]-1))
-                    Wb = np.linalg.solve(W0[I][:, I], W1[index_outputDim][I].reshape(-1,1))
+                    W0_sub = (W0.ravel()[(I + (I * W0.shape[1]).reshape((-1,1))).ravel()]).reshape(I.size, I.size)
+                    Wb = np.linalg.solve(W0_sub, W1[index_outputDim][I].reshape(-1,1))
                     for index_selectedDim in range(n_feat):
                         W[index_outputDim, I[index_selectedDim]] = Wb[index_selectedDim]
                     b[0, index_outputDim] = Wb[-1]
                 W = W.T
 
         return W, b
```

## Comparing `fastl2lir-0.8.dist-info/LICENSE` & `fastl2lir-0.9.dist-info/LICENSE`

 * *Files identical despite different names*

