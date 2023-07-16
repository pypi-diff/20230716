# Comparing `tmp/freefang_qt-0.1.2.tar.gz` & `tmp/freefang_qt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freefang_qt-0.1.2.tar", last modified: Wed Jul  5 22:45:26 2023, max compression
+gzip compressed data, was "freefang_qt-0.2.0.tar", last modified: Sun Jul 16 00:15:08 2023, max compression
```

## Comparing `freefang_qt-0.1.2.tar` & `freefang_qt-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/game_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/game_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/gameloop.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/packets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt/qml/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/ActionButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Create_Game.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Game_UI.qml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/HunterKill.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Join_Game.qml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/ProtectorProtect.qml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/SeerReveal.qml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Vote.qml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Werewolfvote.qml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Witch_kill.qml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Witch_revive.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/main.qml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:08.360805 freefang_qt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-16 00:15:08.360805 freefang_qt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:08.356805 freefang_qt-0.2.0/freefang_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/game_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/game_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/gameloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/packets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:08.356805 freefang_qt-0.2.0/freefang_qt/qml/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/ActionButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Create_Game.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Cupidinfatuate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Game_UI.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/HunterKill.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Join_Game.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/ProtectorProtect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/SeerReveal.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Vote.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Werewolfvote.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Witch_kill.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Witch_revive.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/Witchpassturnbtn.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/qml/main.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/freefang_qt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:15:08.356805 freefang_qt-0.2.0/freefang_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 00:15:08.000000 freefang_qt-0.2.0/freefang_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 00:15:08.360805 freefang_qt-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-16 00:14:53.000000 freefang_qt-0.2.0/setup.py
```

### Comparing `freefang_qt-0.1.2/LICENSE` & `freefang_qt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/game_creation.py` & `freefang_qt-0.2.0/freefang_qt/game_creation.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/gameloop.py` & `freefang_qt-0.2.0/freefang_qt/gameloop.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 	playername = ""
 	time = ""
 	up = ""
 	role = ""
 	players = []
 	werewolves = [] #Only used if the player is a werewolf
 	game_started = False
+	lovers = []# used in self.cupid_ifatuate to determine if a first player was chosen.
 
 
 	def __init__(self):
 		super(Game_loop, self).__init__()
 		
 	def handle_time_change(self, packet):
 		self.remove_buttons.emit()
@@ -53,15 +54,16 @@
 		self.chatupdate.emit(f"The role: {packet.headers.role} wakes up")
 		
 		# Associate different roles to their action buttons
 		role_to_btn = {
 			"Werewolf": "Werewolfvote",
 			"Seer": "SeerReveal",
 			"Hunter": "HunterKill",
-			"Protector": "ProtectorProtect"
+			"Protector": "ProtectorProtect",
+			"Cupid": "Cupidinfatuate"
 			#"Witch": "Witch_kill" # The signal function in the QML should also add the reive buttons
 		}
 		
 		btn = role_to_btn[packet.headers.role]
 		self.up = packet.headers.role
 		
 		if packet.headers.role == self.role:
@@ -86,30 +88,34 @@
 		
 	def handle_game_end(self, packet):
 		self.remove_buttons.emit()
 		if packet.headers.outcome == "werewolf_win":
 			self.chatupdate.emit("The werewolves have won")
 		elif packet.headers.outcome == "town_win":
 			self.chatupdate.emit("The village has won")
-			
+		self.chatupdate.emit("Reminder you can press escape to quit!")
+
 	def handle_added_to_game(self, packet):
 		self.chatupdate.emit("You have joined the game")
+		self.chatupdate.emit(f"The game ID is: {packet.headers.gameid}")
+		self.chatupdate.emit("Press escape to quit!")
+
 		for i in packet.headers.players:
 			self.playeradd.emit(i)
 			spl = Player(i)
 			self.players.append(spl)
 		self.playername = packet.headers.username
 	def handle_player_join(self, packet):
