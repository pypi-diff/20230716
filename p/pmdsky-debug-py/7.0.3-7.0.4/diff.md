# Comparing `tmp/pmdsky_debug_py-7.0.3-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 847397 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-12 04:27 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-12 04:27 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   728268 b- defN 23-Jul-12 04:27 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   694694 b- defN 23-Jul-12 04:27 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   715744 b- defN 23-Jul-12 04:27 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   694694 b- defN 23-Jul-12 04:27 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   735188 b- defN 23-Jul-12 04:27 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   694705 b- defN 23-Jul-12 04:27 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   246757 b- defN 23-Jul-12 04:27 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 04:27 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-12 04:28 pmdsky_debug_py-7.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 04:28 pmdsky_debug_py-7.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-12 04:28 pmdsky_debug_py-7.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-12 04:28 pmdsky_debug_py-7.0.3.dist-info/RECORD
-14 files, 4514494 bytes uncompressed, 845499 bytes compressed:  81.3%
+Zip file size: 864219 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-16 04:27 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-16 04:27 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   741315 b- defN 23-Jul-16 04:27 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   707741 b- defN 23-Jul-16 04:27 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   728791 b- defN 23-Jul-16 04:27 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   707741 b- defN 23-Jul-16 04:27 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   748733 b- defN 23-Jul-16 04:27 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   707752 b- defN 23-Jul-16 04:27 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   250307 b- defN 23-Jul-16 04:27 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 04:27 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-16 04:27 pmdsky_debug_py-7.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 04:27 pmdsky_debug_py-7.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-16 04:27 pmdsky_debug_py-7.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-16 04:27 pmdsky_debug_py-7.0.4.dist-info/RECORD
+14 files, 4596824 bytes uncompressed, 862321 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.3.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.3.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.3.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.3.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+e191eae18a"
+RELEASE = "v0.7.0+aa37f0ecb8"
```

## pmdsky_debug_py/eu.py

```diff
@@ -997,24 +997,82 @@
         [0xCC9C],
         [0x200CC9C],
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         [0xCD0C],
         [0x200CD0C],
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         [0xCF24],
         [0x200CF24],
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -15067,14 +15125,23 @@
         None,
         None,
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         None,
         None,
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -15111,23 +15178,45 @@
     RevealTrapsNearby = Symbol(
         None,
         None,
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        None,
+        None,
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x138A0],
         [0x22F0420],
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        None,
+        None,
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         [0x13938],
         [0x22F04B8],
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15758,14 +15847,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        None,
+        None,
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         [0x23074],
         [0x22FFBF4],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -16360,14 +16458,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        None,
