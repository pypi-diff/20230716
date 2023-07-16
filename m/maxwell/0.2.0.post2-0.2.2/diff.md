# Comparing `tmp/maxwell-0.2.0.post2.tar.gz` & `tmp/maxwell-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maxwell-0.2.0.post2.tar", last modified: Wed Nov  2 19:31:45 2022, max compression
+gzip compressed data, was "maxwell-0.2.2.tar", last modified: Sun Jul 16 18:53:35 2023, max compression
```

## Comparing `maxwell-0.2.0.post2.tar` & `maxwell-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2022-11-02 19:31:45.225091 maxwell-0.2.0.post2/
--rw-rw-r--   0 travis    (1000) travis    (1000)    10802 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/LICENSE.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     6353 2022-11-02 19:31:45.225091 maxwell-0.2.0.post2/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     4483 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/README.md
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2022-11-02 19:31:45.225091 maxwell-0.2.0.post2/maxwell/
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/maxwell/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3313 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/maxwell/actions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    19071 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/maxwell/sed.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2407 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/maxwell/train.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      279 2022-11-02 19:20:55.000000 maxwell-0.2.0.post2/maxwell/util.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2022-11-02 19:31:45.225091 maxwell-0.2.0.post2/maxwell.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     6353 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)      305 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       54 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       51 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        8 2022-11-02 19:31:45.000000 maxwell-0.2.0.post2/maxwell.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       38 2022-11-02 19:31:45.225091 maxwell-0.2.0.post2/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)     1971 2022-11-02 19:27:48.000000 maxwell-0.2.0.post2/setup.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-07-16 18:53:35.644069 maxwell-0.2.2/
+-rw-r--r--   0 kbg        (501) staff       (20)    10802 2023-07-16 18:53:16.000000 maxwell-0.2.2/LICENSE.txt
+-rw-r--r--   0 kbg        (501) staff       (20)     5173 2023-07-16 18:53:35.643954 maxwell-0.2.2/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)     4464 2023-07-16 18:53:16.000000 maxwell-0.2.2/README.md
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-07-16 18:53:35.643132 maxwell-0.2.2/maxwell/
+-rw-r--r--   0 kbg        (501) staff       (20)        0 2023-07-16 18:53:16.000000 maxwell-0.2.2/maxwell/__init__.py
+-rw-r--r--   0 kbg        (501) staff       (20)     3313 2023-07-16 18:53:16.000000 maxwell-0.2.2/maxwell/actions.py
+-rw-r--r--   0 kbg        (501) staff       (20)    19178 2023-07-16 18:53:16.000000 maxwell-0.2.2/maxwell/sed.py
+-rw-r--r--   0 kbg        (501) staff       (20)     2090 2023-07-16 18:53:16.000000 maxwell-0.2.2/maxwell/train.py
+-rw-r--r--   0 kbg        (501) staff       (20)      279 2023-07-16 18:53:16.000000 maxwell-0.2.2/maxwell/util.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-07-16 18:53:35.643791 maxwell-0.2.2/maxwell.egg-info/
+-rw-r--r--   0 kbg        (501) staff       (20)     5173 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)      305 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/SOURCES.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        1 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/dependency_links.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       53 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/entry_points.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       38 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/requires.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        8 2023-07-16 18:53:35.000000 maxwell-0.2.2/maxwell.egg-info/top_level.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       38 2023-07-16 18:53:35.644108 maxwell-0.2.2/setup.cfg
+-rw-r--r--   0 kbg        (501) staff       (20)     1913 2023-07-16 18:53:16.000000 maxwell-0.2.2/setup.py
```

### Comparing `maxwell-0.2.0.post2/LICENSE.txt` & `maxwell-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maxwell-0.2.0.post2/PKG-INFO` & `maxwell-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,159 +1,158 @@
 Metadata-Version: 2.1
 Name: maxwell
-Version: 0.2.0.post2
+Version: 0.2.2
 Summary: Stochastic Edit Distance aligner for string transduction
