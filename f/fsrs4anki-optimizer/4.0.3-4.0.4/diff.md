# Comparing `tmp/fsrs4anki_optimizer-4.0.3.tar.gz` & `tmp/fsrs4anki_optimizer-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.0.3.tar", last modified: Fri Jul 14 06:13:39 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.0.4.tar", last modified: Sun Jul 16 12:09:53 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.0.3.tar` & `fsrs4anki_optimizer-4.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50026 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50143 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 12:09:53.000000 fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:09:53.533291 fsrs4anki_optimizer-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 12:09:35.000000 fsrs4anki_optimizer-4.0.4/setup.py
```

### Comparing `fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         remembered_fallbacks["timezone"],
         remembered_fallbacks["revlog_start_date"],
         remembered_fallbacks["next_day"]
     )
     print(analysis)
 
     optimizer.define_model()
+    optimizer.pretrain()
     optimizer.train()
 
     optimizer.predict_memory_states()
     figures = optimizer.find_optimal_retention()
     if show_graphs:
         for f in figures:
             f.show()
```

### Comparing `fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.0.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,14 +400,15 @@
         df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         tqdm.write("Trainset saved.")
 
         S0_dataset = df[df['i'] == 2]
         self.S0_dataset_group = S0_dataset.groupby(by=['r_history', 'delta_t'], group_keys=False).agg({'y': ['mean', 'count']}).reset_index()
+        self.S0_dataset_group.to_csv('stability_for_pretrain.tsv', sep='\t', index=None)
 
         df['retention'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['y'].transform('mean')
         df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['id'].transform('count')
         tqdm.write("Retention calculated.")
 
         df = df.drop(columns=['id', 'cid', 'usn', 'ivl', 'last_ivl', 'factor', 'time', 'type', 'create_date', 'review_date', 'real_days', 'r', 't_history', 'y'])
         df.drop_duplicates(inplace=True)
@@ -484,15 +485,15 @@
             delta_t = group['delta_t']
             recall = group['y']['mean']
             count = group['y']['count']
             total_count = sum(count)
             if total_count < 100:
                 tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
                 continue
-            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (365)))
+            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (60 if total_count < 1000 else 365)))
             stability = params[0]
             rating_stability[int(first_rating)] = stability
             rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
             rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
             if verbose:
@@ -533,15 +534,15 @@
             plt.grid(True)
             plt.xlabel('First rating')
             plt.ylabel('Stability')
             plt.title('Stability for first rating')
             plt.show()
 
         for rating in (1, 2, 3, 4):
-            again_extrap = max(min(S0_rating_curve(1, *params), 365), 0.1)
+            again_extrap = max(min(S0_rating_curve(1, *params), 60), 0.1)
             # if there isn't enough data to calculate the value for "Again" exactly
             if 1 not in rating_stability:
                 # then check if there exists an exact value for "Hard"
                 if 2 in rating_stability:
                     # if it exists, then check whether the extrapolation breaks monotonicity
                     # Again > Hard is possible, but we should allow it only for exact values, otherwise we should assume monotonicity
                     if again_extrap > rating_stability[2]:
@@ -550,15 +551,15 @@
                     else:
                         # if it doesn't break monotonicity, then use the extrapolated value
                         rating_stability[1] = again_extrap
                 # if an exact value for "Hard" doesn't exist, then just use the extrapolation, there's nothing else we can do
                 else:
                     rating_stability[1] = again_extrap
             elif rating not in rating_stability:
-                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 365), 0.1)
+                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 60), 0.1)
 
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
         tqdm.write(f"Pretrain finished!")
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
```

