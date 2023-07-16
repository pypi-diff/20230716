# Comparing `tmp/chacha20poly1305_reuseable-0.2.5.tar.gz` & `tmp/chacha20poly1305_reuseable-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chacha20poly1305_reuseable-0.2.5.tar", max compression
+gzip compressed data, was "chacha20poly1305_reuseable-0.3.0.tar", max compression
```

## Comparing `chacha20poly1305_reuseable-0.2.5.tar` & `chacha20poly1305_reuseable-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12880 2023-04-28 02:22:28.980396 chacha20poly1305_reuseable-0.2.5/LICENSE
--rw-r--r--   0        0        0     4027 2023-04-28 02:22:28.980396 chacha20poly1305_reuseable-0.2.5/README.md
--rw-r--r--   0        0        0      905 2023-04-28 02:22:28.980396 chacha20poly1305_reuseable-0.2.5/build_ext.py
--rw-r--r--   0        0        0     2131 2023-04-28 02:22:29.924457 chacha20poly1305_reuseable-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1772 2023-04-28 02:22:28.980396 chacha20poly1305_reuseable-0.2.5/src/chacha20poly1305_reuseable/__init__.pxd
--rw-r--r--   0        0        0     8865 2023-04-28 02:22:29.900455 chacha20poly1305_reuseable-0.2.5/src/chacha20poly1305_reuseable/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 02:22:28.980396 chacha20poly1305_reuseable-0.2.5/src/chacha20poly1305_reuseable/py.typed
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.5/setup.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    12880 2023-07-16 00:36:30.832306 chacha20poly1305_reuseable-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4027 2023-07-16 00:36:30.832306 chacha20poly1305_reuseable-0.3.0/README.md
+-rw-r--r--   0        0        0      905 2023-07-16 00:36:30.832306 chacha20poly1305_reuseable-0.3.0/build_ext.py
+-rw-r--r--   0        0        0     2131 2023-07-16 00:36:32.164325 chacha20poly1305_reuseable-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1642 2023-07-16 00:36:30.832306 chacha20poly1305_reuseable-0.3.0/src/chacha20poly1305_reuseable/__init__.pxd
+-rw-r--r--   0        0        0     8514 2023-07-16 00:36:32.120324 chacha20poly1305_reuseable-0.3.0/src/chacha20poly1305_reuseable/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 00:36:30.832306 chacha20poly1305_reuseable-0.3.0/src/chacha20poly1305_reuseable/py.typed
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.3.0/setup.py
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.3.0/PKG-INFO
```

### Comparing `chacha20poly1305_reuseable-0.2.5/LICENSE` & `chacha20poly1305_reuseable-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.5/README.md` & `chacha20poly1305_reuseable-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.5/build_ext.py` & `chacha20poly1305_reuseable-0.3.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.5/pyproject.toml` & `chacha20poly1305_reuseable-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chacha20poly1305-reuseable"
-version = "0.2.5"
+version = "0.3.0"
 description = "ChaCha20Poly1305 that is reuseable for asyncio"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/chacha20poly1305-reuseable"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `chacha20poly1305_reuseable-0.2.5/src/chacha20poly1305_reuseable/__init__.py` & `chacha20poly1305_reuseable-0.3.0/src/chacha20poly1305_reuseable/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-__version__ = "0.2.5"
+__version__ = "0.3.0"
 
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 
 import os
 import typing
+from functools import partial
 from typing import Optional, Union
 
 from cryptography import exceptions
 from cryptography.exceptions import InvalidTag
 from cryptography.hazmat.backends.openssl.backend import backend
 from cryptography.hazmat.primitives.ciphers.aead import ChaCha20Poly1305
 
