# Comparing `tmp/yaylib-0.1.5.tar.gz` & `tmp/yaylib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-0.1.5.tar", last modified: Sat Jul  8 15:02:44 2023, max compression
+gzip compressed data, was "yaylib-1.0.0.tar", last modified: Sun Jul 16 09:15:39 2023, max compression
```

## Comparing `yaylib-0.1.5.tar` & `yaylib-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.273987 yaylib-0.1.5/
--rw-rw-rw-   0        0        0     1088 2023-07-08 04:33:49.000000 yaylib-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     8205 2023-07-08 15:02:44.273987 yaylib-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7341 2023-07-08 15:02:21.000000 yaylib-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 15:02:44.273987 yaylib-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-08 14:37:25.000000 yaylib-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.227270 yaylib-0.1.5/tests/
--rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_call.py
--rw-rw-rw-   0        0        0      827 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_cassandra.py
--rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_chat.py
--rw-rw-rw-   0        0        0      229 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_group.py
--rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_misc.py
--rw-rw-rw-   0        0        0     2615 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_post.py
--rw-rw-rw-   0        0        0      920 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_review.py
--rw-rw-rw-   0        0        0      231 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_thread.py
--rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.234213 yaylib-0.1.5/yaylib/
--rw-rw-rw-   0        0        0      288 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.272982 yaylib-0.1.5/yaylib/api/
--rw-rw-rw-   0        0        0      466 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0     8312 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/api.py
--rw-rw-rw-   0        0        0     6242 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/call.py
--rw-rw-rw-   0        0        0     1391 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    11309 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    19089 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8042 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/login.py
--rw-rw-rw-   0        0        0     5067 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    28876 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/post.py
--rw-rw-rw-   0        0        0     2847 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/review.py
--rw-rw-rw-   0        0        0     4074 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    17806 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/user.py
--rw-rw-rw-   0        0        0    67557 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/client.py
--rw-rw-rw-   0        0        0    18106 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/config.py
--rw-rw-rw-   0        0        0      373 2023-07-08 10:04:28.000000 yaylib-0.1.5/yaylib/errors.py
--rw-rw-rw-   0        0        0    52228 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/models.py
--rw-rw-rw-   0        0        0    31004 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/responses.py
--rw-rw-rw-   0        0        0     1428 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.260244 yaylib-0.1.5/yaylib.egg-info/
--rw-rw-rw-   0        0        0     8205 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.775312 yaylib-1.0.0/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    10834 2023-07-16 09:15:39.773997 yaylib-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 09:15:39.775312 yaylib-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.726106 yaylib-1.0.0/tests/
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.0/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.733817 yaylib-1.0.0/yaylib/
+-rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.773997 yaylib-1.0.0/yaylib/api/
+-rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10272 2023-07-16 08:55:57.000000 yaylib-1.0.0/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.0/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14793 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8260 2023-07-16 08:52:39.000000 yaylib-1.0.0/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7401 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    24484 2023-07-16 08:42:11.000000 yaylib-1.0.0/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    86196 2023-07-16 08:15:00.000000 yaylib-1.0.0/yaylib/client.py
+-rw-rw-rw-   0        0        0    19214 2023-07-16 09:09:09.000000 yaylib-1.0.0/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/errors.py
+-rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/models.py
+-rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.0/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4612 2023-07-16 04:28:15.000000 yaylib-1.0.0/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 09:15:39.761319 yaylib-1.0.0/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    10834 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 09:15:39.000000 yaylib-1.0.0/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-0.1.5/LICENSE` & `yaylib-1.0.0/tests/test_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+"""
 MIT License
 
-Copyright (c) 2023 Qvco, Konn
+Copyright (c) 2023-present Qvco, Konn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,7 +16,25 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+"""
+
+import unittest
+
+from config import (
+    tape,
+    user_id,
+    opponent_id,
+    YaylibTestCase,
+)
+
+
+class YaylibGroupTests(YaylibTestCase):
+    path = "./group/"
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `yaylib-0.1.5/PKG-INFO` & `yaylib-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.5
+Version: 1.0.0
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -31,15 +31,15 @@
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
-            <strong>詳しい機能の詳細や使い方はこちらから »</strong>
+            <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
         ·
@@ -48,46 +48,40 @@
 </p>
 
 <!-- TABLE OF CONTENTS -->
 
 <details>
   <summary>Table of Contents</summary>
   <ol>
+    <li><a href="#-installation">インストール</a></li>
+    <li><a href="#-quick-example">使用例</a></li>
+    <li><a href="#crown-yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
     <li><a href="#buy-me-a-coffee">Buy me a coffee</a></li>
-    <li><a href="#インストール">インストール</a></li>
-    <li><a href="#使用例">使用例</a></li>
-    <li><a href="#yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
-    <li><a href="#共同開発について">共同開発について</a></li>
+    <li><a href="#handshake-共同開発について">共同開発について</a></li>
     <li><a href="#免責事項">免責事項</a></li>
     <li><a href="#利用許諾">利用許諾</a></li>
   </ol>
 </details>
 
-<!-- Buy me a coffee -->
-
-## Buy me a coffee
-
-このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
-また、Buy Me a Coffee からご支援いただけますと幸いです。
-
-<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
-
 <!-- インストール -->
 
-## インストール
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
 「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
-開発バージョンをインストールするには、以下の手順を実行します:
+<br>
+
+> **Note**
+> 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
 git clone https://github.com/qvco/yaylib
 
 cd yaylib
 
 pip install -r requirements.txt
@@ -95,42 +89,125 @@
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
-## 使用例
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
+
+#### ✨ 投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!")
+```
+
+#### ✨ 埋め込みリンクの投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
+```
+
+<p align="center">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
+</p>
+
+#### ✨ 画像と一緒に投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+filename = api.upload_image(
+    image_type="post", # 画像の使い道を指定
+    image_path="./path/to/image" # ローカルにある画像のパス
+)
+
+api.create_post("Hello with yaylib!", attachment_filename=filename)
+```
+
+#### ✨ 投稿に返信する
 
-メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", in_reply_to=373189088)
+```
+
+#### ✨ タイムラインを 100 件取得する
 
 ```python
 import yaylib
 
+api = yaylib.Client()
+
+timeline = api.get_timeline(number=100)
+
+for post in timeline.posts:
+    print(post.user.nickname)  # 投稿者
+    print(post.text)  # 本文
+    print(post.likes_count)  # いいね数
+    print(post.reposts_count)  # (´∀｀∩)↑age↑の数
+    print(post.in_reply_to_post_count)  # 返信の数
+```
+
+#### ✨ タイムラインをキーワードで検索して「いいね」する
+
+```python
+import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_post(post.id)
+    response = api.like_posts(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
+#### ✨ タイムラインのユーザーをフォローする
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+timeline = api.get_timeline(number=15)
+
+for post in timeline.posts:
+    api.follow_user(post.user.id)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
-## yaylib で誕生したロボットたち
+## :crown: yaylib で誕生したロボットたち
 
 「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
@@ -157,31 +234,50 @@
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
-## 共同開発について
+## :handshake: 共同開発について
 
-私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
+私たちと開発することに興味を持っていただけているなら、ぜひ参加して頂きたいです！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
-- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
+- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com にメールを送信する</a>
+
+のいずれかの方法で繋がりましょう。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
+<!-- Buy me a coffee -->
+
+## Buy me a coffee
+
+このライブラリが気に入っていただけたら、**リポジトリに<a href="https://github.com/qvco/yaylib/">スターをお願いします</a>(⭐)**  
+また、Buy Me a Coffee からご支援いただけますと幸いです。
+
+<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
-<!-- 利用許諾 -->
+<!-- ライセンス -->
+
+## ライセンス
 
-## 利用許諾
+<p align="center">
+  <a href="https://github.com/qvco">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-791308b393af" width="256" height="256">
+  </a>
+</p>
+
+<p align="center">
+  <strong>MIT © <a href="https://github.com/qvco">Qvco</a> & <a href="https://github.com/konn-koko">Konn</a></strong>
+</p>
 
 フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.5 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.0 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
@@ -19,62 +19,95 @@
 
                                     [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
                            API ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
-          è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
+                   ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
-   1. Buy_me_a_coffee
-   2. ã¤ã³ã¹ãã¼ã«
-   3. ä½¿ç¨ä¾
-   4. yaylib_ã§èªçããã­ããããã¡
+   1. ã¤ã³ã¹ãã¼ã«
+   2. ä½¿ç¨ä¾
+   3. yaylib_ã§èªçããã­ããããã¡
+   4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
-  ## Buy me a coffee
-ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
-â­ï¸ ã¾ããBuy Me a Coffee
-ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
-ã¤ã³ã¹ãã¼ã« **â» Python 3.11
+  ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
-éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
+> **Note** >
+éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
-ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
+[https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
+3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
+åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+shared_url="https://github.com/qvco/yaylib") ```
+                            [Writing Text Threads]
+#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
+ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
+ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
+attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
+import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
+```python import yaylib api = yaylib.Client() timeline = api.get_timeline
+(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
+print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
+(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
+(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_post(post.id) print(post.id,
-response.data) # å®è¡çµæãåºå ```
+post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
+api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
+timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡
+ ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
       cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
             éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
                                                                                                                                  éçºè: ãºãã¼
- ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
-- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
-ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
-ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
+ ## :handshake: å±åéçºã«ã¤ãã¦
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦é ãããã§ãï¼
+- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã -
+nikola.desuga@gmail.com_ã«ã¡ã¼ã«ãéä¿¡ãã
+ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
-CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
+CONTRIBUTING.md)ï¼  ## Buy me a coffee
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
+(â­)** ã¾ããBuy Me a Coffee
+ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
+åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
-## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
+## ã©ã¤ã»ã³ã¹
+   [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
+                                 791308b393af]
+                              MIT Â© Qvco & Konn
+ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
+master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.5/README.md` & `yaylib-1.0.0/yaylib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: yaylib
+Version: 1.0.0
+Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
+Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib
+Author: Qvco, Konn
+Author-email: nikola.desuga@gmail.com
+Maintainer: Qvco, Konn
+Maintainer-email: nikola.desuga@gmail.com
+License: MIT
+Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
@@ -13,15 +31,15 @@
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
-            <strong>詳しい機能の詳細や使い方はこちらから »</strong>
+            <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
         ·
@@ -30,46 +48,40 @@
 </p>
 
 <!-- TABLE OF CONTENTS -->
 
 <details>
   <summary>Table of Contents</summary>
   <ol>
+    <li><a href="#-installation">インストール</a></li>
+    <li><a href="#-quick-example">使用例</a></li>
+    <li><a href="#crown-yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
     <li><a href="#buy-me-a-coffee">Buy me a coffee</a></li>
-    <li><a href="#インストール">インストール</a></li>
-    <li><a href="#使用例">使用例</a></li>
-    <li><a href="#yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
-    <li><a href="#共同開発について">共同開発について</a></li>
+    <li><a href="#handshake-共同開発について">共同開発について</a></li>
     <li><a href="#免責事項">免責事項</a></li>
     <li><a href="#利用許諾">利用許諾</a></li>
   </ol>
 </details>
 
-<!-- Buy me a coffee -->
-
-## Buy me a coffee
-
-このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
-また、Buy Me a Coffee からご支援いただけますと幸いです。
-
-<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
-
 <!-- インストール -->
 
-## インストール
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
 「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
-開発バージョンをインストールするには、以下の手順を実行します:
+<br>
+
+> **Note**
+> 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
 git clone https://github.com/qvco/yaylib
 
 cd yaylib
 
 pip install -r requirements.txt
@@ -77,42 +89,125 @@
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
-## 使用例
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
-メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
+#### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!")
+```
+
+#### ✨ 埋め込みリンクの投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
+```
+
+<p align="center">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
+</p>
+
+#### ✨ 画像と一緒に投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+filename = api.upload_image(
+    image_type="post", # 画像の使い道を指定
+    image_path="./path/to/image" # ローカルにある画像のパス
+)
+
+api.create_post("Hello with yaylib!", attachment_filename=filename)
+```
+
+#### ✨ 投稿に返信する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", in_reply_to=373189088)
+```
+
+#### ✨ タイムラインを 100 件取得する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+
+timeline = api.get_timeline(number=100)
+
+for post in timeline.posts:
+    print(post.user.nickname)  # 投稿者
+    print(post.text)  # 本文
+    print(post.likes_count)  # いいね数
+    print(post.reposts_count)  # (´∀｀∩)↑age↑の数
+    print(post.in_reply_to_post_count)  # 返信の数
+```
+
+#### ✨ タイムラインをキーワードで検索して「いいね」する
+
+```python
+import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_post(post.id)
+    response = api.like_posts(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
+#### ✨ タイムラインのユーザーをフォローする
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+timeline = api.get_timeline(number=15)
+
+for post in timeline.posts:
+    api.follow_user(post.user.id)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
-## yaylib で誕生したロボットたち
+## :crown: yaylib で誕生したロボットたち
 
 「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
@@ -139,31 +234,50 @@
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
-## 共同開発について
+## :handshake: 共同開発について
 
-私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
+私たちと開発することに興味を持っていただけているなら、ぜひ参加して頂きたいです！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
-- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
+- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com にメールを送信する</a>
+
+のいずれかの方法で繋がりましょう。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
+<!-- Buy me a coffee -->
+
+## Buy me a coffee
+
+このライブラリが気に入っていただけたら、**リポジトリに<a href="https://github.com/qvco/yaylib/">スターをお願いします</a>(⭐)**  
+また、Buy Me a Coffee からご支援いただけますと幸いです。
+
+<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
-<!-- 利用許諾 -->
+<!-- ライセンス -->
+
+## ライセンス
 
-## 利用許諾
+<p align="center">
+  <a href="https://github.com/qvco">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-791308b393af" width="256" height="256">
+  </a>
+</p>
+
+<p align="center">
+  <strong>MIT © <a href="https://github.com/qvco">Qvco</a> & <a href="https://github.com/konn-koko">Konn</a></strong>
+</p>
 
 フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,68 +1,113 @@
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.0 Summary: This Python package
+provides an easy-to-use interface for accessing data from Yay! (https://
+yay.space/). With this API Client, you can retrieve user profiles, posts,
+comments, and other content from Yay!, as well as perform common tasks like
+liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
+nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
+nikola.desuga@gmail.com License: MIT Keywords:
+yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
                                     [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
                            API ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
-          è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
+                   ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
-   1. Buy_me_a_coffee
-   2. ã¤ã³ã¹ãã¼ã«
-   3. ä½¿ç¨ä¾
-   4. yaylib_ã§èªçããã­ããããã¡
+   1. ã¤ã³ã¹ãã¼ã«
+   2. ä½¿ç¨ä¾
+   3. yaylib_ã§èªçããã­ããããã¡
+   4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
-  ## Buy me a coffee
-ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
-â­ï¸ ã¾ããBuy Me a Coffee
-ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
-ã¤ã³ã¹ãã¼ã« **â» Python 3.11
+  ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
-éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
+> **Note** >
+éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
-ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
+[https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
+3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
+åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+shared_url="https://github.com/qvco/yaylib") ```
+                            [Writing Text Threads]
+#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
+ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
+ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
+attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
+import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
+```python import yaylib api = yaylib.Client() timeline = api.get_timeline
+(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
+print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
+(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
+(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_post(post.id) print(post.id,
-response.data) # å®è¡çµæãåºå ```
+post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
+api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
+timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡
+ ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
       cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
             éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
                                                                                                                                  éçºè: ãºãã¼
- ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
-- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
-ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
-ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
+ ## :handshake: å±åéçºã«ã¤ãã¦
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦é ãããã§ãï¼
+- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã -
+nikola.desuga@gmail.com_ã«ã¡ã¼ã«ãéä¿¡ãã
+ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
-CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
+CONTRIBUTING.md)ï¼  ## Buy me a coffee
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
+(â­)** ã¾ããBuy Me a Coffee
+ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
+åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
-## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
+## ã©ã¤ã»ã³ã¹
+   [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
+                                 791308b393af]
+                              MIT Â© Qvco & Konn
+ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
+master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.5/setup.py` & `yaylib-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.5/yaylib/api/call.py` & `yaylib-1.0.0/yaylib/api/call.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,156 @@
-from datetime import datetime
-from typing import Dict, List
+"""
+MIT License
 
-from ..config import *
-from ..errors import *
-from ..models import *
-from ..responses import *
-from ..utils import *
+Copyright (c) 2023-present Qvco, Konn
 
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import List
+
+from ..config import Endpoints
+from ..models import Bgm, ConferenceCall, Post
+from ..responses import (
+    BgmsResponse,
+    CallStatusResponse,
+    ConferenceCallResponse,
+    GamesResponse,
+    GenresResponse,
+    PostResponse,
+    PostsResponse,
+    UsersByTimestampResponse,
+)
 
-def bump_call(self, call_id: int, participant_limit: int = None):
+
+def bump_call(
+    self, call_id: int, participant_limit: int = None, access_token: str = None
+):
     params = {}
     if participant_limit:
         params["participant_limit"] = participant_limit
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bump", params=params
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bump",
+        params=params,
+        access_token=access_token,
     )
     self.logger.info("Call bumped.")
     return response
 
 
-def get_user_active_call(self, user_id: int) -> Post:
+def get_user_active_call(self, user_id: int, access_token: str = None) -> Post:
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.POSTS_V1}/active_call",
         params={"user_id": user_id},
         data_type=PostResponse,
+        access_token=access_token,
     ).post
 
 
-def get_bgms(self) -> List[Bgm]:
+def get_bgms(self, access_token: str = None) -> List[Bgm]:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CALLS_V1}/bgm", data_type=BgmsResponse
+        "GET",
+        endpoint=f"{Endpoints.CALLS_V1}/bgm",
+        data_type=BgmsResponse,
+        access_token=access_token,
     ).bgm
 
 
-def get_call(self, call_id: int) -> ConferenceCall:
+def get_call(self, call_id: int, access_token: str = None) -> ConferenceCall:
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.CALLS_V1}/conferences/{call_id}",
         data_type=ConferenceCallResponse,
+        access_token=access_token,
     ).conference_call
 
 
 def get_call_invitable_users(
-    self, call_id: int, from_timestamp: int = None
+    self, call_id: int, from_timestamp: int = None, access_token: str = None
 ) -> UsersByTimestampResponse:
     # @Nullable @Query("user[nickname]")
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/invitable",
         params=params,
         data_type=UsersByTimestampResponse,
+        access_token=access_token,
     )
 
 
-def get_call_status(self, opponent_id: int) -> CallStatusResponse:
+def get_call_status(
+    self, opponent_id: int, access_token: str = None
+) -> CallStatusResponse:
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.CALLS_V1}/phone_status/{opponent_id}",
         data_type=CallStatusResponse,
+        access_token=access_token,
     )
 
 
-def get_games(self, **params) -> GamesResponse:
+def get_games(self, access_token: str = None, **params) -> GamesResponse:
     """
 
     Parameters
     ----------
         - number: int - (optional)
         - ids: List[int] - (optional)
         - from_id: int - (optional)
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.GAMES_V1}/apps",
         params=params,
         data_type=GamesResponse,
+        access_token=access_token,
     )
 
 
-def get_genres(self, **params) -> GenresResponse:
+def get_genres(self, access_token: str = None, **params) -> GenresResponse:
     """
 
     Parameters
     ----------
         - number: int - (optional)
         - from: int - (optional)
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.GENRES_V1}",
         params=params,
         data_type=GenresResponse,
+        access_token=access_token,
     )
 
 
-def get_group_calls(self, **params) -> PostsResponse:
+def get_group_calls(self, access_token: str = None, **params) -> PostsResponse:
     """
 
     Parameters
     ----------
         - number: int - (optional)
         - group_category_id: int - (optional)
         - from_timestamp: int - (optional)
@@ -112,120 +158,142 @@
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.POSTS_V1}/group_calls",
         params=params,
         data_type=PostsResponse,
+        access_token=access_token,
     )
 
 
-def invite_to_call_bulk(self, call_id: int, group_id: int = None):
+def invite_to_call_bulk(
+    self, call_id: int, group_id: int = None, access_token: str = None
+):
     """
 
     Parameters
     ----------
         - call_id: int - (required)
         - group_id: int - (optional)
 
     """
     params = {}
     if group_id:
         params["group_id"] = group_id
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite", params=params
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite",
+        params=params,
+        access_token=access_token,
     )
     self.logger.info("Invited your online followings to the call.")
     return response
 
 
-def invite_users_to_call(self, call_id: int, user_ids: List[int]):
+def invite_users_to_call(
+    self, call_id: int, user_ids: List[int], access_token: str = None
+):
     """
 
     Parameters
     ----------
         - call_id: int - (required)
         - user_ids: List[int] - (required)
 
     """
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/invite",
         payload={"call_id": call_id, "user_ids[]": user_ids},
+        access_token=access_token,
     )
     self.logger.info("Invited users to call.")
     return response
 
 
-def invite_users_to_chat_call(self, chat_room_id: int, room_id: int, room_url: str):
+def invite_users_to_chat_call(
+    self, chat_room_id: int, room_id: int, room_url: str, access_token: str = None
+):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V2}/invite",
         payload={
             "chat_room_id": chat_room_id,
             "room_id": room_id,
             "room_url": room_url,
         },
