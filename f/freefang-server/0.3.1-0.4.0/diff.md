# Comparing `tmp/freefang-server-0.3.1.tar.gz` & `tmp/freefang-server-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freefang-server-0.3.1.tar", last modified: Tue Jul  4 00:10:28 2023, max compression
+gzip compressed data, was "freefang-server-0.4.0.tar", last modified: Sat Jul 15 23:32:35 2023, max compression
```

## Comparing `freefang-server-0.3.1.tar` & `freefang-server-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:10:28.269533 freefang-server-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-04 00:10:16.000000 freefang-server-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 00:10:28.269533 freefang-server-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-04 00:10:16.000000 freefang-server-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:10:28.269533 freefang-server-0.3.1/freefang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-04 00:10:16.000000 freefang-server-0.3.1/freefang/voting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:10:28.269533 freefang-server-0.3.1/freefang_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 00:10:28.000000 freefang-server-0.3.1/freefang_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 00:10:28.000000 freefang-server-0.3.1/freefang_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:10:28.000000 freefang-server-0.3.1/freefang_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 00:10:28.000000 freefang-server-0.3.1/freefang_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 00:10:28.000000 freefang-server-0.3.1/freefang_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 00:10:16.000000 freefang-server-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:10:28.269533 freefang-server-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 00:10:16.000000 freefang-server-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-15 23:32:23.000000 freefang-server-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-15 23:32:35.812506 freefang-server-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 23:32:23.000000 freefang-server-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/freefang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 23:32:23.000000 freefang-server-0.4.0/freefang/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.812506 freefang-server-0.4.0/freefang_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 23:32:35.000000 freefang-server-0.4.0/freefang_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-15 23:32:23.000000 freefang-server-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 23:32:35.812506 freefang-server-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-15 23:32:23.000000 freefang-server-0.4.0/setup.py
```

### Comparing `freefang-server-0.3.1/LICENSE` & `freefang-server-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freefang-server-0.3.1/PKG-INFO` & `freefang-server-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.3.1
+Version: 0.4.0
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -48,7 +48,18 @@
 
 
 # Protocol documentation
 
 Full protocol documentation in PROTOCOL.md with examples and complete descriptions.   
 
 
+# Contribute
+There are many ways you can help the FreeFang project and we would be extremely thankful.
+Those include but aren't limited to:
+
+- Contributing code
+- Contributing ideas
+- Hosting a server
+- Writing a client
+- Finding and reporting bugs
+- Testing on different platforms (Windows, MacOS, *BSD)
+- Spreading the word about FreeFang
```

### Comparing `freefang-server-0.3.1/freefang/main.py` & `freefang-server-0.4.0/freefang/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import time
 import struct 
 import argparse
 import ssl
 import os
 
 VERSIONSTR = """
-FreeFang Server 0.3.1
+FreeFang Server 0.4.0
 Written by @Solirs and @lukakralik
 Licensed under AGPLv3.0
 Source code at https://github.com/FreeFangGame/freefang-server
 """
 
 def parse_ruleset(ruleset, game):
 	if ruleset.town_voting_scheme:
@@ -106,48 +106,51 @@
 						game = models.WWgame()
 						game.playercap = packet.headers.playercap
 						parse_ruleset(packet.headers.ruleset, game)
 	
 						for rl in game.roles: 
 							if rl.nightrole:
 								game.nightroles.append(rl)
-							
+
 						games[gameid] = game
 						net.send_packet(utils.obj_to_json(packets.Game_created(gameid=gameid)), i) # Send player a packet confirming success
 						
 						print("New game")
 					
 					# Game joining
 					elif packet.action == "game_join":
-						if not games.get(packet.headers.gameid): # If the game for the proposed gameid doesn't exist
+						gameid = packet.headers.gameid.strip()
+						if not games.get(gameid): # If the game for the proposed gameid doesn't exist
 							net.send_packet(utils.obj_to_json(packets.Action_failure(error="game_not_found")), i)
+						elif len(packet.headers.name) > 20:
+							net.send_packet(utils.obj_to_json(packets.Action_failure(error="name_too_long")), i)
 						else:
-							game = games[packet.headers.gameid]
+							game = games[gameid]
 
 							if packet.headers.name in [s.name for s in game.players]:
 								net.send_failure(i, "name_already_taken")
 								continue
 								
 							p = models.Player()
 							p.name = packet.headers.name
 							p.connection = i
 							connections[i] = p
 							p.game = game
 							for spl in game.players:
 								net.send_packet(utils.obj_to_json(packets.Player_join(username=p.name)), spl.connection)
 							game.players.append(p)