+        None,
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         None,
         None,
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -16378,14 +16499,33 @@
         None,
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         None,
         None,
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -16411,14 +16551,39 @@
         None,
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        None,
+        None,
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        None,
+        None,
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BDF8],
         [0x2308978],
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16580,14 +16745,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        None,
+        None,
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         [0x31080],
         [0x230DC00],
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16638,14 +16812,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        None,
+        None,
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         [0x3141C],
         [0x230DF9C],
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16721,14 +16906,24 @@
         [0x23101FC],
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         [0x33734],
         [0x23102B4],
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16904,15 +17099,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         [0x36E58],
         [0x23139D8],
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         [0x37010],
         [0x2313B90],
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -16946,24 +17142,28 @@
 
     LowerOffensiveStat = Symbol(
         [0x374DC],
         [0x231405C],
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         [0x376F4],
         [0x2314274],
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         [0x3787C],
         [0x23143FC],
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -16986,14 +17186,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        None,
+        None,
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         [0x37C20],
         [0x23147A0],
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -17122,14 +17331,31 @@
         [0x231587C],
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         [0x38E18],
         [0x2315998],
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -17434,23 +17660,41 @@
         None,
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         [0x3BB00],
         [0x2318680],
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         None,
         None,
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17708,14 +17952,23 @@
         None,
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D6F4],
         [0x231A274],
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17810,14 +18063,54 @@
         [0x3EDEC],
         [0x231B96C],
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        None,
+        None,
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        None,
+        None,
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         [0x3F2DC],
         [0x231BE5C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -18395,17 +18688,16 @@
 
     TryActivateWeather = Symbol(
         [0x59384],
         [0x2335F04],
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         [0x59530],
         [0x23360B0],
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -18465,21 +18757,77 @@
         [0x2336DA4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        None,
+        None,
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        None,
+        None,
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        None,
+        None,
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        None,
+        None,
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         [0x5A478],
         [0x2336FF8],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        None,
+        None,
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         [0x5AF9C],
         [0x2337B1C],
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18507,14 +18855,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         [0x5BEE4],
         [0x2338A64],
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19636,14 +20008,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        None,
+        None,
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         [0x6B344],
         [0x2347EC4],
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -981,24 +981,82 @@
         None,
         None,
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         None,
         None,
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -14626,14 +14684,23 @@
         None,
         None,
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         None,
         None,
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -14670,23 +14737,45 @@
     RevealTrapsNearby = Symbol(
         None,
         None,
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        None,
+        None,
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        None,
+        None,
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         None,
         None,
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15268,14 +15357,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        None,
+        None,
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         None,
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -15870,14 +15968,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        None,
+        None,
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         None,
         None,
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -15888,14 +16009,33 @@
         None,
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         None,
         None,
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -15921,14 +16061,39 @@
         None,
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        None,
+        None,
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        None,
+        None,
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16090,14 +16255,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        None,
+        None,
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         None,
         None,
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16148,14 +16322,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        None,
+        None,
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         None,
         None,
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16231,14 +16416,24 @@
         None,
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         None,
         None,
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16414,15 +16609,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -16456,24 +16652,28 @@
 
     LowerOffensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         None,
         None,
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -16496,14 +16696,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        None,
+        None,
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         None,
         None,
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -16632,14 +16841,31 @@
         None,
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -16944,23 +17170,41 @@
         None,
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         None,
         None,
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         None,
         None,
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17218,14 +17462,23 @@
         None,
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17320,14 +17573,54 @@
         None,
         None,
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        None,
+        None,
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        None,
+        None,
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -17905,17 +18198,16 @@
 
     TryActivateWeather = Symbol(
         None,
         None,
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         None,
         None,
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -17969,21 +18261,77 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        None,
+        None,
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        None,
+        None,
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        None,
+        None,
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        None,
+        None,
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        None,
+        None,
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         None,
         None,
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18011,14 +18359,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19131,14 +19503,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        None,
+        None,
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         None,
         None,
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/jp.py

```diff
@@ -997,24 +997,82 @@
         [0xCC14],
         [0x200CC14],
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         None,
         None,
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         [0xCE9C],
         [0x200CE9C],
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -14870,14 +14928,23 @@
         None,
         None,
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         None,
         None,
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -14914,23 +14981,45 @@
     RevealTrapsNearby = Symbol(
         None,
         None,
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        None,
+        None,
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x13790],
         [0x22F1070],
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        None,
+        None,
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         [0x13828],
         [0x22F1108],
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15515,14 +15604,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        None,
+        None,
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         [0x22CD8],
         [0x23005B8],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -16117,14 +16215,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        None,
+        None,
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         None,
         None,
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -16135,14 +16256,33 @@
         None,
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         None,
         None,
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -16168,14 +16308,39 @@
         None,
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        None,
+        None,
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        None,
+        None,
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BBA0],
         [0x2309480],
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16337,14 +16502,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        None,
+        None,
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         [0x30DEC],
         [0x230E6CC],
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16395,14 +16569,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        None,
+        None,
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         [0x31184],
         [0x230EA64],
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16478,14 +16663,24 @@
         None,
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         [0x3349C],
         [0x2310D7C],
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16661,15 +16856,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         [0x36B88],
         [0x2314468],
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         [0x36D3C],
         [0x231461C],
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -16703,24 +16899,28 @@
 
     LowerOffensiveStat = Symbol(
         [0x37208],
         [0x2314AE8],
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         [0x3741C],
         [0x2314CFC],
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         [0x375A4],
         [0x2314E84],
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -16743,14 +16943,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        None,
+        None,
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         [0x37944],
         [0x2315224],
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -16879,14 +17088,31 @@
         [0x23162F0],
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         [0x38B30],
         [0x2316410],
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -17191,23 +17417,41 @@
         None,
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         [0x3B810],
         [0x23190F0],
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         None,
         None,
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17465,14 +17709,23 @@
         None,
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D404],
         [0x231ACE4],
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17567,14 +17820,54 @@
         [0x3EAFC],
         [0x231C3DC],
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        None,
+        None,
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        None,
+        None,
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         [0x3EFE8],
         [0x231C8C8],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -18152,17 +18445,16 @@
 
     TryActivateWeather = Symbol(
         None,
         None,
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         [0x5917C],
         [0x2336A5C],
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -18222,21 +18514,77 @@
         [0x23375A4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        None,
+        None,
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        None,
+        None,
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        None,
+        None,
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        None,
+        None,
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         [0x59F18],
         [0x23377F8],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        None,
+        None,
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         None,
         None,
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18264,14 +18612,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19390,14 +19762,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        None,
+        None,
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         [0x6ADA4],
         [0x2348684],
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -981,24 +981,82 @@
         None,
         None,
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         None,
         None,
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -14626,14 +14684,23 @@
         None,
         None,
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         None,
         None,
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -14670,23 +14737,45 @@
     RevealTrapsNearby = Symbol(
         None,
         None,
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        None,
+        None,
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        None,
+        None,
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         None,
         None,
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15268,14 +15357,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        None,
+        None,
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         None,
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -15870,14 +15968,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        None,
+        None,
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         None,
         None,
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -15888,14 +16009,33 @@
         None,
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         None,
         None,
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -15921,14 +16061,39 @@
         None,
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        None,
+        None,
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        None,
+        None,
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16090,14 +16255,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        None,
+        None,
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         None,
         None,
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16148,14 +16322,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        None,
+        None,
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         None,
         None,
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16231,14 +16416,24 @@
         None,
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         None,
         None,
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16414,15 +16609,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -16456,24 +16652,28 @@
 
     LowerOffensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         None,
         None,
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -16496,14 +16696,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        None,
+        None,
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         None,
         None,
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -16632,14 +16841,31 @@
         None,
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -16944,23 +17170,41 @@
         None,
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         None,
         None,
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         None,
         None,
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17218,14 +17462,23 @@
         None,
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17320,14 +17573,54 @@
         None,
         None,
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        None,
+        None,
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        None,
+        None,
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -17905,17 +18198,16 @@
 
     TryActivateWeather = Symbol(
         None,
         None,
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         None,
         None,
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -17969,21 +18261,77 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        None,
+        None,
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        None,
+        None,
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        None,
+        None,
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        None,
+        None,
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        None,
+        None,
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         None,
         None,
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18011,14 +18359,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19131,14 +19503,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        None,
+        None,
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         None,
         None,
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/na.py

```diff
@@ -997,24 +997,82 @@
         [0xCC14],
         [0x200CC14],
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        [0xCC38],
+        [0x200CC38],
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         [0xCC84],
         [0x200CC84],
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        [0xCCA8],
+        [0x200CCA8],
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        [0xCCE0],
+        [0x200CCE0],
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        [0xCDAC],
+        [0x200CDAC],
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        [0xCDF8],
+        [0x200CDF8],
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        [0xCE74],
+        [0x200CE74],
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         [0xCE9C],
         [0x200CE9C],
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -15151,14 +15209,23 @@
         [0x12AEC],
         [0x22EED2C],
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        [0x12C10],
+        [0x22EEE50],
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         [0x12CAC],
         [0x22EEEEC],
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -15195,23 +15262,45 @@
     RevealTrapsNearby = Symbol(
         [0x13398],
         [0x22EF5D8],
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        [0x137AC],
+        [0x22EF9EC],
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         [0x1382C],
         [0x22EFA6C],
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        [0x13834],
+        [0x22EFA74],
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         [0x138C4],
         [0x22EFB04],
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15842,14 +15931,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        [0x22F28],
+        [0x22FF168],
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         [0x22F88],
         [0x22FF1C8],
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -16444,14 +16542,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        [0x2A498],
+        [0x23066D8],
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        [0x2A4E8],
+        [0x2306728],
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         [0x2A684],
         [0x23068C4],
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -16462,14 +16583,33 @@
         [0x2306950],
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        [0x2A7C0],
+        [0x2306A00],
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        [0x2A8E8],
+        [0x2306B28],
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         [0x2A9B8],
         [0x2306BF8],
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -16495,14 +16635,39 @@
         [0x23078EC],
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        [0x2BA38],
+        [0x2307C78],
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        [0x2BAD8],
+        [0x2307D18],
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        [0x2BB14],
+        [0x2307D54],
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         [0x2BD0C],
         [0x2307F4C],
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16664,14 +16829,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        [0x30EDC],
+        [0x230D11C],
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         [0x30F4C],
         [0x230D18C],
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16722,14 +16896,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        [0x3123C],
+        [0x230D47C],
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         [0x312E8],
         [0x230D528],
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16805,14 +16990,24 @@
         [0x230F788],
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        [0x33558],
+        [0x230F798],
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         [0x33600],
         [0x230F840],
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16988,15 +17183,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         [0x36D38],
         [0x2312F78],
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         [0x36EF0],
         [0x2313130],
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -17030,24 +17226,28 @@
 
     LowerOffensiveStat = Symbol(
         [0x373BC],
         [0x23135FC],
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         [0x375D4],
         [0x2313814],
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         [0x3775C],
         [0x231399C],
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -17070,14 +17270,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        [0x37AA4],
+        [0x2313CE4],
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         [0x37B00],
         [0x2313D40],
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -17206,14 +17415,31 @@
         [0x2314E1C],
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        [0x38C20],
+        [0x2314E60],
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        [0x38C78],
+        [0x2314EB8],
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         [0x38CF8],
         [0x2314F38],
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -17518,23 +17744,41 @@
         [0x2317AF4],
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         [0x3B9E0],
         [0x2317C20],
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        [0x3BB18],
+        [0x2317D58],
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        [0x3BC48],
+        [0x2317E88],
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         [0x3BD10],
         [0x2317F50],
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17792,14 +18036,23 @@
         [0x2319748],
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        [0x3D58C],
+        [0x23197CC],
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         [0x3D5D4],
         [0x2319814],
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17894,14 +18147,54 @@
         [0x3ECCC],
         [0x231AF0C],
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        [0x3EE20],
+        [0x231B060],
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        [0x3EE64],
+        [0x231B0A4],
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        [0x3EF78],
+        [0x231B1B8],
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        [0x3F0FC],
+        [0x231B33C],
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        [0x3F124],
+        [0x231B364],
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         [0x3F1BC],
         [0x231B3FC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -18479,17 +18772,16 @@
 
     TryActivateWeather = Symbol(
         [0x59284],
         [0x23354C4],
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         [0x59430],
         [0x2335670],
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -18549,21 +18841,77 @@
         [0x23361D4],
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        [0x59FE4],
+        [0x2336224],
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        [0x5A020],
+        [0x2336260],
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        [0x5A180],
+        [0x23363C0],
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        [0x5A1AC],
+        [0x23363EC],
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         [0x5A1E8],
         [0x2336428],
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        [0x5A210],
+        [0x2336450],
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        [0x5A80C],
+        [0x2336A4C],
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        [0x5A844],
+        [0x2336A84],
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         [0x5AD0C],
         [0x2336F4C],
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18591,14 +18939,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        [0x5B8EC],
+        [0x2337B2C],
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        [0x5B928],
+        [0x2337B68],
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        [0x5B95C],
+        [0x2337B9C],
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         [0x5BC54],
         [0x2337E94],
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19720,14 +20092,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        [0x6ACD4],
+        [0x2346F14],
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         [0x6B084],
         [0x23472C4],
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -981,24 +981,82 @@
         None,
         None,
         None,
         "Checks if an item is one of the aura bows received at the start of the"
         " game.\n\nr0: item ID\nreturn: bool",
     )
 
+    IsLosableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be lost after fainting in a dungeon. Specifically calls"
+        " IsAuraBow and checks item::f_in_shop\nso that the player can't keep an aura"
+        " bow they haven't paid for yet.\n\nr0: item pointer\nreturn: bool",
+    )
+
     IsTreasureBox = Symbol(
         None,
         None,
         None,
         "Checks if the given item ID is a treasure box\n\nIn particular, it checks if"
         " the category of the item is CATEGORY_TREASURE_BOXES_1,"
         " CATEGORY_TREASURE_BOXES_2 or CATEGORY_TREASURE_BOXES_3.\n\nr0: item"
         " ID\nreturn: True if the item is a treasure box, false otherwise",
     )
 
+    IsStorableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be put into storage. Specifically checks for the Wonder"
+        " Egg, Poke, and Used TMs. Used TMs\nlikely can't be stored because the move"
+        " the TM teaches would be lost when sent to storage.\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsShoppableItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be bought and sold from a Kecleon shop. Includes items"
+        " like the Gold Thorn, Poke, Golden\nMask, Amber Tear, etc. Also has a special"
+        " check to make sure an item's buy and sell price is more than 0.\n\nr0:"
+        " item_id\nreturn: bool",
+    )
+
+    IsValidTargetItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a valid target item for missions. Returns true for any"
+        " item less than ITEM_UNNAMED_0x16B.\nAppears to check a list for valid items"
+        " above ITEM_UNNAMED_0x16B, but the list is empty?\n\nr0: item_id\nreturn:"
+        " bool",
+    )
+
+    IsItemUsableNow = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item can be used right now. Returns true for all items that are"
+        " not in a shop. If the item is in a\nshop, specifically checks for TMs/HMs and"
+        " items that provide permanent buffs (Gummis, Sitrus Berry, Ginseng,"
+        " etc).\n\nr0: item pointer\nreturn: bool",
+    )
+
+    IsTicketItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if an item is a ticket that can be used in the recycle shop"
+        " (ITEM_PRIZE_TICKET, ITEM_SILVER_TICKET,\nITEM_GOLD_TICKET, and"
+        " ITEM_PRISM_TICKET).\n\nr0: item_id\nreturn: bool",
+    )
+
     InitItem = Symbol(
         None,
         None,
         None,
         "Initialize an item struct with the given information.\n\nThis will resolve the"
         " quantity based on the item type. For Poké, the quantity code will always be"
         " set to 1. For thrown items, the quantity code will be randomly generated on"
@@ -14626,14 +14684,23 @@
         None,
         None,
         None,
         "Tries to drop the defender's item and places it on the floor.\n\nr0: attacker"
         " entity pointer\nr1: defender entity pointer",
     )
 
+    ApplyStealthRockTrapEffect = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from the stealth rock trap but does nothing if the"
+        " defender is a rock type.\n\nr0: attacker entity pointer\nr1: defender entity"
+        " pointer",
+    )
+
     ApplyToxicSpikesTrapEffect = Symbol(
         None,
         None,
         None,
         "Tries to inflict 10 damage on the defender and then tries to poison"
         " them.\n\nr0: attacker entity pointer\nr1: defender entity pointer",
     )
@@ -14670,23 +14737,45 @@
     RevealTrapsNearby = Symbol(
         None,
         None,
         None,
         "Reveals traps within the monster's viewing range.\n\nr0: entity pointer",
     )
 
+    ShouldRunMonsterAi = Symbol(
+        None,
+        None,
+        None,
+        "Checks a monster's monster_behavior to see whether or not the monster should"
+        " use AI. Only called on monsters with\na monster_behavior greater than or"
+        " equal to BEHAVIOR_FIXED_ENEMY. Returns false for BEHAVIOR_FIXED_ENEMY,"
+        " \nBEHAVIOR_WANDERING_ENEMY_0x8, BEHAVIOR_SECRET_BAZAAR_KIRLIA,"
+        " BEHAVIOR_SECRET_BAZAAR_MIME_JR,\nBEHAVIOR_SECRET_BAZAAR_SWALOT,"
+        " BEHAVIOR_SECRET_BAZAAR_LICKILICKY, and"
+        " BEHAVIOR_SECRET_BAZAAR_SHEDINJA.\n\nr0: monster entity pointer\nreturn: bool",
+    )
+
     DebugRecruitingEnabled = Symbol(
         None,
         None,
         None,
         "Always returns true. Called by SpecificRecruitCheck.\n\nSeems to be a function"
         " used during development to disable recruiting. If it returns false,"
         " SpecificRecruitCheck will also return false.\n\nreturn: true",
     )
 
+    TryActivateIqBooster = Symbol(
+        None,
+        None,
+        None,
+        "Increases the IQ of all team members holding the IQ Booster by"
+        " floor_properties::iq_booster_value amount unless the\nvalue is 0.\n\nNo"
+        " params.",
+    )
+
     IsSecretBazaarNpcBehavior = Symbol(
         None,
         None,
         None,
         "Checks if a behavior ID corresponds to one of the Secret Bazaar NPCs.\n\nr0:"
         " monster behavior ID\nreturn: bool",
     )
@@ -15268,14 +15357,23 @@
         " and player-inputted actions. If the action is not ACTION_NOTHING,"
         " ACTION_PASS_TURN, ACTION_WALK or ACTION_UNK_4, the monster's already_acted"
         " field is set to true. Includes a switch based on the action ID that performs"
         " the action, although some of them aren't handled by said swtich.\n\nr0:"
         " Pointer to monster entity",
     )
 
+    TryActivateFlashFireOnAllMonsters = Symbol(
+        None,
+        None,
+        None,
+        "Checks every monster for apply_flash_fire_boost. If it's true, activates Flash"
+        " Fire for the monster and sets\napply_flash_fire_boost back to false.\n\nNo"
+        " params.",
+    )
+
     HasStatusThatPreventsActing = Symbol(
         None,
         None,
         None,
         "Returns true if the monster has any status problem that prevents it from"
         " acting\n\nr0: Entity pointer\nreturn: True if the specified monster can't act"
         " because of a status problem, false otherwise.",
@@ -15870,14 +15968,37 @@
         "Removes the target's reflect, safeguard, light screen, counter, magic coat,"
         " wish, protect, mirror coat, endure, mini counter?, mirror move, conversion 2,"
         " vital throw, mist, metal burst, aqua ring or lucky chant status due to the"
         " action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    TryRemoveSnatchedMonsterFromDungeonStruct = Symbol(
+        None,
+        None,
+        None,
+        "If the target is afflicted with snatch, change dungeon::snatch_monster and"
+        " dungeon::snatch_status_unique_id back\nto NULL and 0 respectively. This"
+        " function does not actually remove the status and visual flags for snatch"
+        " from\nthe monster, it simply removes it from the dungeon struct. After"
+        " calling, the user should ensure the monster\ndoes not still have the snatch"
+        " status.\n\nr0: pointer to user\nr1: pointer to target",
+    )
+
+    EndCurseClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's curse (1), decoy (2), snatch (3), gastro acid (4), heal"
+        " block (5), or embargo (6) status\ndue to the action of the user, and prints"
+        " the event to the log.\n\nr0: pointer to user\nr1: pointer to target\nr2:"
+        " curse class status being afflicted after (0 is the status is only being"
+        " removed)\nr3: flag to log a message",
+    )
+
     EndLeechSeedClassStatus = Symbol(
         None,
         None,
         None,
         "Cures the target's leech seed or destiny bond status due to the action of the"
         " user, and prints the event to the log.\n\nr0: pointer to user\nr1: pointer to"
         " target",
@@ -15888,14 +16009,33 @@
         None,
         None,
         "Removes the target's sure shot, whiffer, set damage or focus energy status due"
         " to the action of the user, and prints the event to the log.\n\nr0: pointer to"
         " user\nr1: pointer to target",
     )
 
