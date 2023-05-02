# Comparing `tmp/pomice-2.4.1.tar.gz` & `tmp/pomice-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomice-2.4.1.tar", last modified: Fri Apr  7 00:28:52 2023, max compression
+gzip compressed data, was "pomice-2.5.0.tar", last modified: Tue May  2 01:06:04 2023, max compression
```

## Comparing `pomice-2.4.1.tar` & `pomice-2.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 00:28:52.259773 pomice-2.4.1/
--rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     5445 2023-04-07 00:28:52.259773 pomice-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4680 2023-04-06 02:52:29.000000 pomice-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 00:28:52.187768 pomice-2.4.1/pomice/
--rw-rw-rw-   0        0        0      853 2023-04-07 00:28:12.000000 pomice-2.4.1/pomice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:28:52.235155 pomice-2.4.1/pomice/applemusic/
--rw-rw-rw-   0        0        0      151 2023-03-11 15:22:18.000000 pomice-2.4.1/pomice/applemusic/__init__.py
--rw-rw-rw-   0        0        0     6107 2023-03-27 04:08:42.000000 pomice-2.4.1/pomice/applemusic/client.py
--rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.4.1/pomice/applemusic/exceptions.py
--rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.4.1/pomice/applemusic/objects.py
--rw-rw-rw-   0        0        0     8145 2023-03-27 02:36:38.000000 pomice-2.4.1/pomice/enums.py
--rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.4.1/pomice/events.py
--rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.4.1/pomice/exceptions.py
--rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.4.1/pomice/filters.py
--rw-rw-rw-   0        0        0     5302 2023-04-05 02:18:43.000000 pomice-2.4.1/pomice/objects.py
--rw-rw-rw-   0        0        0    23531 2023-04-07 00:27:42.000000 pomice-2.4.1/pomice/player.py
--rw-rw-rw-   0        0        0    34773 2023-04-06 02:57:31.000000 pomice-2.4.1/pomice/pool.py
--rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.4.1/pomice/py.typed
--rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.4.1/pomice/queue.py
--rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.4.1/pomice/routeplanner.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:28:52.257750 pomice-2.4.1/pomice/spotify/
--rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.4.1/pomice/spotify/__init__.py
--rw-rw-rw-   0        0        0     6522 2023-03-27 04:08:42.000000 pomice-2.4.1/pomice/spotify/client.py
--rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.4.1/pomice/spotify/exceptions.py
--rw-rw-rw-   0        0        0     3445 2023-04-05 02:18:43.000000 pomice-2.4.1/pomice/spotify/objects.py
--rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.4.1/pomice/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:28:52.207923 pomice-2.4.1/pomice.egg-info/
--rw-rw-rw-   0        0        0     5445 2023-04-07 00:28:52.000000 pomice-2.4.1/pomice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-07 00:28:52.000000 pomice-2.4.1/pomice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 00:28:52.000000 pomice-2.4.1/pomice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-07 00:28:52.000000 pomice-2.4.1/pomice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 00:28:52.000000 pomice-2.4.1/pomice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 00:28:52.259773 pomice-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2192 2023-03-13 23:27:32.000000 pomice-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.770781 pomice-2.5.0/
+-rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5445 2023-05-02 01:06:04.768782 pomice-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.673258 pomice-2.5.0/pomice/
+-rw-rw-rw-   0        0        0      853 2023-05-02 01:03:25.000000 pomice-2.5.0/pomice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.738954 pomice-2.5.0/pomice/applemusic/
+-rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.5.0/pomice/applemusic/__init__.py
+-rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.5.0/pomice/applemusic/client.py
+-rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/applemusic/exceptions.py
+-rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.5.0/pomice/applemusic/objects.py
+-rw-rw-rw-   0        0        0     8145 2023-03-27 02:36:38.000000 pomice-2.5.0/pomice/enums.py
+-rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.5.0/pomice/events.py
+-rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.5.0/pomice/exceptions.py
+-rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.5.0/pomice/filters.py
+-rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.5.0/pomice/objects.py
+-rw-rw-rw-   0        0        0    23884 2023-05-01 11:42:50.000000 pomice-2.5.0/pomice/player.py
+-rw-rw-rw-   0        0        0    35277 2023-05-02 01:01:04.000000 pomice-2.5.0/pomice/pool.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.5.0/pomice/py.typed
+-rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.5.0/pomice/queue.py
+-rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/routeplanner.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.765737 pomice-2.5.0/pomice/spotify/
+-rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/spotify/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.5.0/pomice/spotify/client.py
+-rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/spotify/exceptions.py
+-rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.5.0/pomice/spotify/objects.py
+-rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.5.0/pomice/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.721193 pomice-2.5.0/pomice.egg-info/
+-rw-rw-rw-   0        0        0     5445 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 01:06:04.771781 pomice-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2171 2023-04-29 18:06:01.000000 pomice-2.5.0/setup.py
```

### Comparing `pomice-2.4.1/LICENSE` & `pomice-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/PKG-INFO` & `pomice-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.4.1
+Version: 2.5.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.4.1/README.md` & `pomice-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/__init__.py` & `pomice-2.5.0/pomice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     raise DiscordPyOutdated(
         "You must have discord.py (v2.0 or greater) to use this library. "
         "Uninstall your current version and install discord.py 2.0 "
         "using 'pip install discord.py'",
     )
 
