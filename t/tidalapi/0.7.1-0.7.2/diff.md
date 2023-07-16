# Comparing `tmp/tidalapi-0.7.1.tar.gz` & `tmp/tidalapi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidalapi-0.7.1.tar", last modified: Mon May 22 20:27:54 2023, max compression
+gzip compressed data, was "tidalapi-0.7.2.tar", max compression
```

## Comparing `tidalapi-0.7.1.tar` & `tidalapi-0.7.2.tar`

### file list

```diff
@@ -1,50 +1,17 @@
-drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3554 2023-05-22 20:27:42.000000 tidalapi-0.7.1/HISTORY.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     7651 2023-05-21 21:11:51.000000 tidalapi-0.7.1/LICENSE
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      199 2023-05-21 21:11:51.000000 tidalapi-0.7.1/MANIFEST.in
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5548 2023-05-22 20:27:54.796436 tidalapi-0.7.1/PKG-INFO
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1158 2023-05-22 20:09:13.000000 tidalapi-0.7.1/README.rst
-drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.792436 tidalapi-0.7.1/docs/
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2450 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/api.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2464 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/conf.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      387 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/config.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       12 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/genindex.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       27 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/history.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      262 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/index.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2201 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/login.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      890 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/migration.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2537 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/pages.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1035 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/playlist.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       26 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/py-modindex.rst
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      155 2023-05-22 20:27:54.796436 tidalapi-0.7.1/setup.cfg
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1458 2023-05-22 19:50:46.000000 tidalapi-0.7.1/setup.py
-drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tests/
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        0 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/__init__.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3306 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/conftest.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2880 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/cover.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3499 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_album.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4356 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_artist.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1839 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_genres.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5749 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_media.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3843 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_page.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4982 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_playlist.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4249 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_session.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     6716 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_user.py
-drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tidalapi/
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      464 2023-05-22 20:08:43.000000 tidalapi-0.7.1/tidalapi/__init__.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     7470 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/album.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     6600 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/artist.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2405 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/genre.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     8535 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/media.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3472 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/mix.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    11356 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/page.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     8474 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/playlist.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5986 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/request.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    25114 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/session.py
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    11906 2023-05-22 19:46:49.000000 tidalapi-0.7.1/tidalapi/user.py
-drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tidalapi.egg-info/
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5548 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/PKG-INFO
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      821 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/SOURCES.txt
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        1 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/dependency_links.txt
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       25 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/requires.txt
--rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        9 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/top_level.txt
+-rw-r--r--   0        0        0     4575 2023-07-16 21:14:51.014704 tidalapi-0.7.2/HISTORY.rst
+-rw-r--r--   0        0        0     7651 2023-05-21 21:11:51.414585 tidalapi-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1468 2023-07-12 20:29:27.927285 tidalapi-0.7.2/README.rst
+-rw-r--r--   0        0        0     1499 2023-07-16 20:49:53.950754 tidalapi-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-07-16 20:49:53.950754 tidalapi-0.7.2/tidalapi/__init__.py
+-rw-r--r--   0        0        0     9094 2023-07-16 21:02:11.835122 tidalapi-0.7.2/tidalapi/album.py
+-rw-r--r--   0        0        0     6797 2023-07-16 21:02:11.847122 tidalapi-0.7.2/tidalapi/artist.py
+-rw-r--r--   0        0        0     2724 2023-07-12 20:29:27.931287 tidalapi-0.7.2/tidalapi/genre.py
+-rw-r--r--   0        0        0    11867 2023-07-16 21:02:11.871122 tidalapi-0.7.2/tidalapi/media.py
+-rw-r--r--   0        0        0     4994 2023-07-16 21:02:11.879122 tidalapi-0.7.2/tidalapi/mix.py
+-rw-r--r--   0        0        0    12188 2023-07-16 21:02:11.899122 tidalapi-0.7.2/tidalapi/page.py
+-rw-r--r--   0        0        0     9183 2023-07-16 21:02:11.911122 tidalapi-0.7.2/tidalapi/playlist.py
+-rw-r--r--   0        0        0     6018 2023-07-16 20:49:47.082821 tidalapi-0.7.2/tidalapi/request.py
+-rw-r--r--   0        0        0    26313 2023-07-12 20:29:27.931287 tidalapi-0.7.2/tidalapi/session.py
+-rw-r--r--   0        0        0       55 2023-07-12 20:29:27.931287 tidalapi-0.7.2/tidalapi/types.py
+-rw-r--r--   0        0        0    11742 2023-07-12 20:29:27.931287 tidalapi-0.7.2/tidalapi/user.py
+-rw-r--r--   0        0        0     7148 1970-01-01 00:00:00.000000 tidalapi-0.7.2/PKG-INFO
```

### Comparing `tidalapi-0.7.1/LICENSE` & `tidalapi-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.1/PKG-INFO` & `tidalapi-0.7.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: tidalapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Unofficial API for TIDAL music streaming service.
-Home-page: https://github.com/tamland/python-tidal
+Home-page: https://tidalapi.netlify.app
+License: LGPL-3.0-or-later
 Author: Thomas Amland
 Author-email: thomas.amland@googlemail.com
 Maintainer: tehkillerbee
 Maintainer-email: josaksel.dk@gmail.com
-License: LGPL
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://tidalapi.netlify.app
+Project-URL: Repository, https://github.com/tamland/python-tidal
+Description-Content-Type: text/x-rst
 
 tidalapi
 ========
 
 .. image:: https://img.shields.io/pypi/v/tidalapi.svg
     :target: https://pypi.org/project/tidalapi
 
 .. image:: https://api.netlify.com/api/v1/badges/f05c0752-4565-4940-90df-d2b3fe91c84b/deploy-status
     :target: https://tidalapi.netlify.com/
 
 Unofficial Python API for TIDAL music streaming service.
 
+Requires Python 3.7 or higher.
 
 0.7.0 Rewrite
 -------------
 
 The 0.7.0 rewrite is now complete, see the `migration guide <https://tidalapi.netlify.app/migration.html#migrating-from-0-6-x-0-7-x>`_ for dealing with it
 
 Installation
@@ -67,20 +72,45 @@
 
 
 Documentation
 -------------
 
 Documentation is available at https://tidalapi.netlify.app/
 
+Development
+-----------
 
+This project uses poetry for dependency management and packaging. To install dependencies and setup the project for development, run:
 
+.. code-block:: bash
+    
+        $ pip install pipx
+        $ pipx install poetry
+        $ poetry install --no-root
+
+.. :changelog:
 
 History
 =======
 
+v0.7.2
+------
+* (BREAKING!) Drop support for python3.8 and older
+* Improved tests - 2e0byo_
+* Add type to album object - jozefKruszynski_
+* Add mix images and tests - jozefKruszynski_
+* Add mypy and fix immediate typing errors - arusahni_
+* New attribute to media.Track() class: 'full_name' - WilliamGuisan_
+* Fix Track.stream() method - ssnailed_
+* Fixed key error for gender when parsing user json - mkaufhol_
+* Drop (almost) all user data we don't use. - 2e0byo_
+* Add typing for media, genres, mixes, and albums - arusahni_
+* Replace TypedDict and NamedTuple with dataclasses - arusahni_
+* Fix circular Imports and Typing - PretzelVector_
+
 v0.7.1
 ------
 * Quick fix for "got key error 'picture'" error. - BlackLight_
 * Bring back Radio support - bjesus_
 * Added function for multiple deletions at once bloedboemmel_
 * Use UTC instead of local time for expiry_time lutzbuerkle_
 
@@ -169,7 +199,19 @@
 .. _1nikolas: https://github.com/1nikolas
 .. _divadsn: https://github.com/divadsn
 .. _BlackLight: https://github.com/BlackLight
 .. _lutzbuerkle: https://github.com/lutzbuerkle
 .. _retired-guy: https://github.com/retired-guy
 .. _bjesus: https://github.com/bjesus
 .. _bloedboemmel: https://github.com/bloedboemmel
+.. _2e0byo: https://github.com/2e0byo
+.. _jozefKruszynski: https://github.com/jozefKruszynski
+.. _arusahni: https://github.com/arusahni
+.. _WilliamGuisan: https://github.com/WilliamGuisan
+.. _ssnailed: https://github.com/ssnailed
+.. _mkaufhol: https://github.com/mkaufhol
+.. _PretzelVector: https://github.com/PretzelVector
+.. _tehkillerbee: https://github.com/tehkillerbee
+
+
+
+
```

### Comparing `tidalapi-0.7.1/tidalapi/album.py` & `tidalapi-0.7.2/tidalapi/album.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,194 +13,238 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
+from datetime import datetime
+from typing import TYPE_CHECKING, List, Optional, Union, cast
+
 import dateutil.parser
 
-DEFAULT_ALBUM_IMAGE = "https://tidal.com/browse/assets/images/defaultImages/defaultAlbumImage.png"
+from tidalapi.types import JsonObj
 
+if TYPE_CHECKING:
+    from tidalapi.artist import Artist
+    from tidalapi.media import Track, Video
+    from tidalapi.page import Page
+    from tidalapi.session import Session
 
-class Album(object):
-    """
-    Contains information about a TIDAL album.
+DEFAULT_ALBUM_IMAGE = (
+    "https://tidal.com/browse/assets/images/defaultImages/defaultAlbumImage.png"
+)
 
-    If the album is created from a media object, this object will only contain
-    the id, name, cover and video cover. TIDAL does this to reduce the network load.
 
+class Album:
+    """Contains information about a TIDAL album.
+
+    If the album is created from a media object, this object will only contain the id,
+    name, cover and video cover. TIDAL does this to reduce the network load.
     """
-    id = None
-    name = None
+
+    id: Optional[str] = None
+    name: Optional[str] = None
     cover = None
     video_cover = None
+    type = None
 
-    duration = -1
-    available = False
-    num_tracks = -1
-    num_videos = -1
-    num_volumes = -1
-    tidal_release_date = None
-    release_date = None
+    duration: Optional[int] = -1
+    available: Optional[bool] = False
+    num_tracks: Optional[int] = -1
+    num_videos: Optional[int] = -1
+    num_volumes: Optional[int] = -1
+    tidal_release_date: Optional[datetime] = None
+    release_date: Optional[datetime] = None
     copyright = None
     version = None
-    explicit = True
-    universal_product_number = -1
-    popularity = -1
-    user_date_added = None
+    explicit: Optional[bool] = True
+    universal_product_number: Optional[int] = -1
+    popularity: Optional[int] = -1
+    user_date_added: Optional[datetime] = None
 
-    artist = None
-    artists = None
+    artist: Optional["Artist"] = None
+    artists: Optional[List["Artist"]] = None
 
-    def __init__(self, session, album_id):
+    def __init__(self, session: "Session", album_id: Optional[str]):
         self.session = session
         self.requests = session.request
         self.artist = session.artist()
         self.id = album_id
-        if album_id:
-            self.requests.map_request('albums/%s' % album_id, parse=self.parse)
+        if self.id:
+            self.requests.map_request(f"albums/{album_id}", parse=self.parse)
 
-    def parse(self, json_obj, artist=None, artists=None):
+    def parse(
+        self,
+        json_obj: JsonObj,
+        artist: Optional["Artist"] = None,
+        artists: Optional[List["Artist"]] = None,
+    ) -> "Album":
         if artists is None:
-            artists = self.session.parse_artists(json_obj['artists'])
+            artists = self.session.parse_artists(json_obj["artists"])
 
         # Sometimes the artist field is not filled, an example is 140196345
-        if not 'artist' in json_obj:
+        if "artist" not in json_obj:
             artist = artists[0]
         elif artist is None:
-            artist = self.session.parse_artist(json_obj['artist'])
+            artist = self.session.parse_artist(json_obj["artist"])
 
-        self.id = json_obj['id']
-        self.name = json_obj['title']
-        self.cover = json_obj['cover']
-        self.video_cover = json_obj['videoCover']
-
-        self.duration = json_obj.get('duration')
-        self.available = json_obj.get('streamReady')
-        self.num_tracks = json_obj.get('numberOfTracks')
-        self.num_videos = json_obj.get('numberOfVideos')
-        self.num_volumes = json_obj.get('numberOfVolumes')
-        self.copyright = json_obj.get('copyright')
-        self.version = json_obj.get('version')
-        self.explicit = json_obj.get('explicit')
-        self.universal_product_number = json_obj.get('upc')
-        self.popularity = json_obj.get('popularity')
+        self.id = json_obj["id"]
+        self.name = json_obj["title"]
+        self.cover = json_obj["cover"]
+        self.video_cover = json_obj["videoCover"]
+        self.duration = json_obj.get("duration")
+        self.available = json_obj.get("streamReady")
+        self.num_tracks = json_obj.get("numberOfTracks")
+        self.num_videos = json_obj.get("numberOfVideos")
+        self.num_volumes = json_obj.get("numberOfVolumes")
+        self.copyright = json_obj.get("copyright")
+        self.version = json_obj.get("version")
+        self.explicit = json_obj.get("explicit")
+        self.universal_product_number = json_obj.get("upc")
+        self.popularity = json_obj.get("popularity")
+        self.type = json_obj.get("type")
 
         self.artist = artist
         self.artists = artists
 
-        release_date = json_obj.get('releaseDate')
-        self.release_date = dateutil.parser.isoparse(release_date) if release_date else None
-
-        tidal_release_date = json_obj.get('streamStartDate')
-        self.tidal_release_date = dateutil.parser.isoparse(tidal_release_date) if tidal_release_date else None
-
-        user_date_added = json_obj.get('dateAdded')
-        self.user_date_added = dateutil.parser.isoparse(user_date_added) if user_date_added else None
+        release_date = json_obj.get("releaseDate")
+        self.release_date = (
+            dateutil.parser.isoparse(release_date) if release_date else None
+        )
+
+        tidal_release_date = json_obj.get("streamStartDate")
+        self.tidal_release_date = (
+            dateutil.parser.isoparse(tidal_release_date) if tidal_release_date else None
+        )
+
+        user_date_added = json_obj.get("dateAdded")
+        self.user_date_added = (
+            dateutil.parser.isoparse(user_date_added) if user_date_added else None
+        )
 
         return copy.copy(self)
 
     @property
-    def year(self):
-        """
-        Convenience function to get the year using :class:`available_release_date`
+    def year(self) -> Optional[int]:
+        """Convenience function to get the year using :class:`available_release_date`
 
         :return: An :any:`python:int` containing the year the track was released
         """
         return self.available_release_date.year if self.available_release_date else None
 
     @property