+    EndInvisibleClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's invisible, transformed, mobile, or slip status due to the"
+        " action of the user, and prints\nthe event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target\nr2: flag to not log a message when removing slip"
+        " status",
+    )
+
+    EndBlinkerClassStatus = Symbol(
+        None,
+        None,
+        None,
+        "Removes the target's blinker, cross-eyed, eyedrops, or dropeye status due to"
+        " the action of the user, and\nprints the event to the log.\n\nr0: pointer to"
+        " user\nr1: pointer to target",
+    )
+
     EndMuzzledStatus = Symbol(
         None,
         None,
         None,
         "Removes the target's muzzled status due to the action of the user, and prints"
         " the event to the log.\n\nr0: pointer to user\nr1: pointer to target",
     )
@@ -15921,14 +16061,39 @@
         None,
         None,
         "Tries to transfer the the negative blinker class status conditions from the"
         " user to\nthe target.\n\nr0: user entity pointer\nr1: target entity"
         " pointer\nreturn: Whether or not the status could be transferred",
     )
 
+    EndFrozenStatus = Symbol(
+        None,
+        None,
+        None,
+        "Cures the target's freeze status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    EndProtectStatus = Symbol(
+        None,
+        None,
+        None,
+        "Ends the target's protect status due to the action of the user.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
+    TryRestoreRoostTyping = Symbol(
+        None,
+        None,
+        None,
+        "Tries to restore the target's original typings before the Roost effect took"
+        " place. Does nothing if the target\nis not affected by Roost.\n\nr0: user"
+        " entity pointer\nr1: target entity pointer",
+    )
+
     TryTriggerMonsterHouse = Symbol(
         None,
         None,
         None,
         "Triggers a Monster House for an entity, if the right conditions are"
         " met.\n\nConditions: entity is valid and on the team, the tile is a Monster"
         " House tile, and the Monster House hasn't already been triggered.\n\nThis"
@@ -16090,14 +16255,23 @@
         " 8 fraction bits)\nstack[3]: move ID\nstack[4]: flag to account for certain"
         " effects (Flash Fire, Reflect, Light Screen, aura bows, Def. Scarf, Zinc"
         " Band). Only ever set to false when computing recoil damage for Jump Kick/Hi"
         " Jump Kick missing, which is based on the damage that would have been done if"
         " the move didn't miss.",
     )
 
+    ApplyDamageAndEffectsWrapper = Symbol(
+        None,
+        None,
+        None,
+        "A wrapper for ApplyDamageAndEffects used for applying damage from sources such"
+        " as statuses, traps, liquid ooze,\nhunger, and possibly more.\n\nr0: monster"
+        " entity pointer\nr1: damage amount\nr2: damage message\nr3: damage source",
+    )
+
     CalcRecoilDamageFixed = Symbol(
         None,
         None,
         None,
         "Appears to calculate recoil damage to a monster.\n\nThis function wraps"
         " CalcDamageFixed using the monster as both the attacker and the defender,"
         " after doing some basic checks (like if the monster is already at 0 HP) and"
@@ -16148,14 +16322,25 @@
         "Updates the shopkeeper mode of a monster in response to being struck by an"
         " attack.\n\nIf the defender is in normal shopkeeper mode (not aggressive),"
         " nothing happens. Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if"
         " the attacker is a team member, or SHOPKEEPER_MODE_ATTACK_ENEMIES"
         " otherwise.\n\nr0: attacker pointer\nr1: defender pointer",
     )
 
+    UpdateShopkeeperModeAfterTrap = Symbol(
+        None,
+        None,
+        None,
+        "Updates the shopkeeper mode of a monster in response to stepping on a"
+        " trap.\n\nIf in the normal shopkeeper mode (not aggressive), nothing happens."
+        " Otherwise, the mode is set to SHOPKEEPER_MODE_ATTACK_TEAM if the trap is from"
+        " a team member or SHOPKEEPER_MODE_ATTACK_ENEMIES otherwise.\n\nr0: shopkeeper"
+        " pointer\nr1: bool non team member trap",
+    )
+
     ResetDamageCalcDiagnostics = Symbol(
         None,
         None,
         None,
         "Resets the damage calculation diagnostic info stored on the dungeon struct."
         " Called unconditionally at the start of CalcDamage.\n\nNo params.",
     )
@@ -16231,14 +16416,24 @@
         None,
         None,
         "Gets the exclusive item boost for defense/special defense for a monster\n\nr0:"
         " entity pointer\nr1: move category index (0 for physical, 1 for"
         " special)\nreturn: boost",
     )
 
