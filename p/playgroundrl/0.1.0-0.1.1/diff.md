# Comparing `tmp/playgroundrl-0.1.0.tar.gz` & `tmp/playgroundrl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl-0.1.0.tar", last modified: Wed Jul 26 19:07:17 2023, max compression
+gzip compressed data, was "playgroundrl-0.1.1.tar", last modified: Mon Aug  7 02:21:38 2023, max compression
```

## Comparing `playgroundrl-0.1.0.tar` & `playgroundrl-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092923 playgroundrl-0.1.0/
--rw-r--r--   0 rayan      (501) staff       (20)      170 2023-07-26 19:07:17.092966 playgroundrl-0.1.0/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      452 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-07-26 19:07:17.093125 playgroundrl-0.1.0/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      456 2023-07-26 19:07:01.000000 playgroundrl-0.1.0/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.090927 playgroundrl-0.1.0/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092157 playgroundrl-0.1.0/src/playgroundrl/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-02-27 07:47:18.000000 playgroundrl-0.1.0/src/playgroundrl/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     1313 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/src/playgroundrl/actions.py
--rw-r--r--   0 rayan      (501) staff       (20)    13029 2023-07-26 19:03:20.000000 playgroundrl-0.1.0/src/playgroundrl/client.py
--rw-r--r--   0 rayan      (501) staff       (20)     5421 2023-07-25 01:29:43.000000 playgroundrl-0.1.0/src/playgroundrl/state.py
--rw-r--r--   0 rayan      (501) staff       (20)      418 2023-06-29 23:39:57.000000 playgroundrl-0.1.0/src/playgroundrl/util.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-07-26 19:07:17.092830 playgroundrl-0.1.0/src/playgroundrl.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      170 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      362 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       52 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)       13 2023-07-26 19:07:17.000000 playgroundrl-0.1.0/src/playgroundrl.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-08-07 02:21:38.019448 playgroundrl-0.1.1/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-08-07 02:21:38.019567 playgroundrl-0.1.1/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      452 2023-08-05 16:36:16.000000 playgroundrl-0.1.1/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2023-08-07 02:21:38.019862 playgroundrl-0.1.1/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      457 2023-08-07 02:21:00.000000 playgroundrl-0.1.1/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-08-07 02:21:38.014950 playgroundrl-0.1.1/src/
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-08-07 02:21:38.017653 playgroundrl-0.1.1/src/playgroundrl/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-04-08 20:30:44.000000 playgroundrl-0.1.1/src/playgroundrl/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     1313 2023-08-05 16:36:16.000000 playgroundrl-0.1.1/src/playgroundrl/actions.py
+-rw-r--r--   0 langston   (501) staff       (20)     2972 2023-08-06 20:09:29.000000 playgroundrl-0.1.1/src/playgroundrl/args.py
+-rw-r--r--   0 langston   (501) staff       (20)    13573 2023-08-07 01:45:33.000000 playgroundrl-0.1.1/src/playgroundrl/client.py
+-rw-r--r--   0 langston   (501) staff       (20)     5421 2023-08-05 16:36:16.000000 playgroundrl-0.1.1/src/playgroundrl/state.py
+-rw-r--r--   0 langston   (501) staff       (20)      418 2023-08-05 16:36:16.000000 playgroundrl-0.1.1/src/playgroundrl/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-08-07 02:21:38.019182 playgroundrl-0.1.1/src/playgroundrl.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-08-07 02:21:38.000000 playgroundrl-0.1.1/src/playgroundrl.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      387 2023-08-07 02:21:38.000000 playgroundrl-0.1.1/src/playgroundrl.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2023-08-07 02:21:38.000000 playgroundrl-0.1.1/src/playgroundrl.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       52 2023-08-07 02:21:38.000000 playgroundrl-0.1.1/src/playgroundrl.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)       13 2023-08-07 02:21:38.000000 playgroundrl-0.1.1/src/playgroundrl.egg-info/top_level.txt
```

### Comparing `playgroundrl-0.1.0/src/playgroundrl/actions.py` & `playgroundrl-0.1.1/src/playgroundrl/actions.py`

 * *Files identical despite different names*

### Comparing `playgroundrl-0.1.0/src/playgroundrl/client.py` & `playgroundrl-0.1.1/src/playgroundrl/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from playgroundrl.actions import DictLikeAction
 import socketio
-from abc import ABC, abstractmethod
+from abc import ABC
 import requests
 import webbrowser
 from urllib.parse import urljoin
 from typing import Dict, Union
 from enum import Enum
 from .state import *
 import cattrs
 import json
 import codecs
 import pickle
