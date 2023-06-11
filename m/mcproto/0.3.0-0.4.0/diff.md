# Comparing `tmp/mcproto-0.3.0.tar.gz` & `tmp/mcproto-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcproto-0.3.0.tar", max compression
+gzip compressed data, was "mcproto-0.4.0.tar", max compression
```

## Comparing `mcproto-0.3.0.tar` & `mcproto-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,31 @@
--rw-r--r--   0        0        0     2744 2023-06-08 15:40:16.419106 mcproto-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2924 2023-06-08 15:40:16.423106 mcproto-0.3.0/LICENSE-THIRD-PARTY.txt
--rw-r--r--   0        0        0     7651 2023-06-08 15:40:16.423106 mcproto-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0    17616 2023-06-08 15:40:16.423106 mcproto-0.3.0/README.md
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/__init__.py
--rw-r--r--   0        0        0     3211 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/buffer.py
--rw-r--r--   0        0        0    12532 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/connection.py
--rw-r--r--   0        0        0      590 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/__init__.py
--rw-r--r--   0        0        0     1028 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/abc.py
--rw-r--r--   0        0        0     3514 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/interactions.py
--rw-r--r--   0        0        0     3913 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/map.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/__init__.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/handshaking/__init__.py
--rw-r--r--   0        0        0     2215 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/handshaking/handshake.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/login/__init__.py
--rw-r--r--   0        0        0     7924 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/login/login.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/ping.py
--rw-r--r--   0        0        0     1492 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/status.py
--rw-r--r--   0        0        0      277 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/__init__.py
--rw-r--r--   0        0        0    24710 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/base_io.py
--rw-r--r--   0        0        0     1553 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/py.typed
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/__init__.py
--rw-r--r--   0        0        0      204 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/abc.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/__init__.py
--rw-r--r--   0        0        0     2001 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/chat.py
--rw-r--r--   0        0        0      709 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/uuid.py
--rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/__init__.py
--rw-r--r--   0        0        0     3415 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/abc.py
--rw-r--r--   0        0        0     4385 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/deprecation.py
--rw-r--r--   0        0        0    14537 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/version_map.py
--rw-r--r--   0        0        0     5879 2023-06-08 15:40:36.504008 mcproto-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    19005 1970-01-01 00:00:00.000000 mcproto-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6328 2023-06-11 18:36:44.066709 mcproto-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2927 2023-06-11 18:36:44.066709 mcproto-0.4.0/LICENSE-THIRD-PARTY.txt
+-rw-r--r--   0        0        0     7651 2023-06-11 18:36:44.066709 mcproto-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0    17244 2023-06-11 18:36:44.066709 mcproto-0.4.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.066709 mcproto-0.4.0/mcproto/__init__.py
+-rw-r--r--   0        0        0     3211 2023-06-11 18:36:44.066709 mcproto-0.4.0/mcproto/buffer.py
+-rw-r--r--   0        0        0    12532 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/connection.py
+-rw-r--r--   0        0        0      565 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/handshaking/__init__.py
+-rw-r--r--   0        0        0     2218 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/handshaking/handshake.py
+-rw-r--r--   0        0        0     3435 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/interactions.py
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/login/__init__.py
+-rw-r--r--   0        0        0     7917 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/login/login.py
+-rw-r--r--   0        0        0     1028 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/packet.py
+-rw-r--r--   0        0        0     5158 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/packet_map.py
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/status/__init__.py
+-rw-r--r--   0        0        0     1153 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/status/ping.py
+-rw-r--r--   0        0        0     1495 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/packets/status/status.py
+-rw-r--r--   0        0        0      277 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/protocol/__init__.py
+-rw-r--r--   0        0        0    24710 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/protocol/base_io.py
+-rw-r--r--   0        0        0     1553 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/protocol/utils.py
+-rw-r--r--   0        0        0        0 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/py.typed
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/types/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/types/abc.py
+-rw-r--r--   0        0        0     2001 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/types/chat.py
+-rw-r--r--   0        0        0      709 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/types/uuid.py
+-rw-r--r--   0        0        0       35 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/utils/__init__.py
+-rw-r--r--   0        0        0     3415 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/utils/abc.py
+-rw-r--r--   0        0        0     4385 2023-06-11 18:36:44.070710 mcproto-0.4.0/mcproto/utils/deprecation.py
+-rw-r--r--   0        0        0     5736 2023-06-11 18:36:56.426940 mcproto-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18633 1970-01-01 00:00:00.000000 mcproto-0.4.0/PKG-INFO
```

### Comparing `mcproto-0.3.0/LICENSE-THIRD-PARTY.txt` & `mcproto-0.4.0/LICENSE-THIRD-PARTY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 SOFTWARE.
 
 ---------------------------------------------------------------------------------------------------
                                  GNU LESSER GENERAL PUBLIC LICENSE
 Applies to:
     - Copyright (c) 2022, Milo Weinberg <iapetus011@gmail.com>
       All rights reserved.