-							net.send_packet(utils.obj_to_json(packets.Added_to_game(username=packet.headers.name, players=[i.name for i in game.players])), i) # Send player a packet confirming success
+							net.send_packet(utils.obj_to_json(packets.Added_to_game(username=packet.headers.name, players=[i.name for i in game.players], gameid=gameid)), i) # Send player a packet confirming success
 
 							if len(game.players) == game.playercap:
 
 								thread = threading.Thread(target=game.gameloop)
 								for i in game.players:
 									inputs.remove(i.connection)
 									outputs.remove(i.connection)
-								del games[packet.headers.gameid]
+								del games[gameid]
 								thread.start()
 					elif packet.action == "pre_game_message":
 						sender = connections[i]
 						for spl in sender.game.players:
 							net.send_message(sender.name, packet.headers.message, spl.connection)
 								
 				except Exception as e:
```

### Comparing `freefang-server-0.3.1/freefang/models.py` & `freefang-server-0.4.0/freefang/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		self.name = ""
 		self.connection = 0
 		self.voted_by = 0 # Number of people who voted for this player
 		self.voted = False
 		self.time = 0 # 0 = Night, 1 = Day
 		self.protected = None # name of the protected player
 		self.game = None
-
+		self.lover = None
 		#Witch stuff
 		self.haskilled = 0
 		self.hasrevived = 0
 	def iswerewolf(self):
 		return issubclass(self.role, Werewolf) and self.alive
 			
 
@@ -47,18 +47,18 @@
 		self.inputs = []
 		self.outputs = []
 		self.read = []
 		self.write = []
 		self.msgqueues = {}
 		self.nightroles = [] # Roles that should be woken up at night, in order
 		self.up = 0 # The current role which is woken up, 0 if day.
-		self.action_to_function = {"werewolf_vote": Werewolf.vote, "town_vote": Villager.vote, "town_message": self.townmessage, "werewolf_message": self.werewolfmessage, "hunter_kill": Hunter.kill, "seer_reveal":Seer.reveal, "protector_protect": Protector.protect, "witch_kill": Witch.kill, "witch_revive": Witch.revive}
+		self.action_to_function = {"werewolf_vote": Werewolf.vote, "town_vote": Villager.vote, "town_message": self.townmessage, "werewolf_message": self.werewolfmessage, "hunter_kill": Hunter.kill, "seer_reveal":Seer.reveal, "protector_protect": Protector.protect, "witch_kill": Witch.kill, "witch_revive": Witch.revive, "witch_pass_turn": Witch.passturn, "cupid_infatuate": Cupid.infatuate}
 		self.votes = []
 		self.connections = {} # Dictionnary associating connections to players
-
+		self.firstnight = True
 		self.roles = {} # The number of players for each role should be decided by the client upon game creation and should be implemented alongside the protocol
 		
 		self.town_voting_scheme = "absmaj"
 		self.werewolf_voting_scheme = "relmaj"
 	
 	# This function is a shortcut to send a packet and remove the player if the connection is dead
 	def send_packet(self, packet, con):
@@ -87,19 +87,24 @@
 				self.werewolves.append(spl)
 			else:
 				self.villagers.append(spl)
 			
 				
 	def townmessage(self, headers, game, connection):
 
+		if (not headers.sender.alive):
+			return 1;
+		
 		for i in self.players:
 			fn.send_message(headers.sender.name, headers.message, i.connection) # Send it to all players
 	
 	def werewolfmessage(self, headers, game, connection):
-
+		if (not headers.sender.alive):
+			return 1;
+		
 		for i in self.werewolves:
 			fn.send_message(headers.sender.name, headers.message, i.connection) # Send it to all werewolves
 		
 		
 			
 	def update_player_count(self):
 		num_players = len(self.players)
@@ -148,24 +153,28 @@
 		event = packets.Player_death(name=player.name, role=player.role.__name__, reason=reason)
 		
 		self.sendall(utils.obj_to_json(event))
 		
 		# Remove player from various lists reserved to living players
 		if player in self.werewolves:
 			self.werewolves.remove(player)
-		else:
+		else if player in self.villagers:
 			self.villagers.remove(player)
 			
 		self.alive.remove(player)
 		
 		# If the dead player is a hunter we need to wait for him to make his kill
 		if player.role == Hunter:
 			self.up = Hunter
 			self.eventloop()
-		
+		if player.lover:
+			player.lover.lover = None
+			self.kill_player(player.lover)
+			player.lover = None
+
 		# Add player to list of dead players
 		self.dead.append(player)
 
 		self.roles[player.role] -= 1
 		
 
 	def handle_disconnections(self):
