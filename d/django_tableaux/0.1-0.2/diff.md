# Comparing `tmp/django_tableaux-0.1.tar.gz` & `tmp/django_tableaux-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tableaux-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_tableaux-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_tableaux-0.1.tar` & `django_tableaux-0.2.tar`

### file list

```diff
@@ -1,42 +1,48 @@
--rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.1/.gitignore
--rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.1/LICENSE
--rw-r--r--   0        0        0     1113 2023-07-15 16:59:49.675807 django_tableaux-0.1/README.rst
--rw-r--r--   0        0        0     1121 2023-07-15 17:05:45.177989 django_tableaux-0.1/django_tableaux/__init__.py
--rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.1/django_tableaux/apps.py
--rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.1/django_tableaux/buttons.py
--rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.1/django_tableaux/columns.py
--rw-r--r--   0        0        0     7282 2023-07-15 11:12:22.982745 django_tableaux-0.1/django_tableaux/static/django_tableaux/js/django_tableaux.js
--rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/_alert.html
--rw-r--r--   0        0        0      717 2023-07-15 11:12:22.983745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_content.html
--rw-r--r--   0        0        0      990 2023-07-15 11:12:22.983745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_head.html
--rw-r--r--   0        0        0      614 2023-07-15 11:12:22.983745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_table.html
--rw-r--r--   0        0        0     3308 2023-07-15 11:12:22.984745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/bootstrap4.html
--rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/bootstrap5_base.html
--rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/button.html
--rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/cell_error.html
--rw-r--r--   0        0        0      345 2023-07-15 11:12:22.984745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/cell_form.html
--rw-r--r--   0        0        0     1355 2023-07-15 11:12:22.985745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
--rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/filter_settings.html
--rw-r--r--   0        0        0     1005 2023-07-15 11:12:22.985745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/filter_toolbar.html
--rw-r--r--   0        0        0     1348 2023-07-15 11:12:22.985745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_base.html
--rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_filter.html
--rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_form.html
--rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/paginator.html
--rw-r--r--   0        0        0        0 2023-07-15 11:12:22.986745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/render_row_mobile.html
--rw-r--r--   0        0        0     3103 2023-07-15 11:12:22.987744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/render_rows.html
--rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/render_table_data.html
--rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/select_checkbox.html
--rw-r--r--   0        0        0     1136 2023-07-15 11:12:22.987744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/tables_pro.html
--rw-r--r--   0        0        0     1151 2023-07-15 11:12:22.988745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_actions.html
--rw-r--r--   0        0        0      150 2023-07-15 11:12:22.988745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
--rw-r--r--   0        0        0     1095 2023-07-15 11:12:22.988745 django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_columns.html
--rw-r--r--   0        0        0      579 2023-07-15 11:12:22.989744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_rows.html
--rw-r--r--   0        0        0      514 2023-07-15 11:12:22.989744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/main.html
--rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.1/django_tableaux/templates/django_tableaux/width_request.html
--rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.1/django_tableaux/templatetags/__init__.py
--rw-r--r--   0        0        0      626 2023-07-15 11:12:22.990745 django_tableaux-0.1/django_tableaux/templatetags/django_tableaux.py
--rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.1/django_tableaux/tests.py
--rw-r--r--   0        0        0     3697 2023-07-15 11:12:22.991745 django_tableaux-0.1/django_tableaux/utils.py
--rw-r--r--   0        0        0    18303 2023-07-15 11:12:22.991745 django_tableaux-0.1/django_tableaux/views.py
--rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.1/pyproject.toml
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_tableaux-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.2/.gitignore
+-rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.2/LICENSE
+-rw-r--r--   0        0        0     1113 2023-07-15 16:59:49.675807 django_tableaux-0.2/README.rst
+-rw-r--r--   0        0        0     1121 2023-07-16 08:01:26.633734 django_tableaux-0.2/django_tableaux/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.2/django_tableaux/apps.py
+-rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.2/django_tableaux/buttons.py
+-rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.2/django_tableaux/columns.py
+-rw-r--r--   0        0        0     7282 2023-07-15 11:12:22.982745 django_tableaux-0.2/django_tableaux/static/django_tableaux/js/django_tableaux.js
+-rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/_alert.html
+-rw-r--r--   0        0        0      717 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_content.html
+-rw-r--r--   0        0        0      990 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_head.html
+-rw-r--r--   0        0        0      614 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_table.html
+-rw-r--r--   0        0        0     3308 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap4.html
+-rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap5_base.html
+-rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/button.html
+-rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/cell_error.html
+-rw-r--r--   0        0        0      345 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/cell_form.html
+-rw-r--r--   0        0        0     1355 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
+-rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_settings.html
+-rw-r--r--   0        0        0     1005 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_toolbar.html
+-rw-r--r--   0        0        0     1348 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_base.html
+-rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_filter.html
+-rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_form.html
+-rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/paginator.html
+-rw-r--r--   0        0        0        0 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_row_mobile.html
+-rw-r--r--   0        0        0     3103 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_rows.html
+-rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_table_data.html
+-rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/select_checkbox.html
+-rw-r--r--   0        0        0     1136 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/tables_pro.html
+-rw-r--r--   0        0        0     1151 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_actions.html
+-rw-r--r--   0        0        0      150 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
+-rw-r--r--   0        0        0     1095 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_columns.html
+-rw-r--r--   0        0        0      579 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_rows.html
+-rw-r--r--   0        0        0      514 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/main.html
+-rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/width_request.html
+-rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templatetags/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-15 11:12:22.990745 django_tableaux-0.2/django_tableaux/templatetags/django_tableaux.py
+-rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.2/django_tableaux/tests.py
+-rw-r--r--   0        0        0     3697 2023-07-15 11:12:22.991745 django_tableaux-0.2/django_tableaux/utils.py
+-rw-r--r--   0        0        0    18303 2023-07-15 11:12:22.991745 django_tableaux-0.2/django_tableaux/views.py
+-rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.2/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-07-16 07:29:21.544621 django_tableaux-0.2/tables/manage.py
+-rw-r--r--   0        0        0        0 2023-07-16 07:29:20.892757 django_tableaux-0.2/tables/tables/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-16 07:29:21.547623 django_tableaux-0.2/tables/tables/asgi.py
+-rw-r--r--   0        0        0     3376 2023-07-16 07:29:31.315465 django_tableaux-0.2/tables/tables/settings.py
+-rw-r--r--   0        0        0      784 2023-07-16 07:29:21.554622 django_tableaux-0.2/tables/tables/urls.py
+-rw-r--r--   0        0        0      405 2023-07-16 07:29:21.554622 django_tableaux-0.2/tables/tables/wsgi.py
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_tableaux-0.2/PKG-INFO
```

