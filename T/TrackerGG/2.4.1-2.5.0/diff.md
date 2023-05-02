# Comparing `tmp/TrackerGG-2.4.1.tar.gz` & `tmp/TrackerGG-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackerGG-2.4.1.tar", last modified: Mon May  1 11:10:56 2023, max compression
+gzip compressed data, was "TrackerGG-2.5.0.tar", last modified: Tue May  2 07:14:56 2023, max compression
```

## Comparing `TrackerGG-2.4.1.tar` & `TrackerGG-2.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.047335 TrackerGG-2.4.1/
--rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-05-01 11:10:56.039583 TrackerGG-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.025067 TrackerGG-2.4.1/TrackerGG/
-drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.038586 TrackerGG-2.4.1/TrackerGG/Models/
--rw-rw-rw-   0        0        0      753 2023-05-01 02:11:36.000000 TrackerGG-2.4.1/TrackerGG/Models/__init__.py
--rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.4.1/TrackerGG/Models/csgo.py
--rw-rw-rw-   0        0        0     1477 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/platform.py
--rw-rw-rw-   0        0        0     1399 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/segment.py
--rw-rw-rw-   0        0        0     2059 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/user.py
--rw-rw-rw-   0        0        0      903 2023-05-01 02:11:19.000000 TrackerGG-2.4.1/TrackerGG/__init__.py
--rw-rw-rw-   0        0        0     5390 2023-05-01 11:04:08.000000 TrackerGG-2.4.1/TrackerGG/client.py
--rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/httpclient.py
--rw-rw-rw-   0        0        0     1693 2023-05-01 10:58:10.000000 TrackerGG-2.4.1/TrackerGG/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.032582 TrackerGG-2.4.1/TrackerGG.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 11:10:56.047841 TrackerGG-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-01 11:10:13.000000 TrackerGG-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.570174 TrackerGG-2.5.0/
+-rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1425 2023-05-02 07:14:56.568163 TrackerGG-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.512987 TrackerGG-2.5.0/TrackerGG/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.566166 TrackerGG-2.5.0/TrackerGG/Models/
+-rw-rw-rw-   0        0        0      821 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/__init__.py
+-rw-rw-rw-   0        0        0     3416 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/apex.py
+-rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.5.0/TrackerGG/Models/csgo.py
+-rw-rw-rw-   0        0        0     1506 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/platform.py
+-rw-rw-rw-   0        0        0     1445 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/segment.py
+-rw-rw-rw-   0        0        0     2073 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/Models/user.py
+-rw-rw-rw-   0        0        0      972 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/__init__.py
+-rw-rw-rw-   0        0        0     7666 2023-05-02 07:13:38.000000 TrackerGG-2.5.0/TrackerGG/client.py
+-rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.5.0/TrackerGG/httpclient.py
+-rw-rw-rw-   0        0        0     1703 2023-05-01 23:37:40.000000 TrackerGG-2.5.0/TrackerGG/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:14:56.531482 TrackerGG-2.5.0/TrackerGG.egg-info/
+-rw-rw-rw-   0        0        0     1425 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 07:14:56.000000 TrackerGG-2.5.0/TrackerGG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 07:14:56.571174 TrackerGG-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-02 07:14:44.000000 TrackerGG-2.5.0/setup.py
```

### Comparing `TrackerGG-2.4.1/LICENSE` & `TrackerGG-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.1/PKG-INFO` & `TrackerGG-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.4.1
+Version: 2.5.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.4.1/README.md` & `TrackerGG-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.1/TrackerGG/Models/__init__.py` & `TrackerGG-2.5.0/TrackerGG/Models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,12 @@
 """
 
 from .csgo import CSGOProfile
 from .csgo import CSGOMapSegment
 from .csgo import CSGOQueryData
 from .csgo import CSGOWeaponSegment
 from .csgo import CSGOWeapon
+
+from .apex import ApexProfile
+from .apex import ApexQueryData
+
 from .platform import Platform
```

### Comparing `TrackerGG-2.4.1/TrackerGG/Models/csgo.py` & `TrackerGG-2.5.0/TrackerGG/Models/csgo.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.1/TrackerGG/Models/platform.py` & `TrackerGG-2.5.0/TrackerGG/Models/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class Platform(Enum):
     steam = "steam"
     origin = "origin"
     xbl = "xbl"
     psn = "psn"
     uplay = "uplay"
+    battlenet = "battlenet"
 
 
 class PlatformInfo:
     def __init__(self, data: Dict[str, Union[str, int, None]]):
         platforms = {
             "steam": Platform.steam,
             "origin": Platform.origin,
```

### Comparing `TrackerGG-2.4.1/TrackerGG/Models/segment.py` & `TrackerGG-2.5.0/TrackerGG/Models/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 """
 
 from typing import Dict, Union, Any, Optional
 
 
 class Stat:
     def __init__(self, data: Dict[str, Union[int, float, str, dict, None]]):