-    def available_release_date(self):
-        """
-        Get the release date if it's available, otherwise get the day it was released on TIDAL
+    def available_release_date(self) -> Optional[datetime]:
+        """Get the release date if it's available, otherwise get the day it was released
+        on TIDAL.
 
-        :return: A :any:`python:datetime.datetime` object with the release date, or the tidal release date, can be None
+        :return: A :any:`python:datetime.datetime` object with the release date, or the
+            tidal release date, can be None
         """
         if self.release_date:
             return self.release_date
         if self.tidal_release_date:
             return self.tidal_release_date
         return None
 
-    def tracks(self, limit=None, offset=0):
-        """
-        Returns the tracks in classes album.
+    def tracks(self, limit: Optional[int] = None, offset: int = 0) -> List["Track"]:
+        """Returns the tracks in classes album.
 
         :param limit: The amount of items you want returned.
         :param offset: The position of the first item you want to include.
         :return: A list of the :class:`Tracks <.Track>` in the album.
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.requests.map_request('albums/%s/tracks' % self.id, params, parse=self.session.parse_track)
+        params = {"limit": limit, "offset": offset}
+        tracks = self.requests.map_request(
+            "albums/%s/tracks" % self.id, params, parse=self.session.parse_track
+        )
+        assert isinstance(tracks, list)
+        return cast(List["Track"], tracks)
 
-    def items(self, limit=100, offset=0):
-        """
-        Gets the first 100 tracks and videos in the album from TIDAL.
+    def items(self, limit: int = 100, offset: int = 0) -> List[Union["Track", "Video"]]:
+        """Gets the first 'limit' tracks and videos in the album from TIDAL.
 
+        :param limit: The number of items you want to retrieve
         :param offset: The index you want to start retrieving items from
         :return: A list of :class:`Tracks<.Track>` and :class:`Videos`<.Video>`
         """
-        params = {'offset': offset, 'limit': limit}
-        return self.requests.map_request('albums/%s/items' % self.id, params=params, parse=self.session.parse_media)
+        params = {"offset": offset, "limit": limit}
+        items = self.requests.map_request(
+            "albums/%s/items" % self.id, params=params, parse=self.session.parse_media
+        )
+        assert isinstance(items, list)
+        return cast(List[Union["Track", "Video"]], items)
 
-    def image(self, dimensions, default=DEFAULT_ALBUM_IMAGE):
-        """
-        A url to an album image cover
+    def image(self, dimensions: int, default: str = DEFAULT_ALBUM_IMAGE) -> str:
+        """A url to an album image cover.
 
         :param dimensions: The width and height that you want from the image
-        :type dimensions: int
+        :param default: An optional default image to serve if one is not available
         :return: A url to the image.
 
         Valid resolutions: 80x80, 160x160, 320x320, 640x640, 1280x1280
         """
         if not self.cover:
             return default
 
         if dimensions not in [80, 160, 320, 640, 1280]:
             raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
 
-        return self.session.config.image_url % (self.cover.replace('-', '/'), dimensions, dimensions)
+        return self.session.config.image_url % (
+            self.cover.replace("-", "/"),
+            dimensions,
+            dimensions,
+        )
 
-    def video(self, dimensions):
-        """
-        Creates a url to an mp4 video cover for the album.
+    def video(self, dimensions: int) -> str:
+        """Creates a url to an mp4 video cover for the album.
 
         Valid resolutions: 80x80, 160x160, 320x320, 640x640, 1280x1280
 
         :param dimensions: The width an height of the video
         :type dimensions: int
         :return: A url to an mp4 of the video cover.
         """
         if not self.video_cover:
             raise AttributeError("This album does not have a video cover.")
 
         if dimensions not in [80, 160, 320, 640, 1280]:
             raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
 
-        return self.session.config.video_url % (self.video_cover.replace('-', '/'), dimensions, dimensions)
+        return self.session.config.video_url % (
+            self.video_cover.replace("-", "/"),
+            dimensions,
+            dimensions,
+        )
 
-    def page(self):
+    def page(self) -> "Page":
         """
         Retrieve the album page as seen on https://listen.tidal.com/album/$id
 
         :return: A :class:`Page` containing the different categories, e.g. similar artists and albums
         """
-        return self.session.page.get("pages/album", params={"albumId": self.id})
+        page = self.session.page.get("pages/album", params={"albumId": self.id})
+        return cast("Page", page)
 
-    def similar(self):
-        """
-        Retrieve albums similar to the current one
+    def similar(self) -> List["Album"]:
+        """Retrieve albums similar to the current one.
 
         :return: A :any:`list` of similar albums
         """
-        return self.requests.map_request('albums/%s/similar' % self.id, parse=self.session.parse_album)
+        albums = self.requests.map_request(
+            "albums/%s/similar" % self.id, parse=self.session.parse_album
+        )
+        assert isinstance(albums, list)
+        return cast(List["Album"], albums)
 
     def review(self) -> str:
-        """
-        Retrieve the album review
+        """Retrieve the album review.
 
         :return: A :class:`str` containing the album review, with wimp links
         :raises: :class:`requests.HTTPError` if there isn't a review yet
         """
         # morguldir: TODO: Add parsing of wimplinks?
-        return self.requests.request('GET', 'albums/%s/review' % self.id).json()['text']
+        review = self.requests.request("GET", "albums/%s/review" % self.id).json()[
+            "text"
+        ]
+        assert isinstance(review, str)
+        return review
```

### Comparing `tidalapi-0.7.1/tidalapi/artist.py` & `tidalapi-0.7.2/tidalapi/artist.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,182 +11,190 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-A module containing information and functions related to TIDAL artists.
-"""
+"""A module containing information and functions related to TIDAL artists."""
 
 import copy
 from enum import Enum
+from typing import List
+
 import dateutil.parser
 
 IMG_URL = "http://images.osl.wimpmusic.com/im/im?w={width}&h={height}&{id_type}={id}"
 
 
 class Artist(object):
     id = None
     name = None
     roles = None
     role = None
     picture = None
     user_date_added = None
+    bio = None
 
     def __init__(self, session, artist_id):
         self.session = session
         self.request = self.session.request
         self.id = artist_id
         if artist_id:
-            self.request.map_request('artists/%s' % artist_id, parse=self.parse_artist)
+            self.request.map_request("artists/%s" % artist_id, parse=self.parse_artist)
 
-    def parse_artist(self, json_obj):
+    def parse_artist(self, json_obj) -> "Artist":
         """
 
         :param json_obj:
         :return:
         """
-        self.id = json_obj['id']
-        self.name = json_obj['name']
-
+        self.id = json_obj["id"]
+        self.name = json_obj["name"]
 
         # Artists do not have roles as playlist creators.
         self.roles = None
         self.role = None
-        if json_obj.get('type') or json_obj.get('artistTypes'):
+        if json_obj.get("type") or json_obj.get("artistTypes"):
             roles = []
-            for role in json_obj.get('artistTypes', [json_obj.get('type')]):
+            for role in json_obj.get("artistTypes", [json_obj.get("type")]):
                 roles.append(Role(role))
 
             self.roles = roles
             self.role = roles[0]
 
-        self.picture = json_obj.get('picture')
+        self.picture = json_obj.get("picture")
 
-        user_date_added = json_obj.get('dateAdded')
-        self.user_date_added = dateutil.parser.isoparse(user_date_added) if user_date_added else None
+        user_date_added = json_obj.get("dateAdded")
+        self.user_date_added = (
+            dateutil.parser.isoparse(user_date_added) if user_date_added else None
+        )
 
         return copy.copy(self)
 
-    def parse_artists(self, json_obj):
-        """
-        Parses a TIDAL artist, replaces the current artist object.
-        Made for use inside of the python tidalapi module.
+    def parse_artists(self, json_obj) -> List["Artist"]:
+        """Parses a TIDAL artist, replaces the current artist object. Made for use
+        inside of the python tidalapi module.
 
         :param json_obj: Json data returned from api.tidal.com containing an artist
-        :return: Returns a copy of the original :exc:'Artist': object
+        :return: Returns a copy of the original :exc: 'Artist': object
         """
         return list(map(self.parse_artist, json_obj))
 
     def _get_albums(self, params=None):
-        return self.request.map_request('artists/%s/albums' % self.id, params, parse=self.session.parse_album)
+        return self.request.map_request(
+            "artists/%s/albums" % self.id, params, parse=self.session.parse_album
+        )
 
     def get_albums(self, limit=None, offset=0):
-        """
-        Queries TIDAL for the artists albums.
+        """Queries TIDAL for the artists albums.
 
         :return: A list of :class:`Albums<tidalapi.album.Album>`
         """
-        params = {'limit': limit, 'offset': offset}
+        params = {"limit": limit, "offset": offset}
         return self._get_albums(params)
 
     def get_albums_ep_singles(self, limit=None, offset=0):
-        """
-        Queries TIDAL for the artists extended plays and singles.
+        """Queries TIDAL for the artists extended plays and singles.
 
         :return: A list of :class:`Albums <tidalapi.album.Album>`
         """
-        params = {'filter': 'EPSANDSINGLES', 'limit': limit, 'offset': offset}
+        params = {"filter": "EPSANDSINGLES", "limit": limit, "offset": offset}
         return self._get_albums(params)
 
     def get_albums_other(self, limit=None, offset=0):
-        """
-        Queries TIDAL for albums the artist has appeared on as a featured artist.
+        """Queries TIDAL for albums the artist has appeared on as a featured artist.
 
         :return: A list of :class:`Albums <tidalapi.album.Album>`
         """
-        params = {'filter': 'COMPILATIONS', 'limit': limit, 'offset': offset}
+        params = {"filter": "COMPILATIONS", "limit": limit, "offset": offset}
         return self._get_albums(params)
 
     def get_top_tracks(self, limit=None, offset=0):
-        """
-        Queries TIDAL for the artists tracks, sorted by popularity.
+        """Queries TIDAL for the artists tracks, sorted by popularity.
 
         :return: A list of :class:`Tracks <tidalapi.media.Track>`
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.request.map_request('artists/%s/toptracks' % self.id, params=params, parse=self.session.parse_track)
+        params = {"limit": limit, "offset": offset}
+        return self.request.map_request(
+            "artists/%s/toptracks" % self.id,
+            params=params,
+            parse=self.session.parse_track,
+        )
 
     def get_videos(self, limit=None, offset=0):
-        """
-        Queries tidal for the artists videos.
+        """Queries tidal for the artists videos.
 
         :return: A list of :class:`Videos <tidalapi.media.Video>`
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.request.map_request('artists/%s/videos' % self.id, params=params, parse=self.session.parse_video)
+        params = {"limit": limit, "offset": offset}
+        return self.request.map_request(
+            "artists/%s/videos" % self.id, params=params, parse=self.session.parse_video
+        )
 
     def get_bio(self):
-        """
-        Queries TIDAL for the artists biography
+        """Queries TIDAL for the artists biography.
 
-        :return: A string containing the bio, as well as identifiers to other TIDAL objects inside the bio.
+        :return: A string containing the bio, as well as identifiers to other TIDAL
+            objects inside the bio.
         """
         # morguldir: TODO: Add parsing of wimplinks?
-        return self.request.request('GET', 'artists/%s/bio' % self.id).json()['text']
+        return self.request.request("GET", "artists/%s/bio" % self.id).json()["text"]
 
     def get_similar(self):
-        """
-        Queries TIDAL for similar artists
+        """Queries TIDAL for similar artists.
 
         :return: A list of :class:`Artists <tidalapi.artist.Artist>`
         """
-        return self.request.map_request('artists/%s/similar' % self.id, parse=self.parse_artist)
+        return self.request.map_request(
+            "artists/%s/similar" % self.id, parse=self.parse_artist
+        )
 
     def get_radio(self):
-        """
-        Queries TIDAL for the artist radio, which is a mix of tracks that are similar to what the artist makes.
+        """Queries TIDAL for the artist radio, which is a mix of tracks that are similar
+        to what the artist makes.
 
         :return: A list of :class:`Tracks <tidalapi.media.Track>`
         """
-        params = {'limit': 100}
-        return self.request.map_request('artists/%s/radio' % self.id, params=params, parse=self.session.parse_track)
+        params = {"limit": 100}
+        return self.request.map_request(
+            "artists/%s/radio" % self.id, params=params, parse=self.session.parse_track
+        )
 
     def image(self, dimensions):
-        """
-        A url to an artist picture
+        """A url to an artist picture.
 
         :param dimensions: The width and height that you want from the image
         :type dimensions: int
         :return: A url to the image.
 
         Valid resolutions: 160x160, 320x320, 480x480, 750x750
         """
         if dimensions not in [160, 320, 480, 750]:
             raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
 
         if not self.picture:
-            json = self.request.request('get', 'artists/%s' % self.id).json()
-            self.picture = json.get('picture')
+            json = self.request.request("get", "artists/%s" % self.id).json()
+            self.picture = json.get("picture")
 
-        return self.session.config.image_url % (self.picture.replace('-', '/'), dimensions, dimensions)
+        return self.session.config.image_url % (
+            self.picture.replace("-", "/"),
+            dimensions,
+            dimensions,
+        )
 
     def page(self):
         """
         Retrieve the artist page as seen on https://listen.tidal.com/artist/$id
 
         :return: A :class:`.Page` containing all the categories from the page, e.g. tracks, influencers and credits
         """
         return self.session.page.get("pages/artist", params={"artistId": self.id})
 
 
 class Role(Enum):
-    """
-    An Enum with different roles an artist can have.
-    """
-    main = 'MAIN'
-    featured = 'FEATURED'
-    contributor = 'CONTRIBUTOR'
-    artist = 'ARTIST'
+    """An Enum with different roles an artist can have."""
+
+    main = "MAIN"
+    featured = "FEATURED"
+    contributor = "CONTRIBUTOR"
+    artist = "ARTIST"
```

### Comparing `tidalapi-0.7.1/tidalapi/genre.py` & `tidalapi-0.7.2/tidalapi/genre.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,64 +11,67 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-"""
+""""""
 
 import copy
+from typing import TYPE_CHECKING, Any, List, Optional
 
+from tidalapi.types import JsonObj
 
-class Genre(object):
-    """
+if TYPE_CHECKING:
+    from tidalapi.session import Session, TypeRelation
 
-    """
 
-    name = ""
-    path = ""
-    playlists = False
-    artists = False
-    albums = False
-    tracks = False
-    videos = False
-    image = ""
+class Genre:
+    name: str = ""
+    path: str = ""
+    playlists: bool = False
+    artists: bool = False
+    albums: bool = False
+    tracks: bool = False
+    videos: bool = False
+    image: str = ""
 
