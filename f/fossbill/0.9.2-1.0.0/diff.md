# Comparing `tmp/fossbill-0.9.2-py3-none-any.whl.zip` & `tmp/fossbill-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,55 +1,66 @@
-Zip file size: 65847 bytes, number of entries: 53
--rw-r--r--  2.0 unx     1504 b- defN 23-Jul-07 10:16 fossbill/__init__.py
--rw-r--r--  2.0 unx     3177 b- defN 23-Jul-07 10:16 fossbill/alembic.ini
--rw-r--r--  2.0 unx    11111 b- defN 23-Jul-07 10:16 fossbill/auth.py
--rw-r--r--  2.0 unx    28284 b- defN 23-Jul-07 10:16 fossbill/bill.py
--rw-r--r--  2.0 unx     5102 b- defN 23-Jul-07 10:16 fossbill/client.py
--rw-r--r--  2.0 unx     9311 b- defN 23-Jul-07 10:16 fossbill/database.py
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-07 10:16 fossbill/landing.py
--rw-r--r--  2.0 unx     9272 b- defN 23-Jul-07 10:16 fossbill/payment.py
--rw-r--r--  2.0 unx     6679 b- defN 23-Jul-07 10:16 fossbill/product.py
--rw-r--r--  2.0 unx    12061 b- defN 23-Jul-07 10:16 fossbill/user.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Jul-07 10:16 fossbill/alembic/env.py
--rw-r--r--  2.0 unx      510 b- defN 23-Jul-07 10:16 fossbill/alembic/script.py.mako
--rw-r--r--  2.0 unx     7758 b- defN 23-Jul-07 10:16 fossbill/alembic/versions/fda694e67f67_init.py
--rw-r--r--  2.0 unx      450 b- defN 23-Jul-07 10:17 fossbill/locale/en_US/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx    16388 b- defN 23-Jul-07 10:17 fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx      259 b- defN 23-Jul-07 10:16 fossbill/static/bill.css
--rw-r--r--  2.0 unx     2164 b- defN 23-Jul-07 10:16 fossbill/static/style.css
--rw-r--r--  2.0 unx     1331 b- defN 23-Jul-07 10:16 fossbill/templates/base.html
--rw-r--r--  2.0 unx     1588 b- defN 23-Jul-07 10:16 fossbill/templates/macros.html
--rw-r--r--  2.0 unx      395 b- defN 23-Jul-07 10:16 fossbill/templates/auth/ask_reset_password.html
--rw-r--r--  2.0 unx      670 b- defN 23-Jul-07 10:16 fossbill/templates/auth/login.html
--rw-r--r--  2.0 unx      538 b- defN 23-Jul-07 10:16 fossbill/templates/auth/register.html
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 10:16 fossbill/templates/auth/reset_password_email.plain
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-07 10:16 fossbill/templates/auth/use_reset_password.html
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-07 10:16 fossbill/templates/bill/bill_email.plain
--rw-r--r--  2.0 unx      598 b- defN 23-Jul-07 10:16 fossbill/templates/bill/create.html
--rw-r--r--  2.0 unx     1247 b- defN 23-Jul-07 10:16 fossbill/templates/bill/generated_bill.html
--rw-r--r--  2.0 unx     2384 b- defN 23-Jul-07 10:16 fossbill/templates/bill/generated_quote.html
--rw-r--r--  2.0 unx     5373 b- defN 23-Jul-07 10:16 fossbill/templates/bill/index.html
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-07 10:16 fossbill/templates/bill/quote_email.plain
--rw-r--r--  2.0 unx      732 b- defN 23-Jul-07 10:16 fossbill/templates/bill/send_bill_email.html
--rw-r--r--  2.0 unx      733 b- defN 23-Jul-07 10:16 fossbill/templates/bill/send_quote_email.html
--rw-r--r--  2.0 unx     7949 b- defN 23-Jul-07 10:16 fossbill/templates/bill/update.html
--rw-r--r--  2.0 unx     1039 b- defN 23-Jul-07 10:16 fossbill/templates/bill/update_bill.html
--rw-r--r--  2.0 unx     3428 b- defN 23-Jul-07 10:16 fossbill/templates/bill/update_quote.html
--rw-r--r--  2.0 unx     1193 b- defN 23-Jul-07 10:16 fossbill/templates/client/create.html
--rw-r--r--  2.0 unx     1981 b- defN 23-Jul-07 10:16 fossbill/templates/client/index.html
--rw-r--r--  2.0 unx     1553 b- defN 23-Jul-07 10:16 fossbill/templates/client/update.html
--rw-r--r--  2.0 unx      836 b- defN 23-Jul-07 10:16 fossbill/templates/landing/dashboard.html
--rw-r--r--  2.0 unx     1194 b- defN 23-Jul-07 10:16 fossbill/templates/landing/welcome.html
--rw-r--r--  2.0 unx     3308 b- defN 23-Jul-07 10:16 fossbill/templates/payment/home.html
--rw-r--r--  2.0 unx     1381 b- defN 23-Jul-07 10:16 fossbill/templates/payment/invoice.html
--rw-r--r--  2.0 unx     1155 b- defN 23-Jul-07 10:16 fossbill/templates/product/create.html
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-07 10:16 fossbill/templates/product/index.html
--rw-r--r--  2.0 unx     1492 b- defN 23-Jul-07 10:16 fossbill/templates/product/update.html
--rw-r--r--  2.0 unx      630 b- defN 23-Jul-07 10:16 fossbill/templates/user/import_export_user.html
--rw-r--r--  2.0 unx       91 b- defN 23-Jul-07 10:16 fossbill/templates/user/test_email.plain
--rw-r--r--  2.0 unx     6041 b- defN 23-Jul-07 10:16 fossbill/templates/user/update.html
--rw-r--r--  2.0 unx    34523 b- defN 23-Jul-07 10:18 fossbill-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-07 10:18 fossbill-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 10:18 fossbill-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-07 10:18 fossbill-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4749 b- defN 23-Jul-07 10:18 fossbill-0.9.2.dist-info/RECORD
-53 files, 208126 bytes uncompressed, 58195 bytes compressed:  72.0%
+Zip file size: 75605 bytes, number of entries: 64
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jul-16 09:41 fossbill/__init__.py
+-rw-r--r--  2.0 unx     3177 b- defN 23-Jul-16 09:41 fossbill/alembic.ini
+-rw-r--r--  2.0 unx    11367 b- defN 23-Jul-16 09:41 fossbill/auth.py
+-rw-r--r--  2.0 unx    28130 b- defN 23-Jul-16 09:41 fossbill/bill.py
+-rw-r--r--  2.0 unx     5399 b- defN 23-Jul-16 09:41 fossbill/customer.py
+-rw-r--r--  2.0 unx     9672 b- defN 23-Jul-16 09:41 fossbill/database.py
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-16 09:41 fossbill/landing.py
+-rw-r--r--  2.0 unx    12464 b- defN 23-Jul-16 09:41 fossbill/me.py
+-rw-r--r--  2.0 unx    10699 b- defN 23-Jul-16 09:41 fossbill/payment.py
+-rw-r--r--  2.0 unx     6880 b- defN 23-Jul-16 09:41 fossbill/product.py
+-rw-r--r--  2.0 unx     3160 b- defN 23-Jul-16 09:41 fossbill/user.py
+-rw-r--r--  2.0 unx     1836 b- defN 23-Jul-16 09:41 fossbill/alembic/env.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jul-16 09:41 fossbill/alembic/script.py.mako
+-rw-r--r--  2.0 unx      704 b- defN 23-Jul-16 09:41 fossbill/alembic/versions/21487ff4ab8c_store_receipt_url_in_payment.py
+-rw-r--r--  2.0 unx      492 b- defN 23-Jul-16 09:41 fossbill/alembic/versions/7899e98936b3_bills_date_to_created_at.py
+-rw-r--r--  2.0 unx     1355 b- defN 23-Jul-16 09:41 fossbill/alembic/versions/ac14f3a73a29_rename_client_to_customer.py
+-rw-r--r--  2.0 unx     7770 b- defN 23-Jul-16 09:41 fossbill/alembic/versions/fda694e67f67_init.py
+-rw-r--r--  2.0 unx      800 b- defN 23-Jul-16 09:41 fossbill/alembic/versions/ff51555aa2ba_add_date_on_bills_and_quotes.py
+-rw-r--r--  2.0 unx      451 b- defN 23-Jul-16 09:43 fossbill/locale/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx    17250 b- defN 23-Jul-16 09:43 fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx      454 b- defN 23-Jul-16 09:41 fossbill/static/bill.css
+-rw-r--r--  2.0 unx     2711 b- defN 23-Jul-16 09:41 fossbill/static/style.css
+-rw-r--r--  2.0 unx     1744 b- defN 23-Jul-16 09:41 fossbill/templates/base.html
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jul-16 09:41 fossbill/templates/macros.html
+-rw-r--r--  2.0 unx      423 b- defN 23-Jul-16 09:41 fossbill/templates/auth/ask_reset_password.html
+-rw-r--r--  2.0 unx      698 b- defN 23-Jul-16 09:41 fossbill/templates/auth/login.html
+-rw-r--r--  2.0 unx      566 b- defN 23-Jul-16 09:41 fossbill/templates/auth/register.html
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-16 09:41 fossbill/templates/auth/reset_password_email.plain
+-rw-r--r--  2.0 unx      546 b- defN 23-Jul-16 09:41 fossbill/templates/auth/use_reset_password.html
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-16 09:41 fossbill/templates/bill/bill_email.plain
+-rw-r--r--  2.0 unx      642 b- defN 23-Jul-16 09:41 fossbill/templates/bill/create.html
+-rw-r--r--  2.0 unx     2532 b- defN 23-Jul-16 09:41 fossbill/templates/bill/create_row.html
+-rw-r--r--  2.0 unx     1559 b- defN 23-Jul-16 09:41 fossbill/templates/bill/finish.html
+-rw-r--r--  2.0 unx      933 b- defN 23-Jul-16 09:41 fossbill/templates/bill/generated_bill.html
+-rw-r--r--  2.0 unx     2494 b- defN 23-Jul-16 09:41 fossbill/templates/bill/generated_draft.html
+-rw-r--r--  2.0 unx      479 b- defN 23-Jul-16 09:41 fossbill/templates/bill/generated_quote.html
+-rw-r--r--  2.0 unx     6094 b- defN 23-Jul-16 09:41 fossbill/templates/bill/index.html
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-16 09:41 fossbill/templates/bill/quote_email.plain
+-rw-r--r--  2.0 unx      762 b- defN 23-Jul-16 09:41 fossbill/templates/bill/send_bill_email.html
+-rw-r--r--  2.0 unx      763 b- defN 23-Jul-16 09:41 fossbill/templates/bill/send_quote_email.html
+-rw-r--r--  2.0 unx     4494 b- defN 23-Jul-16 09:41 fossbill/templates/bill/update.html
+-rw-r--r--  2.0 unx     1612 b- defN 23-Jul-16 09:41 fossbill/templates/bill/update_bill.html
+-rw-r--r--  2.0 unx     3022 b- defN 23-Jul-16 09:41 fossbill/templates/bill/update_quote.html
+-rw-r--r--  2.0 unx     1147 b- defN 23-Jul-16 09:41 fossbill/templates/bill/update_row.html
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jul-16 09:41 fossbill/templates/customer/create.html
+-rw-r--r--  2.0 unx     2078 b- defN 23-Jul-16 09:41 fossbill/templates/customer/index.html
+-rw-r--r--  2.0 unx     1625 b- defN 23-Jul-16 09:41 fossbill/templates/customer/update.html
+-rw-r--r--  2.0 unx      840 b- defN 23-Jul-16 09:41 fossbill/templates/landing/dashboard.html
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jul-16 09:41 fossbill/templates/landing/welcome.html
+-rw-r--r--  2.0 unx      639 b- defN 23-Jul-16 09:41 fossbill/templates/me/import_export_user.html
+-rw-r--r--  2.0 unx       91 b- defN 23-Jul-16 09:41 fossbill/templates/me/test_email.plain
+-rw-r--r--  2.0 unx     6537 b- defN 23-Jul-16 09:41 fossbill/templates/me/update.html
+-rw-r--r--  2.0 unx      153 b- defN 23-Jul-16 09:41 fossbill/templates/payment/charged_notice.plain
+-rw-r--r--  2.0 unx     3474 b- defN 23-Jul-16 09:41 fossbill/templates/payment/index.html
+-rw-r--r--  2.0 unx     1381 b- defN 23-Jul-16 09:41 fossbill/templates/payment/invoice.html
+-rw-r--r--  2.0 unx     1486 b- defN 23-Jul-16 09:41 fossbill/templates/product/create.html
+-rw-r--r--  2.0 unx     2913 b- defN 23-Jul-16 09:41 fossbill/templates/product/index.html
+-rw-r--r--  2.0 unx     1548 b- defN 23-Jul-16 09:41 fossbill/templates/product/update.html
+-rw-r--r--  2.0 unx     3458 b- defN 23-Jul-16 09:41 fossbill/templates/user/index.html
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jul-16 09:43 fossbill-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-16 09:43 fossbill-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 09:43 fossbill-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-16 09:43 fossbill-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5899 b- defN 23-Jul-16 09:43 fossbill-1.0.0.dist-info/RECORD
+64 files, 229397 bytes uncompressed, 66061 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: fossbill/auth.py
 Comment: 
 
 Filename: fossbill/bill.py
 Comment: 
 
-Filename: fossbill/client.py
+Filename: fossbill/customer.py
 Comment: 
 
 Filename: fossbill/database.py
 Comment: 
 
 Filename: fossbill/landing.py
 Comment: 
 
+Filename: fossbill/me.py
+Comment: 
+
 Filename: fossbill/payment.py
 Comment: 
 
 Filename: fossbill/product.py
 Comment: 
 
 Filename: fossbill/user.py
@@ -30,17 +33,29 @@
 
 Filename: fossbill/alembic/env.py
 Comment: 
 
 Filename: fossbill/alembic/script.py.mako
 Comment: 
 
+Filename: fossbill/alembic/versions/21487ff4ab8c_store_receipt_url_in_payment.py
+Comment: 
+
+Filename: fossbill/alembic/versions/7899e98936b3_bills_date_to_created_at.py
+Comment: 
+
+Filename: fossbill/alembic/versions/ac14f3a73a29_rename_client_to_customer.py
+Comment: 
+
 Filename: fossbill/alembic/versions/fda694e67f67_init.py
 Comment: 
 
+Filename: fossbill/alembic/versions/ff51555aa2ba_add_date_on_bills_and_quotes.py
+Comment: 
+
 Filename: fossbill/locale/en_US/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: fossbill/static/bill.css
@@ -72,17 +87,26 @@
 
 Filename: fossbill/templates/bill/bill_email.plain
 Comment: 
 
 Filename: fossbill/templates/bill/create.html
 Comment: 
 
+Filename: fossbill/templates/bill/create_row.html
+Comment: 
+
+Filename: fossbill/templates/bill/finish.html
+Comment: 
+
 Filename: fossbill/templates/bill/generated_bill.html
 Comment: 
 
+Filename: fossbill/templates/bill/generated_draft.html
+Comment: 
+
 Filename: fossbill/templates/bill/generated_quote.html
 Comment: 
 
 Filename: fossbill/templates/bill/index.html
 Comment: 
 
 Filename: fossbill/templates/bill/quote_email.plain
@@ -99,62 +123,71 @@
 
 Filename: fossbill/templates/bill/update_bill.html
 Comment: 
 
 Filename: fossbill/templates/bill/update_quote.html
 Comment: 
 
-Filename: fossbill/templates/client/create.html
+Filename: fossbill/templates/bill/update_row.html
+Comment: 
+
+Filename: fossbill/templates/customer/create.html
 Comment: 
 
-Filename: fossbill/templates/client/index.html
+Filename: fossbill/templates/customer/index.html
 Comment: 
 
-Filename: fossbill/templates/client/update.html
+Filename: fossbill/templates/customer/update.html
 Comment: 
 
 Filename: fossbill/templates/landing/dashboard.html
 Comment: 
 
 Filename: fossbill/templates/landing/welcome.html
 Comment: 
 
-Filename: fossbill/templates/payment/home.html
+Filename: fossbill/templates/me/import_export_user.html
 Comment: 
 
-Filename: fossbill/templates/payment/invoice.html
+Filename: fossbill/templates/me/test_email.plain
 Comment: 
 
-Filename: fossbill/templates/product/create.html
+Filename: fossbill/templates/me/update.html
 Comment: 
 
-Filename: fossbill/templates/product/index.html
+Filename: fossbill/templates/payment/charged_notice.plain
 Comment: 
 
-Filename: fossbill/templates/product/update.html
+Filename: fossbill/templates/payment/index.html
 Comment: 
 
-Filename: fossbill/templates/user/import_export_user.html
+Filename: fossbill/templates/payment/invoice.html
 Comment: 
 
-Filename: fossbill/templates/user/test_email.plain
+Filename: fossbill/templates/product/create.html
+Comment: 
+
+Filename: fossbill/templates/product/index.html
+Comment: 
+
+Filename: fossbill/templates/product/update.html
 Comment: 
 
-Filename: fossbill/templates/user/update.html
+Filename: fossbill/templates/user/index.html
 Comment: 
 
-Filename: fossbill-0.9.2.dist-info/LICENSE
+Filename: fossbill-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: fossbill-0.9.2.dist-info/METADATA
+Filename: fossbill-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: fossbill-0.9.2.dist-info/WHEEL
+Filename: fossbill-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: fossbill-0.9.2.dist-info/top_level.txt
+Filename: fossbill-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fossbill-0.9.2.dist-info/RECORD
+Filename: fossbill-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fossbill/__init__.py

```diff
@@ -21,27 +21,31 @@
 
     if test_config is None:
         import toml
         app.config.from_file("config.toml", load=toml.load, silent=True)
 
     from . import auth
     app.register_blueprint(auth.bp)
+    auth.setup(app)
 
     from . import product
     app.register_blueprint(product.bp)
 
-    from . import client
-    app.register_blueprint(client.bp)
+    from . import customer
+    app.register_blueprint(customer.bp)
 
     from . import bill
     app.register_blueprint(bill.bp)
 
     from . import user
     app.register_blueprint(user.bp)
 
+    from . import me
+    app.register_blueprint(me.bp)
+
     from . import landing
     app.register_blueprint(landing.bp)
     app.add_url_rule('/', endpoint='home')
 
     from . import payment
     app.register_blueprint(payment.bp)
```

## fossbill/auth.py

```diff
@@ -1,24 +1,48 @@
 import functools
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, session, url_for
 )
+from werkzeug.exceptions import abort
 from werkzeug.security import check_password_hash, generate_password_hash
 from fossbill.database import get_db
 from sqlalchemy import insert, select
 from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 import gettext
 import os
 import uuid
 import smtplib
 from email.message import EmailMessage
 import datetime
+import binascii
 
 bp = Blueprint('auth', __name__, url_prefix='/auth')
 
+def csrf_token():
+    if '_csrf_token' not in session:
+        session['_csrf_token'] = binascii.hexlify(os.urandom(64)).decode()
+    return """<input
+        type='hidden'
+        name='_csrf_token'
+        value='{}' />""".format(session['_csrf_token'])
+
+@bp.before_app_request
+def csrf_required():
+    if current_app.config.get('TESTING'):
+        return
+    if request.method != 'POST':
+        return
+    if not request.form.get('_csrf_token'):
+         abort(403)
+    if request.form.get('_csrf_token') != session.get('_csrf_token'):
+         abort(403)
+
+def setup(app):
+    app.jinja_env.globals['csrf_token'] = csrf_token
+
 def get_system_smtp_server():
     if current_app.config['SMTP_SECURITY'] == "TLS":
         server = smtplib.SMTP_SSL(
             host=current_app.config['SMTP_HOST'],
             port=current_app.config['SMTP_PORT'],
             timeout=10
         )
@@ -134,41 +158,26 @@
 
         if error is not None:
             flash(error)
         else:
             engine, metadata = get_db()
 
             user_prefs = metadata.tables['user_pref']
-            user_password_reset_tokens = metadata.tables['user_password_reset_token']
 
             try:
                 with engine.connect() as conn:
                     stmt = select(user_prefs).where(
                         user_prefs.c.email == request.form['email']
                     )
                     result = conn.execute(stmt)
                     user_pref = result.fetchone()
 
-                    if user_pref:
-                        stmt = insert(user_password_reset_tokens).values(
-                            token=str(uuid.uuid4()),
-                            user_id=user_pref.user_id,
-                            expire_at=datetime.datetime.now() + datetime.timedelta(minutes=10),
-                        )
-                        result = conn.execute(stmt)
-
-                        stmt = select(user_password_reset_tokens).where(
-                            user_password_reset_tokens.c.id == result.inserted_primary_key[0]
-                        )
-                        result = conn.execute(stmt)
-                        reset_token = result.fetchone()
-
-                        send_user_password_reset_token(reset_token, user_pref)
-
-                        conn.commit()
+                if user_pref:
+                    reset_token = build_user_password_reset_token(user_pref)
+                    send_user_password_reset_token(reset_token, user_pref)
             except SQLAlchemyError as e:
                 current_app.logger.error(str(e))
                 error = f"Something went wrong."
             except smtplib.SMTPException as e:
                 current_app.logger.error(str(e))
                 flash(_("We failed to send the mail: " + str(e)))
             else:
@@ -275,15 +284,15 @@
     return True
 
 def user_pref_smtp_enough(view):
     @functools.wraps(view)
     def wrapped_view(**kwargs):
         if not is_user_pref_smtp_enough():
             flash(_("We need more of your SMTP configuration."), 'important')
-            return redirect(url_for("user.update"))
+            return redirect(url_for("me.update"))
 
         return view(**kwargs)
 
     return wrapped_view
 
 @bp.route('/logout')
 @login_required
@@ -310,34 +319,40 @@
 
     user_prefs = metadata.tables['user_pref']
     stmt = select(user_prefs).where(user_prefs.c.user_id == user_id)
     with engine.connect() as conn:
         result = conn.execute(stmt)
     g.user_pref = result.fetchone()
 
-    # To be retro-compatible
-    if g.user_pref:
-        return
-    with engine.connect() as conn:
-        stmt = insert(user_prefs).values(user_id=user_id)
-        result = conn.execute(stmt)
-        conn.commit()
-
-    # Retry
-    stmt = select(user_prefs).where(user_prefs.c.user_id == user_id)
-    with engine.connect() as conn:
-        result = conn.execute(stmt)
-    g.user_pref = result.fetchone()
-
 @bp.before_app_request
 def setup_locale():
     if g.user_pref is not None:
         g.locale = g.user_pref.locale
     else:
         g.locale = request.accept_languages.best_match(["en_US", "fr_FR"])
     if not g.locale:
         g.locale = 'en_US'
 
     localedir = os.path.abspath(os.path.dirname(os.path.abspath(__file__))) + "/locale"
     translation = gettext.translation("messages", localedir, languages=[g.locale, "en_US"])
     translation.install()
     current_app.jinja_env.install_gettext_translations(translation)
+
+def build_user_password_reset_token(user_pref):
+    engine, metadata = get_db()
+    user_password_reset_tokens = metadata.tables['user_password_reset_token']
+
+    with engine.connect() as conn:
+        stmt = insert(user_password_reset_tokens).values(
+            token=str(uuid.uuid4()),
+            user_id=user_pref.user_id,
+            expire_at=datetime.datetime.now() + datetime.timedelta(minutes=10),
+        )
+        result = conn.execute(stmt)
+
+        stmt = select(user_password_reset_tokens).where(
+            user_password_reset_tokens.c.id == result.inserted_primary_key[0]
+        )
+        result = conn.execute(stmt)
+        conn.commit()
+
+        return result.fetchone()
```

## fossbill/bill.py

