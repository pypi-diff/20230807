# Comparing `tmp/VodBot-1.1.7.tar.gz` & `tmp/VodBot-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VodBot-1.1.7.tar", last modified: Sat May  6 00:23:07 2023, max compression
+gzip compressed data, was "VodBot-1.1.8.tar", last modified: Mon Aug  7 02:59:43 2023, max compression
```

## Comparing `VodBot-1.1.7.tar` & `VodBot-1.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 00:23:07.846178 VodBot-1.1.7/
--rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.7/LICENSE.md
--rw-rw-rw-   0        0        0     4208 2023-05-06 00:23:07.845669 VodBot-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 00:23:07.817491 VodBot-1.1.7/VodBot.egg-info/
--rw-rw-rw-   0        0        0     4208 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      198 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 00:23:07.000000 VodBot-1.1.7/VodBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 00:23:07.846178 VodBot-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:23:07.830899 VodBot-1.1.7/vodbot/
--rw-rw-rw-   0        0        0       47 2023-05-06 00:02:15.000000 VodBot-1.1.7/vodbot/__init__.py
--rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.7/vodbot/__main__.py
--rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.7/vodbot/cache.py
--rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.7/vodbot/chatlog.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:23:07.840020 VodBot-1.1.7/vodbot/commands/
--rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.7/vodbot/commands/__init__.py
--rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.7/vodbot/commands/export.py
--rw-rw-rw-   0        0        0     3460 2023-05-03 01:36:40.000000 VodBot-1.1.7/vodbot/commands/info.py
--rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.7/vodbot/commands/init.py
--rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.7/vodbot/commands/pull.py
--rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.7/vodbot/commands/stage.py
--rw-rw-rw-   0        0        0    12978 2023-05-03 01:01:36.000000 VodBot-1.1.7/vodbot/commands/upload.py
--rw-rw-rw-   0        0        0    16412 2023-04-17 22:27:35.000000 VodBot-1.1.7/vodbot/config.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:23:07.844663 VodBot-1.1.7/vodbot/itd/
--rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.7/vodbot/itd/__init__.py
--rw-rw-rw-   0        0        0     3372 2023-05-03 01:01:36.000000 VodBot-1.1.7/vodbot/itd/download.py
--rw-rw-rw-   0        0        0     4625 2023-05-05 23:49:49.000000 VodBot-1.1.7/vodbot/itd/gql.py
--rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.7/vodbot/itd/worker.py
--rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.7/vodbot/printer.py
--rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.7/vodbot/thumbnail.py
--rw-rw-rw-   0        0        0    10250 2023-05-05 23:49:53.000000 VodBot-1.1.7/vodbot/twitch.py
--rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.7/vodbot/util.py
--rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.7/vodbot/video.py
--rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.7/vodbot/webhook.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.480494 VodBot-1.1.8/
+-rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.8/LICENSE.md
+-rw-rw-rw-   0        0        0     4208 2023-08-07 02:59:43.479488 VodBot-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.454381 VodBot-1.1.8/VodBot.egg-info/
+-rw-rw-rw-   0        0        0     4208 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      198 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:59:43.480494 VodBot-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.465559 VodBot-1.1.8/vodbot/
+-rw-rw-rw-   0        0        0       47 2023-08-07 02:59:06.000000 VodBot-1.1.8/vodbot/__init__.py
+-rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.8/vodbot/__main__.py
+-rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.8/vodbot/cache.py
+-rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.8/vodbot/chatlog.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.474294 VodBot-1.1.8/vodbot/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.8/vodbot/commands/__init__.py
+-rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.8/vodbot/commands/export.py
+-rw-rw-rw-   0        0        0     3460 2023-05-03 01:36:40.000000 VodBot-1.1.8/vodbot/commands/info.py
+-rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.8/vodbot/commands/init.py
+-rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.8/vodbot/commands/pull.py
+-rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.8/vodbot/commands/stage.py
+-rw-rw-rw-   0        0        0    12978 2023-05-03 01:01:36.000000 VodBot-1.1.8/vodbot/commands/upload.py
+-rw-rw-rw-   0        0        0    16532 2023-05-06 00:49:37.000000 VodBot-1.1.8/vodbot/config.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.478981 VodBot-1.1.8/vodbot/itd/
+-rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.8/vodbot/itd/__init__.py
+-rw-rw-rw-   0        0        0     3372 2023-05-03 01:01:36.000000 VodBot-1.1.8/vodbot/itd/download.py
+-rw-rw-rw-   0        0        0     4231 2023-08-07 02:29:41.000000 VodBot-1.1.8/vodbot/itd/gql.py
+-rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.8/vodbot/itd/worker.py
+-rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.8/vodbot/printer.py
+-rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.8/vodbot/thumbnail.py
+-rw-rw-rw-   0        0        0    10291 2023-08-07 02:29:32.000000 VodBot-1.1.8/vodbot/twitch.py
+-rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.8/vodbot/util.py
+-rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.8/vodbot/video.py
+-rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.8/vodbot/webhook.py
```

### Comparing `VodBot-1.1.7/LICENSE.md` & `VodBot-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/PKG-INFO` & `VodBot-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.7
+Version: 1.1.8
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.7/README.md` & `VodBot-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/VodBot.egg-info/PKG-INFO` & `VodBot-1.1.8/VodBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.7
+Version: 1.1.8
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.7/VodBot.egg-info/SOURCES.txt` & `VodBot-1.1.8/VodBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/setup.py` & `VodBot-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/__main__.py` & `VodBot-1.1.8/vodbot/__main__.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/cache.py` & `VodBot-1.1.8/vodbot/cache.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/chatlog.py` & `VodBot-1.1.8/vodbot/chatlog.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/export.py` & `VodBot-1.1.8/vodbot/commands/export.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/info.py` & `VodBot-1.1.8/vodbot/commands/info.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/init.py` & `VodBot-1.1.8/vodbot/commands/init.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/pull.py` & `VodBot-1.1.8/vodbot/commands/pull.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/stage.py` & `VodBot-1.1.8/vodbot/commands/stage.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/commands/upload.py` & `VodBot-1.1.8/vodbot/commands/upload.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/config.py` & `VodBot-1.1.8/vodbot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,17 @@
 	# Determines if chat logs get pulled with VODs and saved alongside metadata. This is a master
 	# switch for every channel, if false then no chat gets saved.
 	save_chat: bool = True
 
 	# Client ID for accessing Twitch's public facing but privately documented GraphQL interface, 
 	# which is significantly more advanced than the V5 API. Do not change this to a specific user's
 	# ID unless you want to risk a ban, although it allows for accessing private info such as