+import logging
+
+logger = logging.getLogger("playgroundrl")
 
 
 class GameType(Enum):
     """Enumeration of different supported games"""
 
     SNAKE = "snake"
 
@@ -68,15 +71,14 @@
     """Models playing models"""
 
     OPEN = 2
     """Both humans and models playing each other"""
 
 
 # TODO: Handle retrying and what happens if we never receive a message back ()
-# TODO: Turn print statements into logging statements
 # TODO: Turn Dict messages into classes
 # TODO: Kill the client better, sometimes it hangs
 # TODO: Create enums for game_types (MODEL_ONLY=1, OPEN_POOL=2)
 class PlaygroundClient(ABC):
     """
     The base client to interface with the server. Handles all non-game specific logic.
 
@@ -87,36 +89,51 @@
         self,
         game: GameType,
         model_name: str,
         auth: Dict = None,
         auth_file: str = None,
         endpoint: str = "https://cdn.playgroundrl.com:8083",
         render_gameplay: bool = False,
-        # additional_parameters: Dict[str, str] = {},
+        log_level: str = None,
     ):
         """
         Initializes a client Object and connects to the server.
 
         :param game: String representing game name. 'tictactoe', 'chess', or 'snake'.
+
         :param model_name: Name of your RL model. Should be distinct in your user.
+
         :param auth: Dictionary containing auth data. In simple case, should contain
                 'email' and 'api_key' fields.