-        - mcproto/packets/abc.py: GameState and PacketDirection enum classes
+        - mcproto/packets/packet.py: GameState and PacketDirection enum classes
 ---------------------------------------------------------------------------------------------------
 Fulltext of the license can be seen in the LICENSE.txt file, as it matches the current license of
 this project, this file just disclaims the copyrighted sections used in our codebase.
```

### Comparing `mcproto-0.3.0/LICENSE.txt` & `mcproto-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/README.md` & `mcproto-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -182,93 +182,80 @@
 def start():
     # Just some boilerplate code that can run our asynchronous main function
     asyncio.run(main())
 ```
 
 ### Using packet classes for communication
 
+The first thing you'll need to understand about packet classes in mcproto is that they're generally going to support
+the latest minecraft version, and while any the versions are usually mostly compatible, mcproto does NOT guarantee
+support for any older protocol versions.
+
 #### Obtaining the packet map
 
-The first thing you'll need to understand about packet classes in mcproto is that they're versioned depending on the
-protocol version you're using. As we've already seen with minecraft packets, they're following a certain format, and
-for given packet direction and game state, the packet numbers are unique.
-
-This is how we can detect what packet is being received, but because of the different versions that the library can
-support, we will need to use a packet map, that will contain all of the mappings for given protocol version, from
-which, knowing the state and direction, we can get a dictionary with packet IDs as keys, and the individual packet
-classes as values.
-
-This dictionary is crucial to receiving packets, as it's the only thing that tells us which packet class should be
-used, once we receive a packet and learn about the packet id. Otherwise we wouldn't know what to do with the data we
-obtained.
-
-The first game state we'll be in, before doing anything will always be the handshaking state, so let's see how we could
-generate this dictionary for this state, for all of the receiving (client bound) packets.
-
-```python
-from mcproto.packets import PACKET_MAP
-from mcproto.packets.abc import PacketDirection, GameState
-
-handshaking_packet_map = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.HANDSHAKING
-)
+As we've already seen in the example before, packets follow certain format, and every packet has it's associated ID
+number, direction (client->server or server->client), and game state (status/handshaking/login/play). The packet IDs
+are unique to given direction and game state combination.
 
-print(handshaking_packet_map)  # {}
-```
+For example in clientbound direction (packets sent from server to the client), when in the status game state, there
+will always be unique ID numbers for the different packets. In this case, there would actually only be 2 packets here:
+The Ping response packet, which has an ID of 1, and the Status response packet, with an ID of 0.
 
-Notice that the packet map is actually empty, and this is simply because there (currently) aren't any client bound
-packets a server can send out for the handshaking game state. Let's see the status gamestate instead:
+To receive a packet, we therefore need to know both the game state, and the direction, as only then are we able to
+figure out what the type of packet it is. In mcproto, packet receiving therefore requires a "packet map", which is a
+mapping (dictionary) of packet id -> packet class. Here's an example of obtaining a packet map:
 
 ```python
-status_packet_map = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS,
-)
+from mcproto.packets import generate_packet_map, GameState, PacketDirection
 
