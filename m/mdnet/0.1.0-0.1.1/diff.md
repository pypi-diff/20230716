# Comparing `tmp/mdnet-0.1.0.tar.gz` & `tmp/mdnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdnet-0.1.0.tar", last modified: Sun Jul 16 11:15:01 2023, max compression
+gzip compressed data, was "mdnet-0.1.1.tar", last modified: Sun Jul 16 12:23:50 2023, max compression
```

## Comparing `mdnet-0.1.0.tar` & `mdnet-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 11:15:01.387604 mdnet-0.1.0/
--rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 11:15:01.387604 mdnet-0.1.0/PKG-INFO
--rw-r--r--   0 gnat      (1000) gnat      (1000)     1738 2023-07-16 10:55:14.000000 mdnet-0.1.0/README.md
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 11:15:01.386604 mdnet-0.1.0/mdnet/
--rw-r--r--   0 gnat      (1000) gnat      (1000)     2050 2023-07-16 10:58:49.000000 mdnet-0.1.0/mdnet/mdnet.py
--rw-r--r--   0 gnat      (1000) gnat      (1000)      303 2023-07-16 10:59:54.000000 mdnet-0.1.0/mdnet/setup.py
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 11:15:01.387604 mdnet-0.1.0/mdnet.egg-info/
--rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/PKG-INFO
--rw-r--r--   0 gnat      (1000) gnat      (1000)      215 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/SOURCES.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)        1 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/dependency_links.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       43 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/entry_points.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       35 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/requires.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)        6 2023-07-16 11:15:01.000000 mdnet-0.1.0/mdnet.egg-info/top_level.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       38 2023-07-16 11:15:01.387604 mdnet-0.1.0/setup.cfg
+drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.395879 mdnet-0.1.1/
+-rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 12:23:50.394879 mdnet-0.1.1/PKG-INFO
+-rw-r--r--   0 gnat      (1000) gnat      (1000)     2502 2023-07-16 12:21:28.000000 mdnet-0.1.1/README.md
+drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.394879 mdnet-0.1.1/mdnet/
+-rw-r--r--   0 gnat      (1000) gnat      (1000)     2133 2023-07-16 12:13:07.000000 mdnet-0.1.1/mdnet/mdnet.py
+-rw-r--r--   0 gnat      (1000) gnat      (1000)      303 2023-07-16 12:17:34.000000 mdnet-0.1.1/mdnet/setup.py
+drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.394879 mdnet-0.1.1/mdnet.egg-info/
+-rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/PKG-INFO
+-rw-r--r--   0 gnat      (1000) gnat      (1000)      215 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/SOURCES.txt
+-rw-r--r--   0 gnat      (1000) gnat      (1000)        1 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/dependency_links.txt
+-rw-r--r--   0 gnat      (1000) gnat      (1000)       43 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/entry_points.txt
+-rw-r--r--   0 gnat      (1000) gnat      (1000)       35 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/requires.txt
+-rw-r--r--   0 gnat      (1000) gnat      (1000)        6 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/top_level.txt
+-rw-r--r--   0 gnat      (1000) gnat      (1000)       38 2023-07-16 12:23:50.395879 mdnet-0.1.1/setup.cfg
```

### Comparing `mdnet-0.1.0/README.md` & `mdnet-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -27,26 +27,41 @@
 The templates should be Jinja2 templates. The post template will be rendered with the following variables:
 - 'title': The title of the post
 - 'date': the date of the post
 - 'content': the content of the post
 
 The index template will be rendered with a posts variable, which is a list of dictionaries. Each dictionary contains the 'title', 'date', and 'file' (filename) of a post.
 
+## Writing Posts
+Posts should be written in Markdown and include YAML Front Matter. Front Matter is a block of YAML at the top of the file that is used for storing metadata about the file. Here's an example of a post:
+```
+---
+title: My First Post
+date: 2023-07-14
+tldr: This is a short description of my post.
+---
+# My First Post
+
+This is the content of my post. You can write anything you want here, in Markdown format.
+```
+
+In this example, the Front Matter is the part between the '---' lines. It includes a 'title', a 'date', and a 'tldr' summary. These values will be used to populate the template when generating the HTML file.
+
+The rest of the file, after the second '---', is the content of the post. This should be written in Markdown, and it will be converted to HTML when generating the site.
+
 ## Example
 Here's an example of how you might structure your project:
+```
 my_blog/
-    mdnet/
-        __init__.py
-        mdnet.py
     templates/
         post.html
         index.html
     posts/
         post1.md
         post2.md
     output/
-
+```
 You can generate the site with this command:
 ```
 mdnet posts output templates/post.html templates/index.html
 ```
 This will generate HTML files in the output directory.
```

### Comparing `mdnet-0.1.0/mdnet/mdnet.py` & `mdnet-0.1.1/mdnet/mdnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,27 @@
     return template.render(title=metadata['title'], date=metadata['date'], content=content)
 
 def render_index(template_path, posts):
     template = get_template(template_path)
     return template.render(posts=posts)
 
 def generate_site(input_dir, output_dir, template_path, index_path):
+    posts_dir = output_dir / 'posts'
+    posts_dir.mkdir(exist_ok=True)
+
     posts = []
     for md_file in Path(input_dir).iterdir():
         if md_file.suffix == ".md":
             post = frontmatter.load(md_file)
-            html_file = output_dir / (post.metadata['title'] + ".html")
+            html_file = posts_dir / (post.metadata['title'] + ".html")
             html_file.write_text(render_template(template_path, post.metadata, convert_md_to_html(post.content)))
             posts.append({'title' : post.metadata['title'], 
                           'date' : post.metadata['date'],
                           'tldr' : post.metadata['tldr'],
-                          'file' : html_file.name})
+                          'file' : 'posts/' + html_file.name})
     
     (output_dir / 'index.html').write_text(render_index(index_path, posts))
 
 def main():
     parser = argparse.ArgumentParser(description="Generate a static site from Markdown files.")
     parser.add_argument("input_dir", help="The directory containing the Markdown files.")
     parser.add_argument("output_dir", help="The directory to output the HTML files to.")
```