+
         :param auth_file: File containing endpoint and authdata (mutually exclusive with `auth and `endpoint`).
                 Expects a JSON file, structured as {"endpoint": ..., "auth": {"api_key": ..., "email": ...}}
         :param endpoint: URL of backend endpoint to connect to. Mainly used for
                 connecting to development server.
+
         :param render_gameplay: Whether to visualize game-play server-side
+
+        :param log_level: If set, we automatically initialize the logger, and log messages of level
+            `log_level` and above. Otherwise, logs are logged to 'playgroundrl`, and you can set the
+            log level manually with logging.getLogger("playgroundrl").setLevel(...).
+            See https://docs.python.org/3/library/logging.html.
         """
 
+        if log_level is not None:
+            logging.basicConfig(level=log_level)
+            logging.getLogger("playgroundrl").setLevel(log_level)
+
         # Retrieve user id
         # urljoin has weird behavior when it's not terminated right
         if auth_file is not None:
             with open(auth_file, "r") as f:
                 data = json.loads(f.read())
-                endpoint = data["endpoint"]
+                if "endpoint" in data:
+                    endpoint = data["endpoint"]
+                # Otherwise, use default endpoint
                 auth = data["auth"]
 
         if not endpoint.endswith("/"):
             endpoint += "/"
 
         url = urljoin(endpoint, "email_to_uid")
         response = requests.get(url, params={"email": auth["email"]})
@@ -166,17 +183,16 @@
 
         Returns the action for the client to take,
         or none for no action.
         """
         # TODO: Make self, state, and reward proper objects
         pass
 
-    @abstractmethod
     def gameover_callback(self) -> None:
-        """User-defined callback to run an action when the game ends"""
+        """Optional user-defined callback to run an action when the game ends"""
         pass
 
     ### PUBLIC FUNCTIONS ###
 
     def wait_for_game(self):
         """
         Wait for currently running game to complete
@@ -191,17 +207,17 @@
         Returns whether it is our move
         """
         _user = state.player_moving_id
         return _user in self.player_ids
 
     def run(
         self,
-        pool: Pool = Pool(1),
+        pool: Pool = Pool(2),
         num_games: int = 1,
-        maximum_messages: int = 5000,
+        maximum_messages: int = 50000,
         self_training: bool = False,
         game_parameters: Dict = {},
         create_lobby: bool = False,
         lobby_id: str = None,
         # TODO: This doesn't really work
         wait_for_game_end=True,
     ) -> None:
@@ -212,36 +228,36 @@
         :param maximum_messages: A timeout to prevent games from going on forever.
         :param self_training: Perform self-training. Instead of being matched with another
             player, this class will be responsible for all players in the game
         :param wait_for_game_end: Don't return from `run` until the game completes
         :param create_lobby: Optional parameter giving the option to create a lobby
         :param lobby_id: Optional parameter giving the option to join an existing lobby
         """
-        print("Run called")
+        logger.info("Run called")
         assert pool.value in [1, 2]
         self.pool = pool
         self.game_id = None
         self.self_training = self_training
         self.maximum_messages = maximum_messages
         self.game_parameters = game_parameters
         self.exchanged = 0
         self.wait_for_game_end = wait_for_game_end
         self.create_lobby = create_lobby
         self.lobby_id = lobby_id
 
-        print("Connecting....")
+        logger.debug("Connecting....")
         self.sio = socketio.Client()
         self.sio.connect(self.endpoint, auth=self.auth, namespaces=["/"])
         self._register_handlers()
 
         if self.render_gameplay:
             self.sio.emit("request_server_side_sid", {})
-        print("Connected!")
+        logger.info("Connected!")
 
-        print("  --running")
+        logger.info("  --running")
         self.running = True
         self.num_games -= 1
         # TODO: modify this to include the petting zoo game parameters
         start_game_payload = (
             {
                 "game": self.game_type.value,
                 "game_type": self.pool.value,
@@ -277,20 +293,20 @@
         self.sio.on("lobby_update", lambda msg: self._on_lobby_update_msg(msg))
         self.sio.on("*", lambda type, msg: self._default_callback(type, msg))
 
     def _on_get_server_side_sid(self, msg):
         self.server_side_sid = msg["server_side_sid"]
 
     def _on_state_msg(self, msg):
-        print(" --state_msg received: ")  # , msg)
+        logger.info(" --state_msg received: ")  # , msg)
         state = msg["state"]
         reward = msg["reward"]
         is_game_over = msg["is_game_over"]
         if is_game_over or self.exchanged > self.maximum_messages:
-            print("Game is over or max number of messages has been reached...")
+            logger.info("Game is over or max number of messages has been reached...")
             self.gameover_callback()
             return
 
         if self.game_type.value == "petting_zoo":
             # get python variables from serialized version
             unpickled = pickle.loads(codecs.decode(state.encode(), "base64"))
             raw_action = self.gym_callback(*unpickled)
@@ -305,47 +321,46 @@
             action = self.callback(state, reward)
 
         if action is not None:
             if issubclass(type(action), DictLikeAction):
                 # TODO: This is an unecessary JSON serialization
                 action = json.dumps(cattrs.unstructure(action))
             payload = {"action": action, "game_id": self.game_id}
-            print(" -- sending action: ", action)
+            logger.info(f" -- sending action: {action}")
             self.sio.emit("submit_agent_action", payload)
 
         self.exchanged += 1
 
     def _on_action_ack_msg(self, msg):
-        print(" --ack message received", msg)
-        # self.sio.emit('get_state', {'game_id': self.game_id})
+        logger.info(" --ack message received {msg}")
 
     # TODO: handle this gracefully
     def _on_game_over_msg(self, msg):
-        print(
+        logger.info(
             f"  --Game ended. Outcome for player {msg['player_id']}:  {msg['outcome']}"
         )
         if self.num_games <= 0:
-            print("  --No more games to run. Disconnecting...")
+            logger.debug("  --No more games to run. Disconnecting...")
             self.sio.disconnect()
             self.running = False
             return
         # TODO: This is an ugly hack
-        print(" --Starting the next game...")
+        logger.info(" --Starting the next game...")
         self.run(
             Pool(self.pool),
             self.num_games,
             self.maximum_messages,
             self.self_training,
             self.wait_for_game_end,
             self.create_lobby,
             self.lobby_id,
         )
 
     def _on_send_game_id_msg(self, msg):
-        print("  --send_game_id message received", msg)
+        logger.info("  --send_game_id message received {msg}")
         if (
             self.render_gameplay
             and self.game_id is None
             and self.server_side_sid is not None
             and not self.launched_renderer
         ):
             # TODO: figure out a cleaner way to do this
@@ -354,15 +369,15 @@
                 .replace(":8000/", "/")
                 .replace("stagingcdn", "dev")
                 .replace("cdn.", "")
             )
             if ".com" not in url:
                 url = url[:-1]
                 url += ":3000/"
-            print("URL", url)
+
             webbrowser.open(
                 url
                 + self.game_type.value.replace("_", "")
                 + "/?listen_to_sid="
                 + self.server_side_sid
                 + "&game_id="
                 + msg["game_id"]
@@ -376,15 +391,15 @@
         self.player_ids = msg["player_ids"]
 
         self.sio.emit(
             "get_state", {"game_id": self.game_id, "player_id": self.player_ids[0]}
         )
 
     def _on_lobby_update_msg(self, msg):
-        print(f"Receiving lobby update with id {msg['lobby_id']}")
+        logger.info(f"Receiving lobby update with id {msg['lobby_id']}")
         self.lobby_id = msg["lobby_id"]
 
     def _default_callback(self, msg_type, msg):
         raise Exception("Received unexpected data from server ->", msg_type, msg)
 
     def _on_error_msg(self, msg):
         raise Exception(msg)
```

### Comparing `playgroundrl-0.1.0/src/playgroundrl/state.py` & `playgroundrl-0.1.1/src/playgroundrl/state.py`

 * *Files identical despite different names*

