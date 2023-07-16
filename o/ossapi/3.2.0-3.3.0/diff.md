# Comparing `tmp/ossapi-3.2.0.tar.gz` & `tmp/ossapi-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.2.0.tar", last modified: Sat May 27 00:17:15 2023, max compression
+gzip compressed data, was "ossapi-3.3.0.tar", last modified: Sun Jul 16 05:16:59 2023, max compression
```

## Comparing `ossapi-3.2.0.tar` & `ossapi-3.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.039376 ossapi-3.2.0/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.2.0/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-05-27 00:17:15.039150 ossapi-3.2.0/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-05-27 00:03:28.000000 ossapi-3.2.0/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.037145 ossapi-3.2.0/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3882 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.2.0/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-18 20:48:22.000000 ossapi-3.2.0/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-04-18 20:48:16.000000 ossapi-3.2.0/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-04-29 22:39:56.000000 ossapi-3.2.0/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    87037 2023-05-27 00:14:44.000000 ossapi-3.2.0/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    89789 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.2.0/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-04-29 20:32:03.000000 ossapi-3.2.0/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.037961 ossapi-3.2.0/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-05-27 00:14:54.000000 ossapi-3.2.0/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-05-27 00:17:15.039418 ossapi-3.2.0/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.038892 ossapi-3.2.0/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.2.0/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.2.0/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)    10591 2023-05-27 00:03:28.000000 ossapi-3.2.0/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-29 20:32:03.000000 ossapi-3.2.0/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.2.0/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.231699 ossapi-3.3.0/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.3.0/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10291 2023-07-16 05:16:59.231436 ossapi-3.3.0/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9784 2023-07-16 04:59:00.000000 ossapi-3.3.0/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.227842 ossapi-3.3.0/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3990 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.3.0/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    17243 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-04-18 20:48:16.000000 ossapi-3.3.0/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36554 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-06-05 19:43:51.000000 ossapi-3.3.0/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    87794 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    92896 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.3.0/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-05-28 18:35:43.000000 ossapi-3.3.0/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.229058 ossapi-3.3.0/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10291 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-07-16 05:00:22.000000 ossapi-3.3.0/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-07-16 05:16:59.231762 ossapi-3.3.0/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.231076 ossapi-3.3.0/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.3.0/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.3.0/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11001 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_v1.py
```

### Comparing `ossapi-3.2.0/LICENSE` & `ossapi-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/PKG-INFO` & `ossapi-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.2.0
+Version: 3.3.0
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: async
 License-File: LICENSE
 
 # ossapi ([documentation](https://circleguard.github.io/ossapi/)) [![PyPI version](https://badge.fury.io/py/ossapi.svg)](https://pypi.org/project/ossapi/)
 
-ossapi is a python wrapper for the osu! api which has complete coverage of both [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki). ossapi provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
+ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
+* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
   * [Forums](#endpoints-forums)
@@ -69,15 +70,15 @@
 ```python
 from ossapi import Ossapi
 
 # create a new client at https://osu.ppy.sh/home/account/edit#oauth
 api = Ossapi(client_id, client_secret)
 
 # see docs for full list of endpoints
-print(api.user("tybug2").username)
+print(api.user("tybug").username)
 print(api.user(12092800, mode="osu").username)
 print(api.beatmap(221777).id)
 ```
 
 ## Async
 
 ossapi provides an async variant, `OssapiAsync`, which has an identical interface to `Ossapi`:
@@ -85,21 +86,37 @@
 ```python
 import asyncio
 from ossapi import Ossapi
 
 api = Ossapi(client_id, client_secret)
 
 async def main():
-    await api.user("tybug2")
+    await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://circleguard.github.io/ossapi/async.html)
 
+## Lazer
+
+You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+
+```python
+from ossapi import Ossapi
+
+api_lazer = Ossapi(client_id, client_secret, domain="lazer")
+
+# best score on the lazer server (lazer + osu scores combined)
+scores = api_lazer.user_scores(12092800, "best")
+print(scores[0].pp)
+```
+
+[Read more about domains on the docs.](https://circleguard.github.io/ossapi/domains.html)
+
 ## Endpoints
 
 All endpoints for api v2.
 
 * Beatmaps<a name="endpoints-beatmaps"></a>
   * [`api.beatmap`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap)
   * [`api.beatmap_attributes`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap_attributes)
@@ -166,15 +183,15 @@
   * [`api.user_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.user_scores)
   * [`api.users`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.users)
 * Wiki<a name="endpoints-wiki"></a>
   * [`api.wiki_page`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.wiki_page)
 
 ## API v1 Usage
 
-You can get your api v1 key at <https://osu.ppy.sh/p/api/>. Note that due to a [redirection bug](https://github.com/ppy/osu-web/issues/2867), you may need to log in and wait 30 seconds before being able to access the api page through the above link.
+You can get your api v1 key at <https://osu.ppy.sh/home/account/edit#legacy-api>.
 
 Basic usage:
 
 ```python
 from ossapi import OssapiV1
 
 api = OssapiV1("key")
```

### Comparing `ossapi-3.2.0/README.md` & `ossapi-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # ossapi ([documentation](https://circleguard.github.io/ossapi/)) [![PyPI version](https://badge.fury.io/py/ossapi.svg)](https://pypi.org/project/ossapi/)
 
-ossapi is a python wrapper for the osu! api which has complete coverage of both [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki). ossapi provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
+ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
+* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
   * [Forums](#endpoints-forums)
@@ -55,15 +56,15 @@
 ```python
 from ossapi import Ossapi
 
 # create a new client at https://osu.ppy.sh/home/account/edit#oauth
 api = Ossapi(client_id, client_secret)
 
 # see docs for full list of endpoints
-print(api.user("tybug2").username)
+print(api.user("tybug").username)
 print(api.user(12092800, mode="osu").username)
 print(api.beatmap(221777).id)
 ```
 
 ## Async
 
 ossapi provides an async variant, `OssapiAsync`, which has an identical interface to `Ossapi`:
@@ -71,21 +72,37 @@
 ```python
 import asyncio
 from ossapi import Ossapi
 
 api = Ossapi(client_id, client_secret)
 
 async def main():
-    await api.user("tybug2")
+    await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://circleguard.github.io/ossapi/async.html)
 
+## Lazer
+
+You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+
+```python
+from ossapi import Ossapi
+
+api_lazer = Ossapi(client_id, client_secret, domain="lazer")
+
+# best score on the lazer server (lazer + osu scores combined)
+scores = api_lazer.user_scores(12092800, "best")
+print(scores[0].pp)
+```
+
+[Read more about domains on the docs.](https://circleguard.github.io/ossapi/domains.html)
+
 ## Endpoints
 
 All endpoints for api v2.
 
 * Beatmaps<a name="endpoints-beatmaps"></a>
   * [`api.beatmap`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap)
   * [`api.beatmap_attributes`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap_attributes)
@@ -152,15 +169,15 @@
   * [`api.user_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.user_scores)
   * [`api.users`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.users)
 * Wiki<a name="endpoints-wiki"></a>
   * [`api.wiki_page`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.wiki_page)
 
 ## API v1 Usage
 
