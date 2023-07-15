# Comparing `tmp/mispr-0.0.2.tar.gz` & `tmp/mispr-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mispr-0.0.2.tar", last modified: Fri Jan 14 05:54:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