@@ -237,14 +246,15 @@
 							# Set end to true to end the loop after message sending is done, then break as no more packets are needed
 							end = True
 							break
 						else: # If 1 is returned then something went wrong, the packet is probably bad (for example voting someone who doesnt exist)
 							fn.send_failure(i, error=None)
 							pass
 					except Exception as e:
+						print("===HANDLED ERROR===")
 						traceback.print_exc()
 						fn.send_failure(i, error=None)
 				except:
 					self.remove_player(i)
 					
 
 
@@ -285,26 +295,32 @@
 		# Setup I/O channels for select as well as message queue for each player
 		self.inputs = [i.connection for i in self.players]
 		self.outputs = [i.connection for i in self.players]
 
 		while self.game_continues(): 
 			# Game should go on as long as there are villagers and werewolves, keeping the day night cycle
 			self.sendall(utils.obj_to_json(packets.Time_change(time="night"))) # Notify everyone night has fallen
-
 			for i in self.nightroles:
-				if self.roles[i] > 0:
+				# This is to make sure a player who was killed during the night does not wake up
+				playerwithrole = [x for x in self.players if x.role == i][0]
+				if self.roles[i] > 0 and not playerwithrole in self.nightdeaths:
+					# If the role is a first night role and its not the first night, we skip it.
+					if i.firstnightrole and not self.firstnight:
+						continue
+
 					self.queueall(utils.obj_to_json(packets.Role_wakeup(role=i.__name__))) # Notify everyone role has woken up
 					self.up = i
 					# Run the role's wake up event function
 					try:
 						i.onwakeup(self)
 					except:
+						traceback.print_exc()
 						pass
 					self.eventloop()
-			
+			self.firstnight = False
 			# Remove all protections 
 			for player in self.players:
 				player.protected = None
 			self.sendall(utils.obj_to_json(packets.Time_change(time="day"))) # Notify everyone day has risen
 			self.up = 0
 			self.time = 1