-print(status_packet_map)  # Will print:
-# {1: mcproto.packets.v757.status.ping.PingPong, 0: mcproto.packets.v757.status.status.StatusResponse}
+STATUS_CLIENTBOUND_MAP = generate_packet_map(PacketDirection.CLIENTBOUND, GameState.STATUS)
 ```
 
-Cool! These are all of the packets, with their IDs that the server can send in STATUS game state.
+Which, if you were to print it, would look like this:
+
+```
+{
+    0: <class 'mcproto.packets.status.status.StatusResponse'>
+    1: <class 'mcproto.packets.status.ping.PingPong'>,
+}
+```
 
-#### Creating our own packets
+Telling us that in the status gamestate, for the clientbound direction, these are the only packet we can receive,
+and showing us the actual packet classes for every possible ID number.
 
+#### Building our own packets
 
-Now, we could create a similar packet map for sending out the packets, and just use it to construct our packets,
-however this is not the recommended approach, as it's kind of hard to remember all of the packet IDs, and (at least
-currently) it means not having any typing information about what packet class will we get. For that reason, it's
-recommended to import packets that we want to send out manually, like so:
+Our first packet will always have to be a Handshake, this is the only packet in the entire handshaking state, and it's
+a "gateway", after which we get moved to a different state, specifically, either to STATUS (to obtain information about
+the server, such as motd, amount of players, or other details you'd see in the multiplayer screen in your MC client).
 
 ```python
-from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
+from mcproto.packets.handshaking.handshake import Handshake, NextState
 
 my_handshake = Handshake(
-    # Once again, we use an old protocol version so that even older servers will work
+    # Once again, we use an old protocol version so that even older servers will respond
     protocol_version=47,
     server_address="mc.hypixel.net",
     server_port=25565,
     next_state=NextState.STATUS,
 )
 ```
 
 That's it! We've now constructed a full handshake packet with all of the data it should contain. You might remember
 from the example above, that we originally had to look at the protocol specification, find the handshake packet and
 construct it's data as a Buffer with all of these variables.
 
-With these packet classes, you can simply follow your editor's function hints to see what this packet requires, pass it
-in and the data will be constructed for you from these attributes, once we'll be to sending it.
+With these packet classes, you can simply follow your editor's autocompletion to see what this packet requires, pass it
+in and the data will be constructed for you from these attributes, without constantly cross-checking with the wiki.
 
 For completion, let's also construct the status request packet that we were sending to instruct the server to send us
 back the status response packet.
 
 ```python
-from mcproto.packets.v757.status.status import StatusRequest
+from mcproto.packets.status.status import StatusRequest
 
 my_status_request = StatusRequest()
 ```
 
 This one was even easier, as the status request packet alone doesn't contain any special data, it's just a request to
 the server to send us some data back.
 
@@ -282,98 +269,89 @@
 from mcproto.connection import TCPAsyncConnection
 
 async def main():
     ip = "mc.hypixel.net"
     port = 25565
 
     async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
-        await async_write_packet(connection, my_handshake)  
+        await async_write_packet(connection, my_handshake)
         # my_handshake is a packet we've created in the example before
 ```
 
-How quick was that? Now compare this to the manual version.
+Much easier than the manual version, isn't it?
 
 #### Receiving packets
 
 Alright, we might now know how to send a packet, but how do we receive one? Let's see:
 
 ```python
-from mcproto.packets import PACKET_MAP
-
-# Let's prepare the packet map we'll be using, say we're already in the STATUS game state now
-STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS
-)
-
 # Let's say we already have a connection at this moment, after all, how else would
 # we've gotten into the STATUS game state.
-# Also, let's do something different, let's say we have a synchronous connection
+# Also, let's do something different, let's say we have a synchronous connection, just for fun
 from mcproto.connection import TCPSyncConnection
 conn: TCPSyncConnection
 
 # With a synchronous connection, comes synchronous reader, so instead of using async_read_packet,
 # we'll use sync_read_packet here
 from mcproto.packets import sync_read_packet
 
-packet = sync_read_packet(conn, STATUS_PACKET_MAP)
-
-# Cool! We've got back a packet, but what packet is it? Let's import the packet classes it could
-# be and check against them
-from mcproto.packets.v757.status.status import StatusResponse
-from mcproto.packets.v757.status.ping import PingPong
+# But remember? To read a packet, we'll need to have that packet map, telling us which IDs represent
+# which actual packet types. Let's pass in the one we've constructed before
+packet = sync_read_packet(conn, STATUS_CLIENTBOUND_MAP)
+
+# Cool! We've got back a packet, let's see what kind of packet we got back
+from mcproto.packets.status.status import StatusResponse
+from mcproto.packets.status.ping import PingPong
 
 if isinstance(packet, StatusResponse):
     ...
 elif isinstance(packet, PingPong):
     ...
 else:
     raise Exception("Impossible, there aren't other client bound packets in the STATUS game state")
 ```
 
 #### Requesting status
 
