# Comparing `tmp/exception-reports-1.1.0.tar.gz` & `tmp/exception_reports-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exception-reports-1.1.0.tar", last modified: Mon Oct  1 06:23:52 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

