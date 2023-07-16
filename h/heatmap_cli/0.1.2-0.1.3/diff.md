# Comparing `tmp/heatmap_cli-0.1.2.tar.gz` & `tmp/heatmap_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.1.2.tar` & `heatmap_cli-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      143 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.gitignore
--rw-r--r--   0        0        0     2411 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/.python-version
--rw-r--r--   0        0        0      712 2023-07-10 16:30:45.947135 heatmap_cli-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2002 2023-07-10 15:30:51.824917 heatmap_cli-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      489 2023-07-10 15:32:42.498460 heatmap_cli-0.1.2/Pipfile
--rw-r--r--   0        0        0   100071 2023-07-10 15:28:50.451408 heatmap_cli-0.1.2/Pipfile.lock
--rw-r--r--   0        0        0     1927 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/README.md
--rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.1.2/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-10 16:31:31.987887 heatmap_cli-0.1.2/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     5395 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1077 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      303 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tests/test_version_flag.py
--rw-r--r--   0        0        0      673 2023-07-10 15:24:28.649268 heatmap_cli-0.1.2/tox.ini
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 heatmap_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/.gitignore
+-rw-r--r--   0        0        0     2465 2023-07-12 17:30:43.846915 heatmap_cli-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/.python-version
+-rw-r--r--   0        0        0      861 2023-07-16 01:33:45.437513 heatmap_cli-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2002 2023-07-14 00:05:31.556357 heatmap_cli-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      502 2023-07-11 18:27:30.048786 heatmap_cli-0.1.3/Pipfile
+-rw-r--r--   0        0        0   112832 2023-07-14 00:02:43.363808 heatmap_cli-0.1.3/Pipfile.lock
+-rw-r--r--   0        0        0     1927 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-07-16 01:34:05.737145 heatmap_cli-0.1.3/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     5395 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      303 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tests/test_version_flag.py
+-rw-r--r--   0        0        0      673 2023-07-10 15:24:28.649268 heatmap_cli-0.1.3/tox.ini
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 heatmap_cli-0.1.3/PKG-INFO
```

### Comparing `heatmap_cli-0.1.2/.gitignore` & `heatmap_cli-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/.pre-commit-config.yaml` & `heatmap_cli-0.1.3/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
       - id: validate-pyproject
         name: validate-pyproject
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
       - id: codespell
+        args:
+          - --ignore-words-list=astroid
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0
     hooks:
       - id: prettier
 
   - repo: https://github.com/pycqa/isort
```

### Comparing `heatmap_cli-0.1.2/CHANGELOG.md` & `heatmap_cli-0.1.3/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.1.3 (2023-07-16)
+
+### Fixed
+
+- Fix missing `pylint` dependency when running `pre-commit`
+- Ignore word when running codespell pre-commit hook
+
 ## v0.1.2 (2023-07-11)
 
 ### Changed
 
 - Link to license from contributing doc
 - Use the same output folder for sphinx doc generation
 - Revise `pyenv` installation with plugins in contributing doc
```

### Comparing `heatmap_cli-0.1.2/CONTRIBUTING.md` & `heatmap_cli-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/LICENSE.md` & `heatmap_cli-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/Pipfile.lock` & `heatmap_cli-0.1.3/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9670524691358025%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ed8ff138dfd0bd29c1c47d73779ecdf62e73179a3358a78ba95d6e5b5c266bcf'}}",*

 * * "'default'": "{'fonttools': {'hashes': "*

 * *              "['sha256:0614b6348866092d00df3dfb37e037fc06412ca67087de361a2777ea5ed62c16', "*

 * *              "'sha256:06eac087ea55b3ebb2207d93b5ac56c847163899f05f5a77e1910f688fe10030', "*

 * *              "'sha256:19d461c801b8904d201c6c38a99bfcfef673bfdfe0c7f026f582ef78896434e0', "*

 * *              "'sha256:381558eafffc1432d08ca58063e71c7376ecaae48e9318354a9 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "635ce0c287e6f94d9a88fb77f2ebeeb34743e7f7b9aedf2ef1a8b76b66a7b2e7"