-openssl_assert = backend.openssl_assert
-EVP_CIPHER_CTX_ctrl = backend._lib.EVP_CIPHER_CTX_ctrl
-EVP_CTRL_AEAD_SET_TAG = backend._lib.EVP_CTRL_AEAD_SET_TAG
-EVP_CTRL_AEAD_SET_IVLEN = backend._lib.EVP_CTRL_AEAD_SET_IVLEN
-EVP_CipherInit_ex = backend._lib.EVP_CipherInit_ex
-EVP_CIPHER_CTX_new = backend._lib.EVP_CIPHER_CTX_new
-EVP_CIPHER_CTX_free = backend._lib.EVP_CIPHER_CTX_free
-EVP_get_cipherbyname = backend._lib.EVP_get_cipherbyname
-EVP_CIPHER_CTX_set_key_length = backend._lib.EVP_CIPHER_CTX_set_key_length
-EVP_CipherUpdate = backend._lib.EVP_CipherUpdate
-EVP_CipherFinal_ex = backend._lib.EVP_CipherFinal_ex
-EVP_CTRL_AEAD_GET_TAG = backend._lib.EVP_CTRL_AEAD_GET_TAG
-
-ffi_from_buffer = backend._ffi.from_buffer
-ffi_gc = backend._ffi.gc
-ffi_new = backend._ffi.new
-ffi_buffer = backend._ffi.buffer
+openssl_failure = partial(backend.openssl_assert, False)
+lib = backend._lib
+ffi = backend._ffi
+
+EVP_CIPHER_CTX_ctrl = lib.EVP_CIPHER_CTX_ctrl
+EVP_CTRL_AEAD_SET_TAG = lib.EVP_CTRL_AEAD_SET_TAG
+EVP_CTRL_AEAD_SET_IVLEN = lib.EVP_CTRL_AEAD_SET_IVLEN
+EVP_CipherInit_ex = lib.EVP_CipherInit_ex
+EVP_CIPHER_CTX_new = lib.EVP_CIPHER_CTX_new
+EVP_CIPHER_CTX_free = lib.EVP_CIPHER_CTX_free
+EVP_get_cipherbyname = lib.EVP_get_cipherbyname
+EVP_CIPHER_CTX_set_key_length = lib.EVP_CIPHER_CTX_set_key_length
+EVP_CipherUpdate = lib.EVP_CipherUpdate
+EVP_CipherFinal_ex = lib.EVP_CipherFinal_ex
+EVP_CTRL_AEAD_GET_TAG = lib.EVP_CTRL_AEAD_GET_TAG
+
+ffi_from_buffer = ffi.from_buffer
+ffi_gc = ffi.gc
+ffi_new = ffi.new
+ffi_buffer = ffi.buffer
 
-NULL = backend._ffi.NULL
+NULL = ffi.NULL
 
 _ENCRYPT = 1
 _DECRYPT = 0
 
 _bytes = bytes
 
 
@@ -52,195 +56,180 @@
         raise TypeError("data must be bytes")
     if not isinstance(associated_data, bytes):
         raise TypeError("associated_data must be bytes")
     if len(nonce) != nonce_len:
         raise ValueError("Nonce must be 12 bytes")
 
 
+MAX_SIZE = 2**32
+KEY_LEN = 32
+NONCE_LEN = 12
+NONCE_LEN_UINT = NONCE_LEN
+TAG_LENGTH = 16
+CIPHER_NAME = b"chacha20-poly1305"
+
+
 class ChaCha20Poly1305Reusable(ChaCha20Poly1305):
     """A reuseable version of ChaCha20Poly1305.
 
     This is modified version of ChaCha20Poly1305 that does not recreate
     the underlying ctx each time. It is not thread-safe and should not
     only be called in the thread it was created.
 
     The primary use case for this code is HAP streams.
     """
 
-    _MAX_SIZE = 2**32
-    _KEY_LEN = 32
-    _NONCE_LEN = 12
-    _TAG_LENGTH = 16
-
     def __init__(self, key: Union[_bytes, bytearray]) -> None:
         if not backend.aead_cipher_supported(self):
             raise exceptions.UnsupportedAlgorithm(
                 "ChaCha20Poly1305Reusable is not supported by this version of OpenSSL",
                 exceptions._Reasons.UNSUPPORTED_CIPHER,
             )
 
         if not isinstance(key, (bytes, bytearray)):
             raise TypeError("key must be bytes or bytearay")
 
