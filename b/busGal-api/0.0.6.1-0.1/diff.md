# Comparing `tmp/busGal_api-0.0.6.1.tar.gz` & `tmp/busGal_api-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busGal_api-0.0.6.1.tar", last modified: Mon Nov 14 14:33:05 2022, max compression
+gzip compressed data, was "busGal_api-0.1.tar", last modified: Sun Jul 16 21:42:53 2023, max compression
```

## Comparing `busGal_api-0.0.6.1.tar` & `busGal_api-0.1.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35150 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/busGal_api/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/busGal_api/accounts/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10196 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/accounts/http_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/busGal_api/buses/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/buses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/buses/equivalent_stops.py
--rw-r--r--   0 runner    (1001) docker     (121)     9526 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/buses/http_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/busGal_api/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/busGal_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-11-14 14:33:04.000000 busGal_api-0.0.6.1/busGal_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-14 14:33:04.000000 busGal_api-0.0.6.1/busGal_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 14:33:04.000000 busGal_api-0.0.6.1/busGal_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-14 14:33:04.000000 busGal_api-0.0.6.1/busGal_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-14 14:33:04.000000 busGal_api-0.0.6.1/busGal_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 14:33:05.008417 busGal_api-0.0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-11-14 14:32:51.000000 busGal_api-0.0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:53.075267 busGal_api-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-16 21:42:40.000000 busGal_api-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-16 21:42:53.075267 busGal_api-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-16 21:42:40.000000 busGal_api-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:53.075267 busGal_api-0.1/busGal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:53.075267 busGal_api-0.1/busGal_api/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/known_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/rest_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:53.075267 busGal_api-0.1/busGal_api/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/expeditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/stops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-16 21:42:40.000000 busGal_api-0.1/busGal_api/transport/warning_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:42:53.075267 busGal_api-0.1/busGal_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-16 21:42:53.000000 busGal_api-0.1/busGal_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-16 21:42:53.000000 busGal_api-0.1/busGal_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:42:53.000000 busGal_api-0.1/busGal_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 21:42:53.000000 busGal_api-0.1/busGal_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 21:42:53.000000 busGal_api-0.1/busGal_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 21:42:53.075267 busGal_api-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-16 21:42:40.000000 busGal_api-0.1/setup.py
```

### Comparing `busGal_api-0.0.6.1/LICENSE` & `busGal_api-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `busGal_api-0.0.6.1/busGal_api/accounts/http_api.py` & `busGal_api-0.1/busGal_api/accounts/accounts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,368 +1,323 @@
-from ..requests import *
-from urllib.parse import quote_plus as urlencode
+from . import _rest_adapter
+from ..rest_adapter import RestAdapter
 
-def register_account(email, password, name, last_name, identity_type, identity_number, phone_number):
-    """
-    Register an user account
-
-    :param email: Email address
-    :type email: str
-
-    :param password: Password (Must be at least 6 character length, including a digit and an upper case letter)
-    :type email: str
-
-    :param name: First name
-    :type name: str
-
-    :param last_name: Last name
-    :type last_name: str
-
-    :param identity_type: Identity type: "DNI" or "other"
-    :type identity_type: str
-
-    :param identity_number: Identity number e.g. your DNI
-    :type identity_number: str
-
-    :param phone_number: Phone number
-    :type phone_number: str
-    """
-    if identity_type == "DNI":
-        identity_type = 1
-    elif identity_type == "other":
-        identity_type = 2
-    else:
-        raise Exception("identity_type must be 'DNI' or 'other'")
+## vvv Classes vvv ##
 
-    data = {
-        "check_data_protection": 1,
-        "email": email,
-        "password": password,
-        "name": name,
-        "last_name": last_name,
-        "identity_type": identity_type,
-        "identity_number": identity_number,
-        "phone_number": str(phone_number)
-    }
-    url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/user/register"
-    make_post_request(url, data)
 
-def recover_password(email):
+class Card():
     """
-    Recover an account's password (sends an email with a new temporal one)
-
-    :param email: Email address
-    :type email: str
+    A card
     """
-    url = f"https://tpgal-ws.xunta.gal/tpgal_ws/rest/user/password?email={urlencode(email)}"
-    make_get_request(url)
 
-class _Card():
-    """
-    Class that represents a card. If an object of this class is deleted, so will be the card, it's in the destructor (__del__)
-    """
-    def __init__(self, account, number):
+    def __init__(self, account: 'Account', number: int, is_xente_nova: bool, alias: str = None, pending: float = None, cashed: float = None, expired: float = None, summary_movements: list[dict] = None, travels: int = None) -> None:
         self.account = account
         """
         The user account the card belongs to
-
-        :type: Account
         """
 
         self.number = number
         """
         Number of the card
-
-        :type: int
         """
 
-        self.is_xente_nova = None
+        self.is_xente_nova = is_xente_nova
         """
-        Whether the card is Xente Nova or no
-
-        :type: bool
+        Whether the card is Xente Nova (type 0 in the API) or not (type 1)
         """
 
-        self.alias = None
+        self.alias = alias
         """
         The alias of the card
-
-        :type: str
         """
 
-        self.pending = None
+        self.pending = pending
         """
-        Amount of money pending of return from the Xunta (cantos cartos débeche o pirolas)
-
-        :type: float
+        Amount of money pending of return
         """
 
-        self.cashed = None
+        self.cashed = cashed
+        """
+        Amount of money cashed
         """
-        Amount of money cashed from the Xunta (cantos cartos lle roubaches ó pirolas)
 
-        :type: float
+        self.expired = expired
+        """
+        Amount of money expired because it wasn't cashed
         """
 
-        self.expired = None
+        self.summary_movements = summary_movements
+        """
+        The summary of the movemnts of the card
         """
-        Amount of money expired from the Xunta (cantos cartos quedouse o pirolas)
 
-        :type: float
+        self.travels = travels
+        """
+        Number of travels done. Given in card summary (`Account.get_cards`)
         """
-        self.refresh_data()
 
-    def refresh_data(self):
+    def refresh_data(self, months: int = 12) -> None:
         """
         Obtains the card's details and sets them to the object
+
+        :params months: How many months to get `summary_movements` for
         """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/cards/get"
-        data = {
-            "months": 12,
-            "number": self.number
-        }
-        json = self.account._make_post_request(url, data)
-        json_data = json["results"]
-
-        self.is_xente_nova = json_data["type"] == 0
-        self.alias = json_data["alias"]
-        self.pending = json_data["total_pending"]
-        self.cashed = json_data["total_cashed"]
-        self.expired = json_data["total_expired"]
 
-    def rename(self, alias):
+        card = self.account.get_card(number=self.number,
+                                     months=months)
+
+        self.is_xente_nova = card.is_xente_nova
+        self.alias = card.alias
+        self.pending = card.pending
+        self.cashed = card.cashed
+        self.expired = card.expired
+        self.summary_movements = card.summary_movements
+
+    def rename(self, alias: str) -> None:
         """
         Change the alias of the card
 
         :param alias: New alias for the card
-        :type alias: str
         """
-        self.account.rename_card(self.number, alias)
+        self.account.rename_card(number=self.number,
+                                 alias=alias)
+
+    def __repr__(self) -> str:
+        return f"{self.alias}: {self.number}"
+
 
 class Account():
     """
-    Class that represents a user account. Either email and password or token and user_id (not really necessary) must be specified
+    Class that represents a user account. Either both email and password or token must be specified
 
     :param email: Email address to login with
-    :type email: str
 
     :param password: Password to log in with
-    :type password: str
 
     :param token: Auth token to use for the requests. It will be auto-obtained if email and password are specified
-    :type token: str
 
-    :param user_id: The user account's id. Not really needed for anything unless you are doing weird shit with the JWTs
-    :type user_id: int
+    :param token_type: Usually `Bearer`, and that's the default
     """
-    def __init__(self, email=None, password=None, token=None, user_id=None):
-        if token is None:
-            self.token = token
-            self.login(email, password)
-        else:
-            self.token = token
+
+    def __init__(self, email: str = None, password: str = None, token: str = None, token_type: str = "Bearer", user_id: int = None, name: str = None, last_name: str = None, identity_number: str = None, identity_type: int = None, phone_number: str = None) -> None:
+        self.rest_adapter = RestAdapter(_rest_adapter.url)
+        """
+        The `busGal_api.rest_adapter.RestAdapter` this classe's methods use to do authenticated requests
+        """
+
+        if token:
+            self.rest_adapter.token = token
+            """
+            The user token. It is a JWT
             """
-            The user token. It is a JWT.
 
-            :type: str
+            self.rest_adapter.token_type = token_type
+            """
+            The type of token
             """
 
             self.user_id = user_id
             """
-            The user id. You won't probably need this
-
-            :type: int
+            The user id
             """
+        elif email and password:
+            self.login(email, password)
+        else:
+            raise TypeError(
+                "Account.__init__() expected either the 'token' or both the 'email' and 'password' arguments")
+
+        self.email = None
+        """
+        Email of the user
+        """
 
         self.name = None
         """
         First name of the user
-
-        :type: str
         """
 
         self.last_name = None
         """
         Last name of the user
-
-        :type: str
-        """
-
-        self.email  = None
-        """
-        Email of the user
-
-        :type: str
         """
 
         self.identity_number = None
         """
         Identity number of the user e.g. DNI
-
-        :type: str
         """
 
         self.identity_type = None
         """
-        Identity type. It can be "DNI" or "other"
-
-        :type: str
+        Identity type. It can be:
+        - 1: DNI
+        - 2: Other
         """
 
         self.phone_number = None
         """
         The user's phone number
+        """
 
-        :type: str
+    def _parse_token(self, data: dict) -> None:
+        """
+        Set token info obtained from an authenticated request or `login`
         """
 
-        self.refresh_data()
+        self.rest_adapter.token = data["token"]["user_token"]
+        self.token_type = data["token"]["token_type"]
 
-    def _make_post_request(self, url, data):
+    def login(self, email: str, password: str) -> None:
+        """
+        Logins with the given email and password and returns a token, which is also set to self.token
         """
-        Calls make_post_request using the object's token, which is updated after every request. Not intended to be used by clients
 
-        :param url: Full url to make the request to
-        :type url: str
+        data = _rest_adapter.post("/user/login",
+                                  data={"email": email,
+                                        "password": password})
 
-        :param data: Data to send, it will be sent as application/json
-        :type data: dict
+        self.user_id = data["user_id"]
 
-        :return: Dictionary made from the request's json
-        :rtype: dict
-        """
-        json = make_post_request(url, data, self.token)
-        self.token = json["results"]["token"]["user_token"] # A new token is returned in every request, tokens don't seem to expire, but just in case we'll do as in the app.
-        return json
+        self._parse_token(data)
 
-    def _make_get_request(self, url):
+    def refresh_data(self) -> None:
         """
-        Calls make_get_request using the object's token, which is updated after every request. Not intended to be used by clients
+        Obtains the user's details and sets them to the object
+        """
+
+        data = self.rest_adapter.get("/user/private/profile")
 
-        :param url: Full url to make the request to
-        :type url: str
+        self.name = data["name"]
+        self.last_name = data["last_name"]
+        self.email = data["email"]
+        self.identity_number = data["identity_number"]
+        self.identity_type = data["identity_type"]
+        self.phone_number = data["phone_number"]
 
-        :return: Dictionary made from the request's json
-        :rtype: dict
+    def get_cards(self, months: int = 0) -> list[Card]:
         """
-        json = make_get_request(url, self.token)
-        self.token = json["results"]["token"]["user_token"] # A new token is returned in every request, tokens don't seem to expire, but just in case we'll do as in the app.
-        return json
+        Get all the user cards
 
-    def login(self, email, password):
+        :param months: Something. Works well if set to 0
         """
-        Logins with the given email and password and returns a token, which is also set to self.token
 
-        :param email: Email address to login with
-        :type email: str
+        data = self.rest_adapter.post("/cards/summary",
+                                      data={"months": 0})
 
-        :param password: Password to login with
-        :type password: str
+        return [_parse_card(el, self) for el in data["cards"]]
 
-        :return: User token
-        :rtype: str
+    def get_card(self, number: int, months: int = 12) -> Card:
+        """
+        Get the object for the user's card with the specified number
+
+        :params months: How many months to get `summary_movements` for
         """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/user/login"
-        data = {
-         "email": email,
-         "password": password
-        }
-        json = self._make_post_request(url, data) # This function already sets self.token to the returned token
 
-        self.user_id = json["results"]["user_id"]
+        data = self.rest_adapter.get("/cards/get",
+                                     ep_params={"months": months,
+                                                "number": number})
 
-        return self.token
+        return _parse_card(data, self)
 
-    def refresh_data(self):
+    def add_card(self, number: int, alias: str) -> None:
         """
-        Obtains the user's details and sets them to the object
+        Add a card to the user with the specified number and alias
         """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/user/private/profile"
-        json = self._make_get_request(url)
-        user_data = json["results"]
-
-        self.name = user_data["name"]
-        self.last_name = user_data["last_name"]
-        self.email  = user_data["email"]
-        self.identity_number = user_data["identity_number"]
-        self.identity_type = "DNI" if user_data["identity_type"] == 1 else "other" # else is used here, "other" is 2
-        self.phone_number = user_data["phone_number"]
 
-    def get_cards(self):
+        self.rest_adapter.post("/cards/register",
+                               data={"alias": alias,
+                                     "number": str(number),
+                                     "type": 0})  # The app sends  this as 0 for both Xente Nova and normal cards
+
+    def rename_card(self, number: int, alias: str) -> None:
         """
-        Get all the user cards
+        Change the alias of a card with the specified number
 
-        :return: List with all the obtained cards' objects
-        :rtype: list(_Card)
+        :param alias: New alias for the card
         """
 
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/cards/summary"
-        data = {"months": 0}
-        json = self._make_post_request(url, data)
+        self.rest_adapter.post("/cards/update",
+                               data={"alias": alias,
+                                     "number": str(number)})
 
-        cards_data = json["results"]["cards"]
-        cards = []
-        for card in cards_data:
-            card = self.get_card(int(card["number"]))
-            cards.append(card)
+    def delete_card(self, number: int) -> None:
+        """
+        Delete the card with the specified number
+        """
 
-        return cards
+        self.rest_adapter.post("/cards/unregister",
+                               data={"number": str(number)})
 
-    def get_card(self, number):
-        """
-        Get the object for the user's card with the specified number
+    def __repr__(self) -> str:
+        return self.email
 
-        :param number: Number of the card
-        :type number: str
+## ^^^ Classes ^^^ ##
 
-        :return: Card object
-        :rtype: _Card
-        """
-        card = _Card(self, number)
+## vvv Methods vvv ##
 
-        return card
 
-    def add_card(self, number, alias):
-        """
-        Add a card to the user with the specified number and alias
+def _parse_card(data: dict, account: Account) -> Card:
+    """
+    Build a `Card` from a dict of API data
+    """
 
-        :param number: Number of the card
-        :type number: str
+    return Card(account=account,
+                number=data["number"],
+                is_xente_nova=data["type"] == 0,
+                travels=data.get("travels"),
+                alias=data.get("alias"),
+                pending=data.get("pending", data.get("total_pending")),
+                cashed=data.get("total_cashed"),
+                expired=data.get("expired"),
+                summary_movements=data.get("summary_datas")
+                )
 
-        :param alias: Alias for the card
-        :type alias: str
-        """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/cards/register"
-        data = {
-            "alias": alias,
-            "number": str(number),
-            "type": 0 # Idk what this is for, it is 0 for both Xente Nova and normal cards
-        }
-        self._make_post_request(url, data)
 
-    def rename_card(self, number, alias):
-        """
-        Change the alias of a card with the specified number
+def register_account(email: str, password: str, name: str, last_name: str, identity_type: str, identity_number: str, phone_number: str) -> None:
+    """
+    Register an user account
 
-        :param number: Number of the card
-        :type number: str
+    :param email: Email address
 
-        :param alias: New alias for the card
-        :type alias: str
-        """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/cards/update"
-        data = {
-            "alias": alias,
-            "number": str(number)
-        }
-        self._make_post_request(url, data)
+    :param password: Password (Must be at least 6 character length, including a digit and an upper case letter)
 
-    def delete_card(self, number):
-        """
-        Delete the card with the specified number
+    :param name: First name
 
-        :param number: Number of the card
-        :type number: str
-        """
-        url = "https://tpgal-ws.xunta.gal/tpgal_ws/rest/cards/unregister"
-        data = {"number": str(number)}
-        self._make_post_request(url, data)
+    :param last_name: Last name
+
+    :param identity_type: Identity type: "DNI" or "other"
+
+    :param identity_number: Identity number e.g. your DNI
+
+    :param phone_number: Phone number
+    """
+
+    if identity_type == "DNI":
+        identity_type = 1
+    elif identity_type == "other":
+        identity_type = 2
+    else:
+        raise Exception("identity_type must be 'DNI' or 'other'")
+
+    _rest_adapter.post("/user/register",
+                       data={
+                           "check_data_protection": 1,
+                           "email": email,
+                           "password": password,
+                           "name": name,
+                           "last_name": last_name,
+                           "identity_type": identity_type,
+                           "identity_number": identity_number,
+                           "phone_number": str(phone_number)
+                       })
+
+
+def recover_password(email: str) -> None:
+    """
+    Recover an account's password (sends an email with a new temporal one)
+
+    :param email: Email address
+    """
+
+    _rest_adapter.get("/user/password",
+                      ep_params={"email": email})
+
+## ^^^ Methods ^^^ ##
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `busGal_api-0.0.6.1/setup.py` & `busGal_api-0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6.1' 
-DESCRIPTION = 'Python API wrapper for bus.gal'
-with open("README.rst", "r", encoding="utf-8") as fh:
+VERSION = '0.1' 
+DESCRIPTION = 'Python API wrapper for the galician public transport'
+with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
         name="busGal_api", 
         version=VERSION,
         author="Pedro Rey Anca",
         author_email="contact@peprolinbot.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=["certifi>=2021.5.30", "chardet>=4.0.0", "idna>=2.10", "requests>=2.25.1", "urllib3>=1.26.5"],
+        install_requires=["requests>=2.25.1"],
         url="https://github.com/peprolinbot/bus.gal-api",
         project_urls={
             "Bug Tracker": "https://github.com/peprolinbot/bus.gal-api/issues",
             "Documentation": "https://busgal-api.readthedocs.io/en/latest/",
         },
-        keywords=['python'],
+        keywords=['bus', 'buses', 'transport', 'public transport', 'galicia', 'api'],
         classifiers= [
-            "Development Status :: 3 - Alpha",
+            "Development Status :: 4 - Beta",
             "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Topic :: Software Development :: Libraries :: Python Modules"
         ]
 )
```

