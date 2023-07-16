# Comparing `tmp/stream_gears-0.1.8.tar.gz` & `tmp/stream_gears-0.1.9.tar.gz`

## Comparing `stream_gears-0.1.8.tar` & `stream_gears-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 stream_gears-0.1.8/Cargo.toml
--rw-r--r--   0     1001      121       81 2022-07-02 16:09:10.000000 stream_gears-0.1.8/.github/Dockerfile
--rw-r--r--   0     1001      121     1900 2022-07-02 16:09:10.000000 stream_gears-0.1.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      121      747 2022-07-02 16:09:10.000000 stream_gears-0.1.8/.gitignore
--rw-r--r--   0     1001      121    66269 2022-07-02 16:09:10.000000 stream_gears-0.1.8/Cargo.lock
--rw-r--r--   0     1001      121     1063 2022-07-02 16:09:10.000000 stream_gears-0.1.8/LICENSE
--rw-r--r--   0     1001      121      487 2022-07-02 16:09:10.000000 stream_gears-0.1.8/README.md
--rw-r--r--   0     1001      121      321 2022-07-02 16:09:10.000000 stream_gears-0.1.8/pyproject.toml
--rwxr-xr-x   0     1001      121      741 2022-07-02 16:09:41.000000 stream_gears-0.1.8/run-maturin-action.sh
--rw-r--r--   0     1001      121     4671 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/downloader/hls.rs
--rw-r--r--   0     1001      121    13420 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/downloader/httpflv.rs
--rw-r--r--   0     1001      121     1829 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/downloader/util.rs
--rw-r--r--   0     1001      121     3711 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/downloader.rs
--rw-r--r--   0     1001      121      440 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/error.rs
--rw-r--r--   0     1001      121    18691 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/flv_parser.rs
--rw-r--r--   0     1001      121     3185 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/flv_writer.rs
--rw-r--r--   0     1001      121     4479 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/lib.rs
--rw-r--r--   0     1001      121     6157 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/main.rs
--rw-r--r--   0     1001      121     2837 2022-07-02 16:09:10.000000 stream_gears-0.1.8/src/uploader.rs
--rw-r--r--   0     1001      121      361 2022-07-02 16:09:10.000000 stream_gears-0.1.8/tests/test_download.py
--rw-r--r--   0     1001      121      318 2022-07-02 16:09:10.000000 stream_gears-0.1.8/tests/test_upload.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 stream_gears-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 stream_gears-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      121       81 2022-07-03 15:49:44.000000 stream_gears-0.1.9/.github/Dockerfile
+-rw-r--r--   0     1001      121     1900 2022-07-03 15:49:44.000000 stream_gears-0.1.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      121      747 2022-07-03 15:49:44.000000 stream_gears-0.1.9/.gitignore
+-rw-r--r--   0     1001      121    66271 2022-07-03 15:49:44.000000 stream_gears-0.1.9/Cargo.lock
+-rw-r--r--   0     1001      121     1063 2022-07-03 15:49:44.000000 stream_gears-0.1.9/LICENSE
+-rw-r--r--   0     1001      121      487 2022-07-03 15:49:44.000000 stream_gears-0.1.9/README.md
+-rw-r--r--   0     1001      121      321 2022-07-03 15:49:44.000000 stream_gears-0.1.9/pyproject.toml
+-rwxr-xr-x   0     1001      121      741 2022-07-03 15:50:10.000000 stream_gears-0.1.9/run-maturin-action.sh
+-rw-r--r--   0     1001      121     4671 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/downloader/hls.rs
+-rw-r--r--   0     1001      121    13820 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/downloader/httpflv.rs
+-rw-r--r--   0     1001      121     1829 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/downloader/util.rs
+-rw-r--r--   0     1001      121     3713 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/downloader.rs
+-rw-r--r--   0     1001      121      440 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/error.rs
+-rw-r--r--   0     1001      121    18691 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/flv_parser.rs
+-rw-r--r--   0     1001      121     3185 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/flv_writer.rs
+-rw-r--r--   0     1001      121     4479 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      121     6168 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/main.rs
+-rw-r--r--   0     1001      121     2837 2022-07-03 15:49:44.000000 stream_gears-0.1.9/src/uploader.rs
+-rw-r--r--   0     1001      121      361 2022-07-03 15:49:44.000000 stream_gears-0.1.9/tests/test_download.py
+-rw-r--r--   0     1001      121      318 2022-07-03 15:49:44.000000 stream_gears-0.1.9/tests/test_upload.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 stream_gears-0.1.9/PKG-INFO
```

### Comparing `stream_gears-0.1.8/Cargo.toml` & `stream_gears-0.1.9/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "stream-gears"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 
 [profile.release]
 lto = true
 codegen-units = 1
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `stream_gears-0.1.8/.github/workflows/CI.yml` & `stream_gears-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/.gitignore` & `stream_gears-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/Cargo.lock` & `stream_gears-0.1.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base-x"
-version = "0.2.10"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc19a4937b4fbd3fe3379793130e42060d10627a360f2127802b10b87e7baf74"
+checksum = "4cbbc9d0964165b47557570cce6c952866c2678457aca742aafc9fb771d30270"
 
 [[package]]
 name = "base64"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "904dfeac50f3cdaba28fc6f57fdcddb75f49ed61346676a78c4ffe55877802fd"
 
@@ -151,17 +151,17 @@
 name = "bumpalo"
 version = "3.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37ccbd214614c6783386c1af30caf03192f17891059cecc394b4fb119e363de3"
 
 [[package]]
 name = "bytemuck"
-version = "1.9.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdead85bdec19c194affaeeb670c0e41fe23de31459efd1c174d049269cf02cc"
+checksum = "c53dfa917ec274df8ed3c572698f381a24eef2efba9492d797301b72b6db408a"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -200,47 +200,47 @@
  "num-traits",
  "time 0.1.44",
  "winapi",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.6"
+version = "3.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f1fe12880bae935d142c8702d500c63a4e8634b6c3c57ad72bf978fc7b6249a"
+checksum = "190814073e85d238f31ff738fcb0bf6910cedeb73376c87cd69291028966fd83"
 dependencies = [
  "atty",
  "bitflags",
  "clap_derive",
  "clap_lex",
  "indexmap",
  "once_cell",
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.6"
+version = "3.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed6db9e867166a43a53f7199b5e4d1f522a1e5bd626654be263c999ce59df39a"
+checksum = "759bf187376e1afa7b85b959e6a664a3e7a95203415dba952ad19139e798f902"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87eba3c8c7f42ef17f6c659fc7416d0f4758cd3e58861ee63c5fa4a4dde649e4"
+checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "color_quant"
 version = "1.1.0"
@@ -288,15 +288,15 @@
 [[package]]
 name = "cookie"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94d4706de1b0fa5b132270cddffa8585166037822e260a944fe161acd137ca05"
 dependencies = [
  "percent-encoding",
- "time 0.3.10",
+ "time 0.3.11",
  "version_check",
 ]
 
 [[package]]
 name = "cookie_store"
 version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -320,15 +320,15 @@
 dependencies = [
  "cookie 0.16.0",
  "idna",
  "log",
  "publicsuffix",
  "serde",
  "serde_json",
- "time 0.3.10",
+ "time 0.3.11",
  "url",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -386,17 +386,17 @@
  "memoffset",
  "once_cell",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.9"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ff1f980957787286a554052d03c7aee98d99cc32e09f6d45f0a814133c87978"
+checksum = "7d82ee10ce34d7bc12c2122495e7593a9c41347ecdd64185af4ecf72cb1a7f83"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "crypto-bigint"
@@ -454,17 +454,17 @@
 name = "discard"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "212d0f5754cb6769937f4501cc0e67f4f4483c8d2c3e1e922ee9edbe4ab4c7c0"
 
 [[package]]
 name = "either"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
+checksum = "3f107b87b6afc2a64fd13cac55fe06d6c8859f12d4b14cbcdd2c67d0976781be"
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -635,17 +635,17 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gif"
-version = "0.11.3"
+version = "0.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3a7187e78088aead22ceedeee99779455b23fc231fe13ec443f99bb71694e5b"
+checksum = "3edd93c6756b4dfaf2709eafcc345ba2636565295c198a9cfbf75fa5e3e00b06"
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
 name = "glob"
@@ -811,17 +811,17 @@
  "png",
  "scoped_threadpool",
  "tiff",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.0"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c6392766afd7964e2531940894cffe4bd8d7d17dbc3c1c4857040fd4b33bdb3"
+checksum = "10a35a97730320ffe8e2d410b5d3b69279b98d2c14bdb8b70ea89ecf7888d41e"
 dependencies = [
  "autocfg 1.1.0",
  "hashbrown 0.12.1",
 ]
 
 [[package]]
 name = "indicatif"
@@ -898,17 +898,17 @@
 name = "libm"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33a33a362ce288760ec6a508b94caaec573ae7d3bbbd91b87aa0bad4456839db"
 
 [[package]]
 name = "linked-hash-map"
-version = "0.5.4"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb9b38af92608140b86b693604b9ffcc5824240a484d1ecd4795bacb2fe88f3"
+checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "327fa5b6a6940e4699ec49a9beae1ea4845c6bab9314e4f84ac68742139d8c53"
 dependencies = [
@@ -1771,37 +1771,37 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.137"
+version = "1.0.138"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61ea8d54c77f8315140a05f4c7237403bf38b72704d031543aa1d16abbf517d1"
+checksum = "1578c6245786b9d168c5447eeacfb96856573ca56c9d68fdcf394be134882a47"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.137"
+version = "1.0.138"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f26faba0c3959972377d3b2d306ee9f71faee9714294e41bb777f83f88578be"
+checksum = "023e9b1467aef8a10fb88f25611870ada9800ef7e22afce356bb0d2387b6f27c"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7ce2b32a1aed03c558dc61a5cd328f15aff2dbc17daad8fb8af04d2100e15c"
+checksum = "82c2c1fdcd807d1098552c5b9a36e425e42e9fbd7c6a37a8425f390f781f7fa7"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1865,17 +1865,17 @@
 name = "slab"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb703cfe953bccee95685111adeedb76fabe4e97549a58d16f03ea7b9367bb32"
 
 [[package]]
 name = "smallvec"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2dd574626839106c320a323308629dcb1acfc96e32a8cba364ddc61ac23ee83"
+checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
 
 [[package]]
 name = "socket2"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "66d72b759436ae32898a2af0a14218dbf55efde3feeb170eb623637db85ee1e0"
 dependencies = [
@@ -1954,15 +1954,15 @@
 name = "stdweb-internal-runtime"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "213701ba3370744dcd1a12960caa4843b3d68b4d1c0a5d575e0d65b2ee9d16c0"
 
 [[package]]
 name = "stream-gears"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anyhow",
  "biliup",
  "byteorder",
  "bytes",
  "chrono",
  "m3u8-rs",
@@ -2132,17 +2132,17 @@
  "time-macros 0.1.1",
  "version_check",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.10"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82501a4c1c0330d640a6e176a3d6a204f5ec5237aca029029d21864a902e27b0"
+checksum = "72c91f41dcb2f096c05f0873d667dceec1087ce5bcf984ec8ffb19acddbb3217"
 dependencies = [
  "itoa",
  "libc",
  "num_threads",
  "time-macros 0.2.4",
 ]
 
@@ -2277,34 +2277,34 @@
 [[package]]
 name = "tracing-appender"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09d48f71a791638519505cefafe162606f706c25592e4bde4d97600c0195312e"
 dependencies = [
  "crossbeam-channel",
- "time 0.3.10",
+ "time 0.3.11",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc6b8ad3567499f98a1db7a752b07a7c8c7c7c34c332ec00effb2b0027974b7c"
+checksum = "11c75893af559bc8e10716548bdef5cb2b983f8e637db9d0e15126b61b484ee2"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.27"
+version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7709595b8878a4965ce5e87ebf880a7d39c9afc6837721b21a5a816a8117d921"
+checksum = "7b7358be39f2f274f322d2aaed611acc57f382e8eb1e5b48cb9ae30933495ce7"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-log"
@@ -2315,17 +2315,17 @@
  "lazy_static",
  "log",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.11"
+version = "0.3.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bc28f93baff38037f64e6f43d34cfa1605f27a49c34e8a04c5e78b0babf2596"
+checksum = "3a713421342a5a666b7577783721d3117f1b69a393df803ee17bb73b1e122a59"
 dependencies = [
  "ansi_term",
  "sharded-slab",
  "smallvec",
  "thread_local",
  "tracing-core",
  "tracing-log",
@@ -2373,17 +2373,17 @@
 name = "unicode-ident"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bd2fe26506023ed7b5e1e315add59d6f584c621d037f9368fea9cfb988f368c"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.19"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54590932941a9e9266f0832deed84ebe1bf2e4c9e4a3554d393d18f5e854bf9"
+checksum = "854cbdc4f7bc6ae19c820d44abdc3277ac3e1b2b93db20a636825d9322fb60e6"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
 version = "0.1.9"
```

