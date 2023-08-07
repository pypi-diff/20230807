# Comparing `tmp/monthify-0.4.6.tar.gz` & `tmp/monthify-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.4.6.tar", max compression
+gzip compressed data, was "monthify-0.4.8.tar", max compression
```

## Comparing `monthify-0.4.6.tar` & `monthify-0.4.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.4.6/README.md
--rw-r--r--   0        0        0      735 2023-07-02 01:29:05.096437 monthify-0.4.6/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.4.6/monthify/__main__.py
--rw-r--r--   0        0        0     1739 2023-08-01 19:57:31.582312 monthify-0.4.6/monthify/args.py
--rw-r--r--   0        0        0     1103 2023-07-02 01:14:09.885599 monthify-0.4.6/monthify/auth.py
--rw-r--r--   0        0        0      811 2023-07-02 01:14:09.885599 monthify-0.4.6/monthify/config.py
--rw-r--r--   0        0        0     3319 2023-08-01 20:00:17.933206 monthify-0.4.6/monthify/main.py
--rw-r--r--   0        0        0    19913 2023-08-01 20:00:17.934206 monthify-0.4.6/monthify/script.py
--rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.4.6/monthify/track.py
--rw-r--r--   0        0        0     1980 2023-08-01 19:57:31.582312 monthify-0.4.6/monthify/utils.py
--rw-r--r--   0        0        0      815 2023-08-01 20:01:13.479811 monthify-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.4.8/README.md
+-rw-r--r--   0        0        0      735 2023-07-02 01:29:05.096437 monthify-0.4.8/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.4.8/monthify/__main__.py
+-rw-r--r--   0        0        0     1739 2023-08-01 19:57:31.582312 monthify-0.4.8/monthify/args.py
+-rw-r--r--   0        0        0     1103 2023-07-02 01:14:09.885599 monthify-0.4.8/monthify/auth.py
+-rw-r--r--   0        0        0      811 2023-07-02 01:14:09.885599 monthify-0.4.8/monthify/config.py
+-rw-r--r--   0        0        0     3273 2023-08-06 09:37:33.569263 monthify-0.4.8/monthify/main.py
+-rw-r--r--   0        0        0    18572 2023-08-07 07:51:37.815320 monthify-0.4.8/monthify/script.py
+-rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.4.8/monthify/track.py
+-rw-r--r--   0        0        0     1980 2023-08-01 19:57:31.582312 monthify-0.4.8/monthify/utils.py
+-rw-r--r--   0        0        0      815 2023-08-07 07:51:37.815320 monthify-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.4.8/PKG-INFO
```

### Comparing `monthify-0.4.6/README.md` & `monthify-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/__init__.py` & `monthify-0.4.8/monthify/__init__.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/args.py` & `monthify-0.4.8/monthify/args.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/auth.py` & `monthify-0.4.8/monthify/auth.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/config.py` & `monthify-0.4.8/monthify/config.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/main.py` & `monthify-0.4.8/monthify/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
                 CLIENT_SECRET=CLIENT_SECRET,
                 LOCATION=appdata_location,
                 REDIRECT="https://open.spotify.com/",
                 SCOPES=(
                     "user-library-read",
                     "playlist-read-private",
                     "playlist-modify-private",
-                    "playlist-modify-public",
                 ),
             ),
             SKIP_PLAYLIST_CREATION=SKIP_PLAYLIST_CREATION,
             LOGOUT=LOGOUT,
             CREATE_PLAYLIST=CREATE_PLAYLIST,
             MAKE_PUBLIC=MAKE_PUBLIC,
         )
```

### Comparing `monthify-0.4.6/monthify/script.py` & `monthify-0.4.8/monthify/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,27 @@
 from monthify import ERROR, SUCCESS, appdata_location, console, logger
 from monthify.auth import Auth
 from monthify.track import Track
 from monthify.utils import conditional_decorator, normalize_text, sort_chronologically
 
 MAX_RESULTS = 10000
 CACHE_LIFETIME = 30
-MAX_WORKERS = 3
+MAX_WORKERS = 10
 
 existing_playlists_file = f"{appdata_location}/existing_playlists_file.dat"
 last_run_file = f"{appdata_location}/last_run.txt"
 last_run_format = "%Y-%m-%d %H:%M:%S"
 saved_tracks_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 saved_playlists_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 user_cache: TTLCache = TTLCache(maxsize=1, ttl=86400)