-You can get your api v1 key at <https://osu.ppy.sh/p/api/>. Note that due to a [redirection bug](https://github.com/ppy/osu-web/issues/2867), you may need to log in and wait 30 seconds before being able to access the api page through the above link.
+You can get your api v1 key at <https://osu.ppy.sh/home/account/edit#legacy-api>.
 
 Basic usage:
 
 ```python
 from ossapi import OssapiV1
 
 api = OssapiV1("key")
```

### Comparing `ossapi-3.2.0/ossapi/__init__.py` & `ossapi-3.3.0/ossapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
     Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
     ChangelogListing, MultiplayerScores,
     BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
     UserCompact, BeatmapsetCompact, ForumPoll, Room, RoomPlaylistItem,
     RoomPlaylistItemMod, RoomLeaderboardScore, RoomLeaderboardUserScore,
     RoomLeaderboard, Match, Matches, MatchResponse, ScoreMatchInfo, MatchGame,
-    MatchEventDetail, MatchEvent, ScoringType, TeamType)
+    MatchEventDetail, MatchEvent, ScoringType, TeamType, StatisticsVariant,
+    Events)
 from ossapi.enums import (GameMode, ScoreType, RankingFilter, RankingType,
     UserBeatmapType, BeatmapDiscussionPostSort, UserLookupKey,
     BeatmapsetEventType, CommentableType, CommentSort, ForumTopicSort,
     SearchMode, MultiplayerScoresSort, BeatmapsetDiscussionVote,
     BeatmapsetDiscussionVoteSort, BeatmapsetStatus, MessageType,
     BeatmapsetSearchCategory, BeatmapsetSearchMode,
     BeatmapsetSearchExplicitContent, BeatmapsetSearchLanguage,
     BeatmapsetSearchGenre, NewsPostKey, BeatmapsetSearchSort, RoomType,
-    RoomCategory, RoomSearchType, MatchEventType)
+    RoomCategory, RoomSearchType, MatchEventType, Variant, EventsSort)
 from ossapi.mod import Mod
 from ossapi.replay import Replay
 from ossapi.encoder import ModelEncoder, serialize_model
 from ossapi.ossapiv2_async import OssapiAsync
 
 from oauthlib.oauth2 import AccessDeniedError, TokenExpiredError
 from oauthlib.oauth2.rfc6749.errors import InsufficientScopeError
@@ -51,25 +52,25 @@
     "Spotlights", "WikiPage", "_Event", "Event", "BeatmapsetDiscussionPosts",
     "Build", "ChangelogListing", "MultiplayerScores",
     "BeatmapsetDiscussionVotes", "CreatePMResponse",
     "BeatmapsetDiscussions", "UserCompact", "BeatmapsetCompact", "ForumPoll",
     "Room", "RoomPlaylistItem", "RoomPlaylistItemMod", "RoomLeaderboardScore",
     "RoomLeaderboardUserScore", "RoomLeaderboard", "Match", "Matches",
     "MatchResponse", "ScoreMatchInfo", "MatchGame", "MatchEventDetail",
-    "MatchEvent",
+    "MatchEvent", "StatisticsVariant", "Events",
     # OssapiV2 enums
     "GameMode", "ScoreType", "RankingFilter", "RankingType",
     "UserBeatmapType", "BeatmapDiscussionPostSort", "UserLookupKey",
     "BeatmapsetEventType", "CommentableType", "CommentSort", "ForumTopicSort",
     "SearchMode", "MultiplayerScoresSort", "BeatmapsetDiscussionVote",
     "BeatmapsetDiscussionVoteSort", "BeatmapsetStatus", "MessageType",
     "BeatmapsetSearchCategory", "BeatmapsetSearchMode",
     "BeatmapsetSearchExplicitContent", "BeatmapsetSearchLanguage",
     "BeatmapsetSearchGenre", "NewsPostKey", "BeatmapsetSearchSort", "RoomType",
     "RoomCategory", "RoomSearchType", "MatchEventType", "ScoringType",
-    "TeamType",
+    "TeamType", "Variant", "EventsSort",
     # OssapiV2 exceptions
     "AccessDeniedError", "TokenExpiredError", "InsufficientScopeError",
     # misc
     "Mod", "Replay", "__version__", "ModelEncoder",
     "serialize_model"
 ]
```

### Comparing `ossapi-3.2.0/ossapi/encoder.py` & `ossapi-3.3.0/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/ossapi/enums.py` & `ossapi-3.3.0/ossapi/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,16 @@
 
 class UserAccountHistoryType(EnumModel):
     NOTE = "note"
     RESTRICTION = "restriction"
     SILENCE = "silence"
 
 class MessageType(EnumModel):
-    DISQUALIFY = "disqualify"
     HYPE = "hype"
     MAPPER_NOTE = "mapper_note"
-    NOMINATION_RESET = "nomination_reset"
     PRAISE = "praise"
     PROBLEM = "problem"
     REVIEW = "review"
     SUGGESTION = "suggestion"
 
 class BeatmapsetEventType(EnumModel):
     APPROVE =  "approve"
@@ -213,14 +211,15 @@
     TEAM_VERSUS = "team_versus"
 
 class RoomCategory(EnumModel):
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d
     # 430a2/resources/js/interfaces/room-json.ts#L7
     NORMAL = "normal"
     SPOTLIGHT = "spotlight"
+    FEATURED_ARTIST = "featured_artist"
 
 class MatchEventType(EnumModel):
     # https://github.dev/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2
     # d430a2/app/Models/LegacyMatch/Event.php#L30
     PLAYER_LEFT = "player-left"
     PLAYER_JOINED = "player-joined"
     PLAYER_KICKED = "player-kicked"
@@ -242,14 +241,18 @@
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d43
     # 0a2/app/Models/LegacyMatch/Game.php#L47
     HEAD_TO_HEAD = "head-to-head"
     TAG_COOP = "tag-coop"
     TEAM_VS = "team-vs"
     TAG_TEAM_VS = "tag-team-vs"
 
+class Variant(EnumModel):
+    # can't start a python identifier with an integer
+    KEY_4 = "4k"
+    KEY_7 = "7k"
 
 
 # ===============
 # Parameter Enums
 # ===============
 
 class ScoreType(EnumModel):
@@ -294,14 +297,15 @@
     PUBLIC = "PUBLIC"
     PRIVATE = "PRIVATE"
     MULTIPLAYER = "MULTIPLAYER"
     SPECTATOR = "SPECTATOR"
     TEMPORARY = "TEMPORARY"
     PM = "PM"
     GROUP = "GROUP"
+    ANNOUNCE = "ANNOUNCE"
 
 class CommentableType(EnumModel):
     NEWS_POST = "news_post"
     CHANGELOG = "build"
     BEATMAPSET = "beatmapset"
 
 class CommentSort(EnumModel):
@@ -375,16 +379,16 @@
 class BeatmapsetSearchLanguage(EnumModel):
     # default option, made up value
     ANY = 0
     UNSPECIFIED = 1
     ENGLISH = 2
     JAPANESE = 3
     CHINESE = 4
-    KOREAN = 6
     INSTRUMENTAL = 5