+    TeamMemberHasItemActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if any team member is holding a certain item and puts them into the"
+        " array given.\n\nr0: [output] pointer to array of monsters (expected to have"
+        " space for at least 4 pointers)\nr1: item ID\nreturn: number of team members"
+        " with the item active",
+    )
+
     TeamMemberHasExclusiveItemEffectActive = Symbol(
         None,
         None,
         None,
         "Checks if any team member is under the effects of a certain exclusive item"
         " effect.\n\nr0: exclusive item effect ID\nreturn: bool",
     )
@@ -16414,15 +16609,16 @@
 
     TryInflictShadowHoldStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Shadow Hold (AKA Immobilized) status condition on a target"
         " monster if possible.\n\nr0: user entity pointer\nr1: target entity"
-        " pointer\nr2: flag to log a message on failure",
+        " pointer\nr2: flag to only perform the check for inflicting without actually"
+        " inflicting",
     )
 
     TryInflictIngrainStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Ingrain status condition on a target monster if possible.\n\nr0:"
@@ -16456,24 +16652,28 @@
 
     LowerOffensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified offensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     LowerDefensiveStat = Symbol(
         None,
         None,
         None,
         "Lowers the specified defensive stat on the target monster.\n\nr0: user entity"
         " pointer\nr1: target entity pointer\nr2: stat index\nr3: number of"
-        " stages\nstack[0]: ?\nstack[1]: ?",
+        " stages\nstack[0]: flag to check for being protected from stat"
+        " drops\nstack[1]: flag to log a message on failure for"
+        " IsProtectedFromStatDrops",
     )
 
     BoostOffensiveStat = Symbol(
         None,
         None,
         None,
         "Boosts the specified offensive stat on the target monster.\n\nr0: user entity"
@@ -16496,14 +16696,23 @@
         " by a Fire-type move.\n\nThis checks that the defender is valid and Flash Fire"
         " is active, and that Normalize isn't active on the attacker.\n\nr0: attacker"
         " pointer\nr1: defender pointer\nreturn: 2 if Flash Fire should activate and"
         " raise the defender's boost level, 1 if Flash Fire should activate but the"
         " defender's boost level is maxed out, 0 otherwise.",
     )
 
