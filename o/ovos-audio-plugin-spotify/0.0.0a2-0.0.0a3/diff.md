# Comparing `tmp/ovos_audio_plugin_spotify-0.0.0a2-py3-none-any.whl.zip` & `tmp/ovos_audio_plugin_spotify-0.0.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14087 bytes, number of entries: 9
--rw-r--r--  2.0 unx     3269 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify/__init__.py
--rw-r--r--  2.0 unx    28562 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify/spotify_client.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      179 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      889 b- defN 23-Jun-12 13:48 ovos_audio_plugin_spotify-0.0.0a2.dist-info/RECORD
-9 files, 44930 bytes uncompressed, 12511 bytes compressed:  72.2%
+Zip file size: 14135 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     3269 b- defN 23-Jul-16 18:20 ovos_audio_plugin_spotify/__init__.py
+-rw-r--r--  2.0 unx    28658 b- defN 23-Jul-16 18:20 ovos_audio_plugin_spotify/spotify_client.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      179 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      889 b- defN 23-Jul-16 18:21 ovos_audio_plugin_spotify-0.0.0a3.dist-info/RECORD
+9 files, 45026 bytes uncompressed, 12559 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: ovos_audio_plugin_spotify/spotify_client.py
 Comment: 
 
 Filename: ovos_audio_plugin_spotify/version.py
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/LICENSE
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/METADATA
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/WHEEL
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/entry_points.txt
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/top_level.txt
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a2.dist-info/RECORD
+Filename: ovos_audio_plugin_spotify-0.0.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_audio_plugin_spotify/spotify_client.py

```diff
@@ -1,12 +1,15 @@
 import re
 import time
 
 import requests
 import spotipy
+
+from functools import wraps
+
 from ovos_backend_client.api import OAuthApi, DeviceApi
 from ovos_utils import flatten_list
 from ovos_utils.log import LOG
 from ovos_utils.parse import match_one, fuzzy_match
 from requests.exceptions import HTTPError
 from spotipy.oauth2 import SpotifyAuthBase
 
@@ -22,14 +25,15 @@
 class PlaylistNotFoundError(Exception):
     pass
 
 
 class SpotifyNotAuthorizedError(Exception):
     pass
 
+OAUTH_TOKEN_ID = "audioplugin_spotify"
 
 class OVOSSpotifyCredentials(SpotifyAuthBase):
     """ Oauth through ovos-backend-client"""
 
     def __init__(self):
         super().__init__(requests.Session())
         self.access_token = None
@@ -38,38 +42,39 @@
 
     @staticmethod
     def get_token():
         """ Get token with a single retry."""
         retry = False
         d = None
         try:
-            d = OAuthApi().get_oauth_token("spotify")
+            d = OAuthApi().get_oauth_token(OAUTH_TOKEN_ID)
         except HTTPError as e:
             if e.response.status_code == 404:  # Token doesn't exist
                 raise SpotifyNotAuthorizedError
             if e.response.status_code == 401:  # Device isn't paired
                 raise SpotifyNotAuthorizedError
             else:
                 retry = True
         if retry:
-            d = OAuthApi().get_oauth_token("spotify")
+            d = OAuthApi().get_oauth_token(OAUTH_TOKEN_ID)
         if not d:
             raise SpotifyNotAuthorizedError
         return d
 
     def get_access_token(self, force=False):
         if (not self.access_token or time.time() > self.expiration_time or force):
             d = self.get_token()
             self.access_token = d['access_token']
             # get expiration time from message, if missing assume 1 hour
             self.expiration_time = d.get('expiration') or time.time() + 3600
         return self.access_token
 
 
 def refresh_spotify_oauth(func):
+    @wraps(func)
     def wrapper(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
         except HTTPError as e:
             if e.response.status_code == 401:
                 self.client_credentials_manager.get_access_token(force=True)
                 return func(self, *args, **kwargs)
```

## ovos_audio_plugin_spotify/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_audio_plugin_spotify-0.0.0a2.dist-info/LICENSE` & `ovos_audio_plugin_spotify-0.0.0a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_audio_plugin_spotify-0.0.0a2.dist-info/RECORD` & `ovos_audio_plugin_spotify-0.0.0a3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ovos_audio_plugin_spotify/__init__.py,sha256=P9uz5VKUhgtQzxdqkjC5rzRyTqimmOozszpEUGuDUWQ,3269
-ovos_audio_plugin_spotify/spotify_client.py,sha256=GqL7ig4mDFkuUTUKBCQz1s46gG6yZK83TflLOLf11I0,28562
-ovos_audio_plugin_spotify/version.py,sha256=qbOVTdDXh7dwDi60rr2DZTzYPxPV2NRmIEkMGRkodnk,177
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/LICENSE,sha256=ntGHfW0JQ281uH6ycFGfAyFMCThkNAUM3r6HS2aPXA0,11349
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/METADATA,sha256=6IUdl399vaGbshhWwMbfmHA8PTqPrUR8azTQSiZr-r4,387
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/entry_points.txt,sha256=eRqnpnbjSvjP2gy6-F4y1bj6PxZdk9bSuDQMZCg9YSo,179
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/top_level.txt,sha256=61lSsvrOmPf1COig3R9LzTT5MQHYWehvB45eUgCNIZQ,26
-ovos_audio_plugin_spotify-0.0.0a2.dist-info/RECORD,,
+ovos_audio_plugin_spotify/spotify_client.py,sha256=utk8lcrV3Jwx4wbmmu5uZry70V22_bqGDwNnXqM19qk,28658
+ovos_audio_plugin_spotify/version.py,sha256=mdTwoA3M5jrv1DgpMMdhUkhzeydBmSNmT4F8k_15_Ug,177
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/LICENSE,sha256=ntGHfW0JQ281uH6ycFGfAyFMCThkNAUM3r6HS2aPXA0,11349
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/METADATA,sha256=bNib-76i_pdHplqd7nwuaR3movwlAChlVIz2fdeYq3Q,387
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/entry_points.txt,sha256=eRqnpnbjSvjP2gy6-F4y1bj6PxZdk9bSuDQMZCg9YSo,179
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/top_level.txt,sha256=61lSsvrOmPf1COig3R9LzTT5MQHYWehvB45eUgCNIZQ,26
+ovos_audio_plugin_spotify-0.0.0a3.dist-info/RECORD,,
```