-playlist_items_cache: TTLCache = TTLCache(maxsize=100, ttl=86400)
 
 
 class Monthify:
     def __init__(
-        self,
-        auth: Auth,
-        SKIP_PLAYLIST_CREATION: bool,
-        LOGOUT: bool,
-        CREATE_PLAYLIST: bool,
-        MAKE_PUBLIC: bool,
+        self, auth: Auth, SKIP_PLAYLIST_CREATION: bool, LOGOUT: bool, CREATE_PLAYLIST: bool, MAKE_PUBLIC: bool
     ):
         self.MAKE_PUBLIC = MAKE_PUBLIC
         self.LOGOUT = LOGOUT
         self.logout()
         authentication = auth
         self.sp = authentication.get_spotipy()
         self.SKIP_PLAYLIST_CREATION = SKIP_PLAYLIST_CREATION
@@ -68,15 +62,15 @@
         if exists(last_run_file) and stat(last_run_file).st_size != 0:
             with open(last_run_file, "r", encoding="utf_8") as f:
                 self.last_run = f.read()
         else:
             self.last_run = ""
 
         self.playlist_names_with_id: List[Tuple[str, str, str]] = []
-        self.name = """
+        self.name = r"""
         ___  ___            _   _     _  __       
         |  \/  |           | | | |   (_)/ _|      
         | .  . | ___  _ __ | |_| |__  _| |_ _   _ 
         | |\/| |/ _ \| '_ \| __| '_ \| |  _| | | |
         | |  | | (_) | | | | |_| | | | | | | |_| |
         \_|  |_/\___/|_| |_|\__|_| |_|_|_|  \__, |
                                              __/ |