+    ActivateFlashFire = Symbol(
+        None,
+        None,
+        None,
+        "Actually applies the Flash Fire boost with a message log and animation. Passes"
+        " the same monster for attacker and\ndefender, but the attacker goes"
+        " unused.\n\nr0: attacker pointer?\nr1: defender pointer",
+    )
+
     ApplyOffensiveStatMultiplier = Symbol(
         None,
         None,
         None,
         "Applies a multiplier to the specified offensive stat on the target"
         " monster.\n\nThis affects struct"
         " monster_stat_modifiers::offensive_multipliers, for moves like Charm and"
@@ -16632,14 +16841,31 @@
         None,
         None,
         "Activate the Quick Feet ability on the defender, if the monster has it and"
         " it's active.\n\nr0: attacker pointer\nr1: defender pointer\nreturn: bool,"
         " whether or not the ability was activated",
     )
 
+    TryInflictTerrifiedStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Terrified status condition on a target monster if"
+        " possible.\n\nr0: user entity pointer\nr1: target entity pointer",
+    )
+
+    TryInflictGrudgeStatus = Symbol(
+        None,
+        None,
+        None,
+        "Inflicts the Grudge status condition on a target monster if possible.\n\nr0:"
+        " user entity pointer\nr1: target entity pointer\nr2: flag to log a"
+        " message\nreturn: Whether or not the status could be inflicted",
+    )
+
     TryInflictConfusedStatus = Symbol(
         None,
         None,
         None,
         "Inflicts the Confused status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nr2: flag to log a message on"
         " failure\nr3: flag to only perform the check for inflicting without actually"
@@ -16944,23 +17170,41 @@
         None,
         None,
         "Inflicts the Dropeye status condition on a target monster if possible.\n\nr0:"
         " user entity pointer\nr1: target entity pointer\nreturn: Whether or not the"
         " status could be inflicted",
     )
 