+        if data is None:
+            return
         self.rank: Optional[int] = data["rank"]
         self.percentile: Optional[float] = data["percentile"]
         self.description: Optional[str] = data["description"]
         self.metadata: Optional[dict[str, Any]] = data["metadata"]
         self.category: Optional[str] = data["category"]
         self.display_name: str = data["displayName"]
         self.value: int = data["value"]
```

### Comparing `TrackerGG-2.4.1/TrackerGG/Models/user.py` & `TrackerGG-2.5.0/TrackerGG/Models/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class SocialAccount:
     def __init__(self, data: Dict[str, Union[str, int, None]]):
         self.platform_slug: str = data["platformSlug"]
         self.platform_user_id: Union[str, int] = data["platformUserId"]
         self.platform_user_handle: str = data["platformUserHandle"]
         self.platform_user_identifier: Union[str, int] = data["platformUserIdentifier"]
-        self.avatar_url: str = data["avatarUrl"]
+        self.avatar_url: Optional[str] = data.get("avatarUrl")
         self.additional_parameters: Any = data["additionalParameters"]
 
 
 class UserInfo:
     def __init__(self, data: Dict[str, Union[str, int, bool, list, None]]):
         social_accounts = []
         if data["socialAccounts"]:
```

### Comparing `TrackerGG-2.4.1/TrackerGG/__init__.py` & `TrackerGG-2.5.0/TrackerGG/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
+from .Models import Platform
 from .Models import CSGOProfile
 from .Models import CSGOMapSegment
 from .Models import CSGOWeaponSegment
 from .Models import CSGOWeapon
+from .Models import ApexProfile
+
 from .client import CSGOClient
+from .client import ApexClient
+
 from . import utils
-from .Models import Platform
```

### Comparing `TrackerGG-2.4.1/TrackerGG/client.py` & `TrackerGG-2.5.0/TrackerGG/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,45 +20,55 @@
 import json
 from typing import List, Union
 
 from .Models import CSGOProfile
 from .Models import CSGOMapSegment
 from .Models import CSGOWeaponSegment
 from .Models import CSGOQueryData
+from .Models import ApexProfile
+from .Models import ApexQueryData
+from .Models import Platform
+
 from .httpclient import HTTPClient
 from .httpclient import RequestMethod
 from .httpclient import ResponseData
 from .httpclient import Route
 
 
 class TrackerClient:
     """
     Parent class of CSGOClient, ApexClient, etc.
-    This class contains Tracker API Key, Event Loop, HTTP Client for interacting with TrackerAPI
+    This class contains the Tracker API Key, Event Loop, and HTTP Client for interacting with TrackerAPI.
 
     :param api_key: :class:`str` Tracker API Key.
     """
+
     api_key: str
     loop: asyncio.AbstractEventLoop
     http_client: HTTPClient
 
     def __init__(self, api_key: str) -> None:
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+        try:
+            asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+        except AttributeError:
+            pass
+
         self.loop = asyncio.get_event_loop()
         self.api_key = api_key
         self.http_client = HTTPClient(self.loop, self.api_key)
 
 
 class CSGOClient(TrackerClient):
     """
-    A class for interact with Tracker CSGO API
-    This class contains Tracker API Key, Event Loop, HTTP Client for interacting with TrackerAPI
+    A class for interacting with the Tracker CSGO API
+    This class contains the Tracker API Key, Event Loop, and HTTP Client for interacting with TrackerAPI.
 
     :param api_key: :class:`str` Tracker API Key.
     """
+
     def __init__(self, api_key: str) -> None:
         super().__init__(api_key)
 
     async def get_profile(self, identifier: str) -> CSGOProfile:
         """
         Returns career stats for an CSGO player.
 
@@ -76,15 +86,15 @@
 
         json_data: dict = json.loads(response.response_data)
 
         return CSGOProfile(json_data["data"])
 
     async def get_map_segment(self, identifier: str) -> List[CSGOMapSegment]:
         """
-        Returns stats of the map for a CSGO player.
+        Returns the stats of the map for a CSGO player.
 
         :param identifier: :class:`str`
         :return: List[:class:`CSGOMapSegment`]
         :raise AssertionError: If the response code is not 200
         """
         response: ResponseData = await self.http_client.request(
             Route(
@@ -104,15 +114,15 @@
         for segment in json_data["data"]:
             segments.append(CSGOMapSegment(segment))
 
         return segments
 
     async def get_weapon_segment(self, identifier: str) -> List[CSGOWeaponSegment]:
         """