-    def __init__(self, session):
+    def __init__(self, session: "Session"):
         self.session = session
         self.requests = session.request
 
-    def parse_genre(self, json_obj):
-        self.name = json_obj['name']
-        self.path = json_obj['path']
-        self.playlists = json_obj['hasPlaylists']
-        self.artists = json_obj['hasArtists']
-        self.albums = json_obj['hasAlbums']
-        self.tracks = json_obj['hasTracks']
-        self.videos = json_obj['hasVideos']
-        self.image = "http://resources.wimpmusic.com/images/%s/460x306.jpg" % json_obj['image'].replace('-', '/')
+    def parse_genre(self, json_obj: JsonObj) -> "Genre":
+        self.name = json_obj["name"]
+        self.path = json_obj["path"]
+        self.playlists = json_obj["hasPlaylists"]
+        self.artists = json_obj["hasArtists"]
+        self.albums = json_obj["hasAlbums"]
+        self.tracks = json_obj["hasTracks"]
+        self.videos = json_obj["hasVideos"]
+        image_path = json_obj["image"].replace("-", "/")
+        self.image = f"http://resources.wimpmusic.com/images/{image_path}/460x306.jpg"
 
         return copy.copy(self)
 
-    def parse_genres(self, json_obj):
+    def parse_genres(self, json_obj: List[JsonObj]) -> List["Genre"]:
         return list(map(self.parse_genre, json_obj))
 
-    def get_genres(self):
-        return self.parse_genres(self.requests.request('GET', 'genres').json())
+    def get_genres(self) -> List["Genre"]:
+        return self.parse_genres(self.requests.request("GET", "genres").json())
 
-    def items(self, model):
-        """
-        Gets the current genre's items of the specified type
-        :param model: The tidalapi model you want returned. See :class:`Genre`
+    def items(self, model: List[Optional[Any]]) -> List[Optional[Any]]:
+        """Gets the current genre's items of the specified type :param model: The
+        tidalapi model you want returned.
+
+        See :class:`Genre`
         :return:
         """
-        type_index = self.session.type_conversions['type'].index(model)
-        name = self.session.type_conversions['identifier'][type_index]
-        parse = self.session.type_conversions['parse'][type_index]
+        type_relations: "TypeRelation" = next(
+            x for x in self.session.type_conversions if x.type == model
+        )
+        name = type_relations.identifier
+        parse = type_relations.parse
         if getattr(self, name):
-            location = 'genres/{0}/{1}'.format(self.path, name)
+            location = f"genres/{self.path}/{name}"
             return self.requests.map_request(location, parse=parse)
         raise TypeError("This genre does not contain {0}".format(name))
```

### Comparing `tidalapi-0.7.1/tidalapi/media.py` & `tidalapi-0.7.2/tidalapi/playlist.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,237 +11,249 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""A module containing things related to TIDAL playlists."""
 
-"""
-A module containing information about various media types.
-
-Classes: :class:`Media`, :class:`Track`, :class:`Video`
-"""
+from __future__ import annotations
 
 import copy
-import dateutil.parser
-import tidalapi
+from typing import TYPE_CHECKING, List, Optional
+
+if TYPE_CHECKING:
+    import tidalapi
 
+import dateutil.parser
 
-class Media(object):
-    """
-    Base class for generic media, specifically :class:`Track` and :class:`Video`
 
-    This class includes data used by both of the subclasses, and a function to parse both of them.
+class Playlist(object):
+    """An object containing various data about a playlist and methods to work with
+    them."""
 
-    The date_added attribute is only relevant for playlists.
-    For the release date of the actual media, use the release date of the album.
-    """
     id = None
     name = None
+    num_tracks = -1
+    num_videos = -1
+    creator = None
+    description = None
     duration = -1
-    available = True
-    tidal_release_date = None
-    user_date_added = None
-    track_num = -1
-    volume_num = 1
-    explicit = False
-    popularity = -1
-    artist = None
-    #: For the artist credit page
-    artist_roles = None
-    artists = None
-    album = None
+    last_updated = None
+    created = None
     type = None
+    public: Optional[bool] = False
+    popularity = -1
+    promoted_artists = None
+    last_item_added_at = None
+    picture: Optional[str] = None
+    square_picture: Optional[str] = None
+    user_date_added = None
+    _etag = None
 
-    def __init__(self, session, media_id=None):
+    def __init__(self, session, playlist_id):
+        self.id = playlist_id
         self.session = session
-        self.requests = self.session.request
-        self.album = session.album()
-        self.id = media_id
-        if media_id is not None:
-            self._get(self.id)
-
-    def _get(self, media_id):
-        raise NotImplementedError("You are not supposed to use the media class directly.")
+        self.requests = session.request
+        self._base_url = "playlists/%s"
+        if playlist_id:
+            request = self.requests.request("GET", self._base_url % playlist_id)
+            self._etag = request.headers["etag"]
+            self.parse(request.json())
 
     def parse(self, json_obj):
-        """
-        Assigns all
-        :param json_obj:
-        :return:
-        """
-        artists = self.session.parse_artists(json_obj['artists'])
-
-        # Sometimes the artist field is not filled, example: 62300893
-        if 'artist' in json_obj:
-            artist = self.session.parse_artist(json_obj['artist'])
-        else:
-            artist = artists[0]
-
-        album = None
-        if json_obj['album']:
-            album = self.session.album().parse(json_obj['album'], artist, artists)
-
-        self.id = json_obj['id']
-        self.name = json_obj['title']
-        self.duration = json_obj['duration']
-        self.available = bool(json_obj['streamReady'])
-
-        # Removed media does not have a release date.
-        self.tidal_release_date = None
-        release_date = json_obj.get('streamStartDate')
-        self.tidal_release_date = dateutil.parser.isoparse(release_date) if release_date else None
-
-        # When getting items from playlists they have a date added attribute, same with favorites.
-        user_date_added = json_obj.get('dateAdded')
-        self.user_date_added = dateutil.parser.isoparse(user_date_added) if user_date_added else None
-
-        self.track_num = json_obj['trackNumber']
-        self.volume_num = json_obj['volumeNumber']
-        self.explicit = bool(json_obj['explicit'])
-        self.popularity = json_obj['popularity']
-        self.artist = artist
-        self.artists = artists
-        self.album = album
-        self.type = json_obj.get('type')
-
-        self.artist_roles = json_obj.get('artistRoles')
-
-    def parse_media(self, json_obj):
-        """
-        Selects the media type when checking lists that can contain both.
-
-        :param json_obj: The json containing the media
-        :return: Returns a new Video or Track object.
-        """
-        if json_obj.get('type') is None or json_obj['type'] == 'Track':
-            return Track(self.session).parse_track(json_obj)
-        # There are other types like Event, Live, and Video witch match the video class
-        return Video(self.session).parse_video(json_obj)
-
-
-class Track(Media):
-    """
-    An object containing information about a track.
-    """
-    replay_gain = None
-    peak = None
-    isrc = None
-    audio_quality = None
-    version = None
-    copyright = None
-
-    def parse_track(self, json_obj):
-        Media.parse(self, json_obj)
-        self.replay_gain = json_obj['replayGain']
-        # Tracks from the pages endpoints might not actually exist
-        if 'peak' in json_obj and 'isrc' in json_obj:
-            self.peak = json_obj['peak']
-            self.isrc = json_obj['isrc']
-            self.copyright = json_obj['copyright']
-        self.audio_quality = tidalapi.Quality(json_obj['audioQuality'])
-        self.version = json_obj['version']
-
-        return copy.copy(self)
-
-    def _get(self, media_id):
-        """
-        Returns information about a track, and also replaces the track used to call this function.
+        """Parses a playlist from tidal, replaces the current playlist object.
 
-        :param media_id: TIDAL's identifier of the track
-        :return: A :class:`Track` object containing all the information about the track
+        :param json_obj: Json data returned from api.tidal.com containing a playlist
+        :return: Returns a copy of the original :exc: 'Playlist': object
         """
-        parse = self.parse_track
-        return self.requests.map_request('tracks/%s' % media_id, parse=parse)
-
-    def get_url(self):
-        params = {
-            'urlusagemode': 'STREAM',
-            'audioquality' : self.session.config.quality,
-            'assetpresentation': 'FULL',
-        }
-        request = self.requests.request('GET', 'tracks/%s/urlpostpaywall' % self.id, params)
-        return request.json()['urls'][0]
-
-    def lyrics(self):
-        """
-        Retrieves the lyrics for a song
-
-        :return: A :class:`Lyrics` object containing the lyrics
-        :raises: A :class:`requests.HTTPError` if there aren't any lyrics
-        """
-        return self.requests.map_request('tracks/%s/lyrics' % self.id, parse=Lyrics().parse)
-
-    def get_track_radio(self):
-        """
-        Queries TIDAL for the track radio, which is a mix of tracks that are similar to this track.
-
-        :return: A list of :class:`Tracks <tidalapi.media.Track>`
-        """
-        params = {'limit': 100}
-        return self.requests.map_request('tracks/%s/radio' % self.id, params=params, parse=self.session.parse_track)
-
-class Lyrics(object):
-    track_id = -1
-    provider = ""
-    provider_track_id = -1
-    provider_lyrics_id = -1
-    text = ""
-    #: Contains timestamps as well
-    subtitles = ""
-    right_to_left = False
-
-    def parse(self, json_obj):
-        self.track_id = json_obj['trackId']
-        self.provider = json_obj['lyricsProvider']
-        self.provider_track_id = json_obj['providerCommontrackId']
-        self.provider_lyrics_id = json_obj['providerLyricsId']
-        self.text = json_obj['lyrics']
-        self.subtitles = json_obj['subtitles']
-        self.right_to_left = bool(json_obj['isRightToLeft'])
+        self.id = json_obj["uuid"]
+        self.name = json_obj["title"]
+        self.num_tracks = int(json_obj["numberOfTracks"])
+        self.num_videos = int(json_obj["numberOfVideos"])
+        self.description = json_obj["description"]
+        self.duration = int(json_obj["duration"])
+
+        # These can be missing on from the /pages endpoints
+        last_updated = json_obj.get("lastUpdated")
+        self.last_updated = (
+            dateutil.parser.isoparse(last_updated) if last_updated else None
+        )
+        created = json_obj.get("created")
+        self.created = dateutil.parser.isoparse(created) if created else None
+        public = json_obj.get("publicPlaylist")
+        self.public = None if public is None else bool(public)
+        self.popularity = json_obj.get("popularity")
+
+        self.type = json_obj["type"]
+        self.picture = json_obj["image"]
+        self.square_picture = json_obj["squareImage"]
+
+        promoted_artists = json_obj["promotedArtists"]
+        self.promoted_artists = (
+            self.session.parse_artists(promoted_artists) if promoted_artists else None
+        )
+
+        last_item_added_at = json_obj.get("lastItemAddedAt")
+        self.last_item_added_at = (
+            dateutil.parser.isoparse(last_item_added_at) if last_item_added_at else None
+        )
+
+        user_date_added = json_obj.get("dateAdded")
+        self.user_date_added = (
+            dateutil.parser.isoparse(user_date_added) if user_date_added else None
+        )
+
+        creator = json_obj.get("creator")
+        if self.type == "ARTIST" and creator and creator.get("id"):
+            self.creator = self.session.parse_artist(creator)
+        else:
+            self.creator = self.session.parse_user(creator) if creator else None
 
         return copy.copy(self)
 
+    def factory(self):
+        if self.creator and self.creator.id == self.session.user.id:
+            return UserPlaylist(self.session, self.id)
+
+        return self
+
+    def parse_factory(self, json_obj):
+        self.parse(json_obj)
+        return copy.copy(self.factory())
+
+    def tracks(self, limit: Optional[int] = None, offset=0) -> List[tidalapi.Track]:
+        """Gets the playlists̈́' tracks from TIDAL.
+
+        :param limit: The amount of items you want returned.
+        :param offset: The index of the first item you want included.
+        :return: A list of :class:`Tracks <.Track>`
+        """
+        params = {"limit": limit, "offset": offset}
+        request = self.requests.request(
+            "GET", self._base_url % self.id + "/tracks", params=params
+        )
+        self._etag = request.headers["etag"]
+        return self.requests.map_json(
+            json_obj=request.json(), parse=self.session.parse_track
+        )
+
+    def items(self, limit=100, offset=0):
+        """Fetches up to the first 100 items, including tracks and videos.
+
+        :param limit: The amount of items you want, up to 100.
+        :param offset: The index of the first item you want returned
+        :return: A list of :class:`Tracks<.Track>` and :class:`Videos<.Video>`
+        """
+        params = {"limit": limit, "offset": offset}
+        request = self.requests.request(
+            "GET", self._base_url % self.id + "/items", params=params
+        )
+        self._etag = request.headers["etag"]
+        return self.requests.map_json(request.json(), parse=self.session.parse_media)
+
+    def image(self, dimensions):
+        """A URL to a playlist picture.
+
+        :param dimensions: The width and height that want from the image
+        :type dimensions: int
+        :return: A url to the image
+
+        Original sizes: 160x160, 320x320, 480x480, 640x640, 750x750, 1080x1080
+        """
+
+        if dimensions not in [160, 320, 480, 640, 750, 1080]:
+            raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
+        if self.square_picture is None:
+            raise AttributeError("No picture available")
+        return self.session.config.image_url % (
+            self.square_picture.replace("-", "/"),
+            dimensions,
+            dimensions,
+        )
+
+    def wide_image(self, width=1080, height=720):
+        """Create a url to a wider playlist image.
+
+        :param width: The width of the image
+        :param height: The height of the image
+        :return: Returns a url to the image with the specified resolution
 
-class Video(Media):
-    """
-    An object containing information about a video
-    """
-    release_date = None
-    video_quality = None
-    cover = None
-
-    def parse_video(self, json_obj):
-        Media.parse(self, json_obj)
-        release_date = json_obj.get('releaseDate')
-        self.release_date = dateutil.parser.isoparse(release_date) if release_date else None
-        self.cover = json_obj['imageId']
-        # Videos found in the /pages endpoints don't have quality
-        self.video_quality = json_obj.get('quality')
-
-        return copy.copy(self)
-
-    def _get(self, media_id):
+        Valid sizes: 160x107, 480x320, 750x500, 1080x720
         """
-        Returns information about the video, and replaces the object used to call this function.
 
-        :param media_id: TIDAL's identifier of the video
-        :return: A :class:`Video` object containing all the information about the video.
-        """
-        parse = self.parse_video
-        return self.requests.map_request('videos/%s' % media_id, parse=parse)
-
-    def get_url(self):
-        params = {
-            'urlusagemode': 'STREAM',
-            'videoquality': self.session.config.video_quality,
-            'assetpresentation': 'FULL'
-        }
-        request = self.requests.request('GET', 'videos/%s/urlpostpaywall' % self.id, params)
-        return request.json()['urls'][0]
-
-    def image(self, width=1080, height=720):
         if (width, height) not in [(160, 107), (480, 320), (750, 500), (1080, 720)]:
             raise ValueError("Invalid resolution {} x {}".format(width, height))
