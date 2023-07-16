# Comparing `tmp/lazrs-0.5.0.tar.gz` & `tmp/lazrs-0.5.1.tar.gz`

## Comparing `lazrs-0.5.0.tar` & `lazrs-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 lazrs-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123     4823 2022-12-27 12:38:22.000000 lazrs-0.5.0/.github/workflows/build.yml
--rw-r--r--   0     1001      123       54 2022-12-27 12:38:22.000000 lazrs-0.5.0/.gitignore
--rw-r--r--   0     1001      123     1077 2022-12-27 12:38:22.000000 lazrs-0.5.0/LICENSE.txt
--rw-r--r--   0     1001      123      305 2022-12-27 12:38:22.000000 lazrs-0.5.0/README.md
--rw-r--r--   0     1001      123      722 2022-12-27 12:38:22.000000 lazrs-0.5.0/noxfile.py
--rw-r--r--   0     1001      123      233 2022-12-27 12:38:22.000000 lazrs-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123     5522 2022-12-27 12:38:22.000000 lazrs-0.5.0/src/adapters.rs
--rw-r--r--   0     1001      123    17058 2022-12-27 12:38:22.000000 lazrs-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123    10530 2022-12-27 12:38:42.000000 lazrs-0.5.0/Cargo.lock
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 lazrs-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 lazrs-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123     4823 2023-07-16 17:29:45.000000 lazrs-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0     1001      123       54 2023-07-16 17:29:45.000000 lazrs-0.5.1/.gitignore
+-rw-r--r--   0     1001      123     1077 2023-07-16 17:29:45.000000 lazrs-0.5.1/LICENSE.txt
+-rw-r--r--   0     1001      123      305 2023-07-16 17:29:45.000000 lazrs-0.5.1/README.md
+-rw-r--r--   0     1001      123      715 2023-07-16 17:29:45.000000 lazrs-0.5.1/noxfile.py
+-rw-r--r--   0     1001      123      233 2023-07-16 17:29:45.000000 lazrs-0.5.1/pyproject.toml
+-rw-r--r--   0     1001      123     5522 2023-07-16 17:29:45.000000 lazrs-0.5.1/src/adapters.rs
+-rw-r--r--   0     1001      123    17058 2023-07-16 17:29:45.000000 lazrs-0.5.1/src/lib.rs
+-rw-r--r--   0     1001      123    10511 2023-07-16 17:29:54.000000 lazrs-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 lazrs-0.5.1/PKG-INFO
```

### Comparing `lazrs-0.5.0/.github/workflows/build.yml` & `lazrs-0.5.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.0/LICENSE.txt` & `lazrs-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.0/noxfile.py` & `lazrs-0.5.1/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 
 WHEEL_DIR = Path(os.environ.get("CARGO_TARGET_DIR", '.target')) / "wheels"
 
 Path('dist').mkdir(exist_ok=True)
 
 
-@nox.session(python=['3.7', '3.8', '3.9', '3.10', '3.11'])
+@nox.session(python=['3.8', '3.9', '3.10', '3.11'])
 def build_wheel(session):
     session.install('maturin')
     session.run('cargo', 'clean', external=True)
     session.run('maturin', 'build', '--interpreter', 'python', '--release')
 
     wheels = list(WHEEL_DIR.glob('*.whl'))
     assert len(wheels) == 1
```

### Comparing `lazrs-0.5.0/src/adapters.rs` & `lazrs-0.5.1/src/adapters.rs`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.0/src/lib.rs` & `lazrs-0.5.1/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use pyo3::{create_exception, wrap_pyfunction};
 
 use crate::adapters::{PyReadableFileObject, PyWriteableFileObject};
 use std::io::{BufReader, BufWriter, Read, Write};
 
 mod adapters;
 
-create_exception!(pylaz, LazrsError, pyo3::exceptions::PyRuntimeError);
+create_exception!(lazrs, LazrsError, pyo3::exceptions::PyRuntimeError);
 
 fn as_bytes(object: &PyAny) -> PyResult<&[u8]> {
     let buffer = pyo3::buffer::PyBuffer::<u8>::get(object)?;
 
     let slc =
         unsafe { std::slice::from_raw_parts(buffer.buf_ptr() as *const u8, buffer.len_bytes()) };
```

### Comparing `lazrs-0.5.0/Cargo.lock` & `lazrs-0.5.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,106 +24,103 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "laz"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "004b211256fe9c0c4e25309ee6b6517d0710be209c7083d45a4c9feb0fc54141"
+checksum = "78438fec528e9c26c15001f3d64ecfe1daef73a41a20a268037f748248c0c51e"
 dependencies = [
  "byteorder",
  "num-traits",
  "rayon",
 ]
 
 [[package]]
 name = "lazrs"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
  "laz",
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -132,17 +129,17 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.15"
@@ -150,56 +147,56 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "92de25114670a878b1261c79c9f8f729fb97e95bac93f6312f583c60dd6a1dfe"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
@@ -258,142 +255,142 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "5907a1b7c277254a8b15170f6e7c97cfa60ee7872a3217663bb81151e48184bb"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cac410af5d00ab6884528b4ab69d1e8e146e8d471201800fa1b4524126de6ad3"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `lazrs-0.5.0/PKG-INFO` & `lazrs-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazrs
-Version: 0.5.0
+Version: 0.5.1
 License-File: LICENSE.txt
 Summary: Python bindings for laz-rs
 Author: tmontaigu <thomas.montaigu@laposte.net>
 Author-email: tmontaigu <thomas.montaigu@laposte.net>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

