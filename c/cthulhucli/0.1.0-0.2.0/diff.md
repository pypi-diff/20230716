# Comparing `tmp/cthulhucli-0.1.0-py3-none-any.whl.zip` & `tmp/cthulhucli-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 186401 bytes, number of entries: 10
+Zip file size: 186399 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 12:50 cthulhucli/__init__.py
--rw-r--r--  2.0 unx   674943 b- defN 23-Jul-15 11:54 cthulhucli/coc-ccg.data
+-rw-r--r--  2.0 unx   674899 b- defN 23-Jul-15 15:25 cthulhucli/coc-ccg.data
 -rw-r--r--  2.0 unx   963049 b- defN 23-Jul-15 14:26 cthulhucli/coc-lcg.data
--rw-r--r--  2.0 unx    29524 b- defN 23-Jul-15 14:31 cthulhucli/cthulhucli.py
--rw-r--r--  2.0 unx       28 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      419 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jul-15 14:40 cthulhucli-0.1.0.dist-info/RECORD
-10 files, 1668947 bytes uncompressed, 184993 bytes compressed:  88.9%
+-rw-r--r--  2.0 unx    29614 b- defN 23-Jul-16 16:42 cthulhucli/cthulhucli.py
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      419 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-16 16:42 cthulhucli-0.2.0.dist-info/RECORD
+10 files, 1668993 bytes uncompressed, 184991 bytes compressed:  88.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: cthulhucli/coc-lcg.data
 Comment: 
 
 Filename: cthulhucli/cthulhucli.py
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/LICENSE.txt
+Filename: cthulhucli-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/METADATA
+Filename: cthulhucli-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/WHEEL
+Filename: cthulhucli-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/entry_points.txt
+Filename: cthulhucli-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/top_level.txt
+Filename: cthulhucli-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cthulhucli-0.1.0.dist-info/RECORD
+Filename: cthulhucli-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cthulhucli/coc-ccg.data