### Comparing `stream_gears-0.1.8/LICENSE` & `stream_gears-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/run-maturin-action.sh` & `stream_gears-0.1.9/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/downloader/hls.rs` & `stream_gears-0.1.9/src/downloader/hls.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/downloader/httpflv.rs` & `stream_gears-0.1.9/src/downloader/httpflv.rs`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     // let mut writer = BufWriter::new(file);
     // flv_writer::to_json(&mut writer, &header)?;
 
     let mut out = FlvFile::new(file_name)?;
     let mut downloaded_size = 9 + 4;
     let mut on_meta_data = None;
     let mut aac_sequence_header = None;
-    let mut h264_sequence_header = None;
+    let mut h264_sequence_header: Option<(TagHeader, Bytes, Bytes)> = None;
     let mut prev_timestamp = 0;
     let mut create_new = false;
     loop {
         let tag_header_bytes = connection.read_frame(11)?;
         if tag_header_bytes.is_empty() {
             // let mut rdr = Cursor::new(tag_header_bytes);
             // println!("{}", rdr.read_u32::<BigEndian>().unwrap());
@@ -91,21 +91,26 @@
                 }
             }
             TagData::Video(video_data) => {
                 let (packet_type, composition_time) = if CodecId::H264 == video_data.codec_id {
                     let (_, avc_video_header) = avc_video_packet_header(video_data.video_data)
                         .expect("Error in parsing avc video packet header.");
                     if avc_video_header.packet_type == AVCPacketType::SequenceHeader {
-                        if h264_sequence_header.is_some() {
-                            warn!("Unexpected h264 sequence header tag. {tag_header:?}");
-                            // panic!("Unexpected h264 sequence header tag.");
-                            create_new = true;
-                        }
-                        h264_sequence_header =
-                            Some((tag_header, bytes.clone(), previous_tag_size.clone()));
+                        h264_sequence_header = match h264_sequence_header {
+                            None => Some((tag_header, bytes.clone(), previous_tag_size.clone())),
+                            Some((_, binary_data, _)) => {
+                                warn!("Unexpected h264 sequence header tag. {tag_header:?}");
+                                // panic!("Unexpected h264 sequence header tag.");
+                                if bytes != binary_data {
+                                    create_new = true;
+                                    warn!("Different h264 sequence header tag. {tag_header:?}");
+                                }
+                                Some((tag_header, bytes.clone(), previous_tag_size.clone()))
+                            }
+                        };
                     }
                     (
                         Some(avc_video_header.packet_type),
                         Some(avc_video_header.composition_time),
                     )
                 } else {
                     (None, None)
```

### Comparing `stream_gears-0.1.8/src/downloader/util.rs` & `stream_gears-0.1.9/src/downloader/util.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/downloader.rs` & `stream_gears-0.1.9/src/downloader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -112,12 +112,12 @@
             HeaderValue::from_static("https://live.bilibili.com"),
         );
         download(
             "",
             headers,
             "testdouyu%Y-%m-%dT%H_%M_%S",
             // Segment::Size(20 * 1024 * 1024, 0),
-            Segment::Time(std::time::Duration::from_secs(60), Default::default()),
+            Segment::Time(std::time::Duration::from_secs(6000), Default::default()),
         )?;
         Ok(())
     }
 }
```

### Comparing `stream_gears-0.1.8/src/flv_parser.rs` & `stream_gears-0.1.9/src/flv_parser.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/flv_writer.rs` & `stream_gears-0.1.9/src/flv_writer.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/lib.rs` & `stream_gears-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/src/main.rs` & `stream_gears-0.1.9/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     let file_name = &args[1];
     let flv_file = std::fs::File::open(file_name)?;
     let buf_reader = BufReader::new(flv_file);
     let mut connection = Connection::new(buf_reader);
     connection.read_frame(9)?;
     download(
         connection,
-        &(file_name.to_owned() + "new"),
+        &(file_name.to_owned() + "new%H_%M_%S%.f"),
         Segment::Time(Duration::from_secs(60 * 60 * 24), Default::default()),
     );
     // Ok(result)
     // generate_json()?;
     Ok(())
 }
```

### Comparing `stream_gears-0.1.8/src/uploader.rs` & `stream_gears-0.1.9/src/uploader.rs`

 * *Files identical despite different names*

### Comparing `stream_gears-0.1.8/PKG-INFO` & `stream_gears-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-gears
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