-	# deleted chat messages and account info.
-	gql_client: str = "kimne78kx3ncx6brgo4mv6wki5h1ko"
+	# deleted chat messages and account info. Recommended values (public client ID's) are
+	# "kimne78kx3ncx6brgo4mv6wki5h1ko" or "kd1unb4b3q4t58fwlpcbzcbnm76a8fp".
+	gql_client: str = "kd1unb4b3q4t58fwlpcbzcbnm76a8fp"
 
 	# Number of threads that can concurrently work to download files from Twitch.
 	# Defaults to the number of cores on the machine (or 1 in cases where that can't be measured).
 	max_workers: int = field(default=cpu_count() or 1, metadata=config(mm_field=fields.Int(validate=validate.Range(1))))
 	# Number of bytes to stream-write to temporary video files at a time.
 	# Defaults to 1024 bytes.
 	chunk_size: int = field(default=1024, metadata=config(mm_field=fields.Int(validate=validate.Range(1024))))
```

### Comparing `VodBot-1.1.7/vodbot/itd/download.py` & `VodBot-1.1.8/vodbot/itd/download.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/itd/gql.py` & `VodBot-1.1.8/vodbot/itd/gql.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,145 +4,123 @@
 from urllib.parse import urlencode
 
 
 GQL_URL = "https://gql.twitch.tv/gql"
 GQL_HEADERS = {"Client-ID": ""}
 
 
+class GQLException(Exception):
+	pass
+
+
 # We use Twitch's private client ID for GQL calls
 def set_client_id(client_id: str):
 	global GQL_HEADERS
 	GQL_HEADERS["Client-ID"] = client_id
 
-def _process_query_errors(resp):
-	if 400 <= resp.status_code < 500:
-		data = resp.json()
-		raise Exception(data["message"]) # TODO: make exceptions?
-	resp.raise_for_status()
-
-	if "errors" in resp:
-		raise Exception(resp["errors"])
-
 
-def gql_get(params={}):
-	resp = requests.get(GQL_URL, params=params, headers=GQL_HEADERS)
-	_process_query_errors(resp)
-	return resp
+def _process_query_errors(resp):
+	j = resp.json()
+	if 400 <= resp.status_code < 500 or "errors" in j:
+		raise GQLException(j)
 
 
 def gql_post(json=None, data=None):
+	global GQL_URL, GQL_HEADERS
 	resp = requests.post(GQL_URL, json=json, data=data, headers=GQL_HEADERS)
 	_process_query_errors(resp)
 	return resp
 
 
 def gql_query(query=None, data=None):
 	return gql_post(json={"query":query}, data=data)