+    KOREAN = 6
     FRENCH = 7
     GERMAN = 8
     SWEDISH = 9
     SPANISH = 10
     ITALIAN = 11
     RUSSIAN = 12
     POLISH = 13
@@ -421,14 +425,17 @@
 class RoomSearchType(EnumModel):
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d4
     # 30a2/routes/web.php#L462
     OWNED = "owned"
     PARTICIPATED = "participated"
     ENDED = "ended"
 
+class EventsSort(EnumModel):
+    NEW = "id_desc"
+    OLD = "id_asc"
 
 
 # =================
 # Documented Models
 # =================
 
 class Failtimes(Model):
@@ -605,14 +612,22 @@
     # undocumented
     year: Optional[int]
 
 class ForumPostBody(Model):
     html: str
     raw: str
 
+class ForumPollText(Model):
+    bbcode: str
+    html: str
+
+class ForumPollTitle(Model):
+    bbcode: str
+    html: str
+
 class ReviewsConfig(Model):
     max_blocks: int
 
 class RankHighest(Model):
     rank: int
     updated_at: Datetime
```

### Comparing `ossapi-3.2.0/ossapi/mod.py` & `ossapi-3.3.0/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/ossapi/models.py` & `ossapi-3.3.0/ossapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     ProfilePage, GameMode, RankStatus, Failtimes, Covers, Hype, Availability,
     Nominations, Statistics, Grade, Weight, MessageType, KudosuAction,
     KudosuGiver, KudosuPost, EventType, EventAchivement, EventUser,
     EventBeatmap, BeatmapsetApproval, EventBeatmapset, KudosuVote,
     BeatmapsetEventType, UserRelationType, UserLevel, UserGradeCounts,
     GithubUser, ChangelogSearch, ForumTopicType, ForumPostBody, ForumTopicSort,
     ChannelType, ReviewsConfig, NewsSearch, Nomination, RankHighest, RoomType,
