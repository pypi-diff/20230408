# Comparing `tmp/SignalCliApi-0.1.3.tar.gz` & `tmp/SignalCliApi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SignalCliApi-0.1.3.tar", last modified: Tue Apr  4 12:00:52 2023, max compression
+gzip compressed data, was "SignalCliApi-0.1.4.tar", last modified: Sat Apr  8 16:45:22 2023, max compression
```

## Comparing `SignalCliApi-0.1.3.tar` & `SignalCliApi-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-04 12:00:52.500935 SignalCliApi-0.1.3/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-04 12:00:52.500935 SignalCliApi-0.1.3/PKG-INFO
--rw-rw-r--   0 streak    (1000) streak    (1000)      618 2023-04-03 23:46:50.000000 SignalCliApi-0.1.3/README.md
--rw-rw-r--   0 streak    (1000) streak    (1000)      104 2023-04-03 20:42:22.000000 SignalCliApi-0.1.3/pyproject.toml
--rw-rw-r--   0 streak    (1000) streak    (1000)      638 2023-04-04 12:00:52.504935 SignalCliApi-0.1.3/setup.cfg
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-04 12:00:52.472933 SignalCliApi-0.1.3/src/
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-04 12:00:52.500935 SignalCliApi-0.1.3/src/SignalCliApi/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1166 2023-03-28 15:06:47.000000 SignalCliApi-0.1.3/src/SignalCliApi/__init__.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     9512 2023-03-28 15:06:47.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalAccount.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     5855 2023-03-30 23:44:19.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalAccounts.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6695 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalAttachment.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3691 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalCallMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    22598 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalCli.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7012 2023-04-04 11:59:45.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalCommon.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    11244 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalContact.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    19396 2023-04-04 02:26:27.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalContacts.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6647 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalDevice.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4928 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalDevices.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    16961 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalGroup.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     2297 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalGroupUpdate.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6415 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalGroups.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3505 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalMention.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    11990 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalMentions.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    14927 2023-03-30 23:16:09.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    36318 2023-04-04 11:59:07.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalMessages.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6938 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalPreview.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    20782 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalProfile.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     9333 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalQuote.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    10958 2023-03-28 16:37:40.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalReaction.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7435 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalReactions.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6846 2023-04-04 06:41:59.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalReceipt.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    20080 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalReceiveThread.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    24680 2023-03-31 00:39:14.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalReceivedMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    22908 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalSentMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    15925 2023-03-28 15:06:47.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalSticker.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3901 2023-04-04 06:41:59.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalStoryMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7502 2023-03-28 14:59:03.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalSyncMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3674 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalTextAttachment.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4073 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalThumbnail.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7762 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalTimestamp.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4279 2023-04-04 06:41:58.000000 SignalCliApi-0.1.3/src/SignalCliApi/signalTypingMessage.py
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-04 12:00:52.500935 SignalCliApi-0.1.3/src/SignalCliApi.egg-info/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-04 12:00:52.000000 SignalCliApi-0.1.3/src/SignalCliApi.egg-info/PKG-INFO
--rw-rw-r--   0 streak    (1000) streak    (1000)     1396 2023-04-04 12:00:52.000000 SignalCliApi-0.1.3/src/SignalCliApi.egg-info/SOURCES.txt
--rw-rw-r--   0 streak    (1000) streak    (1000)        1 2023-04-04 12:00:52.000000 SignalCliApi-0.1.3/src/SignalCliApi.egg-info/dependency_links.txt
--rw-rw-r--   0 streak    (1000) streak    (1000)       13 2023-04-04 12:00:52.000000 SignalCliApi-0.1.3/src/SignalCliApi.egg-info/top_level.txt
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 16:45:22.766288 SignalCliApi-0.1.4/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 16:45:22.766288 SignalCliApi-0.1.4/PKG-INFO
+-rw-rw-r--   0 streak    (1000) streak    (1000)      618 2023-04-03 23:46:50.000000 SignalCliApi-0.1.4/README.md
+-rw-rw-r--   0 streak    (1000) streak    (1000)      104 2023-04-03 20:42:22.000000 SignalCliApi-0.1.4/pyproject.toml
+-rw-rw-r--   0 streak    (1000) streak    (1000)      638 2023-04-08 16:45:22.766288 SignalCliApi-0.1.4/setup.cfg
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 16:45:22.706289 SignalCliApi-0.1.4/src/
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 16:45:22.762288 SignalCliApi-0.1.4/src/SignalCliApi/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1166 2023-03-28 15:06:47.000000 SignalCliApi-0.1.4/src/SignalCliApi/__init__.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     9512 2023-03-28 15:06:47.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalAccount.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     5855 2023-03-30 23:44:19.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalAccounts.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6695 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalAttachment.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3691 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalCallMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    22638 2023-04-08 15:04:52.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalCli.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7012 2023-04-04 19:35:53.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalCommon.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    11244 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalContact.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    19396 2023-04-04 02:26:27.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalContacts.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6647 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalDevice.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4928 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalDevices.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    16961 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalGroup.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     2297 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalGroupUpdate.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6415 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalGroups.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3505 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalMention.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    11990 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalMentions.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    14927 2023-03-30 23:16:09.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    36318 2023-04-04 11:59:07.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalMessages.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6938 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalPreview.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    20782 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalProfile.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     9333 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalQuote.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    10958 2023-03-28 16:37:40.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalReaction.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7435 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalReactions.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6844 2023-04-04 19:33:56.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalReceipt.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    20080 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalReceiveThread.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    24680 2023-03-31 00:39:14.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalReceivedMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    22908 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalSentMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    15925 2023-03-28 15:06:47.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalSticker.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3901 2023-04-04 06:41:59.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalStoryMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7502 2023-03-28 14:59:03.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalSyncMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3674 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalTextAttachment.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4073 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalThumbnail.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7762 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalTimestamp.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4279 2023-04-04 06:41:58.000000 SignalCliApi-0.1.4/src/SignalCliApi/signalTypingMessage.py
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 16:45:22.762288 SignalCliApi-0.1.4/src/SignalCliApi.egg-info/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 16:45:22.000000 SignalCliApi-0.1.4/src/SignalCliApi.egg-info/PKG-INFO
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1396 2023-04-08 16:45:22.000000 SignalCliApi-0.1.4/src/SignalCliApi.egg-info/SOURCES.txt
+-rw-rw-r--   0 streak    (1000) streak    (1000)        1 2023-04-08 16:45:22.000000 SignalCliApi-0.1.4/src/SignalCliApi.egg-info/dependency_links.txt
+-rw-rw-r--   0 streak    (1000) streak    (1000)       13 2023-04-08 16:45:22.000000 SignalCliApi-0.1.4/src/SignalCliApi.egg-info/top_level.txt
```

### Comparing `SignalCliApi-0.1.3/PKG-INFO` & `SignalCliApi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SignalCliApi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 Home-page: https://peternearing.ca/signal
 Author: Peter Nearing
 Author-email: me@peternearing.ca
 Project-URL: Docs, https://peternearing.ca/signal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