-__version__ = "2.4.1"
+__version__ = "2.5.0"
 __title__ = "pomice"
 __author__ = "cloudwithax"
 __license__ = "GPL-3.0"
 __copyright__ = "Copyright (c) 2023, cloudwithax"
 
 from .enums import *
 from .events import *
```

### Comparing `pomice-2.4.1/pomice/applemusic/client.py` & `pomice-2.5.0/pomice/applemusic/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 AM_URL_REGEX = re.compile(
     r"https?://music.apple.com/(?P<country>[a-zA-Z]{2})/(?P<type>album|playlist|song|artist)/(?P<name>.+)/(?P<id>[^?]+)",
 )
 AM_SINGLE_IN_ALBUM_REGEX = re.compile(
     r"https?://music.apple.com/(?P<country>[a-zA-Z]{2})/(?P<type>album|playlist|song|artist)/(?P<name>.+)/(?P<id>.+)(\?i=)(?P<id2>.+)",
 )
+
+AM_SCRIPT_REGEX = re.compile(r'<script.*?src="(/assets/index-.*?)"')
+
 AM_REQ_URL = "https://api.music.apple.com/v1/catalog/{country}/{type}s/{id}"
 AM_BASE_URL = "https://api.music.apple.com"
 
 
 class Client:
     """The base Apple Music client for Pomice.
     This will do all the heavy lifting of getting tracks from Apple Music
@@ -35,43 +38,69 @@
     def __init__(self) -> None:
         self.expiry: datetime = datetime(1970, 1, 1)
         self.token: str = ""
         self.headers: Dict[str, str] = {}
         self.session: aiohttp.ClientSession = None  # type: ignore
         self._log = logging.getLogger(__name__)
 
+    async def _set_session(self, session: aiohttp.ClientSession) -> None:
+        self.session = session
+
     async def request_token(self) -> None:
-        if not self.session:
-            self.session = aiohttp.ClientSession()
+        # First lets get the raw response from the main page
 
-        async with self.session.get("https://music.apple.com/assets/index.919fe17f.js") as resp:
-            if resp.status != 200:
-                raise AppleMusicRequestException(
-                    f"Error while fetching results: {resp.status} {resp.reason}",
-                )
-            text = await resp.text()
-            match = re.search('"(eyJ.+?)"', text)
-            if not match:
-                raise AppleMusicRequestException(
-                    "Could not find token in response.",
-                )
-            result = match.group(1)
+        resp = await self.session.get("https://music.apple.com")
+
+        if resp.status != 200:
+            raise AppleMusicRequestException(
+                f"Error while fetching results: {resp.status} {resp.reason}",
+            )
+
+        # Looking for script tag that fits criteria
+
+        text = await resp.text()
+        match = re.search(AM_SCRIPT_REGEX, text)
+
+        if not match:
+            raise AppleMusicRequestException(
+                "Could not find valid script URL in response.",
+            )
+
+        # Found the script file, lets grab our token
+
+        result = match.group(1)
+        asset_url = result
+
+        resp = await self.session.get("https://music.apple.com" + asset_url)
+
+        if resp.status != 200:
+            raise AppleMusicRequestException(
+                f"Error while fetching results: {resp.status} {resp.reason}",
+            )
+
+        text = await resp.text()
+        match = re.search('"(eyJ.+?)"', text)
+        if not match:
+            raise AppleMusicRequestException(
+                "Could not find token in response.",
+            )
+        result = match.group(1)
 
-            self.token = result
-            self.headers = {
-                "Authorization": f"Bearer {result}",
-                "Origin": "https://apple.com",
-            }
-            token_split = self.token.split(".")[1]
-            token_json = base64.b64decode(
-                token_split + "=" * (-len(token_split) % 4),
-            ).decode()
-            token_data = json.loads(token_json)
-            self.expiry = datetime.fromtimestamp(token_data["exp"])
-            self._log.debug(f"Fetched Apple Music bearer token successfully")
+        self.token = result
+        self.headers = {
+            "Authorization": f"Bearer {result}",
+            "Origin": "https://apple.com",
+        }
+        token_split = self.token.split(".")[1]
+        token_json = base64.b64decode(
+            token_split + "=" * (-len(token_split) % 4),
+        ).decode()
+        token_data = json.loads(token_json)
+        self.expiry = datetime.fromtimestamp(token_data["exp"])
+        self._log.debug(f"Fetched Apple Music bearer token successfully")
 
     async def search(self, query: str) -> Union[Album, Playlist, Song, Artist]:
         if not self.token or datetime.utcnow() > self.expiry:
             await self.request_token()
 
         result = AM_URL_REGEX.match(query)
         if not result:
@@ -89,74 +118,72 @@
             # so we're gonna scan for that and correct it
             id = sia_result.group("id2")
             type = "song"
             request_url = AM_REQ_URL.format(country=country, type=type, id=id)
         else:
             request_url = AM_REQ_URL.format(country=country, type=type, id=id)
 
-        async with self.session.get(request_url, headers=self.headers) as resp:
-            if resp.status != 200:
-                raise AppleMusicRequestException(
-                    f"Error while fetching results: {resp.status} {resp.reason}",
-                )
-            data: dict = await resp.json(loads=json.loads)
-            self._log.debug(
-                f"Made request to Apple Music API with status {resp.status} and response {data}",
+        resp = await self.session.get(request_url, headers=self.headers)
+
+        if resp.status != 200:
+            raise AppleMusicRequestException(
+                f"Error while fetching results: {resp.status} {resp.reason}",
             )
 
+        data: dict = await resp.json(loads=json.loads)
+        self._log.debug(
+            f"Made request to Apple Music API with status {resp.status} and response {data}",
+        )
+
         data = data["data"][0]
 
         if type == "song":
             return Song(data)
 
-        if type == "album":
+        elif type == "album":
             return Album(data)
 
-        if type == "artist":
-            async with self.session.get(
+        elif type == "artist":
+            resp = await self.session.get(
                 f"{request_url}/view/top-songs",
                 headers=self.headers,
-            ) as resp:
-                if resp.status != 200:
-                    raise AppleMusicRequestException(
-                        f"Error while fetching results: {resp.status} {resp.reason}",
-                    )
-                top_tracks: dict = await resp.json(loads=json.loads)
-                artist_tracks: dict = top_tracks["data"]
+            )
+            if resp.status != 200:
+                raise AppleMusicRequestException(
+                    f"Error while fetching results: {resp.status} {resp.reason}",
+                )
+
+            top_tracks: dict = await resp.json(loads=json.loads)
+            artist_tracks: dict = top_tracks["data"]
 
             return Artist(data, tracks=artist_tracks)
+        else:
+            track_data: dict = data["relationships"]["tracks"]
+            album_tracks: List[Song] = [Song(track) for track in track_data["data"]]
 
-        track_data: dict = data["relationships"]["tracks"]
-        album_tracks: List[Song] = [Song(track) for track in track_data["data"]]
+            if not len(album_tracks):
+                raise AppleMusicRequestException(
+                    "This playlist is empty and therefore cannot be queued.",
+                )
 
-        if not len(album_tracks):
-            raise AppleMusicRequestException(
-                "This playlist is empty and therefore cannot be queued.",
-            )
+            _next = track_data.get("next")
+            if _next:
+                next_page_url = AM_BASE_URL + _next
 
-        _next = track_data.get("next")
-        if _next:
-            next_page_url = AM_BASE_URL + _next
+                while next_page_url is not None:
+                    resp = await self.session.get(next_page_url, headers=self.headers)
 
-            while next_page_url is not None:
-                async with self.session.get(next_page_url, headers=self.headers) as resp:
                     if resp.status != 200:
                         raise AppleMusicRequestException(
                             f"Error while fetching results: {resp.status} {resp.reason}",
                         )
 
                     next_data: dict = await resp.json(loads=json.loads)
+                    album_tracks.extend(Song(track) for track in next_data["data"])
 
-                album_tracks.extend(Song(track) for track in next_data["data"])
+                    _next = next_data.get("next")
+                    if _next:
+                        next_page_url = AM_BASE_URL + _next
+                    else:
+                        next_page_url = None
 
-                _next = next_data.get("next")
-                if _next:
-                    next_page_url = AM_BASE_URL + _next
-                else:
-                    next_page_url = None
-
-        return Playlist(data, album_tracks)
-
-    async def close(self) -> None:
-        if self.session:
-            await self.session.close()
-            self.session = None  # type: ignore
+            return Playlist(data, album_tracks)
```

### Comparing `pomice-2.4.1/pomice/applemusic/objects.py` & `pomice-2.5.0/pomice/applemusic/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/enums.py` & `pomice-2.5.0/pomice/enums.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/events.py` & `pomice-2.5.0/pomice/events.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/exceptions.py` & `pomice-2.5.0/pomice/exceptions.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/filters.py` & `pomice-2.5.0/pomice/filters.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/objects.py` & `pomice-2.5.0/pomice/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/player.py` & `pomice-2.5.0/pomice/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
             if filter.tag == filter_tag:
                 del self._filters[index]
 
     def has_filter(self, *, filter_tag: str) -> bool:
         """Checks if a filter exists in the list of filters using its filter tag"""
         return any(f for f in self._filters if f.tag == filter_tag)
 
+    def has_filter_type(self, *, filter_type: Filter) -> bool:
+        """Checks if any filters applied match the specified filter type."""
+        return any(f for f in self._filters if type(f) == type(filter_type))
+
     def reset_filters(self) -> None:
         """Removes all filters from the list"""
         self._filters = []
 
     def get_preload_filters(self) -> List[Filter]:
         """Get all preloaded filters"""
         return [f for f in self._filters if f.preload == True]
@@ -330,24 +334,26 @@
         event.dispatch(self._bot)
 
         if isinstance(event, TrackStartEvent):
             self._ending_track = self._current
 
         self._log.debug(f"Dispatched event {data['type']} to player.")
 
+    async def _refresh_endpoint_uri(self, session_id: Optional[str]) -> None:
+        self._player_endpoint_uri = f"sessions/{session_id}/players"
+
     async def _swap_node(self, *, new_node: Node) -> None:
         if self.current:
             data: dict = {"position": self.position, "encodedTrack": self.current.track_id}
 
         del self._node._players[self._guild.id]
         self._node = new_node
         self._node._players[self._guild.id] = self
         # reassign uri to update session id
-        self._player_endpoint_uri = f"sessions/{self._node._session_id}/players"
-
+        await self._refresh_endpoint_uri(new_node._session_id)
         await self._dispatch_voice_update()
         await self._node.send(
             method="PATCH",
             path=self._player_endpoint_uri,
             guild_id=self._guild.id,
             data=data or None,
         )
```

### Comparing `pomice-2.4.1/pomice/pool.py` & `pomice-2.5.0/pomice/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
         heartbeat: int = 30,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         session: Optional[aiohttp.ClientSession] = None,
-        spotify_client_id: Optional[int] = None,
+        spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         apple_music: bool = False,
         fallback: bool = False,
         log_level: LogLevel = LogLevel.INFO,
         log_handler: Optional[logging.Handler] = None,
     ):
         if not isinstance(port, int):
@@ -155,15 +155,15 @@
             "Authorization": self._password,
             "User-Id": str(self._bot_user.id),
             "Client-Name": f"Pomice/{__version__}",
         }
 
         self._players: Dict[int, Player] = {}
 
-        self._spotify_client_id: Optional[int] = spotify_client_id
+        self._spotify_client_id: Optional[str] = spotify_client_id
         self._spotify_client_secret: Optional[str] = spotify_client_secret
 
         self._apple_music_client: Optional[applemusic.Client] = None
 
         if self._spotify_client_id and self._spotify_client_secret:
             self._spotify_client: spotify.Client = spotify.Client(
                 self._spotify_client_id,
@@ -270,14 +270,21 @@
         if self._version < LavalinkVersion(3, 7, 0):
             self._available = False
             raise LavalinkVersionIncompatible(
                 "The Lavalink version you're using is incompatible. "
                 "Lavalink version 3.7.0 or above is required to use this library.",
             )
 
+    async def _set_ext_client_session(self, session: aiohttp.ClientSession) -> None:
+        if self._spotify_client:
+            await self._spotify_client._set_session(session=session)
+
+        if self._apple_music_client:
+            await self._apple_music_client._set_session(session=session)
+
     async def _update_handler(self, data: dict) -> None:
         await self._bot.wait_until_ready()
 
         if not data:
             return
 
         if data["t"] == "VOICE_SERVER_UPDATE":
@@ -315,15 +322,15 @@
             msg = await self._websocket.receive()
             if msg.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
                 if self._fallback:
                     await self._handle_node_switch()
                 retry = backoff.delay()
                 await asyncio.sleep(retry)
                 if not self.is_connected:
-                    self._loop.create_task(self.connect())
+                    self._loop.create_task(self.connect(reconnect=True))
             else:
                 self._loop.create_task(self._handle_payload(msg.json()))
 
     async def _handle_payload(self, data: dict) -> None:
         op = data.get("op", None)
         if not op:
             return
@@ -369,77 +376,87 @@
             f"{self._rest_uri}/"
             f'{f"v{self._version.major}/" if include_version else ""}'
             f"{path}"
             f'{f"/{guild_id}" if guild_id else ""}'
             f'{f"?{query}" if query else ""}'
         )
 
-        async with self._session.request(
+        resp = await self._session.request(
             method=method,
             url=uri,
             headers=self._headers,
             json=data or {},
-        ) as resp:
-            self._log.debug(f"Making REST request with method {method} to {uri}")
-            if resp.status >= 300:
-                resp_data: dict = await resp.json()
-                raise NodeRestException(
-                    f'Error fetching from Lavalink REST api: {resp.status} {resp.reason}: {resp_data["message"]}',
-                )
-
-            if method == "DELETE" or resp.status == 204:
-                self._log.debug(
-                    f"REST request with method {method} to {uri} completed sucessfully and returned no data.",
-                )
-                return await resp.json(content_type=None)
+        )
+        self._log.debug(
+            f"Making REST request to Node {self._identifier} with method {method} to {uri}",
+        )
+        if resp.status >= 300:
+            resp_data: dict = await resp.json()
+            raise NodeRestException(
+                f'Error from Node {self._identifier} fetching from Lavalink REST api: {resp.status} {resp.reason}: {resp_data["message"]}',
+            )
 
-            if resp.content_type == "text/plain":
-                self._log.debug(
-                    f"REST request with method {method} to {uri} completed sucessfully and returned text with body {await resp.text()}",
-                )
-                return await resp.text()
+        if method == "DELETE" or resp.status == 204:
+            self._log.debug(
+                f"REST request to Node {self._identifier} with method {method} to {uri} completed sucessfully and returned no data.",
+            )
+            return await resp.json(content_type=None)
 
+        if resp.content_type == "text/plain":
             self._log.debug(
-                f"REST request with method {method} to {uri} completed sucessfully and returned JSON with body {await resp.json()}",
+                f"REST request to Node {self._identifier} with method {method} to {uri} completed sucessfully and returned text with body {await resp.text()}",
             )
-            return await resp.json()
+            return await resp.text()
+
+        self._log.debug(
+            f"REST request to Node {self._identifier} with method {method} to {uri} completed sucessfully and returned JSON with body {await resp.json()}",
+        )
+        return await resp.json()
 
     def get_player(self, guild_id: int) -> Optional[Player]:
         """Takes a guild ID as a parameter. Returns a pomice Player object or None."""
         return self._players.get(guild_id, None)
 
-    async def connect(self) -> "Node":
+    async def connect(self, *, reconnect: bool = False) -> "Node":
         """Initiates a connection with a Lavalink node and adds it to the node pool."""
         await self._bot.wait_until_ready()
 
         start = time.perf_counter()
 
         if not self._session:
             self._session = aiohttp.ClientSession()
 
         try:
-            version: str = await self.send(
-                method="GET",
-                path="version",
-                ignore_if_available=True,
-                include_version=False,
-            )
+            if not reconnect:
+                version: str = await self.send(
+                    method="GET",
+                    path="version",
+                    ignore_if_available=True,
+                    include_version=False,
+                )
 
-            await self._handle_version_check(version=version)
+                await self._handle_version_check(version=version)
+                await self._set_ext_client_session(session=self._session)
 
-            self._log.debug(f"Version check from node successful. Returned version {version}")
+                self._log.debug(
+                    f"Version check from Node {self._identifier} successful. Returned version {version}",
+                )
 
             self._websocket = await self._session.ws_connect(
                 f"{self._websocket_uri}/v{self._version.major}/websocket",
                 headers=self._headers,
                 heartbeat=self._heartbeat,
             )
 
+            if reconnect:
+                for player in self.players.values():
+                    await player._refresh_endpoint_uri(self._session_id)
+
             self._log.debug(
-                f"Connected to node websocket using {self._websocket_uri}/v{self._version.major}/websocket",
+                f"Node {self._identifier} successfully connected to websocket using {self._websocket_uri}/v{self._version.major}/websocket",
             )
 
             if not self._task:
                 self._task = self._loop.create_task(self._listen())
 
             self._available = True
 
@@ -472,22 +489,14 @@
             await player.destroy()
             self._log.debug("All players disconnected from node.")
 
         await self._websocket.close()
         await self._session.close()
         self._log.debug("Websocket and http session closed.")
 
-        if self._spotify_client:
-            await self._spotify_client.close()
-            self._log.debug("Spotify client session closed.")
-
-        if self._apple_music_client:
-            await self._apple_music_client.close()
-            self._log.debug("Apple Music client session closed.")
-
         del self._pool._nodes[self._identifier]
         self.available = False
         self._task.cancel()
 
         end = time.perf_counter()
         self._log.info(
             f"Successfully disconnected from node {self._identifier} and closed all sessions. Took {end - start:.3f}s",
@@ -924,15 +933,15 @@
         host: str,
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
         heartbeat: int = 30,
         loop: Optional[asyncio.AbstractEventLoop] = None,
-        spotify_client_id: Optional[int] = None,
+        spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         session: Optional[aiohttp.ClientSession] = None,
         apple_music: bool = False,
         fallback: bool = False,
         log_level: LogLevel = LogLevel.INFO,
         log_handler: Optional[logging.Handler] = None,
     ) -> Node:
```

### Comparing `pomice-2.4.1/pomice/queue.py` & `pomice-2.5.0/pomice/queue.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/routeplanner.py` & `pomice-2.5.0/pomice/routeplanner.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/spotify/client.py` & `pomice-2.5.0/pomice/spotify/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 class Client:
     """The base client for the Spotify module of Pomice.
     This class will do all the heavy lifting of getting all the metadata
     for any Spotify URL you throw at it.
     """
 
-    def __init__(self, client_id: int, client_secret: str) -> None:
-        self._client_id: int = client_id
+    def __init__(self, client_id: str, client_secret: str) -> None:
+        self._client_id: str = client_id
         self._client_secret: str = client_secret
 
         self.session: aiohttp.ClientSession = None  # type: ignore
 
         self._bearer_token: Optional[str] = None
         self._expiry: float = 0.0
         self._auth_token = b64encode(
@@ -45,28 +45,29 @@
         )
         self._grant_headers = {
             "Authorization": f"Basic {self._auth_token.decode()}",
         }
         self._bearer_headers: Optional[Dict] = None
         self._log = logging.getLogger(__name__)
 
+    async def _set_session(self, session: aiohttp.ClientSession) -> None:
+        self.session = session
+
     async def _fetch_bearer_token(self) -> None:
         _data = {"grant_type": "client_credentials"}
 
-        if not self.session:
-            self.session = aiohttp.ClientSession()
+        resp = await self.session.post(GRANT_URL, data=_data, headers=self._grant_headers)
 
-        async with self.session.post(GRANT_URL, data=_data, headers=self._grant_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestException(
-                    f"Error fetching bearer token: {resp.status} {resp.reason}",
-                )
+        if resp.status != 200:
+            raise SpotifyRequestException(
+                f"Error fetching bearer token: {resp.status} {resp.reason}",
+            )
 
-            data: dict = await resp.json(loads=json.loads)
-            self._log.debug(f"Fetched Spotify bearer token successfully")
+        data: dict = await resp.json(loads=json.loads)
+        self._log.debug(f"Fetched Spotify bearer token successfully")
 
         self._bearer_token = data["access_token"]
         self._expiry = time.time() + (int(data["expires_in"]) - 10)
         self._bearer_headers = {
             "Authorization": f"Bearer {self._bearer_token}",
         }
 
@@ -79,42 +80,42 @@
             raise InvalidSpotifyURL("The Spotify link provided is not valid.")
 
         spotify_type = result.group("type")
         spotify_id = result.group("id")
 
         request_url = REQUEST_URL.format(type=spotify_type, id=spotify_id)
 
-        async with self.session.get(request_url, headers=self._bearer_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestException(
-                    f"Error while fetching results: {resp.status} {resp.reason}",
-                )
-
-            data: dict = await resp.json(loads=json.loads)
-            self._log.debug(
-                f"Made request to Spotify API with status {resp.status} and response {data}",
+        resp = await self.session.get(request_url, headers=self._bearer_headers)
+        if resp.status != 200:
+            raise SpotifyRequestException(
+                f"Error while fetching results: {resp.status} {resp.reason}",
             )
 
+        data: dict = await resp.json(loads=json.loads)
+        self._log.debug(
+            f"Made request to Spotify API with status {resp.status} and response {data}",
+        )
+
         if spotify_type == "track":
             return Track(data)
         elif spotify_type == "album":
             return Album(data)
         elif spotify_type == "artist":
-            async with self.session.get(
+            resp = await self.session.get(
                 f"{request_url}/top-tracks?market=US",
                 headers=self._bearer_headers,
-            ) as resp:
-                if resp.status != 200:
-                    raise SpotifyRequestException(
-                        f"Error while fetching results: {resp.status} {resp.reason}",
-                    )
+            )
+            if resp.status != 200:
+                raise SpotifyRequestException(
+                    f"Error while fetching results: {resp.status} {resp.reason}",
+                )
 
-                track_data: dict = await resp.json(loads=json.loads)
-                tracks = track_data["tracks"]
-                return Artist(data, tracks)
+            track_data: dict = await resp.json(loads=json.loads)
+            tracks = track_data["tracks"]
+            return Artist(data, tracks)
         else:
             tracks = [
                 Track(track["track"])
                 for track in data["tracks"]["items"]
                 if track["track"] is not None
             ]
 
@@ -122,21 +123,21 @@
                 raise SpotifyRequestException(
                     "This playlist is empty and therefore cannot be queued.",
                 )
 
             next_page_url = data["tracks"]["next"]
 
             while next_page_url is not None:
-                async with self.session.get(next_page_url, headers=self._bearer_headers) as resp:
-                    if resp.status != 200:
-                        raise SpotifyRequestException(
-                            f"Error while fetching results: {resp.status} {resp.reason}",
-                        )
+                resp = await self.session.get(next_page_url, headers=self._bearer_headers)
+                if resp.status != 200:
+                    raise SpotifyRequestException(
+                        f"Error while fetching results: {resp.status} {resp.reason}",
+                    )
 
-                    next_data: dict = await resp.json(loads=json.loads)
+                next_data: dict = await resp.json(loads=json.loads)
 
                 tracks += [
                     Track(track["track"])
                     for track in next_data["items"]
                     if track["track"] is not None
                 ]
                 next_page_url = next_data["next"]
@@ -160,23 +161,17 @@
             )
 
         request_url = REQUEST_URL.format(
             type="recommendation",
             id=f"?seed_tracks={spotify_id}",
         )
 
-        async with self.session.get(request_url, headers=self._bearer_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestException(
-                    f"Error while fetching results: {resp.status} {resp.reason}",
-                )
-
-            data: dict = await resp.json(loads=json.loads)
+        resp = await self.session.get(request_url, headers=self._bearer_headers)
+        if resp.status != 200:
+            raise SpotifyRequestException(
+                f"Error while fetching results: {resp.status} {resp.reason}",
+            )
 
+        data: dict = await resp.json(loads=json.loads)
         tracks = [Track(track) for track in data["tracks"]]
 
         return tracks
-
-    async def close(self) -> None:
-        if self.session:
-            await self.session.close()
-            self.session = None  # type: ignore
```

### Comparing `pomice-2.4.1/pomice/spotify/objects.py` & `pomice-2.5.0/pomice/spotify/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice/utils.py` & `pomice-2.5.0/pomice/utils.py`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/pomice.egg-info/PKG-INFO` & `pomice-2.5.0/pomice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.4.1
+Version: 2.5.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.4.1/pomice.egg-info/SOURCES.txt` & `pomice-2.5.0/pomice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomice-2.4.1/setup.py` & `pomice-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # type: ignore
 import re
 
 import setuptools
 
 version = ""
-requirements = ["discord.py>=2.0.0", "aiohttp>=3.7.4,<4", "orjson"]
+requirements = ["aiohttp>=3.7.4,<4", "orjson"]
 with open("pomice/__init__.py") as f:
     version = re.search(
         r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
         f.read(),
         re.MULTILINE,
     ).group(1)
```

