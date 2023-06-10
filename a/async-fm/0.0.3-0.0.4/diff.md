# Comparing `tmp/async_fm-0.0.3.tar.gz` & `tmp/async_fm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_fm-0.0.3.tar", max compression
+gzip compressed data, was "async_fm-0.0.4.tar", max compression
```

## Comparing `async_fm-0.0.3.tar` & `async_fm-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-23 06:46:26.589924 async_fm-0.0.3/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-23 06:46:26.589924 async_fm-0.0.3/README.md
--rw-r--r--   0        0        0      683 2023-04-23 06:46:26.589924 async_fm-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      130 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/__init__.py
--rw-r--r--   0        0        0     1298 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/api/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/api/user.py
--rw-r--r--   0        0        0     2424 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/exceptions.py
--rw-r--r--   0        0        0     1235 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/types.py
--rw-r--r--   0        0        0      207 2023-04-23 06:46:26.589924 async_fm-0.0.3/src/asyncfm/utils.py
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-10 22:08:34.648947 async_fm-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1590 2023-06-10 22:08:34.648947 async_fm-0.0.4/README.md
+-rw-r--r--   0        0        0      683 2023-06-10 22:08:34.648947 async_fm-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/__init__.py
+-rw-r--r--   0        0        0     1264 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/api/__init__.py
+-rw-r--r--   0        0        0    14950 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/api/user.py
+-rw-r--r--   0        0        0     2403 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/exceptions.py
+-rw-r--r--   0        0        0     1437 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/types.py
+-rw-r--r--   0        0        0      208 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/utils.py
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.4/PKG-INFO
```

### Comparing `async_fm-0.0.3/LICENSE` & `async_fm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.3/README.md` & `async_fm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.3/pyproject.toml` & `async_fm-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Async-FM"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library for interacting with the Last.fm API asynchronously."
 authors = ["NachABR <nachabr@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asyncfm", from = "src"}]
 homepage = "https://github.com/NachABR/async-fm"
 repository = "https://github.com/NachABR/async-fm.git"
```

### Comparing `async_fm-0.0.3/src/asyncfm/api/__init__.py` & `async_fm-0.0.4/src/asyncfm/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import aiohttp
 from typing import Optional, Dict
 from asyncfm.api.user import LastFMUser
 from asyncfm.exceptions import get_error
 
 
-FM = type["LastFMAPI"]
-
-
 class LastFMAPI:
     def __init__(
         self,
         api_key: str,
         session: "Optional[aiohttp.ClientSession]" = None,
     ):
         self.api_key = api_key
         self.base_url = "http://ws.audioscrobbler.com/2.0/"
-        self.user = LastFMUser(api=self)
         self.session = session
 
+        self.user = LastFMUser(api=self)
+
     async def _request(self, session: "aiohttp.ClientSession", params: Dict[str, str]):
         async with session.get(url=self.base_url, params=params) as response:
+            data = await response.json()
             if response.status == 200:
-                return await response.json()
+                return data
 
-            error_data = await response.json()
+            error_code, error_message = data.get("error"), data.get("message")
 
-            raise (get_error(int(error_data.get("error"))))(
-                int(error_data.get("error")), error_data.get("message", "")
-            )
+            raise get_error(code=error_code)(code=error_code, message=error_message)
 
     async def _make_request(self, params: Dict[str, str]) -> Optional[Dict]:
         params = {"api_key": self.api_key, "format": "json", **params}
 
         if self.session is None:
             async with aiohttp.ClientSession() as session:
                 return await self._request(session=session, params=params)
```

### Comparing `async_fm-0.0.3/src/asyncfm/api/user.py` & `async_fm-0.0.4/src/asyncfm/api/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from datetime import datetime
 from typing import Optional
 
 from asyncfm import api
-from asyncfm.types import Album, APIResponse, Artist, Tag, Track, User
+from asyncfm.types import Album, Responses, Artist, Tag, Track, User
 from asyncfm.utils import get_images_
 
 
 class LastFMUser:
-    def __init__(self, api: "api.FM"):
+    def __init__(self, api: "api.LastFMAPI"):
         self.api = api
 
     async def get_info(self, username: str):
         params = {
             "method": "user.getinfo",
             "user": username,
         }
         data = await self.api._make_request(params=params)
 