+        access_token=access_token,
     )
     self.logger.info("Invited users to chat call.")
     return response
 
 
-def kick_and_ban_from_call(self, call_id: int, user_id: int):
+def kick_and_ban_from_call(self, call_id: int, user_id: int, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/kick",
         payload={"user_id": user_id},
+        access_token=access_token,
     )
     self.logger.info("User has been banned from the call.")
     return response
 
 
 def set_call(
     self,
     call_id: int,
     joinable_by: str,
     game_title: str = None,
     category_id: str = None,
+    access_token: str = None,
 ):
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.CALLS_V1}/{call_id}",
         payload={
             "joinable_by": joinable_by,
             "game_title": game_title,
             "category_id": category_id,
         },
+        access_token=access_token,
     )
     self.logger.info("Started a call")
     return response
 
 
-def set_user_role(self, call_id: int, user_id: int, role: str):
+def set_user_role(
+    self, call_id: int, user_id: int, role: str, access_token: str = None
+):
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/{user_id}",
         payload={"role": role},
+        access_token=access_token,
     )
     self.logger.info(f"User '{user_id}' has been given a role.")
     return response
 
 
-def start_call(self, conference_id: int, call_sid: str = None) -> ConferenceCall:
+def start_call(
+    self, conference_id: int, call_sid: str = None, access_token: str = None
+) -> ConferenceCall:
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V1}/start_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid},
         data_type=ConferenceCallResponse,
+        access_token=access_token,
     ).conference_call
     self.logger.info("Joined the call.")
     return response
 
 
-def stop_call(self, conference_id: int, call_sid: str = None):
+def stop_call(self, conference_id: int, call_sid: str = None, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V1}/leave_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid},
+        access_token=access_token,
     )
     self.logger.info("Left the call.")
     return response
```

### Comparing `yaylib-0.1.5/yaylib/api/cassandra.py` & `yaylib-1.0.0/yaylib/api/cassandra.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,80 @@
-from ..config import *
-from ..errors import *
-from ..models import *
-from ..responses import *
-from ..utils import *
+"""
+MIT License
 
+Copyright (c) 2023-present Qvco, Konn
 
-def get_user_activities(self, **params) -> ActivitiesResponse:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from ..config import Configs
+from ..responses import ActivitiesResponse
+
+
+def get_user_activities(self, access_token: str = None, **params) -> ActivitiesResponse:
     """
 
     Parameters
     ----------
         - important: bool - (required)
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/user_activities",
         params=params,
         data_type=ActivitiesResponse,
+        access_token=access_token,
     )
 
 
-def get_user_merged_activities(self, **params) -> ActivitiesResponse:
+def get_user_merged_activities(
+    self, access_token: str = None, **params
+) -> ActivitiesResponse:
     """
     Parameters
     ----------
 
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/v2/user_activities",
         params=params,
         data_type=ActivitiesResponse,
+        access_token=access_token,
     )
 
 
-def received_notification(self, pid: str, type: str, opened_at: int = None):
+def received_notification(
+    self, pid: str, type: str, opened_at: int = None, access_token: str = None
+):
     # TODO: opened_atはnullalbeか確認する
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "POST",
-        endpoint=f"{self.host}/api/received_push_notifications",
+        endpoint=f"{Configs.YAY_API_URL}/api/received_push_notifications",
         payload={"pid": pid, "type": type, "opened_at": opened_at},
+        access_token=access_token,
     )
```

### Comparing `yaylib-0.1.5/yaylib/api/login.py` & `yaylib-1.0.0/yaylib/api/login.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,265 +1,249 @@
-from datetime import datetime
-from typing import Dict, List
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
 
-import os
-import json
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
 
+from datetime import datetime
 from cryptography.fernet import Fernet
 
-from ..config import *
-from ..errors import *
-from ..models import *
-from ..responses import *
-from ..utils import *
+from ..config import Configs, Endpoints
+from ..errors import AuthenticationError, ForbiddenError
+from ..responses import LoginUserResponse, LoginUpdateResponse, TokenResponse
+from ..utils import (
+    Colors,
+    console_print,
+    load_credentials,
+    save_credentials,
+    decrypt,
+    signed_info_calculating,
+)
 
 
 def change_email(
-    self, email: str, password: str, email_grant_token: str = None
+    self,
+    email: str,
+    password: str,
+    email_grant_token: str = None,
+    access_token: str = None,
 ) -> LoginUpdateResponse:
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.USERS_V1}/change_email",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "email_grant_token": email_grant_token,
         },
         data_type=LoginUpdateResponse,
+        access_token=access_token,
     )
     self.logger.info(self, fname="Your email has been changed.")
     return response
 
 
 def change_password(
-    self, current_password: str, new_password: str
+    self, current_password: str, new_password: str, access_token: str = None
 ) -> LoginUpdateResponse:
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.USERS_V1}/change_email",
         payload={
             "api_key": self.api_key,
             "current_password": current_password,
             "password": new_password,
         },
         data_type=LoginUpdateResponse,
+        access_token=access_token,
     )
     self.logger.info(self, fname="Your password has been changed..")
     return response
 
 
 def get_token(
     self,
     grant_type: str,
     refresh_token: str = None,
     email: str = None,
     password: str = None,
+    access_token: str = None,
 ) -> TokenResponse:
     return self._make_request(
         "POST",
-        endpoint=f"{self.host}/api/v1/oauth/token",
+        endpoint=f"{Configs.YAY_API_URL}/api/v1/oauth/token",
         payload={
             "grant_type": grant_type,
             "email": email,
             "password": password,
             "refresh_token": refresh_token,
         },
         data_type=TokenResponse,
+        access_token=access_token,
     )
 
 
 def is_valid_token(self, access_token: str):
     headers = self.session.headers
     headers.setdefault("Authorization", f"Bearer {access_token}")
     try:
         self.get_web_socket_token(headers)
         return True
     except AuthenticationError:
         return False
 
 
-def save_credentials(self, fernet, access_token, refresh_token, user_id, email=None):
-    credentials = load_credentials(self)
-    updated_credentials = {
-        "access_token": access_token,
-        "refresh_token": refresh_token,
-        "user_id": user_id,
-        "email": email,
-    }
-    if email is None:
-        updated_credentials["email"] = credentials.get("email")
-
-    updated_credentials = encrypt(self, fernet, updated_credentials)
-
-    with open(self.base_path + "credentials.json", "w") as f:
-        json.dump(updated_credentials, f)
-
-
-def load_credentials(self, check_email: str = None):
-    if not os.path.exists(self.base_path + "credentials.json"):
-        return None
-
-    with open(self.base_path + "credentials.json", "r") as f:
-        credentials = json.load(f)
-
-    result = all(
-        key in credentials
-        for key in ("access_token", "refresh_token", "user_id", "email")
-    )
-    credentials = None if result is False else credentials
-
-    if check_email is not None:
-        credentials = None if check_email != credentials["email"] else credentials
-
-    return credentials
-
-
-def encrypt(self, fernet, credentials: dict):
-    credentials.update(
-        {
-            "access_token": fernet.encrypt(
-                credentials.get("access_token").encode()
-            ).decode(),
-            "refresh_token": fernet.encrypt(
-                credentials.get("refresh_token").encode()
-            ).decode(),
-        }
-    )
-    return credentials
-
-
-def decrypt(self, fernet, credentials: dict):
-    credentials.update(
-        {
-            "access_token": fernet.decrypt(credentials.get("access_token")).decode(),
-            "refresh_token": fernet.decrypt(credentials.get("refresh_token")).decode(),
-        }
-    )
-    return credentials
-
-
 def login_with_email(
     self, email: str, password: str, secret_key: str = None
 ) -> LoginUserResponse:
-    credentials = load_credentials(self, email)
-    if credentials is not None:
-        if secret_key is not None:
+    if self.save_session:
+        credentials = load_credentials(base_path=self.base_path, check_email=email)
+        if credentials is not None and secret_key is not None:
             self.secret_key = secret_key
-            fernet = Fernet(secret_key)
-            credentials = decrypt(self, fernet, credentials)
+            self.fernet = Fernet(secret_key)
+            credentials = decrypt(fernet=self.fernet, credentials=credentials)
             self.session.headers.setdefault(
                 "Authorization", f"Bearer {credentials['access_token']}"
             )
             self.logger.info(f"Successfully logged in as '{credentials['user_id']}'")
             return credentials
-        else:
-            message = f"{colors.WARNING}Credential file found. The 'secret_key' must be provided to decrypt the credentials.{colors.RESET}"
+        elif credentials is not None:
+            message = f"{Colors.WARNING}Credential file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
             console_print(message)
 
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/login_with_email",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "uuid": self.uuid,
         },
         data_type=LoginUserResponse,
     )
 
-    message = "Invalid email or password."
     if response.access_token is None:
-        raise ForbiddenError(message)
+        raise ForbiddenError("Invalid email or password.")
 
     self.session.headers.setdefault("Authorization", f"Bearer {response.access_token}")
     self.logger.info(f"Successfully logged in as '{response.user_id}'")
 
-    secret_key = Fernet.generate_key()
-    self.secret_key = secret_key
-    fernet = Fernet(secret_key)
-
-    console_print(
-        f"Your 'secret_key' for {colors.BOLD + email + colors.RESET} is: {colors.OKGREEN + secret_key.decode() + colors.RESET}",
-        "Please copy and securely store this key in a safe location.",
-        "For more information, visit: https://github.com/qvco/yaylib/blob/main/docs/API-Reference/login/login.md",
-    )
+    if self.save_session:
+        secret_key = Fernet.generate_key()
+        self.secret_key = secret_key
+        self.fernet = Fernet(secret_key)
+
+        console_print(
+            f"Your 'secret_key' for {Colors.BOLD + email + Colors.RESET} is: {Colors.OKGREEN + secret_key.decode() + Colors.RESET}",
+            "Please copy and securely store this key in a safe location.",
+            "For more information, visit: https://github.com/qvco/yaylib/blob/master/docs/API-Reference/login/login.md",
+        )
+
+        save_credentials(
+            base_path=self.base_path,
+            fernet=self.fernet,
+            access_token=response.access_token,
+            refresh_token=response.refresh_token,
+            user_id=response.user_id,
+            email=email,
+        )
 
-    save_credentials(
-        self,
-        fernet=fernet,
-        access_token=response.access_token,
-        refresh_token=response.refresh_token,
-        user_id=response.user_id,
-        email=email,
-    )
     return response
 
 
-def logout(self):
+def logout(self, access_token: str = None):
     try:
-        self._check_authorization()
+        self._check_authorization(access_token)
         response = self._make_request(
-            "POST", endpoint=f"{Endpoints.USERS_V1}/logout", payload={"uuid": self.uuid}
+            "POST",
+            endpoint=f"{Endpoints.USERS_V1}/logout",
+            payload={"uuid": self.uuid},
+            access_token=access_token,
         )
         self.session.headers.pop("Authorization", None)
         self.logger.info("User has logged out.")
         return response
 
     except:
         self.logger.error("User is not logged in.")
         return None
 
 
-def resend_confirm_email(self):
+def resend_confirm_email(self, access_token: str = None):
     return self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/resend_confirm_email"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/resend_confirm_email",
+        access_token=access_token,
     )
 
 
-def restore_user(self, user_id: int) -> LoginUserResponse:
+def restore_user(self, user_id: int, access_token: str = None) -> LoginUserResponse:
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/restore",
         payload={
             "user_id": user_id,
             "api_key": self.api_key,
             "uuid": self.uuid,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
         },
+        access_token=access_token,
     )
     self.logger.info("User has been restored.")
     return response
 
 
-def revoke_tokens(self):
+def revoke_tokens(self, access_token: str = None):
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.USERS_V1}/device_tokens"
+        "DELETE",
+        endpoint=f"{Endpoints.USERS_V1}/device_tokens",
+        access_token=access_token,
     )
     self.logger.info("Token has been revoked.")
     return response
 
 
 def save_account_with_email(
     self,
     email: str,
     password: str = None,
     current_password: str = None,
     email_grant_token: str = None,
+    access_token: str = None,
 ) -> LoginUpdateResponse:
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/login_update",
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "current_password": current_password,
             "email_grant_token": email_grant_token,
         },
         data_type=LoginUpdateResponse,
+        access_token=access_token,
     )
     self.logger.info("Account has been save with email.")
     return response
```

### Comparing `yaylib-0.1.5/yaylib/api/misc.py` & `yaylib-1.0.0/yaylib/api/review.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,169 +1,141 @@
-import os
-import httpx
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
 
-from PIL import Image
 from datetime import datetime
-from typing import Dict, List
+from typing import List
 
-from ..config import *
-from ..errors import *
-from ..models import *
-from ..responses import *
-from ..utils import *
+from ..config import Endpoints
+from ..responses import ReviewsResponse
+from ..utils import signed_info_calculating
 
 
-def accept_policy_agreement(self, type: str):
+def create_review(self, user_id: int, comment: str, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/policy_agreements/{type}"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/reviews/{user_id}",
+        payload={"comment": comment},
+        access_token=access_token,
     )
-    self.logger.info("Accepted to policy agreement.")
+    self.logger.info(f"Review has been sent to {user_id}.")
     return response
 
 
-def generate_sns_thumbnail(self, **params):
-    """
-
-    Parameters:
-    ----------
-
-        - resource_type: str - (Required)
-        - resource_id: int - (Required)
-
-    """
+def create_reviews(self, user_ids: List[int], comment: str, access_token: str = None):
+    self._check_authorization(access_token)
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "GET", endpoint=f"{Endpoints.SNS_THUMBNAIL_V1}/generate", params=params
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/reviews",
+        payload={
+            "user_ids": user_ids,
+            "comment": comment,
+            "uuid": self.uuid,
+            "api_key": self.api_key,
+            "timestamp": timestamp,
+            "signed_info": signed_info_calculating(
+                self.uuid, timestamp, shared_key=True
+            ),
+        },
+        access_token=access_token,
     )
-    self.logger.info("SNS thumbnail generated.")
+    self.logger.info("Reviews have been sent to multiple users.")
     return response
 
 
-def get_email_grant_token(self, code: int, email: str) -> EmailGrantTokenResponse:
-    return self._make_request(
-        "POST",
-        endpoint=f"{Endpoints.GET_EMAIL_GRANT_TOKEN}",
-        payload={"code": code, "email": email},
-        data_type=EmailGrantTokenResponse,
-    ).email_grant_token
-
+def delete_reviews(self, review_ids: List[int], access_token: str = None):
+    self._check_authorization(access_token)
+    response = self._make_request(
+        "DELETE",
+        endpoint=f"{Endpoints.USERS_V1}/reviews",
+        params={"review_ids[]": review_ids},
+        access_token=access_token,
+    )
+    self.logger.info("Reviews have been deleted.")
+    return response
 
-def get_email_verification_presigned_url(
-    self, email: str, locale: str, intent: str = None
-) -> str:
-    return self._make_request(
-        "POST",
-        endpoint=f"{Endpoints.EMAIL_VERIFICATION_URL_V1}",
-        payload={
-            "device_uuid": self.device_uuid,
-            "email": email,
-            "locale": locale,
-            "intent": intent,
-        },
-        data_type=EmailVerificationPresignedUrlResponse,
-    ).url
 
+def get_my_reviews(self, access_token: str = None, **params) -> ReviewsResponse:
+    """
 
-def get_file_upload_presigned_urls(self, file_names: List[str]) -> List[PresignedUrl]:
-    return self._make_request(
-        "GET",
-        endpoint=f"{Endpoints.BUCKETS_V1}/presigned_urls",
-        params={"file_names[]": file_names},
-        data_type=PresignedUrlsResponse,
-    ).presigned_urls
+    Parameters
+    ----------
 
+        - from_id: int (optional)
+        - number: int = (optional)
 
-def get_id_checker_presigned_url(self, model: str, action: str, **params) -> str:
-    # TODO: @QueryMap @NotNull Map<String, String> map
-    """
-    Meow..
     """
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
-        endpoint=f"{Endpoints.ID_CHECK_V1}/{model}/{action}",
+        endpoint=f"{Endpoints.USERS_V1}/reviews/mine",
         params=params,
-        data_type=IdCheckerPresignedUrlResponse,
-    ).presigned_url
+        data_type=ReviewsResponse,
+        access_token=access_token,
+    )
 
 
-def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
-    return self._make_request(
-        "GET",
-        endpoint=f"{Endpoints.USERS_V1}/presigned_url",
-        params={"video_file_name": video_file_name},
-        data_type=PresignedUrlResponse,
-    ).presigned_url
+def get_reviews(
+    self, user_id: int, access_token: str = None, **params
+) -> ReviewsResponse:
+    """
 
+    Parameters
+    ----------
 
-def get_web_socket_token(self, headers: dict = None) -> str:
-    self._check_authorization()
+        - user_id: int (required)
+        - from_id: int = (optional)
+        - number: int = (optional)
+
+    """
     return self._make_request(
         "GET",
-        endpoint=f"{Endpoints.USERS_V1}/ws_token",
-        data_type=WebSocketTokenResponse,
-        headers=headers,
-    ).token
+        endpoint=f"{Endpoints.USERS_V1}/reviews/{user_id}",
+        params=params,
+        data_type=ReviewsResponse,
+        access_token=access_token,
+    )
 
 
-def verify_device(
-    self, app_version: str, device_uuid: str, platform: str, verification_string: str
-) -> VerifyDeviceResponse:
-    # TODO: check platform, verification_string
+def pin_review(self, review_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
         "POST",
-        endpoint=f"{Endpoints.GENUINE_DEVICES_V1}/verify",
-        payload={
-            "app_version": app_version,
-            "device_uuid": device_uuid,
-            "platform": platform,
-            "verification_string": verification_string,
-        },
-        data_type=VerifyDeviceResponse,
+        endpoint=f"{Endpoints.PINNED_V1}/reviews",
+        payload={"id": review_id},
+        access_token=access_token,
     )