-    RestoreMovePP = Symbol(
+    RestoreAllMovePP = Symbol(
         None,
         None,
         None,
         "Restores the PP of all the target's moves by the specified amount.\n\nr0: user"
         " entity pointer\nr1: target entity pointer\nr2: PP to restore\nr3: flag to"
         " suppress message logging",
     )
 
+    RestoreOneMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP the target's move in the specified move slot by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: move"
+        " index\nr3: PP to restore\nstack[0]: flag to suppress message logging",
+    )
+
+    RestoreRandomMovePP = Symbol(
+        None,
+        None,
+        None,
+        "Restores the PP of a random one of the target's moves by the specified"
+        " amount.\n\nr0: user entity pointer\nr1: target entity pointer\nr2: PP to"
+        " restore\nr3: flag to suppress message logging",
+    )
+
     ApplyProteinEffect = Symbol(
         None,
         None,
         None,
         "Tries to boost the target's attack stat.\n\nr0: user entity pointer\nr1:"
         " target entity pointer\nr2: attack boost",
     )
@@ -17218,14 +17462,23 @@
         None,
         None,
         "Checks if the monster is under the effect of Mirror Move.\n\nReturns 1 if the"
         " effects is a status, 2 if it comes from an exclusive item, 0"
         " otherwise.\n\nr0: pointer to entity\nreturn: int",
     )
 
+    MistIsActive = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the monster is under the effect of Mist.\n\nReturns 1 if the effects"
+        " is a status, 2 if it comes from an exclusive item, 0 otherwise.\n\nr0:"
+        " pointer to entity\nreturn: int",
+    )
+
     Conversion2IsActive = Symbol(
         None,
         None,
         None,
         "Checks if the monster is under the effect of Conversion 2 (its type was"
         " changed).\n\nReturns 1 if the effects is a status, 2 if it comes from an"
         " exclusive item, 0 otherwise.\n\nr0: pointer to entity\nreturn: int",
@@ -17320,14 +17573,54 @@
         None,
         None,
         None,
         "Gets the current Weather Ball type for the given entity, based on the apparent"
         " weather.\n\nr0: entity pointer\nreturn: type ID",
     )
 