-Now let's actually do something meaningful, and replicate the entire example from the manual version using packets,
-let's see just how much simpler it will be:
+Alright, so let's actually try to put all of this knowledge together, and create something meaningful. Let's replicate
+the status obtaining logic from the manual example, but with these new packet classes:
 
 ```python
 from mcproto.connection import TCPAsyncConnection
-from mcproto.packets import async_write_packet, async_read_packet, PACKET_MAP
-from mcproto.packets.abc import PacketDirection, GameState
-from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
-from mcproto.packets.v757.status.status import StatusRequest, StatusResponse
-
-STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS
-)
+from mcproto.packets import async_write_packet, async_read_packet, generate_packet_map
+from mcproto.packets.packet import PacketDirection, GameState
+from mcproto.packets.handshaking.handshake import Handshake, NextState
+from mcproto.packets.status.status import StatusRequest, StatusResponse
+from mcproto.packets.status.ping import PingPong
+
+STATUS_CLIENTBOUND_MAP = generate_packet_map(PacketDirection.CLIENTBOUND, GameState.STATUS)
 
 
 async def get_status(ip: str, port: int) -> dict:
     handshake_packet = Handshake(
         protocol_version=47,
         server_address=ip,
         server_port=port,
         next_state=NextState.STATUS,
     )
     status_req_packet = StatusRequest()
 
     async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
         # We start out at HANDSHAKING game state
-        await async_write_packet(connection, handshake_packet)  
+        await async_write_packet(connection, handshake_packet)
         # After sending the handshake, we told the server to now move us into the STATUS game state
-        await async_write_packet(connection, status_req_packet)  
+        await async_write_packet(connection, status_req_packet)
         # Since we're still in STATUS game state, we use the status packet map when reading
-        packet = await async_read_packet(connection, STATUS_PACKET_MAP)
+        packet = await async_read_packet(connection, STATUS_CLIENTBOUND_MAP)
 
     # Now that we've got back the packet, we no longer need the connection, we won't be sending
-    # anything else. Let's just make sure it really is the packet we expected
+    # anything else, so let's get out of the context manager.
+
+    # Now, we should always first make sure it really is the packet we expected
     if not isinstance(packet, StatusResponse):
         raise ValueError(f"We've got an unexpected packet back: {packet!r}")
 
-    # Now that we know we're dealing with a status response, let's get out it's data, and return in
+    # Since we know we really are dealing with a status response, let's get out it's data, and return it
     return packet.data
 ```
 
 Well, that wasn't so hard, was it?
```

### Comparing `mcproto-0.3.0/mcproto/buffer.py` & `mcproto-0.4.0/mcproto/buffer.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/connection.py` & `mcproto-0.4.0/mcproto/connection.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/packets/__init__.py` & `mcproto-0.4.0/mcproto/packets/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from __future__ import annotations
 
-from mcproto.packets.abc import ClientBoundPacket, GameState, Packet, PacketDirection, ServerBoundPacket
-from mcproto.packets.interactions import (
-    PACKET_MAP,
-    async_read_packet,
-    async_write_packet,
-    sync_read_packet,
-    sync_write_packet,
-)
-from mcproto.packets.map import PacketMap
+from mcproto.packets.interactions import async_read_packet, async_write_packet, sync_read_packet, sync_write_packet
+from mcproto.packets.packet import ClientBoundPacket, GameState, Packet, PacketDirection, ServerBoundPacket
+from mcproto.packets.packet_map import generate_packet_map
 
 __all__ = [
     "ClientBoundPacket",
     "GameState",
-    "PACKET_MAP",
     "Packet",
     "PacketDirection",
-    "PacketMap",
     "ServerBoundPacket",
     "async_read_packet",
     "async_write_packet",
     "sync_read_packet",
     "sync_write_packet",
+    "generate_packet_map",
 ]
```

### Comparing `mcproto-0.3.0/mcproto/packets/abc.py` & `mcproto-0.4.0/mcproto/packets/packet.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/packets/interactions.py` & `mcproto-0.4.0/mcproto/packets/interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from __future__ import annotations
 
 import gzip
 from collections.abc import Mapping
 from typing import TypeVar
 
 from mcproto.buffer import Buffer
-from mcproto.packets.abc import Packet
-from mcproto.packets.map import PacketMap
+from mcproto.packets.packet import Packet
 from mcproto.protocol.base_io import BaseAsyncReader, BaseAsyncWriter, BaseSyncReader, BaseSyncWriter
 