-    RoomCategory, MatchEventType, ScoringType, TeamType)
+    RoomCategory, MatchEventType, ScoringType, TeamType, Variant, ForumPollText,
+    ForumPollTitle)
 from ossapi.utils import Datetime, Model, BaseModel, Field
 
 T = TypeVar("T")
 S = TypeVar("S")
 
 """
 a type hint of ``Optional[Any]`` or ``Any`` means that I don't know what type it
@@ -82,15 +83,14 @@
     """
     https://osu.ppy.sh/docs/index.html#usercompact
     """
     # required fields
     # ---------------
     avatar_url: str
     country_code: str
-    default_group: str
     id: int
     is_active: bool
     is_bot: bool
     is_deleted: bool
     is_online: bool
     is_supporter: bool
     last_visit: Optional[Datetime]
@@ -103,22 +103,21 @@
     account_history: Optional[List[UserAccountHistory]]
     active_tournament_banner: Optional[ProfileBanner]
     badges: Optional[List[UserBadge]]
     beatmap_playcounts_count: Optional[int]
     blocks: Optional[UserRelation]
     country: Optional[Country]
     cover: Optional[Cover]
+    default_group: Optional[str]
     favourite_beatmapset_count: Optional[int]
-    # undocumented
     follow_user_mapping: Optional[List[int]]
     follower_count: Optional[int]
     friends: Optional[List[UserRelation]]
     graveyard_beatmapset_count: Optional[int]
     groups: Optional[List[UserGroup]]
-    # undocumented
     guest_beatmapset_count: Optional[int]
     is_admin: Optional[bool]
     is_bng: Optional[bool]
     is_full_bn: Optional[bool]
     is_gmt: Optional[bool]
     is_limited_bn: Optional[bool]
     is_moderator: Optional[bool]
@@ -126,34 +125,35 @@
     is_restricted: Optional[bool]
     is_silenced: Optional[bool]
     loved_beatmapset_count: Optional[int]
     # undocumented
     mapping_follower_count: Optional[int]
     monthly_playcounts: Optional[List[UserMonthlyPlaycount]]
     page: Optional[UserPage]
+    pending_beatmapset_count: Optional[int]
     previous_usernames: Optional[List[str]]
+    # deprecated, replaced by rank_history
+    rankHistory: Optional[RankHistory]
+    rank_history: Optional[RankHistory]
     # deprecated, replaced by ranked_beatmapset_count
     ranked_and_approved_beatmapset_count: Optional[int]
     ranked_beatmapset_count: Optional[int]
     replays_watched_counts: Optional[List[UserReplaysWatchedCount]]
     scores_best_count: Optional[int]
     scores_first_count: Optional[int]
     scores_recent_count: Optional[int]
     statistics: Optional[UserStatistics]
     statistics_rulesets: Optional[UserStatisticsRulesets]
     support_level: Optional[int]
     # deprecated, replaced by pending_beatmapset_count
     unranked_beatmapset_count: Optional[int]
-    pending_beatmapset_count: Optional[int]
     unread_pm_count: Optional[int]
     user_achievements: Optional[List[UserAchievement]]
     user_preferences: Optional[UserProfileCustomization]
-    rank_history: Optional[RankHistory]
-    # deprecated, replaced by rank_history
-    rankHistory: Optional[RankHistory]
+
 
     def expand(self) -> User:
         return self._fk_user(self.id)
 
 class User(UserCompact):
     comments_count: int
     cover_url: str
@@ -260,72 +260,71 @@
     # ---------------
     artist: str
     artist_unicode: str
     covers: Covers
     creator: str
     favourite_count: int
     id: int
+    nsfw: bool
+    offset: int
     play_count: int
     preview_url: str
     source: str
     status: RankStatus
+    spotlight: bool
     title: str
     title_unicode: str
     user_id: int
     video: bool
-    nsfw: bool
-    offset: int
-    spotlight: bool
     # documented as being in `Beatmapset` only, but returned by
     # `api.beatmapset_events` which uses a `BeatmapsetCompact`.
     hype: Optional[Hype]
 
     # optional fields
     # ---------------
     beatmaps: Optional[List[Beatmap]]
     converts: Optional[Any]
+    current_nominations: Optional[List[Nomination]]
     current_user_attributes: Optional[Any]
     description: Optional[Any]
     discussions: Optional[Any]
     events: Optional[Any]
     genre: Optional[Any]
     has_favourited: Optional[bool]
     language: Optional[Any]
     nominations: Optional[Any]
+    pack_tags: Optional[List[str]]
     ratings: Optional[Any]
     recent_favourites: Optional[Any]
     related_users: Optional[Any]
-    _user: Optional[UserCompact] = Field(name="user")
-    # undocumented
     track_id: Optional[int]
+    _user: Optional[UserCompact] = Field(name="user")
 
     def expand(self) -> Beatmapset:
         return self._fk_beatmapset(self.id)
 
     def user(self) -> Union[UserCompact, User]:
         return self._fk_user(self.user_id, existing=self._user)
 
 class Beatmapset(BeatmapsetCompact):
     availability: Availability
     bpm: float
     can_be_hyped: bool
+    deleted_at: Optional[Datetime]
     discussion_enabled: bool
     discussion_locked: bool
     is_scoreable: bool
     last_updated: Datetime
     legacy_thread_url: Optional[str]
     nominations_summary: Nominations
     ranked: RankStatus
     ranked_date: Optional[Datetime]
     storyboard: bool
     submitted_date: Optional[Datetime]
     tags: str
-    current_nominations: Optional[List[Nomination]]
-    deleted_at: Optional[Datetime]
-    pack_tags: List[str]
 
     def expand(self) -> Beatmapset:
         return self
 
 # undocumented, but defined here to avoid a forward reference in Score.
 class ScoreMatchInfo(Model):
     slot: int
@@ -430,26 +429,26 @@
 
     def edited_by(self) -> Optional[User]:
         return self._fk_user(self.edited_by_id)
 
 class CommentBundle(Model):
     commentable_meta: List[CommentableMeta]
     comments: List[Comment]
+    cursor: CursorT
     has_more: bool
     has_more_id: Optional[int]
     included_comments: List[Comment]
     pinned_comments: Optional[List[Comment]]
+    # TODO this should be type CommentSort
     sort: str
     top_level_count: Optional[int]
     total: Optional[int]
     user_follow: bool
     user_votes: List[int]
     users: List[UserCompact]
-    # undocumented
-    cursor: CursorT
 
 class ForumPost(Model):
     created_at: Datetime
     deleted_at: Optional[Datetime]
     edited_at: Optional[Datetime]
     edited_by_id: Optional[int]
     forum_id: int
@@ -473,19 +472,35 @@
     is_locked: bool
     last_post_id: int
     post_count: int
     title: str
     type: ForumTopicType
     updated_at: Datetime
     user_id: int
-    poll: Any
+    poll: Optional[ForumPollModel]
 
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
+class ForumPollModel(Model):
+    allow_vote_change: bool
+    ended_at: Optional[Datetime]
+    hide_incomplete_results: bool
+    last_vote_at: Optional[Datetime]
+    max_votes: int
+    options: List[ForumPollOption]
+    started_at: Datetime
+    title: ForumPollTitle
+    total_vote_count: int
+
+class ForumPollOption(Model):
+    id: int
+    text: ForumPollText
+    vote_count: Optional[int]
+
 class ForumTopicAndPosts(Model):
     cursor: CursorT
     search: ForumTopicSearch
     posts: List[ForumPost]
     topic: ForumTopic
     cursor_string: Optional[str]
 
@@ -575,21 +590,17 @@
     parent_id: Optional[int]
     # a point of time which is ``timestamp`` milliseconds into the map
     timestamp: Optional[int]
     resolved: bool
     can_be_resolved: bool
     can_grant_kudosu: bool
     created_at: Datetime
-    # documented as non-optional, api.beatmapset_events() might give a null
-    # response for this? but very rarely. need to find a repro case
     current_user_attributes: Any
     updated_at: Datetime
     deleted_at: Optional[Datetime]
-    # similarly as for current_user_attributes, in the past this has been null
-    # but can't find a repro case
     last_post_at: Datetime
     kudosu_denied: bool
     starting_post: Optional[BeatmapsetDiscussionPost]
     posts: Optional[List[BeatmapsetDiscussionPost]]
     _beatmap: Optional[BeatmapCompact] = Field(name="beatmap")
     _beatmapset: Optional[BeatmapsetCompact] = Field(name="beatmapset")
 
@@ -609,14 +620,16 @@
 class BeatmapsetDiscussionVote(Model):
     id: int
     score: int
     user_id: int
     beatmapset_discussion_id: int
     created_at: Datetime
     updated_at: Datetime
+    # TODO is this field ever actually returned? not documented and can't find
+    # a repro case.
     cursor_string: Optional[str]
 
     def user(self):
         return self._fk_user(self.user_id)
 
 class KudosuHistory(Model):
     id: int
@@ -727,14 +740,15 @@
     display_version: str
     id: int
     update_stream: Optional[UpdateStream]
     users: int
     version: Optional[str]
     changelog_entries: Optional[List[ChangelogEntry]]
     versions: Optional[Versions]
+    youtube_id: Optional[str]
 
 class Versions(Model):
     next: Optional[Build]
     previous: Optional[Build]
 
 class UpdateStream(Model):
     display_name: Optional[str]
@@ -847,24 +861,27 @@
     speed_difficulty: Optional[float]
     speed_note_count: Optional[float]
 
     # taiko attributes
     stamina_difficulty: Optional[float]
     rhythm_difficulty: Optional[float]
     colour_difficulty: Optional[float]
-    approach_raty: Optional[float]
-    great_hit_windoy: Optional[float]
+    approach_rate: Optional[float]
+    great_hit_window: Optional[float]
 
     # ctb attributes
     approach_rate: Optional[float]
 
     # mania attributes
     great_hit_window: Optional[float]
     score_multiplier: Optional[float]
 
+class Events(Model):
+    cursor_string: str
+    events: List[Event]
 
 
 # ================
 # Parameter Models
 # ================
 
 # models which aren't used for serialization, but passed to OssapiV2 methods.
@@ -1028,23 +1045,22 @@
     def user(self) -> Optional[User]:
         return self._fk_user(self.user_id)
 
 class ChatChannel(Model):
     channel_id: int
     description: Optional[str]
     icon: Optional[str]
-    # documented as non-optional (to see that it can be null, pm tillerino)
     moderated: Optional[bool]
     name: str
     type: ChannelType
     uuid: Optional[str]
+    message_length_limit: int
 
     # optional fields
     # ---------------
-    first_message_id: Optional[int]
     last_message_id: Optional[int]
     last_read_id: Optional[int]
     recent_messages: Optional[List[ChatMessage]]
     users: Optional[List[int]]
 
 class ChatMessage(Model):
     channel_id: int
@@ -1085,39 +1101,46 @@
     # optional fields
     # ---------------
     target: Optional[UserCompact]
 
     def target(self) -> Union[User, UserCompact]:
         return self._fk_user(self.target_id, existing=self.target)
 
+class StatisticsVariant(Model):
+    mode: GameMode
+    variant: Variant
+    country_rank: Optional[int]
+    global_rank: Optional[int]
+    pp: float
 
 class UserStatistics(Model):
-    level: UserLevel
-    pp: float
-    ranked_score: int
+    count_100: int
+    count_300: int
+    count_50: int
+    count_miss: int
+    country_rank: Optional[int]
+    grade_counts: UserGradeCounts
     hit_accuracy: float
+    is_ranked: bool
+    level: UserLevel
+    maximum_combo: int
     play_count: int
     play_time: int
-    total_score: int
-    total_hits: int
-    maximum_combo: int
-    replays_watched_by_others: int
-    is_ranked: bool
-    grade_counts: UserGradeCounts
-    country_rank: Optional[int]
+    pp: float
+    pp_exp: float
     global_rank: Optional[int]
+    global_rank_exp: Optional[float]
+    # deprecated, replaced by global_rank and country_rank
     rank: Optional[Any]
+    ranked_score: int
+    replays_watched_by_others: int
+    total_hits: int
+    total_score: int
     user: Optional[UserCompact]
-    variants: Optional[Any]
-    global_rank_exp: Optional[float]
-    pp_exp: float
-    count_100: int
-    count_300: int
-    count_50: int
-    count_miss: int
+    variants: Optional[List[StatisticsVariant]]
 
 class UserStatisticsRulesets(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserStatisti
     # csRulesetsTransformer.php
     osu: Optional[UserStatistics]
     taiko: Optional[UserStatistics]
```

### Comparing `ossapi-3.2.0/ossapi/ossapi.py` & `ossapi-3.3.0/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/ossapi/ossapiv2.py` & `ossapi-3.3.0/ossapi/ossapiv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
     Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
     ChangelogListing, MultiplayerScores,
     BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
     UserCompact, NewsListing, NewsPost, SeasonalBackgrounds, BeatmapsetCompact,
     BeatmapUserScores, DifficultyAttributes, Users, Beatmaps,
     CreateForumTopicResponse, ForumPoll, ForumPost, ForumTopic, Room,
-    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel)
+    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel, Events)
 from ossapi.enums import (GameMode, ScoreType, RankingFilter, RankingType,
     UserBeatmapType, BeatmapDiscussionPostSort, UserLookupKey,
     BeatmapsetEventType, CommentableType, CommentSort, ForumTopicSort,
     SearchMode, MultiplayerScoresSort, BeatmapsetDiscussionVote,
     BeatmapsetDiscussionVoteSort, BeatmapsetStatus, MessageType,
     BeatmapsetSearchCategory, BeatmapsetSearchMode,
     BeatmapsetSearchExplicitContent, BeatmapsetSearchGenre,
     BeatmapsetSearchLanguage, NewsPostKey, BeatmapsetSearchSort, RoomSearchType,
-    ChangelogMessageFormat)
+    ChangelogMessageFormat, EventsSort)
 from ossapi.utils import (is_compatible_type, is_primitive_type, is_optional,
     is_base_model_type, is_model_type, is_high_model_type, Field)
 from ossapi.mod import Mod
 from ossapi.replay import Replay
 
 # our `request` function below relies on the ordering of these types. The
 # base type must come first, with any auxiliary types that the base type accepts
@@ -76,14 +76,15 @@
 BeatmapsetSearchModeT = Union[BeatmapsetSearchMode, int]
 BeatmapsetSearchExplicitContentT = Union[BeatmapsetSearchExplicitContent, str]
 BeatmapsetSearchGenreT = Union[BeatmapsetSearchGenre, int]
 BeatmapsetSearchLanguageT = Union[BeatmapsetSearchLanguage, str]
 NewsPostKeyT = Union[NewsPostKey, str]
 BeatmapsetSearchSortT = Union[BeatmapsetSearchSort, str]
 RoomSearchTypeT = Union[RoomSearchType, str]
+EventsSortT = Union[EventsSort, str]
 
 BeatmapIdT = Union[int, BeatmapCompact]
 UserIdT = Union[int, UserCompact]
 BeatmapsetIdT = Union[int, BeatmapCompact, BeatmapsetCompact]
 RoomIdT = Union[int, Room]
 MatchIdT = Union[int, Match]
 
@@ -312,15 +313,15 @@
     domain: Domain or str
         The domain to retrieve information from. This defaults to
         :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, which corresponds to
         osu.ppy.sh, the main website.
         |br|
         To retrieve information from lazer.ppy.sh - for instance, the
         leaderboards on lazer, or a user's best score on lazer - specify
-        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retureve
+        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retrieve
         information from dev.ppy.sh, specify
         :data:`Domain.DEV <ossapi.ossapiv2.Domain.DEV>`.
         |br|
         See :doc:`Domains <domains>` for more about domains.
     """
     TOKEN_URL = "https://{domain}.ppy.sh/oauth/token"
     AUTH_CODE_URL = "https://{domain}.ppy.sh/oauth/authorize"