```diff
@@ -1,16 +1,16 @@
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, url_for
 )
 from werkzeug.exceptions import abort
 from fossbill.auth import login_required, user_pref_smtp_enough
 from fossbill.database import get_db, paginatestmt, pagination, filterstmt
-from fossbill.client import get_client, get_clients
+from fossbill.customer import get_customer, get_customers
 from fossbill.product import get_product, get_products
-from fossbill.user import get_user_smtp_server
+from fossbill.me import get_user_smtp_server
 from fossbill.payment import user_subscription_valid
 from sqlalchemy import insert, select, join, func, literal_column, desc, case
 from sqlalchemy.exc import SQLAlchemyError
 import datetime
 from flask_weasyprint import render_pdf, HTML
 from email.message import EmailMessage
 import smtplib
@@ -67,15 +67,15 @@
     )
 
 @bp.route('/')
 @login_required
 def index():
     engine, metadata = get_db()
     bills = metadata.tables['bill']
-    stmt = bills_view().where(bills.c.user_id == g.user.id).order_by(desc(bills.c.date))
+    stmt = bills_view().where(bills.c.user_id == g.user.id).order_by(desc(bills.c.created_at), desc(bills.c.id))
 
     stmt, filtered = filterstmt(stmt, request)
     statstmt = tostatstmt(stmt)
     stmt, countstmt = paginatestmt(stmt, request)
 
     defaultstats = {
         'count': 0,
@@ -114,36 +114,36 @@
 @bp.route('/create', methods=['GET', 'POST'])
 @login_required
 @user_subscription_valid
 def create():
     if request.method == 'POST':
         error = None
 
-        if request.form.get('client_id'):
+        if request.form.get('customer_id'):
             try:
-                int(request.form['client_id'])
+                int(request.form['customer_id'])
             except ValueError as ve:
-                error = _('Client id should be an integer.')
+                error = _('Customer id should be an integer.')
 
         if error is not None:
             flash(error)
         else:
-            client_id = None
+            customer_id = None
             recipient = ""
 
-            if request.form.get('client_id'):
-                client = get_client(request.form['client_id'], g.user.id)
-                client_id = client.id
-                recipient = client.address
+            if request.form.get('customer_id'):
+                customer = get_customer(request.form['customer_id'], g.user.id)
+                customer_id = customer.id
+                recipient = customer.address
 
             engine, metadata = get_db()
 
             stmt = insert(metadata.tables['bill']).values(
-                client_id=client_id,
-                date=datetime.date.today(),
+                customer_id=customer_id,
+                created_at=datetime.date.today(),
                 recipient=recipient,
                 source=g.user_pref.source,
                 bill_mentions=g.user_pref.bill_mentions,
                 quote_mentions=g.user_pref.quote_mentions,
                 user_id=g.user.id,
             )
             try:
@@ -153,15 +153,15 @@
             except SQLAlchemyError as e:
                 current_app.logger.error(str(e))
                 flash(_("Something went wrong."))
             else:
                 flash(_("Bill created."))
                 return redirect(url_for("bill.update", id=result.inserted_primary_key[0]))
 
-    return render_template('bill/create.html', clients=get_clients(g.user.id))
+    return render_template('bill/create.html', customers=get_customers(g.user.id))
 
 def get_new_bill_number(user_id):
     engine, metadata = get_db()
     bills = metadata.tables['bill']
     stmt = select(func.max(bills.c.bill_number)).where(
         bills.c.user_id == user_id,
         bills.c.bill_number != None,
@@ -263,53 +263,78 @@
 @login_required
 def update(id):
     bill = get_bill(id, g.user.id)
 
     if request.method == 'POST':
         error = None
 
-        if not None == bill.quote_number:
-            flash(_("This bill is not a draft."))
-            return redirect(url_for('bill.update', id=id))
+        form = dict(request.form)
 
-        if not request.form['date']:
-            error = _('Date is required.')
+        if None == bill.quote_number and None == bill.bill_number:
+            if form.get('customer_id'):
+                try:
+                    int(form['customer_id'])
+                except ValueError as ve:
+                    error = _('Customer id should be an integer.')
+                else:
+                    get_customer(form['customer_id'], g.user.id) # to check
+            else:
+                form['customer_id'] = None
 
-        if not request.form['recipient']:
-            error = _('Recipient is required.')
+            if None == form.get('recipient'):
+                error = _('Recipient is required.')
 
-        if not request.form['source']:
-            error = _('Source is required.')
+            if None == form.get('source'):
+                error = _('Source is required.')
+        else:
+            form['customer_id'] = None
+            form['recipient'] = None
+            form['source'] = None
+
+        if None == bill.quote_number and None == bill.bill_number:
+            if None == form.get('quote_mentions'):
+                error = _('Quote mentions are required.')
+        else:
+            form['quote_mentions'] = None
 
-        if error is None:
-            if request.form['client_id']:
-                try:
-                    int(request.form['client_id'])
-                except ValueError as ve:
-                    error = _('Client id should be an integer.')
+        if None == bill.bill_number:
+            if None == form.get('bill_mentions'):
+                error = _('Bill mentions are required.')
+        else:
+            form['bill_mentions'] = None
 
-        if error is not None:
-            flash(error)
+        if bill.bill_number:
+            if not form.get('paid'):
+                error = _('Is paid is required.')
+            elif not form['paid'] in ["1", "0"]:
+                error = _('Is paid can be 0 or 1.')
+            else:
+                form['paid'] = form['paid'] == "1"
         else:
-            client_id = None
-            if request.form['client_id']:
-                get_client(request.form['client_id'], g.user.id) # to check
-                client_id = request.form['client_id']
+            form['paid'] = None
 
-            date = datetime.datetime.strptime(request.form['date'], "%Y-%m-%d")
 
+        if error is not None:
+            flash(error)
+        else:
             engine, metadata = get_db()
             bills = metadata.tables['bill']
 
-            stmt = bills.update().values(
-                client_id=client_id,
-                date=date,
-                recipient=request.form['recipient'],
-                source=request.form['source'],
-            ).where(
+            to_update_values = {
+                'customer_id': form.get('customer_id'),
+                'recipient': form.get('recipient'),
+                'source': form.get('source'),
+                'quote_mentions': form.get('quote_mentions'),
+                'bill_mentions': form.get('bill_mentions'),
+                'comment': form.get('comment'),
+                'paid': form.get('paid'),
+            }
+            to_update_values = {k: v for k, v in to_update_values.items() if v is not None}
+
+            stmt = bills.update().values(**to_update_values).where(
                 bills.c.id == id,
                 bills.c.user_id == g.user.id,
             )
             try:
                 with engine.connect() as conn:
                     result = conn.execute(stmt)
                     conn.commit()
@@ -317,74 +342,37 @@
                 current_app.logger.error(str(e))
                 flash(_("Something went wrong."))
             else:
                 flash(_("Bill updated."))
                 return redirect(url_for("bill.update", id=id))
 
     if None == bill.quote_number and None == bill.bill_number:
-        edit_bill_row = None
-        if request.args.get('edit_bill_row_id'):
-            edit_bill_row = get_bill_row(request.args['edit_bill_row_id'], g.user.id)
-
         return render_template(
             'bill/update.html',
             bill=bill,
             bill_rows=get_bill_rows(bill.id, g.user.id),
-            clients=get_clients(g.user.id),
-            products=get_products(g.user.id),
-            edit_bill_row=edit_bill_row,
+            customers=get_customers(g.user.id),
         )
     elif None == bill.bill_number:
         return render_template(
             'bill/update_quote.html',
             bill=bill,
             bill_rows=get_bill_rows(bill.id, g.user.id),
-            clients=get_clients(g.user.id),
+            customers=get_customers(g.user.id),
             products=get_products(g.user.id),
         )
     else:
         return render_template(
             'bill/update_bill.html',
             bill=bill,
             bill_rows=get_bill_rows(bill.id, g.user.id),
-            clients=get_clients(g.user.id),
+            customers=get_customers(g.user.id),
             products=get_products(g.user.id),
         )
 
-@bp.route('/<int:id>/mark_paid', methods=['POST'])
-@login_required
-def mark_paid(id):
-    bill = get_bill(id, g.user.id)
-    if None == bill.bill_number:
-        flash(_("This bill is not finished."))
-        return redirect(url_for('bill.update', id=id))
-    if bill.paid:
-        flash(_("This bill already is paid."))
-        return redirect(url_for('bill.update', id=id))
-
-    engine, metadata = get_db()
-    bills = metadata.tables['bill']
-
-    try:
-        with engine.connect() as conn:
-            stmt = bills.update().values(
-                paid=True,
-            ).where(
-                bills.c.id == id,
-                bills.c.user_id == g.user.id,
-            )
-            result = conn.execute(stmt)
-            conn.commit()
-    except SQLAlchemyError as e:
-        current_app.logger.error(str(e))
-        flash(_("Something went wrong."))
-    else:
-        flash(_("Bill marked as paid."))
-        return redirect(url_for('bill.update', id=id))
-
 @bp.route('/<int:id>/delete', methods=['POST'])
 @login_required
 def delete(id):
     bill = get_bill(id, g.user.id)
     if not None == bill.quote_number:
         flash(_("This bill is not a draft."))
         return redirect(url_for('bill.update', id=id))
@@ -411,255 +399,205 @@
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         flash(_("Something went wrong."))
     else:
         flash(_("Bill deleted."))
         return redirect(url_for('bill.index'))
 
-@bp.route('/<int:id>/create_row', methods=['POST'])
+@bp.route('/<int:id>/rows/create', methods=['GET', 'POST'])
 @login_required
 def create_row(id):
-    error = None
-
     bill = get_bill(id, g.user.id)
-    if not None == bill.quote_number:
-        flash(_("This bill is not a draft."))
-        return redirect(url_for('bill.update', id=id))
 
-    if request.form.get('product_id'):
-        try:
-            int(request.form['product_id'])
-        except ValueError as ve:
-            error = _('Product id should be an integer.')
-
-        if error is None:
-            product = get_product(request.form['product_id'], g.user.id)
-            label = product.label
-            price = product.price
-            tax_rate = product.tax_rate
-    elif request.form.get('label') or request.form.get('price'):
-        label = request.form['label']
-        if not label:
-            error = _('Label is required.')
-
-        if not request.form['price']:
-            error = _('Price is required.')
+    if request.method == 'POST':
+        error = None
 
-        if not request.form['tax_rate']:
-            error = _('Tax rate is required.')
+        if not None == bill.quote_number:
+            flash(_("This bill is not a draft."))
+            return redirect(url_for('bill.update', id=id))
 
-        if error is None:
+        if request.form.get('product_id'):
             try:
-                price = float(request.form['price'])*100
+                int(request.form['product_id'])
             except ValueError as ve:
-                error = _('Price should be a float.')
+                error = _('Product id should be an integer.')
 
-            try:
-                tax_rate = float(request.form['tax_rate'])
-            except ValueError as ve:
-                error = _('Tax rate should be a float.')
+            if error is None:
+                product = get_product(request.form['product_id'], g.user.id)
+                label = product.label
+                price = product.price
+                tax_rate = product.tax_rate
+        elif request.form.get('label') or request.form.get('price'):
+            label = request.form['label']
+            if not label:
+                error = _('Label is required.')
 
-        if error is None:
-            if tax_rate < 0:
-                error = _('Tax rate should be higher than 0.')
-            elif tax_rate > 100:
-                error = _('Tax rate should be lower than 100.')
-    else:
-        error = _('Either give a product id or all.')
+            if not request.form['price']:
+                error = _('Price is required.')
+
+            if not request.form['tax_rate']:
+                error = _('Tax rate is required.')
 
-    if not request.form['quantity']:
-        error = _('Quantity is required.')
+            if error is None:
+                try:
+                    price = float(request.form['price'])*100
+                except ValueError as ve:
+                    error = _('Price should be a float.')
 
-    if error is None:
-        try:
-            quantity = int(request.form['quantity'])
-        except ValueError as ve:
-            error = _('Quantity should be an integer.')
+                try:
+                    tax_rate = float(request.form['tax_rate'])
+                except ValueError as ve:
+                    error = _('Tax rate should be a float.')
 
-    if error is not None:
-        flash(error)
-    else:
-        engine, metadata = get_db()
-        stmt = insert(metadata.tables['bill_row']).values(
-            user_id=g.user.id,
-            bill_id=id,
-            label=label,
-            price=price,
-            quantity=quantity,
-            tax_rate=tax_rate,
-        )
-        try:
-            with engine.connect() as conn:
-                result = conn.execute(stmt)
-                conn.commit()
-        except SQLAlchemyError as e:
-            current_app.logger.error(str(e))
-            flash(_("Something went wrong."))
+            if error is None:
+                if tax_rate < 0:
+                    error = _('Tax rate should be higher than 0.')
+                elif tax_rate > 100:
+                    error = _('Tax rate should be lower than 100.')
         else:
-            flash(_("Bill row created."))
-            return redirect(url_for(
-                'bill.update',
-                id=id,
-                _anchor="bill_row_"+str(result.inserted_primary_key[0]))
-            )
+            error = _('Either give a product id or all.')
 
-    return redirect(url_for(
-        'bill.update',
-        id=id,
-    ))
+        if not request.form['quantity']:
+            error = _('Quantity is required.')
 
-@bp.route('/<int:id>/update_comment', methods=['POST'])
-@login_required
-def update_comment(id):
-    bill = get_bill(id, g.user.id)
+        if error is None:
+            try:
+                quantity = int(request.form['quantity'])
+            except ValueError as ve:
+                error = _('Quantity should be an integer.')
+
+        if error is not None:
+            flash(error)
+        else:
+            engine, metadata = get_db()
+            stmt = insert(metadata.tables['bill_row']).values(
+                user_id=g.user.id,
+                bill_id=id,
+                label=label,
+                price=price,
+                quantity=quantity,
+                tax_rate=tax_rate,
+            )
+            try:
+                with engine.connect() as conn:
+                    result = conn.execute(stmt)
+                    conn.commit()
+            except SQLAlchemyError as e:
+                current_app.logger.error(str(e))
+                flash(_("Something went wrong."))
+            else:
+                flash(_("Bill row created."))
+                if request.form.get('create_another'):
+                    return redirect(url_for(
+                        "bill.create_row",
+                        create_another=True,
+                        id=id,
+                    ))
+                else:
+                    return redirect(url_for(
+                        'bill.update',
+                        id=id,
+                        _anchor="bill_row_"+str(result.inserted_primary_key[0]))
+                    )
 
-    engine, metadata = get_db()
-    bills = metadata.tables['bill']
-    stmt = bills.update().values(
-        comment=request.form['comment'],
-    ).where(
-        bills.c.id == id,
-        bills.c.user_id == g.user.id,
-    )
-    try:
-        with engine.connect() as conn:
-            result = conn.execute(stmt)
-            conn.commit()
-    except SQLAlchemyError as e:
-        current_app.logger.error(str(e))
-        flash(_("Something went wrong."))
-    else:
-        flash(_("Bill comment updated."))
         return redirect(url_for(
             'bill.update',
-            id=bill.id,
-            _anchor="bill_comment")
-        )
+            id=id,
+        ))
 
-    return redirect(url_for('bill.update', id=bill.id))
+    return render_template(
+        'bill/create_row.html',
+        bill=bill,
+        products=get_products(g.user.id),
+    )
 
-@bp.route('/<int:id>/update_mentions', methods=['POST'])
+@bp.route('/<int:bill_id>/rows/<int:id>/update', methods=['get', 'POST'])
 @login_required
-def update_mentions(id):
-    bill = get_bill(id, g.user.id)
+def update_row(bill_id, id):
+    bill = get_bill(bill_id, g.user.id)
+    bill_row = get_bill_row(id, g.user.id)
 
-    if not None == bill.quote_number:
-        flash(_("This bill is not a draft."))
-        return redirect(url_for('bill.update', id=id))
+    if request.method == 'POST':
+        if not None == bill.quote_number:
+            flash(_("This bill is not a draft."))
+            return redirect(url_for('bill.update', id=bill_row.bill_id))
 
-    quote_mentions = request.form.get('quote_mentions', None)
-    if not quote_mentions:
-        quote_mentions = None
-
-    bill_mentions = request.form.get('bill_mentions', None)
-    if not bill_mentions:
-        bill_mentions = None
+        error = None
 
-    engine, metadata = get_db()
-    bills = metadata.tables['bill']
-    stmt = bills.update().values(
-        quote_mentions=quote_mentions,
-        bill_mentions=bill_mentions,
-    ).where(
-        bills.c.id == id,
-        bills.c.user_id == g.user.id,
-    )
-    try:
-        with engine.connect() as conn:
-            result = conn.execute(stmt)
-            conn.commit()
-    except SQLAlchemyError as e:
-        current_app.logger.error(str(e))
-        flash(_("Something went wrong."))
-    else:
-        flash(_("Bill mentions updated."))
-        return redirect(url_for(
-            'bill.update',
-            id=bill.id,
-            _anchor="bill_mentions")
-        )
+        if not request.form['label']:
+            error = _('Label is required.')
 
-    return redirect(url_for('bill.update', id=bill.id))
+        if not request.form['price']:
+            error = _('Price is required.')
 
-@bp.route('/<int:id>/update_row', methods=['POST'])
-@login_required
-def update_row(id):
-    bill_row = get_bill_row(id, g.user.id)
-    bill = get_bill(bill_row.bill_id, g.user.id)
+        if not request.form['quantity']:
+            error = _('Quantity is required.')
 
-    if not None == bill.quote_number:
-        flash(_("This bill is not a draft."))
-        return redirect(url_for('bill.update', id=bill_row.bill_id))
+        if not request.form['tax_rate']:
+            error = _('Tax rate is required.')
 
-    error = None
+        if error is None:
+            try:
+                float(request.form['price'])*100
+            except ValueError as ve:
+                error = _('Price should be a float.')
 
-    if not request.form['label']:
-        error = _('Label is required.')
+            try:
+                int(request.form['quantity'])
+            except ValueError as ve:
+                error = _('Quantity should be an integer.')
 
-    if not request.form['price']:
-        error = _('Price is required.')
+            try:
+                tax_rate = float(request.form['tax_rate'])
+            except ValueError as ve:
+                error = _('Tax rate should be a float.')
 
-    if not request.form['quantity']:
-        error = _('Quantity is required.')
-
-    if not request.form['tax_rate']:
-        error = _('Tax rate is required.')
-
-    if error is None:
-        try:
-            float(request.form['price'])*100
-        except ValueError as ve:
-            error = _('Price should be a float.')
-
-        try:
-            int(request.form['quantity'])
-        except ValueError as ve:
-            error = _('Quantity should be an integer.')
-
-        try:
-            tax_rate = float(request.form['tax_rate'])
-        except ValueError as ve:
-            error = _('Tax rate should be a float.')
-
-    if error is None:
-        if tax_rate < 0:
-            error = _('Tax rate should be higher than 0.')
-        elif tax_rate > 100:
-            error = _('Tax rate should be lower than 100.')
+        if error is None:
+            if tax_rate < 0:
+                error = _('Tax rate should be higher than 0.')
+            elif tax_rate > 100:
+                error = _('Tax rate should be lower than 100.')
 
-    if error is not None:
-        flash(error)
-    else:
-        engine, metadata = get_db()
-        bill_rows = metadata.tables['bill_row']
-        stmt = bill_rows.update().values(
-            label=request.form['label'],
-            price=float(request.form['price'])*100,
-            quantity=request.form['quantity'],
-            tax_rate=request.form['tax_rate'],
-        ).where(
-            bill_rows.c.id == id,
-            bill_rows.c.user_id == g.user.id,
-        )
-        try:
-            with engine.connect() as conn:
-                result = conn.execute(stmt)
-                conn.commit()
-        except SQLAlchemyError as e:
-            current_app.logger.error(str(e))
-            flash(_("Something went wrong."))
+        if error is not None:
+            flash(error)
         else:
-            flash(_("Bill row updated."))
-            return redirect(url_for(
-                'bill.update',
-                id=bill.id,
-                _anchor="bill_row_"+str(id))
+            engine, metadata = get_db()
+            bill_rows = metadata.tables['bill_row']
+            stmt = bill_rows.update().values(
+                label=request.form['label'],
+                price=float(request.form['price'])*100,
+                quantity=request.form['quantity'],
+                tax_rate=request.form['tax_rate'],
+            ).where(
+                bill_rows.c.id == id,
+                bill_rows.c.user_id == g.user.id,
             )
+            try:
+                with engine.connect() as conn:
+                    result = conn.execute(stmt)
+                    conn.commit()
+            except SQLAlchemyError as e:
+                current_app.logger.error(str(e))
+                flash(_("Something went wrong."))
+            else:
+                flash(_("Bill row updated."))
+                return redirect(url_for(
+                    'bill.update',
+                    id=bill.id,
+                    _anchor="bill_row_"+str(id))
+                )
+
+        return redirect(url_for('bill.update', id=bill.id))
+
+    return render_template(
+        'bill/update_row.html',
+        bill=bill,
+        bill_row=bill_row,
+    )
 
-    return redirect(url_for('bill.update', id=bill.id, edit_bill_row_id=id))
 
 @bp.route('/<int:id>/delete_row', methods=['POST'])
 @login_required
 def delete_row(id):
     bill_row = get_bill_row(id, g.user.id)
     bill = get_bill(bill_row.bill_id, g.user.id)
 
@@ -701,14 +639,15 @@
     bill_rows = get_bill_rows(id, g.user.id)
 
     engine, metadata = get_db()
     bills = metadata.tables['bill']
 
     stmt = bills.update().values(
         quote_number=get_new_quote_number(g.user.id),
+        quote_date=datetime.date.today(),
     ).where(
         bills.c.id == id,
         bills.c.user_id == g.user.id,
     )
 
     try:
         with engine.connect() as conn:
@@ -731,14 +670,15 @@
         return redirect(url_for('bill.update', id=id))
 
     engine, metadata = get_db()
     bills = metadata.tables['bill']
 
     stmt = bills.update().values(
         bill_number=get_new_bill_number(g.user.id),
+        bill_date=datetime.date.today(),
     ).where(
         bills.c.id == id,
         bills.c.user_id == g.user.id,
     )
 
     try:
         with engine.connect() as conn:
@@ -748,14 +688,25 @@
         current_app.logger.error(str(e))
         flash(_("Something went wrong."))
     else:
         flash(_("Bill finished."))
 
     return redirect(url_for('bill.update', id=id))
 
+@bp.route('/<int:id>/view_draft', methods=['GET'])
+@login_required
+def view_draft(id):
+    bill = get_bill(id, g.user.id)
+
+    return render_template(
+        'bill/generated_draft.html',
+        bill=bill,
+        bill_rows=get_bill_rows(bill.id, g.user.id),
+    )
+
 @bp.route('/<int:id>/view_quote', methods=['GET'])
 @login_required
 def view_quote(id):
     bill = get_bill(id, g.user.id)
 
     return render_template(
         'bill/generated_quote.html',
@@ -770,37 +721,51 @@
 
     return render_template(
         'bill/generated_bill.html',
         bill=bill,
         bill_rows=get_bill_rows(bill.id, g.user.id),
     )
 
+@bp.route('/<int:id>/view_draft.pdf', methods=['GET'])
+@login_required
+def view_draft_pdf(id):
+    return render_pdf(
+        url_for('bill.view_draft', id=id),
+        download_filename="fossbill_draft_{}.pdf".format(id)
+    )
+
 @bp.route('/<int:id>/view_quote.pdf', methods=['GET'])
 @login_required
 def view_quote_pdf(id):
-    return render_pdf(url_for('bill.view_quote', id=id))
+    return render_pdf(
+        url_for('bill.view_quote', id=id),
+        download_filename="fossbill_quote_{}.pdf".format(id)
+    )
 
 @bp.route('/<int:id>/view_bill.pdf', methods=['GET'])
 @login_required
 def view_bill_pdf(id):
-    return render_pdf(url_for('bill.view_bill', id=id))
+    return render_pdf(
+        url_for('bill.view_bill', id=id),
+        download_filename="fossbill_bill_{}.pdf".format(id)
+    )
 
 @bp.route('/<int:id>/send_quote_email', methods=['GET', 'POST'])
 @login_required
 @user_pref_smtp_enough
 def send_quote_email(id):
     bill = get_bill(id, g.user.id)
 
     if None == bill.quote_number:
         flash(_("This quote is not generated."))
         return redirect(url_for('bill.update', id=id))
 
-    client = None
-    if bill.client_id:
-        client = get_client(bill.client_id, g.user.id)
+    customer = None
+    if bill.customer_id:
+        customer = get_customer(bill.customer_id, g.user.id)
 
     if request.method == 'POST':
         error = None
         if not request.form['email']:
             error = _('Email is required.')
 
         if not request.form['subject']:
@@ -853,32 +818,32 @@
     )
 
     default_subject = "{} #{}".format(_("Quote"), bill.quote_number)
 
     return render_template(
         'bill/send_quote_email.html',
         bill=bill,
-        client=client,
+        customer=customer,
         default_body=default_body,
         default_subject=default_subject,
     )
 
 @bp.route('/<int:id>/send_bill_email', methods=['GET', 'POST'])
 @login_required
 @user_pref_smtp_enough
 def send_bill_email(id):
     bill = get_bill(id, g.user.id)
 
     if None == bill.bill_number:
         flash(_("This bill is not generated."))
         return redirect(url_for('bill.update', id=id))
 
-    client = None
-    if bill.client_id:
-        client = get_client(bill.client_id, g.user.id)
+    customer = None
+    if bill.customer_id:
+        customer = get_customer(bill.customer_id, g.user.id)
 
     if request.method == 'POST':
         error = None
         if not request.form['email']:
             error = _('Email is required.')
 
         if not request.form['subject']:
@@ -931,11 +896,21 @@
     )
 
     default_subject = "{} #{}".format(_("Bill"), bill.bill_number)
 
     return render_template(
         'bill/send_bill_email.html',
         bill=bill,
-        client=client,
+        customer=customer,
         default_body=default_body,
         default_subject=default_subject,
     )
+
+
+@bp.route('/<int:id>/finish', methods=['GET'])
+@login_required
+def finish(id):
+    bill = get_bill(id, g.user.id)
+    return render_template(
+        'bill/finish.html',
+        bill=bill,
+    )
```

## fossbill/database.py

```diff
@@ -79,15 +79,20 @@
         g.database_url = current_app.config['DATABASE']
         g.engine = create_engine(
             g.database_url,
             echo=current_app.config.get('SQLALCHEMY_ECHO', False),
         )
 
     if 'metadata' not in g:
-        g.metadata = MetaData()
+        g.metadata = MetaData(naming_convention={
+            "fk":
+            "%(table_name)s_%(column_0_name)s_fkey",
+            "ix":
+            "ix_%(table_name)s_%(column_0_name)s",
+        })
 
         user = Table('user', g.metadata,
             Column('id', Integer, primary_key=True),
             Column('username', String(50), unique=True, nullable=False),
             Column('password', String(120), nullable=False),
             Column('stripe_customer', String(256), nullable=True),
             Column('admin', Boolean(), nullable=False, default=False),
@@ -99,50 +104,52 @@
             Column('id', Integer, primary_key=True),
             Column('label', String(120), nullable=False),
             Column('price', Integer, nullable=False),
             Column('tax_rate', Integer, nullable=False),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
         )
 
-        client = Table('client', g.metadata,
+        customer = Table('customer', g.metadata,
             Column('id', Integer, primary_key=True),
             Column('address', String(500), nullable=False),
             Column('email', String(70), nullable=False),
             Column('label', String(40), nullable=False),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
         )
 
-        client = Table('bill', g.metadata,
+        bill = Table('bill', g.metadata,
             Column('id', Integer, primary_key=True),
-            Column('client_id', Integer, ForeignKey("client.id"), nullable=True, index=True),
+            Column('customer_id', Integer, ForeignKey("customer.id"), nullable=True, index=True),
             Column('comment', String(500), nullable=True),
-            Column('date', Date, nullable=False),
+            Column('created_at', Date, nullable=False),
             Column('bill_number', Integer, nullable=True, index=True),
+            Column('bill_date', Date),
             Column('quote_number', Integer, nullable=True, index=True),
+            Column('quote_date', Date),
             Column('recipient', String(500), nullable=True),
             Column('source', String(500), nullable=True),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
             Column('bill_mentions', String(500), nullable=True),
             Column('quote_mentions', String(500), nullable=True),
             Column('paid', Boolean(), nullable=False, server_default='FALSE'),
             UniqueConstraint('user_id', 'bill_number'),
             UniqueConstraint('user_id', 'quote_number'),
         )
 
-        client = Table('bill_row', g.metadata,
+        bill_row = Table('bill_row', g.metadata,
             Column('bill_id', Integer, ForeignKey("bill.id"), nullable=False, index=True),
             Column('id', Integer, primary_key=True),
             Column('label', String(120), nullable=False),
             Column('price', Integer, nullable=False),
             Column('quantity', Integer, nullable=False),
             Column('tax_rate', Integer, nullable=False),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
         )
 
-        client = Table('user_pref', g.metadata,
+        user_pref = Table('user_pref', g.metadata,
             Column('bill_mentions', String(500), nullable=True),
             Column('currency', String(10), nullable=True),
             Column('email', String(254), unique=True, nullable=True),
             Column('id', Integer, primary_key=True),
             Column('locale', String(10), nullable=False, default='en_US'),
             Column('quote_mentions', String(500), nullable=True),
             Column('smtp_host', String(30), nullable=True),
@@ -152,31 +159,32 @@
             Column('smtp_username', String(30), nullable=True),
             Column('smtp_reply_to', String(254), nullable=True),
             Column('smtp_cc', String(508), nullable=True),
             Column('source', String(500), nullable=True),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
         )
 
-        client = Table('user_password_reset_token', g.metadata,
+        user_password_reset_token = Table('user_password_reset_token', g.metadata,
             Column('id', Integer, primary_key=True),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
             Column('token', String(128), nullable=False, unique=True),
-            Column('expire_at', DateTime, nullable=False, server_default=func.now()),
+            Column('expire_at', DateTime, nullable=False, server_default=func.current_timestamp()),
         )
 
         payment = Table('payment', g.metadata,
             Column('id', Integer, primary_key=True),
             Column('user_id', Integer, ForeignKey("user.id"), nullable=False, index=True),
             Column('date', Date, nullable=False),
             Column('valid_for_service_thru', Date, nullable=False),
             Column('amount', Integer, nullable=False),
             Column('currency', String(10), nullable=True),
             Column('payload', JSON, nullable=True),
             Column('card_brand', String(20), nullable=True),
             Column('card_last4', String(4), nullable=True),
+            Column('receipt_url', String(500), nullable=True),
         )
 
     return (g.engine, g.metadata)
 
 bp = Blueprint('db', __name__)
 
 def get_alembic_config():
```

## fossbill/payment.py