-	# resp = requests.post(GQL_URL, json={"query":query}, data=data, headers=GQL_HEADERS)
-	# _process_query_errors(resp)
-	# return resp
 
 
 # GQL Query forms
 # Channel VODs query
 GET_CHANNEL_VIDEOS_QUERY = """
 {{  user(login: "{channel_id}") {{
-		videos( first: {first}, sort: {sort}, after: {after} ) {{
+		videos( first: {first}, sort: {sort}, after: "{after}" ) {{
 			totalCount
 			edges {{ cursor
-				node {{ id title
-					publishedAt broadcastType status
-					lengthSeconds thumbnailURLs
+				node {{
+					id title publishedAt broadcastType status lengthSeconds
 					game {{ id name }}
 					creator {{ id login displayName }}
 }}  }}  }}  }}  }}
 """
 # Channel Clips query
 # period can be LAST_DAY, LAST_WEEK, LAST_MONTH, or ALL_TIME
 GET_CHANNEL_CLIPS_QUERY = """
 {{  user(login: "{channel_id}") {{
 		clips(
-			first: {first}, after: {after},
-			criteria: {{ period: ALL_TIME, sort: VIEWS_DESC }}
+			first: {first}, after: "{after}",
+			criteria: {{ period: ALL_TIME, sort: CREATED_AT_DESC }}
 		) {{
 			edges {{ cursor
-				node {{ id slug title
-					createdAt viewCount
-					durationSeconds url videoOffsetSeconds
+				node {{ id slug title createdAt viewCount
+					durationSeconds videoOffsetSeconds
 					video {{ id }}
 					game {{ id name }}
 					broadcaster {{ id displayName login }}
 					curator {{ id displayName login }}
 }}  }}  }}  }}  }}
 """
 # Single VOD query
 GET_VIDEO_QUERY = """
-{{ video(id: "{video_id}") {{
+{{  video(id: "{video_id}") {{
 		id title publishedAt
 		broadcastType lengthSeconds
-		game {{ id name }}
-		creator {{ id login displayName }}
+		game {{ id name }} creator {{ id login displayName }}
 }}  }}
 """
 # Single Clip query
 GET_CLIP_QUERY = """
 {{  clip(slug: "{clip_slug}") {{
+		id slug title createdAt viewCount durationSeconds videoOffsetSeconds
+		game {{ id name }} video {{ id }}
 		videoQualities {{ frameRate quality sourceURL }}
-		id slug title
-		createdAt viewCount
-		durationSeconds url videoOffsetSeconds
-		video {{ id }}
-		game {{ id name }}
 		broadcaster {{ id displayName login }}
 		curator {{ id displayName login }}
 }}  }}
 """
 # Single Channel info query
 GET_CHANNEL_QUERY = """
 {{  user(login: "{channel_id}") {{
 		id login displayName
 		description createdAt
 		roles {{ isAffiliate isPartner }}
 		stream {{
-			id title type
-			viewersCount createdAt
-			game {{ id name }}
+			id title type viewersCount createdAt game {{ id name }}
 }}  }}  }}
 """
 # IRC Chat query
 GET_VIDEO_COMMENTS_QUERY = """
 {{ video(id: "{video_id}") {{
-	comments(contentOffsetSeconds: 0, after: {after}) {{
+	comments(contentOffsetSeconds: 0, after: "{after}") {{
 		edges {{ cursor node {{
 			contentOffsetSeconds
 			commenter {{ displayName }}
-			message {{ userColor 
-				fragments {{ mention {{ displayName }} text }}
-}}  }}  }}  }}  }} }}
+			message {{ userColor fragments {{ mention {{ displayName }} text }} }}
+}}  }}  }}  }} }}
 """
 # VOD chapters query
 GET_VIDEO_CHAPTERS = """{{
 video(id: {id}) {{
     moments(first:100, momentRequestType: VIDEO_CHAPTER_MARKERS, after: {after}) {{
         edges {{ cursor node {{
-            description type
-            positionMilliseconds
-			durationMilliseconds
+            description type positionMilliseconds durationMilliseconds
 }}  }}  }}  }}  }}
 """
 
 
 VIDEO_ACCESS_QUERY = """
 {{  videoPlaybackAccessToken(
 		id: {video_id},
-		params: {{
-			platform: "web",
-			playerBackend: "mediaplayer",
-			playerType: "site"
-		}}
+		params: {{ platform:"web", playerBackend:"mediaplayer", playerType:"site" }}
 	) {{ signature value }}
 }}
 """
 
 def get_access_token(video_id):
 	"""
 	Gets the VOD player access token, used to stream the VOD to the host.
```

### Comparing `VodBot-1.1.7/vodbot/itd/worker.py` & `VodBot-1.1.8/vodbot/itd/worker.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/printer.py` & `VodBot-1.1.8/vodbot/printer.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/thumbnail.py` & `VodBot-1.1.8/vodbot/thumbnail.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/twitch.py` & `VodBot-1.1.8/vodbot/twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,29 +192,30 @@
 	Uses a (blocking) HTTP request to retrieve VOD info for a specific channel.
 
 	:param channel: A Channel object.
 	:returns: A list of VOD objects.
 	"""
 
 	vods = []