-Home-page: UNKNOWN
-Author: Simon Clematide, Peter Makarov,
-                    Travis M. Bartley
+Author: Simon Clematide, Peter Makarov, Travis M. Bartley
 License: Apache 2.0
-Description: # Maxwell 👹
-        
-        [![PyPI
-        version](https://badge.fury.io/py/Maxwell.svg)](https://pypi.org/project/maxwell/)
-        [![Supported Python
-        versions](https://img.shields.io/pypi/pyversions/maxwell.svg)](https://pypi.org/project/maxwell/)
-        [![CircleCI](https://circleci.com/gh/CUNY-CL/maxwell.svg?style=svg&circle-token=43c60045a43c2b4d4e2ad95dce2968512e7fe8d6)](https://app.circleci.com/pipelines/github/CUNY-CL/maxwell?branch=main)
-        
-        Maxwell is a Python library for learning the stochastic edit distance (SED)
-        between source and target alphabets for string transduction.
-        
-        Given a corpus of source and target string pairs, it uses
-        expectation-maximization to learn the log-probability weights of edit actions
-        (copy, substitution, deletion, insertion) that minimize the number of edits
-        between source and target strings. These weights can then be used for edits over
-        unknown strings through Viterbi decoding.
-        
-        ## Install
-        
-        First install dependencies:
-        
-            pip install -r requirements.txt
-        
-        Then install:
-        
-            python setup.py install
-        
-        Or:
-        
-            python setup.py develop
-        
-        The latter creates a Python module in your environment that updates as you
-        update the code. It can then be imported like a regular Python module:
-        
-        ```python
-        import maxwell
-        ```
-        
-        ## Usage
-        
-        SED training can be done as either a command line tool or imported as a Python
-        dependency.
-        
-        For command-line use, run:
-        
-            maxwell-train \
-                --train-data-path /path/to/train/data \
-                --output-path /path/to/output/file \
-                --num-epoch "${NUM_EPOCHS}"
-        
-        As a library object, you can use the `StochasticEditDistance` class to pass any
-        iterable of source-target pairs for training. Learned edit weights can then be
-        saved with the `write_params` method:
-        
-        ```python
-        from maxwell import sed
-        
-        
-        aligner = sed.StochasticEditDistance.fit_from_data(
-            training_samples, NUM_EPOCHS
-        )
-        aligner.params.write_params("/path/to/output/file")
-        ```
-        
-        After training, parameters can be loaded from file to calculate optimal edits
-        between strings with the `action_sequence` method, which returns a tuple of the
-        learned optimal sequence and the weight given to the sequence:
-        
-        ```python
-        from maxwell import sed
-        
-        
-        params = sed.ParamsDict.read_params("/path/to/learned/parameters/")
-        aligner = sed.StochasticEditDistance(params)
-        optimal_sequence, optimal_cost = aligner.action_sequence(source, target)
-        ```
-        
-        If only weight and no actions are required, `action_sequence_cost` can be called
-        instead:
-        
-        ```python
-        optimal_cost = aligner.action_sequence_cost(source, target)
-        ```
-        
-        Conversely, individual actions can be evaluated with the `action_cost` method:
-        
-        ```python
-        action_cost = aligner.action_cost(action)
-        ```
-        
-        ## Details
-        
-        ### Data
-        
-        The default data format is based on the SIGMORPHON 2017 shared tasks:
-        
-            source   target    ...
-        
-        That is, the first column is the source (a lemma) and the second is the target.
-        
-        In the case where the formatting is different, the `--source-col` and
-        `--target-col` flags can be invoked. For instance, for the SIGMORPHON 2016
-        shared task data format:
-        
-            source   ...    target
-        
-        one would instead use the flag `--target-col 3` to use the third column as
-        target strings (note the use of 1-based indexing).
-        
-        ### Edit actions
-        
-        Edit weights are maintained as a `ParamsDict` object, a dataclass comprising
-        three dictionaries and one floats. The dictionaries, and their indexing, are as
-        follows:
-        
-        1.  `delta_sub` Keys: Tuple of source alphabet X target alphabet. Values:
-            Substitution weight for all non-equivalent source-target pairs. If source
-            symbol == target symbol, a seperate copy probability is used.
-        2.  `delta_del` Keys: All symbols in source string alphabet. Represents deletion
-            from string. Values: Deletion weight for removal of source symbol from
-            string.
-        3.  `delta_ins` Keys: All symbols in target string alphabet. Represents
-            insertion into string. Values: Insertion weight for introduction of target
-            symbol into string.
-        4.  `delta_eos` A float value representing probability of terminating the
-            string.
-        
-        In Python, these values may be accessed through a `StochasticEditDistance`
-        object's `params` attribute.
-        
-        ## Further reading
-        
-        For further reading, please see:
-        
-        Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
-        data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
-        30(1): 1-38.
-        
-        Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
-        Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
 Keywords: computational linguistics,morphology,natural language processing,language
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Maxwell 👹
+
+[![PyPI
+version](https://badge.fury.io/py/Maxwell.svg)](https://pypi.org/project/maxwell/)
+[![Supported Python
+versions](https://img.shields.io/pypi/pyversions/maxwell.svg)](https://pypi.org/project/maxwell/)
+[![CircleCI](https://circleci.com/gh/CUNY-CL/maxwell.svg?style=svg&circle-token=43c60045a43c2b4d4e2ad95dce2968512e7fe8d6)](https://app.circleci.com/pipelines/github/CUNY-CL/maxwell?branch=main)
+
+Maxwell is a Python library for learning the stochastic edit distance (SED)
+between source and target alphabets for string transduction.
+
+Given a corpus of source and target string pairs, it uses
+expectation-maximization to learn the log-probability weights of edit actions
+(copy, substitution, deletion, insertion) that minimize the number of edits
+between source and target strings. These weights can then be used for edits over
+unknown strings through Viterbi decoding.
+
+## Install
+
+First install dependencies:
+
+    pip install -r requirements.txt
+
+Then install:
+
+    python setup.py install
+
+Or:
+
+    python setup.py develop
+
+The latter creates a Python module in your environment that updates as you
+update the code. It can then be imported like a regular Python module:
+
+```python
+import maxwell
+```
+
+## Usage
+
+SED training can be done as either a command line tool or imported as a Python
+dependency.
+
+For command-line use, run:
+
+    maxwell-train \
+        --train /path/to/train/data \
+        --output /path/to/output/file \
+        --epochs "${NUM_EPOCHS}"
+
+As a library object, you can use the `StochasticEditDistance` class to pass any
+iterable of source-target pairs for training. Learned edit weights can then be
+saved with the `write_params` method:
+
+```python
+from maxwell import sed
+
+
+aligner = sed.StochasticEditDistance.fit_from_data(
+    training_samples, NUM_EPOCHS
+)
+aligner.params.write_params("/path/to/output/file")
+```
+
+After training, parameters can be loaded from file to calculate optimal edits
+between strings with the `action_sequence` method, which returns a tuple of the
+learned optimal sequence and the weight given to the sequence:
+
+```python
+from maxwell import sed
+
+
+params = sed.ParamsDict.read_params("/path/to/learned/parameters")
+aligner = sed.StochasticEditDistance(params)
+optimal_sequence, optimal_cost = aligner.action_sequence(source, target)
+```
+
+If only weight and no actions are required, `action_sequence_cost` can be called
+instead:
+
+```python
+optimal_cost = aligner.action_sequence_cost(source, target)
+```
+
+Conversely, individual actions can be evaluated with the `action_cost` method:
+
+```python
+action_cost = aligner.action_cost(action)
+```
+
+## Details
+
+### Data
+
+The default data format is based on the SIGMORPHON 2017 shared tasks:
+
+    source   target    ...
+
+That is, the first column is the source (a lemma) and the second is the target.
+
+In the case where the formatting is different, the `--source-col` and
+`--target-col` flags can be invoked. For instance, for the SIGMORPHON 2016
+shared task data format:
+
+    source   ...    target
+
+one would instead use the flag `--target-col 3` to use the third column as
+target strings (note the use of 1-based indexing).
+
+### Edit actions
+
+Edit weights are maintained as a `ParamsDict` object, a dataclass comprising
+three dictionaries and one floats. The dictionaries, and their indexing, are as
+follows:
+
+1.  `delta_sub` Keys: Tuple of source alphabet X target alphabet. Values:
+    Substitution weight for all non-equivalent source-target pairs. If source
+    symbol == target symbol, a seperate copy probability is used.
+2.  `delta_del` Keys: All symbols in source string alphabet. Represents deletion
+    from string. Values: Deletion weight for removal of source symbol from
+    string.
+3.  `delta_ins` Keys: All symbols in target string alphabet. Represents
+    insertion into string. Values: Insertion weight for introduction of target
+    symbol into string.
+4.  `delta_eos` A float value representing probability of terminating the
+    string.
+
+In Python, these values may be accessed through a `StochasticEditDistance`
+object's `params` attribute.
+
+## Further reading
+
+For further reading, please see:
+
+Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
+data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
+30(1): 1-38.
+
+Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
+Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
```

### Comparing `maxwell-0.2.0.post2/README.md` & `maxwell-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 
 SED training can be done as either a command line tool or imported as a Python
 dependency.
 
 For command-line use, run:
 
     maxwell-train \
-        --train-data-path /path/to/train/data \
-        --output-path /path/to/output/file \
-        --num-epoch "${NUM_EPOCHS}"
+        --train /path/to/train/data \
+        --output /path/to/output/file \
+        --epochs "${NUM_EPOCHS}"
 
 As a library object, you can use the `StochasticEditDistance` class to pass any
 iterable of source-target pairs for training. Learned edit weights can then be
 saved with the `write_params` method:
 
 ```python
 from maxwell import sed
@@ -66,15 +66,15 @@
 between strings with the `action_sequence` method, which returns a tuple of the
 learned optimal sequence and the weight given to the sequence:
 
 ```python
 from maxwell import sed
 
 
-params = sed.ParamsDict.read_params("/path/to/learned/parameters/")
+params = sed.ParamsDict.read_params("/path/to/learned/parameters")
 aligner = sed.StochasticEditDistance(params)
 optimal_sequence, optimal_cost = aligner.action_sequence(source, target)
 ```
 
 If only weight and no actions are required, `action_sequence_cost` can be called
 instead:
```

### Comparing `maxwell-0.2.0.post2/maxwell/actions.py` & `maxwell-0.2.2/maxwell/actions.py`

 * *Files identical despite different names*

### Comparing `maxwell-0.2.0.post2/maxwell/sed.py` & `maxwell-0.2.2/maxwell/sed.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import abc
 import dataclasses
 import pickle
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple
 
 import numpy
 import tqdm
+
 from scipy import special
 
 from . import actions, util
 
 LARGE_NEG_CONST = -1e6
 
 
@@ -296,39 +297,40 @@
 
     def log_likelihood(
         self,
         sources: Iterable[Sequence[Any]],
         targets: Iterable[Sequence[Any]],
     ) -> float:
         """Computes log likelihood."""
-        ll = numpy.mean(
-            [
-                self.forward_evaluate(source, target)[-1, -1]
-                for source, target in zip(sources, targets)
-            ]
-        )
-        return float(ll)
+        with tqdm.tqdm(
+            zip(sources, targets), total=len(sources), leave=False
+        ) as pbar:
+            ll = []
+            pbar.set_description("Calculating log-likelihood")
+            for source, target in pbar:
+                ll.append(self.forward_evaluate(source, target)[-1, -1])
+        return float(numpy.mean(ll))
 
     def em(
         self,
         sources: Sequence[Any],
         targets: Sequence[Any],
         epochs: int = 10,
     ) -> None:
         """Update parameters using expectation-maximization.
 
         Args:
             sources (Sequence[Any]): source strings.
             targets (Sequence[Any]): target strings.
             epochs (int): number of EM epochs.
         """
-        loglike = self.log_likelihood(sources, targets)
+        loglike = numpy.NINF
         gammas = ParamDict.from_params(self.params)
-        for epoch in range(epochs):
-            with tqdm.tqdm(zip(sources, targets), total=len(sources)) as pbar:
+        with tqdm.tqdm(zip(sources, targets), total=len(sources)) as pbar:
+            for epoch in range(epochs):
                 pbar.set_description(f"Epoch {epoch}")
                 pbar.set_postfix(loglike=loglike)
                 for source, target in pbar:
                     self.e_step(source, target, gammas)  # Updates gammas.
                 self.m_step(gammas)  # Updates gammas.
                 self.params.update_params(gammas)  # Updates model parameters.
                 loglike = self.log_likelihood(sources, targets)
```

### Comparing `maxwell-0.2.0.post2/maxwell.egg-info/PKG-INFO` & `maxwell-0.2.2/maxwell.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,159 +1,158 @@
 Metadata-Version: 2.1
 Name: maxwell
-Version: 0.2.0.post2
+Version: 0.2.2
 Summary: Stochastic Edit Distance aligner for string transduction
-Home-page: UNKNOWN
-Author: Simon Clematide, Peter Makarov,
-                    Travis M. Bartley
+Author: Simon Clematide, Peter Makarov, Travis M. Bartley
 License: Apache 2.0
-Description: # Maxwell 👹
-        
-        [![PyPI
-        version](https://badge.fury.io/py/Maxwell.svg)](https://pypi.org/project/maxwell/)
-        [![Supported Python
-        versions](https://img.shields.io/pypi/pyversions/maxwell.svg)](https://pypi.org/project/maxwell/)
-        [![CircleCI](https://circleci.com/gh/CUNY-CL/maxwell.svg?style=svg&circle-token=43c60045a43c2b4d4e2ad95dce2968512e7fe8d6)](https://app.circleci.com/pipelines/github/CUNY-CL/maxwell?branch=main)
-        
-        Maxwell is a Python library for learning the stochastic edit distance (SED)
-        between source and target alphabets for string transduction.
-        
-        Given a corpus of source and target string pairs, it uses
-        expectation-maximization to learn the log-probability weights of edit actions
-        (copy, substitution, deletion, insertion) that minimize the number of edits
-        between source and target strings. These weights can then be used for edits over
-        unknown strings through Viterbi decoding.
-        
-        ## Install
-        
-        First install dependencies:
-        
-            pip install -r requirements.txt
-        
-        Then install:
-        
-            python setup.py install
-        
-        Or:
-        
-            python setup.py develop
-        
-        The latter creates a Python module in your environment that updates as you
-        update the code. It can then be imported like a regular Python module:
-        
-        ```python
-        import maxwell
-        ```
-        
-        ## Usage
-        
-        SED training can be done as either a command line tool or imported as a Python
-        dependency.
-        
-        For command-line use, run:
-        
-            maxwell-train \
-                --train-data-path /path/to/train/data \
-                --output-path /path/to/output/file \
-                --num-epoch "${NUM_EPOCHS}"
-        
-        As a library object, you can use the `StochasticEditDistance` class to pass any
-        iterable of source-target pairs for training. Learned edit weights can then be
-        saved with the `write_params` method:
-        
-        ```python
-        from maxwell import sed
-        
-        
-        aligner = sed.StochasticEditDistance.fit_from_data(
-            training_samples, NUM_EPOCHS
-        )
-        aligner.params.write_params("/path/to/output/file")
-        ```
-        
-        After training, parameters can be loaded from file to calculate optimal edits
-        between strings with the `action_sequence` method, which returns a tuple of the
-        learned optimal sequence and the weight given to the sequence:
-        
-        ```python
-        from maxwell import sed
-        
-        
-        params = sed.ParamsDict.read_params("/path/to/learned/parameters/")
-        aligner = sed.StochasticEditDistance(params)
-        optimal_sequence, optimal_cost = aligner.action_sequence(source, target)
-        ```
-        
-        If only weight and no actions are required, `action_sequence_cost` can be called
-        instead:
-        
-        ```python
-        optimal_cost = aligner.action_sequence_cost(source, target)
-        ```
-        
-        Conversely, individual actions can be evaluated with the `action_cost` method:
-        
-        ```python
-        action_cost = aligner.action_cost(action)
-        ```
-        
-        ## Details
-        
-        ### Data
-        
-        The default data format is based on the SIGMORPHON 2017 shared tasks:
-        
-            source   target    ...
-        
-        That is, the first column is the source (a lemma) and the second is the target.
-        
-        In the case where the formatting is different, the `--source-col` and
-        `--target-col` flags can be invoked. For instance, for the SIGMORPHON 2016
-        shared task data format:
-        
-            source   ...    target
-        
-        one would instead use the flag `--target-col 3` to use the third column as
-        target strings (note the use of 1-based indexing).
-        
-        ### Edit actions
-        
-        Edit weights are maintained as a `ParamsDict` object, a dataclass comprising
-        three dictionaries and one floats. The dictionaries, and their indexing, are as
-        follows:
-        
-        1.  `delta_sub` Keys: Tuple of source alphabet X target alphabet. Values:
-            Substitution weight for all non-equivalent source-target pairs. If source
-            symbol == target symbol, a seperate copy probability is used.
-        2.  `delta_del` Keys: All symbols in source string alphabet. Represents deletion
-            from string. Values: Deletion weight for removal of source symbol from
-            string.
-        3.  `delta_ins` Keys: All symbols in target string alphabet. Represents
-            insertion into string. Values: Insertion weight for introduction of target
-            symbol into string.
-        4.  `delta_eos` A float value representing probability of terminating the
-            string.
-        
-        In Python, these values may be accessed through a `StochasticEditDistance`
-        object's `params` attribute.
-        
-        ## Further reading
-        
-        For further reading, please see:
-        
-        Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
-        data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
-        30(1): 1-38.
-        
-        Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
-        Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
 Keywords: computational linguistics,morphology,natural language processing,language
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Maxwell 👹
+
+[![PyPI
+version](https://badge.fury.io/py/Maxwell.svg)](https://pypi.org/project/maxwell/)
+[![Supported Python
+versions](https://img.shields.io/pypi/pyversions/maxwell.svg)](https://pypi.org/project/maxwell/)
+[![CircleCI](https://circleci.com/gh/CUNY-CL/maxwell.svg?style=svg&circle-token=43c60045a43c2b4d4e2ad95dce2968512e7fe8d6)](https://app.circleci.com/pipelines/github/CUNY-CL/maxwell?branch=main)
+
+Maxwell is a Python library for learning the stochastic edit distance (SED)
+between source and target alphabets for string transduction.
+
+Given a corpus of source and target string pairs, it uses
+expectation-maximization to learn the log-probability weights of edit actions
+(copy, substitution, deletion, insertion) that minimize the number of edits
+between source and target strings. These weights can then be used for edits over
+unknown strings through Viterbi decoding.
+
+## Install
+
+First install dependencies:
+
+    pip install -r requirements.txt
+
+Then install:
+
+    python setup.py install
+
+Or:
+
+    python setup.py develop
+
+The latter creates a Python module in your environment that updates as you
+update the code. It can then be imported like a regular Python module:
+
+```python
+import maxwell
+```
+
+## Usage
+
+SED training can be done as either a command line tool or imported as a Python
+dependency.
+
+For command-line use, run:
+
+    maxwell-train \
+        --train /path/to/train/data \
+        --output /path/to/output/file \
+        --epochs "${NUM_EPOCHS}"
+
+As a library object, you can use the `StochasticEditDistance` class to pass any
+iterable of source-target pairs for training. Learned edit weights can then be
+saved with the `write_params` method:
+
+```python
+from maxwell import sed
+
+
+aligner = sed.StochasticEditDistance.fit_from_data(
+    training_samples, NUM_EPOCHS
+)
+aligner.params.write_params("/path/to/output/file")
+```
+
+After training, parameters can be loaded from file to calculate optimal edits
+between strings with the `action_sequence` method, which returns a tuple of the
+learned optimal sequence and the weight given to the sequence:
+
+```python
+from maxwell import sed
+
+
+params = sed.ParamsDict.read_params("/path/to/learned/parameters")
+aligner = sed.StochasticEditDistance(params)
+optimal_sequence, optimal_cost = aligner.action_sequence(source, target)
+```
+
+If only weight and no actions are required, `action_sequence_cost` can be called
+instead:
+
+```python
+optimal_cost = aligner.action_sequence_cost(source, target)
+```
+
+Conversely, individual actions can be evaluated with the `action_cost` method:
+
+```python
+action_cost = aligner.action_cost(action)
+```
+
+## Details
+
+### Data
+
+The default data format is based on the SIGMORPHON 2017 shared tasks:
+
+    source   target    ...
+
+That is, the first column is the source (a lemma) and the second is the target.
+
+In the case where the formatting is different, the `--source-col` and
+`--target-col` flags can be invoked. For instance, for the SIGMORPHON 2016
+shared task data format:
+
+    source   ...    target
+
+one would instead use the flag `--target-col 3` to use the third column as
+target strings (note the use of 1-based indexing).
+
+### Edit actions
+
+Edit weights are maintained as a `ParamsDict` object, a dataclass comprising
+three dictionaries and one floats. The dictionaries, and their indexing, are as
+follows:
+
+1.  `delta_sub` Keys: Tuple of source alphabet X target alphabet. Values:
+    Substitution weight for all non-equivalent source-target pairs. If source
+    symbol == target symbol, a seperate copy probability is used.
+2.  `delta_del` Keys: All symbols in source string alphabet. Represents deletion
+    from string. Values: Deletion weight for removal of source symbol from
+    string.
+3.  `delta_ins` Keys: All symbols in target string alphabet. Represents
+    insertion into string. Values: Insertion weight for introduction of target
+    symbol into string.
+4.  `delta_eos` A float value representing probability of terminating the
+    string.
+
+In Python, these values may be accessed through a `StochasticEditDistance`
+object's `params` attribute.
+
+## Further reading
+
+For further reading, please see:
+
+Dempster, A., Laird, N., and Rubin, D. 1977. Maximum likelihood from incomplete
+data via the EM algorithm. *Journal of the Royal Statistical Society, Series B*
+30(1): 1-38.
+
+Ristad, E. S. and Yianilos, P. N. 1998. Learning string-edit distance. *IEEE
+Transactions on Pattern Analysis and Machine Intelligence* 20(5): 522-532.
```

### Comparing `maxwell-0.2.0.post2/setup.py` & `maxwell-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 _THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 
 
 with open(os.path.join(_THIS_DIR, "README.md")) as f:
     _LONG_DESCRIPTION = f.read().strip()
 
 
-__version__ = "0.2.0.post2"
+__version__ = "0.2.2"
 
 
 def main() -> None:
     setuptools.setup(
         name="maxwell",
         version=__version__,
         description="Stochastic Edit Distance aligner for string transduction",
         long_description=_LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
-        author="""Simon Clematide, Peter Makarov,
-                    Travis M. Bartley""",
+        author="Simon Clematide, Peter Makarov, Travis M. Bartley",
         keywords=[
             "computational linguistics",
             "morphology",
             "natural language processing",
             "language",
         ],
         classifiers=[
@@ -44,15 +43,14 @@
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
             "Topic :: Text Processing :: Linguistic",
         ],
         license="Apache 2.0",
         python_requires=">=3.9",
         install_requires=[
-            "click>=8.1.3",
             "numpy>=1.20.1",
             "scipy>=1.6",
             "tqdm>=4.64.1",
         ],
         packages=setuptools.find_packages(exclude=["maxwell.tests"]),
         entry_points={
             "console_scripts": [
```