```diff
@@ -2,19 +2,21 @@
 import functools
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, url_for
 )
 from werkzeug.exceptions import abort
 from fossbill.auth import login_required
 from fossbill.database import get_db
-from fossbill.auth import load_logged_in_user
+from fossbill.auth import load_logged_in_user, get_system_smtp_server
 from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy import insert, select
+from sqlalchemy import insert, select, join
 import datetime
 from flask_weasyprint import render_pdf, HTML
+import smtplib
+from email.message import EmailMessage
 
 bp = Blueprint('payment', __name__, url_prefix='/payments')
 
 def get_stripe():
     if 'stripe' not in g:
         g.stripe = stripe
         g.stripe.set_app_info(
@@ -27,15 +29,15 @@
 
     return stripe
 
 def payment_enabled(view):
     @functools.wraps(view)
     def wrapped_view(**kwargs):
         if not current_app.config.get('PAYMENT_ENABLED'):
-            return redirect(url_for('user.update'))
+            return redirect(url_for('landing.home'))
 
         return view(**kwargs)
 
     return wrapped_view
 
 def user_charged(user):
     if not user.due_at:
@@ -56,61 +58,87 @@
 
     return datetime.date.today() <= user.created_at + datetime.timedelta(days=grace_days())
 
 def user_subscription_valid(view):
     @functools.wraps(view)
     def wrapped_view(**kwargs):
         if not g.user.admin and not (user_charged(g.user) or user_grace_period(g.user)):
-            return redirect(url_for('payment.home'))
+            return redirect(url_for('payment.index'))
 
         return view(**kwargs)
 
     return wrapped_view
 
-def charge_user(user):
+def send_charged_user_notice(payment, user_pref):
+    body = render_template(
+        'payment/charged_notice.plain',
+        payment=payment,
+    )
+
+    msg = EmailMessage()
+    msg["From"] = current_app.config['SMTP_USERNAME']
+    msg["To"] = user_pref.email
+    msg["Subject"] = "Fossbill - Payment notice"
+    msg.set_content(body)
+
+    server = get_system_smtp_server()
+    server.send_message(msg)
+    server.quit()
+
+def charge_user(user, user_pref):
     if (user_charged(user) or user_grace_period(user)):
         return
 
     stripe = get_stripe()
 
     charge = stripe.Charge.create(
         amount=10 * 100,
         currency="eur",
         customer=user.stripe_customer,
         description="Fossbill.org subscription monthly payment"
     )
 
     engine, metadata = get_db()
+    payments = metadata.tables['payment']
 
     with engine.connect() as conn:
         stmt = metadata.tables['user'].update().values(
             due_at=datetime.date.today() + datetime.timedelta(days=30)
         ).where(
             metadata.tables['user'].c.id == user.id,
         )
         result = conn.execute(stmt)
 
-        stmt = insert(metadata.tables['payment']).values(
+        stmt = insert(payments).values(
             user_id=user.id,
             payload=charge,
             date=datetime.date.today(),
             valid_for_service_thru=datetime.date.today() + datetime.timedelta(days=30),
             amount=charge['amount'],
             currency=charge['currency'],
             card_brand=charge['payment_method_details']['card']['brand'].capitalize(),
             card_last4=charge['payment_method_details']['card']['last4'],
+            receipt_url=charge['receipt_url'],
         )
         result = conn.execute(stmt)
 
         conn.commit()
 
+        stmt = select(payments).where(
+            payments.c.id == result.inserted_primary_key[0]
+        )
+        result = conn.execute(stmt)
+
+        if user_pref.email:
+            send_charged_user_notice(result.fetchone(), user_pref)
+
 @bp.route('/')
 @login_required
 @payment_enabled
-def home():
+def index():
     if user_charged(g.user):
         flash(_('Subscription active and expire the {}').format(g.user.due_at))
     elif user_grace_period(g.user):
         flash(_('Grace period on. Register a payment method.'), 'warning')
     else:
         flash(_('Your subscription is disabled. Please update your payment method.'), 'important')
 
@@ -126,15 +154,15 @@
         current_app.logger.error(str(e))
         error = f"Something went wrong."
         payments = []
     else:
         payments = result.fetchall()
 
     return render_template(
-        'payment/home.html',
+        'payment/index.html',
         payments=payments,
     )
 
 @bp.route('/new_payment_method', methods=['POST'])
 @login_required
 @payment_enabled
 def new_payment_method():
@@ -176,44 +204,50 @@
             )
             with engine.connect() as conn:
                 result = conn.execute(stmt)
                 conn.commit()
 
         except SQLAlchemyError as e:
             current_app.logger.error(str(e))
-            error = f"Something went wrong."
+            error = _("Something went wrong.")
         except stripe.error.CardError as e:
             current_app.logger.error(str(e))
-            error = f"Payment went wrong."
-
-        if user_charged(g.user) or user_grace_period(g.user):
-            flash(_("Payment method created."))
-            return redirect(url_for("payment.home"))
+            error = _("Payment went wrong.")
         else:
-            try:
-                load_logged_in_user() # refresh stripe_customer
-                charge_user(g.user)
-            except SQLAlchemyError as e:
-                current_app.logger.error(str(e))
-                error = f"Something went wrong."
-            except stripe.error.CardError as e:
-                current_app.logger.error(str(e))
-                error = f"Payment went wrong."
+            if user_charged(g.user) or user_grace_period(g.user):
+                flash(_("Payment method created."))
+                return redirect(url_for("payment.index"))
             else:
-                flash(_("Payment method created, and card has been charged."))
+                try:
+                    load_logged_in_user() # refresh stripe_customer
+                    charge_user(g.user, g.user_pref)
+                except SQLAlchemyError as e:
+                    current_app.logger.error(str(e))
+                    error = _("Something went wrong.")
+                except stripe.error.CardError as e:
+                    current_app.logger.error(str(e))
+                    error = _("Payment went wrong.")
+                except smtplib.SMTPException as e:
+                    current_app.logger.error(str(e))
+                    error = _("Email notice went wrong.")
+                else:
+                    flash(_("Payment method created, and card has been charged."))
+                    return redirect(url_for("payment.index"))
 
-    return redirect(url_for("payment.home"))
+    flash(error)
+
+    return redirect(url_for("payment.index"))
 
 @bp.route('/drop_payment_methods', methods=['POST'])
 @login_required
 @payment_enabled
 def drop_payment_methods():
     if not g.user.stripe_customer:
         flash(_("You don't have any payment method registered yet."))
-        return redirect(url_for("payment.home"))
+        return redirect(url_for("payment.index"))
 
     stripe = get_stripe()
 
     try:
         stripe.Customer.delete(g.user.stripe_customer)
 
         engine, metadata = get_db()
@@ -231,16 +265,19 @@
         current_app.logger.error(str(e))
         error = f"Something went wrong."
     except stripe.error.CustomerError as e:
         current_app.logger.error(str(e))
         error = f"Stripe went wrong."
     else:
         flash(_("Payment method deleted."))
+        return redirect(url_for("payment.index"))
+
+    flash(error)
 
-    return redirect(url_for("payment.home"))
+    return redirect(url_for("payment.index"))
 
 @bp.route('/<int:id>/invoice', methods=['GET'])
 @login_required
 @payment_enabled
 def invoice(id):
     engine, metadata = get_db()
     payments = metadata.tables['payment']
@@ -269,16 +306,20 @@
         url_for('payment.invoice', id=id),
         download_filename="fossbill_invoice_{}.pdf".format(id)
     )
 
 @bp.cli.command('charge-users')
 def charge_users():
     engine, metadata = get_db()
+
     users = metadata.tables['user']
-    stmt = select(users).where(
+    user_prefs = metadata.tables['user_pref']
+
+    j = join(users, user_prefs, users.c.id == user_prefs.c.user_id)
+    stmt = select(users, user_prefs).select_from(j).where(
         users.c.stripe_customer != None,
         ((users.c.due_at == None) | (datetime.date.today() > users.c.due_at)) &
         (datetime.date.today() - datetime.timedelta(days=grace_days()) > users.c.created_at)
     )
 
     try:
         with engine.connect() as conn:
@@ -288,16 +329,16 @@
         print(f"Something went wrong.")
         return
 
     print("Starting charging...")
     for to_charge_user in to_charge_users:
             print("Charging user {} card.".format(to_charge_user.id))
             try:
-                charge_user(to_charge_user)
+                charge_user(to_charge_user, to_charge_user)
             except SQLAlchemyError as e:
-                current_app.logger.error(str(e))
-                error = f"Something went wrong."
+                print("Something went wrong: " + str(e))
             except stripe.error.CardError as e:
-                current_app.logger.error(str(e))
-                error = f"Payment went wrong."
+                print("Payment went wrong: " + str(e))
+            except smtplib.SMTPException as e:
+                print("Email notice went wrong: " + str(e))
 
     print("Done!")
```

## fossbill/product.py

```diff
@@ -1,26 +1,26 @@
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, url_for
 )
 from werkzeug.exceptions import abort
 from fossbill.auth import login_required
 from fossbill.database import get_db, paginatestmt, pagination, filterstmt
-from sqlalchemy import insert, select
+from sqlalchemy import insert, select, desc
 from sqlalchemy.exc import SQLAlchemyError
 
 bp = Blueprint('product', __name__, url_prefix='/products')
 
 @bp.route('/')
 @login_required
 def index():
     engine, metadata = get_db()
     products = metadata.tables['product']
     stmt = select(products).where(
         products.c.user_id == g.user.id,
-    )
+    ).order_by(desc(products.c.id))
     stmt, filtered = filterstmt(stmt, request)
     stmt, countstmt = paginatestmt(stmt, request)
     try:
         with engine.connect() as conn:
             result = conn.execute(stmt)
             count = conn.execute(countstmt)
     except SQLAlchemyError as e:
@@ -87,15 +87,18 @@
                     result = conn.execute(stmt)
                     conn.commit()
             except SQLAlchemyError as e:
                 current_app.logger.error(str(e))
                 error = "Something went wrong."
             else:
                 flash(_("Product created."))
-                return redirect(url_for("product.index"))
+                if request.form.get('create_another'):
+                    return redirect(url_for("product.create", create_another=True))
+                else:
+                    return redirect(url_for("product.index"))
 
             flash(error)
 
     return render_template('product/create.html')
 
 def get_product(id, user_id):
     engine, metadata = get_db()
```

## fossbill/user.py

```diff
@@ -1,380 +1,103 @@
+import functools
 from flask import (
-    Blueprint, flash, g, current_app, redirect, render_template, request, url_for,
-    session, send_file
+    Blueprint, flash, g, current_app, redirect, render_template, request, url_for
 )
 from werkzeug.exceptions import abort
-from fossbill.auth import login_required, user_pref_smtp_enough
-from fossbill.database import get_db
-from fossbill.auth import setup_locale
-from fossbill.auth import load_logged_in_user
-from sqlalchemy import insert, select
+from fossbill.auth import login_required, build_user_password_reset_token, send_user_password_reset_token
+from fossbill.database import get_db, paginatestmt, pagination, filterstmt
+from sqlalchemy import insert, select, join, func, literal_column, desc, case
 from sqlalchemy.exc import SQLAlchemyError
 import smtplib
-from email.message import EmailMessage
-import tarfile
-import io
-import csv
-
-bp = Blueprint('user', __name__, url_prefix='/me')
-
-def get_user_smtp_server(user_pref):
-    if user_pref.smtp_security == "TLS":
-        server = smtplib.SMTP_SSL(
-            host=user_pref.smtp_host,
-            port=user_pref.smtp_port,
-            timeout=10
-        )
-    else:
-        server = smtplib.SMTP(
-            host=user_pref.smtp_host,
-            port=user_pref.smtp_port,
-            timeout=10
-        )
-        if user_pref.smtp_security == "STARTTLS":
-            server.starttls()
-
-    server.login(user_pref.smtp_username, user_pref.smtp_password)
-
-    return server
-
-@bp.route('/test_email', methods=['POST'])
-@login_required
-@user_pref_smtp_enough
-def test_email():
-    body = render_template('user/test_email.plain')
-
-    msg = EmailMessage()
-    msg["From"] = g.user_pref.smtp_username
-    msg["To"] = g.user_pref.email
-    msg["Subject"] = _("Test email from Fossbill")
-    msg.set_content(body)
-
-    if g.user_pref.smtp_reply_to:
-        msg["Reply-To"] = g.user_pref.smtp_reply_to
-    if g.user_pref.smtp_cc:
-        msg["Cc"] = g.user_pref.smtp_cc
-
-    try:
-        server = get_user_smtp_server(g.user_pref)
-        server.send_message(msg)
-        server.quit()
-    except smtplib.SMTPException as e:
-        flash(_("We failed to send the mail: " + str(e)))
-        return redirect(url_for("user.update"))
 
-    flash(_("We sent an email to you."))
-    return redirect(url_for("user.update"))
-
-@bp.route('/update', methods=('GET', 'POST'))
-@login_required
-def update():
-    if request.method == 'POST':
-        error = None
-
-        smtp_host = request.form.get('smtp_host', None)
-        if not smtp_host:
-            smtp_host = None
-
-        smtp_username = request.form.get('smtp_username', None)
-        if not smtp_username:
-            smtp_username = None
-
-        smtp_password = request.form.get('smtp_password', None)
-        if not smtp_password:
-            smtp_password = None
-
-        smtp_port = request.form.get('smtp_port', None)
-        if not smtp_port:
-            smtp_port = None
-        else:
-            try:
-                int(smtp_port)
-            except ValueError as ve:
-                error = _('SMTP Port should be an integer.')
-
-        smtp_security = request.form.get('smtp_security', None)
-        if not smtp_security:
-            smtp_security = None
-        else:
-            available_protocols = ['TLS', 'STARTTLS']
-            if not smtp_security in available_protocols:
-                error = _('SMTP Security should be one of {available_protocols}.').format(
-                    available_protocols=', '.join(available_protocols)
-                )
-
-        smtp_reply_to = request.form.get('smtp_reply_to', None)
-        if not smtp_reply_to:
-            smtp_reply_to = None
-
-        smtp_cc = request.form.get('smtp_cc', None)
-        if not smtp_cc:
-            smtp_cc = None
-
-        quote_mentions = request.form.get('quote_mentions', None)
-        if not quote_mentions:
-            quote_mentions = None
-
-        bill_mentions = request.form.get('bill_mentions', None)
-        if not bill_mentions:
-            bill_mentions = None
-
-        available_locales = ['en_US', 'fr_FR']
-        if not request.form.get('locale') in available_locales:
-            error = _('Locale should be one of {available_locales}.').format(
-                available_locales = ', '.join(available_locales)
-            )
-
-        email = request.form.get('email', None)
-        if not email:
-            email = None
-
-        currency = request.form.get('currency', None)
-        if not currency:
-            currency = None
-
-        source = request.form.get('source', None)
-        if not source:
-            source = None
-
-        if error is None:
-            engine, metadata = get_db()
-            user_prefs = metadata.tables['user_pref']
-
-            stmt = user_prefs.update().values(
-                bill_mentions=bill_mentions,
-                currency=currency,
-                email=email,
-                locale=request.form['locale'],
-                quote_mentions=quote_mentions,
-                smtp_host=smtp_host,
-                smtp_password=smtp_password,
-                smtp_port=smtp_port,
-                smtp_security=smtp_security,
-                smtp_username=smtp_username,
-                smtp_reply_to=smtp_reply_to,
-                smtp_cc=smtp_cc,
-                source=source,
-            ).where(
-                user_prefs.c.user_id == g.user.id,
-            )
-            try:
-                with engine.connect() as conn:
-                    result = conn.execute(stmt)
-                    conn.commit()
-            except SQLAlchemyError as e:
-                current_app.logger.error(str(e))
-                error = f"Something went wrong."
-            else:
-                load_logged_in_user() # refresh stripe_customer
-                setup_locale() # refresh locale
-                flash(_("User updated."))
-                return redirect(url_for("user.update"))
+bp = Blueprint('user', __name__, url_prefix='/users')
 
-        flash(error)
+def admin_required(view):
+    @functools.wraps(view)
+    def wrapped_view(**kwargs):
+        if not g.user.admin:
+            abort(404)
 
-    return render_template('user/update.html')
+        return view(**kwargs)
 
+    return wrapped_view
 
-@bp.route('/delete', methods=['POST'])
+@bp.route('/')
+@admin_required
 @login_required
-def delete():
+def index():
     engine, metadata = get_db()
 
+    users = metadata.tables['user']
+    user_prefs = metadata.tables['user_pref']
+
+    j = join(users, user_prefs, users.c.id == user_prefs.c.user_id)
+    stmt = select(users, user_prefs).select_from(j)
+    stmt, filtered = filterstmt(stmt, request)
+    stmt, countstmt = paginatestmt(stmt, request)
     try:
         with engine.connect() as conn:
-            for table_name in ['user_pref', 'bill_row', 'bill', 'client', 'product', 'payment']:
-                table = metadata.tables[table_name]
-                stmt = table.delete().where(
-                    table.c.user_id == g.user.id,
-                )
-                result = conn.execute(stmt)
-
-            stmt = metadata.tables['user'].delete().where(
-                metadata.tables['user'].c.id == g.user.id,
-            )
             result = conn.execute(stmt)
-
-            conn.commit()
-
-            session.clear()
-
-            return redirect(url_for("landing.home"))
+            count = conn.execute(countstmt)
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         flash(_("Something went wrong."))
+        users = []
+        count = 0
+    else:
+        users = result.fetchall()
+        count = count.fetchone().count
 
-    return redirect(url_for("user.update"))
+    return render_template(
+        'user/index.html',
+        users=users,
+        pagination=pagination(count, request),
+        filtered=filtered,
+    )
 
-@bp.route('/delete_bills', methods=['POST'])
-@login_required
-def delete_bills():
+def get_user_user_pref(id):
     engine, metadata = get_db()
 
+    users = metadata.tables['user']
+    user_prefs = metadata.tables['user_pref']
+
+    j = join(users, user_prefs, users.c.id == user_prefs.c.user_id)
+    stmt = select(users, user_prefs).select_from(j).where(
+        users.c.id == id
+    )
+
     try:
         with engine.connect() as conn:
-            for table_name in ['bill_row', 'bill']:
-                table = metadata.tables[table_name]
-                stmt = table.delete().where(
-                    table.c.user_id == g.user.id,
-                )
-                result = conn.execute(stmt)
-
-            conn.commit()
-            flash(_("All bills has been deleted."))
+            result = conn.execute(stmt)
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
-        flash(_("Something went wrong."))
-
-    return redirect(url_for("user.update"))
-
-@bp.route('/import_export_user')
-@login_required
-def import_export_user():
-    return render_template('user/import_export_user.html')
-
-@bp.route('/import_user', methods=['POST'])
-@login_required
-def import_user():
-    error = None
-    if 'file' not in request.files or request.files['file'].filename == '':
-        error = _('File is required.')
-
-    if error is None:
-        file = tarfile.open(fileobj=request.files['file'].stream)
-
-        try:
-            import_user_tar_file(file)
-        except KeyError as e:
-            error = _("The file format seems incorrect.")
-        except SQLAlchemyError as e:
-            current_app.logger.error(str(e))
-            error = _("Something went wrong.")
-        else:
-            flash(_("User data imported."))
-            return redirect(url_for("landing.home"))
-
-    flash(error)
-    return redirect(url_for("user.import_export_user"))
-
-def import_user_tar_file(file):
-    engine, metadata = get_db()
-    with engine.connect() as conn:
-        for table_name in ['bill_row', 'bill', 'client', 'product']:
-            table = metadata.tables[table_name]
-            stmt = table.delete().where(
-                table.c.user_id == g.user.id,
-            )
-            conn.execute(stmt)
-
-        clientfile = io.TextIOWrapper(file.extractfile('client.csv'))
-        clientreader = csv.reader(clientfile)
-        clientids = {}
-        for row in clientreader:
-            stmt = insert(metadata.tables['client']).values(
-                address=row[1],
-                email=row[2],
-                label=row[3],
-                user_id=g.user.id,
-            )
-            result = conn.execute(stmt)
-            clientids[row[0]] = result.inserted_primary_key[0]
-
-        productfile = io.TextIOWrapper(file.extractfile('product.csv'))
-        productreader = csv.reader(productfile)
-        for row in productreader:
-            stmt = insert(metadata.tables['product']).values(
-                label=row[0],
-                price=row[1],
-                tax_rate=row[2],
-                user_id=g.user.id,
-            )
-            conn.execute(stmt)
-
-        billfile = io.TextIOWrapper(file.extractfile('bill.csv'))
-        billreader = csv.reader(billfile)
-        billids = {}
-        for row in billreader:
-            stmt = insert(metadata.tables['bill']).values(
-                client_id=clientids[row[1]] or None,
-                comment=row[2],
-                date=row[3],
-                bill_number=row[4] or None,
-                quote_number=row[5] or None,
-                recipient=row[6],
-                source=row[7],
-                bill_mentions=row[7],
-                quote_mentions=row[9],
-                paid=row[10] == 'False',
-                user_id=g.user.id,
-            )
-            result = conn.execute(stmt)
-            billids[row[0]] = result.inserted_primary_key[0]
+        abort(500, "Something went wrong.")
+    else:
+        user = result.fetchone()
 
-        billrowfile = io.TextIOWrapper(file.extractfile('bill_row.csv'))
-        billrowreader = csv.reader(billrowfile)
-        for row in billrowreader:
-            stmt = insert(metadata.tables['bill_row']).values(
-                bill_id=billids[row[0]],
-                label=row[1],
-                price=row[2],
-                quantity=row[3],
-                tax_rate=row[4],
-                user_id=g.user.id,
-            )
-            conn.execute(stmt)
+    if user is None:
+        abort(404, f"User {id} doesn't exist.")
 
-        conn.commit()
+    return user
 
-@bp.route('/export_user')
+@bp.route('/<int:id>/generate_reset_password', methods=['POST'])
+@admin_required
 @login_required
-def export_user():
-    tarfilebuf = io.BytesIO()
-    file = tarfile.open(fileobj=tarfilebuf, mode='w:bz2')
-
-    add_tarfile_from_table(file, 'client', ['id', 'address', 'email', 'label'])
-    add_tarfile_from_table(file, 'product', ['label', 'price', 'tax_rate'])
-    add_tarfile_from_table(file, 'bill', [
-        'id',
-        'client_id',
-        'comment',
-        'date',
-        'bill_number',
-        'quote_number',
-        'recipient',
-        'source',
-        'bill_mentions',
-        'quote_mentions',
-        'paid'
-    ])
-    add_tarfile_from_table(file, 'bill_row', [
-        'bill_id',
-        'label',
-        'price',
-        'quantity',
-        'tax_rate',
-    ])
-
-    file.close()
-
-    tarfilebuf.seek(0)
+def generate_reset_password(id):
+    user = get_user_user_pref(id)
 
-    return send_file(tarfilebuf, download_name="fossbill_export.tar.bz2")
+    try:
+        reset_token = build_user_password_reset_token(user)
+        if user.email:
+                send_user_password_reset_token(reset_token, user)
+                flash(_("A password reset token has been generated, and sent"))
+        else:
+            flash(_("A password reset token has been generated."))
+        flash(_(url_for("auth.use_reset_password", _external=True, token=reset_token.token)))
+    except SQLAlchemyError as e:
+        current_app.logger.error(str(e))
+        error = f"Something went wrong."
+    except smtplib.SMTPException as e:
+        current_app.logger.error(str(e))
+        flash(_("We failed to send the mail: " + str(e)))
 
-def add_tarfile_from_table(file, table, columns):
-    engine, metadata = get_db()
-    with engine.connect() as conn:
-        filebuf = io.BytesIO()
-        textbuf = io.TextIOWrapper(filebuf)
-        writer = csv.writer(textbuf)
-        stmt = select(metadata.tables[table]).where(
-            metadata.tables[table].c.user_id == g.user.id,
-        )
-        result = conn.execute(stmt)
-        rows = result.fetchall()
-        for row in rows:
-            writer.writerow([getattr(row, column) for column in columns])
-        textbuf.flush()
-        filebuf.seek(0)
-        info = tarfile.TarInfo('{}.csv'.format(table))
-        info.size=filebuf.getbuffer().nbytes
-        file.addfile(tarinfo=info, fileobj=filebuf)
+    return redirect(url_for("user.index"))
```

## fossbill/alembic/versions/fda694e67f67_init.py

```diff
@@ -63,15 +63,15 @@
     sa.PrimaryKeyConstraint('id')
     )
     op.create_index(op.f('ix_product_user_id'), 'product', ['user_id'], unique=False)
     op.create_table('user_password_reset_token',
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('user_id', sa.Integer(), nullable=False),
     sa.Column('token', sa.String(length=128), nullable=False),
-    sa.Column('expire_at', sa.DateTime(), server_default=sa.text('now()'), nullable=False),
+    sa.Column('expire_at', sa.DateTime(), server_default=sa.text('current_timestamp'), nullable=False),
     sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
     sa.PrimaryKeyConstraint('id'),
     sa.UniqueConstraint('token')
     )
     op.create_index(op.f('ix_user_password_reset_token_user_id'), 'user_password_reset_token', ['user_id'], unique=False)
     op.create_table('user_pref',
     sa.Column('bill_mentions', sa.String(length=500), nullable=True),
```

## fossbill/locale/en_US/LC_MESSAGES/messages.mo

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: fossbill 0.3.0*

```diff
@@ -1,29 +1,29 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 9401 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 9501 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
-00000040: 2066 6f73 7362 696c 6c20 302e 332e 300a   fossbill 0.3.0.
-00000050: 5265 706f 7274 2d4d 7367 6964 2d42 7567  Report-Msgid-Bug
-00000060: 732d 546f 3a20 454d 4149 4c40 4144 4452  s-To: EMAIL@ADDR
-00000070: 4553 530a 504f 542d 4372 6561 7469 6f6e  ESS.POT-Creation
-00000080: 2d44 6174 653a 2032 3032 332d 3037 2d30  -Date: 2023-07-0
-00000090: 3720 3130 3a31 372b 3030 3030 0a50 4f2d  7 10:17+0000.PO-
-000000a0: 5265 7669 7369 6f6e 2d44 6174 653a 2032  Revision-Date: 2
-000000b0: 3032 332d 3034 2d32 3420 3132 3a31 342b  023-04-24 12:14+
-000000c0: 3032 3030 0a4c 6173 742d 5472 616e 736c  0200.Last-Transl
-000000d0: 6174 6f72 3a20 4655 4c4c 204e 414d 4520  ator: FULL NAME 
-000000e0: 3c45 4d41 494c 4041 4444 5245 5353 3e0a  <EMAIL@ADDRESS>.
-000000f0: 4c61 6e67 7561 6765 3a20 656e 5f55 530a  Language: en_US.
-00000100: 4c61 6e67 7561 6765 2d54 6561 6d3a 2065  Language-Team: e
-00000110: 6e5f 5553 203c 4c4c 406c 692e 6f72 673e  n_US <LL@li.org>
-00000120: 0a50 6c75 7261 6c2d 466f 726d 733a 206e  .Plural-Forms: n
-00000130: 706c 7572 616c 733d 323b 2070 6c75 7261  plurals=2; plura
-00000140: 6c3d 286e 2021 3d20 3129 3b0a 4d49 4d45  l=(n != 1);.MIME
-00000150: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
-00000160: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000170: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
-00000180: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
-00000190: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
-000001a0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
-000001b0: 4279 3a20 4261 6265 6c20 322e 3132 2e31  By: Babel 2.12.1
-000001c0: 0a00                                     ..
+00000040: 2050 524f 4a45 4354 2056 4552 5349 4f4e   PROJECT VERSION
+00000050: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
+00000060: 6773 2d54 6f3a 2045 4d41 494c 4041 4444  gs-To: EMAIL@ADD
+00000070: 5245 5353 0a50 4f54 2d43 7265 6174 696f  RESS.POT-Creatio
+00000080: 6e2d 4461 7465 3a20 3230 3233 2d30 372d  n-Date: 2023-07-
+00000090: 3136 2030 393a 3433 2b30 3030 300a 504f  16 09:43+0000.PO
+000000a0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
+000000b0: 5945 4152 2d4d 4f2d 4441 2048 4f3a 4d49  YEAR-MO-DA HO:MI
+000000c0: 2b5a 4f4e 450a 4c61 7374 2d54 7261 6e73  +ZONE.Last-Trans
+000000d0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
+000000e0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
+000000f0: 0a4c 616e 6775 6167 653a 2065 6e5f 5553  .Language: en_US
+00000100: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
+00000110: 656e 5f55 5320 3c4c 4c40 6c69 2e6f 7267  en_US <LL@li.org
+00000120: 3e0a 506c 7572 616c 2d46 6f72 6d73 3a20  >.Plural-Forms: 
+00000130: 6e70 6c75 7261 6c73 3d32 3b20 706c 7572  nplurals=2; plur
+00000140: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
+00000150: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
+00000160: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000170: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
+00000180: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
+00000190: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
+000001a0: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
+000001b0: 2d42 793a 2042 6162 656c 2032 2e31 322e  -By: Babel 2.12.
+000001c0: 310a 00                                  1..
```

## fossbill/locale/fr_FR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: fossbill 0.3.0\n"
+"Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-07 10:17+0000\n"
-"PO-Revision-Date: 2023-04-24 13:12+0200\n"
+"POT-Creation-Date: 2023-07-16 09:43+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -57,22 +57,25 @@
 "Voici le devis #%(quotenumber)s\n"
 "\n"
 "Cordialement,\n"
 
 msgid "%(cardbrand)s ending with %(last4)s"
 msgstr "%(cardbrand)s se terminant par %(last4)s"
 
+msgid "A password reset token has been generated, and sent"
+msgstr "Un token de reset de mot de passe a été généré, et envoyé."
+
+msgid "A password reset token has been generated."
+msgstr "Un token de reset de mot de passe a été généré."
+
 msgid "Action"
 msgstr "Action"
 
-msgid "Add a row from an existing product."
-msgstr "Ajouter une ligne depuis un produit existant."
-
-msgid "Add a row from scratch."
-msgstr "Ajouter une ligne de zéro."
+msgid "Active payment"
+msgstr "Paiement actif"
 
 msgid "Address"
 msgstr "Adresse"
 
 msgid "All bills has been deleted."
 msgstr "Toutes les factures ont été supprimées."
 
@@ -90,34 +93,28 @@
 
 msgid "Bill"
 msgstr "Facture"
 
 msgid "Bill #%(billnumber)s"
 msgstr "Facture #%(billnumber)s"
 
-msgid "Bill comment updated."
-msgstr "Commentaire de facture modifié."
-
 msgid "Bill created."
 msgstr "Facture crée."
 
 msgid "Bill deleted."
 msgstr "Facture supprimée."
 
 msgid "Bill finished."
 msgstr "Facture générée."
 
-msgid "Bill marked as paid."
-msgstr "Facture marquée comme payée."
-
 msgid "Bill mentions"
 msgstr "Mentions de factures"
 
-msgid "Bill mentions updated."
-msgstr "Mentions de facture modifiés."
+msgid "Bill mentions are required."
+msgstr "Les mentions de facture sont requis"
 
 msgid "Bill number"
 msgstr "Numéro de facture"
 
 msgid "Bill row created."
 msgstr "Ligne de facture crée."
 
@@ -157,65 +154,81 @@
 
 msgid "Card"
 msgstr "Carte"
 
 msgid "Choose an option"
 msgstr "Choisir une option"
 
-msgid "Client"
-msgstr "Client"
-
-msgid "Client created."
-msgstr "Client créé."
-
-msgid "Client deleted."
-msgstr "Client supprimé."
-
-msgid "Client id should be an integer."
-msgstr "Id de client doit être un chiffre entier."
-
-msgid "Client updated."
-msgstr "Client modifié."
-
-msgid "Clients"
-msgstr "Clients"
-
 msgid "Comment"
 msgstr "Commentaire"
 
+msgid "Contact"
+msgstr "Contacter"
+
 msgid "Count"
 msgstr "Compte"
 
+msgid "Create a bill now, but you can't create a quote later."
+msgstr ""
+"Créer une facture maintenant, mais vous ne pourrez créer un devis plus tard."
+
+msgid "Create a quote first, then create a bill later."
+msgstr "Créer un devis d'abord, et crée une facture plus tard."
+
+msgid "Create another?"
+msgstr "Continuer?"
+
 msgid "Create bill"
 msgstr "Créer la facture"
 
 msgid "Create quote"
 msgstr "Créer le devis"
 
 msgid "Create row"
 msgstr "Créer une ligne"
 
+msgid "Create the bill."
+msgstr "Créer la facture."
+
+msgid "Created after"
+msgstr "Crée après"
+
+msgid "Created at"
+msgstr "Crée le"
+
+msgid "Created before"
+msgstr "Crée avant"
+
 msgid "Currency"
 msgstr "Monnaie"
 