-		self.chatupdate.emit(f"{packet.headers.name} joined the game")
+		self.chatupdate.emit(f"<font color=\"red\">{packet.headers.name}</font> joined the game")
 		self.playeradd.emit(packet.headers.name)
 		spl = Player(packet.headers.name)
 		self.players.append(spl)
 
 	def handle_chat_message(self, packet):
-		self.chatupdate.emit(f"{packet.headers.sender}: {packet.headers.message}")
+		self.chatupdate.emit(f"<font color=\"red\">{packet.headers.sender}</font>: {packet.headers.message}")
 		
 	def handle_seer_role_reveal(self, packet):
 		self.chatupdate.emit(f"{packet.headers.name} has the role {packet.headers.role}")
 	def begin_town_vote(self, packet):
 		self.chatupdate.emit("The town may now vote")
 		self.setaction.emit("Vote")
 	def handle_leave(self, packet):
@@ -117,30 +123,32 @@
 		self.playerrm.emit(packet.headers.name)
 
 	def handle_werewolf_vote(self, packet):
 		self.chatupdate.emit(f"{packet.headers.sender} votes for {packet.headers.target}")
 
 	# This function should be the one that creates the buttons allowing the witch to do its action
 	def handle_witch_send_dead(self, packet):
-		deadplayers = " ".join(packet.dead)
+		deadplayers = " ".join(packet.headers.dead)
 		self.chatupdate.emit(f"The following players {deadplayers} died during this night.")
 		self.chatupdate.emit(f"Would you like to revive someone, kill someone else, or pass?")
 
-		self.witchaction.emit(packet.dead)
+		self.witchaction.emit(packet.headers.dead)
 
 	# Handle the packet that is sent to all werewolves on game start
 	# Which contains the names of all other werewolves
 	def handle_show_werewolves(self, packet):
 		for i in packet.headers.werewolves:
 		 	if i != self.playername:
 					self.werewolves.append(i)
 			
 		if len(self.werewolves) > 0:
 			self.chatupdate.emit(f"Your fellow werewolves are {' '.join(self.werewolves)}")
 		
+	def handle_player_coupled(self, packet):
+		self.chatupdate.emit(f"Cupid has coupled you with {packet.headers.lover}, if one of you dies then the other will also die from the grief.")
 
 	def getplayerbyname(self, player):
 		return [i for i in self.players if i.name == player][0]
 
 	@Slot(str, result=bool)
 	def isalive(self, player):
 		spl = self.getplayerbyname(player)
@@ -159,15 +167,16 @@
 			"player_join": self.handle_player_join,
 			"chat_message": self.handle_chat_message,
 			"seer_role_reveal": self.handle_seer_role_reveal,
 			"town_vote_begin": self.begin_town_vote,
 			"player_leave": self.handle_leave,
 			"werewolf_vote": self.handle_werewolf_vote,
 			"witch_send_dead": self.handle_witch_send_dead,
-			"show_werewolves": self.handle_show_werewolves
+			"show_werewolves": self.handle_show_werewolves,
+			"player_coupled": self.handle_player_coupled
 		}
 		if packet_to_func.get(packet.action):
 			packet_to_func[packet.action](packet)
 			return 0
 		else:
 			return 1
 
@@ -250,11 +259,44 @@
 		net.send_packet(packet, global_data.socket)		
 			
 	@Slot(str)
 	def witch_revive(self, player):
 		self.remove_buttons.emit()
 		packet = utils.object_to_json(packets.Witch_revive(player))
 		net.send_packet(packet, global_data.socket)		
-			
+	@Slot()
+	def witch_pass_turn(self):
+		self.remove_buttons.emit()
+		packet = utils.object_to_json(packets.Witch_pass_turn())
+		net.send_packet(packet, global_data.socket)		
+
+				
 	@Slot(str, result=bool)
 	def iswerewolf(self, player):
 		return player in self.werewolves