@@ -1631,14 +1632,42 @@
         -----
         Implements the `Get a Comment
         <https://osu.ppy.sh/docs/index.html#get-a-comment>`__ endpoint.
         """
         return self._get(CommentBundle, f"/comments/{comment_id}")
 
 
+    # /events
+    # -------
+
+    @request(Scope.PUBLIC, category="events")
+    def events(self,
+        *,
+        sort: Optional[EventsSortT] = None,
+        cursor_string: Optional[str] = None
+    ) -> Events:
+        """
+        Get most recent events, in order of creation time.
+
+        Parameters
+        ----------
+        sort
+            Sort events by oldest or newest.
+        cursor_string
+            Cursor for pagination.
+
+        Notes
+        -----
+        Implements the `Get Events
+        <https://osu.ppy.sh/docs/index.html#get-events>`__ endpoint.
+        """
+        params = {"cursor_string": cursor_string, "sort": sort}
+        return self._get(Events, "/events", params)
+
+
     # /forums
     # -------
 
     @request(Scope.FORUM_WRITE, category="forums")
     def forum_create_topic(self,
        forum_id: int,
        title: str,
```

### Comparing `ossapi-3.2.0/ossapi/ossapiv2_async.py` & `ossapi-3.3.0/ossapi/ossapiv2_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,24 @@
     BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
     Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
     ChangelogListing, MultiplayerScores,
     BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
     UserCompact, NewsListing, NewsPost, SeasonalBackgrounds, BeatmapsetCompact,
     BeatmapUserScores, DifficultyAttributes, Users, Beatmaps,
     CreateForumTopicResponse, ForumPoll, ForumPost, ForumTopic, Room,
-    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel)
+    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel, Events)
 from ossapi.enums import (GameMode, ScoreType, RankingFilter, RankingType,
     UserBeatmapType, BeatmapDiscussionPostSort, UserLookupKey,
     BeatmapsetEventType, CommentableType, CommentSort, ForumTopicSort,
     SearchMode, MultiplayerScoresSort, BeatmapsetDiscussionVote,
     BeatmapsetDiscussionVoteSort, BeatmapsetStatus, MessageType,
     BeatmapsetSearchCategory, BeatmapsetSearchMode,
     BeatmapsetSearchExplicitContent, BeatmapsetSearchGenre,
     BeatmapsetSearchLanguage, NewsPostKey, BeatmapsetSearchSort, RoomSearchType,
-    ChangelogMessageFormat)
+    ChangelogMessageFormat, EventsSort)
 from ossapi.utils import (is_compatible_type, is_primitive_type, is_optional,
     is_base_model_type, is_model_type, is_high_model_type, Field)
 from ossapi.mod import Mod
 from ossapi.replay import Replay
 
 
 class Oauth2SessionAsync(OAuth2Session):
@@ -142,14 +142,15 @@
 BeatmapsetSearchModeT = Union[BeatmapsetSearchMode, int]
 BeatmapsetSearchExplicitContentT = Union[BeatmapsetSearchExplicitContent, str]
 BeatmapsetSearchGenreT = Union[BeatmapsetSearchGenre, int]
 BeatmapsetSearchLanguageT = Union[BeatmapsetSearchLanguage, str]
 NewsPostKeyT = Union[NewsPostKey, str]
 BeatmapsetSearchSortT = Union[BeatmapsetSearchSort, str]
 RoomSearchTypeT = Union[RoomSearchType, str]
+EventsSortT = Union[EventsSort, str]
 
 BeatmapIdT = Union[int, BeatmapCompact]
 UserIdT = Union[int, UserCompact]
 BeatmapsetIdT = Union[int, BeatmapCompact, BeatmapsetCompact]
 RoomIdT = Union[int, Room]
 MatchIdT = Union[int, Match]
 
@@ -292,14 +293,27 @@
     CHAT_WRITE = "chat.write"
     DELEGATE = "delegate"
     FORUM_WRITE = "forum.write"
     FRIENDS_READ = "friends.read"
     IDENTIFY = "identify"
     PUBLIC = "public"
 
+class Domain(Enum):
+    """
+    Different possible api domains. These correspond to different deployments of
+    the osu server: osu.ppy.sh, lazer.ppy.sh, and dev.ppy.sh respectively.
+
+    The default domain, and the one the vast majority of users want, is
+    :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, and corresponds to the
+    main website. To retrieve information from the lazer website or the dev
+    website, use the corresponding domain.
+    """
+    OSU = "osu"
+    LAZER = "lazer"
+    DEV = "dev"
 
 class OssapiAsync:
     """
     Async equivalent of :class:`~ossapi.ossapiv2.Ossapi`. Main (async) entry
     point into osu! api v2.
 
     Parameters