+msgid "Customer"
+msgstr "Customer"
+
+msgid "Customer created."
+msgstr "Customer créé."
+
+msgid "Customer deleted."
+msgstr "Customer supprimé."
+
+msgid "Customer id should be an integer."
+msgstr "Id de client doit être un chiffre entier."
+
+msgid "Customer updated."
+msgstr "Customer modifié."
+
+msgid "Customers"
+msgstr "Customers"
+
 msgid "Dashboard"
 msgstr "Tableau de bord"
 
 msgid "Date"
 msgstr "Date"
 
-msgid "Date after"
-msgstr "Date après"
-
-msgid "Date before"
-msgstr "Date avant"
-
-msgid "Date is required."
-msgstr "Date requise."
-
 msgid "Default source"
 msgstr "Origine par défaut"
 
 msgid "Delete"
 msgstr "Supprimer"
 
 msgid "Delete bills"
@@ -229,50 +242,59 @@
 
 msgid "Detail"
 msgstr "Ligne"
 
 msgid "Details"
 msgstr "Détail"
 
+msgid "Disabled"
+msgstr "Désactivé"
+
 msgid "Draft"
 msgstr "Brouillon"
 
-msgid "Edit \"%(clientlabel)s\""
-msgstr "Modifier \"%(clientlabel)s\""
+msgid "Due at"
+msgstr "Expire le"
+
+msgid "Edit"
+msgstr "Modifier"
+
+msgid "Edit \"%(customerlabel)s\""
+msgstr "Modifier \"%(customerlabel)s\""
 
 msgid "Edit \"%(productlabel)s\""
 msgstr "Modifier \"%(productlabel)s\""
 
 msgid "Edit \"%(username)s\""
 msgstr "Modifier \"%(username)s\""
 
-msgid "Edit bill \"#%(billnumber)s\""
-msgstr "Modifier la facture \"#%(billnumber)s\""
-
-msgid "Edit draft"
-msgstr "Modifier le brouillon"
-
-msgid "Edit quote \"#%(quotenumber)s\""
-msgstr "Modifier le devis \"#%(quotenumber)s\""
+msgid "Edit row"
+msgstr "Modifier la ligne"
 
 msgid "Either give a product id or all."
 msgstr "Utilisez soit un id de produit soit tous."
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Email is required."
 msgstr "E-mail requis."
 
+msgid "Email notice went wrong."
+msgstr "La notification email a échoué."
+
 msgid "Email sent."
 msgstr "Email envoyé."
 
 msgid "Empty"
 msgstr "Vide"
 
+msgid "Enabled"
+msgstr "Activé"
+
 msgid "English"
 msgstr "Anglais"
 
 msgid "Ex: $"
 msgstr "Ex: €"
 
 msgid "Ex: Consulting day"
@@ -300,14 +322,20 @@
 
 msgid "File is required."
 msgstr "Fichier requis."
 
 msgid "Filter"
 msgstr "Filtrer"
 
+msgid "Finish draft"
+msgstr "Finaliser le brouillon"
+
+msgid "Finish quote"
+msgstr "Finir le devis"
+
 msgid "First"
 msgstr "Prem"
 
 msgid "Forgotten password"
 msgstr "Mot de passe perdu"
 
 msgid "Fossbill - User password reset"
@@ -334,20 +362,26 @@
 
 msgid "French"
 msgstr "Français"
 
 msgid "From"
 msgstr "De"
 
+msgid "From an existing product."
+msgstr "Depuis un produit éxistant."
+
 msgid "From quote #%(quotenumber)s"
 msgstr "Du devis #%(quotenumber)s"
 
 msgid "From scratch"
 msgstr "Depuis rien"
 
+msgid "From scratch."
+msgstr "De rien."
+
 msgid "Generated %(date)s"
 msgstr "Généré le %(date)s"
 
 msgid "Grace period on. Register a payment method."
 msgstr "Periode gratuite active. Enregistrer un moyen de payment."
 
 msgid "Gross amount"
@@ -388,14 +422,20 @@
 
 msgid "Invoice"
 msgstr "Facture"
 
 msgid "Invoice #%(invoiceid)s"
 msgstr "Facture #%(invoiceid)s"
 
+msgid "Is paid can be 0 or 1."
+msgstr "Est payé peut être 0 ou 1."
+
+msgid "Is paid is required."
+msgstr "Est payé est requis."
+
 msgid "Is paid?"
 msgstr "Est payé?"
 
 msgid "Issued %(date)s"
 msgstr "Généré le %(date)s"
 
 msgid ""
@@ -424,24 +464,21 @@
 
 msgid "Log In"
 msgstr "Connection"
 
 msgid "Log Out"
 msgstr "Déconnection"
 
-msgid "Mark as paid"
-msgstr "Marquer comme payé"
-
 msgid "New"
 msgstr "Nouveau"
 
 msgid "New Bill"
 msgstr "Nouvelle facture"
 
-msgid "New Client"
+msgid "New Customer"
 msgstr "Nouveau client"
 
 msgid "New Product"
 msgstr "Nouveau produit"
 
 msgid "New card"
 msgstr "Nouvelle carte"
@@ -466,32 +503,35 @@
 
 msgid "Password updated."
 msgstr "Mot de passe modifié."
 
 msgid "Payment details"
 msgstr "Détails du paiement"
 
+msgid "Payment enabled?"
+msgstr "Paiement actif?"
+
 msgid "Payment method created, and card has been charged."
 msgstr "Moyen de paiement crée, et virement effectué."
 
 msgid "Payment method created."
 msgstr "Moyen de paiement créé."
 
 msgid "Payment method deleted."
 msgstr "Moyen de paiement supprimé."
 
+msgid "Payment went wrong."
+msgstr "Le paiement a échoué."
+
 msgid "Payments"
 msgstr "Paiements"
 
 msgid "Prev"
 msgstr "Préc"
 
-msgid "Preview quote"
-msgstr "Prévisualiser le devis"
-
 msgid "Price"
 msgstr "Prix"
 
 msgid "Price greater than"
 msgstr "Prix supérieur à"
 
 msgid "Price is required."
@@ -541,14 +581,17 @@
 
 msgid "Quote finished."
 msgstr "Devis généré."
 
 msgid "Quote mentions"
 msgstr "Mentions de devis"
 
+msgid "Quote mentions are required."
+msgstr "Les mentions de devis sont requis."
+
 msgid "Quote number"
 msgstr "Numéro de devis"
 
 msgid "Receipt"
 msgstr "Reçu"
 
 msgid "Recipient"
@@ -562,14 +605,17 @@
 
 msgid "Reset"
 msgstr "Réinitialiser"
 
 msgid "Reset password"
 msgstr "Reset de mot de passe"
 
+msgid "Return"
+msgstr "Retour"
+
 msgid "SMTP Port should be an integer."
 msgstr "Port SMTP doit être un chiffre entier."
 
 msgid "SMTP Security should be one of {available_protocols}."
 msgstr "Sécurité SMTP doit être l'une des {available_protocols}."
 
 msgid "SMTP cc"
@@ -604,17 +650,14 @@
 
 msgid "Send bill email"
 msgstr "Envoyer le mail de la facture"
 
 msgid "Send quote email"
 msgstr "Envoyer le mail du devis"
 
-msgid "Show"
-msgstr "Voir"
-
 msgid "Show filters"
 msgstr "Afficher les filtres"
 
 msgid "Something went wrong."
 msgstr "Quelque chose a échoué."
 
 msgid "Source"
@@ -686,30 +729,27 @@
 msgstr ""
 "Merci beaucoup de vous être enregistré, et bienvenue à bord ! Fossbill est "
 "un outil simple. Voici quelques pistes pour commencer :"
 
 msgid "The file format seems incorrect."
 msgstr "Le format du fichier semble incorrect."
 
+msgid "The quote already has been generated."
+msgstr "Le devis a déja été généré."
+
 msgid "The top-left part on generated bills. Represent your company."
 msgstr ""
 "Partie en haut à gauche sur les factures générés. Représente votre entité."
 
 msgid "This bill already is finished."
 msgstr "Cette facture est déja générée."
 
-msgid "This bill already is paid."
-msgstr "Cette facture a déja été payée."
-
 msgid "This bill is not a draft."
 msgstr "Cette facture n'est pas un brouillon."
 
-msgid "This bill is not finished."
-msgstr "Cette facture n'est pas générée."
-
 msgid "This bill is not generated."
 msgstr "Cette facture n'est pas générée."
 
 msgid "This quote is not generated."
 msgstr "Ce devis n'est pas généré."
 
 msgid "To"
@@ -723,17 +763,14 @@
 
 msgid "Total"
 msgstr "Total"
 
 msgid "Type"
 msgstr "Type"
 
-msgid "Update"
-msgstr "Modifier"
-
 msgid "Used for password recovery. Must be unique."
 msgstr "Utilisé pour la récupération de mot de passe. Doit être unique."
 
 msgid "User data imported."
 msgstr "Données utilisateur importés."
 
 msgid "User updated."
@@ -741,20 +778,26 @@
 
 msgid "Username"
 msgstr "Utilisateur"
 
 msgid "Username is required."
 msgstr "Nom d'utilisateur requis."
 
+msgid "Users"
+msgstr "Utilisateurs"
+
 msgid "Valid for service through"
 msgstr "Valide pour le service jusqu'au"
 
 msgid "View bill"
 msgstr "Voir la facture"
 
+msgid "View draft"
+msgstr "Voir le brouillon"
+
 msgid "View quote"
 msgstr "Voir le devis"
 
 msgid "We failed to send the mail: "
 msgstr "Nous avons échoué à envoyer le mail: "
 
 msgid "We need more of your SMTP configuration."
@@ -787,16 +830,16 @@
 "email que vous voulez, vos factures et devis."
 
 msgid "You don't have any payment method registered yet."
 msgstr "Vous n'avez pas encore de moyen de paiement enregistré."
 
 msgid ""
 "You should start by editing your user preference. Then add some products you "
-"use frequently. You can also prepare your client list. Registering products "
-"and clients isnt necessary but it make generating bills faster."
+"use frequently. You can also prepare your customer list. Registering "
+"products and customers isnt necessary but it make generating bills faster."
 msgstr ""
 "Vous devriez commencer par modifier vos informations d'utilisateur. Ensuite "
 "enregistrer quelques produits que vous utiliserez souvent. Vous pouvez aussi "
 "préparer votre liste de clients. Enregistrer vos produits et vos clients "
 "n'est pas obligatoire, mais cela rends la génération de facture plus rapide."
 
 msgid "Your subscription is disabled. Please update your payment method."
```

## fossbill/static/bill.css

```diff
@@ -1,6 +1,19 @@
 html { font-family: sans-serif }
 .persons { display: flex; justify-content: space-between; }
 .persons > * { min-width: 10rem; }
 h1 { text-align: center; font-size: 1.5rem; margin-top: 3rem; margin-bottom: 5rem; }
 table { width: 100% }
 th { text-align: left }