-
-        return self.session.config.image_url % (self.cover.replace('-', '/'), width, height)
+        if self.picture is None:
+            raise AttributeError("No picture available")
+        return self.session.config.image_url % (
+            self.picture.replace("-", "/"),
+            width,
+            height,
+        )
+
+
+class UserPlaylist(Playlist):
+    def _reparse(self):
+        request = self.requests.request("GET", self._base_url % self.id)
+        self._etag = request.headers["etag"]
+        self.requests.map_json(request.json(), parse=self.parse)
+
+    def edit(self, title=None, description=None):
+        if not title:
+            title = self.name
+        if not description:
+            description = self.description
+
+        data = {"title": title, "description": description}
+        self.requests.request("POST", self._base_url % self.id, data=data)
+
+    def delete(self):
+        self.requests.request("DELETE", self._base_url % self.id)
+
+    def add(self, media_ids):
+        data = {
+            "onArtifactNotFound": "SKIP",
+            "onDupes": "SKIP",
+            "trackIds": ",".join(map(str, media_ids)),
+        }
+        params = {"limit": 100}
+        headers = {"If-None-Match": self._etag}
+        self.requests.request(
+            "POST",
+            self._base_url % self.id + "/items",
+            params=params,
+            data=data,
+            headers=headers,
+        )
+        self._reparse()
+
+    def remove_by_index(self, index):
+        headers = {"If-None-Match": self._etag}
+        self.requests.request(
+            "DELETE", (self._base_url + "/items/%i") % (self.id, index), headers=headers
+        )
+
+    def remove_by_indices(self, indices):
+        headers = {"If-None-Match": self._etag}
+        track_index_string = ",".join([str(x) for x in indices])
+        self.requests.request(
+            "DELETE",
+            (self._base_url + "/tracks/%s") % (self.id, track_index_string),
+            headers=headers,
+        )
+
+    def _calculate_id(self, media_id):
+        i = 0
+        while i < self.num_tracks:
+            items = self.items(100, i)
+            for index, item in enumerate(items):
+                if item.id == media_id:
+                    # Return the amount of items we have gone through plus the index in the last list.
+                    return index + i
+
+            i += len(items)
+
+    def remove_by_id(self, media_id):
+        index = self._calculate_id(media_id)
+        self.remove_by_index(index)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tidalapi-0.7.1/tidalapi/mix.py` & `tidalapi-0.7.2/tidalapi/mix.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,99 +10,143 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""A module containing functions relating to TIDAL mixes."""
+
+from __future__ import annotations
 
-"""
-A module containing functions relating to TIDAL mixes.
-"""
 import copy
+from dataclasses import dataclass
 from enum import Enum
+from typing import TYPE_CHECKING, List, Optional, Union
+
+from tidalapi.types import JsonObj
+
+if TYPE_CHECKING:
+    from tidalapi.media import Track, Video
+    from tidalapi.session import Session
 
 
 class MixType(Enum):
-    """
-    An enum to track all the different types of mixes
-    """
-    video_daily = 'VIDEO_DAILY_MIX'
-    daily = 'DAILY_MIX'
-    discovery = 'DISCOVERY_MIX'
-    new_release = 'NEW_RELEASE_MIX'
-    track = 'TRACK_MIX'
-    artist = 'ARTIST_MIX'
-    songwriter = 'SONGWRITER_MIX'
-    producter = 'PRODUCER_MIX'
-    history_alltime = 'HISTORY_ALLTIME_MIX'
-    history_monthly = 'HISTORY_MONTHLY_MIX'
-    history_yearly = 'HISTORY_YEARLY_MIX'
+    """An enum to track all the different types of mixes."""
 
+    video_daily = "VIDEO_DAILY_MIX"
+    daily = "DAILY_MIX"
+    discovery = "DISCOVERY_MIX"
+    new_release = "NEW_RELEASE_MIX"
+    track = "TRACK_MIX"
+    artist = "ARTIST_MIX"
+    songwriter = "SONGWRITER_MIX"
+    producter = "PRODUCER_MIX"
+    history_alltime = "HISTORY_ALLTIME_MIX"
+    history_monthly = "HISTORY_MONTHLY_MIX"
+    history_yearly = "HISTORY_YEARLY_MIX"
+
+
+@dataclass
+class ImageResponse:
+    small: str
+    medium: str
+    large: str
 
-class Mix(object):
-    """
-    A mix from TIDAL, e.g. the listen.tidal.com/view/pages/my_collection_my_mixes
 
-    These get used for many things, like artist/track radio's, recommendations, and historical plays
+class Mix:
+    """A mix from TIDAL, e.g. the listen.tidal.com/view/pages/my_collection_my_mixes.
+
+    These get used for many things, like artist/track radio's, recommendations, and
+    historical plays
     """
-    id = ""
-    title = ""
-    sub_title = ""
+
+    id: str = ""
+    title: str = ""
+    sub_title: str = ""
     sharing_images = None
-    mix_type = None
-    content_behaviour = ""
-    short_subtitle = ""
+    mix_type: Optional[MixType] = None
+    content_behaviour: str = ""
+    short_subtitle: str = ""
+    images: Optional[ImageResponse] = None
     _retrieved = False
-    _items = None
+    _items: Optional[List[Union["Video", "Track"]]] = None
 
-    def __init__(self, session, mix_id):
+    def __init__(self, session: Session, mix_id: str):
         self.session = session
         self.request = session.request
         if mix_id is not None:
             self.get(mix_id)
 
-    def get(self, mix_id=None):
-        """
-        Returns information about a mix, and also replaces the mix object used to call this function.
+    def get(self, mix_id: Optional[str] = None) -> "Mix":
+        """Returns information about a mix, and also replaces the mix object used to
+        call this function.
 
         :param mix_id: TIDAL's identifier of the mix
         :return: A :class:`Mix` object containing all the information about the mix
         """
         if mix_id is None:
             mix_id = self.id
 
-        params = {'mixId': mix_id,
-                  'deviceType': 'BROWSER'}
+        params = {"mixId": mix_id, "deviceType": "BROWSER"}
         parse = self.session.parse_page
-        result = self.request.map_request('pages/mix', parse=parse, params=params)
+        result = self.request.map_request("pages/mix", parse=parse, params=params)
+        assert not isinstance(result, list)
         self._retrieved = True
         self.__dict__.update(result.categories[0].__dict__)
         self._items = result.categories[1].items
         return self
 
-    def parse(self, json_obj):
-        """ Parse a mix into a :class:`Mix`, replaces the calling object
+    def parse(self, json_obj: JsonObj) -> "Mix":
+        """Parse a mix into a :class:`Mix`, replaces the calling object.
 
         :param json_obj: The json of a mix to be parsed
         :return: A copy of the parsed mix
         """
-        self.id = json_obj['id']
-        self.title = json_obj['title']
-        self.sub_title = json_obj['subTitle']
-        self.sharing_images = json_obj['sharingImages']
-        self.mix_type = MixType(json_obj['mixType'])
-        self.content_behaviour = json_obj['contentBehavior']
-        self.short_subtitle = json_obj['shortSubtitle']
+        self.id = json_obj["id"]
+        self.title = json_obj["title"]
+        self.sub_title = json_obj["subTitle"]
+        self.sharing_images = json_obj["sharingImages"]
+        self.mix_type = MixType(json_obj["mixType"])
+        self.content_behaviour = json_obj["contentBehavior"]
+        self.short_subtitle = json_obj["shortSubtitle"]
+        images = json_obj["images"]
+        self.images = ImageResponse(
+            small=images["SMALL"]["url"],
+            medium=images["MEDIUM"]["url"],
+            large=images["LARGE"]["url"],
+        )
 
         return copy.copy(self)
 
-    def items(self):
-        """
-        Returns all the items in the mix, retrieves them with :class:`get` as well if not already done
+    def items(self) -> List[Union["Video", "Track"]]:
+        """Returns all the items in the mix, retrieves them with :class:`get` as well if
+        not already done.
 
         :return: A :class:`list` of videos and/or tracks from the mix
         """
         if not self._retrieved:
             self.get(self.id)
-
+        if not self._items:
+            raise ValueError("Retrieved items missing")
         return self._items
+
+    def image(self, dimensions: int) -> str:
+        """A URL to a Mix picture.
+
+        :param dimensions: The width and height the requested image should be
+        :type dimensions: int
+        :return: A url to the image
+
+        Original sizes: 320x320, 640x640, 1500x1500
+        """
+        if not self.images:
+            raise ValueError("No images present.")
+
+        if dimensions == 320:
+            return self.images.small
+        elif dimensions == 640:
+            return self.images.medium
+        elif dimensions == 1500:
+            return self.images.large
+
+        raise ValueError(f"Invalid resolution {dimensions} x {dimensions}")
```

### Comparing `tidalapi-0.7.1/tidalapi/page.py` & `tidalapi-0.7.2/tidalapi/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,338 +10,349 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
 """
 Module for parsing TIDAL's pages format found at https://listen.tidal.com/v1/pages
 """
 
 import copy
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union, cast
+
+from tidalapi.types import JsonObj
+
+if TYPE_CHECKING:
+    import tidalapi
+
 
 class Page(object):
     """
     A page from the https://listen.tidal.com/view/pages/ endpoint
 
     The :class:`categories` field will the most complete information
     However it is an iterable that goes through all the visible items on the page as well, in the natural reading order
     """
+
     title = ""
-    categories = None
-    _categories_iter = None
+    categories: Optional[List[Any]] = None
+    _categories_iter: Optional[Iterator[Any]] = None
 
     def __init__(self, session, title):
         self.request = session.request
         self.categories = None
         self.title = title
         self.page_category = PageCategory(session)
 
     def __iter__(self):
+        if self.categories is None:
+            raise AttributeError("No categories found")
         self._categories_iter = iter(self.categories)
         self._category = next(self._categories_iter)
         self._items_iter = iter(self._category.items)
         return self
 
     def __next__(self):
         if self._category == StopIteration:
             return StopIteration
         try:
             item = next(self._items_iter)
         except StopIteration:
+            if self._categories_iter is None:
+                raise AttributeError("No categories found")
             self._category = next(self._categories_iter)
             self._items_iter = iter(self._category.items)
             return self.__next__()
         return item
 
     def next(self):
         return self.__next__()
 
-    def parse(self, json_obj):
-        """
-        Goes through everything in the page, and gets the title and adds all the rows to the categories field
-        :param json_obj: The json to be parsed
-        :return: A copy of the Page that you can use to browse all the items
-        """
-        self.title = json_obj['title']
+    def parse(self, json_obj: JsonObj) -> "Page":
+        """Goes through everything in the page, and gets the title and adds all the rows
+        to the categories field :param json_obj: The json to be parsed :return: A copy
+        of the Page that you can use to browse all the items."""
+        self.title = json_obj["title"]
         self.categories = []
-        for row in json_obj['rows']:
-            page_item = self.page_category.parse(row['modules'][0])
+        for row in json_obj["rows"]:
+            page_item = self.page_category.parse(row["modules"][0])
             self.categories.append(page_item)
 
         return copy.copy(self)
 
-    def get(self, endpoint, params=None):
-        """
-        Retrieve a page from the specified endpoint, overwrites the calling page
+    def get(self, endpoint: str, params: Optional[Dict[str, Any]] = None) -> "Page":
+        """Retrieve a page from the specified endpoint, overwrites the calling page.
 
         :param params: Parameter to retrieve the page with
         :param endpoint: The endpoint you want to retrieve
         :return: A copy of the new :class:`.Page` at the requested endpoint
         """
         url = endpoint
 
         if params is None:
             params = {}
         if "deviceType" not in params:
             params["deviceType"] = "BROWSER"
 
-        json_obj = self.request.request('GET', url, params=params).json()
+        json_obj = self.request.request("GET", url, params=params).json()
         return self.parse(json_obj)
 
 
 class PageCategory(object):
     type = None
     title = None
-    description = ""
-    session = None
+    description: Optional[str] = ""
     requests = None
-    _more = None
+    _more: Optional[dict[str, Union[dict[str, str], str]]] = None
 
-    def __init__(self, session):
+    def __init__(self, session: "tidalapi.session.Session"):
         self.session = session
         self.request = session.request
         self.item_types = {
-            'ALBUM_LIST': self.session.parse_album,
-            'ARTIST_LIST': self.session.parse_artist,
-            'TRACK_LIST': self.session.parse_track,
-            'PLAYLIST_LIST': self.session.parse_playlist,
-            'VIDEO_LIST': self.session.parse_video,
-            'MIX_LIST': self.session.parse_mix,
+            "ALBUM_LIST": self.session.parse_album,
+            "ARTIST_LIST": self.session.parse_artist,
+            "TRACK_LIST": self.session.parse_track,
+            "PLAYLIST_LIST": self.session.parse_playlist,
+            "VIDEO_LIST": self.session.parse_video,
+            "MIX_LIST": self.session.parse_mix,
         }
 
     def parse(self, json_obj):
         result = None
-        category_type = json_obj['type']
-        if category_type in ('PAGE_LINKS_CLOUD', 'PAGE_LINKS'):
-            category = PageLinks(self.session)
-        elif category_type in ('FEATURED_PROMOTIONS', 'MULTIPLE_TOP_PROMOTIONS'):
+        category_type = json_obj["type"]
+        if category_type in ("PAGE_LINKS_CLOUD", "PAGE_LINKS"):
+            category: Union[
+                PageLinks, FeaturedItems, ItemList, TextBlock, LinkList
+            ] = PageLinks(self.session)
+        elif category_type in ("FEATURED_PROMOTIONS", "MULTIPLE_TOP_PROMOTIONS"):
             category = FeaturedItems(self.session)
         elif category_type in self.item_types.keys():
             category = ItemList(self.session)