@@ -359,47 +373,67 @@
         :class:`~ossapi.ossapiv2.Ossapi` after manually authenticating with the
         osu! api.
     refresh_token: str
         Refresh token from the osu! api. Allows instantiating
         :class:`~ossapi.ossapiv2.Ossapi` after manually authenticating with the
         osu! api. Optional if using :data:`Grant.CLIENT_CREDENTIALS
         <ossapi.ossapiv2.Grant.CLIENT_CREDENTIALS>`.
+    domain: Domain or str
+        The domain to retrieve information from. This defaults to
+        :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, which corresponds to
+        osu.ppy.sh, the main website.
+        |br|
+        To retrieve information from lazer.ppy.sh - for instance, the
+        leaderboards on lazer, or a user's best score on lazer - specify
+        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retureve
+        information from dev.ppy.sh, specify
+        :data:`Domain.DEV <ossapi.ossapiv2.Domain.DEV>`.
+        |br|
+        See :doc:`Domains <domains>` for more about domains.
     """
-    TOKEN_URL = "https://osu.ppy.sh/oauth/token"
-    AUTH_CODE_URL = "https://osu.ppy.sh/oauth/authorize"
-    BASE_URL = "https://osu.ppy.sh/api/v2"
+    TOKEN_URL = "https://{domain}.ppy.sh/oauth/token"
+    AUTH_CODE_URL = "https://{domain}.ppy.sh/oauth/authorize"
+    BASE_URL = "https://{domain}.ppy.sh/api/v2"
 
     def __init__(self,
         client_id: int,
         client_secret: str,
         redirect_uri: Optional[str] = None,
         scopes: List[Union[str, Scope]] = [Scope.PUBLIC],
         *,
         grant: Optional[Union[Grant, str]] = None,
         strict: bool = False,
         token_directory: Optional[str] = None,
         token_key: Optional[str] = None,
         access_token: Optional[str] = None,
-        refresh_token: Optional[str] = None
+        refresh_token: Optional[str] = None,
+        domain: Union[str, Domain] = Domain.OSU
     ):
         if not grant:
             grant = (Grant.AUTHORIZATION_CODE if redirect_uri else
                 Grant.CLIENT_CREDENTIALS)
         grant = Grant(grant)
 
+        domain = Domain(domain)
+
+        self.token_url = self.TOKEN_URL.format(domain=domain.value)
+        self.auth_code_url = self.AUTH_CODE_URL.format(domain=domain.value)
+        self.base_url = self.BASE_URL.format(domain=domain.value)
+
         self.grant = grant
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.scopes = [Scope(scope) for scope in scopes]
         self.strict = strict
+        self.domain = domain
 
         self.log = logging.getLogger(__name__)
         self.token_key = token_key or self.gen_token_key(self.grant,
-            self.client_id, self.client_secret, self.scopes)
+            self.client_id, self.client_secret, self.scopes, self.domain.value)
 
         # support saving tokens when being run from pyinstaller
         if hasattr(sys, '_MEIPASS') and not token_directory:
             token_directory = sys._MEIPASS # pylint: disable=no-member
 
         self.token_directory = (
             Path(token_directory) if token_directory else Path(__file__).parent
@@ -426,32 +460,46 @@
                 "refresh_token": refresh_token
             }
             token = OAuth2Token(params)
 
         self.session = self.authenticate(token=token)
 
     @staticmethod
-    def gen_token_key(grant, client_id, client_secret, scopes):
+    def gen_token_key(grant, client_id, client_secret, scopes,
+        domain=Domain.OSU
+    ):
         """
         The unique key / hash for the given set of parameters. This is intended
         to provide a way to allow multiple OssapiV2's to live at the same time,
         by eg saving their tokens to different files based on their key.
 
         This function is also deterministic, to eg allow tokens to be reused if
         OssapiV2 is instantiated twice with the same parameters. This avoids the
         need to reauthenticate unless absolutely necessary.
         """
         grant = Grant(grant)
         scopes = [Scope(scope) for scope in scopes]
+        domain = Domain(domain)
+
         m = hashlib.sha256()
         m.update(grant.value.encode("utf-8"))
         m.update(str(client_id).encode("utf-8"))
         m.update(client_secret.encode("utf-8"))
+
         for scope in scopes:
             m.update(scope.value.encode("utf-8"))
+
+        # for backwards compatability, only hash the domain when it's
+        # non-default. This ensures keys from before and after domains were
+        # introduced coincide.
+        # This intentionally treats Domain.OSU and Domain.LAZER as the same key,
+        # as those domains share account and oauth credentials.
+        if domain is Domain.DEV:
+            m.update(domain.value.encode("utf-8"))
+
         return m.hexdigest()
 
     @staticmethod
     def remove_token(key, token_directory=None):
         """
         Removes the token file associated with the given key. If
         ``token_directory`` is passed, looks there for the token file instead of
@@ -483,15 +531,15 @@
             if self.grant is Grant.AUTHORIZATION_CODE:
                 auto_refresh_kwargs = {
                     "client_id": self.client_id,
                     "client_secret": self.client_secret
                 }
                 return Oauth2SessionAsync(self.client_id, token=token,
                     redirect_uri=self.redirect_uri,
-                    auto_refresh_url=self.TOKEN_URL,
+                    auto_refresh_url=self.token_url,
                     auto_refresh_kwargs=auto_refresh_kwargs,
                     token_updater=self._save_token,
                     scope=[scope.value for scope in self.scopes])
 
         if self.grant is Grant.CLIENT_CREDENTIALS:
             return self._new_client_grant(self.client_id, self.client_secret)
 
@@ -501,15 +549,15 @@
     def _new_client_grant(self, client_id, client_secret):
         """
         Authenticates with the api from scratch on the client grant.
         """
         self.log.info("initializing client credentials grant")
         client = BackendApplicationClient(client_id=client_id, scope=["public"])
         session = Oauth2SessionAsync(client=client)
