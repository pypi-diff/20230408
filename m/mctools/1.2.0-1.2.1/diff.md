# Comparing `tmp/mctools-1.2.0.tar.gz` & `tmp/mctools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctools-1.2.0.tar", last modified: Tue Aug 16 01:48:08 2022, max compression
+gzip compressed data, was "mctools-1.2.1.tar", last modified: Sat Apr  8 20:11:14 2023, max compression
```

## Comparing `mctools-1.2.0.tar` & `mctools-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 01:48:08.531345 mctools-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-16 01:47:58.000000 mctools-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-16 01:47:58.000000 mctools-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9922 2022-08-16 01:48:08.531345 mctools-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-08-16 01:47:58.000000 mctools-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-16 01:47:58.000000 mctools-1.2.0/mcli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 01:48:08.531345 mctools-1.2.0/mctools/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15992 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    23391 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/formattertools.py
--rw-r--r--   0 runner    (1001) docker     (121)    32173 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/mclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     8832 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)    10184 2022-08-16 01:47:58.000000 mctools-1.2.0/mctools/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 01:48:08.531345 mctools-1.2.0/mctools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9922 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-16 01:48:08.000000 mctools-1.2.0/mctools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 01:48:08.531345 mctools-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8517 2022-08-16 01:47:58.000000 mctools-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.235259 mctools-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 20:10:58.000000 mctools-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 20:10:58.000000 mctools-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-04-08 20:11:14.235259 mctools-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-08 20:10:58.000000 mctools-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 20:10:58.000000 mctools-1.2.1/mcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.231259 mctools-1.2.1/mctools/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/formattertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32274 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/mclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-08 20:10:58.000000 mctools-1.2.1/mctools/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:11:14.235259 mctools-1.2.1/mctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 20:11:14.000000 mctools-1.2.1/mctools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:11:14.235259 mctools-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-04-08 20:10:58.000000 mctools-1.2.1/setup.py
```

### Comparing `mctools-1.2.0/LICENSE` & `mctools-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/PKG-INFO` & `mctools-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctools
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python implementations of common Minecraft protocols.
 Home-page: https://github.com/Owen-Cochell/mctools
 Author: Owen Cochell
 Author-email: owencochell@hotmail.com
 Project-URL: Bug Reports, https://github.com/Owen-Cochell/mctools/issues
 Project-URL: Source, https://github.com/Owen-Cochell/mctools
 Project-URL: Documentation, https://mctools.readthedocs.io/
@@ -45,14 +45,15 @@
 All of this can be achieved using simple, intuitive calls to mctools. mctools does all the heavy lifting for you!
 Also, mctools has no external dependencies(Unless you are a windows user and need color support),
 and only uses the python standard library. Just download and go!
 
 # Example
 
 Send a command to the Minecraft server via rcon:
+
 ```python
 from mctools import RCONClient  # Import the RCONClient
 
 HOST = 'mc.server.net'  # Hostname of the Minecraft server
 PORT = 1234  # Port number of the RCON server
 
 # Create the RCONClient:
@@ -63,14 +64,15 @@
 
 if rcon.login("password"):
 
     # Send command to RCON - broadcast message to all players:
 
     resp = rcon.command("broadcast Hello RCON!")
 ```
+
  # Installation 
  
  You can install mctools via pip:
 
     $ pip install mctools
 
  If you are a windows user and want color support, then install mctools like so:
@@ -94,39 +96,39 @@
     §6ClearLag: §fAll commands for ClearLag
     §6Essentials: §fAll commands for Essentials
     §6LuckPerms: §fAll commands for LuckPerms
     §6Minecraft: §fAll commands for Minecraft
     §6Vault: §fAll commands for Vault
     §6WorldEdit: §fAll commands for WorldEdit
 