-__all__ = ["async_read_packet", "async_write_packet", "sync_read_packet", "sync_write_packet", "PACKET_MAP"]
+__all__ = ["async_read_packet", "async_write_packet", "sync_read_packet", "sync_write_packet"]
 
 T_Packet = TypeVar("T_Packet", bound=Packet)
 
 # PACKET FORMAT:
 # | Field name  | Field type    | Notes                                 |
 # |-------------|---------------|---------------------------------------|
 # | Length      | 32-bit varint | Length (in bytes) of PacketID + Data  |
 # | Packet ID   | 32-bit varint |                                       |
 # | Data        | byte array    | Internal data to packet of given id   |
 
 
 # Since the read functions here require PACKET_MAP, we can't move these functions
 # directly into BaseWriter/BaseReader classes, as that would be a circular import
 
-PACKET_MAP = PacketMap()
-
 
 def _serialize_packet(packet: Packet, *, compressed: bool = False) -> Buffer:
     """Serialize the internal packet data, along with it's packet id."""
     packet_data = packet.serialize()
 
     # Base packet buffer should only contain packet id and internal packet data
     packet_buf = Buffer()
```

### Comparing `mcproto-0.3.0/mcproto/packets/v757/handshaking/handshake.py` & `mcproto-0.4.0/mcproto/packets/handshaking/handshake.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from enum import IntEnum
 from typing import ClassVar, Union, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
-from mcproto.packets.abc import GameState, ServerBoundPacket
+from mcproto.packets.packet import GameState, ServerBoundPacket
 from mcproto.protocol.base_io import StructFormat
 
 __all__ = [
     "NextState",
     "Handshake",
 ]
