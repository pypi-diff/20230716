# Comparing `tmp/zylo-1.0.9.tar.gz` & `tmp/zylo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.9.tar", last modified: Fri Jul 14 10:04:12 2023, max compression
+gzip compressed data, was "zylo-2.0.0.tar", last modified: Sun Jul 16 18:59:13 2023, max compression
```

## Comparing `zylo-1.0.9.tar` & `zylo-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.013692 zylo-1.0.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 10:04:12.013692 zylo-1.0.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1046 2023-07-14 10:03:34.000000 zylo-1.0.9/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-14 10:04:12.013692 zylo-1.0.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-07-14 10:00:37.000000 zylo-1.0.9/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.009692 zylo-1.0.9/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-14 08:14:27.000000 zylo-1.0.9/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-07-14 10:02:42.000000 zylo-1.0.9/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-07-14 06:36:57.000000 zylo-1.0.9/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-14 06:48:09.000000 zylo-1.0.9/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-1.0.9/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2346 2023-07-14 06:25:13.000000 zylo-1.0.9/zylo/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.9/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.9/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.009692 zylo-1.0.9/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-16 18:59:13.629248 zylo-2.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-07-16 18:59:13.629248 zylo-2.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4709 2023-07-16 18:55:41.000000 zylo-2.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-16 18:59:13.629248 zylo-2.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-07-16 18:58:32.000000 zylo-2.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-16 18:59:13.625251 zylo-2.0.0/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-14 08:14:27.000000 zylo-2.0.0/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-07-14 10:05:50.000000 zylo-2.0.0/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5828 2023-07-16 18:46:56.000000 zylo-2.0.0/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1793 2023-07-16 18:47:12.000000 zylo-2.0.0/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-2.0.0/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-16 18:57:34.000000 zylo-2.0.0/zylo/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-2.0.0/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-16 18:47:33.000000 zylo-2.0.0/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-16 18:59:13.629248 zylo-2.0.0/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-07-16 18:59:13.000000 zylo-2.0.0/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-16 18:59:13.000000 zylo-2.0.0/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-16 18:59:13.000000 zylo-2.0.0/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-16 18:59:13.000000 zylo-2.0.0/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-16 18:59:13.000000 zylo-2.0.0/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.9/setup.py` & `zylo-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.9',
+    version='2.0.0',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
-    install_requires=['werkzeug', 'jinja2', 'cryptography', 'zylo-admin'],  
+    install_requires=['werkzeug', 'jinja2', 'cryptography', 'zylo-admin', 'itsdangerous'],  
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `zylo-1.0.9/zylo/JwT.py` & `zylo-2.0.0/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.9/zylo/app.py` & `zylo-2.0.0/zylo/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,167 @@
-import json
+import os
+import base64
 from werkzeug.wrappers import Request, Response
 from werkzeug.routing import Map, Rule
-from werkzeug.exceptions import HTTPException, default_exceptions, NotFound, MethodNotAllowed
+from werkzeug.exceptions import HTTPException, NotFound
+from werkzeug.middleware.shared_data import SharedDataMiddleware
+from werkzeug.debug import DebuggedApplication
 from jinja2 import Environment, FileSystemLoader
-from .sessions import SessionManager
+from sessions import session_manager
+from blueprint import Blueprint
 from werkzeug.urls import url_encode
-from .limiter import Limiter
-import os
+from itsdangerous import URLSafeTimedSerializer
+import json
 import mimetypes
 
+# Create the application
 class Zylo:
-    def __init__(self, __name__={} ):
+    def __init__(self, __name__=None):
+        self.template_folder='views'
         self.url_map = Map()
-        self.routes = {}
-        self.template_env = Environment(loader=FileSystemLoader('views'))
-        self.static_folder = 'static'
-        self.session_manager = SessionManager()
+        self.static_folder = "static"
+        self.error_handlers = {}
+        self.middlewares = []
+        self.template_env = Environment(loader=FileSystemLoader(self.template_folder))
+        self.host = 'localhost'
+        self.port = 8000
+        self.debug = True
+        self.secret_key = os.urandom(24)
+        self.serializer = URLSafeTimedSerializer(base64.urlsafe_b64encode(self.secret_key))
         self.blueprints = []
-        self.template_folder = None
-        self.limiter = Limiter()
-        self.before_request_funcs = []
-        self.after_request_funcs = []
         self.__name__ = __name__
 
-    def route(self, rule, methods=['GET'], endpoint=None,):
-        def decorator(func):
-            self.routes[endpoint or func.__name__] = (rule, methods, func)
-            return func
+    def add_url_rule(self, rule, endpoint, handler, methods=['GET']):
+        def view_func(request, **values):
+            return handler(request, **values)
+        self.url_map.add(Rule(rule, endpoint=endpoint, methods=methods))
+        setattr(self, endpoint, view_func)
+
+
+    def route(self, rule, methods=['GET']):
+        def decorator(handler):
+            self.add_url_rule(rule, handler.__name__, handler, methods)
+            return handler
+
         return decorator
 
-    def register_blueprint(self, blueprint):
-        self.blueprints.append(blueprint)
-        blueprint.register(self)
-        
+    def errorhandler(self, code):
+        def decorator(handler):
+            self.error_handlers[code] = handler
+            return handler
+
+        return decorator
+
+    def use(self, middleware):
+        self.middlewares.append(middleware)
+
     def url_for_static(self, filename):
         return f'/static/{filename}'
-    
+
     def serve_static(self, filename):
         static_path = os.path.join(self.static_folder, filename)
         if os.path.isfile(static_path):
             mimetype, _ = mimetypes.guess_type(static_path)
             if mimetype:
                 return Response(open(static_path, 'rb').read(), mimetype=mimetype)
         raise NotFound()
-    
-    def before_request(self, func):
-        self.before_request_funcs.append(func)
-        return func
-
-    def after_request(self, func):
-        self.after_request_funcs.append(func)
-        return func
-
-    def run(self, host='localhost', port=8000, debug=True):
-        app = self
-        host = host
-        port = port
-        debug = debug
-
-        @Request.application
-        def application(request):
-            try:
-                session_token = request.cookies.get('session_token')
-                session_data = app.session_manager.get_session(session_token)
-                request.session = session_data
-
-                adapter = app.url_map.bind_to_environ(request.environ)
-                try:
-                    endpoint, values = adapter.match()
-                except NotFound:
-                    for blueprint in app.blueprints:
-                        adapter = blueprint.url_map.bind_to_environ(request.environ)
-                        try:
-                            endpoint, values = adapter.match()
-                            break
-                        except NotFound:
-                            pass
-                    else:
-                        raise
-                rule, methods, func = app.routes[endpoint]
-                if request.method not in methods:
-                    raise MethodNotAllowed(valid_methods=methods)
-
-                if hasattr(request, 'session'):
-                    if not session_token or not session_data:
-                        session_token = app.session_manager.create_session()
-                        session_data = {}
-                        request.session = session_data
-                        response = func(request, **values)
-                        response.set_cookie('session_token', session_token)
-                    else:
-                        response = func(request, **values)
 
-                    app.session_manager.update_session(session_token, request.session)
-
-                return response
+    def register_blueprint(self, blueprint):
+        self.blueprints.append(blueprint)
 
-            except HTTPException as e:
-                return e
+    def handle_request(self, request):
+        adapter = self.url_map.bind_to_environ(request.environ)
+        try:
+            endpoint, values = adapter.match()
+            handler = getattr(self, endpoint)
+            response = handler(request, **values)
+        except NotFound as e:
+            response = self.handle_error(404, e, request)
+        except HTTPException as e:
+            response = e
+        return response
 
-        if debug:
-            from werkzeug.debug import DebuggedApplication
-            application = DebuggedApplication(application, evalex=True)
-
-        for endpoint, (rule, _, _) in self.routes.items():
-            self.url_map.add(Rule(rule, endpoint=endpoint))
-            print(f"Registered route: {rule} --> {endpoint}")
+    def handle_error(self, code, error, request):
+        handler = self.error_handlers.get(code)
+        if handler:
+            return handler(error, request)
+        else:
+            return error
 
+    def wsgi_app(self, environ, start_response):
+        request = Request(environ)
         for blueprint in self.blueprints:
-            blueprint.register(self)
+            if request.path.startswith(blueprint.url_prefix):
+                request.blueprint = blueprint
+                response = blueprint.wsgi_app(environ, start_response)
+                return response
+        session_id = request.cookies.get('session_id')
+        session_data = session_manager.load_session(session_id)
+        request.session = session_data
+        response = self.handle_request(request)
+        session_id = session_manager.save_session(request.session)
+        response.set_cookie('session_id', session_id, secure=True, httponly=True)
+        return response(environ, start_response)
+
+    def __call__(self, environ, start_response):
+        app = self.wsgi_app
+        for middleware in reversed(self.middlewares):
+            app = middleware(app)
+        return app(environ, start_response)
+
+    def run(self, host=None, port=None, debug=None, secret_key=None):
+        if host is not None:
+            self.host = host
+        if port is not None:
+            self.port = port
+        if debug is not None:
+            self.debug = debug
+        if secret_key is not None:
+            self.secret_key = secret_key
+
+        if self.debug:
+            app = DebuggedApplication(self, evalex=True)
+        else:
+            app = self
 
         from werkzeug.serving import run_simple
-        run_simple(host, port, application, use_reloader=debug)
+        run_simple(self.host, self.port, app, use_reloader=True)
 
 app = Zylo()
 
 def render_template(template_name, **kwargs):
     template = app.template_env.get_template(template_name)
     kwargs['url_for_static'] = app.url_for_static
     return Response(template.render(**kwargs), mimetype='text/html')
 
 def jsonify(data):
-    response = Response()
-    response.headers['Content-Type'] = 'application/json'
-    response.data = json.dumps(data)
-    return response
-
-def redirect(location):
-    response = Response()
-    response.status_code = 302
-    response.headers['Location'] = location
-    return response
-
-def url_for(endpoint):
-    rule, _, _ = app.routes[endpoint]
-    url_map = app.url_map.bind(app.host, app.port)
-    return url_map.build(rule, force_external=True)
+    json_data = json.dumps(data)
+    return Response(json_data, mimetype='application/json')
 
-def redirect_args(location, **kwargs):
-    url = location
-    if kwargs:
-        query_params = url_encode(kwargs)
-        url += f'?{query_params}'
-    return Response(status=302, headers={'Location': url})
+def redirect(location, code=302):
+    return Response('', status=code, headers={'Location': location})
 
-def send_file(filename, mimetype=None, as_attachment=False):
-    response = Response()
-    response.headers['Content-Disposition'] = f'attachment; filename="{filename}"' if as_attachment else f'inline; filename="{filename}"'
-    if mimetype is not None:
-        response.headers['Content-Type'] = mimetype
-    return response
+def url_for(endpoint, **values):
+    return app.url_map.build(endpoint, values)
 
-def static_engine(static_folder):
-    app.static_folder = static_folder
+def send_file(filename, mimetype):
+    with open(filename, 'rb') as f:
+        content = f.read()
+    headers = {'Content-Type': mimetype, 'Content-Disposition': f'attachment; filename={os.path.basename(filename)}'}
+    return Response(content, headers=headers)
 
+def static_engine(static_folder):
+    app.wsgi_app = SharedDataMiddleware(app.wsgi_app, {'/static': static_folder})
 
 def template_engine(template_folder):
-    app.template_folder = template_folder
     app.template_env = Environment(loader=FileSystemLoader(template_folder))
 
-# Add Werkzeug's default error handlers
-for code in default_exceptions:
-    handler = default_exceptions[code]
-
-    def error_handler(error):
-        response = Response()
-        response.status_code = error.code
-        response.data = f'{error.code} {error.name}'
-        return response
-
-    handler = error_handler
+def save_json_file(data, filename):
+    with open(filename, 'w') as f:
+        json.dump(data, f)
 
+def redirect_args(location, **kwargs):
+    url = location
+    if kwargs:
+        query_params = url_encode(kwargs)
+        url += f'?{query_params}'
+    return Response(status=302, headers={'Location': url})
```

### Comparing `zylo-1.0.9/zylo/chiper.py` & `zylo-2.0.0/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.9/zylo/mailer.py` & `zylo-2.0.0/zylo/mailer.py`

 * *Files identical despite different names*

