# Comparing `tmp/SignalCliApi-0.1.5.tar.gz` & `tmp/SignalCliApi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SignalCliApi-0.1.5.tar", last modified: Sat Apr  8 17:59:32 2023, max compression
+gzip compressed data, was "SignalCliApi-0.1.6.tar", last modified: Sat Apr  8 18:53:39 2023, max compression
```

## Comparing `SignalCliApi-0.1.5.tar` & `SignalCliApi-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 17:59:32.249073 SignalCliApi-0.1.5/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 17:59:32.249073 SignalCliApi-0.1.5/PKG-INFO
--rw-rw-r--   0 streak    (1000) streak    (1000)      618 2023-04-03 23:46:50.000000 SignalCliApi-0.1.5/README.md
--rw-rw-r--   0 streak    (1000) streak    (1000)      104 2023-04-03 20:42:22.000000 SignalCliApi-0.1.5/pyproject.toml
--rw-rw-r--   0 streak    (1000) streak    (1000)      638 2023-04-08 17:59:32.253073 SignalCliApi-0.1.5/setup.cfg
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 17:59:32.213072 SignalCliApi-0.1.5/src/
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 17:59:32.245073 SignalCliApi-0.1.5/src/SignalCliApi/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1166 2023-03-28 15:06:47.000000 SignalCliApi-0.1.5/src/SignalCliApi/__init__.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     9512 2023-03-28 15:06:47.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalAccount.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     5855 2023-03-30 23:44:19.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalAccounts.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6695 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalAttachment.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3691 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalCallMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    22638 2023-04-08 15:04:52.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalCli.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7012 2023-04-08 17:58:55.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalCommon.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    11244 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalContact.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    19396 2023-04-04 02:26:27.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalContacts.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6647 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalDevice.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4928 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalDevices.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    16961 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalGroup.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     2297 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalGroupUpdate.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6415 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalGroups.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3505 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalMention.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    11990 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalMentions.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    14927 2023-03-30 23:16:09.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    36314 2023-04-08 17:56:48.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalMessages.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6938 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalPreview.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    20782 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalProfile.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     9333 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalQuote.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    10958 2023-03-28 16:37:40.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalReaction.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7435 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalReactions.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     6844 2023-04-04 19:33:56.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalReceipt.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    20080 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalReceiveThread.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    24680 2023-03-31 00:39:14.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalReceivedMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    22908 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalSentMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)    15925 2023-03-28 15:06:47.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalSticker.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3901 2023-04-04 06:41:59.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalStoryMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7502 2023-03-28 14:59:03.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalSyncMessage.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     3674 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalTextAttachment.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4073 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalThumbnail.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     7762 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalTimestamp.py
--rw-rw-r--   0 streak    (1000) streak    (1000)     4279 2023-04-04 06:41:58.000000 SignalCliApi-0.1.5/src/SignalCliApi/signalTypingMessage.py
-drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 17:59:32.249073 SignalCliApi-0.1.5/src/SignalCliApi.egg-info/
--rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 17:59:32.000000 SignalCliApi-0.1.5/src/SignalCliApi.egg-info/PKG-INFO
--rw-rw-r--   0 streak    (1000) streak    (1000)     1396 2023-04-08 17:59:32.000000 SignalCliApi-0.1.5/src/SignalCliApi.egg-info/SOURCES.txt
--rw-rw-r--   0 streak    (1000) streak    (1000)        1 2023-04-08 17:59:32.000000 SignalCliApi-0.1.5/src/SignalCliApi.egg-info/dependency_links.txt
--rw-rw-r--   0 streak    (1000) streak    (1000)       13 2023-04-08 17:59:32.000000 SignalCliApi-0.1.5/src/SignalCliApi.egg-info/top_level.txt
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 18:53:39.243920 SignalCliApi-0.1.6/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 18:53:39.243920 SignalCliApi-0.1.6/PKG-INFO
+-rw-rw-r--   0 streak    (1000) streak    (1000)      618 2023-04-03 23:46:50.000000 SignalCliApi-0.1.6/README.md
+-rw-rw-r--   0 streak    (1000) streak    (1000)      104 2023-04-03 20:42:22.000000 SignalCliApi-0.1.6/pyproject.toml
+-rw-rw-r--   0 streak    (1000) streak    (1000)      638 2023-04-08 18:53:39.247920 SignalCliApi-0.1.6/setup.cfg
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 18:53:39.175920 SignalCliApi-0.1.6/src/
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 18:53:39.243920 SignalCliApi-0.1.6/src/SignalCliApi/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1166 2023-03-28 15:06:47.000000 SignalCliApi-0.1.6/src/SignalCliApi/__init__.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     9512 2023-03-28 15:06:47.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalAccount.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     5855 2023-03-30 23:44:19.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalAccounts.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6694 2023-04-08 18:04:38.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalAttachment.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3689 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalCallMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    22638 2023-04-08 15:04:52.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalCli.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7012 2023-04-08 18:52:07.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalCommon.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    11244 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalContact.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    19396 2023-04-04 02:26:27.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalContacts.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6647 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalDevice.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4928 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalDevices.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    16961 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalGroup.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     2297 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalGroupUpdate.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6415 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalGroups.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3503 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalMention.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    11988 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalMentions.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    14997 2023-04-08 18:04:02.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    36314 2023-04-08 17:56:48.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalMessages.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6943 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalPreview.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    20782 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalProfile.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     9333 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalQuote.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    10945 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalReaction.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7435 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalReactions.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     6842 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalReceipt.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    20080 2023-04-04 06:41:58.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalReceiveThread.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    24698 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalReceivedMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    22882 2023-04-08 18:19:49.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalSentMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)    15902 2023-04-08 18:43:54.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalSticker.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     5965 2023-04-08 18:43:54.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalStoryMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     7489 2023-04-08 18:43:54.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalSyncMessage.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     3659 2023-04-08 18:43:54.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalTextAttachment.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4080 2023-04-08 18:43:54.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalThumbnail.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     8300 2023-04-08 18:48:40.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalTimestamp.py
+-rw-rw-r--   0 streak    (1000) streak    (1000)     4275 2023-04-08 18:50:23.000000 SignalCliApi-0.1.6/src/SignalCliApi/signalTypingMessage.py
+drwxrwxr-x   0 streak    (1000) streak    (1000)        0 2023-04-08 18:53:39.243920 SignalCliApi-0.1.6/src/SignalCliApi.egg-info/
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1109 2023-04-08 18:53:39.000000 SignalCliApi-0.1.6/src/SignalCliApi.egg-info/PKG-INFO
+-rw-rw-r--   0 streak    (1000) streak    (1000)     1396 2023-04-08 18:53:39.000000 SignalCliApi-0.1.6/src/SignalCliApi.egg-info/SOURCES.txt
+-rw-rw-r--   0 streak    (1000) streak    (1000)        1 2023-04-08 18:53:39.000000 SignalCliApi-0.1.6/src/SignalCliApi.egg-info/dependency_links.txt
+-rw-rw-r--   0 streak    (1000) streak    (1000)       13 2023-04-08 18:53:39.000000 SignalCliApi-0.1.6/src/SignalCliApi.egg-info/top_level.txt
```

### Comparing `SignalCliApi-0.1.5/PKG-INFO` & `SignalCliApi-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SignalCliApi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 Home-page: https://peternearing.ca/signal
 Author: Peter Nearing
 Author-email: me@peternearing.ca
 Project-URL: Docs, https://peternearing.ca/signal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