```

### Comparing `mcproto-0.3.0/mcproto/packets/v757/login/login.py` & `mcproto-0.4.0/mcproto/packets/login/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import ClassVar, Optional, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
-from mcproto.packets.abc import ClientBoundPacket, GameState, ServerBoundPacket
-from mcproto.types.v757.chat import ChatMessage
-from mcproto.types.v757.uuid import UUID
+from mcproto.packets.packet import ClientBoundPacket, GameState, ServerBoundPacket
+from mcproto.types.chat import ChatMessage
+from mcproto.types.uuid import UUID
 
 __all__ = [
     "LoginStart",
     "LoginEncryptionRequest",
     "LoginEncryptionResponse",
     "LoginSuccess",
     "LoginDisconnect",
```

### Comparing `mcproto-0.3.0/mcproto/packets/v757/status/ping.py` & `mcproto-0.4.0/mcproto/packets/status/ping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import ClassVar, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
-from mcproto.packets.abc import ClientBoundPacket, GameState, ServerBoundPacket
+from mcproto.packets.packet import ClientBoundPacket, GameState, ServerBoundPacket
 from mcproto.protocol.base_io import StructFormat
 
 __all__ = ["PingPong"]
 
 
 @final
 class PingPong(ClientBoundPacket, ServerBoundPacket):
```

### Comparing `mcproto-0.3.0/mcproto/packets/v757/status/status.py` & `mcproto-0.4.0/mcproto/packets/status/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 from typing import Any, ClassVar, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
-from mcproto.packets.abc import ClientBoundPacket, GameState, ServerBoundPacket
+from mcproto.packets.packet import ClientBoundPacket, GameState, ServerBoundPacket
 
 __all__ = ["StatusRequest", "StatusResponse"]
 
 
 @final
 class StatusRequest(ServerBoundPacket):
     """Request from the client to get information on the server. (Client -> Server)"""
```

### Comparing `mcproto-0.3.0/mcproto/protocol/base_io.py` & `mcproto-0.4.0/mcproto/protocol/base_io.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/protocol/utils.py` & `mcproto-0.4.0/mcproto/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/types/v757/chat.py` & `mcproto-0.4.0/mcproto/types/chat.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/types/v757/uuid.py` & `mcproto-0.4.0/mcproto/types/uuid.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/utils/abc.py` & `mcproto-0.4.0/mcproto/utils/abc.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/mcproto/utils/deprecation.py` & `mcproto-0.4.0/mcproto/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.3.0/pyproject.toml` & `mcproto-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mcproto"
-version = "0.3.0" # Versioning handled by poetry-dynamic-versioning
+version = "0.4.0" # Versioning handled by poetry-dynamic-versioning
 description = "Library providing easy interactions with minecraft servers"
 authors = ["ItsDrike <itsdrike@protonmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/py-mine/mcproto"
 documentation = "https://mcproto.readthedocs.io/"
 classifiers = [
@@ -65,27 +65,27 @@
 pep8-naming = "^0.13.3"
 black = ">=22.3,<24.0"
 isort = "^5.10.1"
 pyright = "^1.1.313"
 slotscheck = "^0.16.1"
 
 [tool.poetry.group.release.dependencies]
-towncrier = "^22.12.0"
+towncrier = ">=22.12,<24.0"
 
 [tool.poetry.group.release-ci]
 optional = true
 
 [tool.poetry.group.release-ci.dependencies]
 poetry-dynamic-versioning = "^0.22.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.2.1"
+sphinx = ">=6.2.1,<8.0.0"
 tomli = { version = "^2.0.1", python = "<3.11" }
 m2r2 = "^0.3.3.post2"
 packaging = "^23.1"
 sphinx-autodoc-typehints = "^1.23"
 sphinx-copybutton = "^0.5.2"
 furo = ">=2022.12.7"
 sphinxcontrib-towncrier = "^0.3.2a0"
@@ -104,18 +104,14 @@
 profile = "black"
 line_length = 119
 atomic = true
 order_by_type = false
 case_sensitive = true
 combine_as_imports = true
 
-[tool.codespell]
-skip = "./.venv/*,./htmlcov/*,./.git,./.mypy_cache/*,./.pytest_cache/*,./poetry.lock"
-ignore-words-list = "ned"
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 asyncio_mode = "auto"
 testpaths = ["tests"]
 addopts = "--strict-markers --cov --no-cov-on-fail"
 
 [tool.coverage.report]
@@ -176,15 +172,14 @@
 [tool.taskipy.tasks]
 precommit = "pre-commit install"
 lint = "pre-commit run --all-files"
 black = "black ."
 isort = "isort ."
 pyright = "pyright ."
 flake8 = "flake8 ."
-codespell = "codespell ."
 slotscheck = "slotscheck -m mcproto"
 test = "pytest -v --failed-first"
 retest = "pytest -v --last-failed"
 test-nocov = "pytest -v --no-cov --failed-first"
 retest-nocov = "pytest -v --no-cov --last-failed"
 changelog-preview = "towncrier build --draft --version next"
 docs = "sphinx-build -b dirhtml -d ./docs/_build/doctrees -W -E -T --keep-going ./docs ./docs/_build/html"
```

### Comparing `mcproto-0.3.0/PKG-INFO` & `mcproto-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcproto
-Version: 0.3.0
+Version: 0.4.0
 Summary: Library providing easy interactions with minecraft servers
 Home-page: https://github.com/py-mine/mcproto
 License: LGPL-3.0-or-later
 Author: ItsDrike
 Author-email: itsdrike@protonmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -214,93 +214,80 @@
 def start():
     # Just some boilerplate code that can run our asynchronous main function
     asyncio.run(main())
 ```
 
 ### Using packet classes for communication
 
-#### Obtaining the packet map
+The first thing you'll need to understand about packet classes in mcproto is that they're generally going to support
+the latest minecraft version, and while any the versions are usually mostly compatible, mcproto does NOT guarantee
+support for any older protocol versions.
 
-The first thing you'll need to understand about packet classes in mcproto is that they're versioned depending on the
-protocol version you're using. As we've already seen with minecraft packets, they're following a certain format, and
-for given packet direction and game state, the packet numbers are unique.
-
-This is how we can detect what packet is being received, but because of the different versions that the library can
-support, we will need to use a packet map, that will contain all of the mappings for given protocol version, from
-which, knowing the state and direction, we can get a dictionary with packet IDs as keys, and the individual packet
-classes as values.
-
-This dictionary is crucial to receiving packets, as it's the only thing that tells us which packet class should be
-used, once we receive a packet and learn about the packet id. Otherwise we wouldn't know what to do with the data we
-obtained.
+#### Obtaining the packet map
 
-The first game state we'll be in, before doing anything will always be the handshaking state, so let's see how we could
-generate this dictionary for this state, for all of the receiving (client bound) packets.
+As we've already seen in the example before, packets follow certain format, and every packet has it's associated ID
+number, direction (client->server or server->client), and game state (status/handshaking/login/play). The packet IDs
+are unique to given direction and game state combination.
+
+For example in clientbound direction (packets sent from server to the client), when in the status game state, there
+will always be unique ID numbers for the different packets. In this case, there would actually only be 2 packets here:
+The Ping response packet, which has an ID of 1, and the Status response packet, with an ID of 0.
+
+To receive a packet, we therefore need to know both the game state, and the direction, as only then are we able to
+figure out what the type of packet it is. In mcproto, packet receiving therefore requires a "packet map", which is a
+mapping (dictionary) of packet id -> packet class. Here's an example of obtaining a packet map:
 
 ```python
-from mcproto.packets import PACKET_MAP
-from mcproto.packets.abc import PacketDirection, GameState
-
-handshaking_packet_map = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.HANDSHAKING
-)
+from mcproto.packets import generate_packet_map, GameState, PacketDirection
 
-print(handshaking_packet_map)  # {}
+STATUS_CLIENTBOUND_MAP = generate_packet_map(PacketDirection.CLIENTBOUND, GameState.STATUS)
 ```
 
-Notice that the packet map is actually empty, and this is simply because there (currently) aren't any client bound
-packets a server can send out for the handshaking game state. Let's see the status gamestate instead:
+Which, if you were to print it, would look like this:
 
-```python
-status_packet_map = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS,
-)
-
-print(status_packet_map)  # Will print:
-# {1: mcproto.packets.v757.status.ping.PingPong, 0: mcproto.packets.v757.status.status.StatusResponse}
+```
+{
+    0: <class 'mcproto.packets.status.status.StatusResponse'>
+    1: <class 'mcproto.packets.status.ping.PingPong'>,
+}
 ```
 
-Cool! These are all of the packets, with their IDs that the server can send in STATUS game state.
-
-#### Creating our own packets
+Telling us that in the status gamestate, for the clientbound direction, these are the only packet we can receive,
+and showing us the actual packet classes for every possible ID number.
 
+#### Building our own packets
 
-Now, we could create a similar packet map for sending out the packets, and just use it to construct our packets,
-however this is not the recommended approach, as it's kind of hard to remember all of the packet IDs, and (at least
-currently) it means not having any typing information about what packet class will we get. For that reason, it's
-recommended to import packets that we want to send out manually, like so:
+Our first packet will always have to be a Handshake, this is the only packet in the entire handshaking state, and it's
+a "gateway", after which we get moved to a different state, specifically, either to STATUS (to obtain information about
+the server, such as motd, amount of players, or other details you'd see in the multiplayer screen in your MC client).
 
 ```python
-from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
+from mcproto.packets.handshaking.handshake import Handshake, NextState
 
 my_handshake = Handshake(
-    # Once again, we use an old protocol version so that even older servers will work
+    # Once again, we use an old protocol version so that even older servers will respond
     protocol_version=47,
     server_address="mc.hypixel.net",
     server_port=25565,
     next_state=NextState.STATUS,
 )
 ```
 
 That's it! We've now constructed a full handshake packet with all of the data it should contain. You might remember
 from the example above, that we originally had to look at the protocol specification, find the handshake packet and
 construct it's data as a Buffer with all of these variables.
 
-With these packet classes, you can simply follow your editor's function hints to see what this packet requires, pass it
-in and the data will be constructed for you from these attributes, once we'll be to sending it.
+With these packet classes, you can simply follow your editor's autocompletion to see what this packet requires, pass it
+in and the data will be constructed for you from these attributes, without constantly cross-checking with the wiki.
 
 For completion, let's also construct the status request packet that we were sending to instruct the server to send us
 back the status response packet.
 
 ```python
-from mcproto.packets.v757.status.status import StatusRequest
+from mcproto.packets.status.status import StatusRequest
 
 my_status_request = StatusRequest()
 ```
 
 This one was even easier, as the status request packet alone doesn't contain any special data, it's just a request to
 the server to send us some data back.
 
@@ -314,99 +301,90 @@
 from mcproto.connection import TCPAsyncConnection
 
 async def main():
     ip = "mc.hypixel.net"
     port = 25565
 
     async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
-        await async_write_packet(connection, my_handshake)  
+        await async_write_packet(connection, my_handshake)
         # my_handshake is a packet we've created in the example before
 ```
 
-How quick was that? Now compare this to the manual version.
+Much easier than the manual version, isn't it?
 
 #### Receiving packets
 
 Alright, we might now know how to send a packet, but how do we receive one? Let's see:
 
 ```python
-from mcproto.packets import PACKET_MAP
-
-# Let's prepare the packet map we'll be using, say we're already in the STATUS game state now
-STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS
-)
-
 # Let's say we already have a connection at this moment, after all, how else would
 # we've gotten into the STATUS game state.