### Comparing `django_tableaux-0.1/.gitignore` & `django_tableaux-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/LICENSE` & `django_tableaux-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/README.rst` & `django_tableaux-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/__init__.py` & `django_tableaux-0.2/django_tableaux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 * Edit specific fields directly inside the table
 * Easy integration with generic views for CRUD operations
 
 The project is still in beta but is fully usable.
 
 Full documentation to follow.
 """
-__version__ = "0.1"
+__version__ = "0.2"
```

### Comparing `django_tableaux-0.1/django_tableaux/buttons.py` & `django_tableaux-0.2/django_tableaux/buttons.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/columns.py` & `django_tableaux-0.2/django_tableaux/columns.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/static/django_tableaux/js/django_tableaux.js` & `django_tableaux-0.2/django_tableaux/static/django_tableaux/js/django_tableaux.js`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_content.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_content.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_head.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_head.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/block_table.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_table.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/bootstrap4.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/bootstrap5_base.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap5_base.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/custom_bootstrap4.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/custom_bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/filter_toolbar.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_toolbar.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_base.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_base.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_filter.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_filter.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/modal_form.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_form.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/paginator.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/paginator.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/render_rows.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_rows.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/tables_pro.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/tables_pro.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_actions.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_actions.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_columns.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_columns.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/_rows.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_rows.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templates/django_tableaux/toolbar/main.html` & `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/main.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/templatetags/django_tableaux.py` & `django_tableaux-0.2/django_tableaux/templatetags/django_tableaux.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/tests.py` & `django_tableaux-0.2/django_tableaux/tests.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/utils.py` & `django_tableaux-0.2/django_tableaux/utils.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/django_tableaux/views.py` & `django_tableaux-0.2/django_tableaux/views.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.1/PKG-INFO` & `django_tableaux-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tableaux
-Version: 0.1
+Version: 0.2
 Summary: Django_tableaux: Django tables with Advanced User eXperience
 Author-email: Ian Stewart <is@iskt.co.uk>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/ianastewart/django_tableaux/
 
 ===============
```