-    self.logger.info("Device has been verified.")
+    self.logger.info("Pinned the review.")
     return response
 
 
-def upload_image(self, image_type: str, image_path: str) -> str:
-    """
-
-    画像をアップロードしてattachment_filenameを返します。
-
-    Parameteres
-    -----------
-        - image_type: str - (required): "post", "user_avatar" のどちらか
-        - image_path: str - (required): "画像のパス
-
-    """
-    valid_types = ["post", "user_avatar"]
-    if image_type not in valid_types:
-        message = f"Invalid post type. Must be one of {valid_types}"
-        raise ValueError(message)
-
-    date = datetime.now()
-    timestamp = int(date.timestamp() * 1000)
-    filename, ext = os.path.splitext(image_path)
-
-    with Image.open(image_path) as image:
-        width, height = image.size
-
-    base_url = f"{image_type}/{date.year}/{date.month}/{date.day}"
-    mid_url = f"{filename}_{timestamp}_0_size_"
-    original_url = f"{base_url}/{mid_url}{width}x{height}{ext}"
-    thumb_url = f"{base_url}/thumb_{mid_url}{width}x{height}{ext}"
-
-    presigned_urls = get_file_upload_presigned_urls(self, [original_url, thumb_url])
-
-    with open(image_path, "rb") as f:
-        response = httpx.put(presigned_urls[0].url, data=f.read())
-        self._handle_response(response)
-
-    with open(image_path, "rb") as f:
-        response = httpx.put(presigned_urls[1].url, data=f.read())
-        self._handle_response(response)
-
-    self.logger.info(f"Image '{filename}{ext}' is uploaded")
-
-    return presigned_urls[0].filename
-
-
-def upload_video(self, video_path: str):
-    pass
+def unpin_review(self, review_id: int, access_token: str = None):
+    self._check_authorization(access_token)
+    response = self._make_request(
+        "DELETE",
+        endpoint=f"{Endpoints.PINNED_V1}/reviews{review_id}",
+        access_token=access_token,
+    )
+    self.logger.info("Unpinned the review.")
+    return response
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yaylib-0.1.5/yaylib/api/user.py` & `yaylib-1.0.0/yaylib/api/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,250 @@
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 from datetime import datetime
-from typing import Union, Dict, List
+from typing import Union, List
 
-from ..config import *
-from ..errors import *
-from ..models import *
-from ..responses import *
-from ..utils import *
+from ..config import Configs, Endpoints
+from ..models import Footprint, User, UserWrapper
+from ..responses import (
+    ActiveFollowingsResponse,
+    BlockedUserIdsResponse,
+    BlockedUsersResponse,
+    CreatePostResponse,
+    CreateUserResponse,
+    FollowRecommendationsResponse,
+    FollowRequestCountResponse,
+    FollowUsersResponse,
+    FootprintsResponse,
+    HiddenResponse,
+    RefreshCounterRequestsResponse,
+    SocialShareUsersResponse,
+    UserResponse,
+    UsersResponse,
+    RankingUsersResponse,
+    UserEmailResponse,
+    HimaUsersResponse,
+    UsersByTimestampResponse,
+    UserTimestampResponse,
+)
+from ..utils import signed_info_calculating, signed_version_calculating
 
 
-def delete_footprint(self, user_id: int, footprint_id: int):
-    self._check_authorization()
+def delete_footprint(self, user_id: int, footprint_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}"
+        "DELETE",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}",
+        access_token=access_token,
     )
     self.logger.info("Footprint has been deleted.")
     return response
 
 
-def destroy_user(self):
-    self._check_authorization()
+def destroy_user(self, access_token: str = None):
+    self._check_authorization(access_token)
     answer = input("Are you sure you want to delete your account? Y/N")
     if answer.lower() != "y":
         return
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/destroy",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
         },
+        access_token=access_token,
     )
     self.logger.info("User has been deleted.")
     return response
 
 
-def follow_user(self, user_id: int):
-    self._check_authorization()
+def follow_user(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/follow"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/follow",
+        access_token=access_token,
     )
-    self.logger.info("Followed the user '{user_id}'.")
+    self.logger.info(f"Followed the user '{user_id}'.")
     return response
 
 
-def follow_users(self, user_ids: List[int]):
-    self._check_authorization()
+def follow_users(self, user_ids: List[int], access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/follow", params={"user_ids[]": user_ids}
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/follow",
+        params={"user_ids[]": user_ids},
+        access_token=access_token,
     )
     self.logger.info("Followed multiple users.")
     return response
 
 
-def get_active_followings(self, **params) -> ActiveFollowingsResponse:
+def get_active_followings(
+    self, access_token: str = None, **params
+) -> ActiveFollowingsResponse:
     """
 
     Parameters:
     ----------
 
         - only_online: bool
         - from_loggedin_at: int = None
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/active_followings",
         params=params,
         data_type=ActiveFollowingsResponse,
+        access_token=access_token,
     )
 
 
-def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
+def get_follow_recommendations(
+    self, access_token: str = None, **params
+) -> FollowRecommendationsResponse:
     """
 
     Parameters:
     ----------
 
         - from_timestamp: int = None,
         - number: int = None,
         - sources: List[str] = None
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.FRIENDS_V1}",
         params=params,
         data_type=FollowRecommendationsResponse,
+        access_token=access_token,
     )
 
 
-def get_follow_request(self, from_timestamp: int = None) -> UsersByTimestampResponse:
+def get_follow_request(
+    self, from_timestamp: int = None, access_token: str = None
+) -> UsersByTimestampResponse:
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/follow_requests",
         params=params,
         data_type=UsersByTimestampResponse,
+        access_token=access_token,
     )
 
 
-def get_follow_request_count(self) -> int:
-    self._check_authorization()
+def get_follow_request_count(self, access_token: str = None) -> int:
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/follow_requests_count",
         data_type=FollowRequestCountResponse,
+        access_token=access_token,
     ).users_count
 
 
-def get_following_users_born(self, birthdate: int = None) -> UsersResponse:
+def get_following_users_born(
+    self, birthdate: int = None, access_token: str = None
+) -> UsersResponse:
     params = {}
     if birthdate:
         params["birthdate"] = birthdate
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/following_born_today",
         params=params,
         data_type=UsersResponse,
+        access_token=access_token,
     )
 
 
-def get_footprints(self, **params) -> List[Footprint]:
+def get_footprints(self, access_token: str = None, **params) -> List[Footprint]:
     """
 
     Parameters:
     ----------
 
         - from_id: int = None
         - number: int = None
         - mode: str = None
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/footprints",
         params=params,
         data_type=FootprintsResponse,
+        access_token=access_token,
     ).footprints
 
 
-def get_fresh_user(self, user_id: int) -> UserResponse:
-    self._check_authorization()
+def get_fresh_user(self, user_id: int, access_token: str = None) -> UserResponse:
+    self._check_authorization(access_token)
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}", data_type=UserResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}",
+        data_type=UserResponse,
+        access_token=access_token,
     )
 
 
-def get_hima_users(self, **params) -> List[UserWrapper]:
+def get_hima_users(self, access_token: str = None, **params) -> List[UserWrapper]:
     """
 
     Parameters:
     ----------
 
         - from_hima_id: int = None
         - number: int = None
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/hima_users",
         params=params,
         data_type=HimaUsersResponse,
+        access_token=access_token,
     ).hima_users
 
 
 def get_user_ranking(self, mode: str) -> RankingUsersResponse:
     """
 
     ユーザーのランキングを取得します
@@ -204,67 +273,80 @@
         "GET",
         endpoint=f"{Endpoints.WEB_V1}/users/ranking",
         params={"mode": mode},
         data_type=RankingUsersResponse,
     )
 
 
-def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
-    self._check_authorization()
+def get_refresh_counter_requests(
+    self, access_token: str = None
+) -> RefreshCounterRequestsResponse:
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/reset_counters",
         data_type=RefreshCounterRequestsResponse,
+        access_token=access_token,
     )
 
 
-def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
+def get_social_shared_users(
+    self, access_token: str = None, **params
+) -> SocialShareUsersResponse:
     """
 
     Parameters:
     ----------
 
         - sns_name: str - (Required)
         - number: int - (Optional)
         - from_id: int - (Optional)
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/social_shared_users",
         params=params,
         data_type=SocialShareUsersResponse,
+        access_token=access_token,
     )
 
 
-def get_timestamp(self) -> UserTimestampResponse:
+def get_timestamp(self, access_token: str = None) -> UserTimestampResponse:
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/timestamp",
         data_type=UserTimestampResponse,
+        access_token=access_token,
     )
 
 
-def get_user(self, user_id: int) -> User:
+def get_user(self, user_id: int, access_token: str = None) -> User:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/{user_id}", data_type=UserResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}",
+        data_type=UserResponse,
+        access_token=access_token,
     ).user
 
 
-def get_user_email(self, user_id: int) -> str:
-    self._check_authorization()
+def get_user_email(self, user_id: int, access_token: str = None) -> str:
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}",
         data_type=UserEmailResponse,
+        access_token=access_token,
     ).email
 
 
-def get_user_followers(self, user_id: int, **params) -> FollowUsersResponse:
+def get_user_followers(
+    self, user_id: int, access_token: str = None, **params
+) -> FollowUsersResponse:
     """
 
     Parameters:
     ----------
 
         - user_id: int - (required)
         - from_follow_id: int - (optional)
@@ -273,151 +355,223 @@
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/{user_id}/followers",
         params=params,
         data_type=FollowUsersResponse,
+        access_token=access_token,
     )
 
 
-def get_user_followings(self, user_id: int, **params) -> FollowUsersResponse:
+def get_user_followings(
+    self, user_id: int, access_token: str = None, **params
+) -> FollowUsersResponse:
     # @Body @Nullable SearchUsersRequest searchUsersRequest
     """
 
     Parameters:
     ----------
 
         - user_id: int
         - from_follow_id: int = None
         - from_timestamp: int = None
         - order_by: str = None
         - number: int - (optional)
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/{user_id}/list_followings",
         params=params,
         data_type=FollowUsersResponse,
+        access_token=access_token,
     )
 
 
-def get_user_from_qr(self, qr: str) -> UserResponse:
+def get_user_from_qr(self, qr: str, access_token: str = None) -> UserResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/qr_codes/{qr}", data_type=UserResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/qr_codes/{qr}",
+        data_type=UserResponse,
+        access_token=access_token,
     )
 
 
-def get_user_without_leaving_footprint(self, user_id: int) -> UserResponse:
+def get_user_without_leaving_footprint(
+    self, user_id: int, access_token: str = None
+) -> UserResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/info/{user_id}", data_type=UserResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/info/{user_id}",
+        data_type=UserResponse,
+        access_token=access_token,
     )
 
 
-def get_users(self, user_ids: List[int]) -> UsersResponse:
+def get_users(self, user_ids: List[int], access_token: str = None) -> UsersResponse:
     headers = self.session.headers
-    headers["X-Jwt"] = self.get_web_socket_token()
+    headers["X-Jwt"] = self.get_web_socket_token(access_token=access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/list_id",
         params={"user_ids[]": user_ids},
         data_type=UsersResponse,
         headers=headers,
+        access_token=access_token,
     )
 
 
-def reduce_kenta_penalty(self, user_id: int):
-    self._check_authorization()
+def reduce_kenta_penalty(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
-        endpoint=f"{self.host}api/v3/users/{user_id}/reduce_penalty",
+        endpoint=f"{Configs.YAY_API_URL}api/v3/users/{user_id}/reduce_penalty",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "signed_version": signed_version_calculating(),
         },
         data_type=CreatePostResponse,
+        access_token=access_token,
     )
     self.logger.info("Penalty has been reduced.")
     return response
 
 
-def refresh_counter(self, counter: str):
+def refresh_counter(self, counter: str, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/reset_counters",
         payload={"counter": counter},
+        access_token=access_token,
     )
     self.logger.info("Requested counter refresh.")
     return response
 
 
-def remove_user_avatar(self):
+def register_user(
+    self,
+    email: str,
+    email_grant_token: str,
+    password: str,
+    nickname: str,
+    birth_date: str,
+    gender: int = -1,
+    country_code: str = "JP",
+    biography: str = None,
+    prefecture: str = None,
+    profile_icon_filename: str = None,
+    cover_image_filename: str = None,
+    # @Nullable @Part("sns_info") SignUpSnsInfoRequest signUpSnsInfoRequest,
+    en: int = None,
+    vn: int = None,
+) -> CreateUserResponse:
+    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/remove_profile_photo"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V3}/register",
+        payload={
+            "app_version": self.api_version,
+            "timestamp": timestamp,
+            "api_key": self.api_key,
+            "signed_version": signed_version_calculating(),
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "uuid": self.uuid,
+            "nickname": nickname,
+            "birth_date": birth_date,
+            "gender": gender,
+            "country_code": country_code,
+            "biography": biography,
+            "prefecture": prefecture,
+            "profile_icon_filename": profile_icon_filename,
+            "cover_image_filename": cover_image_filename,
+            "email": email,
+            "password": password,
+            "email_grant_token": email_grant_token,
+            "en": en,
+            "vn": vn,
+        },
+        data_type=CreateUserResponse,
+    )
+    self.logger.info(f"A new user has been registered. (USER ID: {response.id})")
+    return response
+
+
+def remove_user_avatar(self, access_token: str = None):
+    response = self._make_request(
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/remove_profile_photo",
+        access_token=access_token,
     )
     self.logger.info("Profile image has been removed.")
     return response
 
 
-def remove_user_cover(self):
+def remove_user_cover(self, access_token: str = None):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/remove_cover_image"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/remove_cover_image",
+        access_token=access_token,
     )
     self.logger.info("Profile cover image has been removed.")
     return response
 
 
 def report_user(
     self,
     user_id: int,
     category_id: int,
     reason: str = None,
     screenshot_filename: str = None,
     screenshot_2_filename: str = None,
     screenshot_3_filename: str = None,
     screenshot_4_filename: str = None,
+    access_token: str = None,
 ):
-    self._check_authorization()
+    self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/{user_id}/report",
         payload={
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         },
+        access_token=access_token,
     )
     self.logger.info(f"Reported the user '{user_id}'")
     return response
 
 
-def reset_password(self, email: str, email_grant_token: str, password: str):
+def reset_password(
+    self, email: str, email_grant_token: str, password: str, access_token: str = None
+):
     response = self._make_request(
         "PUT",
         endpoint=f"{Endpoints.USERS_V1}/reset_password",
         payload={
             "email": email,
             "email_grant_token": email_grant_token,
             "password": password,
         },
+        access_token=access_token,
     )
     self.logger.info("Reset the password.")
     return response
 
 
-def search_lobi_users(self, **params) -> UsersResponse:
+def search_lobi_users(self, access_token: str = None, **params) -> UsersResponse:
     """
 
     Parameters:
     ----------
 
         - nickname: str = None
         - number: int = None
@@ -425,18 +579,19 @@
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.LOBI_FRIENDS_V1}",
         params=params,
         data_type=UsersResponse,
+        access_token=access_token,
     )
 
 
-def search_users(self, **params) -> UsersResponse:
+def search_users(self, access_token: str = None, **params) -> UsersResponse:
     """
 
     Parameters:
     ----------
 
         - gender: int = None
         - nickname: str = None