-# Also, let's do something different, let's say we have a synchronous connection
+# Also, let's do something different, let's say we have a synchronous connection, just for fun
 from mcproto.connection import TCPSyncConnection
 conn: TCPSyncConnection
 
 # With a synchronous connection, comes synchronous reader, so instead of using async_read_packet,
 # we'll use sync_read_packet here
 from mcproto.packets import sync_read_packet
 
-packet = sync_read_packet(conn, STATUS_PACKET_MAP)
-
-# Cool! We've got back a packet, but what packet is it? Let's import the packet classes it could
-# be and check against them
-from mcproto.packets.v757.status.status import StatusResponse
-from mcproto.packets.v757.status.ping import PingPong
+# But remember? To read a packet, we'll need to have that packet map, telling us which IDs represent
+# which actual packet types. Let's pass in the one we've constructed before
+packet = sync_read_packet(conn, STATUS_CLIENTBOUND_MAP)
+
+# Cool! We've got back a packet, let's see what kind of packet we got back
+from mcproto.packets.status.status import StatusResponse
+from mcproto.packets.status.ping import PingPong
 
 if isinstance(packet, StatusResponse):
     ...
 elif isinstance(packet, PingPong):
     ...
 else:
     raise Exception("Impossible, there aren't other client bound packets in the STATUS game state")
 ```
 
 #### Requesting status
 
-Now let's actually do something meaningful, and replicate the entire example from the manual version using packets,
-let's see just how much simpler it will be:
+Alright, so let's actually try to put all of this knowledge together, and create something meaningful. Let's replicate
+the status obtaining logic from the manual example, but with these new packet classes:
 
 ```python
 from mcproto.connection import TCPAsyncConnection