+            "sha256": "ed8ff138dfd0bd29c1c47d73779ecdf62e73179a3358a78ba95d6e5b5c266bcf"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.8"
         },
         "sources": [
             {
@@ -67,51 +67,51 @@
                 "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.11.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:00ab569b2a3e591e00425023ade87e8fef90380c1dde61be7691cb524ca5f743",
-                "sha256:022c4a16b412293e7f1ce21b8bab7a6f9d12c4ffdf171fdc67122baddb973069",
-                "sha256:05171f3c546f64d78569f10adc0de72561882352cac39ec7439af12304d8d8c0",
-                "sha256:14037c31138fbd21847ad5e5441dfdde003e0a8f3feb5812a1a21fd1c255ffbd",
-                "sha256:15abb3d055c1b2dff9ce376b6c3db10777cb74b37b52b78f61657634fd348a0d",
-                "sha256:18ea64ac43e94c9e0c23d7a9475f1026be0e25b10dda8f236fc956188761df97",
-                "sha256:1a003608400dd1cca3e089e8c94973c6b51a4fb1ef00ff6d7641617b9242e637",
-                "sha256:1bc4c5b147be8dbc5df9cc8ac5e93ee914ad030fe2a201cc8f02f499db71011d",
-                "sha256:200729d12461e2038700d31f0d49ad5a7b55855dec7525074979a06b46f88505",
-                "sha256:337b6e83d7ee73c40ea62407f2ce03b07c3459e213b6f332b94a69923b9e1cb9",
-                "sha256:37467cee0f32cada2ec08bc16c9c31f9b53ea54b2f5604bf25a1246b5f50593a",
-                "sha256:425b74a608427499b0e45e433c34ddc350820b6f25b7c8761963a08145157a66",
-                "sha256:530c5d35109f3e0cea2535742d6a3bc99c0786cf0cbd7bb2dc9212387f0d908c",
-                "sha256:56d4d85f5374b45b08d2f928517d1e313ea71b4847240398decd0ab3ebbca885",
-                "sha256:5e00334c66f4e83535384cb5339526d01d02d77f142c23b2f97bd6a4f585497a",
-                "sha256:5fdf60f8a5c6bcce7d024a33f7e4bc7921f5b74e8ea13bccd204f2c8b86f3470",
-                "sha256:6a8d71b9a5c884c72741868e845c0e563c5d83dcaf10bb0ceeec3b4b2eb14c67",
-                "sha256:6d5adf4ba114f028fc3f5317a221fd8b0f4ef7a2e5524a2b1e0fd891b093791a",
-                "sha256:7449e5e306f3a930a8944c85d0cbc8429cba13503372a1a40f23124d6fb09b58",
-                "sha256:7961575221e3da0841c75da53833272c520000d76f7f71274dbf43370f8a1065",
-                "sha256:7f6e3fa3da923063c286320e728ba2270e49c73386e3a711aa680f4b0747d692",
-                "sha256:882983279bf39afe4e945109772c2ffad2be2c90983d6559af8b75c19845a80a",
-                "sha256:8a917828dbfdb1cbe50cf40eeae6fbf9c41aef9e535649ed8f4982b2ef65c091",
-                "sha256:8c4305b171b61040b1ee75d18f9baafe58bd3b798d1670078efe2c92436bfb63",
-                "sha256:91784e21a1a085fac07c6a407564f4a77feb471b5954c9ee55a4f9165151f6c1",
-                "sha256:94c915f6716589f78bc00fbc14c5b8de65cfd11ee335d32504f1ef234524cb24",
-                "sha256:97d95b8301b62bdece1af943b88bcb3680fd385f88346a4a899ee145913b414a",
-                "sha256:a954b90d1473c85a22ecf305761d9fd89da93bbd31dae86e7dea436ad2cb5dc9",
-                "sha256:aa83b3f151bc63970f39b2b42a06097c5a22fd7ed9f7ba008e618de4503d3895",
-                "sha256:b802dcbf9bcff74672f292b2466f6589ab8736ce4dcf36f48eb994c2847c4b30",
-                "sha256:bae8c13abbc2511e9a855d2142c0ab01178dd66b1a665798f357da0d06253e0d",
-                "sha256:c55f1b4109dbc3aeb496677b3e636d55ef46dc078c2a5e3f3db4e90f1c6d2907",
-                "sha256:eb52c10fda31159c22c7ed85074e05f8b97da8773ea461706c273e31bcbea836",
-                "sha256:ec468c022d09f1817c691cf884feb1030ef6f1e93e3ea6831b0d8144c06480d1"
+                "sha256:0614b6348866092d00df3dfb37e037fc06412ca67087de361a2777ea5ed62c16",
+                "sha256:06eac087ea55b3ebb2207d93b5ac56c847163899f05f5a77e1910f688fe10030",
+                "sha256:19d461c801b8904d201c6c38a99bfcfef673bfdfe0c7f026f582ef78896434e0",
+                "sha256:381558eafffc1432d08ca58063e71c7376ecaae48e9318354a90a1049a644845",
+                "sha256:3ee75b8ca48f6c48af25e967dce995ef94e46872b35c7d454b983c62c9c7006d",
+                "sha256:415cf7c806a3f56fb280dadcf3c92c85c0415e75665ca957b4a2a2e39c17a5c9",
+                "sha256:465d0f24bf4f75160f441793b55076b7a080a57d3a1f738390af2c20bee24fbb",
+                "sha256:4c654b1facf1f3b742e4d9b2dcdf0fa867b1f007b1b4981cc58a75ef5dca2a3c",
+                "sha256:50f8bdb421270f71b54695c62785e300fab4bb6127be40bf9f3084962a0c3adb",
+                "sha256:5448a87f6ed57ed844b64a05d3792827af584a8584613f6289867f4e77eb603b",
+                "sha256:560ea1a604c927399f36742abf342a4c5f3fee8e8e8a484b774dfe9630bd9a91",
+                "sha256:5b1c2b21b40229166a864f2b0aec06d37f0a204066deb1734c93370e0c76339d",
+                "sha256:69178674505ec81adf4af2a3bbacd0cb9a37ba7831bc3fca307f80e48ab2767b",
+                "sha256:69dbe0154e15b68dd671441ea8f23dad87488b24a6e650d45958f4722819a443",
+                "sha256:6faff25991dec48f8cac882055a09ae1a29fd15bc160bc3d663e789e994664c2",
+                "sha256:72d40a32d6443871ea0d147813caad58394b48729dfa4fbc45dcaac54f9506f2",
+                "sha256:7e22d0144d735f6c7df770509b8c0c33414bf460df0d5dddc98a159e5dbb10eb",
+                "sha256:841c491fa3e9c54e8f9cd5dae059e88f45e086aea090c28be9d42f59c8b99e01",
+                "sha256:86edb95c4d1fe4fae2111d7e0c10c6e42b7790b377bcf1952303469eee5b52bb",
+                "sha256:8f602dd5bcde7e4241419924f23c6f0d66723dd5408a58c3a2f781745c693f45",
+                "sha256:9387b09694fbf8ac7dcf887069068f81fb4124d05e09557ac7daabfbec1744bd",
+                "sha256:b329ae7ce971b5c4148d6cdb8119c0ce4587265b2330d4f2f3776ef851bee020",
+                "sha256:ba2a367ff478cd108d5319c0dc4fd4eb4ea3476dbfc45b00c45718e889cd9463",
+                "sha256:bc9e7b1e268be7a23fc66471b615c324e99c5db39ce8c49dd6dd8e962c7bc1b8",
+                "sha256:c890061915e95b619c1d3cc3c107c6fb021406b701c0c24b03e74830d522f210",
+                "sha256:cc3324e4159e6d1f55c3615b4c1c211f87cc96cc0cc7c946c8447dc1319f2e9d",
+                "sha256:d2dae84a3d0f76884a6102c62f2795b2d6602c2c95cfcce74c8a590b6200e533",
+                "sha256:d45f28c20bb67dee0f4a4caae709f40b0693d764b7b2bf2d58890f36b1bfcef0",
+                "sha256:e38bd91eae257f36c2b7245c0278e9cd9d754f3a66b8d2b548c623ba66e387b6",
+                "sha256:e43f6c7f9ba4f9d29edee530e45f9aa162872ec9549398b85971477a99f2a806",
+                "sha256:ea879afd1d6189fca02a85a7868560c9bb8415dccff6b7ae6d81e4f06b3ab30d",
+                "sha256:eb9dfa87152bd97019adc387b2f29ef6af601de4386f36570ca537ace96d96ed",
+                "sha256:efd59e83223cb77952997fb850c7a7c2a958c9af0642060f536722c2a9e9d53b",
+                "sha256:f3fe90dfb297bd8265238c06787911cd81c2cb89ac5b13e1c911928bdabfce0f"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.40.0"
+            "version": "==4.41.0"
         },
         "heatmap-cli": {
             "editable": true,
             "path": "."
         },
         "importlib-resources": {
             "hashes": [
@@ -422,30 +422,38 @@
                 "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
             ],
             "markers": "python_version >= '2'",
             "version": "==2023.3"
         },
         "zipp": {
             "hashes": [
-                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
-                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
+                "sha256:0b37c326d826d5ca35f2b9685cd750292740774ef16190008b00a0227c256fe0",
+                "sha256:857b158da2cbf427b376da1c24fd11faecbac5a4ac7523c3607f8a01f94c2ec0"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==3.16.0"
+            "version": "==3.16.1"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
+        "astroid": {
+            "hashes": [
+                "sha256:389656ca57b6108f939cf5d2f9a2a825a3be50ba9d589670f393236e0a03b91c",
+                "sha256:903f024859b7c7687d7a7f3a3f73b17301f8e42dfd9cc9df9d4418172d3e2dbd"
+            ],
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.15.6"
+        },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.12.1"
@@ -665,14 +673,22 @@
             "hashes": [
                 "sha256:3a27e95f763a428a739d2add979fa7494c912a32c17c4c38c4d5f082cad165a3",
                 "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.11.0"
         },
+        "dill": {
+            "hashes": [
+                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
+                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==0.3.6"
+        },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
@@ -722,51 +738,51 @@
                 "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.9.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:00ab569b2a3e591e00425023ade87e8fef90380c1dde61be7691cb524ca5f743",
-                "sha256:022c4a16b412293e7f1ce21b8bab7a6f9d12c4ffdf171fdc67122baddb973069",
-                "sha256:05171f3c546f64d78569f10adc0de72561882352cac39ec7439af12304d8d8c0",
-                "sha256:14037c31138fbd21847ad5e5441dfdde003e0a8f3feb5812a1a21fd1c255ffbd",
-                "sha256:15abb3d055c1b2dff9ce376b6c3db10777cb74b37b52b78f61657634fd348a0d",
-                "sha256:18ea64ac43e94c9e0c23d7a9475f1026be0e25b10dda8f236fc956188761df97",
-                "sha256:1a003608400dd1cca3e089e8c94973c6b51a4fb1ef00ff6d7641617b9242e637",
-                "sha256:1bc4c5b147be8dbc5df9cc8ac5e93ee914ad030fe2a201cc8f02f499db71011d",
-                "sha256:200729d12461e2038700d31f0d49ad5a7b55855dec7525074979a06b46f88505",
-                "sha256:337b6e83d7ee73c40ea62407f2ce03b07c3459e213b6f332b94a69923b9e1cb9",
-                "sha256:37467cee0f32cada2ec08bc16c9c31f9b53ea54b2f5604bf25a1246b5f50593a",
-                "sha256:425b74a608427499b0e45e433c34ddc350820b6f25b7c8761963a08145157a66",
-                "sha256:530c5d35109f3e0cea2535742d6a3bc99c0786cf0cbd7bb2dc9212387f0d908c",
-                "sha256:56d4d85f5374b45b08d2f928517d1e313ea71b4847240398decd0ab3ebbca885",
-                "sha256:5e00334c66f4e83535384cb5339526d01d02d77f142c23b2f97bd6a4f585497a",
-                "sha256:5fdf60f8a5c6bcce7d024a33f7e4bc7921f5b74e8ea13bccd204f2c8b86f3470",
-                "sha256:6a8d71b9a5c884c72741868e845c0e563c5d83dcaf10bb0ceeec3b4b2eb14c67",
-                "sha256:6d5adf4ba114f028fc3f5317a221fd8b0f4ef7a2e5524a2b1e0fd891b093791a",
-                "sha256:7449e5e306f3a930a8944c85d0cbc8429cba13503372a1a40f23124d6fb09b58",
-                "sha256:7961575221e3da0841c75da53833272c520000d76f7f71274dbf43370f8a1065",
-                "sha256:7f6e3fa3da923063c286320e728ba2270e49c73386e3a711aa680f4b0747d692",
-                "sha256:882983279bf39afe4e945109772c2ffad2be2c90983d6559af8b75c19845a80a",
-                "sha256:8a917828dbfdb1cbe50cf40eeae6fbf9c41aef9e535649ed8f4982b2ef65c091",
-                "sha256:8c4305b171b61040b1ee75d18f9baafe58bd3b798d1670078efe2c92436bfb63",
-                "sha256:91784e21a1a085fac07c6a407564f4a77feb471b5954c9ee55a4f9165151f6c1",
-                "sha256:94c915f6716589f78bc00fbc14c5b8de65cfd11ee335d32504f1ef234524cb24",
-                "sha256:97d95b8301b62bdece1af943b88bcb3680fd385f88346a4a899ee145913b414a",
-                "sha256:a954b90d1473c85a22ecf305761d9fd89da93bbd31dae86e7dea436ad2cb5dc9",
-                "sha256:aa83b3f151bc63970f39b2b42a06097c5a22fd7ed9f7ba008e618de4503d3895",
-                "sha256:b802dcbf9bcff74672f292b2466f6589ab8736ce4dcf36f48eb994c2847c4b30",
-                "sha256:bae8c13abbc2511e9a855d2142c0ab01178dd66b1a665798f357da0d06253e0d",
-                "sha256:c55f1b4109dbc3aeb496677b3e636d55ef46dc078c2a5e3f3db4e90f1c6d2907",
-                "sha256:eb52c10fda31159c22c7ed85074e05f8b97da8773ea461706c273e31bcbea836",
-                "sha256:ec468c022d09f1817c691cf884feb1030ef6f1e93e3ea6831b0d8144c06480d1"
+                "sha256:0614b6348866092d00df3dfb37e037fc06412ca67087de361a2777ea5ed62c16",
+                "sha256:06eac087ea55b3ebb2207d93b5ac56c847163899f05f5a77e1910f688fe10030",
+                "sha256:19d461c801b8904d201c6c38a99bfcfef673bfdfe0c7f026f582ef78896434e0",
+                "sha256:381558eafffc1432d08ca58063e71c7376ecaae48e9318354a90a1049a644845",
+                "sha256:3ee75b8ca48f6c48af25e967dce995ef94e46872b35c7d454b983c62c9c7006d",
+                "sha256:415cf7c806a3f56fb280dadcf3c92c85c0415e75665ca957b4a2a2e39c17a5c9",
+                "sha256:465d0f24bf4f75160f441793b55076b7a080a57d3a1f738390af2c20bee24fbb",
+                "sha256:4c654b1facf1f3b742e4d9b2dcdf0fa867b1f007b1b4981cc58a75ef5dca2a3c",
+                "sha256:50f8bdb421270f71b54695c62785e300fab4bb6127be40bf9f3084962a0c3adb",
+                "sha256:5448a87f6ed57ed844b64a05d3792827af584a8584613f6289867f4e77eb603b",
+                "sha256:560ea1a604c927399f36742abf342a4c5f3fee8e8e8a484b774dfe9630bd9a91",
+                "sha256:5b1c2b21b40229166a864f2b0aec06d37f0a204066deb1734c93370e0c76339d",
+                "sha256:69178674505ec81adf4af2a3bbacd0cb9a37ba7831bc3fca307f80e48ab2767b",
+                "sha256:69dbe0154e15b68dd671441ea8f23dad87488b24a6e650d45958f4722819a443",
+                "sha256:6faff25991dec48f8cac882055a09ae1a29fd15bc160bc3d663e789e994664c2",
+                "sha256:72d40a32d6443871ea0d147813caad58394b48729dfa4fbc45dcaac54f9506f2",
+                "sha256:7e22d0144d735f6c7df770509b8c0c33414bf460df0d5dddc98a159e5dbb10eb",
+                "sha256:841c491fa3e9c54e8f9cd5dae059e88f45e086aea090c28be9d42f59c8b99e01",
+                "sha256:86edb95c4d1fe4fae2111d7e0c10c6e42b7790b377bcf1952303469eee5b52bb",
+                "sha256:8f602dd5bcde7e4241419924f23c6f0d66723dd5408a58c3a2f781745c693f45",
+                "sha256:9387b09694fbf8ac7dcf887069068f81fb4124d05e09557ac7daabfbec1744bd",
+                "sha256:b329ae7ce971b5c4148d6cdb8119c0ce4587265b2330d4f2f3776ef851bee020",
+                "sha256:ba2a367ff478cd108d5319c0dc4fd4eb4ea3476dbfc45b00c45718e889cd9463",
+                "sha256:bc9e7b1e268be7a23fc66471b615c324e99c5db39ce8c49dd6dd8e962c7bc1b8",
+                "sha256:c890061915e95b619c1d3cc3c107c6fb021406b701c0c24b03e74830d522f210",
+                "sha256:cc3324e4159e6d1f55c3615b4c1c211f87cc96cc0cc7c946c8447dc1319f2e9d",
+                "sha256:d2dae84a3d0f76884a6102c62f2795b2d6602c2c95cfcce74c8a590b6200e533",
+                "sha256:d45f28c20bb67dee0f4a4caae709f40b0693d764b7b2bf2d58890f36b1bfcef0",
+                "sha256:e38bd91eae257f36c2b7245c0278e9cd9d754f3a66b8d2b548c623ba66e387b6",
+                "sha256:e43f6c7f9ba4f9d29edee530e45f9aa162872ec9549398b85971477a99f2a806",
+                "sha256:ea879afd1d6189fca02a85a7868560c9bb8415dccff6b7ae6d81e4f06b3ab30d",
+                "sha256:eb9dfa87152bd97019adc387b2f29ef6af601de4386f36570ca537ace96d96ed",
+                "sha256:efd59e83223cb77952997fb850c7a7c2a958c9af0642060f536722c2a9e9d53b",
+                "sha256:f3fe90dfb297bd8265238c06787911cd81c2cb89ac5b13e1c911928bdabfce0f"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.40.0"
+            "version": "==4.41.0"
         },
         "heatmap-cli": {
             "editable": true,
             "path": "."
         },
         "identify": {
             "hashes": [
@@ -812,14 +828,22 @@
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
+        "isort": {
+            "hashes": [
+                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
+                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
+            ],
+            "markers": "python_full_version >= '3.8.0'",
+            "version": "==5.12.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
@@ -894,14 +918,56 @@
                 "sha256:f6cb459eea32a4e2cf18ba5fcece2dbdf496384413bc1bae15583f19e567f3b2",
                 "sha256:f8ad8285b01b0d4695102546b342b493b3ccc6781fc28c8c6a1bb63e95d22f09",
                 "sha256:f9f39e2f049db33a908319cf46624a569b36983c7c78318e9726a4cb8923b26c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.4.4"
         },
+        "lazy-object-proxy": {
+            "hashes": [
+                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
+                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
+                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
+                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
+                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
+                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
+                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
+                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
+                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
+                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
+                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
+                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
+                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
+                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
+                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
+                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
+                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
+                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
+                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
+                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
+                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
+                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
+                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
+                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
+                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
+                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
+                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
+                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
+                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
+                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
+                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
+                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
+                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
+                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
+                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
+                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.9.0"
+        },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.0.0"
@@ -1005,14 +1071,22 @@
                 "sha256:f081c03f413f59390a80b3e351cc2b2ea0205839714dbc364519bcf51f4b56ca",
                 "sha256:fdbb46fad4fb47443b5b8ac76904b2e7a66556844f33370861b4788db0f8816a",
                 "sha256:fdcd28360dbb6203fb5219b1a5658df226ac9bebc2542a9e8f457de959d713d0"
             ],
             "index": "pypi",
             "version": "==3.7.2"
         },
+        "mccabe": {
+            "hashes": [
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
+        },
         "mdit-py-plugins": {
             "hashes": [
                 "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9",
                 "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.4.0"
@@ -1212,14 +1286,22 @@
             "hashes": [
                 "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
+        "pylint": {
+            "hashes": [
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
+            ],
+            "index": "pypi",
+            "version": "==2.17.4"
+        },
         "pyparsing": {
             "hashes": [
                 "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
                 "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
             "markers": "python_full_version >= '3.6.8'",
             "version": "==3.0.9"
@@ -1440,14 +1522,22 @@
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
+        "tomlkit": {
+            "hashes": [
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
+        },
         "tox": {
             "hashes": [
                 "sha256:57b5ab7e8bb3074edc3c0c0b4b192a4f3799d3723b2c5b76f1fa9f2d40316eea",
                 "sha256:d0d28f3fe6d6d7195c27f8b054c3e99d5451952b54abdae673b71609a581f640"
             ],
             "index": "pypi",
             "version": "==3.28.0"
@@ -1456,14 +1546,22 @@
             "hashes": [
                 "sha256:916c2213577aec0b3b5452c5bfb32fd077f3a3196f50a81ad57d7ef3fc2599e4",
                 "sha256:e470c18af115fe52eeff95e7e3cdd0793613eca19709966fc2724b79d55246cb"
             ],
             "index": "pypi",
             "version": "==1.1.0"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.7.1"
+        },
         "tzdata": {
             "hashes": [
                 "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
                 "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
             ],
             "markers": "python_version >= '2'",
             "version": "==2023.3"
@@ -1480,17 +1578,98 @@
             "hashes": [
                 "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
                 "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==20.23.1"
         },
+        "wrapt": {
+            "hashes": [
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==1.15.0"
+        },
         "zipp": {
             "hashes": [
-                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
-                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
+                "sha256:0b37c326d826d5ca35f2b9685cd750292740774ef16190008b00a0227c256fe0",
+                "sha256:857b158da2cbf427b376da1c24fd11faecbac5a4ac7523c3607f8a01f94c2ec0"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==3.16.0"
+            "version": "==3.16.1"
         }
     }
 }
```

### Comparing `heatmap_cli-0.1.2/README.md` & `heatmap_cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/docs/Makefile` & `heatmap_cli-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/docs/make.bat` & `heatmap_cli-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/docs/source/_static/logo.jpg` & `heatmap_cli-0.1.3/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/docs/source/conf.py` & `heatmap_cli-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/heatmap_cli/__init__.py` & `heatmap_cli-0.1.3/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `heatmap_cli-0.1.2/heatmap_cli/__main__.py` & `heatmap_cli-0.1.3/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/heatmap_cli/cli.py` & `heatmap_cli-0.1.3/heatmap_cli/cli.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/pyproject.toml` & `heatmap_cli-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/tests/conftest.py` & `heatmap_cli-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/tests/fixtures/sample.csv` & `heatmap_cli-0.1.3/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/tests/test_verbose_flag.py` & `heatmap_cli-0.1.3/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/tox.ini` & `heatmap_cli-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.1.2/PKG-INFO` & `heatmap_cli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