-        elif category_type == 'MIX_HEADER':
-            result = self.session.parse_mix(json_obj['mix'])
-        elif category_type == 'ARTIST_HEADER':
-            result = self.session.parse_artist(json_obj['artist'])
-            result.bio = json_obj['bio']
-        elif category_type == 'ALBUM_HEADER':
-            result = self.session.parse_album(json_obj['album'])
-        elif category_type == 'HIGHLIGHT_MODULE':
+        elif category_type == "MIX_HEADER":
+            return self.session.parse_mix(json_obj["mix"])
+        elif category_type == "ARTIST_HEADER":
+            result = self.session.parse_artist(json_obj["artist"])
+            result.bio = json_obj["bio"]
+            return result
+        elif category_type == "ALBUM_HEADER":
+            return self.session.parse_album(json_obj["album"])
+        elif category_type == "HIGHLIGHT_MODULE":
             category = ItemList(self.session)
-        elif category_type == 'MIXED_TYPES_LIST':
+        elif category_type == "MIXED_TYPES_LIST":
             category = ItemList(self.session)
-        elif category_type == 'TEXT_BLOCK':
+        elif category_type == "TEXT_BLOCK":
             category = TextBlock(self.session)
-        elif category_type in ('ITEM_LIST_WITH_ROLES', 'ALBUM_ITEMS'):
+        elif category_type in ("ITEM_LIST_WITH_ROLES", "ALBUM_ITEMS"):
             category = ItemList(self.session)
-        elif category_type == 'ARTICLE_LIST':
-            json_obj['items'] = json_obj['pagedList']['items']
+        elif category_type == "ARTICLE_LIST":
+            json_obj["items"] = json_obj["pagedList"]["items"]
             category = LinkList(self.session)
-        elif category_type == 'SOCIAL':
-            json_obj['items'] = json_obj['socialProfiles']
+        elif category_type == "SOCIAL":
+            json_obj["items"] = json_obj["socialProfiles"]
             category = LinkList(self.session)
         else:
-            raise NotImplementedError('PageType {} not implemented'.format(category_type))
-
-        if result:
-            return result
+            raise NotImplementedError(
+                "PageType {} not implemented".format(category_type)
+            )
 
         return category.parse(json_obj)
 
     def show_more(self):
-        """
-        Get the full list of items on their own :class:`.Page` from a :class:`.PageCategory`
+        """Get the full list of items on their own :class:`.Page` from a
+        :class:`.PageCategory`
 
         :return: A :class:`.Page` more of the items in the category, None if there aren't any
         """
-        return Page(self.session, self._more['title']).get(self._more['apiPath']) if self._more else None
+        if self._more:
+            api_path = self._more["apiPath"]
+            assert isinstance(api_path, str)
+        else:
+            api_path = None
+        return (
+            Page(self.session, self._more["title"]).get(api_path)
+            if api_path and self._more
+            else None
+        )
 
 
 class FeaturedItems(PageCategory):
-    """
-    Items that have been featured by TIDAL
-    """
-    items = None
+    """Items that have been featured by TIDAL."""
+
+    items: Optional[list["PageItem"]] = None
 
     def __init__(self, session):
         super(FeaturedItems, self).__init__(session)
 
     def parse(self, json_obj):
         self.items = []
-        self.title = json_obj['title']
-        self.description = json_obj['description']
+        self.title = json_obj["title"]
+        self.description = json_obj["description"]
 
-        for item in json_obj['items']:
+        for item in json_obj["items"]:
             self.items.append(PageItem(self.session, item))
 
         return self
 
 
 class PageLinks(PageCategory):
-    """
-    A list of :class:`.PageLink` to other parts of TIDAL
-    """
-    items = None
+    """A list of :class:`.PageLink` to other parts of TIDAL."""
+
+    items: Optional[list["PageLink"]] = None
 
     def parse(self, json_obj):
-        """
-        Parse the list of links from TIDAL
+        """Parse the list of links from TIDAL.
 
         :param json_obj: The json to be parsed
         :return: A copy of this page category containing the links in the items field
         """
-        self._more = json_obj.get('showMore')
-        self.title = json_obj['title']
+        self._more = json_obj.get("showMore")
+        self.title = json_obj["title"]
         self.items = []
-        for item in json_obj['pagedList']['items']:
+        for item in json_obj["pagedList"]["items"]:
             self.items.append(PageLink(self.session, item))
 
         return copy.copy(self)
 
 
 class ItemList(PageCategory):
-    """
-    A list of items from TIDAL, can be a list of mixes, for example, or a list of playlists and mixes in some cases
-    """
+    """A list of items from TIDAL, can be a list of mixes, for example, or a list of
+    playlists and mixes in some cases."""
+
     items = None
 
     def parse(self, json_obj):
-        """
-        Parse a list of items on TIDAL from the pages endpoints.
+        """Parse a list of items on TIDAL from the pages endpoints.
 
         :param json_obj: The json from TIDAL to be parsed
         :return: A copy of the ItemList with a list of items
         """
-        self._more = json_obj.get('showMore')
-        self.title = json_obj['title']
-        item_type = json_obj['type']
-        list_key = 'pagedList'
+        self._more = json_obj.get("showMore")
+        self.title = json_obj["title"]
+        item_type = json_obj["type"]
+        list_key = "pagedList"
         session = None
         parse = None
 
         if item_type in self.item_types.keys():
             parse = self.item_types[item_type]
-        elif item_type == 'HIGHLIGHT_MODULE':
+        elif item_type == "HIGHLIGHT_MODULE":
             session = self.session
             # Unwrap subtitle, maybe add a field for it later
-            json_obj[list_key] = {'items': [x['item'] for x in json_obj['highlights']]}
-        elif item_type in ('MIXED_TYPES_LIST', 'ALBUM_ITEMS'):
+            json_obj[list_key] = {"items": [x["item"] for x in json_obj["highlights"]]}
+        elif item_type in ("MIXED_TYPES_LIST", "ALBUM_ITEMS"):
             session = self.session
-        elif item_type == 'ITEM_LIST_WITH_ROLES':
-            for item in json_obj[list_key]['items']:
-                item['item']['artistRoles'] = item['roles']
+        elif item_type == "ITEM_LIST_WITH_ROLES":
+            for item in json_obj[list_key]["items"]:
+                item["item"]["artistRoles"] = item["roles"]
             session = self.session
         else:
             raise NotImplementedError("PageType {} not implemented".format(item_type))
 
         self.items = self.request.map_json(json_obj[list_key], parse, session)
 
         return copy.copy(self)
 
 
 class PageLink(object):
-    """
-    A Link to another :class:`.Page` on TIDAL, Call get() to retrieve the Page
-    """
+    """A Link to another :class:`.Page` on TIDAL, Call get() to retrieve the Page."""
+
     title = None
     icon = None
-    api_path = None
     image_id = None
-    session = None
     requests = None
 
-    def __init__(self, session, json_obj):
+    def __init__(self, session: "tidalapi.session.Session", json_obj):
         self.session = session
         self.request = session.request
-        self.title = json_obj['title']
-        self.icon = json_obj['icon']
-        self.api_path = json_obj['apiPath']
-        self.image_id = json_obj['imageId']
+        self.title = json_obj["title"]
+        self.icon = json_obj["icon"]
+        self.api_path = cast(str, json_obj["apiPath"])
+        self.image_id = json_obj["imageId"]
 
     def get(self):
-        """
-        Requests the linked page from TIDAL
-        :return: A :class:`Page` at the api_path
-        """
-        return self.request.map_request(self.api_path, params={'deviceType': 'DESKTOP'}, parse=self.session.parse_page)
+        """Requests the linked page from TIDAL :return: A :class:`Page` at the
+        api_path."""
+        return self.request.map_request(
+            self.api_path,
+            params={"deviceType": "DESKTOP"},
+            parse=self.session.parse_page,
+        )
 
 
 class PageItem(object):
-    """
-    An Item from a :class:`.PageCategory` from the /pages endpoint, call get() to retrieve the actual item
-    """
+    """An Item from a :class:`.PageCategory` from the /pages endpoint, call get() to
+    retrieve the actual item."""
+
     header = ""
     short_header = ""
     short_sub_header = ""
     image_id = ""
     type = ""
     artifact_id = ""
     text = ""
     featured = False
 
     def __init__(self, session, json_obj):
         self.session = session
         self.request = session.request
-        self.header = json_obj['header']
-        self.short_header = json_obj['shortHeader']
-        self.short_sub_header = json_obj['shortSubHeader']
-        self.image_id = json_obj['imageId']
-        self.type = json_obj['type']
-        self.artifact_id = json_obj['artifactId']
-        self.text = json_obj['text']
-        self.featured = bool(json_obj['featured'])
+        self.header = json_obj["header"]
+        self.short_header = json_obj["shortHeader"]
+        self.short_sub_header = json_obj["shortSubHeader"]
+        self.image_id = json_obj["imageId"]
+        self.type = json_obj["type"]
+        self.artifact_id = json_obj["artifactId"]
+        self.text = json_obj["text"]
+        self.featured = bool(json_obj["featured"])
 
     def get(self):
-        """
-        Retrieve the PageItem with the artifact_id matching the type
+        """Retrieve the PageItem with the artifact_id matching the type.
 
         :return: The fully parsed item, e.g. :class:`.Playlist`, :class:`.Video`, :class:`.Track`
         """
-        if self.type == 'PLAYLIST':
+        if self.type == "PLAYLIST":
             result = self.session.playlist(self.artifact_id)
-        elif self.type == 'VIDEO':
+        elif self.type == "VIDEO":
             result = self.session.video(self.artifact_id)
-        elif self.type == 'TRACK':
+        elif self.type == "TRACK":
             result = self.session.track(self.artifact_id)
-        elif self.type == 'ARTIST':
+        elif self.type == "ARTIST":
             result = self.session.artist(self.artifact_id)
         else:
             raise NotImplementedError("PageItem type %s not implemented" % self.type)
 
         return result
 
 
 class TextBlock(object):
-    """
-    A block of text, with a named icon, which seems to be left up to the application
-    """
+    """A block of text, with a named icon, which seems to be left up to the
+    application."""
+
     text = ""
     icon = ""
     items = None
 
     def __init__(self, session):
         self.session = session
 
     def parse(self, json_obj):
-        self.text = json_obj['text']
-        self.icon = json_obj['icon']
+        self.text = json_obj["text"]
+        self.icon = json_obj["icon"]
         self.items = [self.text]
 
         return copy.copy(self)
 
 
 class LinkList(PageCategory):
-    """
-    A list of items containing links, e.g. social links or articles
-    """
+    """A list of items containing links, e.g. social links or articles."""
+
     items = None
     title = None
     description = None
 
     def parse(self, json_obj):
-        self.items = json_obj['items']
-        self.title = json_obj['title']
-        self.description = json_obj['description']
+        self.items = json_obj["items"]
+        self.title = json_obj["title"]
+        self.description = json_obj["description"]
 
         return copy.copy(self)
```

### Comparing `tidalapi-0.7.1/tidalapi/request.py` & `tidalapi-0.7.2/tidalapi/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,82 +11,81 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-A module containing functions relating to TIDAL api requests.
-"""
+"""A module containing functions relating to TIDAL api requests."""
 
 import json
 import logging
-import requests
+from typing import Any, List
+from urllib.parse import urljoin
 
-try:
-    from urlparse import urljoin
-except ImportError:
-    from urllib.parse import urljoin
+import requests
 
 log = logging.getLogger(__name__)
 
 
 class Requests(object):
-    """
-    A class for handling api requests to TIDAL.
-    """
+    """A class for handling api requests to TIDAL."""
 
     def __init__(self, session):
         self.session = session
         self.config = session.config
 
     def basic_request(self, method, path, params=None, data=None, headers=None):
         request_params = {
-            'sessionId': self.session.session_id,
-            'countryCode': self.session.country_code,
-            'limit': self.config.item_limit,
+            "sessionId": self.session.session_id,
+            "countryCode": self.session.country_code,
+            "limit": self.config.item_limit,
         }
 
         if params:
-            # Don't update items with a none value, as we prefer a default value, requests also does not support them.
+            # Don't update items with a none value, as we prefer a default value.
+            # requests also does not support them.
             not_none = filter(lambda item: item[1] is not None, params.items())
             request_params.update(not_none)
 
         if not headers:
             headers = {}
         if self.session.token_type:
-            headers['authorization'] = self.session.token_type + ' ' + self.session.access_token
+            headers["authorization"] = (
+                self.session.token_type + " " + self.session.access_token
+            )
 
         url = urljoin(self.session.config.api_location, path)
-        request = self.session.request_session.request(method, url, params=request_params, data=data, headers=headers)
+        request = self.session.request_session.request(
+            method, url, params=request_params, data=data, headers=headers
+        )
 
         refresh_token = self.session.refresh_token
         if not request.ok and refresh_token:
             json_resp = None
             try:
                 json_resp = request.json()
-            except requests.JSONDecodeError:
+            except json.decoder.JSONDecodeError:
                 pass
 
-            if json_resp and json_resp.get('userMessage', '').startswith("The token has expired."):
+            if json_resp and json_resp.get("userMessage", "").startswith(
+                "The token has expired."
+            ):
                 log.debug("The access token has expired, trying to refresh it.")
                 refreshed = self.session.token_refresh(refresh_token)
                 if refreshed:
                     request = self.basic_request(method, url, params, data, headers)
             else:
-                log.warning('HTTP error on %d', request.status_code)
-                log.debug('Response text\n%s', request.text)
+                log.warning("HTTP error on %d", request.status_code)
+                log.debug("Response text\n%s", request.text)
 
         return request
 
     def request(self, method, path, params=None, data=None, headers=None):
-        """
-        Method for tidal requests.
+        """Method for tidal requests.
 
         Not meant for use outside of this library.
 
         :param method: The type of request to make
         :param path: The TIDAL api endpoint you want to use.
         :param params: The parameters you want to supply with the request.
         :param data: The data you want to supply with the request.
@@ -98,68 +97,66 @@
         log.debug("request: %s", request.request.url)
         request.raise_for_status()
         if request.content:
             log.debug("response: %s", json.dumps(request.json(), indent=4))
         return request
 
     def map_request(self, url, params=None, parse=None):
-        """
-        Returns the data about object(s) at the specified url,
-        with the method specified in the parse argument
+        """Returns the data about object(s) at the specified url, with the method
+        specified in the parse argument.
 
         Not meant for use outside of this library
 
         :param url: TIDAL api endpoint that contains the data
         :param params: TIDAL parameters to use when getting the data
         :param parse: The method used to parse the data at the url
-        :return: The object(s) at the url, with the same type as the class of the parse method.
+        :return: The object(s) at the url, with the same type as the class of the parse
+            method.
         """