+	@Slot(str)
+	def cupid_infatuate(self, player):
+		if (len(self.lovers) == 0):
+			self.lovers.append(player)
+			return
+		else:
+			if (self.lovers[0] == player):
+				return
+			
+			self.lovers.append(player)
+			self.remove_buttons.emit()
+			packet = utils.object_to_json(packets.Cupid_infatuate(self.lovers[0], self.lovers[1]))
+			net.send_packet(packet, global_data.socket)		
+
+	@Slot()
+	def quitgame(self):
+		self.timer.stop()
+		global_data.socket.close()
+		# Reset game to a blank state
+		self.playername = ""
+		self.time = ""
+		self.up = ""
+		self.role = ""
+		self.players = []
+		self.werewolves = [] #Only used if the player is a werewolf
+		self.game_started = False
+		self.lovers = []# used in self.cupid_ifatuate to determine if a first player was chosen.
```

### Comparing `freefang_qt-0.1.2/freefang_qt/main.py` & `freefang_qt-0.2.0/freefang_qt/main.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/net.py` & `freefang_qt-0.2.0/freefang_qt/net.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/packets.py` & `freefang_qt-0.2.0/freefang_qt/packets.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,8 +77,24 @@
 		}
 
 class Witch_revive:
 	def __init__(self, target):
 		self.action = "witch_revive"
 		self.headers = {
 			"target": target
-		}
+		}
+
+
+class Witch_pass_turn:
+	def __init__(self):
+		self.action = "witch_pass_turn"
+		self.headers = {
+		}
+
+class Cupid_infatuate:
+	def __init__(self, targ1, targ2):
+		self.action = "cupid_infatuate"
+		self.headers = {
+			"target1": targ1,
+			"target2": targ2
+		}
+
```

### Comparing `freefang_qt-0.1.2/freefang_qt/qml/Create_Game.qml` & `freefang_qt-0.2.0/freefang_qt/qml/Create_Game.qml`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/qml/Game_UI.qml` & `freefang_qt-0.2.0/freefang_qt/qml/Game_UI.qml`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 				}
 				}
 
 			}
 		}
 		Component {
 			id: chatdelegate
-			Item {
-				width: 200; height: 28
-				Label {
-					text: " " + message
-					color: "white"
+			Label {
+
+				id: chatlabel
+				width: chat.width
+				text: message
+				color: "white"
+
+				wrapMode: Text.Wrap
 
-				}
 			}
 		}
 
 		ListModel {
 			 id: chatmodel
 		}
 		ListModel {
@@ -64,30 +66,37 @@
 
 
 			ColumnLayout{
 
 				id: chatlayout
 				height: parent.height
 				width: parent.width
+
+
 				ScrollView {
+					id: chatsv
 					height: 180
+					Layout.leftMargin: 5
+
 					Layout.fillHeight: true
 					Layout.fillWidth: true
+					width: 1400
+					clip: true
+
 
 					ScrollBar.vertical.policy: ScrollBar.AsNeeded
 					ListView {
-						anchors.topMargin: 20
-						anchors.leftMargin: 50
+						spacing: 4
 						Layout.fillHeight: true
 						Layout.fillWidth: true
 					   
 						id: chat
 						model: chatmodel
 						delegate: chatdelegate
-
+    					clip: true
 					}
 
 			   }
 				TextField{
 						id: chat_input
 						placeholderText: "Message"
 						height: 10
@@ -120,33 +129,37 @@
 
 			ScrollView {
 			
 				width: parent.width
 				height: parent.height
 			   
 				ScrollBar.vertical.policy: ScrollBar.AsNeeded
+			
 				ListView {
 					spacing: 13
 					Layout.fillHeight: true
 					Layout.fillWidth: true
 				   
 					id: players
 					model: playermodel
 					delegate: playerdelegate
+					clip: true
 
 				}
 
 		   }
 		}
 
 				Connections {
 						target: game_loop
 
 						function onChatupdate(msg) {
+
 							chatmodel.append({message: msg})
+							chatsv.ScrollBar.vertical.position = 1
 						}
 						function onPlayeradd(spl){
 
 							playermodel.append({player: spl, buttonsrc: ""})
 
 						}
 						function onPlayerrm(spl){
@@ -180,11 +193,15 @@
 							for( var i = 0; i < playermodel.rowCount(); i++ ) {
 								if (playermodel.get(i).player != game_loop.playername && game_loop.isalive(playermodel.get(i).player)){
 									playermodel.get(i).buttonsrc = "Witch_kill.qml";
 								} 
 								if(deaths.indexOf(playermodel.get(i).player) > -1){
 									playermodel.get(i).buttonsrc = "Witch_revive.qml"
 								}
+								if (playermodel.get(i).player == game_loop.playername){
+									playermodel.get(i).buttonsrc = "Witchpassturnbtn.qml"
+
+								}
 							}
 						}
 				}
 }
```

### Comparing `freefang_qt-0.1.2/freefang_qt/qml/Join_Game.qml` & `freefang_qt-0.2.0/freefang_qt/qml/Join_Game.qml`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.2/freefang_qt/qml/main.qml` & `freefang_qt-0.2.0/freefang_qt/qml/main.qml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 import QtQuick
 import QtQuick.Controls
 import QtQuick.Layouts
 import QtQuick.Controls.Material 
-
+import QtQuick.Dialogs
 
 ApplicationWindow {
+	id: mainwin
     visible: true
     width: 700
     height: 500
     visibility: "Maximized"
     title: "freefang-qt"
-    property string version: "0.1.1"
+    property string version: "0.4.0"
 	property string gameid: "Game ID here"
 	property string gameserver: "127.0.0.1:9999"
 	property int playercap: 5
 	color: "#202020"
+
+	MessageDialog{
+		id: mainmenumd
+		text: "Are you sure you want to go back to the main menu?"
+    	buttons: MessageDialog.Ok | MessageDialog.Cancel	
+		onAccepted: {
+			stack.pop(null);
+			game_loop.quitgame();
+		}
+	}
+
+    Shortcut {
+        sequence: "Esc"
+        onActivated: {
+			mainmenumd.open();
+		}
+    }
+    
 	Connections {
 			target: game_creation_ui
 
 			function onGameidupdated(msg) {
 				gameid = msg;
 			}
 			function onGameserverupdated(msg) {
@@ -98,13 +117,15 @@
 				Item {
 					// Spacer
 					Layout.fillHeight: true
 				}
 
 			
         }
+
+
         
 
 }
 }
```

### Comparing `freefang_qt-0.1.2/freefang_qt.egg-info/SOURCES.txt` & `freefang_qt-0.2.0/freefang_qt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 freefang_qt.egg-info/SOURCES.txt
 freefang_qt.egg-info/dependency_links.txt
 freefang_qt.egg-info/entry_points.txt
 freefang_qt.egg-info/requires.txt
 freefang_qt.egg-info/top_level.txt
 freefang_qt/qml/ActionButton.qml
 freefang_qt/qml/Create_Game.qml
+freefang_qt/qml/Cupidinfatuate.qml
 freefang_qt/qml/Game_UI.qml
 freefang_qt/qml/HunterKill.qml
 freefang_qt/qml/Join_Game.qml
 freefang_qt/qml/ProtectorProtect.qml
 freefang_qt/qml/SeerReveal.qml
 freefang_qt/qml/Vote.qml
 freefang_qt/qml/Werewolfvote.qml
 freefang_qt/qml/Witch_kill.qml
 freefang_qt/qml/Witch_revive.qml
+freefang_qt/qml/Witchpassturnbtn.qml
 freefang_qt/qml/main.qml
```

### Comparing `freefang_qt-0.1.2/pyproject.toml` & `freefang_qt-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name  = "freefang_qt"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Solaris", email="iusegentoobtw@protonmail.com" }
 ]
 dependencies = [
 	"pyside6"
 ]
```