```

### Comparing `SignalCliApi-0.1.3/README.md` & `SignalCliApi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/setup.cfg` & `SignalCliApi-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SignalCliApi
-version = 0.1.3
+version = 0.1.4
 author = Peter Nearing
 author_email = me@peternearing.ca
 description = A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://peternearing.ca/signal
 project_urls =
```

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/__init__.py` & `SignalCliApi-0.1.4/src/SignalCliApi/__init__.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalAccount.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalAccount.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalAccounts.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalAccounts.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalAttachment.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalAttachment.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalCallMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalCallMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalCli.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalCli.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,26 +90,26 @@
                 # noinspection PyPep8
                 error_message = "socket path '%s' already exists. Perhaps signal is already running." % self._server_address
                 raise FileExistsError(error_message)
 
         # set var to hold main signal process
         self._process: Optional[Popen] = None
         # Set sync socket:
-        self._sync_socket: socket.socket = None
+        self._sync_socket: Optional[socket.socket] = None
         # Set command socket:
-        self._command_socket: socket.socket = None
+        self._command_socket: Optional[socket.socket] = None
         # Set var to hold link process:
         self._link_process: Optional[Popen] = None
         # Set qrencode exec path:
         self._qrencode_exec_path: Optional[str] = find_qrencode()
         # Set external properties and objects:
         # Set accounts:
-        self.accounts: Accounts = None
+        self.accounts: Optional[Accounts] = None
         # Set sticker packs:
-        self.sticker_packs: StickerPacks = None
+        self.sticker_packs: Optional[StickerPacks] = None
 
         # Start signal-cli if requested:
         if start_signal:
             # Build signal-cli command line:
             signal_command_line = [self._signal_exec_path]
             if log_file_path is not None:
                 signal_command_line.extend(['--verbose', '--log-file', log_file_path])
```

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalCommon.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalCommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import select
 import re
 
 DEBUG:bool = False
 ###################
 # Version:
 ###################