- As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters, 
+ As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters,
  then the output will look like this:
 
     --------- Help: Index (1/40) --------------------
     Use /help [n] to get page n of help.
     Aliases: Lists command aliases
     Bukkit: All commands for Bukkit
     ClearLag: All commands for ClearLag
     Essentials: All commands for Essentials
     LuckPerms: All commands for LuckPerms
     Minecraft: All commands for Minecraft
     Vault: All commands for Vault
     WorldEdit: All commands for WorldEdit
 
  Much easier to read and process. mctools handles this operation automatically, so you don't have to.
- mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the 
+ mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the
  player sample list.
 
- To learn more about formatters, and how to create your own, 
+ To learn more about formatters, and how to create your own,
  then please check out the [formatting documentation](https://mctools.readthedocs.io/en/latest/format.html).
 
  # MCLI - mctools Command Line Interface
 
  mctools is shipped with a CLI front end called mcli, which you can use to start rcon sessions, get stats
- via query/ping, check if a Minecraft server is up, ect. 
+ via query/ping, check if a Minecraft server is up, ect.
 
  After installing mctools(through pip or setuptools), you can invoke mcli like so:
  
     $ mcli --help
 
  You can also run mcli.py(which is located in the parent directory) if you downloaded the source code and did not
  install via pip/setuptools.
@@ -161,14 +163,26 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+## 1.2.1
+
+We now correctly disable length checking in RCONClient if specified by the user.
+
+The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
+This change applies to all clients, as they all use this method.
+
+Added a 'DEFAULT_TIMEOUT' constant and moved some protocol attributes to BaseProtocol to prevent redundancy.
+Protocol objects now init the parent BaseProtocol object.
+
+Fixed some spelling errors, added more type hinting, made some more minor changes to the documentation.
+
 ## 1.2.0
 
  Clients (of any type!) can now be started after being stopped,
  so creating a new client after stopping it is no longer necessary.
 
  The PINGClient will now auto stop itself after each operation.
 
@@ -203,15 +217,15 @@
   
  - Fixed RCON packet fragmentation issue, mctools should now properly detect and handle RCON packet fragmentation
  - Fixed bug where PINGFormatter was looking for 'dark_grey' instead of 'dark_gray'
  - Fixed bug where ChatObjectFormatter did not properly parse ChatObjects
  - We now raise an exception if the RCON write data is too big, instead of leaving the connection in a unstable state
     
   ### Features Added:
-  
+
  - Users can now specify the format method on a per-call basis
  - Users can change the timeout value after the object is instantiated
  - The RCON login check feature can be disabled, meaning that you can attempt to send packets
  even if you are not authenticated
  - Clients can now return raw packets
  - RCON now has custom exceptions
```

### Comparing `mctools-1.2.0/README.md` & `mctools-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 All of this can be achieved using simple, intuitive calls to mctools. mctools does all the heavy lifting for you!
 Also, mctools has no external dependencies(Unless you are a windows user and need color support),
 and only uses the python standard library. Just download and go!
 
 # Example
 
 Send a command to the Minecraft server via rcon:
+
 ```python
 from mctools import RCONClient  # Import the RCONClient
 
 HOST = 'mc.server.net'  # Hostname of the Minecraft server
 PORT = 1234  # Port number of the RCON server
 
 # Create the RCONClient:
@@ -38,14 +39,15 @@
 
 if rcon.login("password"):
 
     # Send command to RCON - broadcast message to all players:
 
     resp = rcon.command("broadcast Hello RCON!")
 ```
+
  # Installation 
  
  You can install mctools via pip:
 
     $ pip install mctools
 
  If you are a windows user and want color support, then install mctools like so:
@@ -69,39 +71,39 @@
     §6ClearLag: §fAll commands for ClearLag
     §6Essentials: §fAll commands for Essentials
     §6LuckPerms: §fAll commands for LuckPerms
     §6Minecraft: §fAll commands for Minecraft
     §6Vault: §fAll commands for Vault
     §6WorldEdit: §fAll commands for WorldEdit
 
- As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters, 
+ As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters,
  then the output will look like this:
 
     --------- Help: Index (1/40) --------------------
     Use /help [n] to get page n of help.
     Aliases: Lists command aliases
     Bukkit: All commands for Bukkit
     ClearLag: All commands for ClearLag
     Essentials: All commands for Essentials
     LuckPerms: All commands for LuckPerms
     Minecraft: All commands for Minecraft
     Vault: All commands for Vault
     WorldEdit: All commands for WorldEdit
 
  Much easier to read and process. mctools handles this operation automatically, so you don't have to.
- mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the 
+ mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the
  player sample list.
 
- To learn more about formatters, and how to create your own, 
+ To learn more about formatters, and how to create your own,
  then please check out the [formatting documentation](https://mctools.readthedocs.io/en/latest/format.html).
 
  # MCLI - mctools Command Line Interface
 
  mctools is shipped with a CLI front end called mcli, which you can use to start rcon sessions, get stats
- via query/ping, check if a Minecraft server is up, ect. 
+ via query/ping, check if a Minecraft server is up, ect.
 
  After installing mctools(through pip or setuptools), you can invoke mcli like so:
  
     $ mcli --help
 
  You can also run mcli.py(which is located in the parent directory) if you downloaded the source code and did not
  install via pip/setuptools.
@@ -136,14 +138,26 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+## 1.2.1
+
+We now correctly disable length checking in RCONClient if specified by the user.
+
+The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
+This change applies to all clients, as they all use this method.
+
+Added a 'DEFAULT_TIMEOUT' constant and moved some protocol attributes to BaseProtocol to prevent redundancy.
+Protocol objects now init the parent BaseProtocol object.
+
+Fixed some spelling errors, added more type hinting, made some more minor changes to the documentation.
+
 ## 1.2.0
 
  Clients (of any type!) can now be started after being stopped,
  so creating a new client after stopping it is no longer necessary.
 
  The PINGClient will now auto stop itself after each operation.
 
@@ -178,15 +192,15 @@
   
  - Fixed RCON packet fragmentation issue, mctools should now properly detect and handle RCON packet fragmentation
  - Fixed bug where PINGFormatter was looking for 'dark_grey' instead of 'dark_gray'
  - Fixed bug where ChatObjectFormatter did not properly parse ChatObjects
  - We now raise an exception if the RCON write data is too big, instead of leaving the connection in a unstable state
     
   ### Features Added:
-  
+
  - Users can now specify the format method on a per-call basis
  - Users can change the timeout value after the object is instantiated
  - The RCON login check feature can be disabled, meaning that you can attempt to send packets
  even if you are not authenticated
  - Clients can now return raw packets
  - RCON now has custom exceptions
  
@@ -217,8 +231,8 @@
  The documentation has been updated to reflect these changes.
 
  # Conclusion
 
  mctools offers a pythonic, reliable way to interact with Minecraft servers, without being too complicated.
  Please check the documentation for more information. More features (hopefully) coming soon!
 
- Thank you for reading!
+ Thank you for reading!
```

### Comparing `mctools-1.2.0/mctools/__main__.py` & `mctools-1.2.1/mctools/__main__.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/mctools/encoding.py` & `mctools-1.2.1/mctools/encoding.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/mctools/errors.py` & `mctools-1.2.1/mctools/errors.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/mctools/formattertools.py` & `mctools-1.2.1/mctools/formattertools.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/mctools/mclient.py` & `mctools-1.2.1/mctools/mclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 
 import time
 
 from typing import Union
 
-from mctools.protocol import BaseProtocol, RCONProtocol, QUERYProtocol, PINGProtocol
+from mctools.protocol import BaseProtocol, RCONProtocol, QUERYProtocol, PINGProtocol, DEFAULT_TIMEOUT
 from mctools.packet import RCONPacket, QUERYPacket, PINGPacket
 from mctools.formattertools import BaseFormatter, FormatterCollection, DefaultFormatter, QUERYFormatter, PINGFormatter
 from mctools.errors import RCONAuthenticationError, RCONMalformedPacketError
 
 
 class BaseClient(object):
 
@@ -171,15 +171,15 @@
     :type reqid: int
     :param format_method: Format method to use. You should specify this using the Client constants
     :param format_method: int
     :param timeout: Sets the timeout value for socket operations
     :type timeout: int
     """
 
-    def __init__(self, host, port=25575, reqid=None, format_method=BaseClient.REPLACE, timeout=60):
+    def __init__(self, host, port=25575, reqid=None, format_method=BaseClient.REPLACE, timeout=DEFAULT_TIMEOUT):
 
         self.proto: RCONProtocol = RCONProtocol(host, port, timeout)  # RCONProtocol, used for communicating with RCON server
         self.formatters: FormatterCollection = FormatterCollection()  # Formatters instance, formats text from server
         self.auth = False  # Value determining if we are authenticated
         self.format = format_method  # Value determining how to format output
 
         self.reqid = self.gen_reqid() if reqid is None else int(reqid)  # Generating a request ID
@@ -342,15 +342,15 @@
 
                 pack.payload = pack.payload + temp_pack.payload
 
         # Return our junk:
 
         return pack
 
-    def login(self, password):
+    def login(self, password) -> bool:
         """
         Authenticates with the RCON server using the given password.
         If we are already authenticated, then we simply return True.
 
         :param password: RCON Password
         :type password: str
         :return: True if successful, False if failure
@@ -379,15 +379,15 @@
 
         # Request ID matches!
 
         self.auth = True
 
         return True
 
-    def authenticate(self, password):
+    def authenticate(self, password) -> bool:
         """
         Convenience function, does the same thing that 'login' does, authenticates you with the RCON server.
 
         :param password: Password to authenticate with
         :type password: str
         :return: True if successful, False if failure
         :rtype: bool
@@ -417,22 +417,22 @@
 
             .. warning::
 
                 Disabling fragmentation checks could lead to instability!
                 Do so at your own risk!
 
         :type frag_check: bool
-        :param length_check: Determines if we should check and handel outgoing packet length
+        :param length_check: Determines if we should check and handle outgoing packet length
 
             .. warning::
 
                 Disabling length checks could lead to instability!
                 Do so at your own risk!
     
-        :type legnth_check: bool
+        :type length_check: bool
         :return: Response text from server
         :rtype: str, RCONPacket
         :raises:
             RCONAuthenticationError: If we are not authenticated to the RCON server,
             and authentication checking is enabled. We also raise this if the server refuses to serve us,
             regardless of weather auth checking is enabled.
             RCONMalformedPacketError: If the packet we received is broken or is not the correct packet.
@@ -453,15 +453,15 @@
 
             # Not authenticated, let the user know this:
 
             raise RCONAuthenticationError("Not authenticated to the RCON server!")
 
         # Sending command packet:
 
-        pack = self.raw_send(self.proto.COMMAND, com, frag_check=frag_check)
+        pack = self.raw_send(self.proto.COMMAND, com, frag_check=frag_check, length_check=length_check)
 
         # Get the formatted content:
 
         pack = self._format(pack, com, format_method=format_method)
 
         if return_packet:
 
@@ -548,15 +548,15 @@
     :type reqid: int
     :param format_method: Format method to use. You should specify this using the Client constants
     :type format_method: int
     :param timeout: Sets the timeout value for socket operations
     :type timeout: int
     """
 
-    def __init__(self, host: str, port: int=25565, reqid: int=None, format_method: int=BaseClient.REPLACE, timeout: int=60):
+    def __init__(self, host: str, port: int=25565, reqid: int=None, format_method: int=BaseClient.REPLACE, timeout: int=DEFAULT_TIMEOUT):
 
         self.proto: QUERYProtocol = QUERYProtocol(host, port, timeout)  # Query protocol instance
         self.formatters: FormatterCollection = FormatterCollection()  # Formatters instance
         self.format = format_method  # Format type to use
 
         self.reqid = self.gen_reqid() if reqid is None else int(reqid)
 
@@ -591,15 +591,15 @@
         Determines if we are connected.
         (UPD doesn't really work that way, so we simply return if we have been started).
 
         :return: True if started, False for otherwise.
         :rtype: bool
         """
 
-        return self.proto.started
+        return self.proto.connected
 
     def raw_send(self, reqtype: int, chall: Union[str, None], packet_type: str) -> QUERYPacket:
         """
         Creates a packet from the given arguments and sends it.
         Returns a response.
 
         :param reqtype: Request type
@@ -806,15 +806,15 @@
     :param timeout: Sets the timeout value for socket operations
     :type timeout: int
     :param proto_num: Protocol number to use, can specify which version we are emulating.
                       Defaults to 0, which is the latest.
     :type proto_num: int
     """
 
-    def __init__(self, host: str, port: int=25565, reqid: int=None, format_method: int=BaseClient.REPLACE, timeout: int=60, proto_num: int=0):
+    def __init__(self, host: str, port: int=25565, reqid: int=None, format_method: int=BaseClient.REPLACE, timeout: int=DEFAULT_TIMEOUT, proto_num: int=0):
 
         self.proto: PINGProtocol = PINGProtocol(host, port, timeout)
         self.host = host  # Host of the Minecraft server
         self.port = int(port)  # Port of the Minecraft server
         self.formatters: FormatterCollection = FormatterCollection()  # Formatters method
         self.format = format_method  # Formatting method to use
         self.protonum = proto_num  # Protocol number we are using - 0 means we are using the latest
```

### Comparing `mctools-1.2.0/mctools/packet.py` & `mctools-1.2.1/mctools/packet.py`

 * *Files identical despite different names*

### Comparing `mctools-1.2.0/mctools/protocol.py` & `mctools-1.2.1/mctools/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 import struct
 import socket
 
 from mctools.packet import RCONPacket, QUERYPacket, PINGPacket
 from mctools.encoding import PINGEncoder
 from mctools.errors import RCONCommunicationError, RCONLengthError, ProtoConnectionClosed
 
+# Default timeout:
+DEFAULT_TIMEOUT = 60
+
 
 class BaseProtocol(object):
     """
     Parent Class for protocol implementations.
     Every protocol instance should inherit this class!
     """
 
     def __init__(self) -> None:
         
         # Dummy init, primarily meant to specify the socket parameter:
 
         self.sock: socket.socket
 
+        self.timeout = DEFAULT_TIMEOUT  # Defines and sets the timeout value
+        self.connected = False  # Value determining if we are connected
+
     def start(self):
         """
         Method to start the connection to remote entity.
         This raises a NotImplementedErrorException, as it should be overridden in the child class.
         """
 
         raise NotImplementedError("Override this method in child class!")
@@ -74,14 +80,16 @@
 
         while len(byts) < length:
 
             last = self.sock.recv(length - len(byts))
 
             byts = byts + last
 
+            print(byts)
+
             if last == b'':
 
                 # We received nothing, lets close this connection:
 
                 self.stop()
 
                 # Raise the 'ConnectionClosed' exception:
@@ -123,19 +131,31 @@
 
     def set_timeout(self, timeout):
         """
         Sets the timeout value for the underlying socket object.
 
         :param timeout: Value in seconds to set the timeout to
         :type timeout: int
+
+        .. versionadded:: 1.1.0
+
+        This method now works before the protocol object is started
         """
 
-        # Set the timeout:
+        # First, set the timeout value:
+
+        self.timeout = timeout
 
-        self.sock.settimeout(timeout)
+        # Next, determine if we should set the socket timeout:
+
+        if self.connected:
+
+            # Set the timeout:
+
+            self.sock.settimeout(timeout)
 
     def __del__(self):
         """
         Attempts to close the socket:
         """
 
         try:
@@ -157,22 +177,27 @@
     :type port: int
     :param timeout: Timeout value for socket operations.
     :type timeout: int
     """
 
     def __init__(self, host, port, timeout):
 
+        # Init super class
+        super().__init__()
+
         self.host = host  # Host of the RCON server
         self.port = int(port)  # Port of the RCON server
         self.LOGIN = 3  # Packet type used for logging in
         self.COMMAND = 2  # Packet type for issuing a command
         self.RESPONSE = 0  # Packet type for response
         self.MAX_SIZE = 4096  # Maximum packet size
-        self.connected = False  # Value determining if we are connected
-        self.timeout = timeout  # Global timeout value
+
+        # Finally, set the timeout:
+
+        self.set_timeout(timeout)
 
     def start(self):
         """
         Starts the connection to the RCON server.
         """
 
         if self.connected:
@@ -272,40 +297,47 @@
     :param timeout: Timeout value for socket operations
     :type timeout: int
 
     """
 
     def __init__(self, host, port, timeout):
 
+        # Init super class
+        super().__init__()
+
         self.host = host  # Host of the Query server
         self.port = int(port)  # Port of the Query server
-        self.started = False  # Determining if we have started communicating with the Query server
-        self.timeout = timeout
+
+        # Finally, set the timeout:
+
+        self.set_timeout(timeout)
 
     def start(self):
         """
         Sets the protocol object as ready to communicate.
         """
 
-        self.started = True
-        
         # Create an ip4 UPD socket:
 
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
         # Set the timeout:
-        
+
         self.sock.settimeout(self.timeout)  # Setting timeout value for socket
 
+        # Set our connected status:
+
+        self.connected = True
+
     def stop(self):
         """
         Sets the protocol object as not ready to communicate.
         """
 
-        self.started = False
+        self.connected = False
 
     def send(self, pack):
         """
         Sends a packet to the Query server.
 
         :param pack: Packet to send
         :type pack: QUERYPacket
@@ -348,18 +380,23 @@
     :type port: int
     :param timeout: Timeout value used for socket operations
     :type timeout: int
     """
 
     def __init__(self, host, port, timeout):
 
+        # Init super class
+        super().__init__()
+
         self.host = host  # Host of the Minecraft server
         self.port = int(port)  # Port of the Minecraft server
-        self.connected = False  # Value determining if we are connected
-        self.timeout = timeout
+
+        # Finally, set the timeout:
+
+        self.set_timeout(timeout)
 
     def start(self):
         """
         Starts the connection to the Minecraft server.
         """
 
         # Create an ip4 TCP socket:
```

### Comparing `mctools-1.2.0/mctools.egg-info/PKG-INFO` & `mctools-1.2.1/mctools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctools
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python implementations of common Minecraft protocols.
 Home-page: https://github.com/Owen-Cochell/mctools
 Author: Owen Cochell
 Author-email: owencochell@hotmail.com
 Project-URL: Bug Reports, https://github.com/Owen-Cochell/mctools/issues
 Project-URL: Source, https://github.com/Owen-Cochell/mctools
 Project-URL: Documentation, https://mctools.readthedocs.io/
@@ -45,14 +45,15 @@
 All of this can be achieved using simple, intuitive calls to mctools. mctools does all the heavy lifting for you!
 Also, mctools has no external dependencies(Unless you are a windows user and need color support),
 and only uses the python standard library. Just download and go!
 
 # Example
 
 Send a command to the Minecraft server via rcon:
+
 ```python
 from mctools import RCONClient  # Import the RCONClient
 
 HOST = 'mc.server.net'  # Hostname of the Minecraft server
 PORT = 1234  # Port number of the RCON server
 
 # Create the RCONClient:
@@ -63,14 +64,15 @@
 
 if rcon.login("password"):
 
     # Send command to RCON - broadcast message to all players:
 
     resp = rcon.command("broadcast Hello RCON!")
 ```
+
  # Installation 
  
  You can install mctools via pip:
 
     $ pip install mctools
 
  If you are a windows user and want color support, then install mctools like so:
@@ -94,39 +96,39 @@
     §6ClearLag: §fAll commands for ClearLag
     §6Essentials: §fAll commands for Essentials
     §6LuckPerms: §fAll commands for LuckPerms
     §6Minecraft: §fAll commands for Minecraft
     §6Vault: §fAll commands for Vault
     §6WorldEdit: §fAll commands for WorldEdit
 
- As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters, 
+ As you can see, this text is somewhat hard to read. If you told mctools to remove the formatting characters,
  then the output will look like this:
 
     --------- Help: Index (1/40) --------------------
     Use /help [n] to get page n of help.
     Aliases: Lists command aliases
     Bukkit: All commands for Bukkit
     ClearLag: All commands for ClearLag
     Essentials: All commands for Essentials
     LuckPerms: All commands for LuckPerms
     Minecraft: All commands for Minecraft
     Vault: All commands for Vault
     WorldEdit: All commands for WorldEdit
 
  Much easier to read and process. mctools handles this operation automatically, so you don't have to.
- mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the 
+ mctools also handles situations where content is sent in ChatObject notation, and can extract messages from the
  player sample list.
 
- To learn more about formatters, and how to create your own, 
+ To learn more about formatters, and how to create your own,
  then please check out the [formatting documentation](https://mctools.readthedocs.io/en/latest/format.html).
 
  # MCLI - mctools Command Line Interface
 
  mctools is shipped with a CLI front end called mcli, which you can use to start rcon sessions, get stats
- via query/ping, check if a Minecraft server is up, ect. 
+ via query/ping, check if a Minecraft server is up, ect.
 
  After installing mctools(through pip or setuptools), you can invoke mcli like so:
  
     $ mcli --help
 
  You can also run mcli.py(which is located in the parent directory) if you downloaded the source code and did not
  install via pip/setuptools.
@@ -161,14 +163,26 @@
  way to get it included. Feel free to email me or open an issue if you have any problems.
 
  If you are interested in helping in the development of mctools, then send me an email, and we can get talking!
  Believe me, there is plenty of work that needs to be done. More help would be greatly appreciated!
 
  # Changelog
 
+## 1.2.1
+
+We now correctly disable length checking in RCONClient if specified by the user.
+
+The 'set_timeout()' method in BaseProtocol will now work correctly even if the protocol object is not started.
+This change applies to all clients, as they all use this method.
+
+Added a 'DEFAULT_TIMEOUT' constant and moved some protocol attributes to BaseProtocol to prevent redundancy.
+Protocol objects now init the parent BaseProtocol object.
+
+Fixed some spelling errors, added more type hinting, made some more minor changes to the documentation.
+
 ## 1.2.0
 
  Clients (of any type!) can now be started after being stopped,
  so creating a new client after stopping it is no longer necessary.
 
  The PINGClient will now auto stop itself after each operation.
 
@@ -203,15 +217,15 @@
   
  - Fixed RCON packet fragmentation issue, mctools should now properly detect and handle RCON packet fragmentation
  - Fixed bug where PINGFormatter was looking for 'dark_grey' instead of 'dark_gray'
  - Fixed bug where ChatObjectFormatter did not properly parse ChatObjects
  - We now raise an exception if the RCON write data is too big, instead of leaving the connection in a unstable state
     
   ### Features Added:
-  
+
  - Users can now specify the format method on a per-call basis
  - Users can change the timeout value after the object is instantiated
  - The RCON login check feature can be disabled, meaning that you can attempt to send packets
  even if you are not authenticated
  - Clients can now return raw packets
  - RCON now has custom exceptions
```

### Comparing `mctools-1.2.0/setup.py` & `mctools-1.2.1/setup.py`

 * *Files identical despite different names*

