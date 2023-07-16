# Comparing `tmp/wcfhttp-39.0.0.1.tar.gz` & `tmp/wcfhttp-39.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-39.0.0.1.tar", last modified: Thu Jul 13 16:19:43 2023, max compression
+gzip compressed data, was "wcfhttp-39.0.2.0.tar", last modified: Sun Jul 16 16:25:43 2023, max compression
```

## Comparing `wcfhttp-39.0.0.1.tar` & `wcfhttp-39.0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1828 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-13 16:19:43.734645 wcfhttp-39.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1421 2023-07-13 15:41:43.000000 wcfhttp-39.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.719024 wcfhttp-39.0.0.1/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    15462 2023-07-13 16:18:20.000000 wcfhttp-39.0.0.1/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.1/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:19:43.719024 wcfhttp-39.0.0.1/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1828 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 16:19:43.000000 wcfhttp-39.0.0.1/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1842 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-16 16:25:43.951925 wcfhttp-39.0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-07-16 16:22:36.000000 wcfhttp-39.0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.936301 wcfhttp-39.0.2.0/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.2.0/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    16617 2023-07-16 16:22:36.000000 wcfhttp-39.0.2.0/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     2317 2023-07-15 02:26:29.000000 wcfhttp-39.0.2.0/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:25:43.936301 wcfhttp-39.0.2.0/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1842 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 16:25:43.000000 wcfhttp-39.0.2.0/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-39.0.0.1/PKG-INFO` & `wcfhttp-39.0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.1
+Version: 39.0.2.0
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -42,10 +42,10 @@
 # 新消息转发到指定地址
 wcfhttp --cb http://your_host:your_port/callback
 ```
 
 ### 接收消息回调接口文档
 参考文档（默认地址为：http://localhost:9999/docs ）`接收消息回调样例`。
 
-|![碲矿](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/TEQuant.jpg)|![赞赏](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/QR.jpeg)|
+|![碲矿](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/assets/TEQuant.jpg)|![赞赏](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/assets/QR.jpeg)|
 |:-:|:-:|
 |后台回复 `WeChatFerry` 加群交流|如果你觉得有用|
```

### Comparing `wcfhttp-39.0.0.1/setup.py` & `wcfhttp-39.0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
         "fastapi",
         "uvicorn[standard]",
-        "wcferry>=39.0.0.0",
+        "wcferry>=39.0.2.0",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-39.0.0.1/wcfhttp/core.py` & `wcfhttp-39.0.2.0/wcfhttp/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import base64
 import logging
+from queue import Empty
+from threading import Thread
 from typing import Any
 
 import requests
-from fastapi import Body, FastAPI
+from fastapi import Body, Query, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "39.0.0.1"
+__version__ = "39.0.2.0"
 
 
 class Msg(BaseModel):
-    id: str
+    id: int
+    ts: int
+    sign: str
     type: int
     xml: str
     sender: str
     roomid: str
     content: str
     thumb: str
     extra: str
@@ -42,52 +46,68 @@
         self.add_api_route("/wxid", self.get_self_wxid, methods=["GET"], summary="获取登录账号 wxid")
         self.add_api_route("/user-info", self.get_user_info, methods=["GET"], summary="获取登录账号个人信息")
         self.add_api_route("/msg-types", self.get_msg_types, methods=["GET"], summary="获取消息类型")
         self.add_api_route("/contacts", self.get_contacts, methods=["GET"], summary="获取完整通讯录")
         self.add_api_route("/friends", self.get_friends, methods=["GET"], summary="获取好友列表")
         self.add_api_route("/dbs", self.get_dbs, methods=["GET"], summary="获取所有数据库")
         self.add_api_route("/{db}/tables", self.get_tables, methods=["GET"], summary="获取 db 中所有表")
+        self.add_api_route("/pyq/", self.refresh_pyq, methods=["GET"], summary="刷新朋友圈（数据从消息回调中查看）")
 
         self.add_api_route("/text", self.send_text, methods=["POST"], summary="发送文本消息")
         self.add_api_route("/image", self.send_image, methods=["POST"], summary="发送图片消息")
         self.add_api_route("/file", self.send_file, methods=["POST"], summary="发送文件消息")
         # self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
         # self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
         self.add_api_route("/sql", self.query_sql, methods=["POST"], summary="执行 SQL，如果数据量大注意分页，以免 OOM")
         self.add_api_route("/new-friend", self.accept_new_friend, methods=["POST"], summary="通过好友申请")
         self.add_api_route("/chatroom-member", self.add_chatroom_members, methods=["POST"], summary="添加群成员")