-        user_data = data["user"]
-        return User(
-            name=user_data["name"],
-            age=user_data.get("age"),
-            subscriber=user_data.get("subscriber"),
-            realname=user_data.get("realname"),
-            bootstrap=user_data.get("bootstrap"),
-            playcount=user_data.get("playcount"),
-            artist_count=user_data.get("artist_count"),
-            playlists=user_data.get("playlists"),
-            track_count=user_data.get("track_count"),
-            album_count=user_data.get("album_count"),
-            image=get_images_(user_data.get("image")),
-            registered=datetime.fromtimestamp(int(user_data["registered"]["unixtime"])),
-            country=user_data.get("country"),
-            gender=user_data.get("gender"),
-            url=user_data.get("url"),
-            type=user_data.get("type"),
-        )
+        if user_data := data.get("user"):
+            return User(
+                name=user_data["name"],
+                age=user_data.get("age"),
+                subscriber=user_data.get("subscriber"),
+                realname=user_data.get("realname"),
+                bootstrap=user_data.get("bootstrap"),
+                playcount=user_data.get("playcount"),
+                artist_count=user_data.get("artist_count"),
+                playlists=user_data.get("playlists"),
+                track_count=user_data.get("track_count"),
+                album_count=user_data.get("album_count"),
+                image=get_images_(user_data.get("image")),
+                registered=datetime.fromtimestamp(user_data["registered"]["unixtime"]),
+                country=user_data.get("country"),
+                gender=user_data.get("gender"),
+                url=user_data.get("url"),
+                type=user_data.get("type"),
+            )
 
     async def get_recent_tracks(
         self,
         username: str,
         limit: int = 5,
         page: int = 1,
         extended: bool = False,
         from_time: int = None,
         to_time: int = None,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Tracks"]:
         """
         Fetches the recent tracks of a Last.fm user.
 
         Args:
         username (str): The Last.fm username to fetch the recent tracks of.
         limit (int, optional): The number of results to fetch per page. Defaults to 50. Maximum is 200.
         page (int, optional): The page number to fetch. Defaults to first page.
@@ -71,15 +71,15 @@
             params["from"] = from_time
         if to_time is not None:
             params["to"] = to_time
 
         data = await self.api._make_request(params=params)
 
         if recent_tracks := data.get("recenttracks"):
-            return APIResponse(
+            return Responses.Tracks(
                 data=list(
                     map(
                         lambda track: Track(
                             artist=track["artist"]["#text"],
                             title=track["name"],
                             album=track["album"]["#text"],
                             images=get_images_(track.get("image")),
@@ -87,23 +87,22 @@
                             and "nowplaying" in track["@attr"],
                         ),
                         recent_tracks["track"],
                     )
                 ),
                 total=recent_tracks.get("@attr", {}).get("total"),
             )
-        return None
 
     async def get_top_artists(
         self,
         username: str,
         period: str = "overall",
         limit: int = 5,
         page: int = 1,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Artists"]:
         """
         Fetches the top artists for a Last.fm user.
 
         Args:
         user (str): The Last.fm username to fetch top artists for.
         period (str, optional): The time period over which to retrieve top artists for. Defaults to "overall". Possible values are "overall", "7day", "1month", "3month", "6month", "12month".
         limit (int, optional): The number of results to fetch per page. Defaults to 50.
@@ -117,33 +116,32 @@
             "user": username,
             "period": period,
             "limit": limit,
             "page": page,
         }
         data = await self.api._make_request(params=params)
         if artists := data.get("topartists"):