+.warning {
+   position: absolute;
+   top: 5rem;
+   left: 20rem;
+   bottom: 0;
+   right: 0;
+   z-index: -1;
+   transform:rotate(-50deg);
+}
+.warning h1 {
+   font-size: 7rem;
+   color: lightgrey;
+}
```

## fossbill/static/style.css

```diff
@@ -1,45 +1,71 @@
 html { font-family: sans-serif; background-color: #303030; color: #eaeaea; }
 a { color: #377ba8; }
-input.danger { color: #cc2f2e; }
-input:not([type=file]), select, textarea, #card-element { background-color: #eaeaea; }
-body { max-width: 960px; margin: 1rem auto 3rem auto; }
-nav { display: flex; align-items: flex-end; justify-content: space-between; }
+body { margin: 1rem 0.5rem 3rem 0.5rem; }
+
+nav { display: flex; flex-direction: column; justify-content: space-between; }
 ul { padding: 0; }
-nav > * { margin: 0; }
+nav > * { margin: 0; margin-top: 0.5rem; }
 nav h1 { font-size: 2rem; }
-nav ul { display: flex; list-style: none; }
+nav ul { display: flex; list-style: none; flex-wrap: wrap; }
 nav ul > *:not(:first-child) { display: block; margin-left: 1rem; }
+
 header { display: flex; align-items: center; margin: 1rem 0 1rem 0; }
 header h1 { flex: auto; padding: 0; margin: 0; }
-.marged { margin: 0 0 0 1rem; }
-form { display: flex; flex-direction: column; }
-form > *:not(:first-child) { margin-top: 0.5rem; }
+
+input:not([type=file]), select, textarea, #card-element { background-color: #eaeaea; }
+input.danger { color: #cc2f2e; }
+
+form, .form { display: flex; flex-direction: column; }
+form > *:not(:first-child), .form > *:not(:first-child) { margin-top: 0.5rem; }
 form label { font-weight: bold; }
 form input { resize: vertical; }
 form textarea { resize: vertical; }
-input[type=submit] { align-self: start; min-width: 8rem; }
+input[type=submit] { align-self: start; }
+
+form.filters { margin-top: 0.5rem; }
+
 .flash--message { margin: 1rem 0; padding: 1rem; background-color: #888888; }
 .flash--important { margin: 1rem 0; padding: 1rem; background-color: #cc2f2e; }
 .flash--warning { margin: 1rem 0; padding: 1rem; background-color: #bc6c25; }
+
 hr { margin: 1rem 0 1rem 0; }
+
+label.action { text-decoration: underline; cursor: pointer; }
 .actions { display: flex; justify-content: flex-start; align-items: center; }
 .actions > * { margin-right: 0.5rem; }
-.flex { display: flex; }
-.flex-align { display: flex; }
-.flex-align > * { flex: 1; }
-.flex-align > #bill_info { flex: 0; }
+
 .pagination { display: flex; justify-content: space-between; }
 .pagination > * { min-width: 2rem; text-align: center; }
-input.hidder:not(:checked) + * { display: none; }
-label.action { text-decoration: underline; cursor: pointer; }
 .pagination { margin-top: 1rem; }
-form.filters { margin-top: 0.5rem; }
-table.index { margin-top: 1rem; table-layout: fixed; }
+
+input.hidder:not(:checked) + * { display: none; }
+
+table.index { margin-top: 1rem; }
 table.summary { margin-top: 1rem; }
 table.summary td { text-align: center; }
 table { width: 100%; border-collapse: collapse; }
 table.index th { padding: 0.5rem 0 0.5rem 0; }
 table thead { background-color: #262626; }
 table tfoot { background-color: #262626; }
 table.index td { min-height: 2rem; }
 tbody tr:nth-child(even) { background-color: #3a3a3a; }
+
+.table-cap { width: 100%; overflow-x: auto; }
+table { min-width: 960px;}
+table td { overflow: hidden; white-space: nowrap; text-overflow: ellipsis; }
+table td:not(.actions) { max-width: 8rem; }
+
+.yes { color: green }
+.no { color: red }
+.center { text-align: center }
+
+@media screen and (max-width: 959px) {
+    .flex-align > *:not(:first-child) { margin-top: 0.5rem; }
+}
+
+@media screen and (min-width: 960px) {
+    body { max-width: 960px; margin: 1rem auto 3rem auto; }
+    nav { align-items: flex-end; flex-direction: row; justify-content: space-between; }
+    .flex-align { display: flex; justify-content: space-between;}
+    .flex-align > * { flex-basis: 48%; }
+}
```

## fossbill/templates/base.html

```diff
@@ -1,23 +1,34 @@
 <!doctype html>
 <title>{% block title %}{% endblock %} - Fossbill</title>
 <link rel="stylesheet" href="{{ url_for('static', filename='style.css') }}">
 <nav>
   <h1><a href="{{ url_for('landing.home') }}">fossbill.org</a></h1>
-  {% if g.user %}
-    {% if config.get('PAYMENT_ENABLED') %}
-      <a href="{{ url_for('payment.home') }}">{% trans %}Payments{% endtrans %}</a>
+  <ul>
+    {% if g.user %}
+      {% if config.get('PAYMENT_ENABLED') %}
+        <a href="{{ url_for('payment.index') }}">{% trans %}Payments{% endtrans %}</a>
+      {% endif %}
+      {% if g.user.admin %}
+        <a href="{{ url_for('user.index') }}">{% trans %}Users{% endtrans %}</a>
+      {% endif %}
     {% endif %}
-  {% endif %}
+    {% if config.get('ADDITIONAL_LINKS') %}
+      {% for additional_link in config.get('ADDITIONAL_LINKS').split('|') %}
+        {% set label, url = additional_link.split(';') %}
+        <a href="{{ url }}">{{ label }}</a>
+      {% endfor %}
+    {% endif %}
+  </ul>
   <ul>
     {% if g.user %}
       <li><a href="{{ url_for('product.index') }}">{% trans %}Products{% endtrans %}</a>
-      <li><a href="{{ url_for('client.index') }}">{% trans %}Clients{% endtrans %}</a>
+      <li><a href="{{ url_for('customer.index') }}">{% trans %}Customers{% endtrans %}</a>
       <li><a href="{{ url_for('bill.index') }}">{% trans %}Bills{% endtrans %}</a>
-      <li><a href="{{ url_for('user.update') }}">~{{ g.user['username'] }}</a>
+      <li><a href="{{ url_for('me.update') }}">~{{ g.user['username'] }}</a>
       <li><a href="{{ url_for('auth.logout') }}" tabindex="-1">{% trans %}Log Out{% endtrans %}</a>
     {% else %}
       <li><a href="{{ url_for('auth.register') }}">{% trans %}Register{% endtrans %}</a>
       <li><a href="{{ url_for('auth.login') }}">{% trans %}Log In{% endtrans %}</a>
     {% endif %}
   </ul>
 </nav>
```

### html2text {}

```diff
@@ -1,14 +1,18 @@
 
 ****** fossbill.org ******
-{% if g.user %} {% if config.get('PAYMENT_ENABLED') %} {%_trans_%}Payments{%
-endtrans_%} {% endif %} {% endif %}
+    * {% if g.user %} {% if config.get('PAYMENT_ENABLED') %} {%_trans
+      %}Payments{%_endtrans_%} {% endif %} {% if g.user.admin %} {%_trans
+      %}Users{%_endtrans_%} {% endif %} {% endif %} {% if config.get
+      ('ADDITIONAL_LINKS') %} {% for additional_link in config.get
+      ('ADDITIONAL_LINKS').split('|') %} {% set label, url =
+      additional_link.split(';') %} {{_label_}} {% endfor %} {% endif %}
     * {% if g.user %}
     * {%_trans_%}Products{%_endtrans_%}
-    * {%_trans_%}Clients{%_endtrans_%}
+    * {%_trans_%}Customers{%_endtrans_%}
     * {%_trans_%}Bills{%_endtrans_%}
     * ~{{_g.user['username']_}}
     * {%_trans_%}Log_Out{%_endtrans_%} {% else %}
     * {%_trans_%}Register{%_endtrans_%}
     * {%_trans_%}Log_In{%_endtrans_%} {% endif %}
  {% block header %}{% endblock %}  {% for category, message in
 get_flashed_messages(with_categories=true) %}
```

## fossbill/templates/auth/ask_reset_password.html

```diff
@@ -5,9 +5,10 @@
 {% endblock %}
 
 {% block content %}
   <form method="post">
     <label for="email">{% trans %}Email{% endtrans %}</label>
     <input name="email" id="email" required autofocus>
     <input type="submit" value="{% trans %}Submit{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/auth/login.html

```diff
@@ -7,12 +7,13 @@
 {% block content %}
   <form method="post">
     <label for="username">{% trans %}Username{% endtrans %}</label>
     <input name="username" id="username" required autofocus>
     <label for="password">{% trans %}Password{% endtrans %}</label>
     <input type="password" name="password" id="password" required>
     <input type="submit" value="{% trans %}Log In{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
   <div class="actions">
     <a href="{{ url_for('auth.ask_reset_password') }}">{% trans %}Forgotten password{% endtrans %}</a>
   </div>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends 'base.html' %} {% block header %}
 ****** {% block title %}{% trans %}Log In{% endtrans %}{% endblock %} ******
 {% endblock %} {% block content %}
 {% trans %}Username{% endtrans %} [username            ] {% trans %}Password{%
-endtrans %} [********************] [{% trans %}Log In{% endtrans %}]
+endtrans %} [********************] [{% trans %}Log In{% endtrans %}] {
+{ csrf_token()|safe }}
 {%_trans_%}Forgotten_password{%_endtrans_%}
 {% endblock %}
```

## fossbill/templates/auth/register.html

```diff
@@ -7,9 +7,10 @@
 {% block content %}
   <form method="post">
     <label for="username">{% trans %}Username{% endtrans %}</label>
     <input name="username" id="username" required autofocus>
     <label for="password">{% trans %}Password{% endtrans %}</label>
     <input type="password" name="password" id="password" required>
     <input type="submit" value="{% trans %}Register{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/auth/use_reset_password.html

```diff
@@ -6,9 +6,10 @@
 
 {% block content %}
   <form method="post">
     <label for="password">{% trans %}Password{% endtrans %}</label>
     <input type="password" name="password" id="password" required autofocus>
     <input type="hidden" name="token" id="token" value="{{ request.args['token'] }}" required>
     <input type="submit" value="{% trans %}Submit{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/bill/create.html

```diff
@@ -2,17 +2,18 @@
 
 {% block header %}
   <h1>{% block title %}{% trans %}New Bill{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
-    <label for="client_id">{% trans %}Client{% endtrans %}</label>
-    <select name="client_id" id="client_id" autofocus>
+    <label for="customer_id">{% trans %}Customer{% endtrans %}</label>
+    <select name="customer_id" id="customer_id" autofocus>
       <option value="">{% trans %}From scratch{% endtrans %}</option>
-      {% for client in clients %}
-        <option value="{{ client.id }}">{{ client.label }}</option>
+      {% for customer in customers %}
+        <option value="{{ customer.id }}">{{ customer.label }}</option>
       {% endfor %}
     </select> 
     <input type="submit" value="{% trans %}Save{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/bill/generated_bill.html

```diff
@@ -6,26 +6,19 @@
   <div class="persons">
     <pre><b>{% trans %}From{% endtrans %}</b>
 {{ bill.source }}</pre>
     <pre><b>{% trans %}To{% endtrans %}</b>
 {{ bill.recipient }}</pre>
   </div>
   <p>
-    {% if None == bill.quote_number and None == bill.bill_number %}
-      <b>{% trans %}Draft{% endtrans %}</b><br>
-      {% trans date=bill.date.strftime("%Y-%m-%d") %}Issued {{ date }}{% endtrans %}
-    {% elif None == bill.bill_number %}
-      <b>{% trans quotenumber=bill.quote_number %}Quote #{{ quotenumber }}{% endtrans %}</b><br>
-      {% trans date=bill.date.strftime("%Y-%m-%d") %}Generated {{ date }}{% endtrans %}
-    {% else %}
-      <b>{% trans billnumber = bill.bill_number %}Bill #{{ billnumber }}{% endtrans %}</b><br>
-      {% if bill.quote_number %}
-        {% trans quotenumber=bill.quote_number %}From quote #{{ quotenumber }}{% endtrans %}<br>
-        {% trans date=bill.date.strftime("%Y-%m-%d") %}Generated {{ date }}{% endtrans %}
-      {% endif %}
+    <b>{% trans billnumber = bill.bill_number %}Bill #{{ billnumber }}{% endtrans %}</b><br>
+    {% trans date=(bill.created_at or bill.bill_date).strftime("%Y-%m-%d") %}Generated {{ date }}{% endtrans %}<br>
+    {% if bill.quote_number %}
+      <b>{% trans quotenumber=bill.quote_number %}From quote #{{ quotenumber }}{% endtrans %}</b><br>
+      {% trans date=(bill.created_at or bill.quote_date).strftime("%Y-%m-%d") %}Generated {{ date }}{% endtrans %}
     {% endif %}
   </p>
 {% endblock %}
 
 {% block mentions %}
-  <pre>{{ bill.bill_mentions or '' }}</pre>
+  <p>{{ (bill.bill_mentions or '')|safe }}</p>
 {% endblock %}
```

## fossbill/templates/bill/generated_quote.html

```diff
@@ -1,149 +1,30 @@
-00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
-00000010: 3c68 746d 6c20 6c61 6e67 3d22 656e 223e  <html lang="en">
-00000020: 0a20 203c 6865 6164 3e0a 2020 2020 3c6d  .  <head>.    <m
-00000030: 6574 6120 6368 6172 7365 743d 2275 7466  eta charset="utf
-00000040: 2d38 223e 0a20 2020 203c 7469 746c 653e  -8">.    <title>
-00000050: 7b25 2062 6c6f 636b 2074 6974 6c65 2025  {% block title %
-00000060: 7d7b 2520 7472 616e 7320 7175 6f74 656e  }{% trans quoten
-00000070: 756d 6265 723d 6269 6c6c 2e71 756f 7465  umber=bill.quote
-00000080: 5f6e 756d 6265 7220 257d 5175 6f74 6520  _number %}Quote 
-00000090: 237b 7b20 7175 6f74 656e 756d 6265 7220  #{{ quotenumber 
-000000a0: 7d7d 7b25 2065 6e64 7472 616e 7320 257d  }}{% endtrans %}
-000000b0: 7b25 2065 6e64 626c 6f63 6b20 257d 3c2f  {% endblock %}</
-000000c0: 7469 746c 653e 0a20 2020 203c 6c69 6e6b  title>.    <link
-000000d0: 2072 656c 3d22 7374 796c 6573 6865 6574   rel="stylesheet
-000000e0: 2220 6872 6566 3d22 7b7b 2075 726c 5f66  " href="{{ url_f
-000000f0: 6f72 2827 7374 6174 6963 272c 2066 696c  or('static', fil
-00000100: 656e 616d 653d 2762 696c 6c2e 6373 7327  ename='bill.css'
-00000110: 2920 7d7d 223e 0a20 203c 2f68 6561 643e  ) }}">.  </head>
-00000120: 0a20 203c 626f 6479 3e0a 2020 2020 7b25  .  <body>.    {%
-00000130: 2062 6c6f 636b 2069 6465 6e74 6966 6965   block identifie
-00000140: 7220 257d 0a20 2020 2020 203c 6469 7620  r %}.      <div 
-00000150: 636c 6173 733d 2270 6572 736f 6e73 223e  class="persons">
-00000160: 0a20 2020 2020 2020 203c 7072 653e 3c62  .        <pre><b
-00000170: 3e7b 2520 7472 616e 7320 257d 4672 6f6d  >{% trans %}From
-00000180: 7b25 2065 6e64 7472 616e 7320 257d 3c2f  {% endtrans %}</
-00000190: 623e 0a7b 7b20 6269 6c6c 2e73 6f75 7263  b>.{{ bill.sourc
-000001a0: 6520 6f72 2027 2720 7d7d 3c2f 7072 653e  e or '' }}</pre>
-000001b0: 0a20 2020 2020 2020 203c 7072 653e 3c62  .        <pre><b
-000001c0: 3e7b 2520 7472 616e 7320 257d 546f 7b25  >{% trans %}To{%
-000001d0: 2065 6e64 7472 616e 7320 257d 3c2f 623e   endtrans %}</b>
-000001e0: 0a7b 7b20 6269 6c6c 2e72 6563 6970 6965  .{{ bill.recipie
-000001f0: 6e74 207d 7d3c 2f70 7265 3e0a 2020 2020  nt }}</pre>.    
-00000200: 2020 3c2f 6469 763e 0a20 2020 2020 203c    </div>.      <
-00000210: 703e 0a20 2020 2020 2020 207b 2520 6966  p>.        {% if
-00000220: 204e 6f6e 6520 3d3d 2062 696c 6c2e 7175   None == bill.qu
-00000230: 6f74 655f 6e75 6d62 6572 2025 7d0a 2020  ote_number %}.  
-00000240: 2020 2020 2020 2020 3c62 3e7b 2520 7472          <b>{% tr
-00000250: 616e 7320 257d 4472 6166 747b 2520 656e  ans %}Draft{% en
-00000260: 6474 7261 6e73 2025 7d3c 2f62 3e3c 6272  dtrans %}</b><br
-00000270: 3e0a 2020 2020 2020 2020 2020 7b25 2074  >.          {% t
-00000280: 7261 6e73 2064 6174 653d 6269 6c6c 2e64  rans date=bill.d
-00000290: 6174 652e 7374 7266 7469 6d65 2822 2559  ate.strftime("%Y
-000002a0: 2d25 6d2d 2564 2229 2025 7d47 656e 6572  -%m-%d") %}Gener
-000002b0: 6174 6564 207b 7b20 6461 7465 207d 7d7b  ated {{ date }}{
-000002c0: 2520 656e 6474 7261 6e73 2025 7d0a 2020  % endtrans %}.  
-000002d0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-000002e0: 0a20 2020 2020 2020 2020 203c 623e 7b25  .          <b>{%
-000002f0: 2074 7261 6e73 2071 756f 7465 6e75 6d62   trans quotenumb
-00000300: 6572 3d62 696c 6c2e 7175 6f74 655f 6e75  er=bill.quote_nu
-00000310: 6d62 6572 2025 7d51 756f 7465 2023 7b7b  mber %}Quote #{{
-00000320: 2071 756f 7465 6e75 6d62 6572 207d 7d7b   quotenumber }}{
-00000330: 2520 656e 6474 7261 6e73 2025 7d3c 2f62  % endtrans %}</b
-00000340: 3e3c 6272 3e0a 2020 2020 2020 2020 2020  ><br>.          
-00000350: 7b25 2074 7261 6e73 2064 6174 653d 6269  {% trans date=bi
-00000360: 6c6c 2e64 6174 652e 7374 7266 7469 6d65  ll.date.strftime
-00000370: 2822 2559 2d25 6d2d 2564 2229 2025 7d49  ("%Y-%m-%d") %}I
-00000380: 7373 7565 6420 7b7b 2064 6174 6520 7d7d  ssued {{ date }}
-00000390: 7b25 2065 6e64 7472 616e 7320 257d 0a20  {% endtrans %}. 
-000003a0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-000003b0: 257d 0a20 2020 2020 203c 2f70 3e0a 2020  %}.      </p>.  
-000003c0: 2020 7b25 2065 6e64 626c 6f63 6b20 257d    {% endblock %}
-000003d0: 0a20 2020 203c 7461 626c 653e 0a20 2020  .    <table>.   
-000003e0: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-000003f0: 3c74 683e 7b25 2074 7261 6e73 2025 7d44  <th>{% trans %}D
-00000400: 6574 6169 6c7b 2520 656e 6474 7261 6e73  etail{% endtrans
-00000410: 2025 7d3c 2f74 683e 0a20 2020 2020 2020   %}</th>.       
-00000420: 203c 7468 3e7b 2520 7472 616e 7320 257d   <th>{% trans %}
-00000430: 5072 6963 657b 2520 656e 6474 7261 6e73  Price{% endtrans
-00000440: 2025 7d3c 2f74 683e 0a20 2020 2020 2020   %}</th>.       
-00000450: 203c 7468 3e7b 2520 7472 616e 7320 257d   <th>{% trans %}
-00000460: 5174 797b 2520 656e 6474 7261 6e73 2025  Qty{% endtrans %
-00000470: 7d3c 2f74 683e 0a20 2020 2020 2020 203c  }</th>.        <
-00000480: 7468 3e7b 2520 7472 616e 7320 257d 416d  th>{% trans %}Am
-00000490: 6f75 6e74 7b25 2065 6e64 7472 616e 7320  ount{% endtrans 
-000004a0: 257d 3c2f 7468 3e0a 2020 2020 2020 2020  %}</th>.        
-000004b0: 3c74 683e 7b25 2074 7261 6e73 2025 7d54  <th>{% trans %}T
-000004c0: 6178 7b25 2065 6e64 7472 616e 7320 257d  ax{% endtrans %}
-000004d0: 3c2f 7468 3e0a 2020 2020 2020 2020 3c74  </th>.        <t
-000004e0: 683e 7b25 2074 7261 6e73 2025 7d54 6f74  h>{% trans %}Tot
-000004f0: 616c 7b25 2065 6e64 7472 616e 7320 257d  al{% endtrans %}
-00000500: 3c2f 7468 3e0a 2020 2020 2020 3c2f 7472  </th>.      </tr
-00000510: 3e0a 2020 2020 2020 7b25 2066 6f72 2062  >.      {% for b
-00000520: 696c 6c5f 726f 7720 696e 2062 696c 6c5f  ill_row in bill_
-00000530: 726f 7773 2025 7d0a 2020 2020 2020 2020  rows %}.        
-00000540: 3c74 723e 0a20 2020 2020 2020 2020 203c  <tr>.          <
-00000550: 7464 3e7b 7b20 6269 6c6c 5f72 6f77 2e6c  td>{{ bill_row.l
-00000560: 6162 656c 207d 7d3c 2f74 643e 0a20 2020  abel }}</td>.   
-00000570: 2020 2020 2020 203c 7464 3e7b 7b20 2862         <td>{{ (b
-00000580: 696c 6c5f 726f 772e 7072 6963 6520 2f20  ill_row.price / 
-00000590: 3130 3029 207c 2072 6f75 6e64 2832 2c20  100) | round(2, 
-000005a0: 2766 6c6f 6f72 2729 207d 7d20 7b7b 2067  'floor') }} {{ g
-000005b0: 2e75 7365 725f 7072 6566 2e63 7572 7265  .user_pref.curre
-000005c0: 6e63 7920 6f72 2022 2220 7d7d 3c2f 7464  ncy or "" }}</td
-000005d0: 3e0a 2020 2020 2020 2020 2020 3c74 643e  >.          <td>
-000005e0: 7b7b 2062 696c 6c5f 726f 772e 7175 616e  {{ bill_row.quan
-000005f0: 7469 7479 207d 7d3c 2f74 643e 0a20 2020  tity }}</td>.   
-00000600: 2020 2020 2020 203c 7464 3e7b 7b20 2862         <td>{{ (b
-00000610: 696c 6c5f 726f 772e 6772 6f73 735f 616d  ill_row.gross_am
-00000620: 6f75 6e74 202f 2031 3030 2920 7c20 726f  ount / 100) | ro
-00000630: 756e 6428 322c 2027 666c 6f6f 7227 2920  und(2, 'floor') 
-00000640: 7d7d 207b 7b20 672e 7573 6572 5f70 7265  }} {{ g.user_pre
-00000650: 662e 6375 7272 656e 6379 206f 7220 2222  f.currency or ""
-00000660: 207d 7d3c 2f74 643e 0a20 2020 2020 2020   }}</td>.       
-00000670: 2020 203c 7464 3e7b 7b20 6269 6c6c 5f72     <td>{{ bill_r
-00000680: 6f77 2e74 6178 5f72 6174 6520 7d7d 2025  ow.tax_rate }} %
-00000690: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000006a0: 3c74 643e 7b7b 2028 2862 696c 6c5f 726f  <td>{{ ((bill_ro
-000006b0: 772e 6772 6f73 735f 616d 6f75 6e74 202b  w.gross_amount +
-000006c0: 2062 696c 6c5f 726f 772e 7461 785f 616d   bill_row.tax_am
-000006d0: 6f75 6e74 2920 2f20 3130 3029 207c 2072  ount) / 100) | r
-000006e0: 6f75 6e64 2832 2c20 2766 6c6f 6f72 2729  ound(2, 'floor')
-000006f0: 207d 7d20 7b7b 2067 2e75 7365 725f 7072   }} {{ g.user_pr
-00000700: 6566 2e63 7572 7265 6e63 7920 6f72 2022  ef.currency or "
-00000710: 2220 7d7d 3c2f 7464 3e0a 2020 2020 2020  " }}</td>.      
-00000720: 2020 3c2f 7472 3e0a 2020 2020 2020 7b25    </tr>.      {%
-00000730: 2065 6e64 666f 7220 257d 0a20 2020 203c   endfor %}.    <
-00000740: 2f74 6162 6c65 3e0a 2020 2020 3c70 3e0a  /table>.    <p>.
-00000750: 2020 2020 2020 3c62 3e7b 2520 7472 616e        <b>{% tran
-00000760: 7320 257d 416d 6f75 6e74 7b25 2065 6e64  s %}Amount{% end
-00000770: 7472 616e 7320 257d 3c2f 623e 207b 7b20  trans %}</b> {{ 
-00000780: 2862 696c 6c2e 6772 6f73 735f 616d 6f75  (bill.gross_amou
-00000790: 6e74 202f 2031 3030 2920 7c20 726f 756e  nt / 100) | roun
-000007a0: 6428 322c 2027 666c 6f6f 7227 2920 7d7d  d(2, 'floor') }}
-000007b0: 207b 7b20 672e 7573 6572 5f70 7265 662e   {{ g.user_pref.
-000007c0: 6375 7272 656e 6379 206f 7220 2222 207d  currency or "" }
-000007d0: 7d3c 6272 3e0a 2020 2020 2020 3c62 3e7b  }<br>.      <b>{
-000007e0: 2520 7472 616e 7320 257d 5461 7865 737b  % trans %}Taxes{
-000007f0: 2520 656e 6474 7261 6e73 2025 7d3c 2f62  % endtrans %}</b
-00000800: 3e20 7b7b 2028 6269 6c6c 2e74 6178 5f61  > {{ (bill.tax_a
-00000810: 6d6f 756e 7420 2f20 3130 3029 207c 2072  mount / 100) | r
-00000820: 6f75 6e64 2832 2c20 2766 6c6f 6f72 2729  ound(2, 'floor')
-00000830: 207d 7d20 7b7b 2067 2e75 7365 725f 7072   }} {{ g.user_pr
-00000840: 6566 2e63 7572 7265 6e63 7920 6f72 2022  ef.currency or "
-00000850: 2220 7d7d 3c62 723e 0a20 2020 2020 203c  " }}<br>.      <
-00000860: 623e 7b25 2074 7261 6e73 2025 7d54 6f74  b>{% trans %}Tot
-00000870: 616c 7b25 2065 6e64 7472 616e 7320 257d  al{% endtrans %}
-00000880: 3c2f 623e 207b 7b20 2862 696c 6c2e 616d  </b> {{ (bill.am
-00000890: 6f75 6e74 202f 2031 3030 2920 7c20 726f  ount / 100) | ro
-000008a0: 756e 6428 322c 2027 666c 6f6f 7227 2920  und(2, 'floor') 
-000008b0: 7d7d 207b 7b20 672e 7573 6572 5f70 7265  }} {{ g.user_pre
-000008c0: 662e 6375 7272 656e 6379 206f 7220 2222  f.currency or ""
-000008d0: 207d 7d3c 6272 3e0a 2020 2020 3c2f 703e   }}<br>.    </p>
-000008e0: 0a20 2020 207b 2520 626c 6f63 6b20 6d65  .    {% block me
-000008f0: 6e74 696f 6e73 2025 7d0a 2020 2020 2020  ntions %}.      
-00000900: 3c70 7265 3e7b 7b20 6269 6c6c 2e71 756f  <pre>{{ bill.quo
-00000910: 7465 5f6d 656e 7469 6f6e 7320 6f72 2027  te_mentions or '
-00000920: 2720 7d7d 3c2f 7072 653e 0a20 2020 207b  ' }}</pre>.    {
-00000930: 2520 656e 6462 6c6f 636b 2025 7d0a 2020  % endblock %}.  
-00000940: 3c2f 626f 6479 3e0a 3c2f 6874 6d6c 3e0a  </body>.</html>.
+00000000: 7b25 2065 7874 656e 6473 2027 6269 6c6c  {% extends 'bill
+00000010: 2f67 656e 6572 6174 6564 5f64 7261 6674  /generated_draft
+00000020: 2e68 746d 6c27 2025 7d0a 0a7b 2520 626c  .html' %}..{% bl
+00000030: 6f63 6b20 6964 656e 7469 6669 6572 2025  ock identifier %
+00000040: 7d0a 2020 3c64 6976 2063 6c61 7373 3d22  }.  <div class="
+00000050: 7065 7273 6f6e 7322 3e0a 2020 2020 3c70  persons">.    <p
+00000060: 7265 3e3c 623e 7b25 2074 7261 6e73 2025  re><b>{% trans %
+00000070: 7d46 726f 6d7b 2520 656e 6474 7261 6e73  }From{% endtrans
+00000080: 2025 7d3c 2f62 3e0a 7b7b 2062 696c 6c2e   %}</b>.{{ bill.
+00000090: 736f 7572 6365 206f 7220 2727 207d 7d3c  source or '' }}<
+000000a0: 2f70 7265 3e0a 2020 2020 3c70 7265 3e3c  /pre>.    <pre><
+000000b0: 623e 7b25 2074 7261 6e73 2025 7d54 6f7b  b>{% trans %}To{
+000000c0: 2520 656e 6474 7261 6e73 2025 7d3c 2f62  % endtrans %}</b
+000000d0: 3e0a 7b7b 2062 696c 6c2e 7265 6369 7069  >.{{ bill.recipi
+000000e0: 656e 7420 7d7d 3c2f 7072 653e 0a20 203c  ent }}</pre>.  <
+000000f0: 2f64 6976 3e0a 2020 3c70 3e0a 2020 2020  /div>.  <p>.    
+00000100: 3c62 3e7b 2520 7472 616e 7320 7175 6f74  <b>{% trans quot
+00000110: 656e 756d 6265 723d 6269 6c6c 2e71 756f  enumber=bill.quo
+00000120: 7465 5f6e 756d 6265 7220 257d 5175 6f74  te_number %}Quot
+00000130: 6520 237b 7b20 7175 6f74 656e 756d 6265  e #{{ quotenumbe
+00000140: 7220 7d7d 7b25 2065 6e64 7472 616e 7320  r }}{% endtrans 
+00000150: 257d 3c2f 623e 3c62 723e 0a20 2020 207b  %}</b><br>.    {
+00000160: 2520 7472 616e 7320 6461 7465 3d28 6269  % trans date=(bi
+00000170: 6c6c 2e71 756f 7465 5f64 6174 6520 6f72  ll.quote_date or
+00000180: 2062 696c 6c2e 6372 6561 7465 645f 6174   bill.created_at
+00000190: 292e 7374 7266 7469 6d65 2822 2559 2d25  ).strftime("%Y-%
+000001a0: 6d2d 2564 2229 2025 7d49 7373 7565 6420  m-%d") %}Issued 
+000001b0: 7b7b 2064 6174 6520 7d7d 7b25 2065 6e64  {{ date }}{% end
+000001c0: 7472 616e 7320 257d 0a20 203c 2f70 3e0a  trans %}.  </p>.
+000001d0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a    {% endblock %}.
```

## fossbill/templates/bill/index.html

```diff
@@ -7,97 +7,120 @@
   <a class="action" href="{{ url_for('bill.create') }}">{% trans %}New{% endtrans %}</a>
 {% endblock %}
 
 {% block content %}
   <label for="filter-hidder">{% trans %}Show filters{% endtrans %}</label>
   <input type="checkbox" id="filter-hidder" class="hidder" {% if filtered %}checked{% endif %}>
   <form class="filters">
-    <label for="quote_number__eq">{% trans %}Quote number{% endtrans %}</label>
-    <input name="quote_number__eq" id="quote_number__eq" type="number" min="0" step="1" {% if filtered %}autofocus{% endif %}
-      value="{{ request.args.get('quote_number__eq', '') }}">
-    <label for="bill_number__eq">{% trans %}Bill number{% endtrans %}</label>
-    <input name="bill_number__eq" id="bill_number__eq" type="number" min="0" step="1"
-      value="{{ request.args.get('bill_number__eq', '') }}">
-    <label for="date__date__ge">{% trans %}Date after{% endtrans %}</label>
-    <input name="date__date__ge" id="date__date__ge" type="date"
-      value="{{ request.args.get('date__date__ge', '') }}">
-    <label for="date__date__le">{% trans %}Date before{% endtrans %}</label>
-    <input name="date__date__le" id="date__date__le" type="date"
-      value="{{ request.args.get('date__date__le', '') }}">
-    <label for="amount__price__ge">{% trans %}Amount greater than{% endtrans %}</label>
-    <input name="amount__price__ge" id="amount__price__ge"
-      value="{{ request.args.get('amount__price__ge', '') }}">
-    <label for="amount__price__le">{% trans %}Amount lower than{% endtrans %}</label>
-    <input name="amount__price__le" id="amount__price__le"
-      value="{{ request.args.get('amount__price__le', '') }}">
-    <label for="recipient__ilike">{% trans %}Recipient{% endtrans %}</label>
-    <input name="recipient__ilike" id="recipient__ilike"
-      value="{{ request.args.get('recipient__ilike', '') }}">
-    <label for="1__select_custom">{% trans %}Type{% endtrans %}</label>
-    <select name="1__select_custom" id="1__select_custom" multiple>
-      <option value="bill_number__null__and__quote_number__null" {{ "selected" if ("bill_number__null__and__quote_number__null" in request.args.getlist('1__select_custom')) }}>{% trans %}Draft{% endtrans %}</option>
-      <option value="bill_number__not_null" {{ "selected" if ("bill_number__not_null" in request.args.getlist('1__select_custom')) }}>{% trans %}Bill{% endtrans %}</option>
-      <option value="quote_number__not_null" {{ "selected" if ("quote_number__not_null" in request.args.getlist('1__select_custom')) }}>{% trans %}Quote{% endtrans %}</option>
-    </select>
-    <label for="paid__eq">{% trans %}Is paid?{% endtrans %}</label>
-    <select name="paid__eq" id="paid__eq">
-      <option value="">{% trans %}Choose an option{% endtrans %}</option>
-      <option value="TRUE" {{ "selected" if ("TRUE" == request.args.get('paid__eq')) }}>{% trans %}Yes{% endtrans %}</option>
-      <option value="FALSE" {{ "selected" if ("FALSE" == request.args.get('paid__eq')) }}>{% trans %}No{% endtrans %}</option>
-    </select>
+    <div class="flex-align">
+      <div class="form">
+        <label for="quote_number__eq">{% trans %}Quote number{% endtrans %}</label>
+        <input name="quote_number__eq" id="quote_number__eq" type="number" min="0" step="1" {% if filtered %}autofocus{% endif %}
+          value="{{ request.args.get('quote_number__eq', '') }}">
+        <label for="bill_number__eq">{% trans %}Bill number{% endtrans %}</label>
+        <input name="bill_number__eq" id="bill_number__eq" type="number" min="0" step="1"
+          value="{{ request.args.get('bill_number__eq', '') }}">
+        <div class="flex-align">
+          <div class="form">
+            <label for="created_at__date__ge">{% trans %}Created after{% endtrans %}</label>
+            <input name="created_at__date__ge" id="created_at__date__ge" type="date"
+              value="{{ request.args.get('created_at__date__ge', '') }}">
+          </div>
+          <div class="form">
+            <label for="created_at__date__le">{% trans %}Created before{% endtrans %}</label>
+            <input name="created_at__date__le" id="created_at__date__le" type="date"
+              value="{{ request.args.get('created_at__date__le', '') }}">
+          </div>
+        </div>
+        <div class="flex-align">
+          <div class="form">
+            <label for="amount__price__ge">{% trans %}Amount greater than{% endtrans %}</label>
+            <input name="amount__price__ge" id="amount__price__ge"
+              value="{{ request.args.get('amount__price__ge', '') }}">
+          </div>
+          <div class="form">
+            <label for="amount__price__le">{% trans %}Amount lower than{% endtrans %}</label>
+            <input name="amount__price__le" id="amount__price__le"
+              value="{{ request.args.get('amount__price__le', '') }}">
+          </div>
+        </div>
+      </div>
+
+      <div class="form">
+        <label for="recipient__ilike">{% trans %}Recipient{% endtrans %}</label>
+        <input name="recipient__ilike" id="recipient__ilike"
+          value="{{ request.args.get('recipient__ilike', '') }}">
+        <label for="1__select_custom">{% trans %}Type{% endtrans %}</label>
+        <select name="1__select_custom" id="1__select_custom" multiple>
+          <option value="bill_number__null__and__quote_number__null" {{ "selected" if ("bill_number__null__and__quote_number__null" in request.args.getlist('1__select_custom')) }}>{% trans %}Draft{% endtrans %}</option>
+          <option value="bill_number__not_null" {{ "selected" if ("bill_number__not_null" in request.args.getlist('1__select_custom')) }}>{% trans %}Bill{% endtrans %}</option>
+          <option value="quote_number__not_null" {{ "selected" if ("quote_number__not_null" in request.args.getlist('1__select_custom')) }}>{% trans %}Quote{% endtrans %}</option>
+        </select>
+        <label for="paid__eq">{% trans %}Is paid?{% endtrans %}</label>
+        <select name="paid__eq" id="paid__eq">
+          <option value="">{% trans %}Choose an option{% endtrans %}</option>
+          <option value="TRUE" {{ "selected" if ("TRUE" == request.args.get('paid__eq')) }}>{% trans %}Yes{% endtrans %}</option>
+          <option value="FALSE" {{ "selected" if ("FALSE" == request.args.get('paid__eq')) }}>{% trans %}No{% endtrans %}</option>
+        </select>
+      </div>
+    </div>
     <div class="actions">
       <input type="submit" value="{% trans %}Filter{% endtrans %}">
       <a href="{{ url_for(".index") }}">{% trans %}Reset{% endtrans %}</a>
     </div>
   </form>
-  <table class="index">
-    <thead>
-      <tr>
-        <th>{% trans %}Quote number{% endtrans %}</th>
-        <th>{% trans %}Bill number{% endtrans %}</th>
-        <th>{% trans %}Date{% endtrans %}</th>
-        <th>{% trans %}Amount{% endtrans %}</th>
-        <th>{% trans %}Recipient{% endtrans %}</th>
-        <th>{% trans %}Action{% endtrans %}</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for bill in bills %}
+  <div class="table-cap">
+    <table class="index">
+      <thead>
+        <tr>
+          <th>{% trans %}Quote number{% endtrans %}</th>
+          <th>{% trans %}Bill number{% endtrans %}</th>
+          <th>{% trans %}Created at{% endtrans %}</th>
+          <th>{% trans %}Amount{% endtrans %}</th>
+          <th>{% trans %}Recipient{% endtrans %}</th>
+          <th>{% trans %}Action{% endtrans %}</th>
+        </tr>
+      </thead>
+      <tbody>
+        {% for bill in bills %}
+          <tr>
+            <td>
+              {% if None != bill.quote_number %}
+                {% trans quotenumber=bill.quote_number %}Quote #{{ quotenumber }}{% endtrans %}
+              {% endif %}
+            </td>
+            <td>
+              {% if None != bill.bill_number %}
+                {% trans billnumber=bill.bill_number %}Bill #{{ billnumber }}{% endtrans %}
+              {% endif %}
+            </td>
+            <td>{{ bill.created_at.strftime("%Y-%m-%d") }}</td>
+            <td>{{ (bill.amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
+            <td>{{ bill.recipient }}</td>
+            <td class="actions">
+              <a href="{{ url_for('bill.update', id=bill.id) }}">{% trans %}Edit{% endtrans %}</a>
+            </td>
+          </tr>
+        {% endfor %}
+      </tbody>
+    </table>
+  </div>
+  <div class="table-cap">
+    <table class="summary">
+      <thead>
         <tr>
-          <td>
-            {% if None != bill.quote_number %}
-              {% trans quotenumber=bill.quote_number %}Quote #{{ quotenumber }}{% endtrans %}
-            {% endif %}
-          </td>
-          <td>
-            {% if None != bill.bill_number %}
-              {% trans billnumber=bill.bill_number %}Bill #{{ billnumber }}{% endtrans %}
-            {% endif %}
-          </td>
-          <td>{{ bill.date.strftime("%Y-%m-%d") }}</td>
-          <td>{{ (bill.amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
-          <td>{% if bill.recipient|length > 30 %}{{ bill.recipient[:30].strip() }}…{% else %}{{ bill.recipient }}{% endif %}</td>
-          <td class="actions">
-            <a href="{{ url_for('bill.update', id=bill.id) }}">{% trans %}Show{% endtrans %}</a>
-          </td>
+          <th>{% trans %}Count{% endtrans %}</th>
+          <th>{% trans %}Gross amount{% endtrans %}</th>
+          <th>{% trans %}Tax amount{% endtrans %}</th>
+          <th>{% trans %}Amount{% endtrans %}</th>
         </tr>
-      {% endfor %}
-    </tbody>
-  </table>
-  <table class="summary">
-    <thead>
-      <tr>
-        <th>{% trans %}Count{% endtrans %}</th>
-        <th>{% trans %}Gross amount{% endtrans %}</th>
-        <th>{% trans %}Tax amount{% endtrans %}</th>
-        <th>{% trans %}Amount{% endtrans %}</th>
-      </tr>
-    </thead>
-    <tbody>
-      <td>{{ stats.count }}</td>
-      <td>{{ (stats.gross_amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
-      <td>{{ (stats.tax_amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
-      <td>{{ (stats.amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
-    </tbody>
-  </table>
+      </thead>
+      <tbody>
+        <td>{{ stats.count }}</td>
+        <td>{{ (stats.gross_amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
+        <td>{{ (stats.tax_amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
+        <td>{{ (stats.amount / 100) | round(2, 'floor') }} {{ g.user_pref.currency or "" }}</td>
+      </tbody>
+    </table>
+  </div>
   {{ paginate(pagination) if pagination.max > 1 }}
 {% endblock %}
```

### html2text {}

```diff
@@ -1,34 +1,43 @@
 {% from 'macros.html' import paginate %} {% extends 'base.html' %} {% block
 header %}
 ****** {% block title %}{% trans %}Bills{% endtrans %}{% endblock %} ******
 {%_trans_%}New{%_endtrans_%} {% endblock %} {% block content %} {% trans %}Show
 filters{% endtrans %}
 % if filtered %}checked{% endif %}>
 {% trans %}Quote number{% endtrans %}
+% if filtered %}autofocus{% endif %} value="{{ request.args.get
+('quote_number__eq', '') }}"> {% trans %}Bill number{% endtrans %} [Unknown
+INPUT type]
+{% trans %}Created after{% endtrans %} [Unknown INPUT type]
+{% trans %}Created before{% endtrans %} [Unknown INPUT type]
+{% trans %}Amount greater than{% endtrans %} [{{ request.args.get
+('amount__price__ge', '') }}]
+{% trans %}Amount lower than{% endtrans %} [{{ request.args.get
+('amount__price__le', '') }}]
 { "selected" if ("bill_number__null__and__quote_number__null" in
 request.args.getlist('1__select_custom')) }}>{% trans %}Draft{% endtrans %}
 { "selected" if ("bill_number__not_null" in request.args.getlist
 ('1__select_custom')) }}>{% trans %}Bill{% endtrans %}
 { "selected" if ("quote_number__not_null" in request.args.getlist
 ('1__select_custom')) }}>{% trans %}Quote{% endtrans %}
 { "selected" if ("TRUE" == request.args.get('paid__eq')) }}>{% trans %}Yes{%
 endtrans %}
 { "selected" if ("FALSE" == request.args.get('paid__eq')) }}>{% trans %}No{%
 endtrans %}
 [{% trans %}Filter{% endtrans %}]
 index") }}">{% trans %}Reset{% endtrans %}
-                                                                                                                                                                                                                                      {% trans
-{% trans %}Quote number{%     {% trans %}Bill number{%    {% trans %}Date{%                                                                                                                                                           %}Action
-endtrans %}                   endtrans %}                 endtrans %}        {% trans %}Amount{% endtrans %}                                             {% trans %}Recipient{% endtrans %}                                           {%
-                                                                                                                                                                                                                                      endtrans
-                                                                                                                                                                                                                                      %}
+                                                                                                                                                                              {% trans
+{% trans %}Quote number{%     {% trans %}Bill number{%    {% trans %}Created at{%                                                                              {% trans       %}Action
+endtrans %}                   endtrans %}                 endtrans %}              {% trans %}Amount{% endtrans %}                                             %}Recipient{%  {%
+                                                                                                                                                               endtrans %}    endtrans
+                                                                                                                                                                              %}
 {% if None !=                 {% if None !=
-bill.quote_number %} {% trans bill.bill_number %} {%      {                                                                                                                                                                           {%_trans
-quotenumber=bill.quote_number trans                       {                  {{ (bill.amount / 100) | round(2, 'floor') }}Â {{ g.user_pref.currency or {% if bill.recipient|length > 30 %}{{ bill.recipient[:30].strip() }}â¦{% %}Show{%
-%}Quote #{{ quotenumber }}{%  billnumber=bill.bill_number bill.date.strftime "" }}                                                                       else %}{{ bill.recipient }}{% endif %}                                       endtrans
-endtrans %} {% endif %}       %}Bill #{{ billnumber }}{%  ("%Y-%m-%d") }}                                                                                                                                                             %}
+bill.quote_number %} {% trans bill.bill_number %} {%      {                                                                                                    {              {%_trans
+quotenumber=bill.quote_number trans                       {                        {{ (bill.amount / 100) | round(2, 'floor') }}Â {{ g.user_pref.currency or {              %}Edit{%
+%}Quote #{{ quotenumber }}{%  billnumber=bill.bill_number bill.created_at.strftime "" }}                                                                       bill.recipient endtrans
+endtrans %} {% endif %}       %}Bill #{{ billnumber }}{%  ("%Y-%m-%d") }}                                                                                      }}             %}
                               endtrans %} {% endif %}
 {% trans %}Count{% {% trans %}Gross  {% trans %}Tax       {% trans %}Amount{%
 endtrans %}        amount{% endtrans amount{% endtrans %} endtrans %}
                    %}
 {{ paginate(pagination) if pagination.max > 1 }} {% endblock %}
```

## fossbill/templates/bill/send_bill_email.html

```diff
@@ -3,15 +3,16 @@
 {% block header %}
   <h1>{% block title %}{% trans %}Send bill email{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
     <label for="email">{% trans %}Email{% endtrans %}</label>
-    <input name="email" id="email" value="{{ request.form['email'] or client.email }}" autofocus>
+    <input name="email" id="email" value="{{ request.form['email'] or customer.email }}" autofocus>
     <label for="subject">{% trans %}Subject{% endtrans %}</label>
     <input name="subject" id="subject" value="{{ request.form['subject'] or default_subject }}">
     <label for="body">{% trans %}Body{% endtrans %}</label>
     <textarea name="body" id="body" rows=6>{{ request.form['body'] or default_body }}</textarea>
     <input type="submit" value="Send">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/bill/send_quote_email.html

```diff
@@ -3,15 +3,16 @@
 {% block header %}
   <h1>{% block title %}{% trans %}Send quote email{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
     <label for="email">{% trans %}Email{% endtrans %}</label>
-    <input name="email" id="email" value="{{ request.form['email'] or client.email }}" autofocus>
+    <input name="email" id="email" value="{{ request.form['email'] or customer.email }}" autofocus>
     <label for="subject">{% trans %}Subject{% endtrans %}</label>
     <input name="subject" id="subject" value="{{ request.form['subject'] or default_subject }}">
     <label for="body">{% trans %}Body{% endtrans %}</label>
     <textarea name="body" id="body" rows=6>{{ request.form['body'] or default_body }}</textarea>
     <input type="submit" value="Send">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/bill/update.html

```diff
@@ -1,149 +1,101 @@
 {% extends 'base.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans %}Edit draft{% endtrans %}{% endblock %}</h1>
+  <h1>{% block title %}{% trans %}Draft{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
-  <div class="flex-align">
-    {% block left_panel %}
-      <form method="post" id="bill_info">
-        <label for="client_id">{% trans %}Client{% endtrans %}</label>
-        <select name="client_id" id="client_id">
-          <option value="">{% trans %}Empty{% endtrans %}</option>
-          {% for client in clients %}
-            <option value="{{ client.id }}" {{ "selected" if bill.client_id == client.id }}>{{ client.label }}</option>
-          {% endfor %}
-        </select>
-
-        <label for="date">{% trans %}Date{% endtrans %}</label>
-        <input name="date" id="date" type="date"
-          value="{{ request.form['date'] or bill.date.strftime("%Y-%m-%d") }}">
-
-        <label for="recipient">{% trans %}Recipient{% endtrans %}</label>
-        <textarea name="recipient" id="recipient" rows="6" title="{% trans %}Taken from customer address.{% endtrans %}"
-          >{{ request.form['recipient'] or bill.recipient or '' }}</textarea>
-
-        <label for="source">{% trans %}Source{% endtrans %}</label>
-        <textarea name="source" id="source" rows="6" title="{% trans %}Taken from your user configuration.{% endtrans %}"
-          >{{ request.form['source'] or bill.source or '' }}</textarea>
+  <form method="post">
+    <div class="flex-align">
+      <div class="form">
+        {% block left_panel %}
+          <label for="customer_id">{% trans %}Customer{% endtrans %}</label>
+          <select name="customer_id" id="customer_id">
+            <option value="">{% trans %}Empty{% endtrans %}</option>
+            {% for customer in customers %}
+              <option value="{{ customer.id }}" {{ "selected" if bill.customer_id == customer.id }}>{{ customer.label }}</option>
+            {% endfor %}
+          </select>
+
+          <label for="recipient">{% trans %}Recipient{% endtrans %}</label>
+          <textarea name="recipient" id="recipient" rows="6" title="{% trans %}Taken from customer address.{% endtrans %}"
+            >{{ request.form['recipient'] or bill.recipient or '' }}</textarea>
+
+          <label for="source">{% trans %}Source{% endtrans %}</label>
+          <textarea name="source" id="source" rows="6" title="{% trans %}Taken from your user configuration.{% endtrans %}"
+            >{{ request.form['source'] or bill.source or '' }}</textarea>
+        {% endblock %}
+      </div>
+
+      <div class="form">
+        {% block mention_panel %}
+          <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
+          <textarea name="quote_mentions" id="quote_mentions" rows="5"
+             title="{% trans %}Taken from your user configuration.{% endtrans %}"
+            >{{ bill.quote_mentions or '' }}</textarea>
+          <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
+
+          <textarea name="bill_mentions" id="bill_mentions" rows="5"
+             title="{% trans %}Taken from your user configuration.{% endtrans %}"
+            >{{ bill.bill_mentions or '' }}</textarea>
+        {% endblock %}
 
-        <input type="submit" value="{% trans %}Save{% endtrans %}">
-      </form>
-    {% endblock %}
-
-    <div class="marged">
-      {% block bill_row_panel %}
-        {% if bill_rows|length > 0 %}
-          <table>
-            <thead>
-              <tr>
-                <th>{% trans %}Label{% endtrans %}</th>
-                <th>{% trans %}Price{% endtrans %}</th>
-                <th>{% trans %}Qty{% endtrans %}</th>
-                <th>{% trans %}Amount{% endtrans %}</th>
-                <th>{% trans %}Tax{% endtrans %}</th>
-                <th>{% trans %}Action{% endtrans %}</th>
-              </tr>
-            </thead>
-            <tbody>
-              {% for bill_row in bill_rows %}
-                <tr>
-                  <td id="bill_row_{{ bill_row.id }}">{{ bill_row.label }}</td>
-                  <td>{{ bill_row.price/100 }}</td>
-                  <td>{{ bill_row.quantity }}</td>
-                  <td>{{ (bill_row.gross_amount / 100) | round(2, 'floor') }}</td>
-                  <td>{{ bill_row.tax_rate }} %</td>
-                  <td class="actions">
-                    <a href="{{ url_for('bill.update', id=bill['id'], edit_bill_row_id=bill_row['id']) }}">{% trans %}Update{% endtrans %}</a>
-                    <form action="{{ url_for('bill.delete_row', id=bill_row['id']) }}" method="post">
-                      <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
-                    </form>
-                  </td>
-                </tr>
-              {% endfor %}
-            </tbody>
-          </table>
-        {% endif %}
-        {% if edit_bill_row %}
-          <form action="{{ url_for('bill.update_row', id=edit_bill_row['id']) }}" method="post">
-            <label for="label">{% trans %}Label{% endtrans %}</label>
-            <input name="label" id="label" value="{{ edit_bill_row.label }}" required autofocus>
-            <label for="price">{% trans %}Price{% endtrans %}</label>
-            <input name="price" id="price" type="number" step="0.01"" value="{{ edit_bill_row.price/100 }}" required>
-            <label for="tax_rate">{% trans %}Tax rate{% endtrans %}</label>
-            <input name="tax_rate" id="tax_rate" type="number" step="0.01" value="{{ edit_bill_row.tax_rate }}" max="100" min="0" required>
-            <label for="quantity">{% trans %}Qty{% endtrans %}</label>
-            <input name="quantity" id="quantity" type="number" value="{{ edit_bill_row.quantity }}" required>
-            <div class="actions">
-              <input type="submit" value="{% trans %}Save{% endtrans %}">
-              <a href="{{ url_for('bill.update', id=bill['id']) }}">{% trans %}Cancel{% endtrans %}</a>
-            </div>
-          </form>
-        {% endif %}
-        <div class="flex-align">
-          <form action="{{ url_for('bill.create_row', id=bill['id']) }}" method="post"
-            title="{% trans %}Add a row from an existing product.{% endtrans %}">
-            <label for="product_id">{% trans %}Product{% endtrans %}</label>
-            <select name="product_id" id="product_id">
-              {% for product in products %}
-                <option value="{{ product.id }}">{{ product.label }} - {{ product.price/100 }}</option>
-              {% endfor %}
-            </select>
-            <label for="quantity2">{% trans %}Quantity{% endtrans %}</label>
-            <input name="quantity" id="quantity2" type="number" required>
-            <input type="submit" value="{% trans %}Create row{% endtrans %}">
-          </form>
-          <form action="{{ url_for('bill.create_row', id=bill['id']) }}" method="post" class="marged"
-            title="{% trans %}Add a row from scratch.{% endtrans %}">
-            <label for="label">{% trans %}Label{% endtrans %}</label>
-            <input name="label" id="label" required>
-            <label for="price">{% trans %}Price{% endtrans %}</label>
-            <input name="price" id="price" type="number" step="0.01" required>
-            <label for="tax_rate">{% trans %}Tax rate{% endtrans %}</label>
-            <input name="tax_rate" id="tax_rate" type="number" step="0.01" max="100" min="0" required>
-            <label for="quantity">{% trans %}Quantity{% endtrans %}</label>
-            <input name="quantity" id="quantity" type="number" required>
-            <input type="submit" value="{% trans %}Create row{% endtrans %}">
-          </form>
-        </div>
-      {% endblock %}
-      <form action="{{ url_for('bill.update_comment', id=bill['id']) }}" id="bill_comment" method="post">
         <label for="comment">{% trans %}Comment{% endtrans %}</label>
         <textarea name="comment" id="comment" rows="5">{{ bill.comment or '' }}</textarea>
-        <input type="submit" value="{% trans %}Save{% endtrans %}">
-      </form>
+      </div>
     </div>
-  </div>
-
-  {% block mention_panel %}
-    <form action="{{ url_for('bill.update_mentions', id=bill['id']) }}" id="bill_mentions" method="post">
-      <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
-      <textarea name="quote_mentions" id="quote_mentions" rows="5"
-         title="{% trans %}Taken from your user configuration.{% endtrans %}"
-        >{{ bill.quote_mentions or '' }}</textarea>
-      <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
-      <textarea name="bill_mentions" id="bill_mentions" rows="5"
-         title="{% trans %}Taken from your user configuration.{% endtrans %}"
-        >{{ bill.bill_mentions or '' }}</textarea>
-      <input type="submit" value="{% trans %}Save{% endtrans %}">
-    </form>
+    <input type="submit" value="{% trans %}Save{% endtrans %}">
+    {{ csrf_token()|safe }}
+  </form>
+
+  {% block bill_row_panel %}
+    {% if bill_rows|length > 0 %}
+      <div class="table-cap">
+        <table class="index" id="bill_rows">
+          <thead>
+            <tr>
+              <th>{% trans %}Label{% endtrans %}</th>
+              <th>{% trans %}Price{% endtrans %}</th>
+              <th>{% trans %}Qty{% endtrans %}</th>
+              <th>{% trans %}Amount{% endtrans %}</th>
+              <th>{% trans %}Tax{% endtrans %}</th>
+              <th>{% trans %}Action{% endtrans %}</th>
+            </tr>
+          </thead>
+          <tbody>
+            {% for bill_row in bill_rows %}
+              <tr>
+                <td id="bill_row_{{ bill_row.id }}">{{ bill_row.label }}</td>
+                <td>{{ bill_row.price/100 }}</td>
+                <td>{{ bill_row.quantity }}</td>
+                <td>{{ (bill_row.gross_amount / 100) | round(2, 'floor') }}</td>
+                <td>{{ bill_row.tax_rate }} %</td>
+                <td class="actions">
+                  <a href="{{ url_for('bill.update_row', bill_id=bill['id'], id=bill_row['id']) }}">{% trans %}Edit{% endtrans %}</a>
+                  <form action="{{ url_for('bill.delete_row', id=bill_row['id']) }}" method="post">
+                    <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+                    {{ csrf_token()|safe }}
+                  </form>
+                </td>
+              </tr>
+            {% endfor %}
+          </tbody>
+        </table>
+      </div>
+    {% endif %}
+    <a href="{{ url_for('bill.create_row', id=bill['id']) }}">{% trans %}Create row{% endtrans %}</a>
   {% endblock %}
 
   <hr>
 
   {% block actions %}
     <div class="actions">
-      <a href="{{ url_for('bill.view_quote_pdf', id=bill['id']) }}">{% trans %}Preview quote{% endtrans %}</a>
-      <form action="{{ url_for('bill.create_quote', id=bill['id']) }}" method="post">
-        <input type="submit" value="{% trans %}Create quote{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
-      </form>
-      <form action="{{ url_for('bill.create_bill', id=bill['id']) }}" method="post">
-        <input type="submit" value="{% trans %}Create bill{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
-      </form>
+      <a href="{{ url_for('bill.view_draft_pdf', id=bill['id']) }}">{% trans %}View draft{% endtrans %}</a>
+      <a href="{{ url_for('bill.finish', id=bill['id']) }}">{% trans %}Finish draft{% endtrans %}</a>
       <form action="{{ url_for('bill.delete', id=bill['id']) }}" method="post">
         <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+        {{ csrf_token()|safe }}
       </form>
     </div>
   {% endblock %}
 {% endblock %}
```

### html2text {}

```diff
@@ -1,66 +1,40 @@
 {% extends 'base.html' %} {% block header %}
-****** {% block title %}{% trans %}Edit draft{% endtrans %}{% endblock %}
-******
+****** {% block title %}{% trans %}Draft{% endtrans %}{% endblock %} ******
 {% endblock %} {% block content %}
-{% block left_panel %}
-{% for client in clients %}
-{ "selected" if bill.client_id == client.id }}>{{ client.label }}
+{% for customer in customers %}
+{ "selected" if bill.customer_id == customer.id }}>{{ customer.label }}
 {% endfor %}
- {% trans %}Date{% endtrans %}
-Y-%m-%d") }}"> {% trans %}Recipient{% endtrans %}
+ {% trans %}Recipient{% endtrans %}
 {{ request.form['recipient'] or bill.recipient or '' }}
  {% trans %}Source{% endtrans %}
 {{ request.form['source'] or bill.source or '' }}
- [{% trans %}Save{% endtrans %}]
-{% endblock %}
+ {% endblock %}
+{% block mention_panel %} {% trans %}Quote mentions{% endtrans %}
+{{ bill.quote_mentions or '' }}
+ {% trans %}Bill mentions{% endtrans %}
+{{ bill.bill_mentions or '' }}
+ {% endblock %} {% trans %}Comment{% endtrans %}
+{{ bill.comment or '' }}
+[{% trans %}Save{% endtrans %}] {{ csrf_token()|safe }}
 {% block bill_row_panel %} {% if bill_rows|length > 0 %}
-                                                                                          {% trans
-{% trans       {% trans        {% trans %}Qty{%  {% trans %}Amount{%    {% trans %}Tax{%  %}Action
-%}Label{%      %}Price{%       endtrans %}       endtrans %}            endtrans %}       {%
-endtrans %}    endtrans %}                                                                endtrans
+{% trans       {% trans                                                                   {% trans
+%}Label{%      %}Price{%       {% trans %}Qty{%  {% trans %}Amount{%    {% trans %}Tax{%  %}Action{%
+endtrans %}    endtrans %}     endtrans %}       endtrans %}            endtrans %}       endtrans
                                                                                           %}
                                                                                           {%_trans
-                                                                                          %}Update
-                                                                                          {%
-{              {               {                 {{                     {                 endtrans
-{              {               {                 (bill_row.gross_amount {                 %}
-bill_row.label bill_row.price/ bill_row.quantity / 100) | round(2,      bill_row.tax_rate [{%
-}}             100 }}          }}                'floor') }}            }} %              trans
-                                                                                          %}Delete
-                                                                                          {%
+                                                                                          %}Edit{%
                                                                                           endtrans
-                                                                                          %}]
-{% endif %} {% if edit_bill_row %}
-{% trans %}Label{% endtrans %} [{{ edit_bill_row.label }}] {% trans %}Price{%
-endtrans %}
- value="{{ edit_bill_row.price/100 }}" required> {% trans %}Tax rate{% endtrans
-%} [Unknown INPUT type] {% trans %}Qty{% endtrans %} [Unknown INPUT type]
-[{% trans %}Save{% endtrans %}] {%_trans_%}Cancel{%_endtrans_%}
-{% endif %}
-{% for product in products %}
-{{ product.label }} - {{ product.price/100 }}
-{% endfor %}
- {% trans %}Quantity{% endtrans %} [Unknown INPUT type] [{% trans %}Create row
-{% endtrans %}]
-{% trans %}Label{% endtrans %} [label               ] {% trans %}Price{%
-endtrans %} [Unknown INPUT type] {% trans %}Tax rate{% endtrans %} [Unknown
-INPUT type] {% trans %}Quantity{% endtrans %} [Unknown INPUT type] [{% trans
-%}Create row{% endtrans %}]
-{% endblock %}
-{% trans %}Comment{% endtrans %}
-{{ bill.comment or '' }}
- [{% trans %}Save{% endtrans %}]
-{% block mention_panel %}
-{% trans %}Quote mentions{% endtrans %}
-{{ bill.quote_mentions or '' }}
- {% trans %}Bill mentions{% endtrans %}
-{{ bill.bill_mentions or '' }}
- [{% trans %}Save{% endtrans %}]
-{% endblock %}
+{              {               {                 {{                     {                 %}
+{              {               {                 (bill_row.gross_amount {                 [{% trans
+bill_row.label bill_row.price/ bill_row.quantity / 100) | round(2,      bill_row.tax_rate %}Delete{%
+}}             100 }}          }}                'floor') }}            }} %              endtrans
+                                                                                          %}] {
+                                                                                          {
+                                                                                          csrf_token
+                                                                                          ()|safe }}
+{% endif %} {%_trans_%}Create_row{%_endtrans_%} {% endblock %}
 ===============================================================================
 {% block actions %}
-{%_trans_%}Preview_quote{%_endtrans_%}
-[{% trans %}Create quote{% endtrans %}]
-[{% trans %}Create bill{% endtrans %}]
-[{% trans %}Delete{% endtrans %}]
+{%_trans_%}View_draft{%_endtrans_%} {%_trans_%}Finish_draft{%_endtrans_%}
+[{% trans %}Delete{% endtrans %}] {{ csrf_token()|safe }}
 {% endblock %} {% endblock %}
```

## fossbill/templates/bill/update_bill.html

```diff
@@ -1,21 +1,33 @@
 {% extends 'bill/update_quote.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans billnumber=bill.bill_number %}Edit bill "#{{ billnumber }}"{% endtrans %}{% endblock %}</h1>
+  <h1>{% block title %}{% trans billnumber=bill.bill_number %}Bill #{{ billnumber }}{% endtrans %}{% endblock %}</h1>
+{% endblock %}
+
+{% block left_panel %}
+  {{ super() }}
+
+  <label for="paid">{% trans %}Is paid?{% endtrans %}</label>
+  <select name="paid" id="paid" type="checkbox">
+    <option value="1" {% if request.form['paid'] == "1" or bill.paid %}selected{% endif %}>{% trans %}Yes{% endtrans %}</option>
+    <option value="0" {% if request.form['paid'] != "1" and not bill.paid %}selected{% endif %}>{% trans %}No{% endtrans %}</option>
+  </select>
+{% endblock %}
+
+{% block mention_panel %}
+  <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
+  <textarea name="quote_mentions" id="quote_mentions" rows="5" disabled>{{ bill.quote_mentions or '' }}</textarea>
+  <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
+  <textarea name="bill_mentions" id="bill_mentions" rows="5" disabled>{{ bill.bill_mentions or '' }}</textarea>
 {% endblock %}
 
 {% block actions %}
   <div class="actions">
     {% if bill.quote_number %}
       <a href="{{ url_for('bill.view_quote_pdf', id=bill['id']) }}">{% trans %}View quote{% endtrans %}</a>
       <a href="{{ url_for('bill.send_quote_email', id=bill['id']) }}">{% trans %}Send quote email{% endtrans %}</a>
     {% endif %}
     <a href="{{ url_for('bill.view_bill_pdf', id=bill['id']) }}">{% trans %}View bill{% endtrans %}</a>
     <a href="{{ url_for('bill.send_bill_email', id=bill['id']) }}">{% trans %}Send bill email{% endtrans %}</a>
-    {% if not bill.paid %}
-      <form action="{{ url_for('bill.mark_paid', id=bill['id']) }}" method="post">
-        <input type="submit" value="{% trans %}Mark as paid{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
-      </form>
-    {% endif %}
   </div>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,10 +1,17 @@
 {% extends 'bill/update_quote.html' %} {% block header %}
-****** {% block title %}{% trans billnumber=bill.bill_number %}Edit bill "#{
-{ billnumber }}"{% endtrans %}{% endblock %} ******
-{% endblock %} {% block actions %}
+****** {% block title %}{% trans billnumber=bill.bill_number %}Bill #{
+{ billnumber }}{% endtrans %}{% endblock %} ******
+% if request.form['paid'] == "1" or bill.paid %}selected{% endif %}>{% trans
+%}Yes{% endtrans %}
+% if request.form['paid'] != "1" and not bill.paid %}selected{% endif %}>{%
+trans %}No{% endtrans %}
+ {% endblock %} {% block mention_panel %} {% trans %}Quote mentions{% endtrans
+%}
+{{ bill.quote_mentions or '' }}
+ {% trans %}Bill mentions{% endtrans %}
+{{ bill.bill_mentions or '' }}
+ {% endblock %} {% block actions %}
 {% if bill.quote_number %} {%_trans_%}View_quote{%_endtrans_%} {%_trans_%}Send
 quote_email{%_endtrans_%} {% endif %} {%_trans_%}View_bill{%_endtrans_%} {%
-trans_%}Send_bill_email{%_endtrans_%} {% if not bill.paid %}
-[{% trans %}Mark as paid{% endtrans %}]
-{% endif %}
+trans_%}Send_bill_email{%_endtrans_%}
 {% endblock %}
```

## fossbill/templates/bill/update_quote.html

```diff
@@ -1,79 +1,71 @@
 {% extends 'bill/update.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans quotenumber=bill.quote_number %}Edit quote "#{{ quotenumber }}"{% endtrans %}{% endblock %}</h1>
+  <h1>{% block title %}{% trans quotenumber=bill.quote_number %}Quote #{{ quotenumber }}{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block left_panel %}
-  <form method="post" id="bill_info">
-    <label for="client_id">{% trans %}Client{% endtrans %}</label>
-    <select name="client_id" id="client_id" disabled>
-      <option value="">{% trans %}Empty{% endtrans %}</option>
-      {% for client in clients %}
-        <option value="{{ client.id }}" {{ "selected" if bill.client_id == client.id }}>{{ client.label }}</option>
-      {% endfor %}
-    </select>
-
-    <label for="date">{% trans %}Date{% endtrans %}</label>
-    <input name="date" id="date" type="date" disabled
-      value="{{ request.form['date'] or bill.date.strftime("%Y-%m-%d") }}">
-
-    <label for="recipient">{% trans %}Recipient{% endtrans %}</label>
-    <textarea name="recipient" id="recipient" rows="6" disabled>{{ request.form['recipient'] or bill.recipient or '' }}</textarea>
-
-    <label for="source">{% trans %}Source{% endtrans %}</label>
-    <textarea name="source" id="source" rows="6" disabled>{{ request.form['source'] or bill.source or '' }}</textarea>
-  </form>
+  <label for="customer_id">{% trans %}Customer{% endtrans %}</label>
+  <select name="customer_id" id="customer_id" disabled>
+    <option value="">{% trans %}Empty{% endtrans %}</option>
+    {% for customer in customers %}
+      <option value="{{ customer.id }}" {{ "selected" if bill.customer_id == customer.id }}>{{ customer.label }}</option>
+    {% endfor %}
+  </select>
+
+  <label for="recipient">{% trans %}Recipient{% endtrans %}</label>
+  <textarea name="recipient" id="recipient" rows="6" disabled>{{ request.form['recipient'] or bill.recipient or '' }}</textarea>
+
+  <label for="source">{% trans %}Source{% endtrans %}</label>
+  <textarea name="source" id="source" rows="6" disabled>{{ request.form['source'] or bill.source or '' }}</textarea>
+{% endblock %}
+
+{% block mention_panel %}
+  <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
+  <textarea name="quote_mentions" id="quote_mentions" rows="5" disabled>{{ bill.quote_mentions or '' }}</textarea>
+  <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
+  <textarea name="bill_mentions" id="bill_mentions" rows="5">{{ bill.bill_mentions or '' }}</textarea>
 {% endblock %}
 
 {% block bill_row_panel %}
-  <table>
-    <thead>
-      <tr>
-        <th>{% trans %}Label{% endtrans %}</th>
-        <th>{% trans %}Price{% endtrans %}</th>
-        <th>{% trans %}Qty{% endtrans %}</th>
-        <th>{% trans %}Amount{% endtrans %}</th>
-        <th>{% trans %}Tax{% endtrans %}</th>
-        <th>{% trans %}Total{% endtrans %}</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for bill_row in bill_rows %}
+  <div class="table-cap">
+    <table class="index">
+      <thead>
         <tr>
-          <td id="bill_row_{{ bill_row.id }}">{{ bill_row.label }}</td>
-          <td>{{ bill_row.price/100 }}</td>
-          <td>{{ bill_row.quantity }}</td>
-          <td>{{ (bill_row.gross_amount / 100) | round(2, 'floor') }}</td>
-          <td>{{ bill_row.tax_rate }} %</td>
-          <td>{{ ((bill_row.gross_amount + bill_row.tax_amount) / 100) | round(2, 'floor') }}</td>
+          <th>{% trans %}Label{% endtrans %}</th>
+          <th>{% trans %}Price{% endtrans %}</th>
+          <th>{% trans %}Qty{% endtrans %}</th>
+          <th>{% trans %}Amount{% endtrans %}</th>
+          <th>{% trans %}Tax{% endtrans %}</th>
+          <th>{% trans %}Total{% endtrans %}</th>
         </tr>
-      {% endfor %}
-    </tbody>
-    <tfoot>
-      <td colspan="3"></td>
-      <td>{{ (bill.gross_amount / 100) | round(2, 'floor') }}</td>
-      <td>{{ (bill.tax_amount / 100) | round(2, 'floor') }}</td>
-      <td>{{ (bill.amount / 100) | round(2, 'floor') }}</td>
-    </tfoot>
-  </table>
-{% endblock %}
-
-{% block mention_panel %}
-  <form action="{{ url_for('bill.update_mentions', id=bill['id']) }}" id="bill_mentions" method="post">
-    <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
-    <textarea name="quote_mentions" id="quote_mentions" rows="5" disabled>{{ bill.quote_mentions or '' }}</textarea>
-    <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
-    <textarea name="bill_mentions" id="bill_mentions" rows="5" disabled>{{ bill.bill_mentions or '' }}</textarea>
-  </form>
+      </thead>
+      <tbody>
+        {% for bill_row in bill_rows %}
+          <tr>
+            <td id="bill_row_{{ bill_row.id }}">{{ bill_row.label }}</td>
+            <td>{{ bill_row.price/100 }}</td>
+            <td>{{ bill_row.quantity }}</td>
+            <td>{{ (bill_row.gross_amount / 100) | round(2, 'floor') }}</td>
+            <td>{{ bill_row.tax_rate }} %</td>
+            <td>{{ ((bill_row.gross_amount + bill_row.tax_amount) / 100) | round(2, 'floor') }}</td>
+          </tr>
+        {% endfor %}
+      </tbody>
+      <tfoot>
+        <td colspan="3"></td>
+        <td>{{ (bill.gross_amount / 100) | round(2, 'floor') }}</td>
+        <td>{{ (bill.tax_amount / 100) | round(2, 'floor') }}</td>
+        <td>{{ (bill.amount / 100) | round(2, 'floor') }}</td>
+      </tfoot>
+    </table>
+  </div>
 {% endblock %}
 
 {% block actions %}
   <div class="actions">
     <a href="{{ url_for('bill.view_quote_pdf', id=bill['id']) }}">{% trans %}View quote{% endtrans %}</a>
     <a href="{{ url_for('bill.send_quote_email', id=bill['id']) }}">{% trans %}Send quote email{% endtrans %}</a>
-    <form action="{{ url_for('bill.create_bill', id=bill['id']) }}" method="post">
-      <input type="submit" value="{% trans %}Create bill{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
-    </form>
+    <a href="{{ url_for('bill.finish', id=bill['id']) }}">{% trans %}Finish quote{% endtrans %}</a>
   </div>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,30 +1,28 @@
 {% extends 'bill/update.html' %} {% block header %}
-****** {% block title %}{% trans quotenumber=bill.quote_number %}Edit quote "#{
-{ quotenumber }}"{% endtrans %}{% endblock %} ******
-{% endblock %} {% block left_panel %}
-{% for client in clients %}
-{ "selected" if bill.client_id == client.id }}>{{ client.label }}
+****** {% block title %}{% trans quotenumber=bill.quote_number %}Quote #{
+{ quotenumber }}{% endtrans %}{% endblock %} ******
+{% for customer in customers %}
+{ "selected" if bill.customer_id == customer.id }}>{{ customer.label }}
 {% endfor %}
- {% trans %}Date{% endtrans %}
-Y-%m-%d") }}"> {% trans %}Recipient{% endtrans %}
+ {% trans %}Recipient{% endtrans %}
 {{ request.form['recipient'] or bill.recipient or '' }}
  {% trans %}Source{% endtrans %}
 {{ request.form['source'] or bill.source or '' }}
-{% endblock %} {% block bill_row_panel %}
+ {% endblock %} {% block mention_panel %} {% trans %}Quote mentions{% endtrans
+%}
+{{ bill.quote_mentions or '' }}
+ {% trans %}Bill mentions{% endtrans %}
+{{ bill.bill_mentions or '' }}
+ {% endblock %} {% block bill_row_panel %}
 {% trans       {% trans        {% trans %}Qty{%  {% trans %}Amount{%    {% trans %}Tax{%  {% trans %}Total{%
 %}Label{%      %}Price{%       endtrans %}       endtrans %}            endtrans %}       endtrans %}
 endtrans %}    endtrans %}
 {              {               {                 {{                     {                 {{ (
 {              {               {                 (bill_row.gross_amount {                 (bill_row.gross_amount
 bill_row.label bill_row.price/ bill_row.quantity / 100) | round(2,      bill_row.tax_rate + bill_row.tax_amount)
 }}             100 }}          }}                'floor') }}            }} %              / 100) | round(2,
                                                                                           'floor') }}
-{% endblock %} {% block mention_panel %}
-{% trans %}Quote mentions{% endtrans %}
-{{ bill.quote_mentions or '' }}
- {% trans %}Bill mentions{% endtrans %}
-{{ bill.bill_mentions or '' }}
 {% endblock %} {% block actions %}
 {%_trans_%}View_quote{%_endtrans_%} {%_trans_%}Send_quote_email{%_endtrans_%}
-[{% trans %}Create bill{% endtrans %}]
+{%_trans_%}Finish_quote{%_endtrans_%}
 {% endblock %}
```

## fossbill/templates/landing/dashboard.html

```diff
@@ -2,11 +2,11 @@
 
 {% block header %}
   <h1>{% block title %}{% trans %}Dashboard{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <p>{% trans %}Thanks a lot for registering, and welcome aboard! Fossbill is a really simple tool. Here some guidelines:{% endtrans %}</p>
-  <p>{% trans %}You should start by editing your user preference. Then add some products you use frequently. You can also prepare your client list. Registering products and clients isnt necessary but it make generating bills faster.{% endtrans %}</p>
+  <p>{% trans %}You should start by editing your user preference. Then add some products you use frequently. You can also prepare your customer list. Registering products and customers isnt necessary but it make generating bills faster.{% endtrans %}</p>
   <p>{% trans %}Bills will be Drafts untill you generate a Quote or directly a Bill from them. Unique numbers will be applied on them.{% endtrans %}</p>
   <p>{% trans %}You can preview and also send them to any email address you want, as quote or bill.{% endtrans %}</p>
 {% endblock %}
```

## fossbill/templates/product/create.html

```diff
@@ -16,10 +16,16 @@
       value="{{ request.form['price'] }}"
       type="number" step="0.01" required>
     <label for="tax_rate">{% trans %}Tax rate{% endtrans %}</label>
     <input name="tax_rate" id="tax_rate"
       placeholder="{% trans %}Ex: 20.0{% endtrans %}" title="{% trans %}Ex: 20.0{% endtrans %}"
       value="{{ request.form['tax_rate'] }}"
       type="number" step="0.01" max="100" min="0" required>
-    <input type="submit" value="{% trans %}Save{% endtrans %}">
+    <div class="actions">
+      <input type="submit" value="{% trans %}Save{% endtrans %}">
+      <label for="create_another">{% trans %}Create another?{% endtrans %}</label>
+      <input name="create_another" id="create_another"
+        {% if request.form.get('create_another') or request.args.get('create_another') %} checked{% endif %} type="checkbox">
+    </div>
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## fossbill/templates/product/index.html

```diff
@@ -10,48 +10,62 @@
 {% block content %}
   <label for="filter-hidder">{% trans %}Show filters{% endtrans %}</label>
   <input type="checkbox" id="filter-hidder" class="hidder" {% if filtered %}checked{% endif %}>
   <form class="filters">
     <label for="label__ilike">{% trans %}Label{% endtrans %}</label>
     <input name="label__ilike" id="label__ilike" {% if filtered %}autofocus{% endif %}
       value="{{ request.args.get('label__ilike', '') }}">
-    <label for="price__price__ge">{% trans %}Price greater than{% endtrans %}</label>
-    <input name="price__price__ge" id="price__price__ge" type="number" step="0.01" min="0"
-      value="{{ request.args.get('price__price__ge', '') }}">
-    <label for="price__price__le">{% trans %}Price lower than{% endtrans %}</label>
-    <input name="price__price__le" id="price__price__le" type="number" step="0.01" min="0"
-      value="{{ request.args.get('price__price__le', '') }}">
-    <label for="tax_rate__ge">{% trans %}Tax rate greater than{% endtrans %}</label>
-    <input name="tax_rate__ge" id="tax_rate__ge" type="number" step="0.01" max="100" min="0"
-      value="{{ request.args.get('tax_rate__ge', '') }}">
-    <label for="tax_rate__le">{% trans %}Tax rate lower than{% endtrans %}</label>
-    <input name="tax_rate__le" id="tax_rate__le" type="number" step="0.01" max="100" min="0"
-      value="{{ request.args.get('tax_rate__le', '') }}">
+    <div class="flex-align">
+      <div class="form">
+        <label for="price__price__ge">{% trans %}Price greater than{% endtrans %}</label>
+        <input name="price__price__ge" id="price__price__ge" type="number" step="0.01" min="0"
+          value="{{ request.args.get('price__price__ge', '') }}">
+      </div>
+      <div class="form">
+        <label for="price__price__le">{% trans %}Price lower than{% endtrans %}</label>
+        <input name="price__price__le" id="price__price__le" type="number" step="0.01" min="0"
+          value="{{ request.args.get('price__price__le', '') }}">
+      </div>
+    </div>
+    <div class="flex-align">
+      <div class="form">
+      <label for="tax_rate__ge">{% trans %}Tax rate greater than{% endtrans %}</label>
+      <input name="tax_rate__ge" id="tax_rate__ge" type="number" step="0.01" max="100" min="0"
+        value="{{ request.args.get('tax_rate__ge', '') }}">
+      </div>
+      <div class="form">
+      <label for="tax_rate__le">{% trans %}Tax rate lower than{% endtrans %}</label>
+      <input name="tax_rate__le" id="tax_rate__le" type="number" step="0.01" max="100" min="0"
+        value="{{ request.args.get('tax_rate__le', '') }}">
+      </div>
+    </div>
     <div class="actions">
       <input type="submit" value="{% trans %}Filter{% endtrans %}">
       <a href="{{ url_for(".index") }}">{% trans %}Reset{% endtrans %}</a>
     </div>
   </form>
-  <table class="index">
-    <thead>
-      <tr>
-        <th>{% trans %}Label{% endtrans %}</th>
-        <th>{% trans %}Price{% endtrans %}</th>
-        <th>{% trans %}Tax rate{% endtrans %}</th>
-        <th>{% trans %}Action{% endtrans %}</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for product in products %}
+  <div class="table-cap">
+    <table class="index">
+      <thead>
         <tr>
-          <td>{{ product.label }}</td>
-          <td>{{ product.price / 100 }}</td>
-          <td>{{ product.tax_rate }}</td>
-          <td class="actions">
-            <a href="{{ url_for('product.update', id=product.id) }}">{% trans %}Show{% endtrans %}</a>
-          </td>
+          <th>{% trans %}Label{% endtrans %}</th>
+          <th>{% trans %}Price{% endtrans %}</th>
+          <th>{% trans %}Tax rate{% endtrans %}</th>
+          <th>{% trans %}Action{% endtrans %}</th>
         </tr>
-      {% endfor %}
-    </tbody>
-  </table>
+      </thead>
+      <tbody>
+        {% for product in products %}
+          <tr>
+            <td>{{ product.label }}</td>
+            <td>{{ product.price / 100 }}</td>
+            <td>{{ product.tax_rate }}</td>
+            <td class="actions">
+              <a href="{{ url_for('product.update', id=product.id) }}">{% trans %}Edit{% endtrans %}</a>
+            </td>
+          </tr>
+        {% endfor %}
+      </tbody>
+    </table>
+  </div>
   {{ paginate(pagination) if pagination.max > 1 }}
 {% endblock %}
```

### html2text {}

```diff
@@ -2,18 +2,19 @@
 header %}
 ****** {% block title %}{% trans %}Products{% endtrans %}{% endblock %} ******
 {%_trans_%}New{%_endtrans_%} {% endblock %} {% block content %} {% trans %}Show
 filters{% endtrans %}
 % if filtered %}checked{% endif %}>
 {% trans %}Label{% endtrans %}
 % if filtered %}autofocus{% endif %} value="{{ request.args.get('label__ilike',
-'') }}"> {% trans %}Price greater than{% endtrans %} [Unknown INPUT type] {%
-trans %}Price lower than{% endtrans %} [Unknown INPUT type] {% trans %}Tax rate
-greater than{% endtrans %} [Unknown INPUT type] {% trans %}Tax rate lower than
-{% endtrans %} [Unknown INPUT type]
+'') }}">
+{% trans %}Price greater than{% endtrans %} [Unknown INPUT type]
+{% trans %}Price lower than{% endtrans %} [Unknown INPUT type]
+{% trans %}Tax rate greater than{% endtrans %} [Unknown INPUT type]
+{% trans %}Tax rate lower than{% endtrans %} [Unknown INPUT type]
 [{% trans %}Filter{% endtrans %}]
 index") }}">{% trans %}Reset{% endtrans %}
 {% trans %}Label{%  {% trans %}Price{% {% trans %}Tax rate {% trans %}Action{%
 endtrans %}         endtrans %}        {% endtrans %}      endtrans %}
-{{ product.label }} {{ product.price / {{ product.tax_rate {%_trans_%}Show{%
+{{ product.label }} {{ product.price / {{ product.tax_rate {%_trans_%}Edit{%
                     100 }}             }}                  endtrans_%}
 {{ paginate(pagination) if pagination.max > 1 }} {% endblock %}
```

## fossbill/templates/product/update.html

```diff
@@ -15,13 +15,15 @@
       placeholder="{% trans %}Ex: 499.99{% endtrans %}" title="{% trans %}Ex: 499.99{% endtrans %}"
       value="{{ request.form['price'] or product.price / 100 }}" type="number" step="0.01" required>
     <label for="tax_rate">{% trans %}Tax rate{% endtrans %}</label>
     <input name="tax_rate" id="tax_rate"
       placeholder="{% trans %}Ex: 20.0{% endtrans %}" title="{% trans %}Ex: 20.0{% endtrans %}"
       value="{{ request.form['tax_rate'] or product.tax_rate }}" type="number" step="0.01" max="100" min="0" required>
     <input type="submit" value="{% trans %}Save{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
   <hr>
   <form action="{{ url_for('product.delete', id=product['id']) }}" method="post">
     <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## Comparing `fossbill/client.py` & `fossbill/customer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, url_for
 )
 from werkzeug.exceptions import abort
 from fossbill.auth import login_required
 from fossbill.database import get_db, paginatestmt, pagination, filterstmt
-from sqlalchemy import insert, select, func
+from sqlalchemy import insert, select, desc
 from sqlalchemy.exc import SQLAlchemyError
 
-bp = Blueprint('client', __name__, url_prefix='/clients')
+bp = Blueprint('customer', __name__, url_prefix='/customers')
 
 @bp.route('/')
 @login_required
 def index():
     engine, metadata = get_db()
-    clients = metadata.tables['client']
-    stmt = select(clients).where(
-        clients.c.user_id == g.user.id,
-    )
+    customers = metadata.tables['customer']
+    stmt = select(customers).where(
+        customers.c.user_id == g.user.id,
+    ).order_by(desc(customers.c.id))
     stmt, filtered = filterstmt(stmt, request)
     stmt, countstmt = paginatestmt(stmt, request)
     try:
         with engine.connect() as conn:
             result = conn.execute(stmt)
             count = conn.execute(countstmt)
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         error = f"Something went wrong."
-        clients = []
+        customers = []
         count = 0
     else:
-        clients = result.fetchall()
+        customers = result.fetchall()
         count = count.fetchone().count
 
     return render_template(
-        'client/index.html',
-        clients=clients,
+        'customer/index.html',
+        customers=customers,
         pagination=pagination(count, request),
         filtered=filtered,
     )
 
 @bp.route('/create', methods=('GET', 'POST'))
 @login_required
 def create():
@@ -49,121 +49,124 @@
             error = _('Label is required.')
 
         if error is not None:
             flash(error)
         else:
             engine, metadata = get_db()
 
-            stmt = insert(metadata.tables['client']).values(
+            stmt = insert(metadata.tables['customer']).values(
                 address=request.form['address'],
                 email=request.form['email'],
                 label=request.form['label'],
                 user_id=g.user.id,
             )
             try:
                 with engine.connect() as conn:
                     result = conn.execute(stmt)
                     conn.commit()
             except SQLAlchemyError as e:
                 current_app.logger.error(str(e))
                 error = f"Something went wrong."
             else:
-                flash(_("Client created."))
-                return redirect(url_for("client.index"))
+                flash(_("Customer created."))
+                if request.form.get('create_another'):
+                    return redirect(url_for("customer.create", create_another=True))
+                else:
+                    return redirect(url_for("customer.index"))
 
             flash(error)
 
-    return render_template('client/create.html')
+    return render_template('customer/create.html')
 
-def get_client(id, user_id):
+def get_customer(id, user_id):
     engine, metadata = get_db()
-    clients = metadata.tables['client']
-    stmt = select(clients).where(
-        clients.c.id == id,
-        clients.c.user_id == user_id,
+    customers = metadata.tables['customer']
+    stmt = select(customers).where(
+        customers.c.id == id,
+        customers.c.user_id == user_id,
     )
     try:
         with engine.connect() as conn:
             result = conn.execute(stmt)
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         abort(500, f"Something went wrong.")
     else:
-        client = result.fetchone()
+        customer = result.fetchone()
 
-    if client is None:
-        abort(404, f"Client id {id} doesn't exist.")
+    if customer is None:
+        abort(404, f"Customer id {id} doesn't exist.")
 
-    return client
+    return customer
 
 @bp.route('/<int:id>/update', methods=('GET', 'POST'))
 @login_required
 def update(id):
-    client = get_client(id, g.user.id)
+    customer = get_customer(id, g.user.id)
 
     if request.method == 'POST':
         error = None
 
         if not request.form['label']:
             error = _('Label is required.')
 
         if error is not None:
             flash(error)
         else:
             engine, metadata = get_db()
-            clients = metadata.tables['client']
+            customers = metadata.tables['customer']
 
-            stmt = clients.update().values(
+            stmt = customers.update().values(
                 address=request.form['address'],
                 email=request.form['email'],
                 label=request.form['label'],
             ).where(
-                clients.c.id == id,
-                clients.c.user_id == g.user.id,
+                customers.c.id == id,
+                customers.c.user_id == g.user.id,
             )
             try:
                 with engine.connect() as conn:
                     result = conn.execute(stmt)
                     conn.commit()
             except SQLAlchemyError as e:
                 current_app.logger.error(str(e))
                 error = f"Something went wrong."
             else:
-                flash(_("Client updated."))
-                return redirect(url_for("client.index"))
+                flash(_("Customer updated."))
+                return redirect(url_for("customer.index"))
 
-    return render_template('client/update.html', client=client)
+    return render_template('customer/update.html', customer=customer)
 
 @bp.route('/<int:id>/delete', methods=('POST',))
 @login_required
 def delete(id):
     engine, metadata = get_db()
-    clients = metadata.tables['client']
+    customers = metadata.tables['customer']
 
-    stmt = clients.delete().where(
-        clients.c.id == id,
-        clients.c.user_id == g.user.id,
+    stmt = customers.delete().where(
+        customers.c.id == id,
+        customers.c.user_id == g.user.id,
     )
     try:
         with engine.connect() as conn:
             result = conn.execute(stmt)
             conn.commit()
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         flash(_("Something went wrong."))
-        return redirect(url_for('client.index'))
+        return redirect(url_for('customer.index'))
     else:
-        flash(_("Client deleted."))
-        return redirect(url_for('client.index'))
+        flash(_("Customer deleted."))
+        return redirect(url_for('customer.index'))
 
-def get_clients(user_id):
+def get_customers(user_id):
     engine, metadata = get_db()
-    clients = metadata.tables['client']
-    stmt = select(clients).where(
-        clients.c.user_id == user_id,
+    customers = metadata.tables['customer']
+    stmt = select(customers).where(
+        customers.c.user_id == user_id,
     )
     try:
         with engine.connect() as conn:
             result = conn.execute(stmt)
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         abort(500, f"Something went wrong.")
```

## Comparing `fossbill/templates/client/create.html` & `fossbill/templates/customer/update.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 {% extends 'base.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans %}New Client{% endtrans %}{% endblock %}</h1>
+  <h1>{% block title %}{% trans customerlabel=customer.label %}Edit "{{ customerlabel }}"{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
     <label for="label">{% trans %}Label{% endtrans %}</label>
     <input name="label" id="label"
       placeholder="{% trans %}Ex: John Doe{% endtrans %}" title="{% trans %}Ex: John Doe{% endtrans %}"
-      value="{{ request.form['label'] }}" required autofocus>
+      value="{{ request.form['label'] or customer.label }}" required autofocus>
     <label for="email">{% trans %}Email{% endtrans %}</label>
     <input name="email" id="email"
       placeholder="{% trans %}Ex: John Doe <contact@john-doe.com>{% endtrans %}" title="{% trans %}Ex: John Doe <contact@john-doe.com>{% endtrans %}"
-      value="{{ request.form['email'] }}">
+      value="{{ request.form['email'] or customer.email }}">
     <label for="address">{% trans %}Address{% endtrans %}</label>
     <textarea name="address" id="address" rows="6"
       placeholder="{% trans %}Ex: John Doe
 221 B Baker street,
 London, United Kingdom
 SIREN: 508 102 811{% endtrans %}" title="{% trans %}Ex: John Doe
 221 B Baker street,
 London, United Kingdom
 SIREN: 508 102 811{% endtrans %}"
-      >{{ request.form['address'] }}</textarea>
-    <input type="submit" value="Save">
+      >{{ request.form['address'] or customer.address }}</textarea>
+    <input type="submit" value="{% trans %}Save{% endtrans %}">
+    {{ csrf_token()|safe }}
+  </form>
+  <hr>
+  <form action="{{ url_for('customer.delete', id=customer['id']) }}" method="post">
+    <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## Comparing `fossbill/templates/client/index.html` & `fossbill/templates/customer/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% from 'macros.html' import paginate %}
 
 {% extends 'base.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans %}Clients{% endtrans %}{% endblock %}</h1>
-  <a class="action" href="{{ url_for('client.create') }}">{% trans %}New{% endtrans %}</a>
+  <h1>{% block title %}{% trans %}Customers{% endtrans %}{% endblock %}</h1>
+  <a class="action" href="{{ url_for('customer.create') }}">{% trans %}New{% endtrans %}</a>
 {% endblock %}
 
 {% block content %}
   <label for="filter-hidder">{% trans %}Show filters{% endtrans %}</label>
   <input type="checkbox" id="filter-hidder" class="hidder" {% if filtered %}checked{% endif %}>
   <form class="filters">
     <label for="label__ilike">{% trans %}Label{% endtrans %}</label>
@@ -21,31 +21,33 @@
     <input name="address__ilike" id="address__ilike"
       value="{{ request.args.get('address__ilike', '') }}">
     <div class="actions">
       <input type="submit" value="{% trans %}Filter{% endtrans %}">
       <a href="{{ url_for(".index") }}">{% trans %}Reset{% endtrans %}</a>
     </div>
   </form>
-  <table class="index">
-    <thead>
-      <tr>
-        <th>{% trans %}Label{% endtrans %}</th>
-        <th>{% trans %}Email{% endtrans %}</th>
-        <th>{% trans %}Address{% endtrans %}</th>
-        <th>{% trans %}Action{% endtrans %}</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for client in clients %}
+  <div class="table-cap">
+    <table class="index">
+      <thead>
         <tr>
-          <td>{{ client.label }}</td>
-          <td>{{ client.email }}</td>
-          <td>{{ client.address[:30].strip() }}…</td>
-          <td class="actions">
-            <a href="{{ url_for('client.update', id=client.id) }}">{% trans %}Show{% endtrans %}</a>
-          </td>
+          <th>{% trans %}Label{% endtrans %}</th>
+          <th>{% trans %}Email{% endtrans %}</th>
+          <th>{% trans %}Address{% endtrans %}</th>
+          <th>{% trans %}Action{% endtrans %}</th>
         </tr>
-      {% endfor %}
-    </tbody>
-  </table>
+      </thead>
+      <tbody>
+        {% for customer in customers %}
+          <tr>
+            <td>{{ customer.label }}</td>
+            <td>{{ customer.email }}</td>
+            <td>{{ customer.address[:30].strip() }}…</td>
+            <td class="actions">
+              <a href="{{ url_for('customer.update', id=customer.id) }}">{% trans %}Edit{% endtrans %}</a>
+            </td>
+          </tr>
+        {% endfor %}
+      </tbody>
+    </table>
+  </div>
   {{ paginate(pagination) if pagination.max > 1 }}
 {% endblock %}
```

### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% from 'macros.html' import paginate %} {% extends 'base.html' %} {% block
 header %}
-****** {% block title %}{% trans %}Clients{% endtrans %}{% endblock %} ******
+****** {% block title %}{% trans %}Customers{% endtrans %}{% endblock %} ******
 {%_trans_%}New{%_endtrans_%} {% endblock %} {% block content %} {% trans %}Show
 filters{% endtrans %}
 % if filtered %}checked{% endif %}>
 {% trans %}Label{% endtrans %}
 % if filtered %}autofocus{% endif %} value="{{ request.args.get('label__ilike',
 '') }}"> {% trans %}Email{% endtrans %} [{{ request.args.get('email__ilike',
 '') }}] {% trans %}Address{% endtrans %} [{{ request.args.get('address__ilike',
 '') }}]
 [{% trans %}Filter{% endtrans %}]
 index") }}">{% trans %}Reset{% endtrans %}
-{% trans %}Label{% {% trans %}Email{% {% trans %}Address{% {% trans %}Action{%
-endtrans %}        endtrans %}        endtrans %}          endtrans %}
-{{ client.label }} {{ client.email }} {{ client.address[:  {%_trans_%}Show{%
-                                      30].strip() }}â¦ endtrans_%}
+{% trans %}Label{% {% trans %}Email{% {% trans %}Address{%   {% trans %}Action
+endtrans %}        endtrans %}        endtrans %}            {% endtrans %}
+{{ customer.label  {{ customer.email  {{ customer.address[:  {%_trans_%}Edit{%
+}}                 }}                 30].strip() }}â¦   endtrans_%}
 {{ paginate(pagination) if pagination.max > 1 }} {% endblock %}
```

## Comparing `fossbill/templates/client/update.html` & `fossbill/templates/customer/create.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 {% extends 'base.html' %}
 
 {% block header %}
-  <h1>{% block title %}{% trans clientlabel=client.label %}Edit "{{ clientlabel }}"{% endtrans %}{% endblock %}</h1>
+  <h1>{% block title %}{% trans %}New Customer{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
     <label for="label">{% trans %}Label{% endtrans %}</label>
     <input name="label" id="label"
       placeholder="{% trans %}Ex: John Doe{% endtrans %}" title="{% trans %}Ex: John Doe{% endtrans %}"
-      value="{{ request.form['label'] or client.label }}" required autofocus>
+      value="{{ request.form['label'] }}" required autofocus>
     <label for="email">{% trans %}Email{% endtrans %}</label>
     <input name="email" id="email"
       placeholder="{% trans %}Ex: John Doe <contact@john-doe.com>{% endtrans %}" title="{% trans %}Ex: John Doe <contact@john-doe.com>{% endtrans %}"
-      value="{{ request.form['email'] or client.email }}">
+      value="{{ request.form['email'] }}">
     <label for="address">{% trans %}Address{% endtrans %}</label>
     <textarea name="address" id="address" rows="6"
       placeholder="{% trans %}Ex: John Doe
 221 B Baker street,
 London, United Kingdom
 SIREN: 508 102 811{% endtrans %}" title="{% trans %}Ex: John Doe
 221 B Baker street,
 London, United Kingdom
 SIREN: 508 102 811{% endtrans %}"
-      >{{ request.form['address'] or client.address }}</textarea>
-    <input type="submit" value="{% trans %}Save{% endtrans %}">
-  </form>
-  <hr>
-  <form action="{{ url_for('client.delete', id=client['id']) }}" method="post">
-    <input class="danger" type="submit" value="{% trans %}Delete{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+      >{{ request.form['address'] }}</textarea>
+    <div class="actions">
+      <input type="submit" value="{% trans %}Save{% endtrans %}">
+      <label for="create_another">{% trans %}Create another?{% endtrans %}</label>
+      <input name="create_another" id="create_another"
+        {% if request.form.get('create_another') or request.args.get('create_another') %} checked{% endif %} type="checkbox">
+    </div>
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

## Comparing `fossbill/templates/payment/home.html` & `fossbill/templates/payment/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,45 +10,49 @@
     <label for="card-element" style="font-weight: bold">
       {% trans %}Payment details{% endtrans %}
     </label>
     <div id="card-element"></div>
     <div id="card-error"></div>
     <input type="hidden" name="stripe_token" id="stripe-token" />
     <input type="submit" value="{% if g.user.stripe_customer %}{% trans %}New card{% endtrans %}{% else %}{% trans %}Save card{% endtrans %}{% endif %}">
+    {{ csrf_token()|safe }}
   </form>
   {% if g.user.stripe_customer %}
     <form action="{{ url_for('payment.drop_payment_methods') }}" method="post">
       <input class="danger" type="submit" value="{% trans %}Delete payment method{% endtrans %}" onclick="return confirm('{% trans %}Are you sure?{% endtrans %}');">
+      {{ csrf_token()|safe }}
     </form>
   {% endif %}
 
   {% if payments|length %}
-    <table class="index">
-      <thead>
-        <tr>
-          <th>{% trans %}Date{% endtrans %}</th>
-          <th>{% trans %}Amount{% endtrans %}</th>
-          <th>{% trans %}Card{% endtrans %}</th>
-          <th>{% trans %}Action{% endtrans %}</th>
-        </tr>
-      </thead>
-      <tbody>
-        {% for payment in payments %}
+    <div class="table-cap">
+      <table class="index">
+        <thead>
           <tr>
-            <td>{{ payment.date }}</td>
-            <td>{{ (payment.amount / 100) | round(2, 'floor') }} {{ payment.currency }}</td>
-            <td>{% trans cardbrand=payment.payload['payment_method_details']['card']['brand']|capitalize, last4=payment.payload['payment_method_details']['card']['last4'] %}{{ cardbrand }} ending with {{ last4 }}{% endtrans %}</td>
-            <td class="actions">
-              <a href="{{ url_for('payment.invoice_pdf', id=payment.id) }}">{% trans %}Invoice{% endtrans %}</a>
-              <a href="{{ payment.payload['receipt_url'] }}">{% trans %}Receipt{% endtrans %}</a>
-            </td>
+            <th>{% trans %}Date{% endtrans %}</th>
+            <th>{% trans %}Amount{% endtrans %}</th>
+            <th>{% trans %}Card{% endtrans %}</th>
+            <th>{% trans %}Action{% endtrans %}</th>
           </tr>
-        {% endfor %}
-      </tbody>
-    </table>
+        </thead>
+        <tbody>
+          {% for payment in payments %}
+            <tr>
+              <td>{{ payment.date }}</td>
+              <td>{{ (payment.amount / 100) | round(2, 'floor') }} {{ payment.currency }}</td>
+              <td>{% trans cardbrand=payment.payload['payment_method_details']['card']['brand']|capitalize, last4=payment.payload['payment_method_details']['card']['last4'] %}{{ cardbrand }} ending with {{ last4 }}{% endtrans %}</td>
+              <td class="actions">
+                <a href="{{ url_for('payment.invoice_pdf', id=payment.id) }}">{% trans %}Invoice{% endtrans %}</a>
+                <a href="{{ payment.receipt_url or payment.payload['receipt_url'] }}">{% trans %}Receipt{% endtrans %}</a>
+              </td>
+            </tr>
+          {% endfor %}
+        </tbody>
+      </table>
+    </div>
   {% endif %}
 
   <script src="https://js.stripe.com/v3/?advancedFraudSignals=false"></script> 
   <script> 
   document.getElementById('payment-form').style.display = 'block'; 
   var stripe = Stripe('{{config.get('STRIPE_PUBLISHABLE_KEY')}}');
   var elements = stripe.elements();
```

## Comparing `fossbill/templates/user/import_export_user.html` & `fossbill/templates/me/import_export_user.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 {% extends 'base.html' %}
 
 {% block header %}
   <h1>{% block title %}{% trans %}Import / Export{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
-  <form method="post" id="bill_info" action="{{ url_for('user.import_user') }}" enctype="multipart/form-data">
+  <form method="post" action="{{ url_for('me.import_user') }}" enctype="multipart/form-data">
     <label for="file">{% trans %}File{% endtrans %}</label>
     <input name="file" id="file" type="file" accept=".tar.bz2" required>
     <div class="flex actions">
       <input type="submit" value="{% trans %}Import{% endtrans %}">
-      <a href="{{ url_for('user.export_user') }}">{% trans %}Export{% endtrans %}</a>
+      <a href="{{ url_for('me.export_user') }}">{% trans %}Export{% endtrans %}</a>
     </div>
+    {{ csrf_token()|safe }}
   </form>
 {% endblock %}
```

### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends 'base.html' %} {% block header %}
 ****** {% block title %}{% trans %}Import / Export{% endtrans %}{% endblock %}
 ******
 {% endblock %} {% block content %}
 {% trans %}File{% endtrans %} [File]
 [{% trans %}Import{% endtrans %}] {%_trans_%}Export{%_endtrans_%}
+{{ csrf_token()|safe }}
 {% endblock %}
```

## Comparing `fossbill/templates/user/update.html` & `fossbill/templates/me/update.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,104 +2,114 @@
 
 {% block header %}
   <h1>{% block title %}{% trans username=g.user.username %}Edit "{{ username }}"{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <form method="post">
-    <label for="locale">{% trans %}Locale{% endtrans %}</label>
-    <select name="locale" id="locale">
-      {% for value, label in {"en_US": _("English"), "fr_FR": _("French")}.items() %}
-        <option value="{{ value }}" {{ "selected" if (request.form['locale'] or g.user_pref.locale) == value }}>{{ label }}</option>
-      {% endfor %}
-    </select>
-
-    <label for="email">{% trans %}Email{% endtrans %}</label>
-    <input name="email" id="email" maxlength="254"
-      title="{% trans %}Used for password recovery. Must be unique.{% endtrans %}"
-      placeholder="{% trans %}Used for password recovery. Must be unique.{% endtrans %}"
-      value="{{ request.form['email'] or g.user_pref.email or "" }}">
-
-    <label for="currency">{% trans %}Currency{% endtrans %}</label>
-    <input name="currency" id="currency" maxlength="10"
-      title="{% trans %}Ex: ${% endtrans %}"
-      placeholder="{% trans %}Ex: ${% endtrans %}"
-      value="{{ request.form['currency'] or g.user_pref.currency or "" }}">
-
-    <label for="source">{% trans %}Default source{% endtrans %}</label>
-    <textarea name="source" id="source" rows="6" maxlength="500"
-      title="{% trans %}The top-left part on generated bills. Represent your company.{% endtrans %}"
-      placeholder="{% trans %}The top-left part on generated bills. Represent your company.{% endtrans %}"
-      >{{ request.form['source'] or g.user_pref.source or "" }}</textarea>
-
-    <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
-    <textarea name="quote_mentions" id="quote_mentions" rows="6" maxlength="500"
-      title="{% trans %}Bottom text on generated quotes.{% endtrans %}"
-      placeholder="{% trans %}Bottom text on generated quotes.{% endtrans %}"
-      >{{ request.form['quote_mentions'] or g.user_pref.quote_mentions or "" }}</textarea>
-
-    <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
-    <textarea name="bill_mentions" id="bill_mentions" rows="6" maxlength="500"
-      title="{% trans %}Bottom text on generated bills.{% endtrans %}"
-      placeholder="{% trans %}Bottom text on generated bills.{% endtrans %}"
-      >{{ request.form['bill_mentions'] or g.user_pref.bill_mentions or "" }}</textarea>
-
-    <label for="smtp_host">{% trans %}SMTP host{% endtrans %}</label>
-    <input name="smtp_host" id="smtp_host" maxlength="30"
-      title="{% trans %}Ex: smtp.foo.bar{% endtrans %}"
-      placeholder="{% trans %}Ex: smtp.foo.bar{% endtrans %}"
-      value="{{ request.form['smtp_host'] or g.user_pref.smtp_host or "" }}">
-
-    <label for="smtp_port">{% trans %}SMTP port{% endtrans %}</label>
-    <input name="smtp_port" id="smtp_port" type="number"
-      title="{% trans %}Ex: 465{% endtrans %}"
-      placeholder="{% trans %}Ex: 465{% endtrans %}"
-      value="{{ request.form['smtp_port'] or g.user_pref.smtp_port or "" }}">
-
-    <label for="smtp_security">{% trans %}SMTP security{% endtrans %}</label>
-    <select name="smtp_security" id="smtp_security">
-      <option value="" {{ "selected" if not (request.form['smtp_security'] or g.user_pref.smtp_security) }}>{% trans %}Select an option{% endtrans %}</option>
-      {% for protocol in ["TLS", "STARTTLS"] %}
-        <option value="{{ protocol }}" {{ "selected" if (request.form['smtp_security'] or g.user_pref.smtp_security) == protocol }}>{{ protocol }}</option>
-      {% endfor %}
-    </select>
-
-    <label for="smtp_username">{% trans %}SMTP username{% endtrans %}</label>
-    <input name="smtp_username" id="smtp_username" maxlength="30"
-      title="{% trans %}Ex: <no-reply@john-doe.com>{% endtrans %}"
-      placeholder="{% trans %}Ex: <no-reply@john-doe.com>{% endtrans %}"
-      value="{{ request.form['smtp_username'] or g.user_pref.smtp_username or "" }}">
-
-    <label for="smtp_password">{% trans %}SMTP password{% endtrans %}</label>
-    <input name="smtp_password" id="smtp_password" type="password" maxlength="30"
-      value="{{ request.form['smtp_password'] or g.user_pref.smtp_password or "" }}">
-
-    <label for="smtp_reply_to">{% trans %}SMTP reply-to{% endtrans %}</label>
-    <input name="smtp_reply_to" id="smtp_reply_to" type="reply_to" maxlength="254"
-      title="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
-      placeholder="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
-      value="{{ request.form['smtp_reply_to'] or g.user_pref.smtp_reply_to or "" }}">
-
-    <label for="smtp_cc">{% trans %}SMTP cc{% endtrans %}</label>
-    <input name="smtp_cc" id="smtp_cc" type="reply_to" maxlength="508"
-      title="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
-      placeholder="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
-      value="{{ request.form['smtp_cc'] or g.user_pref.smtp_cc or "" }}">
+    <div class="flex-align">
+      <div class="form">
+        <label for="locale">{% trans %}Locale{% endtrans %}</label>
+        <select name="locale" id="locale">
+          {% for value, label in {"en_US": _("English"), "fr_FR": _("French")}.items() %}
+            <option value="{{ value }}" {{ "selected" if (request.form['locale'] or g.user_pref.locale) == value }}>{{ label }}</option>
+          {% endfor %}
+        </select>
+
+        <label for="email">{% trans %}Email{% endtrans %}</label>
+        <input name="email" id="email" maxlength="254"
+          title="{% trans %}Used for password recovery. Must be unique.{% endtrans %}"
+          placeholder="{% trans %}Used for password recovery. Must be unique.{% endtrans %}"
+          value="{{ request.form['email'] or g.user_pref.email or "" }}">
+
+        <label for="currency">{% trans %}Currency{% endtrans %}</label>
+        <input name="currency" id="currency" maxlength="10"
+          title="{% trans %}Ex: ${% endtrans %}"
+          placeholder="{% trans %}Ex: ${% endtrans %}"
+          value="{{ request.form['currency'] or g.user_pref.currency or "" }}">
+
+        <label for="source">{% trans %}Default source{% endtrans %}</label>
+        <textarea name="source" id="source" rows="6" maxlength="500"
+          title="{% trans %}The top-left part on generated bills. Represent your company.{% endtrans %}"
+          placeholder="{% trans %}The top-left part on generated bills. Represent your company.{% endtrans %}"
+          >{{ request.form['source'] or g.user_pref.source or "" }}</textarea>
+
+        <label for="quote_mentions">{% trans %}Quote mentions{% endtrans %}</label>
+        <textarea name="quote_mentions" id="quote_mentions" rows="6" maxlength="500"
+          title="{% trans %}Bottom text on generated quotes.{% endtrans %}"
+          placeholder="{% trans %}Bottom text on generated quotes.{% endtrans %}"
+          >{{ request.form['quote_mentions'] or g.user_pref.quote_mentions or "" }}</textarea>
+
+        <label for="bill_mentions">{% trans %}Bill mentions{% endtrans %}</label>
+        <textarea name="bill_mentions" id="bill_mentions" rows="6" maxlength="500"
+          title="{% trans %}Bottom text on generated bills.{% endtrans %}"
+          placeholder="{% trans %}Bottom text on generated bills.{% endtrans %}"
+          >{{ request.form['bill_mentions'] or g.user_pref.bill_mentions or "" }}</textarea>
+      </div>
+
+      <div class="form">
+        <label for="smtp_host">{% trans %}SMTP host{% endtrans %}</label>
+        <input name="smtp_host" id="smtp_host" maxlength="30"
+          title="{% trans %}Ex: smtp.foo.bar{% endtrans %}"
+          placeholder="{% trans %}Ex: smtp.foo.bar{% endtrans %}"
+          value="{{ request.form['smtp_host'] or g.user_pref.smtp_host or "" }}">
+
+        <label for="smtp_port">{% trans %}SMTP port{% endtrans %}</label>
+        <input name="smtp_port" id="smtp_port" type="number"
+          title="{% trans %}Ex: 465{% endtrans %}"
+          placeholder="{% trans %}Ex: 465{% endtrans %}"
+          value="{{ request.form['smtp_port'] or g.user_pref.smtp_port or "" }}">
+
+        <label for="smtp_security">{% trans %}SMTP security{% endtrans %}</label>
+        <select name="smtp_security" id="smtp_security">
+          <option value="" {{ "selected" if not (request.form['smtp_security'] or g.user_pref.smtp_security) }}>{% trans %}Select an option{% endtrans %}</option>
+          {% for protocol in ["TLS", "STARTTLS"] %}
+            <option value="{{ protocol }}" {{ "selected" if (request.form['smtp_security'] or g.user_pref.smtp_security) == protocol }}>{{ protocol }}</option>
+          {% endfor %}
+        </select>
+
+        <label for="smtp_username">{% trans %}SMTP username{% endtrans %}</label>
+        <input name="smtp_username" id="smtp_username" maxlength="30"
+          title="{% trans %}Ex: <no-reply@john-doe.com>{% endtrans %}"
+          placeholder="{% trans %}Ex: <no-reply@john-doe.com>{% endtrans %}"
+          value="{{ request.form['smtp_username'] or g.user_pref.smtp_username or "" }}">
+
+        <label for="smtp_password">{% trans %}SMTP password{% endtrans %}</label>
+        <input name="smtp_password" id="smtp_password" type="password" maxlength="30"
+          value="{{ request.form['smtp_password'] or g.user_pref.smtp_password or "" }}">
+
+        <label for="smtp_reply_to">{% trans %}SMTP reply-to{% endtrans %}</label>
+        <input name="smtp_reply_to" id="smtp_reply_to" type="reply_to" maxlength="254"
+          title="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
+          placeholder="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
+          value="{{ request.form['smtp_reply_to'] or g.user_pref.smtp_reply_to or "" }}">
+
+        <label for="smtp_cc">{% trans %}SMTP cc{% endtrans %}</label>
+        <input name="smtp_cc" id="smtp_cc" type="reply_to" maxlength="508"
+          title="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
+          placeholder="{% trans %}Ex: John Doe <contact@john-doe.com> (Can stay empty){% endtrans %}"
+          value="{{ request.form['smtp_cc'] or g.user_pref.smtp_cc or "" }}">
 
+      </div>
+    </div>
     <input type="submit" value="{% trans %}Save{% endtrans %}">
+    {{ csrf_token()|safe }}
   </form>
 
   <hr>
 
   <div class="actions">
-      <form action="{{ url_for('user.test_email') }}" method="post">
+      <form action="{{ url_for('me.test_email') }}" method="post">
         <input type="submit" value="{% trans %}Test Email{% endtrans %}">
+        {{ csrf_token()|safe }}
       </form>
-      <form action="{{ url_for('user.delete') }}" method="post">
+      <form action="{{ url_for('me.delete') }}" method="post">
         <input class="danger" type="submit" value="{% trans %}Delete user{% endtrans %}" onclick="return confirm('{% trans %}You are about to delete all data associated to this account.\nAre you sure?{% endtrans %}');">
+        {{ csrf_token()|safe }}
       </form>
-      <form action="{{ url_for('user.delete_bills') }}" method="post">
+      <form action="{{ url_for('me.delete_bills') }}" method="post">
         <input class="danger" type="submit" value="{% trans %}Delete bills{% endtrans %}" onclick="return confirm('{% trans %}You are about to delete all of your bills.\nAre you sure?{% endtrans %}');">
+        {{ csrf_token()|safe }}
       </form>
-      <a href="{{ url_for('user.import_export_user') }}">{% trans %}Import / Export{% endtrans %}</a>
+      <a href="{{ url_for('me.import_export_user') }}">{% trans %}Import / Export{% endtrans %}</a>
   </div>
 {% endblock %}
```

## Comparing `fossbill-0.9.2.dist-info/LICENSE` & `fossbill-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fossbill-0.9.2.dist-info/RECORD` & `fossbill-1.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-fossbill/__init__.py,sha256=EXmOhpx8zhD-TNpYEjvcIlv0gnM_LN8EDzECnJp_B1c,1504
+fossbill/__init__.py,sha256=J6-SnwDPfxFd-jX5zY2wwx-51zrvPabsDCPsyoM4XT0,1584
 fossbill/alembic.ini,sha256=aJbEygfNAlh8HRJfjifPeR-AdKEs6RvAn3EcNAktnVM,3177
-fossbill/auth.py,sha256=b8Raao8ezXzKom_q3XGKUtzzpesItfDV0F33JOb_3oY,11111
-fossbill/bill.py,sha256=gueLeIACEkeseTtdgzZfgaO87opVkhbaSheeCtrhigA,28284
-fossbill/client.py,sha256=xAfL0gmZM_q2DrlEp990kXfvlGWN02l4y4k_C8hOBBU,5102
-fossbill/database.py,sha256=-XkMxecdBOmA74xyjipUGzvI6OgLmlvCnnffaazue08,9311
+fossbill/auth.py,sha256=o8aA2y1b69vsitt_TYpRwNs2BMIaENnB6KVftNuAiTE,11367
+fossbill/bill.py,sha256=0iYRiPceIdxKT8h0LsUA9GAJTtwPVk0F0jncMHbgs54,28130
+fossbill/customer.py,sha256=hneNpQRQK4XX2UbUU1CDyaJDGrHC-SYyVW3aXTP_U-g,5399
+fossbill/database.py,sha256=hB8CvYRhp-i47GJ4PcYCNgg3QVMvIvOx86DITno5QXs,9672
 fossbill/landing.py,sha256=iHmECuoW2lCIt19eaXL5w4c7649EGPMf6IqUGIxmhAE,344
-fossbill/payment.py,sha256=8q8lO5n1G1ORVhTUpAOXdPYErfDJugL12sy5Hh5C7eo,9272
-fossbill/product.py,sha256=uZZIIf10R3Mm3w4h1IKE7TOb-TJ1kb9ALIxvfDdxQdw,6679
-fossbill/user.py,sha256=SosLQq_PNmhtfl6U339hf-0BNPIHTYXbhgd1nukAX3s,12061
+fossbill/me.py,sha256=UQl55zOIVl4s8fo2N8Ex5NfgVtc6bk8p6Z3ae5sGH4w,12464
+fossbill/payment.py,sha256=tlhC0IXwCWxVjP_jgjAM8fpehqVsXDEntpWKkFlUEYA,10699
+fossbill/product.py,sha256=p8fPJIMZxozou7auJ1OUTaM6GWFku59Uh_yUE-BTDvQ,6880
+fossbill/user.py,sha256=Vi11FEIWrZqYYbu2BPQRA3EtrPwPrFiwch9gKCWUzB0,3160
 fossbill/alembic/env.py,sha256=AaC0ebQmXmRKI_UtQpDXsgiUTj9b64wyMcoQXBbzWjI,1836
 fossbill/alembic/script.py.mako,sha256=HNlf26BI1xvQKjiUojnj15BPrVUfVVr81IOgliJf83c,510
-fossbill/alembic/versions/fda694e67f67_init.py,sha256=BEab-P-9mpmVMprUknCJCxtfF_cXNtZzwFD1AX2N9ok,7758
-fossbill/locale/en_US/LC_MESSAGES/messages.mo,sha256=LR1qfi_01XmgOGNnMabT3uxhMRLZTtK3EJ6S4ibEqLQ,450
-fossbill/locale/fr_FR/LC_MESSAGES/messages.mo,sha256=OjdwsO9OhNSs6K8w097xD4BGVPgwknnKFZN_9QqUZ68,16388
-fossbill/static/bill.css,sha256=dK8ysx0ar-_0eMarSmn2oi1z5sBGH6KnCIrGGdzzRBI,259
-fossbill/static/style.css,sha256=qSkIzZuMETniGCFdn1b87_D_nH04om_DyAPJsgmQ08A,2164
-fossbill/templates/base.html,sha256=EkivYw8dqUQ-CCDFfApxyx3XkiUx_4jfLYi3vCAjrJ8,1331
+fossbill/alembic/versions/21487ff4ab8c_store_receipt_url_in_payment.py,sha256=HdCOsCFGfLAG6UcwySX2vVxGVZihF5At3FfiCXDa9l4,704
+fossbill/alembic/versions/7899e98936b3_bills_date_to_created_at.py,sha256=orkiLS6CoW4Tl2XoD5-o4J2zp-87dkzZJVq-gEfbnFk,492
+fossbill/alembic/versions/ac14f3a73a29_rename_client_to_customer.py,sha256=ZYYNxX74v8KPSYfjy27dBY1An7GSBgCCWPJlJamSE1o,1355
+fossbill/alembic/versions/fda694e67f67_init.py,sha256=aJdRCEUND0KGp4iBtOGX0_0oAifgdgSHyJ5O4asip_4,7770
+fossbill/alembic/versions/ff51555aa2ba_add_date_on_bills_and_quotes.py,sha256=7Kzt1RN7-9RDZcCjrR2mGHaX-Ya7oQuaeqPmh43QBks,800
+fossbill/locale/en_US/LC_MESSAGES/messages.mo,sha256=FdleA1M_5166vTrvPucTx0Ew_KZSFGTfaFppX8zX4Nw,451
+fossbill/locale/fr_FR/LC_MESSAGES/messages.mo,sha256=ebXLuCWs7ydr8MEjHajrVHJntPvp-4bjR6UbGX0uXG0,17250
+fossbill/static/bill.css,sha256=RK6RFKfr09lF6rmNBm58VijrzZfn4FbRmyFOnV6YtYc,454
+fossbill/static/style.css,sha256=njt0HTmNoI_LbwB9BkAMc-riMQSdmV4nPoHCs6CutQ8,2711
+fossbill/templates/base.html,sha256=Br_cdncS21bisLQVJAQHFxOaA1sQIkKrkKieKrXR8Fg,1744
 fossbill/templates/macros.html,sha256=cVbZO23WeyTx4RdvJZUSXRIzfk4bKIdF_UY5g4Xh-JU,1588
-fossbill/templates/auth/ask_reset_password.html,sha256=y3r-FYTYwF6_gl3qW4ZUCiW5jlSPDgI09s8NnO39fl8,395
-fossbill/templates/auth/login.html,sha256=60hhXzkVvVd7ng7QCPWAjlDYHh9oMuvRiWKcMyCdZtU,670
-fossbill/templates/auth/register.html,sha256=X2_l4Fs8KTWIEVhrAhi9R7pJGBmj1dpwZL49dZ9Dlm0,538
+fossbill/templates/auth/ask_reset_password.html,sha256=OgXkipciXCz_JjjD-tOj5xqfPOoEL1GByUnImPch1fw,423
+fossbill/templates/auth/login.html,sha256=Qge-oGgFfqOTRmG3XazwZLC9Nm7gip7L-UlqZ46vt4M,698
+fossbill/templates/auth/register.html,sha256=NqajXuHBpBTH9CntB6S2KIt_tt_w-t-qu1JV2o30Hbs,566
 fossbill/templates/auth/reset_password_email.plain,sha256=Ojxh1LbmQroZTKAJwrusDvbcyb9rP35KnPTq1YbO-C8,152
-fossbill/templates/auth/use_reset_password.html,sha256=42wBB9yD_OWdADHdp3opjDsMwr2yHDKwT2uvcStRkZQ,518
+fossbill/templates/auth/use_reset_password.html,sha256=jcVM4gSJCsawNtXZIOt1AVRoIVTlltdm0VBqjFfdKfM,546
 fossbill/templates/bill/bill_email.plain,sha256=ZqWZvEwSppsftsvua_CiZ27zQcsHjixEnpbxEWUWcp4,107
-fossbill/templates/bill/create.html,sha256=I1J1M21xy8pjXOArQtvTDidytUjdcKSM3-VS0cO_RZA,598
-fossbill/templates/bill/generated_bill.html,sha256=1M1B0fhO8SPVuwYrHCMAGWlKg4RZ7rOUgJzs1wkuoTo,1247
-fossbill/templates/bill/generated_quote.html,sha256=t6ZQHaG6FHrqNtDQ-eWA6oUsyNUIknGR8LETDThMs7I,2384
-fossbill/templates/bill/index.html,sha256=n8xDpYefD5Zb_PNQyT_dcsCwLKtlHnk25kR6rF7wRrs,5373
+fossbill/templates/bill/create.html,sha256=mm7quPoARbGkdfK2K4yfUjXPpj-fOBJbc0V0jNMPh-I,642
+fossbill/templates/bill/create_row.html,sha256=yzNu07toNXSVbT1MOMRHI6XVFwQoYW01HHY4qVJTgyw,2532
+fossbill/templates/bill/finish.html,sha256=MyE-dQ-2dzid9pGymaO65gq1epvU4qZXu537iRvDe30,1559
+fossbill/templates/bill/generated_bill.html,sha256=kcoc77VSqohnAJJTubmZCdX_ERe1ulaie3FOc14nbxA,933
+fossbill/templates/bill/generated_draft.html,sha256=JKaAHaUSCoS750cyWvQmXIiJBxNpwAi-TWdyJEPLzmI,2494
+fossbill/templates/bill/generated_quote.html,sha256=DJg0fmZprKLvco1cZwXFp1JAf0MoxgaJd-R1xPJ60c8,479
+fossbill/templates/bill/index.html,sha256=ohpLxmDCeRoqTHI7Tx5Vm0vR5BxL_F5sNshnHQp_arE,6094
 fossbill/templates/bill/quote_email.plain,sha256=F7LyDUhhVDvYqZyy_sCrZggQ_fVs1tgfVazdj7IHE0k,108
-fossbill/templates/bill/send_bill_email.html,sha256=iaqQ2SASC4hltdsAfIfvHj3WPUKoLpOP_YIJCVt6RAc,732
-fossbill/templates/bill/send_quote_email.html,sha256=azonhuiTBoQ3IlQRzEAKgSGtEQB2MglDfjrip1HHTnU,733
-fossbill/templates/bill/update.html,sha256=ShDUvZuideTok_i54aZd2uGSa6KQqto5WlSaPxdmAuM,7949
-fossbill/templates/bill/update_bill.html,sha256=d3eDl5I9bjGMhdsRO4zYVadKRAmWXNNZJHoI2MmWBIU,1039
-fossbill/templates/bill/update_quote.html,sha256=uRqNf1isCjoy4y8JhPEoMyNqpgEubAjnUR51CFuAsD4,3428
-fossbill/templates/client/create.html,sha256=OJBZ1S5tDvljj8QXm37Spbf8FBiUnGYgSjmVKpq5jPY,1193
-fossbill/templates/client/index.html,sha256=Cxp8KaEhF4ToXDnbLyMx368R5G_oYjWdX7S3iBQ95wE,1981
-fossbill/templates/client/update.html,sha256=o2hJk_8PHjRu79ZgIJMQVegateaGW7gV5KGye7mQC38,1553
-fossbill/templates/landing/dashboard.html,sha256=sBWllBzLXSzGLlZH4B4d0XC5nG0fA2_y7SBFgZA-qj4,836
+fossbill/templates/bill/send_bill_email.html,sha256=PyHZ8siNN4Yb-lYOCHOR2HqG8GExMrxL4CpXdeyENoo,762
+fossbill/templates/bill/send_quote_email.html,sha256=k6lO2r_3pXnBpDydZzCGh51XiR-huu69F6EG2h-ZY-Q,763
+fossbill/templates/bill/update.html,sha256=ctH9mEYKEqtVmANem5QcPPNMF-gnDfo94M1wzoYce1E,4494
+fossbill/templates/bill/update_bill.html,sha256=r1uyp8BxKInIW9YXk0aU1SOu-ReTk53Yz11Og-uyNZY,1612
+fossbill/templates/bill/update_quote.html,sha256=wMGA4fVw4_EBQwOPW1X1BxSSwVdqUUsPJ4dPx1XPMPk,3022
+fossbill/templates/bill/update_row.html,sha256=dYl9b6qZ68ogMqD6GLKXXJWWvWI08kpa76uoZnUf-B0,1147
+fossbill/templates/customer/create.html,sha256=j7k9cCPCGFcLkHrSe3GPoajwqFzFYnYpjWcVUnvAnuQ,1551
+fossbill/templates/customer/index.html,sha256=m_qhOA6pDiJMb4HKNUKDTXOLj4l5CCsymX-ws5jIQRo,2078
+fossbill/templates/customer/update.html,sha256=xlGQ8L23lDFm8RSshRn9qJ4LbQgeLT_m7REdoHYAN8w,1625
+fossbill/templates/landing/dashboard.html,sha256=7Hb2pCs1FyHu3R8LMfAp1dch7JSbact-cBJ7OvxIUAU,840
 fossbill/templates/landing/welcome.html,sha256=9nJ4XTN-xd-7I61keypXY6oTvjTQoAC0QMC2uOVvLNA,1194
-fossbill/templates/payment/home.html,sha256=j8etoFRc0Aaw7W22n1XRw2DNunM-Z4mvUy0D8v9xCAo,3308
+fossbill/templates/me/import_export_user.html,sha256=kQyFcHyeM6zBEMklhtpmcX9xgFyb-S_VhFLIsvb-3Ag,639
+fossbill/templates/me/test_email.plain,sha256=rxG8bZuAedYS0U83l31S93XeT5YpS6wB5h46ChsU_w0,91
+fossbill/templates/me/update.html,sha256=dr8DlHG7q3xjA_voC1A6ks0ldK1K4V2PxIFYo0ZAYKA,6537
+fossbill/templates/payment/charged_notice.plain,sha256=PfaOxkor6PniuCFGD0j-OUmt2Cc4OylF3kTaUgFqtMg,153
+fossbill/templates/payment/index.html,sha256=WyJLZsvtYByaC9Hdwr3COtdm8D8rCJnST3p597kkJZo,3474
 fossbill/templates/payment/invoice.html,sha256=x_SnaWn7dqUD3E4mq3UzdoeV63uNZlEL8TOz3imGCmc,1381
-fossbill/templates/product/create.html,sha256=Eo_B8mPQgwYYSjdir68i5fgCe_BVHTyvVRjH0nwJDAE,1155
-fossbill/templates/product/index.html,sha256=ynFcx3-SX6VvuAYhHDoCanh-ML6mKBJZwxayJc4MkrY,2566
-fossbill/templates/product/update.html,sha256=KOTZTRRRwH2nblryY0wC0IvuRq9JIXvDaFbhf0ldAsU,1492
-fossbill/templates/user/import_export_user.html,sha256=FVwasyYt30FppOPCZGhJqyWOAJuoEsKS0G5slrI9YF8,630
-fossbill/templates/user/test_email.plain,sha256=rxG8bZuAedYS0U83l31S93XeT5YpS6wB5h46ChsU_w0,91
-fossbill/templates/user/update.html,sha256=Ho7z2qFL_aFxuPXLog8rLhgRZ8cDlQ6cfTQ-vRSKMD0,6041
-fossbill-0.9.2.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
-fossbill-0.9.2.dist-info/METADATA,sha256=JB0NlDT1TysXFyAfv1svpUbxf4qqwCdeQXOa0__lOhE,232
-fossbill-0.9.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fossbill-0.9.2.dist-info/top_level.txt,sha256=_3zpUgFKDVFDozmRBG8VdiIcs6h94lXOUIAg4g1Gur4,9
-fossbill-0.9.2.dist-info/RECORD,,
+fossbill/templates/product/create.html,sha256=Fa_7w6T_kFol9-HBv_JEBpeDCCE0TdVXAUjMJbHX_-o,1486
+fossbill/templates/product/index.html,sha256=lEboPcPsm3_k_sk0pVI07UYGPUtHa0LOVwugv0sMGak,2913
+fossbill/templates/product/update.html,sha256=Cx4EQMiWOKKpL1pljle568iPdXdUF3VOfzyXfTpj3H4,1548
+fossbill/templates/user/index.html,sha256=Q5vEfYR3WDc_F1r_vCCAfKRxfe3hIc-9l7du2uRdlJQ,3458
+fossbill-1.0.0.dist-info/LICENSE,sha256=DZak_2itbUtvHzD3E7GNUYSRK6jdOJ-GqncQ2weavLA,34523
+fossbill-1.0.0.dist-info/METADATA,sha256=Nlha7GbkMCnjS4r33z7YqFv_Hw4fbQ9sqHXozyHIaDs,232
+fossbill-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fossbill-1.0.0.dist-info/top_level.txt,sha256=_3zpUgFKDVFDozmRBG8VdiIcs6h94lXOUIAg4g1Gur4,9
+fossbill-1.0.0.dist-info/RECORD,,
```