@@ -451,88 +606,97 @@
 
     """
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/search",
         params=params,
         data_type=UsersResponse,
+        access_token=access_token,
     )
 
 
-def set_follow_permission_enabled(self, nickname: str, is_private: bool = None):
+def set_follow_permission_enabled(
+    self, nickname: str, is_private: bool = None, access_token: str = None
+):
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/edit",
         payload={
             "nickname": nickname,
             "is_private": is_private,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "signed_version": signed_version_calculating(),
         },
+        access_token=access_token,
     )
     self.logger.info("Follow permission has been enabled.")
     return response
 
 
-def set_setting_follow_recommendation_enabled(self, on: bool):
+def set_setting_follow_recommendation_enabled(self, on: bool, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/visible_on_sns_friend_recommendation_setting",
         params={"on": on},
+        access_token=access_token,
     )
     self.logger.info("Follow recommendation has been enabled.")
     return response
 
 
-def take_action_follow_request(self, target_id: int, action: str):
+def take_action_follow_request(
+    self, target_id: int, action: str, access_token: str = None
+):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/{target_id}/follow_request",
         payload={"action": action},
+        access_token=access_token,
     )
     self.logger.info("Took action follow request.")
     return response
 
 
-def turn_on_hima(self):
-    self._check_authorization()
+def turn_on_hima(self, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "GET",
-        endpoint=f"{Endpoints.USERS_V1}/hima",
+        "GET", endpoint=f"{Endpoints.USERS_V1}/hima", access_token=access_token
     )
     self.logger.info("Turned on 'hima now'.")
     return response
 
 
-def unfollow_user(self, user_id: int):
-    self._check_authorization()
+def unfollow_user(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V2}/{user_id}/unfollow",
+        access_token=access_token,
     )
     self.logger.info(f"Unfollowed the user '{user_id}'")
     return response
 
 
-def update_language(self, language: str):
+def update_language(self, language: str, access_token: str = None):
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/language",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "language": language,
         },
+        access_token=access_token,
     )
     self.logger.info("Language has been updated.")
     return response
 
 
 def update_user(
     self,
@@ -540,16 +704,17 @@
     biography: str = None,
     prefecture: str = None,
     gender: int = None,
     country_code: str = None,
     profile_icon_filename: str = None,
     cover_image_filename: str = None,
     username: str = None,
+    access_token: str = None,
 ):
-    self._check_authorization()
+    self._check_authorization(access_token)
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/edit",
         payload={
             "nickname": nickname,
             "biography": biography,
@@ -560,97 +725,112 @@
             "cover_image_filename": cover_image_filename,
             "username": username,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(self.device_uuid, timestamp),
         },
+        access_token=access_token,
     )
     self.logger.info("User profile has been updated.")
     return response
 
 
 # BlockApi
 
 
-def block_user(self, user_id: int):
-    self._check_authorization()
+def block_user(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/{user_id}/block",
+        access_token=access_token,
     )
     self.logger.info(f"Blocked the user '{user_id}'")
     return response
 
 
-def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
-    self._check_authorization()
+def get_blocked_user_ids(self, access_token: str = None) -> BlockedUserIdsResponse:
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V1}/block_ids",
         data_type=BlockedUserIdsResponse,
+        access_token=access_token,
     )
 
 
-def get_blocked_users(self, from_id: int = None) -> BlockedUsersResponse:
+def get_blocked_users(
+    self, from_id: int = None, access_token: str = None
+) -> BlockedUsersResponse:
     # @Body @NotNull SearchUsersRequest searchUsersRequest
-    self._check_authorization()
+    self._check_authorization(access_token)
     params = {}
     if from_id:
         params["from_id"] = from_id
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.USERS_V2}/blocked",
         params=params,
         data_type=BlockedUsersResponse,
+        access_token=access_token,
     )
 
 
-def unblock_user(self, user_id: int):
-    self._check_authorization()
+def unblock_user(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unblock"
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/unblock",
+        access_token=access_token,
     )
     self.logger.info(f"Unblocked the user '{user_id}'")
     return response
 
 
 # HiddenApi
 
 
-def get_hidden_users_list(self, **params: Union[str, int]) -> HiddenResponse:
+def get_hidden_users_list(
+    self, access_token: str = None, **params: Union[str, int]
+) -> HiddenResponse:
     """
 
     Parameters:
     ----------
 
         - from: str = None
         - number: int = None
 
     """
-    self._check_authorization()
+    self._check_authorization(access_token)
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.HIDDEN_V1}/users",
         params=params,
         data_type=HiddenResponse,
+        access_token=access_token,
     )
 
 
-def hide_user(self, user_id: int):
-    self._check_authorization()
+def hide_user(self, user_id: int, access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.HIDDEN_V1}/users", payload={"user_id": user_id}
+        "POST",
+        endpoint=f"{Endpoints.HIDDEN_V1}/users",
+        payload={"user_id": user_id},
+        access_token=access_token,
     )
     self.logger.info(f"User '{user_id}' is hidden")
     return response
 
 
-def unhide_users(self, user_ids: List[int]):
-    self._check_authorization()
+def unhide_users(self, user_ids: List[int], access_token: str = None):
+    self._check_authorization(access_token)
     response = self._make_request(
         "DELETE",
         endpoint=f"{Endpoints.HIDDEN_V1}/users",
         params={"user_ids[]": user_ids},
+        access_token=access_token,
     )
     self.logger.info("Unhid users")
     return response
```

### Comparing `yaylib-0.1.5/yaylib/client.py` & `yaylib-1.0.0/yaylib/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,327 @@
-from typing import Union, Dict, List
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import Dict, List, Union
 
 from .api import API
-from .api.call import *
-from .api.cassandra import *
-from .api.chat import *
-from .api.group import *
-from .api.login import *
-from .api.misc import *
-from .api.post import *
-from .api.review import *
-from .api.thread import *
-from .api.user import *
-
-from .config import *
-from .errors import (
-    YayError,
-    HTTPError,
-    BadRequestError,
-    AuthenticationError,
-    ForbiddenError,
-    NotFoundError,
-    RateLimitError,
-    YayServerError,
+from .api.call import (
+    bump_call,
+    get_bgms,
+    get_call,
+    get_call_invitable_users,
+    get_call_status,
+    get_games,
+    get_genres,
+    get_group_calls,
+    get_user_active_call,
+    invite_to_call_bulk,
+    invite_users_to_call,
+    invite_users_to_chat_call,
+    kick_and_ban_from_call,
+    set_call,
+    set_user_role,
+    start_call,
+    stop_call,
+)
+from .api.cassandra import (
+    get_user_activities,
+    get_user_merged_activities,
+    received_notification,
+)
+from .api.chat import (
+    accept_chat_request,
+    check_unread_status,
+    create_group_chat,
+    create_private_chat,
+    delete_background,
+    delete_message,
+    edit_chat_room,
+    get_chatable_users,
+    get_gifs_data,
+    get_hidden_chat_rooms,
+    get_main_chat_rooms,
+    get_messages,
+    get_request_chat_rooms,
+    get_chat_room,
+    get_sticker_packs,
+    get_total_chat_requests,
+    hide_chat,
+    invite_to_chat,
+    kick_users_from_chat,
+    pin_chat,
+    read_message,
+    refresh_chat_rooms,
+    remove_chat_rooms,
+    report_chat_room,
+    send_message,
+    unhide_chat,
+    unpin_chat,
+)
+from .api.group import (
+    accept_moderator_offer,
+    accept_ownership_offer,
+    accept_group_join_request,
+    add_related_groups,
+    ban_group_user,
+    check_unread_status,
+    create_group,
+    create_pin_group,
+    decline_moderator_offer,
+    decline_ownership_offer,
+    decline_group_join_request,
+    delete_pin_group,
+    get_banned_group_members,
+    get_group_categories,
+    get_create_group_quota,
+    get_group,
+    get_groups,
+    get_invitable_users,
+    get_joined_statuses,
+    get_group_member,
+    get_group_members,
+    get_my_groups,
+    get_relatable_groups,
+    get_related_groups,
+    get_user_groups,
+    invite_users_to_group,
+    join_group,
+    leave_group,
+    post_gruop_social_shared,
+    remove_group_cover,
+    remove_moderator,
+    remove_related_groups,
+    report_group,
+    send_moderator_offers,
+    send_ownership_offer,
+    set_group_title,
+    take_over_group_ownership,
+    unban_group_member,
+    update_group,
+    withdraw_moderator_offer,
+    withdraw_ownership_offer,
+)
+from .api.login import (
+    change_email,
+    change_password,
+    get_token,
+    is_valid_token,
+    login_with_email,
+    logout,
+    resend_confirm_email,
+    restore_user,
+    revoke_tokens,
+    save_account_with_email,
+)
+from .api.misc import (
+    accept_policy_agreement,
+    generate_sns_thumbnail,
+    send_verification_code,
+    get_email_grant_token,
+    get_email_verification_presigned_url,
+    get_file_upload_presigned_urls,
+    get_id_checker_presigned_url,
+    get_old_file_upload_presigned_url,
+    get_web_socket_token,
+    verify_device,
+    upload_image,
+    upload_video,
+)
+from .api.post import (
+    add_bookmark,
+    add_group_highlight_post,
+    create_call_post,
+    create_group_pin_post,
+    create_pin_post,
+    mention,
+    create_post,
+    create_repost,
+    create_share_post,
+    create_thread_post,
+    delete_all_post,
+    delete_group_pin_post,
+    delete_pin_post,
+    get_bookmark,
+    get_timeline_calls,
+    get_conversation,
+    get_conversation_root_posts,
+    get_following_call_timeline,
+    get_following_timeline,
+    get_group_highlight_posts,
+    get_group_timeline_by_keyword,
+    get_group_timeline,
+    get_timeline_by_hashtag,
+    get_my_posts,
+    get_post,
+    get_post_likers,
+    get_post_reposts,
+    get_posts,
+    get_recommended_post_tags,
+    get_recommended_posts,
+    get_timeline_by_keyword,
+    get_timeline,
+    get_url_metadata,
+    get_user_timeline,
+    like_posts,
+    remove_bookmark,
+    remove_group_highlight_post,
+    remove_posts,
+    report_post,
+    unlike_post,
+    update_post,
+    view_video,
+    vote_survey,
+)
+from .api.review import (
+    create_review,
+    create_reviews,
+    delete_reviews,
+    get_my_reviews,
+    get_reviews,
+    pin_review,
+    unpin_review,
+)
+from .api.thread import (
+    add_post_to_thread,
+    convert_post_to_thread,
+    create_thread,
+    get_group_thread_list,
+    get_thread_joined_statuses,
+    get_thread_posts,
+    join_thread,
+    leave_thread,
+    remove_thread,
+    update_thread,
+)
+from .api.user import (
+    delete_footprint,
+    destroy_user,
+    follow_user,
+    follow_users,
+    get_active_followings,
+    get_follow_recommendations,
+    get_follow_request,
+    get_follow_request_count,
+    get_following_users_born,
+    get_footprints,
+    get_fresh_user,
+    get_hima_users,
+    get_user_ranking,
+    get_refresh_counter_requests,
+    get_social_shared_users,
+    get_timestamp,
+    get_user,
+    get_user_email,
+    get_user_followers,
+    get_user_followings,
+    get_user_from_qr,
+    get_user_without_leaving_footprint,
+    get_users,
+    reduce_kenta_penalty,
+    refresh_counter,
+    register_user,
+    remove_user_avatar,
+    remove_user_cover,
+    report_user,
+    reset_password,
+    search_lobi_users,
+    search_users,
+    set_follow_permission_enabled,
+    set_setting_follow_recommendation_enabled,
+    take_action_follow_request,
+    turn_on_hima,
+    unfollow_user,
+    update_language,
+    update_user,
+    block_user,
+    get_blocked_user_ids,
+    get_blocked_users,
+    unblock_user,
+    get_hidden_users_list,
+    hide_user,
+    unhide_users,
+)
+from .models import (
+    Bgm,
+    ChatRoom,
+    ConferenceCall,
+    CreateGroupQuota,
+    Footprint,
+    GifImageCategory,
+    Message,
+    Post,
+    PresignedUrl,
+    SharedUrl,
+    StickerPack,
+    Survey,
+    ThreadInfo,
+    User,
+    UserWrapper,
+)
+from .responses import (
+    ActiveFollowingsResponse,
+    ActivitiesResponse,
+    BlockedUserIdsResponse,
+    BlockedUsersResponse,
+    BookmarkPostResponse,
+    CallStatusResponse,
+    ChatRoomsResponse,
+    CreateGroupResponse,
+    CreateChatRoomResponse,
+    FollowRecommendationsResponse,
+    FollowUsersResponse,
+    GamesResponse,
+    GenresResponse,
+    GroupCategoriesResponse,
+    GroupResponse,
+    GroupsRelatedResponse,
+    GroupsResponse,
+    GroupThreadListResponse,
+    GroupUserResponse,
+    GroupUsersResponse,
+    HiddenResponse,
+    LoginUserResponse,
+    LoginUpdateResponse,
+    MessageResponse,
+    PostsResponse,
+    PostLikersResponse,
+    PostTagsResponse,
+    LikePostsResponse,
+    RefreshCounterRequestsResponse,
+    ReviewsResponse,
+    SocialShareUsersResponse,
+    TokenResponse,
+    UnreadStatusResponse,
+    UserResponse,
+    UsersResponse,
+    RankingUsersResponse,
+    UsersByTimestampResponse,
+    UserTimestampResponse,
 )
-from .models import *
-from .utils import *
 
 
 class Client(API):
     """
 
     Yay!（イェイ）の API クライアント
 
@@ -57,258 +350,284 @@
 
     Copyright (c) 2023 Qvco, Konn
 
     """
 
     # -CALL
 
-    def get_user_active_call(self, user_id: int) -> Post:
+    def get_user_active_call(self, user_id: int, access_token: str = None) -> Post:
         """
 
         ユーザーが参加中の通話を取得します
 
         """
-        return get_user_active_call(self, user_id)
+        return get_user_active_call(self, user_id, access_token)
 
-    def get_bgms(self) -> List[Bgm]:
+    def get_bgms(self, access_token: str = None) -> List[Bgm]:
         """
 
         通話のBGMを取得します
 
         """
-        return get_bgms(self)
+        return get_bgms(self, access_token)
 
-    def get_call(self, call_id: int) -> ConferenceCall:
+    def get_call(self, call_id: int, access_token: str = None) -> ConferenceCall:
         """
 
         通話の詳細を取得します
 
         """
-        return get_call(self, call_id)
+        return get_call(self, call_id, access_token)
 
     def get_call_invitable_users(
-        self, call_id: int, from_timestamp: int = None
+        self, call_id: int, from_timestamp: int = None, access_token: str = None
     ) -> UsersByTimestampResponse:
         # @Nullable @Query("user[nickname]")
         """
 
         通話に招待可能なユーザーを取得します
 
         """
-        return get_call_invitable_users(self, call_id, from_timestamp)
+        return get_call_invitable_users(self, call_id, from_timestamp, access_token)
 
-    def get_call_status(self, opponent_id: int) -> CallStatusResponse:
+    def get_call_status(
+        self, opponent_id: int, access_token: str = None
+    ) -> CallStatusResponse:
         """
 
         通話の状態を取得します
 
         """
-        return get_call_status(self, opponent_id)
+        return get_call_status(self, opponent_id, access_token)
 
-    def get_games(self, **params) -> GamesResponse:
+    def get_games(self, access_token: str = None, **params) -> GamesResponse:
         """
 
         ゲームを取得します
 
         Parameters
         ----------
             - number: int - (optional)
             - ids: List[int] - (optional)
             - from_id: int - (optional)
 
         """
-        return get_games(self, **params)
+        return get_games(self, access_token, **params)
 
-    def get_genres(self, **params) -> GenresResponse:
+    def get_genres(self, access_token: str = None, **params) -> GenresResponse:
         """
 
         通話のジャンルを取得します
 
         Parameters
         ----------
             - number: int - (optional)
             - from: int - (optional)
 
         """
-        return get_genres(self, **params)
+        return get_genres(self, access_token, **params)
 
-    def get_group_calls(self, **params) -> PostsResponse:
+    def get_group_calls(self, access_token: str = None, **params) -> PostsResponse:
         """
 
         サークルの通話を取得します
 
         Parameters
         ----------
             - number: int - (optional)
             - group_category_id: int - (optional)
             - from_timestamp: int - (optional)
             - scope: str - (optional)
 
         """
-        return get_group_calls(self, **params)
+        return get_group_calls(self, access_token, **params)
 
     def invite_online_followings_to_call(
-        self, call_id: int, group_id: int = None
+        self, call_id: int, group_id: int = None, access_token: str = None
     ) -> dict:
         """
 
         オンラインの友達をまとめて通話に招待します
 
         Parameters
         ----------
             - call_id: int - (required)
             - group_id: int - (optional)
 
         """
-        return invite_to_call_bulk(self, call_id, group_id)
+        return invite_to_call_bulk(self, call_id, group_id, access_token)
 
-    def invite_users_to_call(self, call_id: int, user_ids: List[int]) -> dict:
+    def invite_users_to_call(
+        self, call_id: int, user_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         ユーザーを通話に招待します
 
         Parameters
         ----------
             - call_id: int - (required)
             - user_ids: List[int] - (required)
 
         """
-        return invite_users_to_call(self, call_id, user_ids)
+        return invite_users_to_call(self, call_id, user_ids, access_token)
 
     def invite_users_to_chat_call(
-        self, chat_room_id: int, room_id: int, room_url: str
+        self, chat_room_id: int, room_id: int, room_url: str, access_token: str = None
     ) -> dict:
         """
 
         チャット通話にユーザーを招待します
 
         Parameters
         ----------
 
             - chat_room_id: int - (required)
             - room_id: int - (required)
             - room_url: int - (required)
 
         """
-        return invite_users_to_chat_call(self, chat_room_id, room_id, room_url)
+        return invite_users_to_chat_call(
+            self, chat_room_id, room_id, room_url, access_token
+        )
 