+    ActivateMotorDrive = Symbol(
+        None,
+        None,
+        None,
+        "Displays the message and applies the speed boost for the ability Motor"
+        " Drive.\n\nr0: monster pointer",
+    )
+
+    TryActivateFrisk = Symbol(
+        None,
+        None,
+        None,
+        "Tries to activate the Frisk ability on the defender. The attacker has to be on"
+        " the team and the defender has to be\nholding an item or be able to drop a"
+        " treasure box.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
+    TryActivateBadDreams = Symbol(
+        None,
+        None,
+        None,
+        "Tries to apply the damage from Bad Dreams to all sleeping monsters in the"
+        " room.\n\nr0: monster pointer",
+    )
+
+    ActivateStench = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Stench ability on the monster.\n\nr0: monster pointer",
+    )
+
+    TryActivateSteadfast = Symbol(
+        None,
+        None,
+        None,
+        "Activate the Steadfast ability on the defender, if the monster has it and it's"
+        " active.\n\nr0: attacker pointer\nr1: defender pointer",
+    )
+
     IsInSpawnList = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: spawn_list_ptr\nr1:"
         " monster ID\nreturn: bool",
     )
@@ -17905,17 +18198,16 @@
 
     TryActivateWeather = Symbol(
         None,
         None,
         None,
         "Tries to change the weather based upon the information for each weather type"
         " in the\ndungeon struct. Returns whether the weather was succesfully changed"
-        " or not.\n\nr0: bool to not play the weather change animation?\nr1: bool to"
-        " force weather change? Like play the animation and text for the"
-        " weather?\nreturn: True if the weather changed",
+        " or not.\n\nr0: bool to log message and play animation?\nr1: bool to force"
+        " weather change and animation?\nreturn: True if the weather changed",
     )
 
     DigitCount = Symbol(
         None,
         None,
         None,
         "Counts the number of digits in a nonnegative integer.\n\nIf the number is"
@@ -17969,21 +18261,77 @@
         None,
         None,
         "Checks if the current fixed room on the dungeon generation info corresponds to"
         " a fixed, full-floor layout.\n\nThe first non-full-floor fixed room is 0xA5,"
         " which is for Sealed Chambers.\n\nreturn: bool",
     )
 
+    TrySpawnGoldenChamber = Symbol(
+        None,
+        None,
+        None,
+        "Changes the tileset and fixed room id of the floor for the Golden Chamber if"
+        " the floor should be a\nGolden Chamber.\n\nNo params.",
+    )
+
+    CountItemsOnFloorForAcuteSniffer = Symbol(
+        None,
+        None,
+        None,
+        "Counts the number of items on the floor by checking every tile for an item and"
+        " stores it into\ndungeon::item_sniffer_item_count\n\nNo params.",
+    )
+
+    GetStairsSpawnPosition = Symbol(
+        None,
+        None,
+        None,
+        "Gets the spawn position for the stairs and stores it at the passed"
+        " pointers.\n\nr0: [output] pointer to x coordinate\nr1: [output] pointer to y"
+        " coordinate",
+    )
+
+    PositionIsOnStairs = Symbol(
+        None,
+        None,
+        None,
+        "Checks if this location is on top of the staircase. In the game it is only"
+        " used to check if an outlaw has reached\nthe staircase.\n\nr0: x"
+        " coordinate\nr1: y coordinate\nreturn: bool",
+    )
+
     GetStairsRoom = Symbol(
         None,
         None,
         None,
         "Returns the index of the room that contains the stairs\n\nreturn: Room index",
     )
 
+    GetDefaultTileTextureId = Symbol(
+        None,
+        None,
+        None,
+        "Returns the texture_id of the default tile?\n\nreturn: texture_id",
+    )
+
+    DetermineAllTilesWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for all tiles.\n\nNo params.",
+    )
+
+    DetermineTileWalkableNeighbors = Symbol(
+        None,
+        None,
+        None,
+        "Evaluates the walkable_neighbor_flags for the this tile by checking the 8"
+        " adjacent tiles.\n\nr0: x coordinate\nr1: y coordinate",
+    )
+
     UpdateTrapsVisibility = Symbol(
         None,
         None,
         None,
         "Exact purpose unknown. Gets called whenever a trap tile is shown or"
         " hidden.\n\nNo params.",
     )
@@ -18011,14 +18359,38 @@
         None,
         "Discovers the tiles around the specified position on the minimap.\n\nThe"
         " discovery radius depends on the visibility range of the floor. If"
         " display_data::blinded is true, the function returns early without doing"
         " anything.\n\nr0: Position around which the map should be discovered",
     )
 
+    PositionHasItem = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has an item on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    PositionHasMonster = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position has a monster on it.\n\nr0: Position to"
+        " check\nreturn: bool",
+    )
+
+    TrySmashWall = Symbol(
+        None,
+        None,
+        None,
+        "Checks if the tile at the position is a wall. If so, smash it (turn it into a"
+        " floor tile), play an animation\n\nr0: Wall position to smash\nreturn: bool",
+    )
+
     IsWaterTileset = Symbol(
         None,
         None,
         None,
         "Returns flag tileset_property::is_water_tileset for the current"
         " tileset\n\nreturn: True if the current tileset is a water tileset",
     )
@@ -19131,14 +19503,23 @@
         None,
         "Checks whether any of the items in the bag or any of the items carried by team"
         " members has any of the specified flags set in its flags field.\n\nr0: Flag(s)"
         " to check (0 = f_exists, 1 = f_in_shop, 2 = f_unpaid, etc.)\nreturn: True if"
         " any of the items of the team has the specified flags set, false otherwise.",
     )
 