```diff
@@ -336,15 +336,15 @@
 {"name": "Street Preacher", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Investigator.", "text": "Forced Response: after Street Preacher enters play, choose and exhaust a support card, if able.", "cost": 2, "skill": 2, "terror": 0, "combat": 0, "arcane": 0, "investigation": 2, "transient": false, "steadfast": [["Syndicate", 2]], "era": "CCG", "id": null, "set": "MN", "setname": "Masks of Nyarlathotep", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Syndicate Agent", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Government.", "text": "Disrupt: pay 3 to cancel 1 wound to Syndicate Agent. Then choose and wound a character.", "cost": 4, "skill": 3, "terror": 0, "combat": 2, "arcane": 0, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Syndicate Liaison", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Criminal.", "text": "Forced Response: after Syndicate Liaison enters play, choose and exhaust a ready character, if able.", "cost": 3, "skill": 3, "terror": 0, "combat": 0, "arcane": 2, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "UT", "setname": "Unspeakable Tales", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Syndicate Troubleshooter", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Sorceror.", "text": "Response: after Syndicate Troubleshooter is placed in your discard pile from play, attach it to one of your Domains as a resource.", "cost": 3, "skill": 2, "terror": 0, "combat": 0, "arcane": 2, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Tragic Celebrity", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Criminal. Conspirator.", "text": "While there is at least one Conspiracy card in play, you draw an additional card during your draw phase.", "cost": 2, "skill": 1, "terror": 0, "combat": 0, "arcane": 0, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "CC3", "setname": "Conspiracies of Chaos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Triggerman", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Criminal.", "text": "Loyal. Willpower.", "cost": 2, "skill": 2, "terror": 0, "combat": 1, "arcane": 0, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "FR", "setname": "Forbidden Relics", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Voice on the Phone The New Boss", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": true, "subtypes": "Avatar of Nyarlathotep.", "text": "Response: after you play a Ritual event, choose a character. Until the end of the phase, that character loses an icon of your choice.", "cost": 4, "skill": 3, "terror": 1, "combat": 1, "arcane": 1, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
-{"name": "William Bain, \"The One\"", "descriptor": null, "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Investigator.", "text": "Response: after a character or support card controlled by an opponent is exhausted, pay 1 to look at the top 2 cards of your deck. Put one or both on the bottom of your deck, and the rest back on top of your deck. ", "cost": 3, "skill": 3, "terror": 0, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "KD2", "setname": "Kingsport Dreams", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
+{"name": "William Bain", "descriptor": "\"The One\"", "type": "Character", "faction": "Syndicate", "unique": false, "subtypes": "Investigator.", "text": "Response: after a character or support card controlled by an opponent is exhausted, pay 1 to look at the top 2 cards of your deck. Put one or both on the bottom of your deck, and the rest back on top of your deck. ", "cost": 3, "skill": 3, "terror": 0, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "KD2", "setname": "Kingsport Dreams", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Underground Conspiracy", "descriptor": null, "type": "Conspiracy", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "If you win this story and control at least 1 [Syndicate] character, you may force each opponent to discard his hand.", "cost": 0, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "CC3", "setname": "Conspiracies of Chaos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Abduction", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "Action: choose an exhausted character without any (A) icons. Put that character on top of its owner's deck.\nThen, refresh the domain that was drained to play Abduction.", "cost": 4, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Adoration of Maahes", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "Ritual.", "text": "Action: ready all exhausted Criminal characters.\nThen, if you have played at least 1 other Ritual event this phase, return Adoration of Maahes to your hand instead of discarding it.", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "MN", "setname": "Masks of Nyarlathotep", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Auto-de-fe", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "Action: choose Day or Night.\nThen, put into play all characters and support cards with the printed subtype you chose from all discard piles.", "cost": 3, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Behind Closed Doors", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "Action: shuffle your hand into your deck. Then draw that many cards plus one.", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Best Bias Money Can Buy", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "Lower the cost to play The Best Bias Money Can Buy by 1 (to a minimum of 1) for each Artifact you control.\nResponse: after you succeed at a story, place 2 success tokens on that story.", "cost": 4, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "FR", "setname": "Forbidden Relics", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Blowing the Whistle", "descriptor": null, "type": "Event", "faction": "Syndicate", "unique": false, "subtypes": "", "text": "Action: choose and exhaust up to 3 non-Ancient One characters", "cost": 4, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
@@ -1081,15 +1081,15 @@
 {"name": "Signing the Book", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "Ritual.", "text": "Response: after any player plays a Ritual event, put the top card of your discard pile on the bottom of your deck.\nThen, you may drain a domain you control to return Signing the Book to your hand instead of discarding it.", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Simple Kindness", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Response: after a player plays a Ritual event, refresh all of your domains.", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "MN", "setname": "Masks of Nyarlathotep", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Stars Are Right", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Action: lower the cost for you to play Ancient One characters this phase by 2 (to a minimum of 1).", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Startling Discovery", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Response: after you succeed at a story, put 1 success token on that story card for each icon struggle you won.", "cost": 3, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Strange Aeons", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "Disaster.", "text": "Action: destroy all characters without at least 1 card attached to them.", "cost": 6, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "MN", "setname": "Masks of Nyarlathotep", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Strange Inheritance", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Play during your resource phase.\nAction: choose one of your Domains with 3 or more resources attached. Then, attach Strange Inheritance to that Domain as a resource.", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "UT", "setname": "Unspeakable Tales", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Swarm of Cobras", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Play during your operations phase.\nAction: Each player sacrifices all characters with at least one Curse attached.", "cost": 3, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
-{"name": "\uf020\uf076 Tentacular Spectacular!", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Response: after a card enters play with at least one tentacle in its art, say \"Tentacular Spectacular!\" Then, put 2 success tokens on that story. ", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
+{"name": "Tentacular Spectacular!", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Response: after a card enters play with at least one tentacle in its art, say \"Tentacular Spectacular!\" Then, put 2 success tokens on that story. ", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": true, "restricted": false}
 {"name": "To the Last Breath", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Play only if it is Day.\nAction: choose a Heroic character. Until the end of the phase, that character gets +3 skill and gains Willpower and (C)(C)(A)(A)(I)(I).", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Unhealthy Curiosity", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Action: choose a story. Until the end of the phase, that story gains a struggle icon of your choice.", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Worlds Torn Asunder", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "Disaster.", "text": "Play only if you control at least two of the following characters: Cthulhu, Yog-Sothoth, Hastur or Shub-Niggurath.\nAction: choose a story. Place 5 success tokens on that story card.", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "FR", "setname": "Forbidden Relics", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Written in the Sky", "descriptor": null, "type": "Event", "faction": "Neutral", "unique": false, "subtypes": "", "text": "Response: after you play an Ancient One character, search your deck for a different Ancient One character, reveal it, and put it into your hand.\nThen shuffle your deck.", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "SM1", "setname": "Spawn of Madness", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": ".45 Pistols", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment. Item.", "text": "Attach to a character. Attached character gains a (C) icon.", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "607 Water Street", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": true, "subtypes": "Location.", "text": "Response: after a card with the word Brotherhood in its title enters a discard pile from play, exhaust to return that character to play under its owner's control. ", "cost": 2, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "KD2", "setname": "Kingsport Dreams", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "A Higher Purpose", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment.", "text": "Attach to a character. Attached character gets +3 skill.", "cost": 0, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "UT", "setname": "Unspeakable Tales", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
@@ -1179,23 +1179,23 @@
 {"name": "Windy Gallows Hex", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment. Curse.", "text": "Attached character gains (I)(I) and Heroic.\nAt any time there are 3 or more Curse cards in play, attached character's controller must sacrifice it.", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "FC", "setname": "Forgotten Cities", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Wrapped in Flesh", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment. Curse.", "text": "Attach to a character. Attached character loses all of its printed (T) icons.", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": true, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Yithian Rifle", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment. Weapon.", "text": "Attach to a character. Attached character gains (C).\nResponse: after you win an icon struggle by at least 2 icons, choose and destroy a Weapon card.", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": true, "steadfast": null, "era": "CCG", "id": null, "set": "MN", "setname": "Masks of Nyarlathotep", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Zanthu Tablet", "descriptor": null, "type": "Support", "faction": "Neutral", "unique": false, "subtypes": "Attachment. Item.", "text": "Attach to a character you control. Attached character gains (A)(A).\nResponse: after Zanthu Tablet is placed into any discard pile from play, pay 1 to return it to its owner's hand.", "cost": 1, "skill": null, "terror": 0, "combat": 0, "arcane": 0, "investigation": 0, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "FR", "setname": "Forbidden Relics", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Abysses of Night", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player choose one resource attached to each of his domains. All resources not chosen are sacrificed.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Arkham Willows", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player discards the top 10 cards of his deck.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Beyond the Doors of Sleep", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player that controls no Day or Night cards discards all of his success tokens from all story cards.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
-{"name": "\uf076\uf020The Challenge from Beyond", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Players cannot win this story card.\nForced Response: after a player places one or more success tokens on this story, he draws 2 cards.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
+{"name": "The Challenge from Beyond", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Players cannot win this story card.\nForced Response: after a player places one or more success tokens on this story, he draws 2 cards.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": true, "restricted": false}
 {"name": "The Crooked Manse", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player gains a new Domain with the top 4 cards of his deck attached to it as resources.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Dark Heart of Cairo", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player chooses up to 2 Support cards controlled by the opponent to his left. All chosen Support cards are destroyed.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Digging Deep", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player searches his deck for up to 3 Attachment cards, reveals them to all opponents, and puts them into his hand. Then, each player shuffles his deck.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Dreams of Kingsport", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "After you win this story, choose Day or Night. Each player searches his deck for a card with that subtype, puts that card into play, then shuffles his deck.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Forgotten Sepulchre", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player searches his deck for one character card and one non-Day or non-Night support card and puts them into play. Then each player shuffles his deck.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Horror of the Past", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player shuffles his discard pile into his deck.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Innsmouth Threat", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Discard all success tokens on all story cards.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
-{"name": "\uf076\uf020The Nameless City", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Players need 10 success tokens in order to win this story.\nIf you win this story, you win the game.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
+{"name": "The Nameless City", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Players need 10 success tokens in order to win this story.\nIf you win this story, you win the game.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "PR", "setname": "Promos", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": true, "restricted": false}
 {"name": "Parable of the Faceless One", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player must choose and shuffle one of his won story cards into the Story deck (except Parable of the Faceless One)", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Secret of the North Woods", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Put into play all characters from all discard piles.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Shadows of Nephren-Ka", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player discards his hand.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Squalid Hamlet", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player chooses one of his domains, then attaches the top 5 cards of his discard pile to that domain as resources, if able.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Terror Out of Dunwich", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player chooses one resource attached to each of his Domains. All other resources are destroyed.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "The Thing at the Gate", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player sacrifices all of his characters.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "AE", "setname": "Arkham Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
 {"name": "Throne of the Black Pharaoh", "descriptor": null, "type": "Story", "faction": null, "unique": false, "subtypes": "", "text": "Each player draws 10 cards.", "cost": null, "skill": null, "terror": 1, "combat": 1, "arcane": 1, "investigation": 1, "transient": false, "steadfast": null, "era": "CCG", "id": null, "set": "EE", "setname": "Eldritch Edition", "setid": null, "flavor": null, "illustrator": null, "max": 4, "banned": false, "restricted": false}
```