@@ -158,15 +152,14 @@
         """
 
         logger.info("Starting user saved playlists fetch")
         results = self.get_results(self.sp.current_user_playlists(limit=50))
         logger.info("Ending user saved playlists fetch")
         return results
 
-    @cached(playlist_items_cache)
     def get_playlist_items(self, playlist_id: str) -> List[dict]:
         """
         Retrieves all the tracks in a specified spotify playlist identified by playlist id
         """
 
         logger.info(f"Starting playlist item fetch\n id: {playlist_id}", playlist_id)
         results = self.get_results(self.sp.playlist_items(playlist_id=playlist_id, fields=None, limit=20))
@@ -194,19 +187,15 @@
                 logger.debug(f"Playlist creation took {perf_counter() - t0} s")
                 return log
 
         logger.debug(f"Playlist creation took {perf_counter() - t0} s")
         log += "\n" f"Creating playlist {name}"
         logger.info(f"Creating playlist {name}")
         playlist = sp.user_playlist_create(
-            user=self.current_username,
-            name=name,
-            public=self.MAKE_PUBLIC,
-            collaborative=False,
-            description=f"{name}",
+            user=self.current_username, name=name, public=self.MAKE_PUBLIC, collaborative=False, description=f"{name}"
         )
         created_playlists.append(playlist)
         log += "\n" f"Added {name} playlist"
         log += "\n"
         logger.info(f"Added {name} playlist")
         self.has_created_playlists = len(created_playlists) > 0
         return log
@@ -257,17 +246,15 @@
         with console.status("Retrieving relevant playlist information"):
             playlists = self.get_user_saved_playlists()
             for month, year in self.playlist_names:
                 for item in playlists:
                     if normalize_text((month + " '" + year[2:])) == normalize_text(item["name"]):
                         self.playlist_names_with_id.append((month, year, item["id"]))
                         logger.info(
-                            "Playlist name: {name} id: {id}",
-                            name=str(month + " '" + year[2:]),
-                            id=str(item["id"]),
+                            "Playlist name: {name} id: {id}", name=str(month + " '" + year[2:]), id=str(item["id"])
                         )
 
     def skip(self, status: bool, playlists: Optional[Iterable] = None) -> None:
         """
         Skips playlist generation if status is True
         """
 
@@ -276,15 +263,15 @@
             logger.info("Playlist generation skipped")
         else:
             logger.info("Playlist generation starting")
             if playlists is None:
                 RuntimeError("Playlists have not passed been passed to skip function")
             t0 = perf_counter()
             with ThreadPoolExecutor(max_workers=MAX_WORKERS) as executor:
-                playlist_names = [str(month + " '" + year[2:]) for month, year in self.playlist_names]
+                playlist_names = [str(month + " '" + year[2:]) for month, year in reversed(self.playlist_names)]
 
                 logs = executor.map(self.create_playlist, playlist_names)
                 for log in logs:
                     if log is not None:
                         console.print(log)
 
             logger.debug(f"Entire playlist generation took {perf_counter() - t0} s")
@@ -336,15 +323,15 @@
         else:
             self.skip(False, spotify_playlists)
 
         if self.already_created_playlists:
             with open(existing_playlists_file, "w", encoding="utf_8") as f:
                 f.write("\n".join(self.already_created_playlists))
 
-    def add_to_playlist(self, tracks: Reversible[Track], playlist_id: str) -> None:
+    def add_to_playlist(self, tracks: Reversible[Track], playlist_id: str) -> str:
         """
         Add a list of tracks to a specified playlist using playlist id
         """
 
         logger.info(
             "Attempting to add tracks to playlist: {playlist}\ntracks: {tracks} ",
             tracks=tracks,
@@ -400,37 +387,33 @@
         playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
         playlist_name = f"{month} '{year[2:]}"
         logger.info("Sorting into playlist: {playlist}", playlist=playlist_name)
         log = []
 
         tracks = tuple(track for track in self.get_saved_track_gen() if track.track_month == (month, year))
         if not tracks:
-            return
+            return log
         else:
             log.append(f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]")
             log.append("\t\n")
 
-            logger.info(
-                "Adding tracks to playlist: {playlist}",
-                playlist=str(playlist_id),
-            )
+            logger.info("Adding tracks to playlist: {playlist}", playlist=str(playlist_id))
             t0 = perf_counter()
             addedLog = self.add_to_playlist(tracks, playlist_id)
             logger.debug(f"Finished adding tracks to playlist: {str(playlist_id)} in {perf_counter() - t0:.2f}s")
             log.append(addedLog)
             return log
 
     def sort_all_tracks_by_month(self):
         """
         Sorts saved tracks into appropriate monthly playlist
         """
 
         log = logger.bind(
-            playlist_names=self.playlist_names_with_id,
-            tracks=[track.title for track in self.get_saved_track_gen()],
+            playlist_names=self.playlist_names_with_id, tracks=[track.title for track in self.get_saved_track_gen()]
         )
 
         log.info("Started sort")
 
         console.print("\nBeginning playlist sort")
         try:
             if len(self.playlist_names) != len(self.playlist_names_with_id):
@@ -466,29 +449,7 @@
             count = "One track added"
         elif self.total_tracks_added > 1:
             count = f"Total tracks added to playlists: {self.total_tracks_added}"
 
         console.print(count)
         console.print("Finished playlist sort")
         logger.info("Finished script execution")
-
-    def clean_playlist(self, playlist_id: str):
-        counts = dict()
-        tracks_to_remove = []
-        items = self.get_playlist_items(playlist_id)
-        snapshot_id = self.sp.playlist(playlist_id, fields="snapshot_id")["snapshot_id"]
-        for idx, item in enumerate(items):
-            counts[item["track"]["uri"]] = {
-                "count": (counts.get(item["track"]["uri"], {"count": 0, "positions": []}))["count"] + 1,
-                "positions": [idx + 1],
-            }
-
-        for item_id, values in counts.items():
-            if values["count"] > 1:
-                tracks_to_remove.append({"uri": item_id.split(":")[2], "positions": values["positions"]})
-
-        if tracks_to_remove:
-            tracks_to_remove_chunks = (tracks_to_remove[x : x + 100] for x in range(0, len(tracks_to_remove), 100))
-            for chunk in tracks_to_remove_chunks:
-                self.sp.playlist_remove_specific_occurrences_of_items(
-                    playlist_id=playlist_id, items=chunk, snapshot_id=snapshot_id
-                )
```

### Comparing `monthify-0.4.6/monthify/track.py` & `monthify-0.4.8/monthify/track.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/monthify/utils.py` & `monthify-0.4.8/monthify/utils.py`

 * *Files identical despite different names*

### Comparing `monthify-0.4.6/pyproject.toml` & `monthify-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monthify"
-version = "0.4.6"
+version = "0.4.8"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
```

### Comparing `monthify-0.4.6/PKG-INFO` & `monthify-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.4.6
+Version: 0.4.8
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

