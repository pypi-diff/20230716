# Comparing `tmp/1stcaptcha-1.0.3.tar.gz` & `tmp/1stcaptcha-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1stcaptcha-1.0.3.tar", max compression
+gzip compressed data, was "1stcaptcha-1.0.4.tar", max compression
```

## Comparing `1stcaptcha-1.0.3.tar` & `1stcaptcha-1.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1869 2023-07-12 15:35:58.431699 1stcaptcha-1.0.3/README.md
--rw-r--r--   0        0        0     5910 2023-07-12 15:30:30.128050 1stcaptcha-1.0.3/onest_captcha/__init__.py
--rw-r--r--   0        0        0      724 2023-07-12 15:36:35.386056 1stcaptcha-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 1stcaptcha-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2443 2023-07-16 14:45:32.631339 1stcaptcha-1.0.4/README.md
+-rw-r--r--   0        0        0     7807 2023-07-16 14:39:54.732405 1stcaptcha-1.0.4/onest_captcha/__init__.py
+-rw-r--r--   0        0        0      724 2023-07-16 14:47:02.632674 1stcaptcha-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 1stcaptcha-1.0.4/PKG-INFO
```

### Comparing `1stcaptcha-1.0.3/README.md` & `1stcaptcha-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,36 +20,56 @@
 APIKEY = "0aa92cd8393a49698c408ea0ee56c2a5"
 client = OneStCaptchaClient(apikey=APIKEY)
 ```
 
 ## solver recaptcha v2:
 
 ```python
-site_key = "6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
-site_url = "https://www.google.com/recaptcha/api2/demo"
-invisible = False
-result = client.recaptcha_v2_task_proxyless(site_url, site_key, invisible=invisible)
+result = client.recaptcha_v2_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY", invisible=False)
+if result["code"] == 0:  # success:
+    print(result["token"])
+else:  # wrong
+    print(result["messeage"])
+```
+
+## solver recaptcha v2 enterprise:
+
+```python
+
+result = client.recaptcha_v2_enterprise_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY")
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
 ## solver recaptcha v3:
 
 ```python
-token = client.recaptcha_v3_task_proxyless(site_key="YOUR_SITE_KEY",
-                                           site_url="YOUR_SITE_URL",
-                                           page_action="YOUR_PAGE_ACTION")
+result = client.recaptcha_v3_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY",
+                                            page_action="YOUR_PAGE_ACTION")
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
+## solver recaptcha v3 enterprise:
+
+```python
+result = client.recaptcha_v3_enterprise_task_proxyless(site_key="YOUR_SITE_KEY",
+                                                       site_url="YOUR_SITE_URL",
+                                                       page_action="YOUR_PAGE_ACTION")
+if result["code"] == 0:  # success:
+    print(result.get('token'))
+    print(result.get('user_agent'))
+else:  # wrong
+    print(result["messeage"])
+```
+
 ## solve image2text
 
 ```python
 
 result = client.image_to_text(file="1.jpg")
 if result["code"] == 0:  # success:
     print(result["token"])
```

### Comparing `1stcaptcha-1.0.3/onest_captcha/__init__.py` & `1stcaptcha-1.0.4/onest_captcha/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,16 @@
             r = requests.get(f"{self.BASE_URL}/getresult?apikey=" + self.apikey + "&taskid=" + str(task_id))
             if r.status_code == 200:
                 data = r.json()
                 if data['Code'] == 0:
                     if data['Status'] == "SUCCESS":
                         if type_captcha == "image2text" or type_captcha == "recaptcha_click":
                             return data["Data"]
+                        elif type_captcha == "v3_enterprise":
+                            return data["Data"]
                         return data["Data"]["Token"]
                     elif data['Status'] == "ERROR":
                         raise Exception(data["Message"])
                     time.sleep(time_sleep)
                 else:
                     raise RuntimeError("Error " + data["Message"])
             else:
@@ -59,14 +61,31 @@
                     raise RuntimeError("Error " + str(data))
             else:
                 raise RuntimeError("Error " + r.text)
             return {"code": 0, "token": self.get_result(task_id, timeout, time_sleep)}
         except Exception as e:
             return {"code": 1, "messeage": str(e)}
 
+    def recaptcha_v2_enterprise_task_proxyless(self, site_url, site_key, timeout=180, time_sleep=1):
+        try:
+            r = requests.get(
+                f"{self.BASE_URL}/recaptchav2_enterprise?apikey={self.apikey}&sitekey={site_key}&siteurl={site_url}"
+            )
+            if r.status_code == 200:
+                data = r.json()
+                if data['Code'] == 0:
+                    task_id = data['TaskId']
+                else:
+                    raise RuntimeError("Error " + str(data))
+            else:
+                raise RuntimeError("Error " + r.text)
+            return {"code": 0, "token": self.get_result(task_id, timeout, time_sleep)}
+        except Exception as e:
+            return {"code": 1, "messeage": str(e)}
+
     def recaptcha_v3_task_proxyless(self, site_url, site_key, page_action, min_score: float = 0.3, timeout=180,
                                     time_sleep=1):
         try:
             r = requests.get(
                 f"{self.BASE_URL}/recaptchav3?apikey={self.apikey}&sitekey={site_key}&siteurl={site_url}&version=v3&pageaction={page_action}&minscore={min_score}"
             )
             if r.status_code == 200:
@@ -77,14 +96,40 @@
                     raise RuntimeError("Error " + str(data))
             else:
                 raise RuntimeError("Error " + r.text)
             return {"code": 0, "token": self.get_result(task_id, timeout, time_sleep)}
         except Exception as e:
             return {"code": 1, "messeage": str(e)}
 
+    def recaptcha_v3_enterprise_task_proxyless(
+            self,
+            site_url,
+            site_key,
+            page_action,
+            min_score: float = 0.3,
+            timeout=180,
+            time_sleep=1
+    ):
+        try:
+            r = requests.get(
+                f"{self.BASE_URL}/recaptchav3_enterprise?apikey={self.apikey}&sitekey={site_key}&siteurl={site_url}&pageaction={page_action}&minscore={min_score}"
+            )
+            if r.status_code == 200:
+                data = r.json()
+                if data['Code'] == 0:
+                    task_id = data['TaskId']
+                else:
+                    raise RuntimeError("Error " + str(data))
+            else:
+                raise RuntimeError("Error " + r.text)
+            result = self.get_result(task_id, timeout, time_sleep, type_captcha="v3_enterprise")
+            return {"code": 0, "token": result.get("Token"), "user_agent": result.get("UserAgent")}
+        except Exception as e:
+            return {"code": 1, "messeage": str(e)}
+
     def fun_captcha_task_proxyless(self, site_url, site_key, timeout=180, time_sleep=3):
         try:
             r = requests.get(
                 f"{self.BASE_URL}/funcaptchatokentask?apikey={self.apikey}&sitekey={site_key}&siteurl={site_url}"
             )
             if r.status_code == 200:
                 data = r.json()
```

### Comparing `1stcaptcha-1.0.3/pyproject.toml` & `1stcaptcha-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "1stcaptcha"
 packages = [
     { include = "onest_captcha" },
 ]
-version = "1.0.3"
+version = "1.0.4"
 description = "Solver recaptchaV2, recaptchaV3, hcaptcha, funcaptcha, imageToText, Zalo Captcha,.... Super fast and cheapest"
 authors = ["NguyenLinhUET <nguyenlinh.uet@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/1stcaptcha/1stcaptcha-python"
 homepage = "https://github.com/1stcaptcha/1stcaptcha-python"
 license = "MIT"
 keywords = ["1stcaptcha", "recaptcha", "recaptchav3", "hcaptcha", "funcaptcha", "imagetotext", "zalo captcha", "solver captcha"]
```

### Comparing `1stcaptcha-1.0.3/PKG-INFO` & `1stcaptcha-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1stcaptcha
-Version: 1.0.3
+Version: 1.0.4
 Summary: Solver recaptchaV2, recaptchaV3, hcaptcha, funcaptcha, imageToText, Zalo Captcha,.... Super fast and cheapest
 Home-page: https://github.com/1stcaptcha/1stcaptcha-python
 License: MIT
 Keywords: 1stcaptcha,recaptcha,recaptchav3,hcaptcha,funcaptcha,imagetotext,zalo captcha,solver captcha
 Author: NguyenLinhUET
 Author-email: nguyenlinh.uet@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -41,36 +41,56 @@
 APIKEY = "0aa92cd8393a49698c408ea0ee56c2a5"
 client = OneStCaptchaClient(apikey=APIKEY)
 ```
 
 ## solver recaptcha v2:
 
 ```python
-site_key = "6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
-site_url = "https://www.google.com/recaptcha/api2/demo"
-invisible = False
-result = client.recaptcha_v2_task_proxyless(site_url, site_key, invisible=invisible)
+result = client.recaptcha_v2_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY", invisible=False)
+if result["code"] == 0:  # success:
+    print(result["token"])
+else:  # wrong
+    print(result["messeage"])
+```
+
+## solver recaptcha v2 enterprise:
+
+```python
+
+result = client.recaptcha_v2_enterprise_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY")
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
 ## solver recaptcha v3:
 
 ```python
-token = client.recaptcha_v3_task_proxyless(site_key="YOUR_SITE_KEY",
-                                           site_url="YOUR_SITE_URL",
-                                           page_action="YOUR_PAGE_ACTION")
+result = client.recaptcha_v3_task_proxyless(site_url="YOUR_SITE_URL", site_key="YOUR_SITE_KEY",
+                                            page_action="YOUR_PAGE_ACTION")
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
+## solver recaptcha v3 enterprise:
+
+```python
+result = client.recaptcha_v3_enterprise_task_proxyless(site_key="YOUR_SITE_KEY",
+                                                       site_url="YOUR_SITE_URL",
+                                                       page_action="YOUR_PAGE_ACTION")
+if result["code"] == 0:  # success:
+    print(result.get('token'))
+    print(result.get('user_agent'))
+else:  # wrong
+    print(result["messeage"])
+```
+
 ## solve image2text
 
 ```python
 
 result = client.image_to_text(file="1.jpg")
 if result["code"] == 0:  # success:
     print(result["token"])
```