-            return APIResponse(
+            return Responses.Artists(
                 data=list(
                     map(
                         lambda artist: Artist(
                             name=artist["name"],
                             images=get_images_(artist.get("image")),
                             playcount=artist["playcount"],
                             rank=artist["@attr"]["rank"],
                         ),
                         artists["artist"],
                     )
                 ),
                 total=artists.get("@attr").get("total"),
             )
-        return None
 
     async def get_top_albums(
         self, username: str, period: str = "overall", limit: int = 5, page: int = 1
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Albums"]:
         """
         Fetches the top albums for a Last.fm user.
 
         Args:
             period (str, optional): The time period over which to retrieve top albums for. Defaults to "overall". Possible values are "overall", "7day", "1month", "3month", "6month", "12month".
             limit (int, optional): The number of results to fetch per page. Defaults to 50.
             page (int, optional): The page number to fetch. Defaults to first page.
@@ -156,38 +154,37 @@
             "user": username,
             "period": period,
             "limit": limit,
             "page": page,
         }
         data = await self.api._make_request(params=params)
         if albums := data.get("topalbums"):
-            return APIResponse(
+            return Responses.Albums(
                 data=list(
                     map(
                         lambda album: Album(
                             artist=album["artist"]["name"],
                             title=album["name"],
                             images=get_images_(album.get("image")),
                             playcount=album["playcount"],
                             rank=album["@attr"]["rank"],
                         ),
                         albums["album"],
                     )
                 ),
                 total=albums.get("@attr").get("total"),
             )
-        return None
 
     async def get_top_tracks(
         self,
         username: str,
         period: str = "overall",
         limit: int = 5,
         page: int = 1,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Tracks"]:
         """
         Fetches the top tracks for a Last.fm user.
 
         Args:
         user (str): The Last.fm username to fetch top tracks for.
         period (str, optional): The time period over which to retrieve top tracks for. Defaults to "overall". Possible values are "overall", "7day", "1month", "3month", "6month", "12month".
         limit (int, optional): The number of results to fetch per page. Defaults to 50.
@@ -203,33 +200,32 @@
             "limit": limit,
             "page": page,
         }
 
         data = await self.api._make_request(params=params)
 
         if top_tracks := data.get("toptracks"):
-            return APIResponse(
+            return Responses.Tracks(
                 data=[
                     Track(
                         artist=track["artist"]["name"],
                         title=track["name"],
                         images=get_images_(track.get("image")),
                     )
                     for track in top_tracks["track"]
                 ],
                 total=top_tracks.get("@attr", {}).get("total"),
             )
-        return None
 
     async def get_top_tags(
         self,
         username: str,
         limit: int = 5,
         page: int = 1,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Tags"]:
         """
         Fetches the top tags for a Last.fm user.
 
         Args:
         user (str): The Last.fm username to fetch top tags for.
         limit (int, optional): The number of results to fetch per page. Defaults to 50.
         page (int, optional): The page number to fetch. Defaults to first page.
@@ -243,26 +239,25 @@
             "limit": limit,
             "page": page,
         }
 
         data = await self.api._make_request(params=params)
 
         if top_tags := data.get("toptags"):
-            return APIResponse(
+            return Responses.Tags(
                 data=[Tag(**tag) for tag in top_tags["tag"]],
                 total=len(top_tags["tag"]),
             )
-        return None
 
     async def get_weekly_artist_chart(
         self,
         username: str,
         from_date: Optional[datetime] = None,
         to_date: Optional[datetime] = None,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Artists"]:
         """
         Get the Last.fm chart of top artists for a given week.
 
         Args:
             username (str): The Last.fm username to fetch the chart for.
             from_date (datetime.datetime, optional): The start date of the week.
             to_date (datetime.datetime, optional): The end date of the week.
@@ -275,37 +270,36 @@
             params["from"] = from_date.strftime("%Y-%m-%d")
         if to_date is not None:
             params["to"] = to_date.strftime("%Y-%m-%d")
 
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklyartistchart"):
-            return APIResponse(
+            return Responses.Tracks(
                 data=list(
                     map(
                         lambda artist: Artist(
                             name=artist["name"],
                             playcount=artist["playcount"],
                             images=get_images_(images=images)
                             if (images := artist.get("image"))
                             else None,
                         ),
                         weekly_chart["artist"],
                     )
                 ),
                 total=len(weekly_chart["artist"]),
             )
-        return None
 
     async def get_weekly_album_chart(
         self,
         username: str,
         from_date: Optional[datetime] = None,
         to_date: Optional[datetime] = None,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Albums"]:
         """
         Get the Last.fm chart of top albums for a given week.
 
         Args:
 
         from_date (datetime.datetime, optional): The datetime for the beginning of the week.
         to_date (datetime.datetime, optional): The datetime for the end of the week.
@@ -321,15 +315,15 @@
             params["from"] = from_date.strftime("%Y-%m-%d")
         if to_date:
             params["to"] = to_date.strftime("%Y-%m-%d")
 
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklyalbumchart"):
-            return APIResponse(
+            return Responses.Albums(
                 data=list(
                     map(
                         lambda album: Album(
                             artist=album["artist"]["#text"],
                             title=album["name"],
                             images=get_images_(images=images)
                             if (images := album.get("image"))
@@ -338,22 +332,21 @@
                             playcount=album["playcount"],
                         ),
                         weekly_chart["album"],
                     )
                 ),
                 total=len(weekly_chart["album"]),
             )
-        return None
 
     async def get_weekly_track_chart(
         self,
         username: str,
         from_date: Optional[datetime] = None,
         to_date: Optional[datetime] = None,
-    ) -> Optional["APIResponse"]:
+    ) -> Optional["Responses.Tracks"]:
         """
         Fetches the weekly track chart for a Last.fm user.
 
         Args:
         username (str): The Last.fm username to fetch weekly track chart for.
         from_date (datetime.datetime): The date from which to start the weekly chart.
         to_date (datetime.datetime): The date to which to end the weekly chart.
@@ -369,23 +362,22 @@
         if from_date is not None:
             params["from"] = from_date.strftime("%Y-%m-%d")
         if to_date is not None:
             params["to"] = to_date.strftime("%Y-%m-%d")
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklytrackchart"):
-            return APIResponse(
+            return Responses.Tracks(
                 data=list(
                     map(
                         lambda track: Track(
                             artist=track["artist"]["#text"],
                             title=track["name"],
                             images=get_images_(track.get("image")),
                             rank=track["@attr"]["rank"],
                             playcount=track["playcount"],
                         ),
                         weekly_chart["track"],
                     )
                 ),
                 total=len(weekly_chart["track"]),
             )
-        return None
```

### Comparing `async_fm-0.0.3/src/asyncfm/exceptions.py` & `async_fm-0.0.4/src/asyncfm/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class FMError(Exception):
     def __init__(self, code: int, message: str):
         self.code = code
-        self.message = message.split(" - ", 1)[1]
+        self.message = message
         super().__init__(self.message)
 
 
 class Error(FMError):
     pass
 
 
@@ -73,15 +73,15 @@
     pass
 
 
 class TrialExpiredError(FMError):
     pass
 
 
-class NotExistError(FMError):
+class IgnoredError(FMError):
     pass
 
 
 class NotEnoughContentError(FMError):
     pass
 
 
@@ -129,15 +129,15 @@
         12: SubscribersOnlyError,
         13: InvalidMethodSignatureError,
         14: UnauthorizedTokenError,
         15: ItemNotAvailableError,
         16: ServiceUnavailableError,
         17: LoginError,
         18: TrialExpiredError,
-        19: NotExistError,
+        19: IgnoredError,
         20: NotEnoughContentError,
         21: NotEnoughMembersError,
         22: NotEnoughFansError,
         23: NotEnoughNeighboursError,
         24: NoPeakRadioError,
         25: RadioNotFoundError,
         26: APIKeySuspendedError,
```

### Comparing `async_fm-0.0.3/src/asyncfm/types.py` & `async_fm-0.0.4/src/asyncfm/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Optional, List, Union
+from typing import Optional, List
 from pydantic import BaseModel
 
 
 class Image(BaseModel):
     small: str
     medium: str
     large: str
@@ -59,10 +59,23 @@
 
 class Tag(BaseModel):
     name: str
     count: int
     url: str
 
 
-class APIResponse(BaseModel):
-    data: Optional[List[Union["Album", "Artist", "Track", "Tag"]]]
-    total: int
+class Responses:
+    class Tracks(BaseModel):
+        tracks: List[Track]
+        total: int
+
+    class Artists(BaseModel):
+        artists: List[Artist]
+        total: int
+
+    class Albums(BaseModel):
+        albums: List[Album]
+        total: int
+
+    class Tags(BaseModel):
+        tags: List[Tag]
+        total: int
```

### Comparing `async_fm-0.0.3/PKG-INFO` & `async_fm-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-fm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for interacting with the Last.fm API asynchronously.
 Home-page: https://github.com/NachABR/async-fm
 License: MIT
 Keywords: python,lastfm,aiohttp,async
 Author: NachABR
 Author-email: nachabr@protonmail.com
 Requires-Python: >=3.10,<4.0
```