-        json_obj = self.request('GET', url, params).json()
+        json_obj = self.request("GET", url, params).json()
 
         return self.map_json(json_obj, parse=parse)
 
     @classmethod
     def map_json(cls, json_obj, parse=None, session=None):
-        items = json_obj.get('items')
+        items = json_obj.get("items")
 
         if items is None:
             return parse(json_obj)
 
-        if len(items) > 0 and 'item' in items[0]:
+        if len(items) > 0 and "item" in items[0]:
             # Move created date into the item json data like it is done for playlists tracks.
-            if 'created' in items[0]:
+            if "created" in items[0]:
                 for item in items:
-                    item['item']['dateAdded'] = item['created']
+                    item["item"]["dateAdded"] = item["created"]
 
             lists = []
             for item in items:
                 if session is not None:
-                    parse = session.convert_type(item['type'].lower() + 's', output='parse')
-                lists.append(parse(item['item']))
+                    parse = session.convert_type(
+                        item["type"].lower() + "s", output="parse"
+                    )
+                lists.append(parse(item["item"]))
 
             return lists
         return list(map(parse, items))
 
     def get_items(self, url, parse):
-        """
-        Returns a list of items, used when there are over a 100 items,
-        but TIDAL doesn't always allow more specifying a higher limit.
+        """Returns a list of items, used when there are over a 100 items, but TIDAL
+        doesn't always allow more specifying a higher limit.
 
         Not meant for use outside of this library.
 
         :param url: TIDAL api endpoint where you get the objects.
         :param parse: The method that parses the data in the url
-        :return: A list of the object used for the parse argument.
+        item_List: List[Any] = []
         """
 
-        params = {
-            'offset': 0,
-            'limit': 100
-        }
+        params = {"offset": 0, "limit": 100}
         remaining = 100
-        item_list = []
+        item_list: List[Any] = []
         while remaining == 100:
             items = self.map_request(url, params=params, parse=parse)
             remaining = len(items)
-            params['offset'] += 100
+            params["offset"] += 100
             item_list.extend(items or [])
         return item_list
```

### Comparing `tidalapi-0.7.1/tidalapi/session.py` & `tidalapi-0.7.2/tidalapi/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,415 +12,470 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from __future__ import print_function
-from __future__ import unicode_literals
+from __future__ import annotations, print_function, unicode_literals
 
+import base64
 import concurrent.futures
 import datetime
-import base64
 import logging
 import random
 import time
 import uuid
+from dataclasses import dataclass
 from enum import Enum
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    List,
+    Literal,
+    NamedTuple,
+    Optional,
+    Union,
+    cast,
+    no_type_check,
+)
+from urllib.parse import urljoin
 
 import requests
 
-import tidalapi.playlist
-import tidalapi.request
-import tidalapi.user
-import tidalapi.media
-import tidalapi.artist
-import tidalapi.album
-import tidalapi.genre
-import tidalapi.mix
-
-try:
-    from urlparse import urljoin
-except ImportError:
-    from urllib.parse import urljoin
-
-log = logging.getLogger('__NAME__')
-
-SearchTypes = [tidalapi.artist.Artist,
-               tidalapi.album.Album,
-               tidalapi.media.Track,
-               tidalapi.media.Video,
-               tidalapi.playlist.Playlist,
-               None]
-
-
-class Quality(Enum):
-    lossless = 'LOSSLESS'
-    high = 'HIGH'
-    low = 'LOW'
-    master = 'HI_RES'
-
-
-class VideoQuality(Enum):
-    high = 'HIGH'
-    medium = 'MEDIUM'
-    low = 'LOW'
+if TYPE_CHECKING:
+    import tidalapi
+
+from . import album, artist, genre, media, mix, page, playlist, request, user
+
+log = logging.getLogger("__NAME__")
+SearchTypes: List[Optional[Any]] = [
+    artist.Artist,
+    album.Album,
+    media.Track,
+    media.Video,
+    playlist.Playlist,
+    None,
+]
 
 
 class LinkLogin(object):
-    """
-    The data required for logging in to TIDAL using a remote link, json is the data returned from TIDAL
-    """
+    """The data required for logging in to TIDAL using a remote link, json is the data
+    returned from TIDAL."""
+
     #: Amount of seconds until the code expires
     expires_in = None
     #: The code the user should enter at the uri
     user_code = None
     #: The link the user has to visit
     verification_uri = None
     #: The link the user has to visit, with the code already included
     verification_uri_complete = None
 
     def __init__(self, json):
-        self.expires_in = json['expiresIn']
-        self.user_code = json['userCode']
-        self.verification_uri = json['verificationUri']
-        self.verification_uri_complete = json['verificationUriComplete']
+        self.expires_in = json["expiresIn"]
+        self.user_code = json["userCode"]
+        self.verification_uri = json["verificationUri"]
+        self.verification_uri_complete = json["verificationUriComplete"]
 
 
 class Config(object):
-    """
-    Configuration for TIDAL services.
+    """Configuration for TIDAL services.
 
     The maximum item_limit is 10000, and some endpoints have a maximum of 100 items, which will be shown in the docs.
     In cases where the maximum is 100 items, you will have to use offsets to get more than 100 items.
     Note that changing the ALAC option requires you to log in again, and for you to create a new config object
     IMPORTANT: ALAC=false will mean that video streams turn into audio-only streams.
                Additionally, num_videos will turn into num_tracks in playlists.
     """
-    def __init__(self, quality=Quality.high, video_quality=VideoQuality.high, item_limit=1000, alac=True):
+
+    @no_type_check
+    def __init__(
+        self,
+        quality=media.Quality.high,
+        video_quality=media.VideoQuality.high,
+        item_limit=1000,
+        alac=True,
+    ):
         self.quality = quality.value
         self.video_quality = video_quality.value
-        self.api_location = 'https://api.tidal.com/v1/'
+        self.api_location = "https://api.tidal.com/v1/"
         self.image_url = "https://resources.tidal.com/images/%s/%ix%i.jpg"
         self.video_url = "https://resources.tidal.com/videos/%s/%ix%i.mp4"
 
         self.alac = alac
 
         if item_limit > 10000:
-            log.warning("Item limit was set above 10000, which is not supported by TIDAL, setting to 10000")
+            log.warning(
+                "Item limit was set above 10000, which is not supported by TIDAL, setting to 10000"
+            )
             self.item_limit = 10000
         else:
             self.item_limit = item_limit
 
-        self.api_token = \
-            eval(u'\x67\x6c\x6f\x62\x61\x6c\x73'.
-                 encode("437"))()[u"\x5f\x5f\x6e\x61\x6d\x65\x5f\x5f".
-                                  encode("".join(map(chr, [105, 105, 99, 115, 97][::-1]))).
-                                  decode("".join(map(chr, [117, 116, 70, 95, 56])))]
-        self.api_token += '.' + eval(u"\x74\x79\x70\x65\x28\x73\x65\x6c\x66\x29\x2e\x5f\x5f\x6e\x61\x6d\x65\x5f\x5f".
-                                     encode("".join(map(chr, [105, 105, 99, 115, 97][::-1]))).
-                                     decode("".join(map(chr, [117, 116, 70, 95, 56]))))
+        self.api_token = eval("\x67\x6c\x6f\x62\x61\x6c\x73".encode("437"))()[
+            "\x5f\x5f\x6e\x61\x6d\x65\x5f\x5f".encode(
+                "".join(map(chr, [105, 105, 99, 115, 97][::-1]))
+            ).decode("".join(map(chr, [117, 116, 70, 95, 56])))
+        ]
+        self.api_token += "." + eval(
+            "\x74\x79\x70\x65\x28\x73\x65\x6c\x66\x29\x2e\x5f\x5f\x6e\x61\x6d\x65\x5f\x5f".encode(
+                "".join(map(chr, [105, 105, 99, 115, 97][::-1]))
+            ).decode(
+                "".join(map(chr, [117, 116, 70, 95, 56]))
+            )
+        )
         token = self.api_token
         token = token[:8] + token[16:]
-        self.api_token = list((base64.b64decode("d3RjaThkamFfbHlhQnBKaWQuMkMwb3puT2ZtaXhnMA==").decode()))
-        tok = "".join(([chr(ord(x)-2) for x in token[-6:]]))
+        self.api_token = list(
+            (base64.b64decode("d3RjaThkamFfbHlhQnBKaWQuMkMwb3puT2ZtaXhnMA==").decode())
+        )
+        tok = "".join(([chr(ord(x) - 2) for x in token[-6:]]))
         token2 = token
         token = token[:9]
         token += tok
-        tok2 = "".join(([chr(ord(x)-2) for x in token[:-7]]))
+        tok2 = "".join(([chr(ord(x) - 2) for x in token[:-7]]))
         token = token[8:]
         token = tok2 + token
-        self.api_token = list((base64.b64decode("enJVZzRiWF9IalZfVm5rZ2MuMkF0bURsUGRvZzRldA==").decode()))
+        self.api_token = list(
+            (base64.b64decode("enJVZzRiWF9IalZfVm5rZ2MuMkF0bURsUGRvZzRldA==").decode())
+        )
         for word in token:
             self.api_token.remove(word)
         self.api_token = "".join(self.api_token)
         string = ""
         save = False
         if not isinstance(token2, str):
             save = True
-            string = "".encode('ISO-8859-1')
-            token2 = token2.encode('ISO-8859-1')
+            string = "".encode("ISO-8859-1")
+            token2 = token2.encode("ISO-8859-1")
         tok = string.join(([chr(ord(x) + 24) for x in token2[:-7]]))
         token2 = token2[8:]
         token2 = tok + token2
-        tok2 = string.join(([chr(ord(x)+23) for x in token2[-6:]]))
+        tok2 = string.join(([chr(ord(x) + 23) for x in token2[-6:]]))
         token2 = token2[:9]
         token2 += tok2
-        self.client_id = list((base64.b64decode("VoxKgUt8aHlEhEZ5cYhKgVAucVp2hnOFUH1WgE5+QlY2"
-                                                "dWtYVEptd2x2YnR0UDd3bE1scmM3MnNlND0=").decode('ISO-8859-1')))
+        self.client_id = list(
+            (
+                base64.b64decode(
+                    "VoxKgUt8aHlEhEZ5cYhKgVAucVp2hnOFUH1WgE5+QlY2"
+                    "dWtYVEptd2x2YnR0UDd3bE1scmM3MnNlND0="
+                ).decode("ISO-8859-1")
+            )
+        )
         if save:
-            token2.decode('ISO-8859-1').encode('utf-16')
-            self.client_id = [x.encode('ISO-8859-1') for x in self.client_id]
+            token2.decode("ISO-8859-1").encode("utf-16")
+            self.client_id = [x.encode("ISO-8859-1") for x in self.client_id]
         for word in token2:
             self.client_id.remove(word)
         self.client_id = "".join(self.client_id)
         self.client_secret = self.client_id
         self.client_id = self.api_token
 
 
 class Case(Enum):
     pascal = id
     scream = id
     lower = id
 
+    identifier: List[str]
+    type: List[Union[object, None]]
+    parse: List[Callable]
+
+
+TypeConversionKeys = Literal["identifier", "type", "parse"]
+
+
+@dataclass
+class TypeRelation:
+    identifier: str
+    type: Optional[Any]
+    parse: Callable
+
 
 class Session(object):
-    """
-    Object for interacting with the TIDAL api and
-    """
+    """Object for interacting with the TIDAL api and."""
 
     #: The TIDAL access token, this is what you use with load_oauth_session
     access_token = None
     #: A :class:`datetime` object containing the date the access token will expire
     expiry_time = None
     #: A refresh token for retrieving a new access token through refresh_token
     refresh_token = None
     #: The type of access token, e.g. Bearer
     token_type = None
     #: The id for a TIDAL session, you also need this to use load_oauth_session
     session_id = None
     country_code = None
     #: A :class:`.User` object containing the currently logged in user.
-    user = None
+    user: Union[user.FetchedUser, user.LoggedInUser, user.PlaylistCreator] = None
 
     def __init__(self, config=Config()):
         self.config = config
         self.request_session = requests.Session()
 
         # Objects for keeping the session across all modules.
-        self.request = tidalapi.Requests(session=self)
-        self.genre = tidalapi.Genre(session=self)
+        self.request = request.Requests(session=self)
+        self.genre = genre.Genre(session=self)
 
         self.parse_album = self.album().parse
         self.parse_artist = self.artist().parse_artist
         self.parse_artists = self.artist().parse_artists
         self.parse_playlist = self.playlist().parse
 
         self.parse_track = self.track().parse_track
         self.parse_video = self.video().parse_video
         self.parse_media = self.track().parse_media
         self.parse_mix = self.mix().parse
 
-        self.parse_user = tidalapi.User(self, None).parse
-        self.page = tidalapi.Page(self, None)
+        self.parse_user = user.User(self, None).parse
+        self.page = page.Page(self, None)
         self.parse_page = self.page.parse
 
         # Dictionary to convert between models from this library, to the text they, and to the parsing function.
         # It also helps in converting the other way around. All the information about artist is stored at the
         # Same index, which means you can get the index of the model, and then get the text using that index.
         # There probably is a better way to do this, but this was sadly the most readable way i found of doing it.
-        self.type_conversions = {
-            'identifier': ['artists', 'albums', 'tracks', 'videos', 'playlists', 'mixs'],
-            'type': SearchTypes,
-            'parse': [self.parse_artist, self.parse_album, self.parse_track,
-                      self.parse_video, self.parse_playlist, self.parse_mix]
-        }
-
-    def convert_type(self, search, search_type='identifier', output='identifier', case=Case.lower, suffix=True):
-        index = self.type_conversions[search_type].index(search)
-        result = self.type_conversions[output][index]
+        self.type_conversions: List[TypeRelation] = [
+            TypeRelation(identifier=identifier, type=type, parse=parse)
+            for identifier, type, parse in zip(
+                (
+                    "artists",
+                    "albums",
+                    "tracks",
+                    "videos",
+                    "playlists",
+                    "mixs",
+                ),
+                SearchTypes,
+                (
+                    self.parse_artist,
+                    self.parse_album,
+                    self.parse_track,
+                    self.parse_video,
+                    self.parse_playlist,
+                    self.parse_mix,
+                ),
+            )
+        ]
+
+    def convert_type(
+        self,
+        search,
+        search_type: TypeConversionKeys = "identifier",
+        output: TypeConversionKeys = "identifier",
+        case=Case.lower,
+        suffix=True,
+    ):
+        type_relations = next(
+            x for x in self.type_conversions if getattr(x, search_type) == search
+        )
+        result = getattr(type_relations, output)
 