-        self.add_api_route("/chatroom-member", self.del_chatroom_members, methods=["DELETE"], summary="删除群成员")
         self.add_api_route("/transfer", self.receive_transfer, methods=["POST"], summary="接收转账")
         self.add_api_route("/dec-image", self.decrypt_image, methods=["POST"], summary="解密图片")
 
+        self.add_api_route("/chatroom-member", self.del_chatroom_members, methods=["DELETE"], summary="删除群成员")
+
+    def _forward_msg(self, msg, cb):
+        data = {}
+        data["id"] = msg.id
+        data["ts"] = msg.ts
+        data["sign"] = msg.sign
+        data["type"] = msg.type
+        data["xml"] = msg.xml
+        data["sender"] = msg.sender
+        data["roomid"] = msg.roomid
+        data["content"] = msg.content
+        data["thumb"] = msg.thumb
+        data["extra"] = msg.extra
+        data["is_at"] = msg.is_at(self.wcf.self_wxid)
+        data["is_self"] = msg.from_self()
+        data["is_group"] = msg.from_group()
+
+        try:
+            rsp = requests.post(url=cb, json=data)
+            if rsp.status_code != 200:
+                self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
+        except Exception as e:
+            self.LOG.error(f"消息转发异常: {e}")
+
     def _set_cb(self, cb):
-        def callback(msg: WxMsg):
-            data = {}
-            data["id"] = msg.id
-            data["type"] = msg.type
-            data["xml"] = msg.xml
-            data["sender"] = msg.sender
-            data["roomid"] = msg.roomid
-            data["content"] = msg.content
-            data["thumb"] = msg.thumb
-            data["extra"] = msg.extra
-            data["is_at"] = msg.is_at(self.wcf.self_wxid)
-            data["is_self"] = msg.from_self()
-            data["is_group"] = msg.from_group()
-
-            try:
-                rsp = requests.post(url=cb, json=data)
-                if rsp.status_code != 200:
-                    self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
-            except Exception as e:
-                self.LOG.error(f"消息转发异常: {e}")
+        def callback(wcf: Wcf):
+            while wcf.is_receiving_msg():
+                try:
+                    msg = wcf.get_msg()
+                    self.LOG.info(msg)
+                    self._forward_msg(msg, cb)
+                except Empty:
+                    continue  # Empty message
+                except Exception as e:
+                    self.LOG.error(f"Receiving message error: {e}")
 
         if cb:
             self.LOG.info(f"消息回调: {cb}")
-            self.wcf.enable_recv_msg(callback=callback)
+            self.wcf.enable_receiving_msg(pyq=True)  # 同时允许接收朋友圈消息
+            Thread(target=callback, name="GetMessage", args=(self.wcf,), daemon=True).start()
         else:
             self.LOG.info(f"没有设置回调，打印消息")
             self.wcf.enable_recv_msg(print)
 
     def is_login(self) -> dict:
         """获取登录状态"""
         ret = self.wcf.is_login()
@@ -320,14 +340,26 @@
 
         Returns:
             int: 1 为成功，其他失败
         """
         ret = self.wcf.receive_transfer(wxid, transferid, transactionid)
         return {"status": ret, "message": "成功"if ret == 1 else "失败"}
 
+    def refresh_pyq(self, id: int = Query(0, description="开始 id，0 为最新页")) -> dict:
+        """刷新朋友圈
+
+        Args:
+            id (int): 开始 id，0 为最新页
+
+        Returns:
+            int: 1 为成功，其他失败
+        """
+        ret = self.wcf.refresh_pyq(id)
+        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
+
     def decrypt_image(self,
                       src: str = Body("C:\\...", description="加密的图片路径，从图片消息中获取"),
                       dst: str = Body("C:\\...", description="解密的图片路径")) -> dict:
         """解密图片:
 
         Args:
             src (str): 加密的图片路径
```

### Comparing `wcfhttp-39.0.0.1/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-39.0.2.0/wcfhttp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 39.0.0.1
+Version: 39.0.2.0
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -42,10 +42,10 @@
 # 新消息转发到指定地址
 wcfhttp --cb http://your_host:your_port/callback
 ```
 
 ### 接收消息回调接口文档
 参考文档（默认地址为：http://localhost:9999/docs ）`接收消息回调样例`。
 
-|![碲矿](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/TEQuant.jpg)|![赞赏](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/QR.jpeg)|
+|![碲矿](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/assets/TEQuant.jpg)|![赞赏](https://raw.githubusercontent.com/lich0821/WeChatFerry/master/assets/QR.jpeg)|
 |:-:|:-:|
 |后台回复 `WeChatFerry` 加群交流|如果你觉得有用|
```

