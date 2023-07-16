# Comparing `tmp/1secMail-1.0.0.tar.gz` & `tmp/1secMail-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1secMail-1.0.0.tar", last modified: Fri Jul 14 15:17:55 2023, max compression
+gzip compressed data, was "1secMail-1.1.0.tar", last modified: Sun Jul 16 04:07:25 2023, max compression
```

## Comparing `1secMail-1.0.0.tar` & `1secMail-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.564603 1secMail-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.558721 1secMail-1.0.0/1secMail.egg-info/
--rw-rw-rw-   0        0        0     4060 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2023-07-13 09:01:53.000000 1secMail-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4060 2023-07-14 15:17:55.563241 1secMail-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3197 2023-07-14 03:57:35.000000 1secMail-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.563241 1secMail-1.0.0/secmail/
--rw-rw-rw-   0        0        0      123 2023-07-13 15:44:12.000000 1secMail-1.0.0/secmail/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-07-14 15:17:50.000000 1secMail-1.0.0/secmail/client.py
--rw-rw-rw-   0        0        0      443 2023-07-14 15:09:27.000000 1secMail-1.0.0/secmail/config.py
--rw-rw-rw-   0        0        0     3384 2023-07-14 03:38:35.000000 1secMail-1.0.0/secmail/models.py
--rw-rw-rw-   0        0        0       42 2023-07-14 15:17:55.564603 1secMail-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1473 2023-07-14 15:17:52.000000 1secMail-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:07:25.713727 1secMail-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 04:07:25.706730 1secMail-1.1.0/1secMail.egg-info/
+-rw-rw-rw-   0        0        0     7071 2023-07-16 04:07:25.000000 1secMail-1.1.0/1secMail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-16 04:07:25.000000 1secMail-1.1.0/1secMail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 04:07:25.000000 1secMail-1.1.0/1secMail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-16 04:07:25.000000 1secMail-1.1.0/1secMail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 04:07:25.000000 1secMail-1.1.0/1secMail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2023-07-13 09:01:53.000000 1secMail-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7071 2023-07-16 04:07:25.712726 1secMail-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6156 2023-07-16 03:40:40.000000 1secMail-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 04:07:25.711726 1secMail-1.1.0/secmail/
+-rw-rw-rw-   0        0        0      123 2023-07-13 15:44:12.000000 1secMail-1.1.0/secmail/__init__.py
+-rw-rw-rw-   0        0        0    25520 2023-07-16 03:53:29.000000 1secMail-1.1.0/secmail/client.py
+-rw-rw-rw-   0        0        0      443 2023-07-16 04:04:10.000000 1secMail-1.1.0/secmail/config.py
+-rw-rw-rw-   0        0        0     3387 2023-07-16 02:44:46.000000 1secMail-1.1.0/secmail/models.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 04:07:25.713727 1secMail-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1541 2023-07-16 04:06:59.000000 1secMail-1.1.0/setup.py
```

### Comparing `1secMail-1.0.0/1secMail.egg-info/PKG-INFO` & `1secMail-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: 1secMail
-Version: 1.0.0
-Summary: Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python.
-Home-page: https://github.com/qvco/1secMail-Python
-Download-URL: https://github.com/qvco/1secMail-Python
-Author: qvco
-Author-email: nikola.desuga@gmail.com
-Maintainer: qvco
-Maintainer-email: nikola.desuga@gmail.com
-License: MIT
-Keywords: 1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <br>
   <img src="https://github.com/qvco/1secMail-Python/assets/77382767/fde69c1a-b95f-4d78-af1a-2dca315204bc" alt="1secMail" width="700">
 <!--   <br>
   1secMail for Python
   <br> -->
 </p>
@@ -33,15 +12,16 @@
     <img src="https://img.shields.io/github/release/qvco/1secMail-Python">
     <img src="https://img.shields.io/badge/python-3.8-blue.svg">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg">
   </p>
 
 ### About
 
-This is an easy to use yet full-featured Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily create temporary email addresses for testing, verification, or other purposes where you need a disposable email address.
+This is an easy to use yet full-featured Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily create temporary email addresses for testing, verification, or other purposes where you need a disposable email address.  
+> Asynchronous operations are also supported!:thumbsup:
 
 ### Install
 
 To install the package, you'll need Python 3.8 or above installed on your computer. From your command line:
 
 ```bash
 pip install 1secMail
@@ -88,22 +68,22 @@
 ```
 
 ### Receiving Messages
 
 To wait until a new message is received, use the `await_new_message()` method:
 
 ```python
-message = client.await_new_message(address)
+message = client.await_new_message("bobby-bob@kzccv.com")
 ```
 
 To check all messages received on a particular email address, use the `get_inbox()` method and pass the email address:
 
 ```python
-messages = client.get_inbox("bobby-bob@kzccv.com")
-for message in messages:
+inbox = client.get_inbox("bobby-bob@kzccv.com")
+for message in inbox:
     print(message.id)
     print(message.from_address)
     print(message.subject)
     print(message.date)
 ```
 
 You can also fetch a single message using the `get_message()` method and passing the email address and message ID:
@@ -115,21 +95,130 @@
 print(message.body)
 print(message.text_body)
 print(message.html_body)
 print(message.attachments)
 print(message.date)
 ```
 
-### Attachment Information
+### Downloading an attachment
+
+You can download an attachment from a message in the inbox of a specified email address using the download_attachment method like this:
+
+```python
+client.download_attachment(address, message_id, attachment_filename)
+>>> 'Path: (C:\Users\user\path/config/rocket.png), Size: 49071B'
+```
+
+## Asynchronous Client
+
+### Generating Email Addresses
 
-To check attachment information, loop through the attachments in the message object and print the filename, content type, and size:
+To generate a list of random email addresses, use the `random_email()` method:
 
 ```python
-for attachment in message.attachments:
-    print(attachment.filename)
-    print(attachment.content_type)
-    print(attachment.size)
+import asyncio
+import secmail
+
+async def main():
+    client = secmail.AsyncClient()
+    email_addresses = await client.random_email(amount=3)
+    print(email_addresses)
+
+asyncio.run(main())
+>>> ['c3fho3cry1@1secmail.net', '5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net']
+```
+
+You can also generate a custom email address by specifying the username and domain:
+
+> **Note**
+> Specifying a domain is optional!
+
+```python
+await client.custom_email(username="bobby-bob", domain="kzccv.com")
+>>> 'bobby-bob@kzccv.com'
+```
+
+### Receiving Messages
+
+To wait until a new message is received, use the `await_new_message()` method:
+
+```python
+import asyncio
+import secmail
+
+async def main():
+    client = secmail.AsyncClient()
+    message = await client.await_new_message("bobby-bob@kzccv.com")
+    print(f"{message.from_address}: {message.subject}")
+
+asyncio.run(main())
+```
+
+To check all messages received on a particular email address, use the `get_inbox()` method and pass the email address:
+
+```python
+import asyncio
+import secmail
+
+async def main():
+    client = secmail.AsyncClient()
+    inbox = await client.get_inbox("bobby-bob@kzccv.com")
+    print(f"You have {len(inbox)} messages in your inbox.")
+
+    for message in inbox:
+        print(message.id)
+        print(message.from_address)
+        print(message.subject)
+        print(message.date)
+
+asyncio.run(main())
+```
+
+You can also fetch a single message using the `get_message()` method and passing the email address and message ID:
+
+```python
+import asyncio
+import secmail
+
+async def main():
+    client = secmail.AsyncClient()
+    address = "bobby-bob@kzccv.com"
+    inbox = await client.get_inbox(address)
+    message_id = inbox[0].id
+    message = await client.get_message(address, message_id)
+
+    print(message.id)
+    print(message.subject)
+    print(message.body)
+    print(message.text_body)
+    print(message.html_body)
+    print(message.attachments)
+    print(message.date)
+
+asyncio.run(main())
+```
+
+### Downloading an attachment
+
+You can download an attachment from a message in the inbox of a specified email address using the download_attachment method like this:
+
+```python
+import asyncio
+import secmail
+
+async def main():
+    client = secmail.AsyncClient()
+    address = "bobby-bob@kzccv.com"
+    inbox = await client.get_inbox(address)
+    message_id = inbox[0].id
+    message = await client.get_message(address, message_id)
+    attachment_filename = message.attachments[0].filename
+    await client.download_attachment(address, message_id, attachment_filename)
+
+asyncio.run(main())
+
+>>> 'Path: (C:\Users\user\path/config/rocket.png), Size: 49071B'
 ```
 
 ## Licnese
 
 This software is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) © [Qvco](https://github.com/qvco).
```

#### html2text {}