```

### Comparing `SignalCliApi-0.1.5/README.md` & `SignalCliApi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/setup.cfg` & `SignalCliApi-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SignalCliApi
-version = 0.1.5
+version = 0.1.6
 author = Peter Nearing
 author_email = me@peternearing.ca
 description = A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://peternearing.ca/signal
 project_urls =
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/__init__.py` & `SignalCliApi-0.1.6/src/SignalCliApi/__init__.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalAccount.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalAccount.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalAccounts.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalAccounts.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalAttachment.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalAttachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         return
 
     #########################
     # To / From Dict:
     #########################
     def __to_dict__(self) -> dict:
         attachment_dict = {
-            'content_type': self.content_type,
+            'contentType': self.content_type,
             'id': self.id,
             'filename': self.filename,
             'size': self.size,
             'localPath': self.local_path,
             'thumbnail': None,
         }
         if self.thumbnail is not None:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalCallMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalCallMessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         return
 
     ###############################
     # To / From dict:
     ###############################
     def __to_dict__(self) -> dict:
         call_message_dict: dict[str, object] = super().__to_dict__()
-        call_message_dict['offer_id'] = self.offer_id
+        call_message_dict['offerId'] = self.offer_id
         call_message_dict['sdp'] = self.sdp
         call_message_dict['type'] = self.call_type
         call_message_dict['opaque'] = self.opaque
         return call_message_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
-        self.offer_id = from_dict['offer_id']
+        self.offer_id = from_dict['offerId']
         self.sdp = from_dict['sdp']
         self.call_type = from_dict['type']
         self.opaque = from_dict['opaque']
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalCli.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalCli.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalCommon.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import select
 import re
 
 DEBUG:bool = False
 ###################
 # Version:
 ###################
-VERSION: str = '0.1.5'
+VERSION: str = '0.1.6'
 ########################################
 # Regex:
 ########################################
 phone_number_regex: Pattern = re.compile(r'(?P<number>\+\d+)')
 uuid_regex: Pattern = re.compile(
     r'(?P<uuid>[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-f0-9]{12})')
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalContact.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalContact.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalContacts.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalContacts.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalDevice.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalDevice.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalDevices.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalDevices.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalGroup.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalGroup.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalGroupUpdate.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalGroupUpdate.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalGroups.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalGroups.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalMention.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalMention.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,18 +79,18 @@
         return False
 
     ######################
     # To / From Dict:
     ######################
     def __to_dict__(self) -> dict[str, object]:
         mention_dict = {
-            "contact_id": self.contact.get_id(),
+            "contactId": self.contact.get_id(),
             "start": self.start,
             "length": self.length,
         }
         return mention_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
-        added, self.contact = self._contacts.__get_or_add__("<UNKNOWN-CONTACT>", contact_id=from_dict['contact_id'])
+        added, self.contact = self._contacts.__get_or_add__("<UNKNOWN-CONTACT>", contact_id=from_dict['contactId'])
         self.start = from_dict['start']
         self.length = from_dict['length']
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalMentions.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalMentions.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         mentions_dict = {
             "mentions": [],
         }
         for mention in self._mentions:
             mentions_dict['mentions'].append(mention.__to_dict__())
         return mentions_dict
 
-    def __from_dict__(self, fromDict: dict[str, object]) -> None:
+    def __from_dict__(self, fromDict: dict[str, list]) -> None:
         self._mentions = []
         for mention_dict in fromDict['mentions']:
             self._mentions.append(Mention(contacts=self._contacts, from_dict=mention_dict))
         return
 
     #########################################
     # Helpers:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,24 +159,27 @@
                 self.recipient_type = 'group'
         return
 
     #######################
     # Init:
     #######################
     def __from_raw_message__(self, raw_message: dict) -> None:
-        print("Message.__from_raw_message__")
-        print(raw_message)
+        global DEBUG
+        if DEBUG:
+            print("Message.__from_raw_message__")
+            print(raw_message)
         # Parse Sender