-        if len(key) != self._KEY_LEN:
+        if len(key) != KEY_LEN:
             raise ValueError("ChaCha20Poly1305Reusable key must be 32 bytes.")
 
-        self._cipher_name = b"chacha20-poly1305"
         self._key = key
         self._decrypt_ctx: Optional[object] = None
         self._encrypt_ctx: Optional[object] = None
 
     @classmethod
     def generate_key(cls) -> _bytes:
-        return os.urandom(ChaCha20Poly1305Reusable._KEY_LEN)
+        return os.urandom(KEY_LEN)
 
     def encrypt(
         self,
         nonce: Union[_bytes, bytearray],
         data: _bytes,
         associated_data: typing.Optional[bytes],
     ) -> bytes:
-        if not self._encrypt_ctx:
-            self._encrypt_ctx = _aead_setup_with_fixed_nonce_len(
-                self._cipher_name,
+        encrypt_ctx = self._encrypt_ctx
+        if not encrypt_ctx:
+            encrypt_ctx = _aead_setup_with_fixed_nonce_len(
+                CIPHER_NAME,
                 self._key,
-                self._NONCE_LEN,
+                NONCE_LEN,
                 _ENCRYPT,
             )
+            self._encrypt_ctx = encrypt_ctx
 
         if associated_data is None:
             associated_data = b""
 
-        if len(data) > self._MAX_SIZE or len(associated_data) > self._MAX_SIZE:
+        if len(data) > MAX_SIZE or len(associated_data) > MAX_SIZE:
             # This is OverflowError to match what cffi would raise
             raise OverflowError("Data or associated data too long. Max 2**32 bytes")
 
-        _check_params(self._NONCE_LEN, nonce, data, associated_data)
+        _check_params(NONCE_LEN_UINT, nonce, data, associated_data)
         return _encrypt_with_fixed_nonce_len(
-            self._encrypt_ctx,
+            encrypt_ctx,
             nonce,
             data,
             associated_data,
-            self._TAG_LENGTH,
+            TAG_LENGTH,
         )
 
     def decrypt(
         self,
         nonce: Union[_bytes, bytearray],
         data: _bytes,
         associated_data: typing.Optional[_bytes],
     ) -> bytes:
-        if not self._decrypt_ctx:
-            self._decrypt_ctx = _aead_setup_with_fixed_nonce_len(
-                self._cipher_name,
+        decrypt_ctx = self._decrypt_ctx
+        if not decrypt_ctx:
+            decrypt_ctx = _aead_setup_with_fixed_nonce_len(
+                CIPHER_NAME,
                 self._key,
-                self._NONCE_LEN,
+                NONCE_LEN,
                 _DECRYPT,
             )
+            self._decrypt_ctx = decrypt_ctx
 
         if associated_data is None:
             associated_data = b""
 
-        _check_params(self._NONCE_LEN, nonce, data, associated_data)
+        _check_params(NONCE_LEN_UINT, nonce, data, associated_data)
         return _decrypt_with_fixed_nonce_len(
-            self._decrypt_ctx,
+            decrypt_ctx,
             nonce,
             data,
             associated_data,
-            self._TAG_LENGTH,
+            TAG_LENGTH,
         )
 
 
-def _create_ctx() -> object:
-    ctx = EVP_CIPHER_CTX_new()
-    ctx = ffi_gc(ctx, EVP_CIPHER_CTX_free)
-    return ctx
+def _set_nonce(ctx: object, nonce: Union[_bytes, bytearray], operation: int) -> None:
+    nonce_ptr = ffi_from_buffer(nonce)
+    res = EVP_CipherInit_ex(
+        ctx,
+        NULL,
+        NULL,
+        NULL,
+        nonce_ptr,
+        int(operation == _ENCRYPT),
+    )
+    openssl_assert(res != 0)
 
 
-def _set_cipher(ctx: object, cipher_name: _bytes, operation: int) -> None:
+def _aead_setup_with_fixed_nonce_len(
+    cipher_name: _bytes, key: Union[_bytes, bytearray], nonce_len: int, operation: int
+) -> object:
+    # create the ctx
+    ctx = EVP_CIPHER_CTX_new()
+    ctx = ffi_gc(ctx, EVP_CIPHER_CTX_free)
+    # set the cipher
     evp_cipher = EVP_get_cipherbyname(cipher_name)
     openssl_assert(evp_cipher != NULL)
     res = EVP_CipherInit_ex(
         ctx,
         evp_cipher,
         NULL,
         NULL,
         NULL,
         int(operation == _ENCRYPT),
     )
     openssl_assert(res != 0)
-
-
-def _set_key_len(ctx: object, key_len: int) -> None:
-    res = EVP_CIPHER_CTX_set_key_length(ctx, key_len)
+    # Set the key length
+    res = EVP_CIPHER_CTX_set_key_length(ctx, len(key))
     openssl_assert(res != 0)
-
-
-def _set_key(ctx: object, key: _bytes, operation: int) -> None:
-    key_ptr = ffi_from_buffer(key)
+    # Set the key
     res = EVP_CipherInit_ex(
         ctx,
         NULL,
         NULL,
-        key_ptr,
+        ffi_from_buffer(key),
         NULL,
         int(operation == _ENCRYPT),
     )
     openssl_assert(res != 0)
-
-
-def _set_decrypt_tag(ctx: object, tag: _bytes) -> None:
-    res = EVP_CIPHER_CTX_ctrl(ctx, EVP_CTRL_AEAD_SET_TAG, len(tag), tag)
-    openssl_assert(res != 0)
-
-
-def _set_nonce_len(ctx: object, nonce_len: int) -> None:
+    # set nonce length
     res = EVP_CIPHER_CTX_ctrl(
         ctx,
         EVP_CTRL_AEAD_SET_IVLEN,
         nonce_len,
         NULL,
     )
     openssl_assert(res != 0)
-
-
-def _set_nonce(ctx: object, nonce: Union[_bytes, bytearray], operation: int) -> None:
-    nonce_ptr = ffi_from_buffer(nonce)
-    res = EVP_CipherInit_ex(
-        ctx,
-        NULL,
-        NULL,
-        NULL,
-        nonce_ptr,
-        int(operation == _ENCRYPT),
-    )
-    openssl_assert(res != 0)
-
-
-def _aead_setup_with_fixed_nonce_len(
-    cipher_name: _bytes, key: Union[_bytes, bytearray], nonce_len: int, operation: int
-) -> object:
-    ctx = _create_ctx()
-    _set_cipher(ctx, cipher_name, operation)
-    _set_key_len(ctx, len(key))
-    _set_key(ctx, key, operation)
-    _set_nonce_len(ctx, nonce_len)
     return ctx
 
 
 def _process_aad(ctx: object, associated_data: _bytes) -> None:
     outlen = ffi_new("int *")
     res = EVP_CipherUpdate(ctx, NULL, outlen, associated_data, len(associated_data))
     openssl_assert(res != 0)
 
 
 def _process_data(ctx: object, data: _bytes) -> _bytes:
     outlen = ffi_new("int *")
-    buf = ffi_new("unsigned char[]", len(data))
-    res = EVP_CipherUpdate(ctx, buf, outlen, data, len(data))
+    data_len = len(data)
+    buf = ffi_new("unsigned char[]", data_len)
+    res = EVP_CipherUpdate(ctx, buf, outlen, data, data_len)
     openssl_assert(res != 0)
     return ffi_buffer(buf, outlen[0])[:]
 
 
 def _encrypt_with_fixed_nonce_len(
     ctx: object,
     nonce: Union[_bytes, bytearray],
@@ -261,41 +250,45 @@
     res = EVP_CipherFinal_ex(ctx, NULL, outlen)
     openssl_assert(res != 0)
     openssl_assert(outlen[0] == 0)
     tag_buf = ffi_new("unsigned char[]", tag_length)
     res = EVP_CIPHER_CTX_ctrl(ctx, EVP_CTRL_AEAD_GET_TAG, tag_length, tag_buf)
     openssl_assert(res != 0)
     tag = ffi_buffer(tag_buf)[:]
-
     return processed_data + tag
 
 
-def _tag_from_data(data: _bytes, tag_length: int) -> _bytes:
-    if len(data) < tag_length:
-        raise InvalidTag
-    return data[-tag_length:]
-
-
 def _decrypt_with_fixed_nonce_len(
     ctx: object,
     nonce: Union[_bytes, bytearray],
     data: _bytes,
     associated_data: _bytes,
     tag_length: int,
 ) -> bytes:
-    tag = _tag_from_data(data, tag_length)
-    data = data[:-tag_length]
+    if len(data) < tag_length:
+        raise InvalidTag
+    negative_tag_length = -tag_length
+    tag = data[negative_tag_length:]
+    data = data[:negative_tag_length]
     _set_nonce(ctx, nonce, _DECRYPT)
-    _set_decrypt_tag(ctx, tag)
+    # set the decrypted tag
+    res = EVP_CIPHER_CTX_ctrl(ctx, EVP_CTRL_AEAD_SET_TAG, tag_length, tag)
+    openssl_assert(res != 0)
     return _decrypt_data(ctx, data, associated_data)
 
 
 def _decrypt_data(ctx: object, data: _bytes, associated_data: _bytes) -> _bytes:
     _process_aad(ctx, associated_data)
     processed_data = _process_data(ctx, data)
     outlen = ffi_new("int *")
     res = EVP_CipherFinal_ex(ctx, NULL, outlen)
     if res == 0:
         backend._consume_errors()
         raise InvalidTag
 
     return processed_data
+
+
+def openssl_assert(ok: bool) -> None:
+    """Raise an exception if OpenSSL returns an error."""
+    if not ok:
+        openssl_failure()
```

### Comparing `chacha20poly1305_reuseable-0.2.5/setup.py` & `chacha20poly1305_reuseable-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=36.0.2']
 
 setup_kwargs = {
     'name': 'chacha20poly1305-reuseable',
-    'version': '0.2.5',
+    'version': '0.3.0',
     'description': 'ChaCha20Poly1305 that is reuseable for asyncio',
     'long_description': '# chacha20poly1305_reuseable\n\n<p align="center">\n  <a href="https://github.com/bdraco/chacha20poly1305-reuseable/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bdraco/chacha20poly1305-reuseable/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/chacha20poly1305-reuseable">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/chacha20poly1305-reuseable.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/chacha20poly1305-reuseable/">\n    <img src="https://img.shields.io/pypi/v/chacha20poly1305-reuseable.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/chacha20poly1305-reuseable.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/chacha20poly1305-reuseable.svg?style=flat-square" alt="License">\n</p>\n\nChaCha20Poly1305 that is reuseable for asyncio\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install chacha20poly1305-reuseable`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/bdraco"><img src="https://avatars.githubusercontent.com/u/663432?v=4?s=80" width="80px;" alt=""/><br /><sub><b>J. Nick Koston</b></sub></a><br /><a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Code">💻</a> <a href="#ideas-bdraco" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Documentation">📖</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/chacha20poly1305-reuseable',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['chacha20poly1305_reuseable'] package_data = \ {'': ['*']}
 install_requires = \ ['cryptography>=36.0.2'] setup_kwargs = { 'name':
-'chacha20poly1305-reuseable', 'version': '0.2.5', 'description':
+'chacha20poly1305-reuseable', 'version': '0.3.0', 'description':
 'ChaCha20Poly1305 that is reuseable for asyncio', 'long_description': '#
 chacha20poly1305_reuseable\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `chacha20poly1305_reuseable-0.2.5/PKG-INFO` & `chacha20poly1305_reuseable-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chacha20poly1305-reuseable
-Version: 0.2.5
+Version: 0.3.0
 Summary: ChaCha20Poly1305 that is reuseable for asyncio
 Home-page: https://github.com/bdraco/chacha20poly1305-reuseable
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.2.5 Summary:
+Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.3.0 Summary:
 ChaCha20Poly1305 that is reuseable for asyncio Home-page: https://github.com/
 bdraco/chacha20poly1305-reuseable License: Apache Software License 2.0 Author:
 J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