+    AddHeldItemToBag = Symbol(
+        None,
+        None,
+        None,
+        "Adds the monster's held item to the bag. This is only called on monsters on"
+        " the exploration team.\nmonster::is_not_team_member should be checked to be"
+        " false before calling.\n\nr0: monster pointer",
+    )
+
     GenerateItem = Symbol(
         None,
         None,
         None,
         "Initializes an item struct with the given information.\n\nThis wraps InitItem,"
         " but with extra logic to resolve the item's stickiness. It also calls"
         " GenerateMoneyQuantity for Poké.\n\nr0: pointer to item to initialize\nr1:"
```

## pmdsky_debug_py/protocol.py

```diff
@@ -602,19 +602,49 @@
     ]
 
     IsAuraBow: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsLosableItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsTreasureBox: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    IsStorableItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsShoppableItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsValidTargetItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsItemUsableNow: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    IsTicketItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     InitItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     InitStandardItem: Symbol[
         Optional[List[int]],
@@ -10215,14 +10245,19 @@
     ]
 
     ApplyTripTrapEffect: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ApplyStealthRockTrapEffect: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ApplyToxicSpikesTrapEffect: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ApplyRandomTrapEffect: Symbol[
         Optional[List[int]],
@@ -10240,19 +10275,29 @@
     ]
 
     RevealTrapsNearby: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ShouldRunMonsterAi: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DebugRecruitingEnabled: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateIqBooster: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsSecretBazaarNpcBehavior: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetLeaderAction: Symbol[
         Optional[List[int]],
@@ -10570,14 +10615,19 @@
     ]
 
     ExecuteMonsterAction: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryActivateFlashFireOnAllMonsters: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     HasStatusThatPreventsActing: Symbol[
         Optional[List[int]],
         None,
     ]
 
     IsInvalidSpawnTile: Symbol[
         Optional[List[int]],
@@ -10885,24 +10935,44 @@
     ]
 
     EndReflectClassStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryRemoveSnatchedMonsterFromDungeonStruct: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EndCurseClassStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     EndLeechSeedClassStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     EndSureShotClassStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    EndInvisibleClassStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EndBlinkerClassStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     EndMuzzledStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     EndMiracleEyeStatus: Symbol[
         Optional[List[int]],
@@ -10915,14 +10985,29 @@
     ]
 
     TransferNegativeBlinkerClassStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    EndFrozenStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    EndProtectStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryRestoreRoostTyping: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryTriggerMonsterHouse: Symbol[
         Optional[List[int]],
         None,
     ]
 
     RunMonsterAi: Symbol[
         Optional[List[int]],
@@ -10975,14 +11060,19 @@
     ]
 
     CalcDamage: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ApplyDamageAndEffectsWrapper: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     CalcRecoilDamageFixed: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CalcDamageFixed: Symbol[
         Optional[List[int]],
@@ -11000,14 +11090,19 @@
     ]
 
     UpdateShopkeeperModeAfterAttack: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    UpdateShopkeeperModeAfterTrap: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ResetDamageCalcDiagnostics: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SpecificRecruitCheck: Symbol[
         Optional[List[int]],
@@ -11045,14 +11140,19 @@
     ]
 
     ExclusiveItemDefenseBoost: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TeamMemberHasItemActive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TeamMemberHasExclusiveItemEffectActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TrySpawnEnemyItemDrop: Symbol[
         Optional[List[int]],
@@ -11190,14 +11290,19 @@
     ]
 
     FlashFireShouldActivate: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ActivateFlashFire: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ApplyOffensiveStatMultiplier: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ApplyDefensiveStatMultiplier: Symbol[
         Optional[List[int]],
@@ -11260,14 +11365,24 @@
     ]
 
     TryActivateQuickFeet: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TryInflictTerrifiedStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryInflictGrudgeStatus: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     TryInflictConfusedStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryInflictCoweringStatus: Symbol[
         Optional[List[int]],
@@ -11430,15 +11545,25 @@
     ]
 
     TryInflictDropeyeStatus: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    RestoreMovePP: Symbol[
+    RestoreAllMovePP: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    RestoreOneMovePP: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    RestoreRandomMovePP: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ApplyProteinEffect: Symbol[
         Optional[List[int]],
         None,
@@ -11595,14 +11720,19 @@
     ]
 
     MirrorMoveIsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    MistIsActive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     Conversion2IsActive: Symbol[
         Optional[List[int]],
         None,
     ]
 
     AiConsiderMove: Symbol[
         Optional[List[int]],
@@ -11640,14 +11770,39 @@
     ]
 
     GetEntityWeatherBallType: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    ActivateMotorDrive: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryActivateFrisk: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryActivateBadDreams: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ActivateStench: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TryActivateSteadfast: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsInSpawnList: Symbol[
         Optional[List[int]],
         None,
     ]
 
     ChangeShayminForme: Symbol[
         Optional[List[int]],
@@ -11980,19 +12135,54 @@
     ]
 
     IsFullFloorFixedRoom: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    TrySpawnGoldenChamber: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    CountItemsOnFloorForAcuteSniffer: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetStairsSpawnPosition: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    PositionIsOnStairs: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GetStairsRoom: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    GetDefaultTileTextureId: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    DetermineAllTilesWalkableNeighbors: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    DetermineTileWalkableNeighbors: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     UpdateTrapsVisibility: Symbol[
         Optional[List[int]],
         None,
     ]
 
     DrawTileGrid: Symbol[
         Optional[List[int]],
@@ -12005,14 +12195,29 @@
     ]
 
     DiscoverMinimap: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    PositionHasItem: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    PositionHasMonster: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    TrySmashWall: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     IsWaterTileset: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetRandomSpawnMonsterID: Symbol[
         Optional[List[int]],
@@ -12575,14 +12780,19 @@
     ]
 
     CheckTeamItemsFlags: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    AddHeldItemToBag: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     GenerateItem: Symbol[
         Optional[List[int]],
         None,
     ]
 
     CheckActiveChallengeRequest: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-7.0.3.dist-info/METADATA` & `pmdsky_debug_py-7.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.3
+Version: 7.0.4
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