```diff
@@ -1,51 +1,75 @@
-Metadata-Version: 2.1 Name: 1secMail Version: 1.0.0 Summary: Create and receive
-email in only 1 second! ð§ An API wrapper for www.1secmail.com written in
-Python. Home-page: https://github.com/qvco/1secMail-Python Download-URL: https:
-//github.com/qvco/1secMail-Python Author: qvco Author-email:
-nikola.desuga@gmail.com Maintainer: qvco Maintainer-email:
-nikola.desuga@gmail.com License: MIT Keywords:
-1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown License-File: LICENSE
 
                                   [1secMail]
         *** An API wrapper for www.1secmail.com written in Python. ***
     [https://img.shields.io/github/release/qvco/1secMail-Python] [https://
    img.shields.io/badge/python-3.8-blue.svg] [https://img.shields.io/badge/
                              License-MIT-blue.svg]
 ### About This is an easy to use yet full-featured Python API wrapper for
 www.1secmail.com â using the official 1secMail API. It allows you to easily
 create temporary email addresses for testing, verification, or other purposes
-where you need a disposable email address. ### Install To install the package,
-you'll need Python 3.8 or above installed on your computer. From your command
-line: ```bash pip install 1secMail ```
+where you need a disposable email address. > Asynchronous operations are also
+supported!:thumbsup: ### Install To install the package, you'll need Python 3.8
+or above installed on your computer. From your command line: ```bash pip
+install 1secMail ```
 > **Note** > If you're willing to install the development version, do the
 following: ```bash git clone https://github.com/qvco/1secMail-Python.git cd
 1secMail-Python pip install -r requirements.txt pip install -e . ``` ## Usage
 ### Generating Email Addresses To generate a list of random email addresses,
 use the `random_email()` method: ```python import secmail client =
 secmail.Client() client.random_email(amount=3) >>> ['c3fho3cry1@1secmail.net',
 '5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net'] ``` You can also generate
 a custom email address by specifying the username and domain: > **Note** >
 Specifying a domain is optional! ```python client.custom_email(username="bobby-
 bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' ``` ### Receiving Messages
 To wait until a new message is received, use the `await_new_message()` method:
-```python message = client.await_new_message(address) ``` To check all messages
-received on a particular email address, use the `get_inbox()` method and pass
-the email address: ```python messages = client.get_inbox("bobby-bob@kzccv.com")
-for message in messages: print(message.id) print(message.from_address) print
-(message.subject) print(message.date) ``` You can also fetch a single message
-using the `get_message()` method and passing the email address and message ID:
-```python message = client.get_message(address="bobby-bob@kzccv.com",
-message_id=235200687) print(message.id) print(message.subject) print
-(message.body) print(message.text_body) print(message.html_body) print
-(message.attachments) print(message.date) ``` ### Attachment Information To
-check attachment information, loop through the attachments in the message
-object and print the filename, content type, and size: ```python for attachment
-in message.attachments: print(attachment.filename) print
-(attachment.content_type) print(attachment.size) ``` ## Licnese This software
+```python message = client.await_new_message("bobby-bob@kzccv.com") ``` To
+check all messages received on a particular email address, use the `get_inbox
+()` method and pass the email address: ```python inbox = client.get_inbox
+("bobby-bob@kzccv.com") for message in inbox: print(message.id) print
+(message.from_address) print(message.subject) print(message.date) ``` You can
+also fetch a single message using the `get_message()` method and passing the
+email address and message ID: ```python message = client.get_message
+(address="bobby-bob@kzccv.com", message_id=235200687) print(message.id) print
+(message.subject) print(message.body) print(message.text_body) print
+(message.html_body) print(message.attachments) print(message.date) ``` ###
+Downloading an attachment You can download an attachment from a message in the
+inbox of a specified email address using the download_attachment method like
+this: ```python client.download_attachment(address, message_id,
+attachment_filename) >>> 'Path: (C:\Users\user\path/config/rocket.png), Size:
+49071B' ``` ## Asynchronous Client ### Generating Email Addresses To generate a
+list of random email addresses, use the `random_email()` method: ```python
+import asyncio import secmail async def main(): client = secmail.AsyncClient()
+email_addresses = await client.random_email(amount=3) print(email_addresses)
+asyncio.run(main()) >>> ['c3fho3cry1@1secmail.net', '5qcd3d36zr@1secmail.org',
+'b6fgeothtg@1secmail.net'] ``` You can also generate a custom email address by
+specifying the username and domain: > **Note** > Specifying a domain is
+optional! ```python await client.custom_email(username="bobby-bob",
+domain="kzccv.com") >>> 'bobby-bob@kzccv.com' ``` ### Receiving Messages To
+wait until a new message is received, use the `await_new_message()` method:
+```python import asyncio import secmail async def main(): client =
+secmail.AsyncClient() message = await client.await_new_message("bobby-
+bob@kzccv.com") print(f"{message.from_address}: {message.subject}") asyncio.run
+(main()) ``` To check all messages received on a particular email address, use
+the `get_inbox()` method and pass the email address: ```python import asyncio
+import secmail async def main(): client = secmail.AsyncClient() inbox = await
+client.get_inbox("bobby-bob@kzccv.com") print(f"You have {len(inbox)} messages
+in your inbox.") for message in inbox: print(message.id) print
+(message.from_address) print(message.subject) print(message.date) asyncio.run
+(main()) ``` You can also fetch a single message using the `get_message()`
+method and passing the email address and message ID: ```python import asyncio
+import secmail async def main(): client = secmail.AsyncClient() address =
+"bobby-bob@kzccv.com" inbox = await client.get_inbox(address) message_id =
+inbox[0].id message = await client.get_message(address, message_id) print
+(message.id) print(message.subject) print(message.body) print
+(message.text_body) print(message.html_body) print(message.attachments) print
+(message.date) asyncio.run(main()) ``` ### Downloading an attachment You can
+download an attachment from a message in the inbox of a specified email address
+using the download_attachment method like this: ```python import asyncio import
+secmail async def main(): client = secmail.AsyncClient() address = "bobby-
+bob@kzccv.com" inbox = await client.get_inbox(address) message_id = inbox[0].id
+message = await client.get_message(address, message_id) attachment_filename =
+message.attachments[0].filename await client.download_attachment(address,
+message_id, attachment_filename) asyncio.run(main()) >>> 'Path: (C:
+\Users\user\path/config/rocket.png), Size: 49071B' ``` ## Licnese This software
 is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/
 master/LICENSE) Â© [Qvco](https://github.com/qvco).
```

### Comparing `1secMail-1.0.0/LICENSE` & `1secMail-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `1secMail-1.0.0/secmail/client.py` & `1secMail-1.1.0/secmail/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import os
-import time
+import re
+import asyncio
 import random
 import string
 import httpx
+import time
 import json
 
-from typing import List, Tuple
+from typing import List
 from json import JSONDecodeError
 
 from .config import (
     DOMAIN_LIST,
     GET_DOMAIN_LIST,
     GET_MESSAGES,
     GET_SINGLE_MESSAGE,
     DOWNLOAD,
 )
 from .models import Inbox, Message
 
 
+# errors
+
+
 class SecMailError(Exception):
     """Base exception for 1secMail"""
 
     pass
 
 
 class BadRequestError(SecMailError):
@@ -74,66 +79,80 @@
 
     Exception raised for a 5xx HTTP status code
     """
 
     pass
 
 
+# utils
+
+
+def is_valid_username(username: str) -> bool:
+    if username is None or len(username) > 64:
+        return False
+    return bool(
+        re.match(r"^[A-Za-z][A-Za-z0-9._-]*[A-Za-z0-9]$", username)
+        and not re.search(r"\.\.|\-\-|\_\_|\.$", username)
+    )
+
+
 current_path = os.path.abspath(os.getcwd())
 
 
+# client
+
+
 class Client:
     """An API wrapper for www.1secmail.com written in Python.
 
     >>> import secmail
     >>> client = secmail.Client()
 
     """
 
     def __init__(
         self, base_path=current_path + "/config/", host="www.1secmail.com"
     ) -> None:
         self.base_path = base_path
-        self.host = "https://" + host + "/api/v1/"
+        self.api_url = "https://" + host + "/api/v1/"
         self.client = httpx.Client()
 
-    def _request(self, method, url, params=None, json=None, data_type=None):
-        r = self.client.request(method=method, url=url, params=params, json=json)
+    def _request(self, action: str, params=None, data_type=None):
+        r = self.client.request(method="GET", url=self.api_url + action, params=params)
 
         if r.status_code == 400:
             raise BadRequestError(f"HTTP {r.status_code}: {r.text}")
         if r.status_code == 401:
             raise AuthenticationError(f"HTTP {r.status_code}: {r.text}")
         if r.status_code == 403:
             raise ForbiddenError(f"HTTP {r.status_code}: {r.text}")
         if r.status_code == 404:
             raise NotFoundError(f"HTTP {r.status_code}: {r.text}")
         if r.status_code == 429:
             raise RateLimitError(f"HTTP {r.status_code}: {r.text}")
         if r.status_code == 500:
             raise ServerError(f"HTTP {r.status_code}: {r.text}")
 
+        if action == DOWNLOAD:
+            return r.content
+
         try:
             r = r.json()
         except JSONDecodeError:
             return r.text
 
         if data_type is not None:
             if isinstance(r, list):
                 r = [data_type(result) for result in r]
             elif r is not None:
                 r = data_type(r)
 
         return r
 
     @staticmethod
-    def _split_email(address: str) -> Tuple[str, str]:
-        return address.split("@")
-
-    @staticmethod
     def random_email(amount: int, domain: str = None) -> List[str]:
         """This method generates a list of random email addresses.
 
         Parameters:
         ----------
 
             - `amount`: `int` - The number of email addresses to generate.
@@ -163,21 +182,20 @@
         if domain is not None and domain not in DOMAIN_LIST:
             err_msg = (
                 f"{domain} is not a valid domain name.\nValid Domains: {DOMAIN_LIST}"
             )
             raise ValueError(err_msg)
 
         emails = []
-        for i in range(amount):
-            name = string.ascii_lowercase + string.digits
-            username = "".join(random.choice(name) for i in range(12))
-            if domain is not None:
-                emails.append(username + "@" + domain)
-            else:
-                emails.append(username + "@" + random.choice(DOMAIN_LIST))
+        for _ in range(amount):
+            username = "".join(
+                random.choices(string.ascii_lowercase + string.digits, k=12)
+            )
+            email = f"{username}@{domain or random.choice(DOMAIN_LIST)}"
+            emails.append(email)
 
         return emails
 
     @staticmethod
     def custom_email(username: str, domain: str = None) -> str:
         """This method generates a custom email address.
 
@@ -212,20 +230,19 @@
         """
         if domain is not None and domain not in DOMAIN_LIST:
             err_msg = (
                 f"{domain} is not a valid domain name.\nValid Domains: {DOMAIN_LIST}"
             )
             raise ValueError(err_msg)
 
-        if domain is not None:
-            email = username + "@" + domain
-        else:
-            email = username + "@" + random.choice(DOMAIN_LIST)
+        if is_valid_username(username) is False:
+            err_msg = f"'{username}' is not a valid username."
+            raise ValueError(err_msg)
 
-        return email
+        return f"{username}@{domain or random.choice(DOMAIN_LIST)}"
 
     def await_new_message(self, address: str, fetch_interval=5) -> Inbox:
         """This method waits until a new message is received for the specified email address.
 
         Parameters:
         ----------
         - `address`: `str` - The email address to check for new messages.
@@ -268,15 +285,15 @@
         >>> domains = client.get_active_domains()
 
         The method sends a GET request to the API endpoint to retrieve a list of currently active domains. The list is returned as a list of strings.
 
         Note that the list of active domains may change over time.
 
         """
-        return self._request(method="GET", url=self.host + GET_DOMAIN_LIST)
+        return self._request(action=GET_DOMAIN_LIST)
 
     def get_inbox(self, address: str) -> List[Inbox]:
         """This method retrieves all the messages in the mailbox for the specified email address.
 
         Parameters:
         ----------
         - `address`: `str` - The email address to check for messages.
@@ -290,18 +307,17 @@
         Get all the messages in the mailbox for the email address "johndoe@1secmail.com":
 
         >>> messages = client.get_inbox("johndoe@1secmail.com")
 
         The method sends a GET request to the API endpoint to retrieve all the messages in the mailbox for the specified email address. The messages are returned as a list of inbox objects. If there are no messages in the mailbox, an empty list is returned.
 
         """
-        username, domain = self._split_email(address)
+        username, domain = address.split("@")
         return self._request(
-            method="GET",
-            url=self.host + GET_MESSAGES,
+            action=GET_MESSAGES,
             params={"login": username, "domain": domain},
             data_type=Inbox,
         )
 
     def get_message(self, address: str, message_id: int) -> Message:
         """This method retrieves a detailed message from the mailbox for the specified email address and message ID.
 
@@ -319,18 +335,17 @@
         Get the message with ID 12345 in the mailbox for the email address "johndoe@1secmail.com":
 
         >>> message = client.get_message("johndoe@1secmail.com", 12345)
 
         The method sends a GET request to the API endpoint to retrieve the message with the specified ID in the mailbox for the specified email address. The message is returned as a message object.
 
         """
-        username, domain = self._split_email(address)
+        username, domain = address.split("@")
         return self._request(
-            method="GET",
-            url=self.host + GET_SINGLE_MESSAGE,
+            action=GET_SINGLE_MESSAGE,
             params={"login": username, "domain": domain, "id": message_id},
             data_type=Message,
         )
 
     def save_email(self, address: str) -> None:
         """This method saves the specified email address to a JSON file for future use.
 
@@ -357,20 +372,377 @@
                 data = json.load(f)
 
         data.setdefault("email", []).append(address)
 
         with open(self.base_path + "secmail.json", "w") as f:
             json.dump(data, f, indent=4)
 
-    def download_attachment(self, address: str, message_id: int, filename: str):
-        """Download attachment from message."""
-        username, domain = self._split_email(address)
-        return self._request(
-            method="GET",
-            url=self.host + DOWNLOAD,
+    def download_attachment(
+        self,
+        address: str,
+        message_id: int,
+        filename: str,
+        save_path: str = current_path + "/config/",
+    ):
+        """This method downloads an attachment from a message in the mailbox for the specified email address and message ID.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to check for the message containing the attachment.
+        - `message_id`: `int` - The ID of the message containing the attachment to download.
+        - `filename`: `str` - The name of the attachment file to download.
+        - `save_path`: `str` - Optional. The path to save the downloaded attachment. Default is the current path + "/config/".
+
+        Returns:
+        -------
+        - `str` - A string indicating the path and size of the downloaded attachment.
+
+        Example:
+        -------
+        Download the attachment named "report.pdf" from the message with ID 12345 in the mailbox for the email address "johndoe@1secmail.com":
+
+        >>> download_attachment("johndoe@1secmail.com", 12345, "report.pdf")
+
+        """
+        username, domain = address.split("@")
+        attachment = self._request(
+            action=DOWNLOAD,
             params={
                 "login": username,
                 "domain": domain,
                 "id": message_id,
                 "file": filename,
             },
         )
+
+        if not os.path.exists(self.base_path):
+            os.mkdir(self.base_path)
+
+        with open(save_path + filename, "wb") as attachment_file:
+            size = attachment_file.write(attachment)
+        return "Path: (" + save_path + filename + "), Size: " + str(size) + "B"
+
+
+# async client
+
+
+class AsyncClient:
+    """An API wrapper for www.1secmail.com written in Python.
+
+    >>> import secmail
+    >>> client = secmail.AsyncClient()
+
+    """
+
+    def __init__(
+        self, base_path=current_path + "/config/", host="www.1secmail.com"
+    ) -> None:
+        self.base_path = base_path
+        self.api_url = "https://" + host + "/api/v1/"
+        self.client = httpx.AsyncClient()
+
+    async def _request(self, action: str, params=None, data_type=None):
+        r = await self.client.request(
+            method="GET", url=self.api_url + action, params=params
+        )
+
+        if r.status_code == 400:
+            raise BadRequestError(f"HTTP {r.status_code}: {r.text}")
+        if r.status_code == 401:
+            raise AuthenticationError(f"HTTP {r.status_code}: {r.text}")
+        if r.status_code == 403:
+            raise ForbiddenError(f"HTTP {r.status_code}: {r.text}")
+        if r.status_code == 404:
+            raise NotFoundError(f"HTTP {r.status_code}: {r.text}")
+        if r.status_code == 429:
+            raise RateLimitError(f"HTTP {r.status_code}: {r.text}")
+        if r.status_code == 500:
+            raise ServerError(f"HTTP {r.status_code}: {r.text}")
+
+        if action == DOWNLOAD:
+            return r.content
+
+        try:
+            r = r.json()
+        except JSONDecodeError:
+            return r.text
+
+        if data_type is not None:
+            if isinstance(r, list):
+                r = [data_type(result) for result in r]
+            elif r is not None:
+                r = data_type(r)
+
+        return r
+
+    @staticmethod
+    def random_email(amount: int, domain: str = None) -> List[str]:
+        """This method generates a list of random email addresses.
+
+        Parameters:
+        ----------
+
+            - `amount`: `int` - The number of email addresses to generate.
+            - `domain`: `str` (optional) - The domain name to use for the email addresses. If not provided, a random domain from the valid list of domains will be selected.
+
+        Example:
+        -------
+        Generate a list of 5 email addresses with the domain "1secmail.com":
+
+            >>> client.random_email(amount=5, domain="1secmail.com")
+
+        Valid domains:
+        -------------
+
+            - 1secmail.com
+            - 1secmail.org
+            - 1secmail.net
+            - kzccv.com
+            - qiott.com
+            - wuuvo.com
+            - icznn.com
+            - ezztt.com
+
+        If `domain` is provided and not in the valid list of domains, a ValueError will be raised with a message indicating the invalid domain and the valid list of domains.
+
+        """
+        if domain is not None and domain not in DOMAIN_LIST:
+            err_msg = (
+                f"{domain} is not a valid domain name.\nValid Domains: {DOMAIN_LIST}"
+            )
+            raise ValueError(err_msg)
+
+        emails = []
+        for _ in range(amount):
+            username = "".join(
+                random.choices(string.ascii_lowercase + string.digits, k=12)
+            )
+            email = f"{username}@{domain or random.choice(DOMAIN_LIST)}"
+            emails.append(email)
+
+        return emails
+
+    @staticmethod
+    def custom_email(username: str, domain: str = None) -> str:
+        """This method generates a custom email address.
+
+        Parameters:
+        ----------
+        - `username`: `str` - The username to use for the email address.
+        - `domain`: `str` (optional) - The domain name to use for the email address. If not provided, a random domain from the valid list of domains will be selected.
+
+        Returns:
+        -------
+        - `email`: `str` - The generated email address.
+
+        Example:
+        -------
+        Generate a custom email address with the username "johndoe":
+
+        >>> client.custom_email(username="johndoe")
+
+        Valid domains:
+        -------------
+        - 1secmail.com
+        - 1secmail.org
+        - 1secmail.net
+        - kzccv.com
+        - qiott.com
+        - wuuvo.com
+        - icznn.com
+        - ezztt.com
+
+        If `domain` is provided and not in the valid list of domains, a ValueError will be raised with a message indicating the invalid domain and the valid list of domains.
+
+        """
+        if domain is not None and domain not in DOMAIN_LIST:
+            err_msg = (
+                f"{domain} is not a valid domain name.\nValid Domains: {DOMAIN_LIST}"
+            )
+            raise ValueError(err_msg)
+
+        if is_valid_username(username) is False:
+            err_msg = f"'{username}' is not a valid username."
+            raise ValueError(err_msg)
+
+        return f"{username}@{domain or random.choice(DOMAIN_LIST)}"
+
+    async def await_new_message(self, address: str, fetch_interval=5) -> Inbox:
+        """This method waits until a new message is received for the specified email address.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to check for new messages.
+        - `fetch_interval`: `int` (optional) - The time interval (in seconds) for checking new messages. The default value is 5 seconds.
+
+        Returns:
+        -------
+        - `message`: `Inbox` - The new message received.
+
+        Example:
+        -------
+        Wait for a new message to be received for the email address "johndoe@1secmail.com":
+
+        >>> message = await client.await_new_message("johndoe@1secmail.com")
+
+        The method will continuously check for new messages every `fetch_interval` seconds until a new message is received. Once a new message is received, the message object is returned. The method also maintains a set of message IDs to check if the message is new. If the same message is received again, the method will continue to wait for a new message.
+
+        Note that if no new messages are received for a long time, the method may take a long time to return.
+
+        """
+        ids = {message.id for message in await self.get_inbox(address)}
+        while True:
+            await asyncio.sleep(fetch_interval)
+            new_messages = await self.get_inbox(address)
+            for message in new_messages:
+                if message.id not in ids:
+                    return message
+
+    async def get_active_domains(self) -> List[str]:
+        """This method retrieves a list of currently active domains.
+
+        Returns:
+        -------
+        - `domains`: `List[str]` - A list of active domains.
+
+        Example:
+        -------
+        Get a list of active domains:
+
+        >>> domains = await client.get_active_domains()
+
+        The method sends a GET request to the API endpoint to retrieve a list of currently active domains. The list is returned as a list of strings.
+
+        Note that the list of active domains may change over time.
+
+        """
+        return await self._request(action=GET_DOMAIN_LIST)
+
+    async def get_inbox(self, address: str) -> List[Inbox]:
+        """This method retrieves all the messages in the mailbox for the specified email address.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to check for messages.
+
+        Returns:
+        -------
+        - `messages`: `List[Inbox]` - A list of message objects in the mailbox.
+
+        Example:
+        -------
+        Get all the messages in the mailbox for the email address "johndoe@1secmail.com":
+
+        >>> messages = await client.get_inbox("johndoe@1secmail.com")
+
+        The method sends a GET request to the API endpoint to retrieve all the messages in the mailbox for the specified email address. The messages are returned as a list of inbox objects. If there are no messages in the mailbox, an empty list is returned.
+
+        """
+        username, domain = address.split("@")
+        return await self._request(
+            action=GET_MESSAGES,
+            params={"login": username, "domain": domain},
+            data_type=Inbox,
+        )
+
+    async def get_message(self, address: str, message_id: int) -> Message:
+        """This method retrieves a detailed message from the mailbox for the specified email address and message ID.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to check for the message.
+        - `message_id`: `int` - The ID of the message to retrieve.
+
+        Returns:
+        -------
+        - `message`: `Message` - The message object with the specified ID.
+
+        Example:
+        -------
+        Get the message with ID 12345 in the mailbox for the email address "johndoe@1secmail.com":
+
+        >>> message = await client.get_message("johndoe@1secmail.com", 12345)
+
+        The method sends a GET request to the API endpoint to retrieve the message with the specified ID in the mailbox for the specified email address. The message is returned as a message object.
+
+        """
+        username, domain = address.split("@")
+        return await self._request(
+            action=GET_SINGLE_MESSAGE,
+            params={"login": username, "domain": domain, "id": message_id},
+            data_type=Message,
+        )
+
+    async def save_email(self, address: str) -> None:
+        """This method saves the specified email address to a JSON file for future use.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to save.
+
+        Example:
+        -------
+        Save the email address "johndoe@1secmail.com" to the JSON file:
+
+        >>> await client.save_email("johndoe@1secmail.com")
+
+        The JSON file is saved in the base path specified during client initialization, with the name `secmail.json`.
+
+        """
+        data = {}
+
+        if not os.path.exists(self.base_path):
+            os.mkdir(self.base_path)
+
+        if os.path.exists(self.base_path + "secmail.json"):
+            with open(self.base_path + "secmail.json", "r") as f:
+                data = json.load(f)
+
+        data.setdefault("email", []).append(address)
+
+        with open(self.base_path + "secmail.json", "w") as f:
+            json.dump(data, f, indent=4)
+
+    async def download_attachment(
+        self,
+        address: str,
+        message_id: int,
+        filename: str,
+        save_path: str = current_path + "/config/",
+    ):
+        """This method downloads an attachment from a message in the mailbox for the specified email address and message ID.
+
+        Parameters:
+        ----------
+        - `address`: `str` - The email address to check for the message containing the attachment.
+        - `message_id`: `int` - The ID of the message containing the attachment to download.
+        - `filename`: `str` - The name of the attachment file to download.
+        - `save_path`: `str` - Optional. The path to save the downloaded attachment. Default is the current path + "/config/".
+
+        Returns:
+        -------
+        - `str` - A string indicating the path and size of the downloaded attachment.
+
+        Example:
+        -------
+        Download the attachment named "report.pdf" from the message with ID 12345 in the mailbox for the email address "johndoe@1secmail.com":
+
+        >>> await download_attachment("johndoe@1secmail.com", 12345, "report.pdf")
+
+        """
+        username, domain = address.split("@")
+        attachment = await self._request(
+            action=DOWNLOAD,
+            params={
+                "login": username,
+                "domain": domain,
+                "id": message_id,
+                "file": filename,
+            },
+        )
+
+        if not os.path.exists(self.base_path):
+            os.mkdir(self.base_path)
+
+        with open(save_path + filename, "wb") as attachment_file:
+            size = attachment_file.write(attachment)
+        return "Path: (" + save_path + filename + "), Size: " + str(size) + "B"
```

### Comparing `1secMail-1.0.0/secmail/models.py` & `1secMail-1.1.0/secmail/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,8 +112,8 @@
 
     def __init__(self, response) -> None:
         self.filename = response.get("filename")
         self.content_type = response.get("contentType")
         self.size = response.get("size")
 
     def __repr__(self) -> str:
-        return f"Attachment(id={self.filename}, from_address={self.content_type}, subject={self.size})"
+        return f"Attachment(filename={self.filename}, content_type={self.content_type}, size={self.size})"
```

### Comparing `1secMail-1.0.0/setup.py` & `1secMail-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup, find_packages
 from secmail.config import VERSION
 
 name = "1secMail"
 author = "qvco"
 author_email = "nikola.desuga@gmail.com"
-description = "Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python."
+description = "📧 Simple and intuitive, yet full featured API wrapper for www.1secmail.com, supporting both synchronous and asynchronous operations."
 long_description_content_type = "text/markdown"
 license = "MIT"
 url = "https://github.com/qvco/1secMail-Python"
 
 keywords = [
     "1secmail",
     "onesecmail",
     "tempmail",
     "disposable",
     "temporary",
     "email",
     "api",
     "wrapper",
     "library",
+    "async",
+    "asynchronous",
 ]
 
 install_requires = ["httpx>=0.17.1"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