-        print("DEBUG: %s" % raw_message['sourceNumber'])
+            print("DEBUG: %s" % raw_message['sourceNumber'])
         added, self.sender = self._contacts.__get_or_add__(
             name=raw_message['sourceName'],
             number=raw_message['sourceNumber'],
             uuid=raw_message['sourceUuid']
         )
-        print("DEBUG:", self.sender.number)
+        if DEBUG:
+            print("DEBUG:", self.sender.number)
         if added:
             self._contacts.__save__()
         # Parse recipient:
         self.recipient = None
         if 'dataMessage' in raw_message.keys():
             dataMessage: dict[str, object] = raw_message['dataMessage']
             if 'groupInfo' in dataMessage.keys():
@@ -236,15 +239,15 @@
     ##################################
     # To / From dict:
     ##################################
     def __to_dict__(self) -> dict:
         message_dict = {
             'sender': None,
             'recipient': None,
-            'recipient_type': self.recipient_type,
+            'recipientType': self.recipient_type,
             'device': None,
             'timestamp': None,
             'messageType': self.message_type,
             'isDelivered': self.is_delivered,
             'timeDelivered': None,
             'isRead': self.is_read,
             'timeRead': None,
@@ -267,15 +270,15 @@
             message_dict['timeViewed'] = self.time_viewed.__to_dict__()
         return message_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         # Parse sender:
         added, self.sender = self._contacts.__get_or_add__(name="<UNKNOWN-CONTACT>", contact_id=from_dict['sender'])
         # Parse recipient type:
-        self.recipient_type = from_dict['recipient_type']
+        self.recipient_type = from_dict['recipientType']
         # Parse recipient:
         if from_dict['recipient'] is not None:
             if self.recipient_type == 'contact':
                 added, self.recipient = self._contacts.__get_or_add__(name="<UNKNOWN-CONTACT>",
                                                                       contact_id=from_dict['recipient'])
             elif self.recipient_type == 'group':
                 added, self.recipient = self._groups.__get_or_add__(name="<UNKNOWN-GROUP>",
@@ -290,15 +293,15 @@
         # Parse timestamp:
         self.timestamp = Timestamp(from_dict=from_dict['timestamp'])
         # Parse message Type:
         self.message_type = from_dict['messageType']
         # Parse Delivered: (is and time)
         self.is_delivered = from_dict['isDelivered']
         if from_dict['timeDelivered'] is not None:
-            self.time_delivered = Timestamp(from_dict=from_dict['time_delivered'])
+            self.time_delivered = Timestamp(from_dict=from_dict['timeDelivered'])
         else:
             self.time_delivered = None
         # Parse read (is and time):
         self.is_read = from_dict['isRead']
         if from_dict['timeRead'] is not None:
             self.time_read = Timestamp(from_dict=from_dict['timeRead'])
         else:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalMessages.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalMessages.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalPreview.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalPreview.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from .signalAttachment import Attachment
 from .signalCommon import __type_error__
 
 
 class Preview(object):
     """Class containing a preview of a link."""
+
     def __init__(self,
                  config_path: str,
                  from_dict: dict[str, object] = None,
                  raw_preview: dict[str, object] = None,
                  generate_preview: bool = False,
                  url: Optional[str] = None,
                  title: Optional[str] = None,
@@ -133,15 +134,15 @@
             return
         # Try to open the destination file:
         try:
             fileHandle = open(preview_image_file_path, 'wb')
         except Exception as e:
             if DEBUG:
                 error_message = "Failed to open file '%s' for writing(binary): %s" % (
-                preview_image_file_path, str(e.args))
+                    preview_image_file_path, str(e.args))
                 print(error_message, file=sys.stderr)
             self.image = None
             return
         # Copy the data to the file:
         shutil.copyfileobj(response, fileHandle)
         fileHandle.close()
         # Create the attachment:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalProfile.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalProfile.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalQuote.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalQuote.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalReaction.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalReaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.emoji = reactionDict['emoji']
         added, self.target_author = self._contacts.__get_or_add__(
             name="<UNKNOWN-CONTACT>",
             number=reactionDict['targetAuthorNumber'],
             uuid=reactionDict['targetAuthorUuid'],
         )
         self.target_timestamp = Timestamp(timestamp=reactionDict['targetSentTimestamp'])
-        self.is_remove = reactionDict['is_remove']
+        self.is_remove = reactionDict['isRemove']
         return
 
     ###############################
     # Overrides:
     ###############################
     def __eq__(self, __o: Self) -> bool:
         if isinstance(__o, Reaction):
@@ -93,43 +93,43 @@
     #####################
     # To / From Dict:
     #####################
     def __to_dict__(self) -> dict:
         reaction_dict = super().__to_dict__()
         reaction_dict['emoji'] = self.emoji
         reaction_dict['targetAuthorId'] = None
-        reaction_dict['target_timestamp'] = None
-        reaction_dict['is_remove'] = self.is_remove
-        reaction_dict['is_change'] = self.is_change
-        reaction_dict['previous_emoji'] = self.previous_emoji
+        reaction_dict['targetTimestamp'] = None
+        reaction_dict['isRemove'] = self.is_remove
+        reaction_dict['isChange'] = self.is_change
+        reaction_dict['previousEmoji'] = self.previous_emoji
         if self.target_author is not None:
             reaction_dict['targetAuthorId'] = self.target_author.get_id()
         if self.target_timestamp is not None:
-            reaction_dict['target_timestamp'] = self.target_timestamp.__to_dict__()
+            reaction_dict['targetTimestamp'] = self.target_timestamp.__to_dict__()
         return reaction_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
         # Parse Emoji:
         self.emoji = from_dict['emoji']
         # Parse target author:
         if from_dict['targetAuthorId'] is not None:
             added, self.target_author = self._contacts.__get_or_add__("<UNKNOWN-CONTACT>",
                                                                       contact_id=from_dict['targetAuthorId'])
         else:
             self.target_author = None
         # Parse target timestamp:
-        if from_dict['target_timestamp'] is not None:
-            self.target_timestamp = Timestamp(from_dict=from_dict['target_timestamp'])
+        if from_dict['targetTimestamp'] is not None:
+            self.target_timestamp = Timestamp(from_dict=from_dict['targetTimestamp'])
         # Parse is remove:
-        self.is_remove = from_dict['is_remove']
+        self.is_remove = from_dict['isRemove']
         # Parse is change:
-        self.is_change = from_dict['is_change']
+        self.is_change = from_dict['isChange']
         # Parse previous emoji:
-        self.previous_emoji = from_dict['previous_emoji']
+        self.previous_emoji = from_dict['previousEmoji']
         return
 
     ###########################
     # Send reaction:
     ###########################
     def send(self) -> tuple[bool, str]:
         """
@@ -140,16 +140,16 @@
         send_reaction_command_obj = {
             "jsonrpc": "2.0",
             "id": 10,
             "method": "sendReaction",
             "params": {
                 "account": self._account_id,
                 "emoji": self.emoji,
-                "target_author": self.target_author.get_id(),
-                "target_timestamp": self.target_timestamp.timestamp,
+                "targetAuthor": self.target_author.get_id(),
+                "targetTimestamp": self.target_timestamp.timestamp,
             }
         }
         if self.recipient_type == 'contact':
             send_reaction_command_obj['params']['recipient'] = self.sender.get_id()
         elif self.recipient_type == 'group':
             send_reaction_command_obj['params']['groupId'] = self.recipient.get_id()
         else:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalReactions.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalReactions.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalReceipt.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalReceipt.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,29 +115,29 @@
     def __to_dict__(self) -> dict:
         receipt_dict = super().__to_dict__()
         # Store when:
         receipt_dict['when'] = None
         if self.when is not None:
             receipt_dict['when'] = self.when.__to_dict__()
         # Store receipt type:
-        receipt_dict['receipt_type'] = self.receiptType
+        receipt_dict['receiptType'] = self.receiptType
         # Store target timestamps:
         receipt_dict['timestamps'] = []
         for timestamp in self.timestamps:
             receipt_dict['timestamps'].append(timestamp.__to_dict__())
         return receipt_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
         # Load when:
         self.when = None
         if from_dict['when'] is not None:
             self.when = Timestamp(from_dict=from_dict['when'])
         # Load receipt Type:
-        self.receiptType = from_dict['receipt_type']
+        self.receiptType = from_dict['receiptType']
         # Load target timestamps:
         self.timestamps = []
         for timestampDict in from_dict['timestamps']:
             self.timestamps.append(Timestamp(from_dict=timestampDict))
         return
 
     #########################
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalReceiveThread.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalReceiveThread.py`

 * *Files identical despite different names*

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalReceivedMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalReceivedMessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,16 +216,16 @@
         # Parse mentions:
         if 'mentions' in data_message.keys():
             self.mentions = Mentions(contacts=self._contacts, raw_mentions=data_message['mentions'])
         # Parse sticker:
         if 'sticker' in data_message.keys():
             stickerDict: dict[str, object] = data_message['sticker']
             self._sticker_packs.__update__()  # Update in case this is a new sticker.
-            self.sticker = self._sticker_packs.get_sticker(pack_id=stickerDict['pack_id'],
-                                                           sticker_id=stickerDict['sticker_id'])
+            self.sticker = self._sticker_packs.get_sticker(pack_id=stickerDict['packId'],
+                                                           sticker_id=stickerDict['stickerId'])
         # Parse Quote
         if 'quote' in data_message.keys():
             if self.recipient_type == 'group':
                 self.quote = Quote(config_path=self._config_path, contacts=self._contacts, groups=self._groups,
                                    raw_quote=data_message['quote'], conversation=self.recipient)
             elif self.recipient_type == 'contact':
                 self.quote = Quote(config_path=self._config_path, contacts=self._contacts, groups=self._groups,
@@ -258,29 +258,29 @@
         # receivedMessageDict['reactions'] = None
         # if (self.reactions != None):
         received_message_dict['reactions'] = self.reactions.__to_dict__()
         # Set sticker:
         received_message_dict['sticker'] = None
         if self.sticker is not None:
             received_message_dict['sticker'] = {
-                'pack_id': self.sticker._pack_id,
-                'sticker_id': self.sticker.id
+                'packId': self.sticker._pack_id,
+                'stickerId': self.sticker.id
             }
         # Set quote:
         received_message_dict['quote'] = None
         if self.quote is not None:
             received_message_dict['quote'] = self.quote.__to_dict__()
         # Set expiration:
-        received_message_dict['is_expired'] = self.is_expired
+        received_message_dict['isExpired'] = self.is_expired
         received_message_dict['expiration'] = None
-        received_message_dict['expiration_timestamp'] = None
+        received_message_dict['expirationTimestamp'] = None
         if self.expiration is not None:
             received_message_dict['expiration'] = self.expiration.seconds
         if self.expiration_timestamp is not None:
-            received_message_dict['expiration_timestamp'] = self.expiration_timestamp.__to_dict__()
+            received_message_dict['expirationTimestamp'] = self.expiration_timestamp.__to_dict__()
         # Set previews:
         received_message_dict['previews'] = []
         for preview in self.previews:
             received_message_dict['previews'].append(preview.__to_dict__())
         return received_message_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
@@ -297,55 +297,55 @@
         # Load mentions:
         self.mentions = Mentions(contacts=self._contacts, from_dict=from_dict['mentions'])
         # Load reactions:
         # self.reactions = None
         # if (from_dict['reactions'] != None):
         self.reactions = Reactions(command_socket=self._command_socket, account_id=self._account_id,
                                    contacts=self._contacts, groups=self._groups, devices=self._devices,
-                                   from_dict=from_dict['reactions'])
+                                   this_device=self._this_device, from_dict=from_dict['reactions'])
         # Load sticker:
         self.sticker = None
         if from_dict['sticker'] is not None:
             self.sticker = self._sticker_packs.get_sticker(
-                pack_id=from_dict['sticker']['pack_id'],
-                sticker_id=from_dict['sticker']['sticker_id']
+                pack_id=from_dict['sticker']['packId'],
+                sticker_id=from_dict['sticker']['stickerId']
             )
         # Load quote
         self.quote = None
         if from_dict['quote'] is not None:
             self.quote = Quote(config_path=self._config_path, contacts=self._contacts, groups=self._groups,
                                from_dict=from_dict['quote'])
         # Load expiration:
-        self.is_expired = from_dict['is_expired']
+        self.is_expired = from_dict['isExpired']
         self.expiration = None
         if from_dict['expiration'] is not None:
             self.expiration = timedelta(seconds=from_dict['expiration'])
         self.expiration_timestamp = None
-        if from_dict['expiration_timestamp'] is not None:
-            self.expiration_timestamp = Timestamp(from_dict=from_dict['expiration_timestamp'])
+        if from_dict['expirationTimestamp'] is not None:
+            self.expiration_timestamp = Timestamp(from_dict=from_dict['expirationTimestamp'])
         # Load previews:
         self.previews = []
         for preview_dict in from_dict['previews']:
             self.previews.append(Preview(config_path=self._config_path, from_dict=preview_dict))
         return
 
     #####################
     # Helpers:
     #####################
     def __send_receipt__(self, receipt_type: str) -> Timestamp:
         # Create send receipt command object and json command string.
         send_receipt_command_obj = {
             "jsonrpc": "2.0",
             "id": 0,
-            "method": "send_receipt",
+            "method": "sendReceipt",
             "params": {
                 "account": self._account_id,
                 "recipient": self.sender.get_id(),
                 "type": receipt_type,
-                "target_timestamp": self.timestamp.timestamp,
+                "targetTimestamp": self.timestamp.timestamp,
             }
         }
         json_command_str = json.dumps(send_receipt_command_obj) + '\n'
         # Communicate with signal:
         __socket_send__(self._command_socket, json_command_str)
         response_str = __socket_receive__(self._command_socket)
         # Parse Response:
@@ -409,14 +409,15 @@
         if len(self.mentions) != 0:
             return False
         if self.sticker is not None:
             return False
         if self.quote is not None:
             return False
         return True
+
     #####################
     # Methods:
     #####################
     def mark_delivered(self, when: Timestamp) -> None:
         """
         Mark message as delivered.
         :param when: Timestamp: When the message was delivered.
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalSentMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalSentMessage.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,47 +283,47 @@
         sent_message_dict['reactions'] = None
         if self.reactions is not None:
             sent_message_dict['reactions'] = self.reactions.__to_dict__()
         # Set sticker:
         sent_message_dict['sticker'] = None
         if self.sticker is not None:
             sent_message_dict['sticker'] = {
-                'pack_id': self.sticker._pack_id,
-                'sticker_id': self.sticker.id
+                'packId': self.sticker._pack_id,
+                'stickerId': self.sticker.id
             }
         # Set quote:
         sent_message_dict['quote'] = None
         if self.quote is not None:
             sent_message_dict['quote'] = self.quote.__to_dict__()
         # Set expiration:
         sent_message_dict['expiration'] = None
-        sent_message_dict['expiration_timestamp'] = None
-        sent_message_dict['is_expired'] = self.is_expired
+        sent_message_dict['expirationimestamp'] = None
+        sent_message_dict['isExpired'] = self.is_expired
         if self.expiration is not None:
             sent_message_dict['expiration'] = self.expiration.seconds
         if self.expiration_timestamp is not None:
-            sent_message_dict['expiration_timestamp'] = self.expiration_timestamp.__to_dict__()
+            sent_message_dict['expirationTimestamp'] = self.expiration_timestamp.__to_dict__()
         # Set is sent:
-        sent_message_dict['is_sent'] = self.is_sent
+        sent_message_dict['isSent'] = self.is_sent
         # Set sent_to list:
-        sent_message_dict['sent_to'] = []
+        sent_message_dict['sentTo'] = []
         for contact in self.sent_to:
-            sent_message_dict['sent_to'].append(contact.get_id())
+            sent_message_dict['sentTo'].append(contact.get_id())
         # Set delivery_receipts list:
-        sent_message_dict['delivery_receipts'] = []
+        sent_message_dict['deliveryReceipts'] = []
         for receipt in self.delivery_receipts:
-            sent_message_dict['delivery_receipts'].append(receipt.__to_dict__())
+            sent_message_dict['deliveryReceipts'].append(receipt.__to_dict__())
         # Set read_receipts list:
-        sent_message_dict['read_receipts'] = []
+        sent_message_dict['readReceipts'] = []
         for receipt in self.read_receipts:
-            sent_message_dict['read_receipts'].append(receipt.__to_dict__())
+            sent_message_dict['readReceipts'].append(receipt.__to_dict__())
         # Set viewed_receipts list:
-        sent_message_dict['viewed_receipts'] = []
+        sent_message_dict['viewedReceipts'] = []
         for receipt in self.viewed_receipts:
-            sent_message_dict['viewed_receipts'].append(receipt.__to_dict__())
+            sent_message_dict['viewedReceipts'].append(receipt.__to_dict__())
         return sent_message_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
         # Load Body:
         self.body = from_dict['body']
         # Load attachments:
@@ -343,56 +343,56 @@
             self.reactions = Reactions(command_socket=self._command_socket, account_id=self._account_id,
                                        contacts=self._contacts, groups=self._groups, devices=self._devices,
                                        from_dict=from_dict['reactions'])
         # Load sticker
         self.sticker = None
         if from_dict['sticker'] is not None:
             self.sticker = self._sticker_packs.get_sticker(
-                pack_id=from_dict['sticker']['pack_id'],
-                sticker_id=from_dict['sticker']['sticker_id']
+                pack_id=from_dict['sticker']['packId'],
+                sticker_id=from_dict['sticker']['stickerId']
             )
         # Load Quote:
         self.quote = None
         if from_dict['quote'] is not None:
             self.quote = Quote(from_dict=from_dict['quote'])
         # Load expiration:
         self.expiration = None
         if from_dict['expiration'] is not None:
             self.expiration = timedelta(seconds=from_dict['expiration'])
         self.expiration_timestamp = None
-        if from_dict['expiration_timestamp'] is not None:
-            self.expiration_timestamp = Timestamp(from_dict=from_dict['expiration_timestamp'])
-        self.is_expired = from_dict['is_expired']
+        if from_dict['expirationTimestamp'] is not None:
+            self.expiration_timestamp = Timestamp(from_dict=from_dict['expirationTimestamp'])
+        self.is_expired = from_dict['isExpired']
         # Load is_sent:
-        self.is_sent = from_dict['is_sent']
+        self.is_sent = from_dict['isSent']
         # Load sent_to:
         self.sent_to = []
-        if from_dict['sent_to'] is not None:
-            for contactId in from_dict['sent_to']:
+        if from_dict['sentTo'] is not None:
+            for contactId in from_dict['sentTo']:
                 added, contact = self._contacts.__get_or_add__("<UNKNOWN-CONTACT>", contactId)
                 self.sent_to.append(contact)
         # Load delivery_receipts:
         self.delivery_receipts = []
-        for receiptDict in from_dict['delivery_receipts']:
+        for receiptDict in from_dict['deliveryReceipts']:
             receipt = Receipt(command_socket=self._command_socket, account_id=self._account_id,
                               config_path=self._config_path,
                               contacts=self._contacts, groups=self._groups, devices=self._devices,
                               this_device=self._this_device, from_dict=receiptDict)
             self.delivery_receipts.append(receipt)
         # Load read_receipts:
         self.read_receipts = []
-        for receiptDict in from_dict['read_receipts']:
+        for receiptDict in from_dict['readReceipts']:
             receipt = Receipt(command_socket=self._command_socket, account_id=self._account_id,
                               config_path=self._config_path,
                               contacts=self._contacts, groups=self._groups, devices=self._devices,
                               this_device=self._this_device, from_dict=receiptDict)
             self.read_receipts.append(receipt)
         # Load viewed_receipts:
         self.viewed_receipts = []
-        for receiptDict in from_dict['viewed_receipts']:
+        for receiptDict in from_dict['viewedReceipts']:
             receipt = Receipt(command_socket=self._command_socket, account_id=self._account_id,
                               config_path=self._config_path,
                               contacts=self._contacts, groups=self._groups, devices=self._devices,
                               this_device=self._this_device, from_dict=receiptDict)
 
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalSticker.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalSticker.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             self.__from_manifest__(from_manifest)
         return
 
     ##########################
     # Init:
     ##########################
     def __from_manifest__(self, from_manifest: dict[str, str]) -> None:
-        self.id = from_manifest['contact_id']
+        self.id = from_manifest['id']
         self.emoji = from_manifest['emoji']
         file_name = from_manifest['file']
         self.file_path = os.path.join(self._pack_path, file_name)
-        self.content_type = from_manifest['content_type']
+        self.content_type = from_manifest['contentType']
         return
 
     #######################
     # Overrides:
     #######################
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, Sticker):
@@ -80,28 +80,28 @@
         return sticker_string
 
     #######################
     # To / From Dict:
     #######################
     def __to_dict__(self) -> dict[str, object]:
         sticker_dict = {
-            "_pack_id": self._pack_id,
-            "contact_id": self.id,
+            "_packId": self._pack_id,
+            "contactId": self.id,
             "emoji": self.emoji,
-            "file_path": self.file_path,
-            "content_type": self.content_type
+            "filePath": self.file_path,
+            "contentType": self.content_type
         }
         return sticker_dict
 
     def __from_dict__(self, from_dict: dict[str, object]) -> None:
-        self._pack_id = from_dict['_pack_id']
-        self.id = from_dict['contact_id']
+        self._pack_id = from_dict['_packId']
+        self.id = from_dict['contactId']
         self.emoji = from_dict['emoji']
-        self.file_path = from_dict['file_path']
-        self.content_type = from_dict['content_type']
+        self.file_path = from_dict['filePath']
+        self.content_type = from_dict['contentType']
         return
 
 
 #############################################################################################
 class StickerPack(object):
     """Sticker Pack object."""
 
@@ -126,18 +126,18 @@
             __type_error__("from_manifest", "dict", from_manifest)
         if title is not None and not isinstance(title, str):
             __type_error__("title", "str", title)
         if author is not None and not isinstance(author, str):
             __type_error__("author", "str", author)
         if cover is not None and not isinstance(cover, Sticker):
             __type_error__("cover", "Sticker", cover)
+        sticker_list: list[Sticker] = []
         if stickers is not None and not isinstance(stickers, Iterable):
             __type_error__("stickers", "Iterable[Sticker]", stickers)
         elif stickers is not None:
-            sticker_list: list[Sticker] = []
             for i, sticker in enumerate(stickers):
                 if not isinstance(sticker, Sticker):
                     __type_error__("stickers[%i]" % i, "Sticker", sticker)
                 sticker_list.append(sticker)
         # Set internal Vars:
         self._pack_path: str = pack_path
         # Set external properties:
@@ -185,28 +185,28 @@
         return iter(self.stickers)
 
     ####################
     # To / From Dict:
     ####################
     def __to_dict__(self) -> dict:
         sticker_pack_dict = {
-            'pack_id': self.pack_id,
+            'packId': self.pack_id,
             'title': self.title,
             'author': self.author,
             'cover': None,
             'stickers': [],
         }
         if self.cover is not None:
             sticker_pack_dict['cover'] = self.cover.__to_dict__()
         for sticker in self.stickers:
             sticker_pack_dict['stickers'].append(sticker.__to_dict__())
         return sticker_pack_dict
 
     def __from_dict__(self, from_dict: dict[str, object]) -> None:
-        self.pack_id = from_dict['pack_id']
+        self.pack_id = from_dict['packId']
         self.title = from_dict['title']
         self.author = from_dict['author']
         if from_dict['cover'] is not None:
             self.cover = Sticker(pack_id=self.pack_id, pack_path=self._pack_path, from_dict=from_dict['cover'])
         else:
             self.cover = None
         self.stickers = []
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalSyncMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalSyncMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,39 +130,39 @@
 
     ###########################
     # To / From Dict:
     ###########################
     def __to_dict__(self) -> dict:
         sync_message_dict = super().__to_dict__()
         # Store sync type:
-        sync_message_dict['sync_type'] = self.sync_type
+        sync_message_dict['syncType'] = self.sync_type
         # Store sent message properties:
-        sync_message_dict['raw_sent_message'] = self.raw_sent_message
+        sync_message_dict['rawSentMessage'] = self.raw_sent_message
         # Store the read messages list:
         # Store the list as a list of tuples[contactID:str, timestampDict:dict]
-        sync_message_dict['read_messages'] = []
+        sync_message_dict['readMessages'] = []
         for (contact, timestamp) in self.read_messages:
             target_message_tuple = (contact.get_id(), timestamp.__to_dict__())
-            sync_message_dict['read_messages'].append(target_message_tuple)
+            sync_message_dict['readMessages'].append(target_message_tuple)
         # Store Blocked contacts and groups lists:
-        sync_message_dict['blocked_contacts'] = self.blocked_contacts
-        sync_message_dict['blocked_groups'] = self.blocked_groups
+        sync_message_dict['blockedContacts'] = self.blocked_contacts
+        sync_message_dict['blockedGroups'] = self.blocked_groups
         return sync_message_dict
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
         # Load sync type:
-        self.sync_type = from_dict['sync_type']
+        self.sync_type = from_dict['syncType']
         # Load sent message properties:
-        self.raw_sent_message = from_dict['raw_sent_message']
+        self.raw_sent_message = from_dict['rawSentMessage']
         # Set read messages list:
         # Load read messages:
         self.read_messages = []
-        for (contact_id, timestamp_dict) in from_dict['read_messages']:
+        for (contact_id, timestamp_dict) in from_dict['readMessages']:
             added, contact = self._contacts.__get_or_add__("<UNKNOWN-CONTACT>", contact_id)
             timestamp = Timestamp(from_dict=timestamp_dict)
             self.read_messages.append((contact, timestamp))
         # Set blocked groups and contacts:
-        self.blocked_contacts = from_dict['blocked_contacts']
-        self.blocked_groups = from_dict['blocked_groups']
+        self.blocked_contacts = from_dict['blockedContacts']
+        self.blocked_groups = from_dict['blockedGroups']
 
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalTextAttachment.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalTextAttachment.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,37 +55,37 @@
     ####################
     # Init:
     ####################
     def __from_raw_attachment__(self, raw_attachment: dict[str, object]) -> None:
         # Load text:
         self.text = raw_attachment['text']
         self.style = raw_attachment['style']
-        self.text_background_color = raw_attachment['text_background_color']
-        self.text_foreground_color = raw_attachment['text_foreground_color']
-        self.background_color = raw_attachment['background_color']
+        self.text_background_color = raw_attachment['textBackgroundColor']
+        self.text_foreground_color = raw_attachment['textForegroundColor']
+        self.background_color = raw_attachment['backgroundColor']
         return
 
     ####################
     # To / From dict:
     ####################
     def __to_dict__(self) -> dict[str, object]:
         textAttachmentDict = {
             'text': self.text,
             'style': self.style,
-            'text_background_color': self.text_background_color,
-            'text_foreground_color': self.text_foreground_color,
-            'background_color': self.background_color,
+            'textBackgroundColor': self.text_background_color,
+            'textForegroundColor': self.text_foreground_color,
+            'backgroundColor': self.background_color,
         }
         return textAttachmentDict
 
     def __from_dict__(self, from_dict: dict[str, object]) -> None:
         # Load text:
         self.text = from_dict['text']
         # Load style:
         self.style = from_dict['style']
         # Load text bg colour:
-        self.text_background_color = from_dict['text_background_color']
+        self.text_background_color = from_dict['textBackgroundColor']
         # Load text fg colour:
-        self.text_foreground_color = from_dict['text_foreground_color']
+        self.text_foreground_color = from_dict['textForegroundColor']
         # Load background colour:
-        self.background_color = from_dict['background_color']
+        self.background_color = from_dict['backgroundColor']
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalThumbnail.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalThumbnail.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,38 +53,39 @@
             self.__from_raw_thumbnail__(raw_thumbnail)
         return
 
     ###################
     # Init:
     ###################
     def __from_raw_thumbnail__(self, raw_thumbnail: dict[str, object]) -> None:
-        # print(raw_thumbnail)
-        self.content_type = raw_thumbnail['content_type']
+        if DEBUG:
+            print(raw_thumbnail)
+        self.content_type = raw_thumbnail['contentType']
         self.filename = raw_thumbnail['filename']
-        self.local_path = os.path.join(self._config_path, 'attachments', raw_thumbnail['contact_id'])
+        self.local_path = os.path.join(self._config_path, 'attachments', raw_thumbnail['id'])
         self.exists = os.path.exists(self.local_path)
         self.size = raw_thumbnail['size']
         return
 
     ############################
     # To / From dict:
     ############################
     def __to_dict__(self) -> dict[str, object]:
         thumbnail_dict = {
-            'content_type': self.content_type,
+            'contentType': self.content_type,
             'filename': self.filename,
-            'local_path': self.local_path,
+            'localPath': self.local_path,
             'size': self.size,
         }
         return thumbnail_dict
 
     def __from_dict__(self, fromDict: dict[str, object]) -> None:
-        self.content_type = fromDict['content_type']
+        self.content_type = fromDict['contentType']
         self.filename = fromDict['filename']
-        self.local_path = fromDict['local_path']
+        self.local_path = fromDict['localPath']
         self.exists = False
         if self.local_path is not None:
             self.exists = os.path.exists(self.local_path)
         else:
             self.exists = False
         self.size = fromDict['size']
         return
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalTimestamp.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalTimestamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/env python3
 
 from typing import TypeVar, Optional, IO
 import datetime
-import pytz
-DEBUG: bool = False
-
+import sys
+try:
+    import pytz
+except ModuleNotFoundError:
+    print("Module: pytz not found, you can install using pip3 install pytz")
+    exit(1)
 try:
     from tzlocal import get_localzone
 except ModuleNotFoundError:
     print("Module: tzlocal not found, you can install using 'sudo apt install python3-tzlocal', or by using ", end='')
     print("pip install tzlocal")
-import sys
+    exit(1)
+
 
 from .signalCommon import __type_error__
 
 Self = TypeVar("Self", bound="Timestamp")
+DEBUG: bool = False
 
 
 class Timestamp(object):
     """Time stamp object."""
 
     def __init__(self,
                  timestamp: Optional[int] = None,
@@ -97,28 +102,37 @@
 
     def __float__(self) -> float:
         return self.date_time.timestamp()
 
     def __str__(self) -> str:
         return self.date_time.isoformat()
 
-    def __eq__(self, __o: Self) -> bool:
-        if not isinstance(__o, Timestamp):
+    def __eq__(self, __o: Self | int) -> bool:
+        if not isinstance(__o, Timestamp) and not isinstance(__o, int):
             return False
-        return self.date_time == __o.date_time
-
-    def __lt__(self, __o: Self) -> bool:
-        if not isinstance(__o, Timestamp):
-            raise TypeError("FATAL: only Timestamp is supported.")
-        return self.date_time < __o.date_time
+        if isinstance(__o, Timestamp):
+            return self.date_time == __o.date_time
+        else:
+            return self.timestamp == __o
+
+    def __lt__(self, __o: Self | int) -> bool:
+        if not isinstance(__o, Timestamp) and not isinstance(__o, int):
+            raise TypeError("FATAL: only Timestamp and int are supported.")
+        if isinstance(__o, Timestamp):
+            return self.date_time < __o.date_time
+        else:
+            return self.timestamp < __o
 
     def __gt__(self, __o: Self | int) -> bool:
-        if not isinstance(__o, Timestamp):
+        if not isinstance(__o, Timestamp) and not isinstance(__o, int):
             raise TypeError("FATAL: Only SignalTimestamp and int are supported.")
-        return self.date_time > __o.datetime
+        if isinstance(__o, Timestamp):
+            return self.date_time > __o.datetime
+        else:
+            return self.timestamp > __o
 
     ##########################
     # Getters:
     ##########################
 
     def get_timestamp(self) -> int:
         """
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi/signalTypingMessage.py` & `SignalCliApi-0.1.6/src/SignalCliApi/signalTypingMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,24 +67,24 @@
         self.time_changed = Timestamp(timestamp=typing_dict['timestamp'])
         return
 
     def __to_dict__(self) -> dict:
         typing_message = super().__to_dict__()
         typing_message['action'] = self.action
         if self.time_changed is not None:
-            typing_message['time_changed'] = self.time_changed.__to_dict__()
+            typing_message['timeChanged'] = self.time_changed.__to_dict__()
         else:
-            typing_message['time_changed'] = None
+            typing_message['timeChanged'] = None
         return typing_message
 
     def __from_dict__(self, from_dict: dict) -> None:
         super().__from_dict__(from_dict)
         self.action = from_dict['action']
-        if from_dict['time_changed'] is not None:
-            self.time_changed = Timestamp(from_dict=from_dict['time_changed'])
+        if from_dict['timeChanged'] is not None:
+            self.time_changed = Timestamp(from_dict=from_dict['timeChanged'])
         else:
             self.time_changed = None
         return
 
     def __update_body__(self) -> None:
         if self.sender is not None and self.action is not None and self.time_changed is not None:
             if self.recipient is not None and self.recipient_type is not None:
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi.egg-info/PKG-INFO` & `SignalCliApi-0.1.6/src/SignalCliApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SignalCliApi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python interface to the signal-cli found at https://github.com/AsamK/signal-cli
 Home-page: https://peternearing.ca/signal
 Author: Peter Nearing
 Author-email: me@peternearing.ca
 Project-URL: Docs, https://peternearing.ca/signal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
```

### Comparing `SignalCliApi-0.1.5/src/SignalCliApi.egg-info/SOURCES.txt` & `SignalCliApi-0.1.6/src/SignalCliApi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