-        if output == 'identifier':
+        if output == "identifier":
+            result = cast(str, result)
             if suffix is False:
-                result = result.strip('s')
+                result = result.strip("s")
             if case == Case.scream:
                 result = result.lower()
             elif case == Case.pascal:
                 result = result[0].upper() + result[1:]
 
         return result
 
     def load_session(self, session_id, country_code=None, user_id=None):
-        """
-        Establishes TIDAL login details using a previous session id.
-        May return true if the session-id is invalid/expired, you should verify the login afterwards.
+        """Establishes TIDAL login details using a previous session id. May return true
+        if the session-id is invalid/expired, you should verify the login afterwards.
 
         :param session_id: The UUID of the session you want to use.
         :param country_code: (Optional) Two-letter country code.
         :param user_id: (Optional) The number identifier of the user.
         :return: False if we know the session_id is incorrect, otherwise True
         """
         try:
             uuid.UUID(session_id)
         except ValueError:
             log.error("Session id did not have a valid UUID format")
             return False
 
         self.session_id = session_id
         if not user_id or not country_code:
-            request = self.request.request('GET', 'sessions').json()
-            country_code = request['countryCode']
-            user_id = request['userId']
+            request = self.request.request("GET", "sessions").json()
+            country_code = request["countryCode"]
+            user_id = request["userId"]
 
         self.country_code = country_code
-        self.user = tidalapi.User(self, user_id=user_id).factory()
+        self.user = user.User(self, user_id=user_id).factory()
         return True
 
-    def load_oauth_session(self, token_type, access_token, refresh_token=None, expiry_time=None):
-        """
-        Login to TIDAL using details from a previous OAuth login, automatically
+    def load_oauth_session(
+        self, token_type, access_token, refresh_token=None, expiry_time=None
+    ):
+        """Login to TIDAL using details from a previous OAuth login, automatically
         refreshes expired access tokens if refresh_token is supplied as well.
 
         :param token_type: The type of token, e.g. Bearer
         :param access_token: The access token received from an oauth login or refresh
-        :param refresh_token: (Optional) A refresh token that lets you get a new access token after it has expired
+        :param refresh_token: (Optional) A refresh token that lets you get a new access
+            token after it has expired
         :param expiry_time: (Optional) The datetime the access token will expire
         :return: True if we believe the log in was successful, otherwise false.
         """
         self.token_type = token_type
         self.access_token = access_token
         self.refresh_token = refresh_token
         self.expiry_time = expiry_time
 
-        request = self.request.request('GET', 'sessions')
+        request = self.request.request("GET", "sessions")
         json = request.json()
         if not request.ok:
             return False
 
-        self.session_id = json['sessionId']
-        self.country_code = json['countryCode']
-        self.user = tidalapi.User(self, user_id=json['userId']).factory()
+        self.session_id = json["sessionId"]
+        self.country_code = json["countryCode"]
+        self.user = user.User(self, user_id=json["userId"]).factory()
 
         return True
 
     def login(self, username, password):
-        """
-        Logs in to the TIDAL api.
+        """Logs in to the TIDAL api.
 
         :param username: The TIDAL username
         :param password: The password to your TIDAL account
         :return: Returns true if we think the login was successful.
         """
-        url = urljoin(self.config.api_location, 'login/username')
-        headers = {"X-Tidal-Token": self.config.api_token}
+        url = urljoin(self.config.api_location, "login/username")
+        headers: dict[str, str] = {"X-Tidal-Token": self.config.api_token}
         payload = {
-            'username': username,
-            'password': password,
-            'clientUniqueKey': format(random.getrandbits(64), '02x')
+            "username": username,
+            "password": password,
+            "clientUniqueKey": format(random.getrandbits(64), "02x"),
         }
         request = self.request_session.post(url, data=payload, headers=headers)
 
         if not request.ok:
             log.error("Login failed: %s", request.text)
             request.raise_for_status()
 
         body = request.json()
-        self.session_id = body['sessionId']
-        self.country_code = body['countryCode']
-        self.user = tidalapi.User(self, user_id=body['userId']).factory()
+        self.session_id = body["sessionId"]
+        self.country_code = body["countryCode"]
+        self.user = user.User(self, user_id=body["userId"]).factory()
         return True
 
     def login_oauth_simple(self, function=print):
-        """
-        Login to TIDAL using a remote link. You can select what function you want to use to display the link
+        """Login to TIDAL using a remote link. You can select what function you want to
+        use to display the link.
 
         :param function: The function you want to display the link with
         :raises: TimeoutError: If the login takes too long
         """
         login, future = self.login_oauth()
-        text = "Visit {0} to log in, the code will expire in {1} seconds"
+        text = "Visit https://{0} to log in, the code will expire in {1} seconds"
         function(text.format(login.verification_uri_complete, login.expires_in))
         future.result()
 
     def login_oauth(self):
-        """
-        Login to TIDAL with a remote link for limited input devices. The function will return everything you
-        need to log in through a web browser, and will return an future that will run until login.
+        """Login to TIDAL with a remote link for limited input devices. The function
+        will return everything you need to log in through a web browser, and will return
+        an future that will run until login.
 
         :return: A :class:`LinkLogin` object containing all the data needed to log in remotely, and
             a :class:`concurrent.futures.Future` that will poll until the login is completed, or until the link expires.
         :raises: TimeoutError: If the login takes too long
         """
         login, future = self._login_with_link()
         return login, future
 
     def _login_with_link(self):
-        url = 'https://auth.tidal.com/v1/oauth2/device_authorization'
-        params = {
-            'client_id': self.config.client_id,
-            'scope': 'r_usr w_usr w_sub'
-        }
+        url = "https://auth.tidal.com/v1/oauth2/device_authorization"
+        params = {"client_id": self.config.client_id, "scope": "r_usr w_usr w_sub"}
 
         request = self.request_session.post(url, params)
 
         if not request.ok:
             log.error("Login failed: %s", request.text)
             request.raise_for_status()
 
         json = request.json()
         executor = concurrent.futures.ThreadPoolExecutor()
         return LinkLogin(json), executor.submit(self._process_link_login, json)
 
     def _process_link_login(self, json):
         json = self._wait_for_link_login(json)
-        self.access_token = json['access_token']
-        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(seconds=json['expires_in'])
-        self.refresh_token = json['refresh_token']
-        self.token_type = json['token_type']
-        session = self.request.request('GET', 'sessions')
+        self.access_token = json["access_token"]
+        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(
+            seconds=json["expires_in"]
+        )
+        self.refresh_token = json["refresh_token"]
+        self.token_type = json["token_type"]
+        session = self.request.request("GET", "sessions")
         json = session.json()
-        self.session_id = json['sessionId']
-        self.country_code = json['countryCode']
-        self.user = tidalapi.User(self, user_id=json['userId']).factory()
+        self.session_id = json["sessionId"]
+        self.country_code = json["countryCode"]
+        self.user = user.User(self, user_id=json["userId"]).factory()
 
     def _wait_for_link_login(self, json):
-        expiry = json['expiresIn']
-        interval = json['interval']
-        device_code = json['deviceCode']
-        url = 'https://auth.tidal.com/v1/oauth2/token'
+        expiry = json["expiresIn"]
+        interval = json["interval"]
+        device_code = json["deviceCode"]
+        url = "https://auth.tidal.com/v1/oauth2/token"
         params = {
-            'client_id': self.config.client_id,
-            'client_secret': self.config.client_secret,
-            'device_code': device_code,
-            'grant_type': 'urn:ietf:params:oauth:grant-type:device_code',
-            'scope': 'r_usr w_usr w_sub'
+            "client_id": self.config.client_id,
+            "client_secret": self.config.client_secret,
+            "device_code": device_code,
+            "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
+            "scope": "r_usr w_usr w_sub",
         }
         while expiry > 0:
             request = self.request_session.post(url, params)
             json = request.json()
             if request.ok:
                 return json
             # Because the requests take time, the expiry variable won't be accurate, so stop if TIDAL says it's expired
-            if json['error'] == 'expired_token':
+            if json["error"] == "expired_token":
                 break
             time.sleep(interval)
             expiry = expiry - interval
 
-        raise TimeoutError('You took too long to log in')
+        raise TimeoutError("You took too long to log in")
 
     def token_refresh(self, refresh_token):
-        """
-        Retrieves a new access token using the specified parameters, updating the current access token
+        """Retrieves a new access token using the specified parameters, updating the
+        current access token.
 
         :param refresh_token: The refresh token retrieved when using the OAuth login.
-        :return: True if we believe the token was successfully refreshed, otherwise False
+        :return: True if we believe the token was successfully refreshed, otherwise
+            False
         """
-        url = 'https://auth.tidal.com/v1/oauth2/token'
+        url = "https://auth.tidal.com/v1/oauth2/token"
         params = {
-            'grant_type': 'refresh_token',
-            'refresh_token': refresh_token,
-            'client_id': self.config.client_id,
-            'client_secret': self.config.client_secret
+            "grant_type": "refresh_token",
+            "refresh_token": refresh_token,
+            "client_id": self.config.client_id,
+            "client_secret": self.config.client_secret,
         }
 
         request = self.request_session.post(url, params)
         json = request.json()
         if not request.ok:
             log.warning("The refresh token has expired, a new login is required.")
             return False
-        self.access_token = json['access_token']
-        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(seconds=json['expires_in'])
-        self.token_type = json['token_type']
+        self.access_token = json["access_token"]
+        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(
+            seconds=json["expires_in"]
+        )
+        self.token_type = json["token_type"]
         return True
 
     def search(self, query, models=None, limit=50, offset=0):
-        """
-        Searches TIDAL with the specified query, you can also specify what models you want to search for.
-        While you can set the offset, there aren't more than 300 items available in a search.
+        """Searches TIDAL with the specified query, you can also specify what models you
+        want to search for. While you can set the offset, there aren't more than 300
+        items available in a search.
 
         :param query: The string you want to search for
         :param models: A list of tidalapi models you want to include in the search.
             Valid models are :class:`.Artist`, :class:`.Album`, :class:`.Track`, :class:`.Video`, :class:`.Playlist`
         :param limit: The amount of items you want included, up to 300.
         :param offset: The index you want to start searching at.
         :return: Returns a dictionary of the different models, with the dictionary values containing the search results.
@@ -430,132 +485,141 @@
             models = SearchTypes
 
         types = []
         # This converts the specified TIDAL models in the models list into the text versions so we can parse it.
         for model in models:
             if model not in SearchTypes:
                 raise ValueError("Tried to search for an invalid type")
-            types.append(self.convert_type(model, 'type'))
+            types.append(self.convert_type(model, "type"))
 
         params = {
-            'query': query,
-            'limit': limit,
-            'offset': offset,
-            'types': ",".join(types)
+            "query": query,
+            "limit": limit,
+            "offset": offset,
+            "types": ",".join(types),
         }
 
-        json_obj = self.request.request('GET', 'search', params=params).json()
+        json_obj = self.request.request("GET", "search", params=params).json()
 
         result = {
-            'artists': self.request.map_json(json_obj['artists'], self.parse_artist),
-            'albums': self.request.map_json(json_obj['albums'], self.parse_album),
-            'tracks': self.request.map_json(json_obj['tracks'], self.parse_track),
-            'videos': self.request.map_json(json_obj['videos'], self.parse_video),
-            'playlists': self.request.map_json(json_obj['playlists'], self.parse_playlist)
+            "artists": self.request.map_json(json_obj["artists"], self.parse_artist),
+            "albums": self.request.map_json(json_obj["albums"], self.parse_album),
+            "tracks": self.request.map_json(json_obj["tracks"], self.parse_track),
+            "videos": self.request.map_json(json_obj["videos"], self.parse_video),
+            "playlists": self.request.map_json(
+                json_obj["playlists"], self.parse_playlist
+            ),
         }
 
         # Find the type of the top hit so we can parse it
-        if json_obj['topHit']:
-            top_type = json_obj['topHit']['type'].lower()
-            parse = self.convert_type(top_type, output='parse')
-            result['top_hit'] = self.request.map_json(json_obj['topHit']['value'], parse)
+        if json_obj["topHit"]:
+            top_type = json_obj["topHit"]["type"].lower()
+            parse = self.convert_type(top_type, output="parse")
+            result["top_hit"] = self.request.map_json(
+                json_obj["topHit"]["value"], parse
+            )
         else:
-            result['top_hit'] = None
+            result["top_hit"] = None
 
         return result
 
     def check_login(self):
-        """ Returns true if current session is valid, false otherwise. """
+        """Returns true if current session is valid, false otherwise."""
         if self.user is None or not self.user.id or not self.session_id:
             return False
-        return self.request.basic_request('GET', 'users/%s/subscription' % self.user.id).ok
-
-    def playlist(self, playlist_id=None):
-        """
-        Function to create a playlist object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.Playlist(session=session, playlist_id=playlist_id) <.Playlist>` internally
+        return self.request.basic_request(
+            "GET", "users/%s/subscription" % self.user.id
+        ).ok
+
+    def playlist(
+        self, playlist_id=None
+    ) -> Union[tidalapi.Playlist, tidalapi.UserPlaylist]:
+        """Function to create a playlist object with access to the session instance in a
+        smoother way. Calls :class:`tidalapi.Playlist(session=session,
+        playlist_id=playlist_id) <.Playlist>` internally.
 
         :param playlist_id: (Optional) The TIDAL id of the playlist. You may want access to the methods without an id.
         :return: Returns a :class:`.Playlist` object that has access to the session instance used.
         """
 
-        return tidalapi.Playlist(session=self, playlist_id=playlist_id).factory()
+        return playlist.Playlist(session=self, playlist_id=playlist_id).factory()
 
-    def track(self, track_id=None, with_album=False):
-        """
-        Function to create a Track object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.Track(session=session, track_id=track_id) <.Track>` internally
+    def track(self, track_id=None, with_album=False) -> tidalapi.Track:
+        """Function to create a Track object with access to the session instance in a
+        smoother way. Calls :class:`tidalapi.Track(session=session, track_id=track_id)
+        <.Track>` internally.
 
         :param track_id: (Optional) The TIDAL id of the Track. You may want access to the methods without an id.
         :param with_album: (Optional) Whether to fetch the complete :class:`.Album` for the track or not
         :return: Returns a :class:`.Track` object that has access to the session instance used.
         """
 
-        item = tidalapi.Track(session=self, media_id=track_id)
+        item = media.Track(session=self, media_id=track_id)
         if item.album and with_album:
             album = self.album(item.album.id)
             if album:
                 item.album = album
 
         return item
 
-    def video(self, video_id=None):
-        """
-        Function to create a Video object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.Video(session=session, video_id=video_id) <.Video>` internally
+    def video(self, video_id=None) -> tidalapi.Video:
+        """Function to create a Video object with access to the session instance in a
+        smoother way. Calls :class:`tidalapi.Video(session=session, video_id=video_id)
+        <.Video>` internally.
 
         :param video_id: (Optional) The TIDAL id of the Video. You may want access to the methods without an id.
         :return: Returns a :class:`.Video` object that has access to the session instance used.
         """
 
