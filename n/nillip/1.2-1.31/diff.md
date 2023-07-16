# Comparing `tmp/nillip-1.2.tar.gz` & `tmp/nillip-1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nillip-1.2.tar", last modified: Fri Jul 14 05:14:31 2023, max compression
+gzip compressed data, was "dist/nillip-1.31.tar", last modified: Sun Jul 16 19:42:14 2023, max compression
```

## Comparing `nillip-1.2.tar` & `nillip-1.31.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-14 05:14:31.000000 nillip-1.2/
--rw-r--r--   0 phil       (501) staff       (20)      488 2023-07-14 05:14:31.000000 nillip-1.2/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-14 00:42:39.000000 nillip-1.2/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-14 05:14:31.000000 nillip-1.2/nillip/
--rw-r--r--   0 phil       (501) staff       (20)       19 2023-07-14 01:37:23.000000 nillip-1.2/nillip/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    41294 2023-07-14 05:05:33.000000 nillip-1.2/nillip/nil.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      488 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      229 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/not-zip-safe
--rw-r--r--   0 phil       (501) staff       (20)       15 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-14 05:14:31.000000 nillip-1.2/nillip.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-14 05:14:31.000000 nillip-1.2/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     2534 2023-07-14 05:08:13.000000 nillip-1.2/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/
+-rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 19:42:14.000000 nillip-1.31/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-14 00:42:39.000000 nillip-1.31/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/nillip/
+-rw-r--r--   0 phil       (501) staff       (20)       19 2023-07-15 01:09:26.000000 nillip-1.31/nillip/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    40513 2023-07-16 19:38:48.000000 nillip-1.31/nillip/nil.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      229 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-14 05:14:31.000000 nillip-1.31/nillip.egg-info/not-zip-safe
+-rw-r--r--   0 phil       (501) staff       (20)      134 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-16 19:42:14.000000 nillip-1.31/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1646 2023-07-16 19:42:01.000000 nillip-1.31/setup.py
```

### Comparing `nillip-1.2/nillip/nil.py` & `nillip-1.31/nillip/nil.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,31 +101,14 @@
 
 
 def zorder(ax, zorder):
     plt.setp(ax.lines, zorder=zorder)
     plt.setp(ax.collections, zorder=zorder)
 
 
-def NANify_data(tvt_x, tvt_y, tvt_fn, numpy_seed=42):
-    nan_array_border_inds = load_nan_border_index()
-    tvt_x_naned = []
-    for data in tqdm(tvt_x):
-        data = copy.deepcopy(data)
-        np.random.seed(numpy_seed)
-        inds = np.random.choice(nan_array_border_inds.shape[0], data.shape[0])
-        replace_with_nans = nan_array_border_inds[inds]
-        data[replace_with_nans] = np.nan
-        tvt_x_naned.append(data)
-    del data
-
-    for i, nan_data in enumerate(tqdm(tvt_x_naned)):
-        tvt_x[i] = np.vstack([tvt_x[i], tvt_x_naned[i]])
-        tvt_y[i] = np.concatenate([tvt_y[i], tvt_y[i]])
-        tvt_fn[i] = np.concatenate([tvt_fn[i], tvt_fn[i]])
-    return tvt_x, tvt_y, tvt_fn
 
 
 def quick_spliter(split_nums, len_array):
     l_nums = np.sum(split_nums)
     count = 1 + (len_array // l_nums)
 
     inds = np.ones(l_nums)
@@ -1160,15 +1143,15 @@
                 a = ((a + 255) / 2).astype(np.uint8)
                 h['images'][i, :, :, img_i] = a
 
 
 
 
     # copy over the other info from the OG h5 file
-    copy_over_all_non_image_keys(f, f2)
+    # copy_over_all_non_image_keys(f, f2)
     # copy_h5_key_to_another_h5(f, f2, 'labels', 'labels')
     # copy_h5_key_to_another_h5(f, f2, 'frame_nums', 'frame_nums')
 
 
 def force_write_to_h5(h5_file, data, data_name):
     with h5py.File(h5_file, 'r+') as h:
         try:
@@ -1203,16 +1186,15 @@
     #     shutil.rmtree(dst)
     #     print('waiting 10 seconds to allow model to delete')
     # time.sleep(10)
 
     x = '''python3 "/Users/phil/Dropbox/UPDATE_nillip_PYPI.py"'''
     out = os.popen(x).read()
     print(out)
-    # print(
-    #     'please refer to the open terminal window for further details\nrerun utils.download_resnet_model() to put the model file back')
+    print('please refer to the open terminal window for further details')
 
 
 def make_list(x, suppress_warning=False):
     if not isinstance(x, list):
         if not suppress_warning:
             print("""input is supposed to be a list, converting it but user should do this to suppress this warning""")
         if type(x) is np.str_:
```