## cthulhucli/cthulhucli.py

```diff
@@ -20,15 +20,15 @@
     option,
     pass_context,
     secho,
     style,
 )
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 CARD_TYPES = ["Character", "Conspiracy", "Event", "Story", "Support"]
 CARD_TYPES_UNIQUE = ["Character", "Support"]
 FACTIONS = {
     "The Agency": {"alias": ["Agency"]},
     "Cthulhu": {},
@@ -44,14 +44,15 @@
     alias: faction
     for faction, data in FACTIONS.items()
     for alias in [faction] + data.get("alias", [])
 }
 KEYWORDS = [
     "Dormant",
     "Fast",
+    "Fated",
     "Heroic",
     "Invulnerability",
     "Loyal",
     "Resilient",
     "Steadfast",
     "Toughness",
     "Transient",
@@ -747,18 +748,20 @@
 
 def sortkey(*sortfields):
     def _sortkey(card):
         sortkey = []
         for field in sortfields:
             if field == "subtypes":
                 sortkey.append(len(card["subtypes"].split(".")))
-            elif field in card:
-                sortkey.append(-1 if card[field] == "X" else card[field])
-            else:
+            elif field not in card:
                 sortkey.append(format_card_field(card, field, color=False))
+            elif card[field] is None:
+                sortkey.append(-2)
+            else:
+                sortkey.append(-1 if card[field] == "X" else card[field])
         return sortkey
 
     return _sortkey
 
 
 def sort_cards(cards, options):
     if options["sort"] or options["group"]:
```