-    def kick_user_from_call(self, call_id: int, user_id: int) -> dict:
+    def kick_user_from_call(
+        self, call_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         ユーザーを通話からキックします
 
         Parameters
         ----------
 
             - call_id: int - (required)
             - user_id: int - (required)
 
         """
-        return kick_and_ban_from_call(self, call_id, user_id)
+        return kick_and_ban_from_call(self, call_id, user_id, access_token)
 
     def set_call(
         self,
         call_id: int,
         joinable_by: str,
         game_title: str = None,
         category_id: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         通話を開始します
 
         """
-        return set_call(self, call_id, joinable_by, game_title, category_id)
+        return set_call(
+            self, call_id, joinable_by, game_title, category_id, access_token
+        )
 
-    def set_user_role(self, call_id: int, user_id: int, role: str) -> dict:
+    def set_user_role(
+        self, call_id: int, user_id: int, role: str, access_token: str = None
+    ) -> dict:
         """
 
         通話に参加中ののユーザーに役職を与えます
 
         """
-        return set_user_role(self, call_id, user_id, role)
+        return set_user_role(self, call_id, user_id, role, access_token)
 
-    def join_call(self, conference_id: int, call_sid: str = None) -> ConferenceCall:
+    def join_call(
+        self, conference_id: int, call_sid: str = None, access_token: str = None
+    ) -> ConferenceCall:
         """
 
         通話に参加します
 
         """
-        return start_call(self, conference_id, call_sid)
+        return start_call(self, conference_id, call_sid, access_token)
 
-    def leave_call(self, conference_id: int, call_sid: str = None) -> dict:
+    def leave_call(
+        self, conference_id: int, call_sid: str = None, access_token: str = None
+    ) -> dict:
         """
 
         通話から退出します
 
         """
-        return stop_call(self, conference_id, call_sid)
+        return stop_call(self, conference_id, call_sid, access_token)
 
     # -CASSANDRA
 
-    def get_activities(self, **params) -> ActivitiesResponse:
+    def get_activities(self, access_token: str = None, **params) -> ActivitiesResponse:
         """
 
         通知を取得します
 
         Parameters
         ----------
             - important: bool - (required)
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
-        return get_user_activities(self, **params)
+        return get_user_activities(self, access_token, **params)
 
-    def get_merged_activities(self, **params) -> ActivitiesResponse:
+    def get_merged_activities(
+        self, access_token: str = None, **params
+    ) -> ActivitiesResponse:
         """
 
         全種類の通知を取得します
 
         Parameters
         ----------
 
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
-        return get_user_merged_activities(self, **params)
+        return get_user_merged_activities(self, access_token, **params)
 
-    def received_notification(self, pid: str, type: str, opened_at: int = None) -> dict:
-        return received_notification(self, pid, type, opened_at)
+    def received_notification(
+        self, pid: str, type: str, opened_at: int = None, access_token: str = None
+    ) -> dict:
+        return received_notification(self, pid, type, opened_at, access_token)
 
     # -CHAT
 
-    def accept_chat_request(self, chat_room_ids: List[int]) -> dict:
+    def accept_chat_request(
+        self, chat_room_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         チャットリクエストを承認します
 
         Parameters
         ----------
 
             - chat_room_ids: List[int] - (required)
 
         """
-        return accept_chat_request(self, chat_room_ids)
+        return accept_chat_request(self, chat_room_ids, access_token)
 
-    def check_unread_status(self, from_time: int) -> UnreadStatusResponse:
+    def check_unread_status(
+        self, from_time: int, access_token: str = None
+    ) -> UnreadStatusResponse:
         """
 
         チャットの未読ステータスを確認します
 
         """
-        return check_unread_status(self, from_time)
+        return check_unread_status(self, from_time, access_token)
 
     def create_group_chat(
         self,
         name: str,
         with_user_ids: List[int],
         icon_filename: str = None,
         background_filename: str = None,
+        access_token: str = None,
     ) -> CreateChatRoomResponse:
         """
 
         グループチャットを作成します
 
         Parameters
         ----------
@@ -316,231 +635,262 @@
             - name: str - (required)
             - with_user_ids: List[int] - (required)
             - icon_filename: str - (optional)
             - background_filename: str - (optional)
 
         """
         return create_group_chat(
-            self, name, with_user_ids, icon_filename, background_filename
+            self, name, with_user_ids, icon_filename, background_filename, access_token
         )
 
     def create_private_chat(
-        self, with_user_id: int, matching_id: int = None, hima_chat: bool = False
+        self,
+        with_user_id: int,
+        matching_id: int = None,
+        hima_chat: bool = False,
+        access_token: str = None,
     ) -> CreateChatRoomResponse:
         """
 
         個人チャットを作成します
 
         Parameters
         ----------
 
             - with_user_id: int - (required)
             - matching_id: str - (optional)
             - hima_chat: bool - (optional)
 
         """
-        return create_private_chat(self, with_user_id, matching_id, hima_chat)
+        return create_private_chat(
+            self, with_user_id, matching_id, hima_chat, access_token
+        )
 
-    def delete_background(self, room_id: int) -> dict:
+    def delete_background(self, room_id: int, access_token: str = None) -> dict:
         """
 
         チャットの背景画像を削除します
 
         Parameters
         ----------
 
             - room_id: int - (required)
 
         """
-        return delete_background(self, room_id)
+        return delete_background(self, room_id, access_token)
 
-    def delete_message(self, room_id: int, message_id: int) -> dict:
+    def delete_message(
+        self, room_id: int, message_id: int, access_token: str = None
+    ) -> dict:
         """
 
         メッセージを削除します
 
         Parameters
         ----------
 
             - room_id: int - (required)
             - message_id: int - (required)
 
         """
-        return delete_message(self, room_id, message_id)
+        return delete_message(self, room_id, message_id, access_token)
 
     def edit_chat_room(
         self,
         chat_room_id: int,
         name: str,
         icon_filename: str = None,
         background_filename: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         チャットルームを編集します
 
         """
         return edit_chat_room(
-            self, chat_room_id, name, icon_filename, background_filename
+            self, chat_room_id, name, icon_filename, background_filename, access_token
         )
 
     def get_chatable_users(
         self,
         from_follow_id: int = None,
         from_timestamp: int = None,
         order_by: str = None,
+        access_token: str = None,
     ) -> FollowUsersResponse:
         """
 
         チャット可能なユーザーを取得します
 
         """
-        return get_chatable_users(from_follow_id, from_timestamp, order_by)
+        return get_chatable_users(
+            from_follow_id, from_timestamp, order_by, access_token
+        )
 
-    def get_gifs_data(self) -> List[GifImageCategory]:
+    def get_gifs_data(self, access_token: str = None) -> List[GifImageCategory]:
         """
 
         チャットルームのGIFデータを取得します
 
         """
-        return get_gifs_data(self)
+        return get_gifs_data(self, access_token)
 
-    def get_hidden_chat_rooms(self, **params) -> ChatRoomsResponse:
+    def get_hidden_chat_rooms(
+        self, access_token: str = None, **params
+    ) -> ChatRoomsResponse:
         """
 
         非表示のチャットルームを取得します
 
         Parameters
         ----------
 
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
-        return get_hidden_chat_rooms(self, **params)
+        return get_hidden_chat_rooms(self, access_token, **params)
 
-    def get_main_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
+    def get_main_chat_rooms(
+        self, from_timestamp: int = None, access_token: str = None
+    ) -> ChatRoomsResponse:
         """
 
         メインのチャットルームを取得します
 
         """
-        return get_main_chat_rooms(self, from_timestamp)
+        return get_main_chat_rooms(self, from_timestamp, access_token)
 
-    def get_messages(self, chat_room_id: int, **params) -> List[Message]:
+    def get_messages(
+        self, chat_room_id: int, access_token: str = None, **params
+    ) -> List[Message]:
         """
 
         メッセージを取得します
 
         Parameters
         ---------------
             - from_message_id: int - (optional)
             - to_message_id: int - (optional)
 
         """
-        return get_messages(self, chat_room_id, **params)
+        return get_messages(self, chat_room_id, access_token, **params)
 
-    def get_request_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
+    def get_request_chat_rooms(
+        self, from_timestamp: int = None, access_token: str = None
+    ) -> ChatRoomsResponse:
         """
 
         チャットリクエストを取得します
 
         """
-        return get_request_chat_rooms(self, from_timestamp)
+        return get_request_chat_rooms(self, from_timestamp, access_token)
 
-    def get_chat_room(self, chat_room_id: int) -> ChatRoom:
+    def get_chat_room(self, chat_room_id: int, access_token: str = None) -> ChatRoom:
         """
 
         チャットルームの詳細を取得します
 
         """
-        return get_chat_room(self, chat_room_id)
+        return get_chat_room(self, chat_room_id, access_token)
 
-    def get_sticker_packs(self) -> List[StickerPack]:
+    def get_sticker_packs(self, access_token: str = None) -> List[StickerPack]:
         """
 
         スタンプを取得します
 
         """
-        return get_sticker_packs(self)
+        return get_sticker_packs(self, access_token)
 
-    def get_chat_requests_count(self) -> int:
+    def get_chat_requests_count(self, access_token: str = None) -> int:
         """
 
         チャットリクエストの数を取得します
 
         """
-        return get_total_chat_requests(self)
+        return get_total_chat_requests(self, access_token)
 
-    def hide_chat(self, chat_room_id: int) -> dict:
+    def hide_chat(self, chat_room_id: int, access_token: str = None) -> dict:
         """
 
         チャットルームを非表示にします
 
         """
-        return hide_chat(self, chat_room_id)
+        return hide_chat(self, chat_room_id, access_token)
 
-    def invite_to_chat(self, chat_room_id: int, user_ids: List[int]) -> dict:
+    def invite_to_chat(
+        self, chat_room_id: int, user_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         チャットルームにユーザーを招待します
 
         """
-        return invite_to_chat(self, chat_room_id, user_ids)
+        return invite_to_chat(self, chat_room_id, user_ids, access_token)
 
-    def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]) -> dict:
+    def kick_users_from_chat(
+        self, chat_room_id: int, user_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         チャットルームからユーザーを追放します
 
         """
-        return kick_users_from_chat(self, chat_room_id, user_ids)
+        return kick_users_from_chat(self, chat_room_id, user_ids, access_token)
 
-    def pin_chat(self, room_id: int) -> dict:
+    def pin_chat(self, room_id: int, access_token: str = None) -> dict:
         """
 
         チャットルームをピン止めします
 
         """
-        return pin_chat(self, room_id)
+        return pin_chat(self, room_id, access_token)
 
-    def read_message(self, chat_room_id: int, message_id: int) -> dict:
+    def read_message(
+        self, chat_room_id: int, message_id: int, access_token: str = None
+    ) -> dict:
         """
 
         メッセージを既読にします
 
         """
-        return read_message(self, chat_room_id, message_id)
+        return read_message(self, chat_room_id, message_id, access_token)
 
-    def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
+    def refresh_chat_rooms(
+        self, from_time: int = None, access_token: str = None
+    ) -> ChatRoomsResponse:
         """
 
         チャットルームを更新します
 
         """
-        return refresh_chat_rooms(self, from_time)
+        return refresh_chat_rooms(self, from_time, access_token)
 
-    def remove_chat_rooms(self, chat_room_ids: List[int]) -> dict:
+    def remove_chat_rooms(
+        self, chat_room_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         チャットルームを削除します
 
         """
-        return remove_chat_rooms(self, chat_room_ids)
+        return remove_chat_rooms(self, chat_room_ids, access_token)
 
     def report_chat_room(
         self,
         chat_room_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         チャットルームを通報します
 
         """
         return report_chat_room(
@@ -549,27 +899,29 @@
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename,
+            access_token,
         )
 
     def send_message(
         self,
         chat_room_id: int,
         message_type: str,
         call_type: str = None,
         text: str = None,
         font_size: int = None,
         gif_image_id: int = None,
         attachment_file_name: str = None,
         sticker_pack_id: int = None,
         video_file_name: str = None,
+        access_token: str = None,
     ) -> MessageResponse:
         """
 
         チャットルームにメッセージを送信します
 
         """
         return send_message(
@@ -579,81 +931,90 @@
             call_type,
             text,
             font_size,
             gif_image_id,
             attachment_file_name,
             sticker_pack_id,
             video_file_name,
+            access_token,
         )
 
-    def unhide_chat(self, chat_room_ids: int) -> dict:
+    def unhide_chat(self, chat_room_ids: int, access_token: str = None) -> dict:
         """
 
         チャットの非表示を解除します
 
         """
-        return unhide_chat(self, chat_room_ids)
+        return unhide_chat(self, chat_room_ids, access_token)
 
-    def unpin_chat(self, chat_room_id: int) -> dict:
+    def unpin_chat(self, chat_room_id: int, access_token: str = None) -> dict:
         """
 
         チャットルームのピン止めを解除します
 
         """
-        return unpin_chat(self, chat_room_id)
+        return unpin_chat(self, chat_room_id, access_token)
 
     # -GROUP
 
-    def accept_moderator_offer(self, group_id: int) -> dict:
+    def accept_moderator_offer(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークル副管理人の権限オファーを引き受けます
 
         """
-        return accept_moderator_offer(self, group_id)
+        return accept_moderator_offer(self, group_id, access_token)
 
-    def accept_ownership_offer(self, group_id: int) -> dict:
+    def accept_ownership_offer(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークル管理人の権限オファーを引き受けます
 
         """
-        return accept_ownership_offer(self, group_id)
+        return accept_ownership_offer(self, group_id, access_token)
 
-    def accept_group_join_request(self, group_id: int, user_id: int) -> dict:
+    def accept_group_join_request(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル参加リクエストを承認します
 
         """
-        return accept_group_join_request(self, group_id, user_id)
+        return accept_group_join_request(self, group_id, user_id, access_token)
 
-    def add_related_groups(self, group_id: int, related_group_id: List[int]) -> dict:
+    def add_related_groups(
+        self, group_id: int, related_group_id: List[int], access_token: str = None
+    ) -> dict:
         """
 
         関連サークルを追加します
 
         """
-        return add_related_groups(self, group_id, related_group_id)
+        return add_related_groups(self, group_id, related_group_id, access_token)
 
-    def ban_group_user(self, group_id: int, user_id: int) -> dict:
+    def ban_group_user(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークルからユーザーを追放します
 
         """
-        return ban_group_user(self, group_id, user_id)
+        return ban_group_user(self, group_id, user_id, access_token)
 
-    def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
+    def check_unread_status(
+        self, from_time: int = None, access_token: str = None
+    ) -> UnreadStatusResponse:
         """
 
         サークルの未読ステータスを取得します
 
         """
-        return check_unread_status(self, from_time)
+        return check_unread_status(self, from_time, access_token)
 
     def create_group(
         self,
         topic: str,
         description: str = None,
         secret: bool = None,
         hide_reported_posts: bool = None,
@@ -669,14 +1030,15 @@
         group_category_id: int = None,
         cover_image_filename: str = None,
         sub_category_id: str = None,
         hide_from_game_eight: bool = None,
         allow_members_to_post_media: bool = None,
         allow_members_to_post_url: bool = None,
         guidelines: str = None,
+        access_token: str = None,
     ) -> CreateGroupResponse:
         """
 
         サークルを作成します
 
         """
         return create_group(
@@ -697,143 +1059,154 @@
             group_category_id,
             cover_image_filename,
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
             guidelines,
+            access_token,
         )
 
-    def pin_group(self, group_id: int) -> dict:
+    def pin_group(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークルをピンします
 
         """
-        return create_pin_group(self, group_id)
+        return create_pin_group(self, group_id, access_token)
 
-    def decline_moderator_offer(self, group_id: int) -> dict:
+    def decline_moderator_offer(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークル副管理人の権限オファーを断ります
 
         """
-        return decline_moderator_offer(self, group_id)
+        return decline_moderator_offer(self, group_id, access_token)
 
-    def decline_ownership_offer(self, group_id: int) -> dict:
+    def decline_ownership_offer(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークル管理人の権限オファーを断ります
 
         """
-        return decline_ownership_offer(self, group_id)
+        return decline_ownership_offer(self, group_id, access_token)
 
-    def decline_group_join_request(self, group_id: int, user_id: int) -> dict:
+    def decline_group_join_request(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル参加リクエストを断ります
 
         """
-        return decline_ownership_offer(self, group_id, user_id)
+        return decline_group_join_request(self, group_id, user_id, access_token)
 
-    def unpin_group(self, group_id: int) -> dict:
+    def unpin_group(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークルのピン止めを解除します
 
         """
-        return delete_pin_group(self, group_id)
+        return delete_pin_group(self, group_id, access_token)
 
     def get_banned_group_members(
-        self, group_id: int, page: int = None
+        self, group_id: int, page: int = None, access_token: str = None
     ) -> UsersResponse:
         """
 
         追放されたサークルメンバーを取得します
 
         """
-        return get_banned_group_members(self, group_id, page)
+        return get_banned_group_members(self, group_id, page, access_token)
 
-    def get_group_categories(self, **params) -> GroupCategoriesResponse:
+    def get_group_categories(
+        self, access_token: str = None, **params
+    ) -> GroupCategoriesResponse:
         """
 
         サークルのカテゴリーを取得します
 
         Parameters
         ----------
 
             - page: int - (optional)
             - number: int - (optional)
 
         """
-        return get_group_categories(self, **params)
+        return get_group_categories(self, access_token, **params)
 
-    def get_create_group_quota(self) -> CreateGroupQuota:
+    def get_create_group_quota(self, access_token: str = None) -> CreateGroupQuota:
         """
 
         サークル作成可能な割当量を取得します
 
         """
-        return get_create_group_quota(self)
+        return get_create_group_quota(self, access_token)
 
-    def get_group(self, group_id: int) -> GroupResponse:
+    def get_group(self, group_id: int, access_token: str = None) -> GroupResponse:
         """
 
         サークルの詳細を取得します
 
         """
-        return get_group(self, group_id)
+        return get_group(self, group_id, access_token)
 
-    def get_groups(self, **params) -> GroupsResponse:
+    def get_groups(self, access_token: str = None, **params) -> GroupsResponse:
         """
 
         複数のサークルの詳細を取得します
 
         Parameters
         ----------
 
             - group_category_id: int = None
             - keyword: str = None
             - from_timestamp: int = None
             - sub_category_id: int = None
 
         """
-        return get_groups(self, **params)
+        return get_groups(self, access_token, **params)
 
-    def get_invitable_users(self, group_id: int, **params) -> UsersByTimestampResponse:
+    def get_invitable_users(
+        self, group_id: int, access_token: str = None, **params
+    ) -> UsersByTimestampResponse:
         """
 
         サークルに招待可能なユーザーを取得します
 
         Parameters
         ----------
 
             - from_timestamp: int - (optional)
             - user[nickname]: str - (optional)
 
         """
-        return get_invitable_users(self, group_id, **params)
+        return get_invitable_users(self, group_id, access_token, **params)
 
-    def get_joined_statuses(self, ids: List[int]) -> dict:
+    def get_joined_statuses(self, ids: List[int], access_token: str = None) -> dict:
         """
 
         サークルの参加ステータスを取得します
 
         """
-        return get_joined_statuses(self, ids)
+        return get_joined_statuses(self, ids, access_token)
 
-    def get_group_member(self, group_id: int, user_id: int) -> GroupUserResponse:
+    def get_group_member(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> GroupUserResponse:
         """
 
         特定のサークルメンバーの情報を取得します
 
         """
-        return get_group_member(self, group_id, user_id)
+        return get_group_member(self, group_id, user_id, access_token)
 
-    def get_group_members(self, group_id: int, **params) -> GroupUsersResponse:
+    def get_group_members(
+        self, group_id: int, access_token: str = None, **params
+    ) -> GroupUsersResponse:
         """
 
         サークルメンバーを取得します
 
         Parameters
         ----------
 
@@ -842,136 +1215,149 @@
             - keyword: str - (optional)
             - from_id: int - (optional)
             - from_timestamp: int - (optional)
             - order_by: str - (optional)
             - followed_by_me: bool - (optional)
 
         """
-        return get_group_members(self, group_id, **params)
+        return get_group_members(self, group_id, access_token, **params)
 
-    def get_my_groups(self, from_timestamp: None) -> GroupsResponse:
+    def get_my_groups(
+        self, from_timestamp: None, access_token: str = None
+    ) -> GroupsResponse:
         """
 
         自分のサークルを取得します
 
         """
-        return get_my_groups(self, from_timestamp)
+        return get_my_groups(self, from_timestamp, access_token)
 
-    def get_relatable_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
+    def get_relatable_groups(
+        self, group_id: int, access_token: str = None, **params
+    ) -> GroupsRelatedResponse:
         """
 
         関連がある可能性があるサークルを取得します
 
         Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
-        return get_relatable_groups(self, group_id, **params)
+        return get_relatable_groups(self, group_id, access_token, **params)
 
-    def get_related_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
+    def get_related_groups(
+        self, group_id: int, access_token: str = None, **params
+    ) -> GroupsRelatedResponse:
         """
 
         関連があるサークルを取得します
 
         Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
-        return get_related_groups(self, group_id, **params)
+        return get_related_groups(self, group_id, access_token, **params)
 
-    def get_user_groups(self, **params) -> GroupsResponse:
+    def get_user_groups(self, access_token: str = None, **params) -> GroupsResponse:
         """
 
         特定のユーザーが参加しているサークルを取得します
 
         Parameters
         ----------
 
             - user_id: int - (required)
             - page: int - (optional)
 
         """
-        return get_user_groups(self, **params)
+        return get_user_groups(self, access_token, **params)
 
-    def invite_users_to_group(self, group_id: int, user_ids: List[int]) -> dict:
+    def invite_users_to_group(
+        self, group_id: int, user_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         サークルにユーザーを招待します
 
         """
-        return invite_users_to_group(self, group_id, user_ids)
+        return invite_users_to_group(self, group_id, user_ids, access_token)
 
-    def join_group(self, group_id: int) -> dict:
+    def join_group(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークルに参加します
 
         """
-        return join_group(self, group_id)
+        return join_group(self, group_id, access_token)
 
-    def leave_group(self, group_id: int) -> dict:
+    def leave_group(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークルから脱退します
 
         """
-        return leave_group(self, group_id)
+        return leave_group(self, group_id, access_token)
 
-    def post_gruop_social_shared(self, group_id: int, sns_name: str) -> dict:
+    def post_gruop_social_shared(
+        self, group_id: int, sns_name: str, access_token: str = None
+    ) -> dict:
         """
 
         サークルのソーシャルシェアを投稿します
 
         """
-        return post_gruop_social_shared(self, group_id, sns_name)
+        return post_gruop_social_shared(self, group_id, sns_name, access_token)
 
-    def remove_group_cover(self, group_id: int) -> dict:
+    def remove_group_cover(self, group_id: int, access_token: str = None) -> dict:
         """
 
         サークルのカバー画像を削除します
 
         """
-        return remove_group_cover(self, group_id)
+        return remove_group_cover(self, group_id, access_token)
 
-    def remove_moderator(self, group_id: int, user_id: int) -> dict:
+    def remove_moderator(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークルの副管理人を削除します
 
         """
-        return remove_moderator(self, group_id, user_id)
+        return remove_moderator(self, group_id, user_id, access_token)
 
     def remove_related_groups(
-        self, group_id: int, related_group_ids: List[int]
+        self, group_id: int, related_group_ids: List[int], access_token: str = None
     ) -> dict:
         """
 
         関連のあるサークルを削除します
 
         """
-        return remove_related_groups(self, group_id, related_group_ids)
+        return remove_related_groups(self, group_id, related_group_ids, access_token)
 
     def report_group(
         self,
         group_id: int,
         category_id: int,
         reason: str = None,
         opponent_id: int = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         サークルを通報します
 
         """
         return report_group(
@@ -980,55 +1366,66 @@
             category_id,
             reason,
             opponent_id,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename,
+            access_token,
         )
 
-    def send_moderator_offers(self, group_id: int, user_ids: List[int]) -> dict:
+    def send_moderator_offers(
+        self, group_id: int, user_ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         複数人にサークル副管理人のオファーを送信します
 
         """
-        return send_moderator_offers(self, group_id, user_ids)
+        return send_moderator_offers(self, group_id, user_ids, access_token)
 
-    def send_ownership_offer(self, group_id: int, user_id: int) -> dict:
+    def send_ownership_offer(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル管理人権限のオファーを送信します
 
         """
-        return send_ownership_offer(self, group_id, user_id)
+        return send_ownership_offer(self, group_id, user_id, access_token)
 
-    def set_group_title(self, group_id: int, title: str) -> dict:
+    def set_group_title(
+        self, group_id: int, title: str, access_token: str = None
+    ) -> dict:
         """
 
         サークルのタイトルを設定します
 
         """
-        return set_group_title(self, group_id, title)
+        return set_group_title(self, group_id, title, access_token)
 
-    def take_over_group_ownership(self, group_id: int) -> dict:
+    def take_over_group_ownership(
+        self, group_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル管理人の権限を引き継ぎます
 
         """
-        return take_over_group_ownership(self, group_id)
+        return take_over_group_ownership(self, group_id, access_token)
 
-    def unban_group_member(self, group_id: int, user_id: int) -> dict:
+    def unban_group_member(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         特定のサークルメンバーの追放を解除します
 
         """
-        return unban_group_member(self, group_id, user_id)
+        return unban_group_member(self, group_id, user_id, access_token)
 
     def update_group(
         self,
         group_id: int,
         topic: str,
         description: str = None,
         secret: bool = None,
@@ -1045,14 +1442,15 @@
         group_category_id: int = None,
         cover_image_filename: str = None,
         sub_category_id: str = None,
         hide_from_game_eight: bool = None,
         allow_members_to_post_media: bool = None,
         allow_members_to_post_url: bool = None,
         guidelines: str = None,
+        access_token: str = None,
     ) -> GroupResponse:
         """
 
         サークルを編集します
 
         """
         return update_group(
@@ -1073,212 +1471,240 @@
             group_category_id,
             cover_image_filename,
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
             guidelines,
+            access_token,
         )
 
-    def withdraw_moderator_offer(self, group_id: int, user_id: int) -> dict:
+    def withdraw_moderator_offer(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル副管理人のオファーを取り消します
 
         """
-        return withdraw_moderator_offer(self, group_id, user_id)
+        return withdraw_moderator_offer(self, group_id, user_id, access_token)
 
-    def withdraw_ownership_offer(self, group_id: int, user_id: int) -> dict:
+    def withdraw_ownership_offer(
+        self, group_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークル管理人のオファーを取り消します
 
         """
-        return withdraw_ownership_offer(self, group_id, user_id)
+        return withdraw_ownership_offer(self, group_id, user_id, access_token)
 
     # -LOGIN
 
     def is_valid_token(self, access_token: str):
         """
 
         アクセストークンが有効か検証します
 
         """
         return is_valid_token(self, access_token)
 
     def change_password(
-        self, current_password: str, new_password: str
+        self, current_password: str, new_password: str, access_token: str = None
     ) -> LoginUpdateResponse:
         """
 
         パスワードを変更します
 
         """
-        return change_password(self, current_password, new_password)
+        return change_password(self, current_password, new_password, access_token)
 
     def get_token(
         self,
         grant_type: str,
         refresh_token: str = None,
         email: str = None,
         password: str = None,
+        access_token: str = None,
     ) -> TokenResponse:
         """
 
         トークンを再発行します
 
         """
-        return get_token(self, grant_type, refresh_token, email, password)
+        return get_token(self, grant_type, refresh_token, email, password, access_token)
 
     def login(
         self, email: str, password: str, secret_key: str = None
     ) -> LoginUserResponse:
         """
 
         メールアドレスでログインします
 
         """
         return login_with_email(self, email, password, secret_key)
 
-    def logout(self) -> dict:
+    def logout(self, access_token: str = None) -> dict:
         """
 
         ログアウトします
 
         """
-        return logout(self)
+        return logout(self, access_token)
 
-    def resend_confirm_email(self) -> dict:
+    def resend_confirm_email(self, access_token: str = None) -> dict:
         """
 
         確認メールを再送信します
 
         """
-        return resend_confirm_email(self)
+        return resend_confirm_email(self, access_token)
 
-    def restore_user(self, user_id: int) -> LoginUserResponse:
+    def restore_user(self, user_id: int, access_token: str = None) -> LoginUserResponse:
         """
 
         ユーザーを復元します
 
         """
-        return restore_user(self, user_id)
+        return restore_user(self, user_id, access_token)
 
-    def revoke_tokens(self) -> dict:
+    def revoke_tokens(self, access_token: str = None) -> dict:
         """
 
         トークンを無効化します
 
         """
-        return revoke_tokens(self)
+        return revoke_tokens(self, access_token)
 
     def save_account_with_email(
         self,
         email: str,
         password: str = None,
         current_password: str = None,
         email_grant_token: str = None,
+        access_token: str = None,
     ) -> LoginUpdateResponse:
         """
 
         メールアドレスでアカウントを保存します
 
         """
         return save_account_with_email(
             self,
             email,
             password,
             current_password,
             email_grant_token,
+            access_token,
         )
 
     # -MISC
 
+    def send_verification_code(self, email: str):
+        """
+
+        認証コードを送信します
+
+        """
+        return send_verification_code(self, email)
+
     def get_email_grant_token(self, code: int, email: str) -> str:
         """
 
         email_grant_tokenを取得します
 
         """
         return get_email_grant_token(self, code, email)
 
     def get_email_verification_presigned_url(
-        self, email: str, locale: str, intent: str = None
+        self, email: str, locale: str, intent: str = None, access_token: str = None
     ) -> str:
         """
 
         メールアドレス確認用の署名付きURLを取得します
 
         """
-        return get_email_verification_presigned_url(self, email, locale, intent)
+        return get_email_verification_presigned_url(
+            self, email, locale, intent, access_token
+        )
 
     def get_file_upload_presigned_urls(
-        self, file_names: List[str]
+        self, file_names: List[str], access_token: str = None
     ) -> List[PresignedUrl]:
         """
 
         ファイルアップロード用の署名付きURLを取得します
 
         """
-        return get_file_upload_presigned_urls(self, file_names)
+        return get_file_upload_presigned_urls(self, file_names, access_token)
 
     # def get_id_checker_presigned_url(
     #         self,
     #         model: str,
     #         action: str,
     #         **params
     # ) -> str:
     #     return get_id_checker_presigned_url(self, model, action, **params)
 
-    def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
+    def get_old_file_upload_presigned_url(
+        self, video_file_name: str, access_token: str = None
+    ) -> str:
         """
 
         動画ファイルアップロード用の署名付きURLを取得します
 
         """
-        return get_old_file_upload_presigned_url(self, video_file_name)
+        return get_old_file_upload_presigned_url(self, video_file_name, access_token)
 
-    def get_web_socket_token(self, headers: dict = None) -> str:
+    def get_web_socket_token(
+        self, headers: dict = None, access_token: str = None
+    ) -> str:
         """
 
         Web Socket Tokenを取得します
 
         """
-        return get_web_socket_token(self, headers)
+        return get_web_socket_token(self, headers, access_token)
 
-    def upload_image(self, image_type: str, image_path: str) -> str:
+    def upload_image(
+        self, image_type: str, image_path: str, access_token: str = None
+    ) -> str:
         """
 
         画像をアップロードしてattachment_filenameを返します。
 
         Parameteres
         -----------
             - image_type: str - (required): "post", "user_avatar" のどちらか
             - image_path: str - (required): "画像のパス
 
         """
-        return upload_image(self, image_type, image_path)
+        return upload_image(self, image_type, image_path, access_token)
 
     # -POST
 
-    def add_bookmark(self, user_id: int, post_id: int) -> BookmarkPostResponse:
+    def add_bookmark(
+        self, user_id: int, post_id: int, access_token: str = None
+    ) -> BookmarkPostResponse:
         """
 
         ブックマークに追加します
 
         """
-        return add_bookmark(self, user_id, post_id)
+        return add_bookmark(self, user_id, post_id, access_token)
 
-    def add_group_highlight_post(self, group_id: int, post_id: int) -> dict:
+    def add_group_highlight_post(
+        self, group_id: int, post_id: int, access_token: str = None
+    ) -> dict:
         """
 
         投稿をグループのまとめに追加します
 
         """
-        return add_group_highlight_post(self, group_id, post_id)
+        return add_group_highlight_post(self, group_id, post_id, access_token)
 
     def create_call_post(
         self,
         text: str = None,
         font_size: int = None,
         color: int = None,
         group_id: int = None,
@@ -1292,14 +1718,15 @@
         attachment_3_filename: str = None,
         attachment_4_filename: str = None,
         attachment_5_filename: str = None,
         attachment_6_filename: str = None,
         attachment_7_filename: str = None,
         attachment_8_filename: str = None,
         attachment_9_filename: str = None,
+        access_token: str = None,
     ) -> ConferenceCall:
         """
 
         通話の投稿を作成します
 
         """
         return create_call_post(
@@ -1318,31 +1745,34 @@
             attachment_3_filename,
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
+            access_token,
         )
 
-    def pin_group_post(self, post_id: int, group_id: int) -> dict:
+    def pin_group_post(
+        self, post_id: int, group_id: int, access_token: str = None
+    ) -> dict:
         """
 
         グループの投稿をピンします
 
         """
-        return create_group_pin_post(self, post_id, group_id)
+        return create_group_pin_post(self, post_id, group_id, access_token)
 
-    def pin_post(self, post_id: int) -> dict:
+    def pin_post(self, post_id: int, access_token: str = None) -> dict:
         """
 
         投稿をピンします
 
         """
-        return create_pin_post(self, post_id)
+        return create_pin_post(self, post_id, access_token)
 
     def mention(self, user_id: int) -> str:
         """
 
         メンション用文字列を返します
 
         """
@@ -1365,14 +1795,15 @@
         attachment_4_filename: str = None,
         attachment_5_filename: str = None,
         attachment_6_filename: str = None,
         attachment_7_filename: str = None,
         attachment_8_filename: str = None,
         attachment_9_filename: str = None,
         video_file_name: str = None,
+        access_token: str = None,
     ) -> Post:
         """
 
         投稿を作成します
 
         """
         return create_post(
@@ -1392,14 +1823,15 @@
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
             video_file_name,
+            access_token,
         )
 
     def create_repost(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
@@ -1416,14 +1848,15 @@
         attachment_4_filename: str = None,
         attachment_5_filename: str = None,
         attachment_6_filename: str = None,
         attachment_7_filename: str = None,
         attachment_8_filename: str = None,
         attachment_9_filename: str = None,
         video_file_name: str = None,
+        access_token: str = None,
     ) -> Post:
         """
 
         投稿を(´∀｀∩)↑age↑します
 
         """
         return create_repost(
@@ -1444,32 +1877,41 @@
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
             video_file_name,
+            access_token,
         )
 
     def create_share_post(
         self,
         shareable_type: str,
         shareable_id: int,
         text: str = None,
         font_size: int = None,
         color: int = None,
         group_id: int = None,
+        access_token: str = None,
     ) -> Post:
         """
 
         シェア投稿を作成します
 
         """
         return create_share_post(
-            self, shareable_type, shareable_id, text, font_size, color, group_id
+            self,
+            shareable_type,
+            shareable_id,
+            text,
+            font_size,
+            color,
+            group_id,
+            access_token,
         )
 
     def create_thread_post(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
@@ -1486,14 +1928,15 @@
         attachment_4_filename: str = None,
         attachment_5_filename: str = None,
         attachment_6_filename: str = None,
         attachment_7_filename: str = None,
         attachment_8_filename: str = None,
         attachment_9_filename: str = None,
         video_file_name: str = None,
+        access_token: str = None,
     ) -> Post:
         """
 
         スレッドの投稿を作成します
 
         """
         return create_thread_post(
@@ -1514,49 +1957,52 @@
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
             video_file_name,
+            access_token,
         )
 
-    def delete_all_post(self) -> dict:
+    def delete_all_post(self, access_token: str = None) -> dict:
         """
 
         すべての自分の投稿を削除します
 
         """
-        return delete_all_post(self)
+        return delete_all_post(self, access_token)
 
-    def unpin_group_post(self, group_id: int) -> dict:
+    def unpin_group_post(self, group_id: int, access_token: str = None) -> dict:
         """
 
         グループのピン投稿を解除します
 
         """
-        return delete_group_pin_post(self, group_id)
+        return delete_group_pin_post(self, group_id, access_token)
 
-    def unpin_post(self, post_id: int) -> dict:
+    def unpin_post(self, post_id: int, access_token: str = None) -> dict:
         """
 
         ピン投稿を削除します
 
         """
-        return delete_pin_post(self, post_id)
+        return delete_pin_post(self, post_id, access_token)
 
-    def get_bookmark(self, user_id: int, from_str: str = None) -> PostsResponse:
+    def get_bookmark(
+        self, user_id: int, from_str: str = None, access_token: str = None
+    ) -> PostsResponse:
         """
 
         ブックマークを取得します
 
         """
-        return get_bookmark(self, user_id, from_str)
+        return get_bookmark(self, user_id, from_str, access_token)
 
-    def get_timeline_calls(self, **params) -> PostsResponse:
+    def get_timeline_calls(self, access_token: str = None, **params) -> PostsResponse:
         """
 
         誰でも通話を取得します
 
         Parameters
         ----------
 
@@ -1567,17 +2013,19 @@
             - call_type: str = "voice"
             - include_circle_call: bool = None
             - cross_generation: bool = None
             - exclude_recent_gomimushi: bool = None
             - shared_interest_categories: bool = None
 
         """
-        return get_timeline_calls(self, **params)
+        return get_timeline_calls(self, access_token, **params)
 
-    def get_conversation(self, conversation_id: int, **params) -> PostsResponse:
+    def get_conversation(
+        self, conversation_id: int, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         リプライを含める投稿の会話を取得します
 
         Parameters
         ----------
 
@@ -1585,25 +2033,29 @@
             - group_id: int = None
             - thread_id: int = None
             - from_post_id: int = None
             - number: int = 50
             - reverse: bool = True
 
         """
-        return get_conversation(self, conversation_id, **params)
+        return get_conversation(self, conversation_id, access_token, **params)
 
-    def get_conversation_root_posts(self, post_ids: List[int]) -> PostsResponse:
+    def get_conversation_root_posts(
+        self, post_ids: List[int], access_token: str = None
+    ) -> PostsResponse:
         """
 
         会話の原点の投稿を取得します
 
         """
-        return get_conversation_root_posts(self, post_ids)
+        return get_conversation_root_posts(self, post_ids, access_token)
 
-    def get_following_call_timeline(self, **params) -> PostsResponse:
+    def get_following_call_timeline(
+        self, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         フォロー中の通話を取得します
 
         Parameters
         ----------
 
@@ -1611,17 +2063,19 @@
             - number: int = None
             - category_id: int = None
             - call_type: str = None
             - include_circle_call: bool = None
             - exclude_recent_gomimushi: bool = None
 
         """
-        return get_following_call_timeline(self, **params)
+        return get_following_call_timeline(self, access_token, **params)
 
-    def get_following_timeline(self, **params) -> PostsResponse:
+    def get_following_timeline(
+        self, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         フォロー中のタイムラインを取得します
 
         Parameters
         ----------
 
@@ -1630,33 +2084,35 @@
             - order_by: str = None
             - number: int = None
             - mxn: int = None
             - reduce_selfie: bool = None
             - custom_generation_range: bool = None
 
         """
-        return get_following_timeline(self, **params)
+        return get_following_timeline(self, access_token, **params)
 
-    def get_group_highlight_posts(self, group_id: int, **params) -> PostsResponse:
+    def get_group_highlight_posts(
+        self, group_id: int, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         グループのハイライト投稿を取得します
 
         Parameters
         ----------
 
             - group_id: int
             - from_post: int = None
             - number: int = None
 
         """
-        return get_group_highlight_posts(self, group_id, **params)
+        return get_group_highlight_posts(self, group_id, access_token, **params)
 
     def get_group_timeline_by_keyword(
-        self, group_id: int, keyword: str, **params
+        self, group_id: int, keyword: str, access_token: str = None, **params
     ) -> PostsResponse:
         """
 
         グループの投稿をキーワードで検索します
 
         Parameters
         ----------
@@ -1664,17 +2120,21 @@
             - group_id: int
             - keyword: str
             - from_post_id: int = None
             - number: int = None
             - only_thread_posts: bool = False
 
         """
-        return get_group_timeline_by_keyword(self, group_id, keyword, **params)
+        return get_group_timeline_by_keyword(
+            self, group_id, keyword, access_token, **params
+        )
 
-    def get_group_timeline(self, group_id: int, **params) -> PostsResponse:
+    def get_group_timeline(
+        self, group_id: int, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         グループのタイムラインを取得します
 
         Parameters
         ----------
 
@@ -1682,132 +2142,145 @@
             - from_post_id: int
             - reverse: bool
             - post_type: str
             - number: int
             - only_root: bool
 
         """
-        return get_group_timeline(self, group_id, **params)
+        return get_group_timeline(self, group_id, access_token, **params)
 
-    def get_timeline_by_hashtag(self, hashtag: str, **params) -> PostsResponse:
+    def get_timeline_by_hashtag(
+        self, hashtag: str, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         ハッシュタグでタイムラインを検索します
 
         Parameters
         ----------
 
             - hashtag: str - (required)
             - from_post_id: int - (optional)
             - number: int - (optional)
 
         """
-        return get_timeline_by_hashtag(self, hashtag, **params)
+        return get_timeline_by_hashtag(self, hashtag, access_token, **params)
 
-    def get_my_posts(self, **params) -> PostsResponse:
+    def get_my_posts(self, access_token: str = None, **params) -> PostsResponse:
         """
 
         自分の投稿を取得します
 
         Parameters
         ----------
 
             - from_post_id: int - (optional)
             - number: int - (optional)
             - include_group_post: bool - (optional)
 
         """
-        return get_my_posts(self, **params)
+        return get_my_posts(self, access_token, **params)
 
-    def get_post(self, post_id: int) -> Post:
+    def get_post(self, post_id: int, access_token: str = None) -> Post:
         """
 
         投稿の詳細を取得します
 
         """
-        return get_post(self, post_id)
+        return get_post(self, post_id, access_token)
 
-    def get_post_likers(self, post_id: int, **params) -> PostLikersResponse:
+    def get_post_likers(
+        self, post_id: int, access_token: str = None, **params
+    ) -> PostLikersResponse:
         """
 
         投稿にいいねしたユーザーを取得します
 
         Parameters
         ----------
 
             - from_id: int - (optional)
             - number: int - (optional)
 
         """
-        return get_post_likers(self, post_id, **params)
+        return get_post_likers(self, post_id, access_token, **params)
 
-    def get_reposts(self, post_id: int, **params: int) -> PostsResponse:
+    def get_reposts(
+        self, post_id: int, access_token: str = None, **params: int
+    ) -> PostsResponse:
         """
 
         投稿の(´∀｀∩)↑age↑を取得します
 
         Parameters
         ----------
 
             - post_id: int - (required)
             - from_post_id: int - (optional)
             - number: int - (optional)
 
         """
-        return get_post_reposts(self, post_id, **params)
+        return get_post_reposts(self, post_id, access_token, **params)
 
-    def get_posts(self, post_ids: List[int]) -> PostsResponse:
+    def get_posts(self, post_ids: List[int], access_token: str = None) -> PostsResponse:
         """
 
         複数の投稿を取得します
 
         """
-        return get_posts(self, post_ids)
+        return get_posts(self, post_ids, access_token)
 
     def get_recommended_post_tags(
-        self, tag: str = None, save_recent_search: bool = False
+        self,
+        tag: str = None,
+        save_recent_search: bool = False,
+        access_token: str = None,
     ) -> PostTagsResponse:
         """
 
         おすすめのタグ候補を取得します
 
         """
-        return get_recommended_post_tags(self, tag, save_recent_search)
+        return get_recommended_post_tags(self, tag, save_recent_search, access_token)
 
-    def get_recommended_posts(self, **params) -> PostsResponse:
+    def get_recommended_posts(
+        self, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         おすすめの投稿を取得します
 
         Parameters
         ----------
 
             - experiment_num: int
             - variant_num: int
             - number: int
 
         """
-        return get_recommended_posts(self, **params)
+        return get_recommended_posts(self, access_token, **params)
 
-    def get_timeline_by_keyword(self, keyword: str = None, **params) -> PostsResponse:
+    def get_timeline_by_keyword(
+        self, keyword: str = None, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         キーワードでタイムラインを検索します
 
         Parameters
         ----------
 
             - keyword: str
             - from_post_id: int
             - number: int
 
         """
-        return get_timeline_by_keyword(self, keyword, **params)
+        return get_timeline_by_keyword(self, keyword, access_token, **params)
 
-    def get_timeline(self, **params) -> PostsResponse:
+    def get_timeline(self, access_token: str = None, **params) -> PostsResponse:
         # - from: str - (optional)
         """
 
         タイムラインを取得します
 
         Parameters
         ----------
@@ -1821,83 +2294,90 @@
             - mxn: int - (optional)
             - en: int - (optional)
             - vn: int - (optional)
             - reduce_selfie: bool - (optional)
             - custom_generation_range: bool - (optional)
 
         """
-        return get_timeline(self, **params)
+        return get_timeline(self, access_token, **params)
 
-    def get_url_metadata(self, url: str) -> SharedUrl:
+    def get_url_metadata(self, url: str, access_token: str = None) -> SharedUrl:
         """
 
         URLのメタデータを取得します
 
         """
-        return get_url_metadata(self, url)
+        return get_url_metadata(self, url, access_token)
 
-    def get_user_timeline(self, user_id: int, **params) -> PostsResponse:
+    def get_user_timeline(
+        self, user_id: int, access_token: str = None, **params
+    ) -> PostsResponse:
         """
 
         ユーザーのタイムラインを取得します
 
         Parameters
         ----------
 
             - from_post_id: int - (optional)
             - number: int - (optional)
             - post_type: str - (optional)
 
         """
-        return get_user_timeline(self, user_id, **params)
+        return get_user_timeline(self, user_id, access_token, **params)
 
-    def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
+    def like(self, post_ids: List[int], access_token: str = None) -> LikePostsResponse:
         """
 
         投稿にいいねします
 
         ※ 一度にいいねできる投稿数は最大25個
 
         """
-        return like_posts(self, post_ids)
+        return like_posts(self, post_ids, access_token)
 
-    def remove_bookmark(self, user_id: int, post_id: int) -> dict:
+    def remove_bookmark(
+        self, user_id: int, post_id: int, access_token: str = None
+    ) -> dict:
         """
 
         ブックマークを削除します
 
         """
-        return remove_bookmark(self, user_id, post_id)
+        return remove_bookmark(self, user_id, post_id, access_token)
 
-    def remove_group_highlight_post(self, group_id: int, post_id: int) -> dict:
+    def remove_group_highlight_post(
+        self, group_id: int, post_id: int, access_token: str = None
+    ) -> dict:
         """
 
         サークルのハイライト投稿を解除します
 
         """
-        return remove_group_highlight_post(self, group_id, post_id)
+        return remove_group_highlight_post(self, group_id, post_id, access_token)
 
-    def remove_posts(self, post_ids: List[int]) -> dict:
+    def remove_posts(self, post_ids: List[int], access_token: str = None) -> dict:
         """
 
         複数の投稿を削除します
 
         """
-        return remove_posts(self, post_ids)
+        return remove_posts(self, post_ids, access_token)
 
     def report_post(
         self,
         post_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         投稿を通報します
 
         """
         return report_post(
@@ -1906,357 +2386,399 @@
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename,
+            access_token,
         )
 
-    def unlike_post(self, post_id: int) -> dict:
+    def unlike(self, post_id: int, access_token: str = None) -> dict:
         """
 
         投稿のいいねを解除します
 
         """
-        return unlike_post(self, post_id)
+        return unlike_post(self, post_id, access_token)
 
     def update_post(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
         color: int = None,
         message_tags: str = "[]",
+        access_token: str = None,
     ) -> Post:
         """
 
         投稿を編集します
 
         """
-        return update_post(self, post_id, text, font_size, color, message_tags)
+        return update_post(
+            self, post_id, text, font_size, color, message_tags, access_token
+        )
 
-    def view_video(self, video_id: int) -> dict:
+    def view_video(self, video_id: int, access_token: str = None) -> dict:
         """
 
         動画を視聴します
 
         """
-        return view_video(self, video_id)
+        return view_video(self, video_id, access_token)
 
-    def vote_survey(self, survey_id: int, choice_id: int) -> Survey:
+    def vote_survey(
+        self, survey_id: int, choice_id: int, access_token: str = None
+    ) -> Survey:
         """
 
         アンケートに投票します
 
         """
-        return vote_survey(self, survey_id, choice_id)
+        return vote_survey(self, survey_id, choice_id, access_token)
 
     # -REVIEW
 
-    def create_review(self, user_id: int, comment: str) -> dict:
+    def create_review(
+        self, user_id: int, comment: str, access_token: str = None
+    ) -> dict:
         """
 
         レターを送信します
 
         """
-        return create_review(self, user_id, comment)
+        return create_review(self, user_id, comment, access_token)
 
-    def create_reviews(self, user_ids: List[int], comment: str) -> dict:
+    def create_reviews(
+        self, user_ids: List[int], comment: str, access_token: str = None
+    ) -> dict:
         """
 
         複数人にレターを送信します
 
         """
-        return create_reviews(self, user_ids, comment)
+        return create_reviews(self, user_ids, comment, access_token)
 
-    def delete_reviews(self, review_ids: List[int]) -> dict:
+    def delete_reviews(self, review_ids: List[int], access_token: str = None) -> dict:
         """
 
         レターを削除します
 
         """
-        return delete_reviews(self, review_ids)
+        return delete_reviews(self, review_ids, access_token)
 
-    def get_my_reviews(self, **params) -> ReviewsResponse:
+    def get_my_reviews(self, access_token: str = None, **params) -> ReviewsResponse:
         """
 
         送信したレターを取得します
 
         Parameters
         ----------
 
             - from_id: int (optional)
             - number: int = (optional)
 
         """
-        return get_my_reviews(self, **params)
+        return get_my_reviews(self, access_token, **params)
 
-    def get_reviews(self, user_id: int, **params) -> ReviewsResponse:
+    def get_reviews(
+        self, user_id: int, access_token: str = None, **params
+    ) -> ReviewsResponse:
         """
 
         ユーザーが受け取ったレターを取得します
 
         Parameters
         ----------
 
             - user_id: int (required)
             - from_id: int = (optional)
             - number: int = (optional)
 
         """
-        return get_reviews(self, user_id, **params)
+        return get_reviews(self, user_id, access_token, **params)
 
-    def pin_review(self, review_id: int) -> dict:
+    def pin_review(self, review_id: int, access_token: str = None) -> dict:
         """
 
         レターをピンします
 
         """
-        return pin_review(self, review_id)
+        return pin_review(self, review_id, access_token)
 
-    def unpin_review(self, review_id: int) -> dict:
+    def unpin_review(self, review_id: int, access_token: str = None) -> dict:
         """
 
         レターのピン止めを解除します
 
         """
-        return unpin_review(self, review_id)
+        return unpin_review(self, review_id, access_token)
 
     # -THREAD
 
-    def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
+    def add_post_to_thread(
+        self, post_id: int, thread_id: int, access_token: str = None
+    ) -> ThreadInfo:
         """
 
         投稿をスレッドに追加します
 
         """
-        return add_post_to_thread(self, post_id, thread_id)
+        return add_post_to_thread(self, post_id, thread_id, access_token)
 
     def convert_post_to_thread(
-        self, post_id: int, title: str = None, thread_icon_filename: str = None
+        self,
+        post_id: int,
+        title: str = None,
+        thread_icon_filename: str = None,
+        access_token: str = None,
     ) -> ThreadInfo:
         """
 
         投稿をスレッドに変換します
 
         """
-        return convert_post_to_thread(self, post_id, title, thread_icon_filename)
+        return convert_post_to_thread(
+            self, post_id, title, thread_icon_filename, access_token
+        )
 
     def create_thread(
-        self, group_id: int, title: str, thread_icon_filename: str
+        self,
+        group_id: int,
+        title: str,
+        thread_icon_filename: str,
+        access_token: str = None,
     ) -> ThreadInfo:
         """
 
         スレッドを作成します
 
         """
-        return create_thread(self, group_id, title, thread_icon_filename)
+        return create_thread(self, group_id, title, thread_icon_filename, access_token)
 
     def get_group_thread_list(
-        self, group_id: int, from_str: str = None, **params
+        self, group_id: int, from_str: str = None, access_token: str = None, **params
     ) -> GroupThreadListResponse:
         """
 
         グループのスレッド一覧を取得します
 
         Parameters
         ----------
 
             - group_id: int
             - from_str: str = None
             - join_status: str = None
 
         """
-        return get_group_thread_list(self, group_id, from_str, **params)
+        return get_group_thread_list(self, group_id, from_str, access_token, **params)
 
-    def get_thread_joined_statuses(self, ids: List[int]) -> dict:
+    def get_thread_joined_statuses(
+        self, ids: List[int], access_token: str = None
+    ) -> dict:
         """
 
         スレッド参加ステータスを取得します
 
         """
-        return get_thread_joined_statuses(self, ids)
+        return get_thread_joined_statuses(self, ids, access_token)
 
     def get_thread_posts(
-        self, thread_id: int, from_str: str = None, **params
+        self, thread_id: int, from_str: str = None, access_token: str = None, **params
     ) -> PostsResponse:
         """
 
         スレッドの投稿を取得します
 
         Parameters
         ----------
 
             - post_type: str
             - number: int = None
             - from_str: str = None
 
         """
-        return get_thread_posts(self, thread_id, from_str, **params)
+        return get_thread_posts(self, thread_id, from_str, access_token, **params)
 
-    def join_thread(self, thread_id: int, user_id: int) -> dict:
+    def join_thread(
+        self, thread_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         スレッドに参加します
 
         """
-        return join_thread(self, thread_id, user_id)
+        return join_thread(self, thread_id, user_id, access_token)
 
-    def leave_thread(self, thread_id: int, user_id: int) -> dict:
+    def leave_thread(
+        self, thread_id: int, user_id: int, access_token: str = None
+    ) -> dict:
         """
 
         スレッドから脱退します
 
         """
-        return leave_thread(self, thread_id, user_id)
+        return leave_thread(self, thread_id, user_id, access_token)
 
-    def remove_thread(self, thread_id: int) -> dict:
+    def remove_thread(self, thread_id: int, access_token: str = None) -> dict:
         """
 
         スレッドを削除します
 
         """
-        return remove_thread(self, thread_id)
+        return remove_thread(self, thread_id, access_token)
 
     def update_thread(
-        self, thread_id: int, title: str, thread_icon_filename: str
+        self,
+        thread_id: int,
+        title: str,
+        thread_icon_filename: str,
+        access_token: str = None,
     ) -> dict:
         """
 
         スレッドを編集します
 
         """
-        return update_thread(self, thread_id, title, thread_icon_filename)
+        return update_thread(self, thread_id, title, thread_icon_filename, access_token)
 
     # -USER
 
-    def delete_footprint(self, user_id: int, footprint_id: int) -> dict:
+    def delete_footprint(
+        self, user_id: int, footprint_id: int, access_token: str = None
+    ) -> dict:
         """
 
         足跡を削除します
 
         """
-        return delete_footprint(self, user_id, footprint_id)
+        return delete_footprint(self, user_id, footprint_id, access_token)
 
-    def destroy_user(self) -> dict:
+    def destroy_user(self, access_token: str = None) -> dict:
         """
 
         アカウントを削除します
 
         """
-        return destroy_user(self)
+        return destroy_user(self, access_token)
 
-    def follow_user(self, user_id: int) -> dict:
+    def follow_user(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ユーザーをフォローします
 
         """
-        return follow_user(self, user_id)
+        return follow_user(self, user_id, access_token)
 
-    def follow_users(self, user_ids: List[int]) -> dict:
+    def follow_users(self, user_ids: List[int], access_token: str = None) -> dict:
         """
 
         複数のユーザーをフォローします
 
         """
-        return follow_users(self, user_ids)
+        return follow_users(self, user_ids, access_token)
 
-    def get_active_followings(self, **params) -> ActiveFollowingsResponse:
+    def get_active_followings(
+        self, access_token: str = None, **params
+    ) -> ActiveFollowingsResponse:
         """
 
         アクティブなフォロー中のユーザーを取得します
 
         Parameters
         ----------
 
             - only_online: bool
             - from_loggedin_at: int = None
 
         """
-        return get_active_followings(self, **params)
+        return get_active_followings(self, access_token, **params)
 
-    def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
+    def get_follow_recommendations(
+        self, access_token: str = None, **params
+    ) -> FollowRecommendationsResponse:
         """
 
         フォローするのにおすすめのユーザーを取得します
 
         Parameters
         ----------
 
             - from_timestamp: int = None,
             - number: int = None,
             - sources: List[str] = None
 
         """
-        return get_follow_recommendations(self, **params)
+        return get_follow_recommendations(self, access_token, **params)
 
     def get_follow_request(
-        self, from_timestamp: int = None
+        self, from_timestamp: int = None, access_token: str = None
     ) -> UsersByTimestampResponse:
         """
 
         フォローリクエストを取得します
 
         """
-        return get_follow_request(self, from_timestamp)
+        return get_follow_request(self, from_timestamp, access_token)
 
-    def get_follow_request_count(self) -> int:
+    def get_follow_request_count(self, access_token: str = None) -> int:
         """
 
         フォローリクエストの数を取得します
 
         """
-        return get_follow_request_count(self)
+        return get_follow_request_count(self, access_token)
 
-    def get_following_users_born(self, birthdate: int = None) -> UsersResponse:
+    def get_following_users_born(
+        self, birthdate: int = None, access_token: str = None
+    ) -> UsersResponse:
         """
 
         フォロー中のユーザーの誕生日を取得します
 
         """
-        return get_following_users_born(self, birthdate)
+        return get_following_users_born(self, birthdate, access_token)
 
-    def get_footprints(self, **params) -> List[Footprint]:
+    def get_footprints(self, access_token: str = None, **params) -> List[Footprint]:
         """
 
         足跡を取得します
 
         Parameters
         ----------
 
             - from_id: int = None
             - number: int = None
             - mode: str = None
 
         """
-        return get_footprints(self, **params)
+        return get_footprints(self, access_token, **params)
 
-    def get_fresh_user(self, user_id: int) -> UserResponse:
+    def get_fresh_user(self, user_id: int, access_token: str = None) -> UserResponse:
         """
 
         認証情報などを含んだユーザー情報を取得します
 
         """
-        return get_fresh_user(self, user_id)
+        return get_fresh_user(self, user_id, access_token)
 
-    def get_hima_users(self, **params) -> List[UserWrapper]:
+    def get_hima_users(self, access_token: str = None, **params) -> List[UserWrapper]:
         """
 
         暇なユーザーを取得します
 
         Parameters
         ----------
 
             - from_hima_id: int = None
             - number: int = None
 
         """
-        return get_hima_users(self, **params)
+        return get_hima_users(self, access_token, **params)
 
     def get_user_ranking(self, mode: str) -> RankingUsersResponse:
         """
 
         ユーザーのフォロワーランキングを取得します
 
         Examples:
@@ -2277,157 +2799,207 @@
         >>> 殿堂入りを取得する場合:
 
         >>> api.get_user_ranking(mode="all_time")
 
         """
         return get_user_ranking(self, mode)
 
-    def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
+    def get_refresh_counter_requests(
+        self, access_token: str = None
+    ) -> RefreshCounterRequestsResponse:
         """
 
         カウンター更新のリクエストを取得します
 
         """
-        return get_refresh_counter_requests(self)
+        return get_refresh_counter_requests(self, access_token)
 
-    def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
+    def get_social_shared_users(
+        self, access_token: str = None, **params
+    ) -> SocialShareUsersResponse:
         """
 
         SNS共有をしたユーザーを取得します
 
         Parameters
         ----------
 
             - sns_name: str - (Required)
             - number: int - (Optional)
             - from_id: int - (Optional)
 
         """
-        return get_social_shared_users(self, **params)
+        return get_social_shared_users(self, access_token, **params)
 
-    def get_timestamp(self) -> UserTimestampResponse:
+    def get_timestamp(self, access_token: str = None) -> UserTimestampResponse:
         """
 
         タイムスタンプを取得します
 
         """
-        return get_timestamp(self)
+        return get_timestamp(self, access_token)
 
-    def get_user(self, user_id: int) -> User:
+    def get_user(self, user_id: int, access_token: str = None) -> User:
         """
 
         ユーザーの情報を取得します
 
         """
-        return get_user(self, user_id)
+        return get_user(self, user_id, access_token)
 
-    def get_user_email(self, user_id: int) -> str:
+    def get_user_email(self, user_id: int, access_token: str = None) -> str:
         """
 
         ユーザーのメールアドレスを取得します
 
         """
-        return get_user_email(self, user_id)
+        return get_user_email(self, user_id, access_token)
 
-    def get_user_followers(self, user_id: int, **params) -> FollowUsersResponse:
+    def get_user_followers(
+        self, user_id: int, access_token: str = None, **params
+    ) -> FollowUsersResponse:
         """
 
         ユーザーのフォロワーを取得します
 
         Parameters
         ----------
 
             - user_id: int
             - from_follow_id: int = None
             - followed_by_me: int = None
 
         """
-        return get_user_followers(self, user_id, **params)
+        return get_user_followers(self, user_id, access_token, **params)
 
-    def get_user_followings(self, user_id: int, **params) -> FollowUsersResponse:
+    def get_user_followings(
+        self, user_id: int, access_token: str = None, **params
+    ) -> FollowUsersResponse:
         """
 
         フォロー中のユーザーを取得します
 
         Parameters
         ----------
 
             - user_id: int
             - from_follow_id: int = None
             - from_timestamp: int = None
             - order_by: str = None
 
         """
-        return get_user_followings(self, user_id, **params)
+        return get_user_followings(self, user_id, access_token, **params)
 
-    def get_user_from_qr(self, qr: str) -> UserResponse:
+    def get_user_from_qr(self, qr: str, access_token: str = None) -> UserResponse:
         """
 
         QRコードからユーザーを取得します
 
         """
-        return get_user_from_qr(self, qr)
+        return get_user_from_qr(self, qr, access_token)
 
-    def get_user_without_leaving_footprint(self, user_id: int) -> UserResponse:
+    def get_user_without_leaving_footprint(
+        self, user_id: int, access_token: str = None
+    ) -> UserResponse:
         """
 
         足跡をつけずにユーザーの情報を取得します
 
         """
-        return get_user_without_leaving_footprint(self, user_id)
+        return get_user_without_leaving_footprint(self, user_id, access_token)
 
-    def get_users(self, user_ids: List[int]) -> UsersResponse:
+    def get_users(self, user_ids: List[int], access_token: str = None) -> UsersResponse:
         """
 
         複数のユーザーの情報を取得します
 
         """
-        return get_users(self, user_ids)
+        return get_users(self, user_ids, access_token)
 
-    def reduce_kenta_penalty(self, user_id: int) -> dict:
+    def reduce_kenta_penalty(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ペナルティーを緩和します
 
         """
-        return reduce_kenta_penalty(self, user_id)
+        return reduce_kenta_penalty(self, user_id, access_token)
 
-    def refresh_counter(self, counter: str) -> dict:
+    def refresh_counter(self, counter: str, access_token: str = None) -> dict:
         """
 
         カウンターを更新します
 
         """
-        return refresh_counter(self, counter)
+        return refresh_counter(self, counter, access_token)
+
+    def register_user(
+        self,
+        email: str,
+        email_grant_token: str,
+        password: str,
+        nickname: str,
+        birth_date: str,
+        gender: int = -1,
+        country_code: str = "JP",
+        biography: str = None,
+        prefecture: str = None,
+        profile_icon_filename: str = None,
+        cover_image_filename: str = None,
+        # @Nullable @Part("sns_info") SignUpSnsInfoRequest signUpSnsInfoRequest,
+        en: int = None,
+        vn: int = None,
+    ):
+        """
+
+        Register user
+
+        """
+        return register_user(
+            self,
+            email,
+            email_grant_token,
+            password,
+            nickname,
+            birth_date,
+            gender,
+            country_code,
+            biography,
+            prefecture,
+            profile_icon_filename,
+            cover_image_filename,
+            en,
+            vn,
+        )
 
-    def remove_user_avatar(self) -> dict:
+    def remove_user_avatar(self, access_token: str = None) -> dict:
         """
 
         ユーザーのアイコンを削除します
 
         """
-        return remove_user_avatar(self)
+        return remove_user_avatar(self, access_token)
 
-    def remove_user_cover(self) -> dict:
+    def remove_user_cover(self, access_token: str = None) -> dict:
         """
 
         ユーザーのカバー画像を削除します
 
         """
-        return remove_user_cover(self)
+        return remove_user_cover(self, access_token)
 
     def report_user(
         self,
         user_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         ユーザーを通報します
 
         """
         return report_user(
@@ -2435,40 +3007,47 @@
             user_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
             screenshot_4_filename,
+            access_token,
         )
 
-    def reset_password(self, email: str, email_grant_token: str, password: str) -> dict:
+    def reset_password(
+        self,
+        email: str,
+        email_grant_token: str,
+        password: str,
+        access_token: str = None,
+    ) -> dict:
         """
 
         パスワードをリセットします
 
         """
-        return reset_password(self, email, email_grant_token, password)
+        return reset_password(self, email, email_grant_token, password, access_token)
 
-    def search_lobi_users(self, **params) -> UsersResponse:
+    def search_lobi_users(self, access_token: str = None, **params) -> UsersResponse:
         """
 
         Lobiのユーザーを検索します
 
         Parameters
         ----------
 
             - nickname: str = None
             - number: int = None
             - from_str: str = None
 
         """
-        return search_lobi_users(self**params)
+        return search_lobi_users(self, access_token, **params)
 
-    def search_users(self, **params) -> UsersResponse:
+    def search_users(self, access_token: str = None, **params) -> UsersResponse:
         """
 
         ユーザーを検索します
 
         Parameters
         ----------
 
@@ -2480,55 +3059,58 @@
             - similar_age: bool = None
             - not_recent_gomimushi: bool = None
             - recently_created: bool = None
             - same_prefecture: bool = None
             - save_recent_search: bool = None
 
         """
-        return search_users(self, **params)
+        return search_users(self, access_token, **params)
 
     def set_follow_permission_enabled(
-        self, nickname: str, is_private: bool = None
+        self, nickname: str, is_private: bool = None, access_token: str = None
     ) -> dict:
         """
 
         フォローを許可制に設定します
 
         """
-        return set_follow_permission_enabled(self, nickname, is_private)
+        return set_follow_permission_enabled(self, nickname, is_private, access_token)
 
-    def take_action_follow_request(self, target_id: int, action: str) -> dict:
-        return take_action_follow_request(self, target_id, action)
+    def take_action_follow_request(
+        self, target_id: int, action: str, access_token: str = None
+    ) -> dict:
+        return take_action_follow_request(self, target_id, action, access_token)
 
-    def turn_on_hima(self) -> dict:
+    def turn_on_hima(self, access_token: str = None) -> dict:
         """
 
         ひまなう
 
         """
-        return turn_on_hima(self)
+        return turn_on_hima(self, access_token)
 
-    def unfollow_user(self, user_id: int) -> dict:
+    def unfollow_user(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ユーザーをアンフォローします
 
         """
-        return unfollow_user(self, user_id)
+        return unfollow_user(self, user_id, access_token)
 
     def update_user(
         self,
         nickname: str,
         biography: str = None,
         prefecture: str = None,
         gender: int = None,
         country_code: str = None,
         profile_icon_filename: str = None,
         cover_image_filename: str = None,
         username: str = None,
+        access_token: str = None,
     ) -> dict:
         """
 
         プロフィールを更新します
 
         """
         return update_user(
@@ -2537,70 +3119,75 @@
             biography,
             prefecture,
             gender,
             country_code,
             profile_icon_filename,
             cover_image_filename,
             username,
+            access_token,
         )
 
-    def block_user(self, user_id: int) -> dict:
+    def block_user(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ユーザーをブロックします
 
         """
-        return block_user(self, user_id)
+        return block_user(self, user_id, access_token)
 
-    def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
+    def get_blocked_user_ids(self, access_token: str = None) -> BlockedUserIdsResponse:
         """
 
         あなたをブロックしたユーザーを取得します
 
         """
-        return get_blocked_user_ids(self)
+        return get_blocked_user_ids(self, access_token)
 
-    def get_blocked_users(self, from_id: int = None) -> BlockedUsersResponse:
+    def get_blocked_users(
+        self, from_id: int = None, access_token: str = None
+    ) -> BlockedUsersResponse:
         """
 
         ブロックしたユーザーを取得します
 
         """
-        return get_blocked_users(self, from_id)
+        return get_blocked_users(self, from_id, access_token)
 
-    def unblock_user(self, user_id: int) -> dict:
+    def unblock_user(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ユーザーをアンブロックします
 
         """
-        return unblock_user(self, user_id)
+        return unblock_user(self, user_id, access_token)
 
-    def get_hidden_users_list(self, **params: Union[str, int]) -> HiddenResponse:
+    def get_hidden_users_list(
+        self, access_token: str = None, **params: Union[str, int]
+    ) -> HiddenResponse:
         """
 
         非表示のユーザー一覧を取得します
 
         Parameters
         ----------
 
             - from: str = None
             - number: int = None
 
         """
-        return get_hidden_users_list(self, **params)
+        return get_hidden_users_list(self, access_token, **params)
 
-    def hide_user(self, user_id: int) -> dict:
+    def hide_user(self, user_id: int, access_token: str = None) -> dict:
         """
 
         ユーザーを非表示にします
 
         """
-        return hide_user(self, user_id)
+        return hide_user(self, user_id, access_token)
 
-    def unhide_users(self, user_ids: List[int]) -> dict:
+    def unhide_users(self, user_ids: List[int], access_token: str = None) -> dict:
         """
 
         ユーザーの非表示を解除します
 
         """
-        return unhide_users(self, user_ids)
+        return unhide_users(self, user_ids, access_token)
```

### Comparing `yaylib-0.1.5/yaylib/config.py` & `yaylib-1.0.0/yaylib/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,36 @@
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "0.1.5"
+    YAYLIB_VERSION = "1.0.0"
     YAY_API_VERSION = "3.16"
     YAY_VERSION_NAME = "3.16.1"
     YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
```

### Comparing `yaylib-0.1.5/yaylib/models.py` & `yaylib-1.0.0/yaylib/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 from .utils import parse_datetime
 
 
 class Activity:
     __slots__ = (
         "data",
         "id",
```

### Comparing `yaylib-0.1.5/yaylib/responses.py` & `yaylib-1.0.0/yaylib/responses.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,96 @@
-from .models import *
+"""
+MIT License
+
+Copyright (c) 2023-present Qvco, Konn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from .models import (
+    Activity,
+    BanWord,
+    Bgm,
+    CallGiftHistory,
+    ChatRoom,
+    ChatRoomDraft,
+    Choice,
+    CoinAmount,
+    CoinExpiration,
+    CoinProduct,
+    CoinProductQuota,
+    ConferenceCall,
+    ConferenceCallUserRole,
+    ContactStatus,
+    CreateGroupQuota,
+    TimelineSettings,
+    Error,
+    Footprint,
+    Game,
+    Genre,
+    GifImage,
+    GifImageCategory,
+    Gift,
+    GiftCount,
+    GiftHistory,
+    GiftingAbility,
+    Group,
+    GroupCategory,
+    GroupGiftHistory,
+    GroupUser,
+    HiddenRecommendedPost,
+    Interest,
+    Message,
+    MessageTag,
+    MuteKeyword,
+    PlatformDetails,
+    PopularWord,
+    Post,
+    PostGift,
+    PostTag,
+    PresignedUrl,
+    Promotion,
+    ReceivedGift,
+    RecentSearch,
+    RefreshCounterRequest,
+    Review,
+    SearchCriteria,
+    Setting,
+    Settings,
+    Shareable,
+    SharedUrl,
+    SnsInfo,
+    Sticker,
+    StickerPack,
+    Survey,
+    ThreadInfo,
+    User,
+    UserAuth,
+    UserWrapper,
+    Video,
+    Walkthrough,
+    WalletTransaction,
+)
+from .utils import parse_datetime
 
 
 class ActiveFollowingsResponse:
     __slots__ = ("data", "last_loggedin_at", "users")
 
     def __init__(self, data):
         self.data = data
```

### Comparing `yaylib-0.1.5/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: yaylib
-Version: 0.1.5
-Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
-Home-page: https://github.com/qvco/yaylib
-Download-URL: https://github.com/qvco/yaylib
-Author: Qvco, Konn
-Author-email: nikola.desuga@gmail.com
-Maintainer: Qvco, Konn
-Maintainer-email: nikola.desuga@gmail.com
-License: MIT
-Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div><a id="readme-top"></a></div>
 <div align="center">
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
@@ -31,15 +13,15 @@
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
         あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
-            <strong>詳しい機能の詳細や使い方はこちらから »</strong>
+            <strong>ドキュメントはこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
         ·
@@ -48,46 +30,40 @@
 </p>
 
 <!-- TABLE OF CONTENTS -->
 
 <details>
   <summary>Table of Contents</summary>
   <ol>
+    <li><a href="#-installation">インストール</a></li>
+    <li><a href="#-quick-example">使用例</a></li>
+    <li><a href="#crown-yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
     <li><a href="#buy-me-a-coffee">Buy me a coffee</a></li>
-    <li><a href="#インストール">インストール</a></li>
-    <li><a href="#使用例">使用例</a></li>
-    <li><a href="#yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
-    <li><a href="#共同開発について">共同開発について</a></li>
+    <li><a href="#handshake-共同開発について">共同開発について</a></li>
     <li><a href="#免責事項">免責事項</a></li>
     <li><a href="#利用許諾">利用許諾</a></li>
   </ol>
 </details>
 
-<!-- Buy me a coffee -->
-
-## Buy me a coffee
-
-このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
-また、Buy Me a Coffee からご支援いただけますと幸いです。
-
-<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
-
 <!-- インストール -->
 
-## インストール
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-11d24c8c142b" width="30" height="30" />](https://github.com/qvco) Installation
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
 「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
-開発バージョンをインストールするには、以下の手順を実行します:
+<br>
+
+> **Note**
+> 開発バージョンをインストールする場合は、以下の手順を実行します:
 
 ```bash
 git clone https://github.com/qvco/yaylib
 
 cd yaylib
 
 pip install -r requirements.txt
@@ -95,42 +71,125 @@
 pip install -e .
 ```
 
 「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
-## 使用例
+## [<img src="https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-3994884d2ba3" width="30" height="30" />](https://github.com/qvco) Quick Example
 
-メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
+#### ✨ 投稿を作成する
 
 ```python
 import yaylib
 
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!")
+```
+
+#### ✨ 埋め込みリンクの投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", shared_url="https://github.com/qvco/yaylib")
+```
+
+<p align="center">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/44aa5df8-4654-4f8d-a73f-79d530b8a0e1" alt="Writing Text Threads" width="400px" />
+</p>
+
+#### ✨ 画像と一緒に投稿を作成する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+filename = api.upload_image(
+    image_type="post", # 画像の使い道を指定
+    image_path="./path/to/image" # ローカルにある画像のパス
+)
+
+api.create_post("Hello with yaylib!", attachment_filename=filename)
+```
+
+#### ✨ 投稿に返信する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+api.create_post("Hello with yaylib!", in_reply_to=373189088)
+```
+
+#### ✨ タイムラインを 100 件取得する
+
+```python
+import yaylib
+
+api = yaylib.Client()
+
+timeline = api.get_timeline(number=100)
+
+for post in timeline.posts:
+    print(post.user.nickname)  # 投稿者
+    print(post.text)  # 本文
+    print(post.likes_count)  # いいね数
+    print(post.reposts_count)  # (´∀｀∩)↑age↑の数
+    print(post.in_reply_to_post_count)  # 返信の数
+```
+
+#### ✨ タイムラインをキーワードで検索して「いいね」する
+
+```python
+import yaylib
 
 api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_post(post.id)
+    response = api.like_posts(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
+#### ✨ タイムラインのユーザーをフォローする
+
+```python
+import yaylib
+
+api = yaylib.Client()
+api.login(email="メールアドレス", password="パスワード")
+
+timeline = api.get_timeline(number=15)
+
+for post in timeline.posts:
+    api.follow_user(post.user.id)
+```
+
 より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
-## yaylib で誕生したロボットたち
+## :crown: yaylib で誕生したロボットたち
 
 「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
@@ -157,31 +216,50 @@
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
-## 共同開発について
+## :handshake: 共同開発について
 
-私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
+私たちと開発することに興味を持っていただけているなら、ぜひ参加して頂きたいです！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
-- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
+- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com にメールを送信する</a>
+
+のいずれかの方法で繋がりましょう。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
+<!-- Buy me a coffee -->
+
+## Buy me a coffee
+
+このライブラリが気に入っていただけたら、**リポジトリに<a href="https://github.com/qvco/yaylib/">スターをお願いします</a>(⭐)**  
+また、Buy Me a Coffee からご支援いただけますと幸いです。
+
+<a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
-<!-- 利用許諾 -->
+<!-- ライセンス -->
+
+## ライセンス
 
-## 利用許諾
+<p align="center">
+  <a href="https://github.com/qvco">
+    <img src="https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-791308b393af" width="256" height="256">
+  </a>
+</p>
+
+<p align="center">
+  <strong>MIT © <a href="https://github.com/qvco">Qvco</a> & <a href="https://github.com/konn-koko">Konn</a></strong>
+</p>
 
 フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,80 +1,101 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.5 Summary: This Python package
-provides an easy-to-use interface for accessing data from Yay! (https://
-yay.space/). With this API Client, you can retrieve user profiles, posts,
-comments, and other content from Yay!, as well as perform common tasks like
-liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
-Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
-nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
-nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
                                     [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
                            API ã©ããã¼ã§ãã
    ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
-          è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
+                   ãã­ã¥ã¡ã³ãã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
-   1. Buy_me_a_coffee
-   2. ã¤ã³ã¹ãã¼ã«
-   3. ä½¿ç¨ä¾
-   4. yaylib_ã§èªçããã­ããããã¡
+   1. ã¤ã³ã¹ãã¼ã«
+   2. ä½¿ç¨ä¾
+   3. yaylib_ã§èªçããã­ããããã¡
+   4. Buy_me_a_coffee
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
-  ## Buy me a coffee
-ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
-â­ï¸ ã¾ããBuy Me a Coffee
-ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
-ã¤ã³ã¹ãã¼ã« **â» Python 3.11
+  ## [[https://github.com/qvco/yaylib/assets/77382767/2f632349-0cbc-4c81-bc19-
+11d24c8c142b]](https://github.com/qvco) Installation **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
-éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
+> **Note** >
+éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããå ´åã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
-ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## [
+[https://github.com/qvco/yaylib/assets/77382767/dc7dcea0-c581-4039-8fc2-
+3994884d2ba3]](https://github.com/qvco) Quick Example #### â¨
+æç¨¿ãä½æãã ```python import yaylib api = yaylib.Client() api.login
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
+("Hello with yaylib!") ``` #### â¨
+åãè¾¼ã¿ãªã³ã¯ã®æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+shared_url="https://github.com/qvco/yaylib") ```
+                            [Writing Text Threads]
+#### â¨ ç»åã¨ä¸ç·ã«æç¨¿ãä½æãã ```python import yaylib api =
+yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") filename = api.upload_image( image_type="post", #
+ç»åã®ä½¿ãéãæå® image_path="./path/to/image" #
+ã­ã¼ã«ã«ã«ããç»åã®ãã¹ ) api.create_post("Hello with yaylib!",
+attachment_filename=filename) ``` #### â¨ æç¨¿ã«è¿ä¿¡ãã ```python
+import yaylib api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") api.create_post("Hello with yaylib!",
+in_reply_to=373189088) ``` #### â¨ ã¿ã¤ã ã©ã¤ã³ã 100 ä»¶åå¾ãã
+```python import yaylib api = yaylib.Client() timeline = api.get_timeline
+(number=100) for post in timeline.posts: print(post.user.nickname) # æç¨¿è
+print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
+(post.reposts_count) # (Â´âï½â©)âageâã®æ° print
+(post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_post(post.id) print(post.id,
-response.data) # å®è¡çµæãåºå ```
+post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ``` #### â¨
+ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
+api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
+password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
+timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡
+ ## :crown: yaylib ã§èªçããã­ããããã¡
 ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
 MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
  [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
       cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
             éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
                                                                                                                                  éçºè: ãºãã¼
- ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
-- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
-ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
-ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
+ ## :handshake: å±åéçºã«ã¤ãã¦
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦é ãããã§ãï¼
+- ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã -
+nikola.desuga@gmail.com_ã«ã¡ã¼ã«ãéä¿¡ãã
+ã®ããããã®æ¹æ³ã§ç¹ããã¾ããããè©³ããã¯
 [ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
-CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
+CONTRIBUTING.md)ï¼  ## Buy me a coffee
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããã**ãªãã¸ããªã«ã¹ã¿ã¼ããé¡ããã¾ã
+(â­)** ã¾ããBuy Me a Coffee
+ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
+åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
-## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
+## ã©ã¤ã»ã³ã¹
+   [https://github.com/qvco/yaylib/assets/77382767/5d6aef18-5d98-4c9b-9f54-
+                                 791308b393af]
+                              MIT Â© Qvco & Konn
+ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/yaylib/blob/
+master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.5/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.0/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

