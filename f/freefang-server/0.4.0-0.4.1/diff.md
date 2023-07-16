# Comparing `tmp/freefang-server-0.4.0.tar.gz` & `tmp/freefang-server-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freefang-server-0.4.0.tar", last modified: Sat Jul 15 23:32:35 2023, max compression
+gzip compressed data, was "freefang-server-0.4.1.tar", last modified: Sun Jul 16 00:13:53 2023, max compression
```

## Comparing `freefang-server-0.4.0.tar` & `freefang-server-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-15 23:32:23.000000 freefang-server-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-15 23:32:35.812506 freefang-server-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 23:32:23.000000 freefang-server-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/freefang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/voting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/freefang_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-15 23:32:23.000000 freefang-server-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 23:32:35.812506 freefang-server-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-15 23:32:23.000000 freefang-server-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:13:53.489533 freefang-server-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-16 00:13:36.000000 freefang-server-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-16 00:13:53.489533 freefang-server-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-16 00:13:36.000000 freefang-server-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:13:53.485532 freefang-server-0.4.1/freefang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-16 00:13:36.000000 freefang-server-0.4.1/freefang/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:13:53.489533 freefang-server-0.4.1/freefang_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-16 00:13:53.000000 freefang-server-0.4.1/freefang_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-16 00:13:53.000000 freefang-server-0.4.1/freefang_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:13:53.000000 freefang-server-0.4.1/freefang_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 00:13:53.000000 freefang-server-0.4.1/freefang_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 00:13:53.000000 freefang-server-0.4.1/freefang_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-16 00:13:36.000000 freefang-server-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 00:13:53.489533 freefang-server-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 00:13:36.000000 freefang-server-0.4.1/setup.py
```

### Comparing `freefang-server-0.4.0/LICENSE` & `freefang-server-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/PKG-INFO` & `freefang-server-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `freefang-server-0.4.0/README.md` & `freefang-server-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang/main.py` & `freefang-server-0.4.1/freefang/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import time
 import struct 
 import argparse
 import ssl
 import os
 
 VERSIONSTR = """
-FreeFang Server 0.4.0
+FreeFang Server 0.4.1
 Written by @Solirs and @lukakralik
 Licensed under AGPLv3.0
 Source code at https://github.com/FreeFangGame/freefang-server
 """
 
 def parse_ruleset(ruleset, game):
 	if ruleset.town_voting_scheme:
```

### Comparing `freefang-server-0.4.0/freefang/models.py` & `freefang-server-0.4.1/freefang/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,21 @@
 		self.connections = {} # Dictionnary associating connections to players
 		self.firstnight = True
 		self.roles = {} # The number of players for each role should be decided by the client upon game creation and should be implemented alongside the protocol
 		
 		self.town_voting_scheme = "absmaj"
 		self.werewolf_voting_scheme = "relmaj"
 	
+
+	# Add a player to the list of night deaths
+	def add_to_night_deaths(self, player):
+		if player not in self.nightdeaths:
+			self.nightdeaths.append(player)
+
+
 	# This function is a shortcut to send a packet and remove the player if the connection is dead
 	def send_packet(self, packet, con):
 		try:
 			fn.send_packet(packet, con)
 		except (BrokenPipeError, ConnectionResetError):
 			self.remove_player(con)
 		
@@ -134,37 +141,40 @@
 		
 		
 	def kill_player(self, player, reason=None):
 		
 		# If the player is protected we do nothing. 
 		if player.protected:
 			return 1
+		if not player.alive:
+			return 1
 		print(player.name + " died")
 
 		
 		# If the player died during the night we keep it in a list to notify the other players when the day rises
 		# Otherwise we just send the packet right away
 		if self.up != 0 and self.up != Hunter:
-			self.nightdeaths.append(player)
+			self.add_to_night_deaths(player)
 			return 0
 		player.alive = False
 
 		
 		# Notify everyone that player died
 		event = packets.Player_death(name=player.name, role=player.role.__name__, reason=reason)
 		
 		self.sendall(utils.obj_to_json(event))
 		
 		# Remove player from various lists reserved to living players
 		if player in self.werewolves:
 			self.werewolves.remove(player)
-		else if player in self.villagers:
+		elif player in self.villagers:
 			self.villagers.remove(player)
 			
-		self.alive.remove(player)
+		if player in self.alive:
+			self.alive.remove(player)
 		
 		# If the dead player is a hunter we need to wait for him to make his kill
 		if player.role == Hunter:
 			self.up = Hunter
 			self.eventloop()
 		if player.lover:
 			player.lover.lover = None
@@ -324,14 +334,15 @@
 			self.up = 0
 			self.time = 1
 
 
 			
 			
 			# Notify all players of deaths that happened during the night. 
+			print([s.name for s in self.nightdeaths])
 			for death in self.nightdeaths:
 				self.kill_player(death)
 			self.nightdeaths = []
 			self.up = 0
 			if not self.game_continues(): # Game ended during the night, we dip
 				break
 			self.sendall(utils.obj_to_json(packets.Town_Vote_Begin()))
```

### Comparing `freefang-server-0.4.0/freefang/net.py` & `freefang-server-0.4.1/freefang/net.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang/packets.py` & `freefang-server-0.4.1/freefang/packets.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang/roles.py` & `freefang-server-0.4.1/freefang/roles.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang/utils.py` & `freefang-server-0.4.1/freefang/utils.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang/voting.py` & `freefang-server-0.4.1/freefang/voting.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.4.0/freefang_server.egg-info/PKG-INFO` & `freefang-server-0.4.1/freefang_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `freefang-server-0.4.0/pyproject.toml` & `freefang-server-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name  = "freefang-server"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Solaris", email="iusegentoobtw@protonmail.com" },
   { name="lukakralik", email="luka.kralik@gmail.com"}
 ]
 description = "The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)"
 readme = "README.md"
 classifiers = [
```