-        token = session.fetch_token(token_url=self.TOKEN_URL,
+        token = session.fetch_token(token_url=self.token_url,
             client_id=client_id, client_secret=client_secret)
 
         self._save_token(token)
         return session
 
     def _new_authorization_grant(self, client_id, client_secret, redirect_uri,
         scopes):
@@ -519,21 +567,21 @@
         self.log.info("initializing authorization code")
 
         auto_refresh_kwargs = {
             "client_id": client_id,
             "client_secret": client_secret
         }
         session = Oauth2SessionAsync(client_id, redirect_uri=redirect_uri,
-            auto_refresh_url=self.TOKEN_URL,
+            auto_refresh_url=self.token_url,
             auto_refresh_kwargs=auto_refresh_kwargs,
             token_updater=self._save_token,
             scope=[scope.value for scope in scopes])
 
         authorization_url, _state = (
-            session.authorization_url(self.AUTH_CODE_URL)
+            session.authorization_url(self.auth_code_url)
         )
         webbrowser.open(authorization_url)
 
         # open up a temporary socket so we can receive the GET request to the
         # callback url
         port = int(redirect_uri.rsplit(":", 1)[1].split("/")[0])
         serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -550,15 +598,15 @@
             may now close this tab safely.
             </body></html>
         """)
         connection.close()
         serversocket.close()
 
         code = data.split("code=")[1].split("&state=")[0]
-        token = session.fetch_token(self.TOKEN_URL, client_id=client_id,
+        token = session.fetch_token(self.token_url, client_id=client_id,
             client_secret=client_secret, code=code)
         self._save_token(token)
 
         return session
 
     def _save_token(self, token):
         """
@@ -579,30 +627,30 @@
         # not achieving 100% performance by doing this. The benefit is that we
         # don't require `async with OssapiAsync(...) as api:` syntax in order to
         # use ossapi.
         aiohttp_session = ClientSession()
 
         try:
             r = await self.session.request_async(method,
-                f"{self.BASE_URL}{url}", session=aiohttp_session,
+                f"{self.base_url}{url}", session=aiohttp_session,
                 params=params, data=data)
         except TokenExpiredError:
             # provide "auto refreshing" for client credentials grant. The client
             # grant doesn't actually provide a refresh token, so we can't hook
             # onto OAuth2Session's auto_refresh functionality like we do for the
             # authorization code grant. But we can do something effectively
             # equivalent: whenever we make a request with an expired client
             # grant token, just request a new one.
             if self.grant is not Grant.CLIENT_CREDENTIALS:
                 raise
             self.session = self._new_client_grant(self.client_id,
                 self.client_secret)
             # redo the request now that we have a valid token
             r = await self.session.request_async(method,
-                f"{self.BASE_URL}{url}", session=aiohttp_session,
+                f"{self.base_url}{url}", session=aiohttp_session,
                 params=params, data=data)
 
         # aiohttp annoyingly differentiates between url (no url fragments, for
         # some reason) and real_url (actual url). They also use a URL object
         # here instead of a string.
         url = str(r.real_url)
         self.log.info(f"made {method} request to {url}, data {data}")
@@ -1673,14 +1721,42 @@
         -----
         Implements the `Get a Comment
         <https://osu.ppy.sh/docs/index.html#get-a-comment>`__ endpoint.
         """
         return await self._get(CommentBundle, f"/comments/{comment_id}")
 
 
+    # /events
+    # -------
+
+    @request(Scope.PUBLIC, category="events")
+    async def events(self,
+        *,
+        sort: Optional[EventsSortT] = None,
+        cursor_string: Optional[str] = None
+    ) -> Events:
+        """
+        Get most recent events, in order of creation time.
+
+        Parameters
+        ----------
+        sort
+            Sort events by oldest or newest.
+        cursor_string
+            Cursor for pagination.
+
+        Notes
+        -----
+        Implements the `Get Events
+        <https://osu.ppy.sh/docs/index.html#get-events>`__ endpoint.
+        """
+        params = {"cursor_string": cursor_string, "sort": sort}
+        return await self._get(Events, "/events", params)
+
+
     # /forums
     # -------
 
     @request(Scope.FORUM_WRITE, category="forums")
     async def forum_create_topic(self,
        forum_id: int,
        title: str,
@@ -1984,15 +2060,15 @@
         you unable to make any more api calls until you re-authenticate.
 
         Notes
         -----
         Implements the `Revoke Current Token
         <https://osu.ppy.sh/docs/index.html#revoke-current-token>`__ endpoint.
         """
-        self.session.delete(f"{self.BASE_URL}/oauth/tokens/current")
+        self.session.delete(f"{self.base_url}/oauth/tokens/current")
         self.remove_token(self.token_key, self.token_directory)
 
 
     # /rankings
     # ---------
 
     @request(Scope.PUBLIC, category="rankings")
@@ -2182,15 +2258,22 @@
         -----
         Implements the `Download Score
         <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
         endpoint.
         """
         from aiohttp import ClientSession, ContentTypeError
 
-        url = f"{self.BASE_URL}/scores/{mode.value}/{score_id}/download"
+        if self.domain is Domain.LAZER:
+            raise ValueError("Downloading scores using the lazer domain is not "
+                "currently supported, as lazer itself does not currently "
+                "support replay downloads. This may change in the future. To "
+                "download replays, use the osu domain (ie, a normal Ossapi "
+                "instance.)")
+
+        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
 
         aiohttp_session = ClientSession()
         r = await self.session.request_async("GET", url,
             session=aiohttp_session)
 
         # if the response above succeeded, it will return a raw string
         # instead of json. If it didn't succeed, it will return json with an
```

### Comparing `ossapi-3.2.0/ossapi/replay.py` & `ossapi-3.3.0/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/ossapi/utils.py` & `ossapi-3.3.0/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/ossapi.egg-info/PKG-INFO` & `ossapi-3.3.0/ossapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.2.0
+Version: 3.3.0
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: async
 License-File: LICENSE
 
 # ossapi ([documentation](https://circleguard.github.io/ossapi/)) [![PyPI version](https://badge.fury.io/py/ossapi.svg)](https://pypi.org/project/ossapi/)
 
-ossapi is a python wrapper for the osu! api which has complete coverage of both [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki). ossapi provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
+ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
+* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
   * [Forums](#endpoints-forums)
@@ -69,15 +70,15 @@
 ```python
 from ossapi import Ossapi
 
 # create a new client at https://osu.ppy.sh/home/account/edit#oauth
 api = Ossapi(client_id, client_secret)
 
 # see docs for full list of endpoints
-print(api.user("tybug2").username)
+print(api.user("tybug").username)
 print(api.user(12092800, mode="osu").username)
 print(api.beatmap(221777).id)
 ```
 
 ## Async
 
 ossapi provides an async variant, `OssapiAsync`, which has an identical interface to `Ossapi`:
@@ -85,21 +86,37 @@
 ```python
 import asyncio
 from ossapi import Ossapi
 
 api = Ossapi(client_id, client_secret)
 
 async def main():
-    await api.user("tybug2")
+    await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://circleguard.github.io/ossapi/async.html)
 
+## Lazer
+
+You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+
+```python
+from ossapi import Ossapi
+
+api_lazer = Ossapi(client_id, client_secret, domain="lazer")
+
+# best score on the lazer server (lazer + osu scores combined)
+scores = api_lazer.user_scores(12092800, "best")
+print(scores[0].pp)
+```
+
+[Read more about domains on the docs.](https://circleguard.github.io/ossapi/domains.html)
+
 ## Endpoints
 
 All endpoints for api v2.
 
 * Beatmaps<a name="endpoints-beatmaps"></a>
   * [`api.beatmap`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap)
   * [`api.beatmap_attributes`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.beatmap_attributes)
@@ -166,15 +183,15 @@
   * [`api.user_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.user_scores)
   * [`api.users`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.users)
 * Wiki<a name="endpoints-wiki"></a>
   * [`api.wiki_page`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.wiki_page)
 
 ## API v1 Usage
 
-You can get your api v1 key at <https://osu.ppy.sh/p/api/>. Note that due to a [redirection bug](https://github.com/ppy/osu-web/issues/2867), you may need to log in and wait 30 seconds before being able to access the api page through the above link.
+You can get your api v1 key at <https://osu.ppy.sh/home/account/edit#legacy-api>.
 
 Basic usage:
 
 ```python
 from ossapi import OssapiV1
 
 api = OssapiV1("key")
```

### Comparing `ossapi-3.2.0/pyproject.toml` & `ossapi-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.2.0"
+version = "3.3.0"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.2.0/tests/__init__.py` & `ossapi-3.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/tests/test_cursor.py` & `ossapi-3.3.0/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.2.0/tests/test_endpoints.py` & `ossapi-3.3.0/tests/test_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime
 from unittest import TestCase
 
 from ossapi import (RankingType, BeatmapsetEventType, AccessDeniedError,
-    InsufficientScopeError, Mod, GameMode, ForumPoll, RoomSearchType)
+    InsufficientScopeError, Mod, GameMode, ForumPoll, RoomSearchType,
+    EventsSort)
 
 from tests import (
     TestCaseAuthorizationCode, TestCaseDevServer, UNIT_TEST_MESSAGE,
     api_v2 as api,
     api_v2_full as api_full,
     api_v2_lazer as api_lazer,
     api_v2_dev as api_dev
@@ -105,18 +106,18 @@
 
 class TestUser(TestCase):
     def test_deserialize(self):
         api.user(12092800)
 
     def test_key(self):
         # make sure it automatically falls back to username if not specified
-        api.user("tybug2")
-        api.user("tybug2", key="username")
+        api.user("tybug")
+        api.user("tybug", key="username")
 
-        self.assertRaises(Exception, lambda: api.user("tybug2", key="id"))
+        self.assertRaises(Exception, lambda: api.user("tybug", key="id"))
 
 class TestMe(TestCase):
     def test_insufficient_scope(self):
         # client credentials grant can't request `Scope.IDENTIFY` and so can't
         # access /me
         self.assertRaises(InsufficientScopeError, api.get_me)
 
@@ -134,15 +135,20 @@
 
 class TestChangelogLookup(TestCase):
     def test_deserialize(self):
         api.changelog_build_lookup("lazer")
 
 class TestForumTopic(TestCase):
     def test_deserialize(self):
+        # normal topic
+        # https://osu.ppy.sh/community/forums/topics/141240?n=1
         api.forum_topic(141240)
+        # topic with a poll
+        # https://osu.ppy.sh/community/forums/topics/1781998?n=1
+        api.forum_topic(1781998)
 
 class TestBeatmapsetDiscussionVotes(TestCase):
     def test_deserialize(self):
         api.beatmapset_discussion_votes().votes[0].score
 
 class TestBeatmapsetDiscussions(TestCase):
     def test_deserialize(self):
@@ -212,14 +218,20 @@
         # https://osu.ppy.sh/community/matches/97947404, tournament match
         api.match(97947404)
 
 class TestComments(TestCase):
     def test_deserialize(self):
         api.comments()
 
+class TestEvents(TestCase):
+    def test_deserialize(self):
+        events = api.events()
+        api.events(cursor_string=events.cursor_string)
+        api.events(sort=EventsSort.NEW)
+
 
 # ======================
 # api_full test cases
 # ======================
 
 class TestCreateNewPM(TestCaseAuthorizationCode):
     def test_deserialize(self):
@@ -252,19 +264,19 @@
 # api_lazer test cases
 # ====================
 class TestLazerUser(TestCase):
     def test_lazer_different_from_osu(self):
         # make sure the lazer domain returns something different than the osu
         # domain. ie, we're actually hitting a different db.
 
-        statistics = api.user("tybug2").statistics
+        statistics = api.user("tybug").statistics
         pp_osu = statistics.pp
         pp_exp_osu = statistics.pp_exp
 
-        statistics = api_lazer.user("tybug2").statistics
+        statistics = api_lazer.user("tybug").statistics
         pp_lazer = statistics.pp
         pp_exp_lazer = statistics.pp_exp
 
         # pp_exp is 0 in lazer
         self.assertEqual(pp_exp_lazer, 0)
         # not necessarily an invariant, but happens to be true for my account
         self.assertNotEqual(pp_osu, pp_lazer)
```

### Comparing `ossapi-3.2.0/tests/test_models.py` & `ossapi-3.3.0/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def test_room_as_parameter(self):
         room1 = api.room(257524)
         room2 = api.room(room1)
         self.assertEqual(room1, room2)
 
 class TestExpandableModels(TestCase):
     def test_expand_user(self):
-        user = api.search(query="tybug2").users.data[0]
+        user = api.search(query="tybug").users.data[0]
         # `statistics` is only available on User models, so make sure it's not
         # present before expanding and is present afterwards
         self.assertIsNone(user.statistics)
 
         user = user.expand()
         self.assertIsNotNone(user.statistics)
```

### Comparing `ossapi-3.2.0/tests/test_v1.py` & `ossapi-3.3.0/tests/test_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from unittest import TestCase
 
 from tests import api_v1 as api
 
 class TestGetUser(TestCase):
     def test_deserialize(self):
-        r = api.get_user("tybug2")
+        r = api.get_user("tybug")
 
-        self.assertEqual(r.username, "tybug2")
-        self.assertEqual(api.get_user(12092800).username, "tybug2")
+        self.assertEqual(r.username, "tybug")
+        self.assertEqual(api.get_user(12092800).username, "tybug")
 
 class TestGetBeatmaps(TestCase):
     def test_deserialize(self):
         api.get_beatmaps(beatmapset_id=1051305)
         api.get_beatmaps(beatmap_id=221777)
 
 class TestGetUserBest(TestCase):
@@ -25,15 +25,15 @@
 
         self.assertEqual(len(r1), 155328)
         self.assertEqual(len(r2), 141068)
 
 class TestGetScores(TestCase):
     def test_deserialize(self):
         api.get_scores(221777)
-        api.get_scores(221777, user="tybug2")
+        api.get_scores(221777, user="tybug")
 
 class TestGetUserRecent(TestCase):
     def test_deserialize(self):
         api.get_user_recent(12092800)
 
 class TestGetMatch(TestCase):
     def test_deserialize(self):
```