-from mcproto.packets import async_write_packet, async_read_packet, PACKET_MAP
-from mcproto.packets.abc import PacketDirection, GameState
-from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
-from mcproto.packets.v757.status.status import StatusRequest, StatusResponse
-
-STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
-    protocol_version=757,
-    direction=PacketDirection.CLIENTBOUND,
-    game_state=GameState.STATUS
-)
+from mcproto.packets import async_write_packet, async_read_packet, generate_packet_map
+from mcproto.packets.packet import PacketDirection, GameState
+from mcproto.packets.handshaking.handshake import Handshake, NextState
+from mcproto.packets.status.status import StatusRequest, StatusResponse
+from mcproto.packets.status.ping import PingPong
+
+STATUS_CLIENTBOUND_MAP = generate_packet_map(PacketDirection.CLIENTBOUND, GameState.STATUS)
 
 
 async def get_status(ip: str, port: int) -> dict:
     handshake_packet = Handshake(
         protocol_version=47,
         server_address=ip,
         server_port=port,
         next_state=NextState.STATUS,
     )
     status_req_packet = StatusRequest()
 
     async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
         # We start out at HANDSHAKING game state
-        await async_write_packet(connection, handshake_packet)  
+        await async_write_packet(connection, handshake_packet)
         # After sending the handshake, we told the server to now move us into the STATUS game state
-        await async_write_packet(connection, status_req_packet)  
+        await async_write_packet(connection, status_req_packet)
         # Since we're still in STATUS game state, we use the status packet map when reading
-        packet = await async_read_packet(connection, STATUS_PACKET_MAP)
+        packet = await async_read_packet(connection, STATUS_CLIENTBOUND_MAP)
 
     # Now that we've got back the packet, we no longer need the connection, we won't be sending
-    # anything else. Let's just make sure it really is the packet we expected
+    # anything else, so let's get out of the context manager.
+
+    # Now, we should always first make sure it really is the packet we expected
     if not isinstance(packet, StatusResponse):
         raise ValueError(f"We've got an unexpected packet back: {packet!r}")
 
-    # Now that we know we're dealing with a status response, let's get out it's data, and return in
+    # Since we know we really are dealing with a status response, let's get out it's data, and return it
     return packet.data
 ```
 
 Well, that wasn't so hard, was it?
```