-        return tidalapi.Video(session=self, media_id=video_id)
+        return media.Video(session=self, media_id=video_id)
 
-    def artist(self, artist_id=None):
-        """
-        Function to create a Artist object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.Artist(session=session, artist_id=artist_id) <.Artist>` internally
+    def artist(self, artist_id: Optional[str] = None) -> tidalapi.Artist:
+        """Function to create a Artist object with access to the session instance in a
+        smoother way. Calls :class:`tidalapi.Artist(session=session,
+        artist_id=artist_id) <.Artist>` internally.
 
         :param artist_id: (Optional) The TIDAL id of the Artist. You may want access to the methods without an id.
         :return: Returns a :class:`.Artist` object that has access to the session instance used.
         """
 
-        return tidalapi.Artist(session=self, artist_id=artist_id)
+        return artist.Artist(session=self, artist_id=artist_id)
 
-    def album(self, album_id=None):
-        """
-        Function to create a Album object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.Album(session=session, album_id=album_id) <.Album>` internally
+    def album(self, album_id: Optional[str] = None) -> tidalapi.Album:
+        """Function to create a Album object with access to the session instance in a
+        smoother way. Calls :class:`tidalapi.Album(session=session, album_id=album_id)
+        <.Album>` internally.
 
         :param album_id: (Optional) The TIDAL id of the Album. You may want access to the methods without an id.
         :return: Returns a :class:`.Album` object that has access to the session instance used.
         """
 
-        return tidalapi.Album(session=self, album_id=album_id)
+        return album.Album(session=self, album_id=album_id)
 
-    def mix(self, mix_id=None):
-        """
-        Function to create a mix object with access to the session instance smoothly
-        Calls :class:`tidalapi.Mix(session=session, mix_id=mix_id) <.Album>` internally
+    def mix(self, mix_id=None) -> tidalapi.Mix:
+        """Function to create a mix object with access to the session instance smoothly
+        Calls :class:`tidalapi.Mix(session=session, mix_id=mix_id) <.Album>` internally.
 
         :param mix_id: (Optional) The TIDAL id of the Mix. You may want access to the mix methods without an id.
         :return: Returns a :class:`.Mix` object that has access to the session instance used.
         """
 
-        return tidalapi.Mix(session=self, mix_id=mix_id)
+        return mix.Mix(session=self, mix_id=mix_id)
 
-    def get_user(self, user_id=None):
-        """
-        Function to create a User object with access to the session instance in a smoother way.
-        Calls :class:`tidalapi.User(session=session, user_id=user_id) <.User>` internally
+    def get_user(
+        self, user_id=None
+    ) -> Union[tidalapi.FetchedUser, tidalapi.LoggedInUser, tidalapi.PlaylistCreator]:
+        """Function to create a User object with access to the session instance in a
+        smoother way. Calls :class:`user.User(session=session, user_id=user_id) <.User>`
+        internally.
 
         :param user_id: (Optional) The TIDAL id of the User. You may want access to the methods without an id.
         :return: Returns a :class:`.User` object that has access to the session instance used.
         """
 
-        return tidalapi.User(session=self, user_id=user_id).factory()
+        return user.User(session=self, user_id=user_id).factory()
 
     def home(self):
         """
         Retrieves the Home page, as seen on https://listen.tidal.com
 
         :return: A :class:`.Page` object with the :class:`.PageCategory` list from the home page
         """
```

### Comparing `tidalapi-0.7.1/tidalapi/user.py` & `tidalapi-0.7.2/tidalapi/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-A module containing classes and functions related to tidal users.
+"""A module containing classes and functions related to tidal users.
 
 :class:`User` is a class with user information.
 :class:`Favorites` is class with a users favorites.
 """
 
+from __future__ import annotations
+
 from copy import copy
-import dateutil.parser
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
+
+if TYPE_CHECKING:
+    from . import playlist
 
 
 class User(object):
-    """
-    A class containing various information about a TIDAL user.
+    """A class containing various information about a TIDAL user.
 
-    The attributes of this class are pretty varied. ID is the only attribute you can rely on being set.
-    If you initialized a specific user, you will get id, first_name, last_name, and picture_id.
-    If parsed as a playlist creator, you will get an ID and a name, if the creator isn't an artist, name will be 'user'.
-    If the parsed user is the one logged in, for example in session.user, you will get the remaining attributes, and id.
+    The attributes of this class are pretty varied. ID is the only attribute you can
+    rely on being set. If you initialized a specific user, you will get id, first_name,
+    last_name, and picture_id. If parsed as a playlist creator, you will get an ID and a
+    name, if the creator isn't an artist, name will be 'user'. If the parsed user is the
+    one logged in, for example in session.user, you will get the remaining attributes,
+    and id.
     """
 
     id = -1
 
     def __init__(self, session, user_id):
         self.id = user_id
         self.session = session
@@ -46,15 +50,17 @@
         self.playlist = session.playlist()
 
     def factory(self):
         return self.request.map_request("users/%s" % self.id, parse=self.parse)
 
     def parse(self, json_obj):
         if "username" in json_obj:
-            user = LoggedInUser(self.session, json_obj["id"])
+            user: Union[LoggedInUser, FetchedUser, PlaylistCreator] = LoggedInUser(
+                self.session, json_obj["id"]
+            )
 
         elif "firstName" in json_obj:
             user = FetchedUser(self.session, json_obj["id"])
 
         elif json_obj:
             user = PlaylistCreator(self.session, json_obj["id"])
 
@@ -62,80 +68,69 @@
         else:
             user = PlaylistCreator(self.session, 0)
 
         return user.parse(json_obj)
 
 
 class FetchedUser(User):
-    first_name = None
-    last_name = None
-    picture_id = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    picture_id: Optional[str] = None
 
     def parse(self, json_obj):
         self.id = json_obj["id"]
         self.first_name = json_obj["firstName"]
         self.last_name = json_obj["lastName"]
         self.picture_id = json_obj.get("picture", None)
 
         return copy(self)
 
     def image(self, dimensions):
         if dimensions not in [100, 210, 600]:
             raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
 
+        if self.picture_id is None:
+            raise AttributeError("No picture available")
+
         return self.session.config.image_url % (
             self.picture_id.replace("-", "/"),
             dimensions,
             dimensions,
         )
 
 
 class LoggedInUser(FetchedUser):
-    username = None
-    email = None
-    created = None
-    newsletter = None
-    accepted_eula = None
-    gender = None
-    date_of_birth = None
-    facebook_uid = None
-    apple_uid = None
+    username: Optional[str] = None
+    email: Optional[str] = None
+    profile_metadata: Optional[Dict] = None
 
     def __init__(self, session, user_id):
         super(LoggedInUser, self).__init__(session, user_id)
         self.favorites = Favorites(session, self.id)
 
     def parse(self, json_obj):
         super(LoggedInUser, self).parse(json_obj)
         self.username = json_obj["username"]
         self.email = json_obj["email"]
-        self.created = dateutil.parser.isoparse(json_obj["created"])
-        self.newsletter = json_obj["newsletter"]
-        self.accepted_eula = json_obj["acceptedEULA"]
-        self.gender = json_obj["gender"]
-        self.date_of_birth = json_obj["dateOfBirth"]
-        self.facebook_uid = json_obj["facebookUid"]
-        self.apple_uid = json_obj["appleUid"]
+        self.profile_metadata = json_obj
 
         return copy(self)
 
-    def playlists(self):
-        """
-        Get the playlists created by the user.
+    def playlists(self) -> List[Union[playlist.Playlist, playlist.UserPlaylist]]:
+        """Get the playlists created by the user.
 
         :return: Returns a list of :class:`~tidalapi.playlist.Playlist` objects containing the playlists.
         """
         return self.request.map_request(
             "users/%s/playlists" % self.id, parse=self.playlist.parse_factory
         )
 
     def playlist_and_favorite_playlists(self, offset=0):
-        """
-        Get the playlists created by the user, and the playlists favorited by the user.
-        This function is limited to 50 by TIDAL, requiring pagination.
+        """Get the playlists created by the user, and the playlists favorited by the
+        user. This function is limited to 50 by TIDAL, requiring pagination.
 
         :return: Returns a list of :class:`~tidalapi.playlist.Playlist` objects containing the playlists.
         """
         params = {"limit": 50, "offset": offset}
         endpoint = "users/%s/playlistsAndFavoritePlaylists" % self.id
         json_obj = self.request.request("GET", endpoint, params=params).json()
 
@@ -171,186 +166,168 @@
         else:
             self.name = "user"
 
         return copy(self)
 
 
 class Favorites(object):
-    """
-    An object containing a users favourites.
-    """
+    """An object containing a users favourites."""
 
     def __init__(self, session, user_id):
         self.session = session
         self.requests = session.request
         self.base_url = "users/%s/favorites" % user_id
 
     def add_album(self, album_id):
-        """
-        Adds an album to the users favorites.
+        """Adds an album to the users favorites.
 
         :param album_id: TIDAL's identifier of the album.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "POST", self.base_url + "/albums", data={"albumId": album_id}
         ).ok
 
     def add_artist(self, artist_id):
-        """
-        Adds an artist to the users favorites.
+        """Adds an artist to the users favorites.
 
         :param artist_id: TIDAL's identifier of the artist
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "POST", self.base_url + "/artists", data={"artistId": artist_id}
         ).ok
 
     def add_playlist(self, playlist_id):
-        """
-        Adds a playlist to the users favorites.
+        """Adds a playlist to the users favorites.
 
-        :param playlist_id:  TIDAL's identifier of the playlist.
+        :param playlist_id: TIDAL's identifier of the playlist.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "POST", self.base_url + "/playlists", data={"uuids": playlist_id}
         ).ok
 
     def add_track(self, track_id):
-        """
-        Adds a track to the users favorites.
+        """Adds a track to the users favorites.
 
         :param track_id: TIDAL's identifier of the track.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "POST", self.base_url + "/tracks", data={"trackId": track_id}
         ).ok
 
     def add_video(self, video_id):
-        """
-        Adds a video to the users favorites.
+        """Adds a video to the users favorites.
 
         :param video_id: TIDAL's identifier of the video.
         :return: A boolean indicating whether the request was successful or not.
         """
         params = {"limit": "100"}
         return self.requests.request(
             "POST",
             self.base_url + "/videos",
             data={"videoIds": video_id},
             params=params,
         ).ok
 
     def remove_artist(self, artist_id):
-        """
-        Removes a track from the users favorites.
+        """Removes a track from the users favorites.
 
         :param artist_id: TIDAL's identifier of the artist.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "DELETE", self.base_url + "/artists/%s" % artist_id
         ).ok
 
     def remove_album(self, album_id):
-        """
-        Removes an album from the users favorites.
+        """Removes an album from the users favorites.
 
         :param album_id: TIDAL's identifier of the album
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "DELETE", self.base_url + "/albums/%s" % album_id
         ).ok
 
     def remove_playlist(self, playlist_id):
-        """
-        Removes a playlist from the users favorites.
+        """Removes a playlist from the users favorites.
 
         :param playlist_id: TIDAL's identifier of the playlist.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "DELETE", self.base_url + "/playlists/%s" % playlist_id
         ).ok
 
     def remove_track(self, track_id):
-        """
-        Removes a track from the users favorites.
+        """Removes a track from the users favorites.
 
         :param track_id: TIDAL's identifier of the track.
         :return: A boolean indicating whether the request was successful or not.
         """
         return self.requests.request(
             "DELETE", self.base_url + "/tracks/%s" % track_id
         ).ok
 
     def remove_video(self, video_id):
-        """
-        Removes a video from the users favorites.
+        """Removes a video from the users favorites.
 
         :param video_id: TIDAL's identifier of the video.
         :return: A boolean indicating whether the request was successful or not.
-
         """
         return self.requests.request(
             "DELETE", self.base_url + "/videos/%s" % video_id
         ).ok
 
     def artists(self, limit=None, offset=0):
-        """
-        Get the users favorite artists
+        """Get the users favorite artists.
 
         :return: A :class:`list` of :class:`~tidalapi.artist.Artist` objects containing the favorite artists.
         """
         params = {"limit": limit, "offset": offset}
         return self.requests.map_request(
             self.base_url + "/artists", params=params, parse=self.session.parse_artist
         )
 
     def albums(self, limit=None, offset=0):
-        """
-        Get the users favorite albums
+        """Get the users favorite albums.
 
         :return: A :class:`list` of :class:`~tidalapi.album.Album` objects containing the favorite albums.
         """
         params = {"limit": limit, "offset": offset}
         return self.requests.map_request(
             self.base_url + "/albums", params=params, parse=self.session.parse_album
         )
 
     def playlists(self, limit=None, offset=0):
-        """
-        Get the users favorite playlists
+        """Get the users favorite playlists.
 
         :return: A :class:`list` :class:`~tidalapi.playlist.Playlist` objects containing the favorite playlists.
         """
         params = {"limit": limit, "offset": offset}
         return self.requests.map_request(
             self.base_url + "/playlists",
             params=params,
             parse=self.session.parse_playlist,
         )
 
     def tracks(self, limit=None, offset=0):
-        """
-        Get the users favorite tracks
+        """Get the users favorite tracks.
 
         :return: A :class:`list` of :class:`~tidalapi.track.Track` objects containing all of the favorite tracks.
         """
         params = {"limit": limit, "offset": offset}
         return self.requests.map_request(
             self.base_url + "/tracks", params=params, parse=self.session.parse_track
         )
 
     def videos(self):
-        """
-        Get the users favorite videos
+        """Get the users favorite videos.
 
         :return: A :class:`list` of :class:`~tidalapi.media.Video` objects containing all the favorite videos
         """
         return self.requests.get_items(
             self.base_url + "/videos", parse=self.session.parse_media
         )
```