```

### Comparing `freefang-server-0.3.1/freefang/net.py` & `freefang-server-0.4.0/freefang/net.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.3.1/freefang/packets.py` & `freefang-server-0.4.0/freefang/packets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class Added_to_game: #Packet for when a player is added to a game
-	def __init__(self, username, players):
+	def __init__(self, username, players, gameid):
 		self.action = "added_to_game"
 		self.headers = {
 			"username": username,
-			"players": players # List of the players currently in the game
+			"players": players, # List of the players currently in the game
+			"gameid": gameid
 		}
 
 class Player_join:
 	def __init__(self, username):
 		self.action = "player_join"
 		self.headers = {
 			"name": username,
@@ -99,38 +100,47 @@
 	def __init__(self, outcome):
 		self.action = "game_end"
 		self.headers = {
 			"outcome": outcome
 		}
 
 class ChatMessage:
-    def __init__(self, sender, message, timestamp):
-        self.action = "chat_message"
-        self.headers = {
-            "sender": sender,
-            "message": message,
-            "timestamp": timestamp
-        }
+	def __init__(self, sender, message, timestamp):
+		self.action = "chat_message"
+		self.headers = {
+			"sender": sender,
+			"message": message,
+			"timestamp": timestamp
+		}
 
 class SeerReveal:
-    def __init__(self, role, name):
-        self.action = "seer_role_reveal"
-        self.headers = {
+	def __init__(self, role, name):
+		self.action = "seer_role_reveal"
+		self.headers = {
 			"role": role,
 			"name": name
-        }
-        
+		}
+		
 class Town_Vote_Begin:
 	def __init__(self):
 		self.action = "town_vote_begin"
 
 class Check_alive:
 	def __init__(self):
 		self.action = "check_alive"
 	
 # This packet is supposed to be sent to the witch upon wakeup to
 # Notify them of the players which have died during the night
 class Witch_send_dead:
 	def __init__(self, players):
 		self.action = "witch_send_dead"
-		self.dead = players
-	
+		self.headers = {
+			"dead": players
+		}
+	
+# Sent to players who are coupled with eachother by the Cupid role
+class Player_coupled:
+	def __init__(self, player):
+		self.action = "player_coupled"
+		self.headers = {
+			"lover": player
+		}
```

### Comparing `freefang-server-0.3.1/freefang/roles.py` & `freefang-server-0.4.0/freefang/roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 			
 			
 
 			
 
 class Werewolf(Role):
 	nightrole = 1
-	order = 3
+	order = 4
+	firstnightrole = 0
 	def __init__(self):
 		super(Werewolf, self).__init__()
 		pass
 		
 	@staticmethod
 	def vote(headers, game, connection):
 		
@@ -105,15 +106,17 @@
 		else:
 			return 1
 		
 		
 # The seer is supposed to be able to learn about the role of one player each night
 class Seer:
 	nightrole = 1
-	order = 2
+	order = 3
+	firstnightrole = 0
+
 	@staticmethod
 	def reveal(headers, game, connection):
 		target = game.getplayerbyname(headers.target)
 		# Check if the player is actually a seer, if the role currently woken up is seer, and if the target is alive
 		if game.up == Seer and headers.sender.role == Seer and target.alive and headers.sender.alive:
 			# Create packet
 			packet = packets.SeerReveal(target.role.__name__, target.name)
@@ -131,16 +134,18 @@
 		if game.up == Hunter and headers.sender.role == Hunter and target.alive:
 			game.kill_player(target, reason="hunter_kill")
 			return 2
 		return 1
 
 # can prevent one person of his choosing from dying at each night	
 class Protector(Role):
+	firstnightrole = 0
+
 	nightrole = 1
-	order = 1
+	order = 2
 	def __init__(self):
 		super(Protector, self).__init__()
 	
 	@staticmethod
 	def protect(headers, game, connection):
 		target = game.getplayerbyname(headers.target)
     
@@ -148,17 +153,41 @@
 		if headers.sender.alive and target.alive and game.up == Protector:
 			target.protected = True
 			return 2
 		return 1
 
 # The witch can kill and revive one player per game who died during the night.
 # She is supposed to wake up last as she can only revive people who died during each night she wakes up in
+
+class Cupid(Role):
+	firstnightrole = 1
+	nightrole = 1
+	order = 1
+	@staticmethod
+	def infatuate(headers, game, connection):
+		target1 = game.getplayerbyname(headers.target1)
+		target2 = game.getplayerbyname(headers.target2)
+
+		if game.up == Cupid and headers.sender.role == Cupid:
+			target1.lover = target2
+			target2.lover = target1
+
+			game.send_packet(utils.obj_to_json(packets.Player_coupled(target1.name)), target2.connection)
+			game.send_packet(utils.obj_to_json(packets.Player_coupled(target2.name)), target1.connection)
+			
+			return 2
+		else:
+			return 1
+	
+
+
 class Witch(Role):
+	firstnightrole = 0
 	nightrole = 1
-	order = 4
+	order = 5
 	@staticmethod
 	def kill(headers, game, connection):
 		target = game.getplayerbyname(headers.target)
 		if game.up == Witch and headers.sender.role == Witch and not headers.sender.haskilled and target.alive:
 			game.kill_player(target)
 			headers.sender.haskilled = 1
 			return 2
@@ -176,14 +205,18 @@
 		else:
 			return 1
 	@staticmethod
 	def onwakeup(game):
 		dead = [i.name for i in game.nightdeaths]
 		event = utils.obj_to_json(packets.Witch_send_dead(dead))
 		game.sendrole(event, Witch)
+	
+	@staticmethod
+	def passturn(headers, game, connection):
+		return 2
 
 class Vote:
     def __init__(self, target, sender):
         self.sender = sender
         self.target = target
 
 class TownVote(Vote):
```

### Comparing `freefang-server-0.3.1/freefang/utils.py` & `freefang-server-0.4.0/freefang/utils.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.3.1/freefang/voting.py` & `freefang-server-0.4.0/freefang/voting.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.3.1/freefang_server.egg-info/PKG-INFO` & `freefang-server-0.4.0/freefang_server.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.3.1
+Version: 0.4.0
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -48,7 +48,18 @@
 
 
 # Protocol documentation
 
 Full protocol documentation in PROTOCOL.md with examples and complete descriptions.   
 
 
+# Contribute
+There are many ways you can help the FreeFang project and we would be extremely thankful.
+Those include but aren't limited to:
+
+- Contributing code
+- Contributing ideas
+- Hosting a server
+- Writing a client
+- Finding and reporting bugs
+- Testing on different platforms (Windows, MacOS, *BSD)
+- Spreading the word about FreeFang
```

### Comparing `freefang-server-0.3.1/pyproject.toml` & `freefang-server-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name  = "freefang-server"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Solaris", email="iusegentoobtw@protonmail.com" },
   { name="lukakralik", email="luka.kralik@gmail.com"}
 ]
 description = "The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)"
 readme = "README.md"
 classifiers = [
```