-	pagination = "null"
+	pagination = ""
 	while True:
 		# get videos of multiple types
 		# past streams = ARCHIVE, segment of stream = HIGHLIGHT, upload = UPLOAD, premiere = PAST_PREMIERE
 		query = gql.GET_CHANNEL_VIDEOS_QUERY.format(
 			channel_id=channel.login,
 			after=pagination, first=100,
 			sort="TIME"
 		)
-		resp = gql.gql_query(query=query).json()["data"]["user"]["videos"]
+		resp = gql.gql_query(query=query).json()
+		resp = resp["data"]["user"]["videos"]
 
 		if not resp or not resp["edges"]:
 			break
 
-		pagination = f'"{resp["edges"][-1]["cursor"]}"'
+		pagination = resp["edges"][-1]["cursor"]
 		
 		for vod in resp["edges"]:
 			v = vod["node"]
 			c, g, b, s = v["creator"], v["game"], v["broadcastType"], v["status"]
 
 			# check broadcast type
 			if not any(b==t for t in ["ARCHIVE", "HIGHLIGHT", "UPLOAD", "PAST_PREMIERE"]):
@@ -236,15 +237,15 @@
 			while True:
 				query = gql.GET_VIDEO_CHAPTERS.format(
 					id=v["id"], after=chapter_page
 				)
 				resp = gql.gql_query(query=query).json()
 				resp = resp["data"]["video"]["moments"]
 				
-				if not resp or not resp["edges"]:
+				if not resp or not resp["edges"] or not resp["edges"][-1]["cursor"]:
 					break
 
 				chapter_page = f'"{resp["edges"][-1]["cursor"]}"'
 
 				for chap in resp["edges"]:
 					n = chap["node"]
 					chapters.append(
@@ -280,26 +281,27 @@
 	Uses a (blocking) HTTP request to retrieve Clip info for a specific channel.
 
 	:param channel: A Channel object.
 	:returns: A list of Clip objects.
 	"""
 
 	clips = []
-	pagination = "null"
+	pagination = ""
+	
 	while True:
 		query = gql.GET_CHANNEL_CLIPS_QUERY.format(
 			channel_id=channel.login,
 			after=pagination, first=100
 		)
 		resp = gql.gql_query(query=query).json()["data"]["user"]["clips"]
 
 		if not resp or not resp["edges"]:
 			break
 
-		pagination = f'"{resp["edges"][-1]["cursor"]}"'
+		pagination = {resp["edges"][-1]["cursor"]}
 		
 		for clip in resp["edges"]:
 			c = clip["node"]
 			b, w, g, v = c["broadcaster"], c["curator"], c["game"], c["video"]
 			v_id = "unknown" if v is None else v["id"]
 
 			w_id, w_login, w_name = b["id"], b["login"], b["displayName"]
@@ -335,25 +337,27 @@
 	Uses a (blocking) HTTP request to retrieve chat logs for a specific video.
 
 	:param video_id: A video ID string.
 	:returns: A list of ChatMessage objects.
 	"""
 
 	messages = []
-	pagination = "null"
+	pagination = ""
+
 	while True:
 		query = gql.GET_VIDEO_COMMENTS_QUERY.format(
 			video_id=video_id, first=100, after=pagination
 		)
-		resp = gql.gql_query(query=query).json()["data"]["video"]["comments"]
+		resp = gql.gql_query(query=query).json()
+		resp = resp["data"]["video"]["comments"]
 
 		if not resp or not resp["edges"]:
 			break
 
-		pagination = f'"{resp["edges"][-1]["cursor"]}"'
+		pagination = {resp["edges"][-1]["cursor"]}
 
 		for comment in resp["edges"]:
 			c = comment["node"]
 			
 			usr = "-BANNED?_USER-"
 			if c["commenter"] is not None:
 				usr = c["commenter"]["displayName"]
```

### Comparing `VodBot-1.1.7/vodbot/util.py` & `VodBot-1.1.8/vodbot/util.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/video.py` & `VodBot-1.1.8/vodbot/video.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.7/vodbot/webhook.py` & `VodBot-1.1.8/vodbot/webhook.py`

 * *Files identical despite different names*