-        Returns stats of the weapon for a CSGO player.
+        Returns the stats of the weapon for a CSGO player.
 
         :param identifier: :class:`str`
         :return: List[:class:`CSGOWeaponSegment`]
         :raise AssertionError: If the response code is not 200
         """
         response: ResponseData = await self.http_client.request(
             Route(
@@ -132,15 +142,15 @@
         for segment in json_data["data"]:
             segments.append(CSGOWeaponSegment(segment))
 
         return segments
 
     async def search_profile(self, query: str) -> Union[None, List[CSGOQueryData]]:
         """
-        Returns search data for a CSGO player using a unique identifier
+        Returns search data for a CSGO player using a unique identifier.
 
         :param query: :class:`str`
         :return: Union[None, List[:class:`CSGOQueryData`]]
         :raise AssertionError: If the response code is not 200
         """
         response: ResponseData = await self.http_client.request(
             Route(
@@ -160,7 +170,70 @@
 
         if json_data["data"]:
             query_data = []
             for dat in json_data["data"]:
                 query_data.append(CSGOQueryData(dat))
 
         return query_data
+
+
+class ApexClient(TrackerClient):
+    def __init__(self, api_key: str) -> None:
+        super().__init__(api_key)
+
+    async def get_profile(self, identifier: str, platform: Platform) -> ApexProfile:
+        """
+        Returns career stats for an Apex player.
+
+        :param platform: :class:`Platform`
+        :param identifier: :class:`str`
+        :return: :class:`ApexProfile`
+        :raise AssertionError: If the response code is not 200
+        """
+        response: ResponseData = await self.http_client.request(
+            Route(
+                RequestMethod.GET,
+                f"/apex/standard/profile/{platform.value}/{identifier}",
+            )
+        )
+
+        assert response.status == 200, (
+            "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+        )
+
+        json_data: dict = json.loads(response.response_data)
+
+        return ApexProfile(json_data["data"])
+
+    async def search_profile(
+        self, query: str, platform: Platform
+    ) -> Union[None, List[ApexQueryData]]:
+        """
+        Returns search data for an Apex player using a unique identifier.
+
+        :param platform: :class:`Platform`
+        :param query: :class:`str`
+        :return: Union[None, List[:class:`ApexQueryData`]]
+        :raise AssertionError: If the response code is not 200
+        """
+        response: ResponseData = await self.http_client.request(
+            Route(
+                RequestMethod.GET,
+                f"/apex/standard/search",
+                params={"platform": platform.value, "query": query},
+            )
+        )
+
+        assert response.status == 200, (
+            "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+        )
+
+        json_data: dict = json.loads(response.response_data)
+
+        query_data = None
+
+        if json_data["data"]:
+            query_data = []
+            for dat in json_data["data"]:
+                query_data.append(ApexQueryData(dat))
+
+        return query_data
```

### Comparing `TrackerGG-2.4.1/TrackerGG/httpclient.py` & `TrackerGG-2.5.0/TrackerGG/httpclient.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.1/TrackerGG/utils.py` & `TrackerGG-2.5.0/TrackerGG/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from typing import List, Union
 
 
 def query_map_by_key(
     maps: List[CSGOMapSegment], key: str
 ) -> Union[CSGOMapSegment, int]:
     """
-    Returns CSGOMapSegment that matches key
-    Returns -1 if there is no matching CSGOMapSegment Object
+    Returns a CSGOMapSegment that matches key.
+    Returns -1 if there is no matching CSGOMapSegment Object.
 
     :param maps: List[:class:`CSGOMapSegment`]
     :param key: :class:`str`
     :return: Union[:class:`CSGOMapSegment`, :class:`int`]
     """
     for _map in maps:
         if _map.attributes["key"] == key:
@@ -39,16 +39,16 @@
     return -1
 
 
 def query_weapon(
     weapons: List[CSGOWeaponSegment], key: CSGOWeapon
 ) -> Union[CSGOWeaponSegment, int]:
     """
-    Returns CSGOWeaponSegment that matches key
-    Returns -1 if there is no matching CSGOWeaponSegment Object
+    Returns a CSGO weapon segment that matches key.
+    Returns -1 if there is no matching CSGOWeaponSegment Object.
 
     :param weapons: List[:class:`CSGOWeaponSegment`]
     :param key: :class:`CSGOWeapon`
     :return: Union[:class:`CSGOWeaponSegment`, :class:`int`]
     """
     for _weapon in weapons:
         if _weapon.attributes["key"] == key.value:
```

### Comparing `TrackerGG-2.4.1/TrackerGG.egg-info/PKG-INFO` & `TrackerGG-2.5.0/TrackerGG.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.4.1
+Version: 2.5.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.4.1/setup.py` & `TrackerGG-2.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setuptools.setup(
     name="TrackerGG",
-    version="2.4.1",
+    version="2.5.0",
     author="DevRuby",
     author_email="hiveruby@gmail.com",
     description="TrackerGG API Wrapper Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dev-ruby/TrackerGG",
     packages=setuptools.find_packages(),
```