-VERSION: str = '0.1.3'
+VERSION: str = '0.1.4'
 ########################################
 # Regex:
 ########################################
 phone_number_regex: Pattern = re.compile(r'(?P<number>\+\d+)')
 uuid_regex: Pattern = re.compile(
     r'(?P<uuid>[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-f0-9]{12})')
```

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalContact.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalContact.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalContacts.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalContacts.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalDevice.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalDevice.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalDevices.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalDevices.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalGroup.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalGroup.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalGroupUpdate.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalGroupUpdate.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalGroups.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalGroups.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalMention.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalMention.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalMentions.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalMentions.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalMessages.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalMessages.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalPreview.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalPreview.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalProfile.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalProfile.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalQuote.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalQuote.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalReaction.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalReaction.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalReactions.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalReactions.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalReceipt.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalReceipt.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         super().__from_raw_message__(raw_message)
         receipt_message: dict[str, object] = raw_message['receiptMessage']
         # Load when:
         self.when = Timestamp(timestamp=receipt_message['when'])
         # Load receipt type:
         if receipt_message['isDelivery']:
             self.receiptType = self.TYPE_DELIVERY
-        elif receipt_message['is_read']:
+        elif receipt_message['isRead']:
             self.receiptType = self.TYPE_READ
-        elif receipt_message['is_viewed']:
+        elif receipt_message['isViewed']:
             self.receiptType = self.TYPE_VIEWED
         else:
             errorMessage = "Unknown receipt type... receiptMessage= %s" % str(receipt_message)
             raise RuntimeError(errorMessage)
         # Load target timestamps:
         self.timestamps = []
         for target_timestamp in receipt_message['timestamps']:
```

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalReceiveThread.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalReceiveThread.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalReceivedMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalReceivedMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalSentMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalSentMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalSticker.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalSticker.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalStoryMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalStoryMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalSyncMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalSyncMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalTextAttachment.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalTextAttachment.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalThumbnail.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalThumbnail.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalTimestamp.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalTimestamp.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi/signalTypingMessage.py` & `SignalCliApi-0.1.4/src/SignalCliApi/signalTypingMessage.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi.egg-info/PKG-INFO` & `SignalCliApi-0.1.4/src/SignalCliApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SignalCliApi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 Home-page: https://peternearing.ca/signal
 Author: Peter Nearing
 Author-email: me@peternearing.ca
 Project-URL: Docs, https://peternearing.ca/signal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
```

### Comparing `SignalCliApi-0.1.3/src/SignalCliApi.egg-info/SOURCES.txt` & `SignalCliApi-0.1.4/src/SignalCliApi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

