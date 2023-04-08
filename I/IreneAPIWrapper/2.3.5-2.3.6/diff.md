# Comparing `tmp/IreneAPIWrapper-2.3.5.tar.gz` & `tmp/IreneAPIWrapper-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IreneAPIWrapper-2.3.5.tar", last modified: Tue Mar 28 05:33:59 2023, max compression
+gzip compressed data, was "IreneAPIWrapper-2.3.6.tar", last modified: Fri Apr  7 22:44:41 2023, max compression
```

## Comparing `IreneAPIWrapper-2.3.5.tar` & `IreneAPIWrapper-2.3.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.831792 IreneAPIWrapper-2.3.5/IreneAPIWrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/affiliation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/automedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/abstractmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/mediasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/biasgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/bloodtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/difficulty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/fandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/groupalias.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/guessinggame.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/personalias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/preloadcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/reactionrolemessages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/social.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/statsupdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tiktokaccount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/twitchaccount.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/twitteraccount.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/unscramblegame.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/urban.py
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/userstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/wolfram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/IreneAPIWrapper/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper/sections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:33:59.835792 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 05:33:59.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-28 05:33:59.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 05:33:59.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 05:33:59.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 05:33:59.000000 IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 05:33:59.851792 IreneAPIWrapper-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-28 05:33:50.000000 IreneAPIWrapper-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.600279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/affiliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/automedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/abstractmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/mediasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/biasgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/bloodtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/difficulty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/fandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/groupalias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guessinggame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/personalias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/preloadcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reactionrolemessages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/statsupdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tiktokaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitchaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitteraccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/unscramblegame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/urban.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/userstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/wolfram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.608279 IreneAPIWrapper-2.3.6/IreneAPIWrapper/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper/sections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:44:41.600279 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 22:44:41.000000 IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:44:41.612279 IreneAPIWrapper-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-07 22:44:30.000000 IreneAPIWrapper-2.3.6/setup.py
```

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/exceptions.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/__init__.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/affiliation.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/automedia.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/automedia.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/abstractmodel.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/abstractmodel.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/alias.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/alias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/mediasource.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/mediasource.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/base/receiver.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/base/receiver.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,27 +27,29 @@
     obj = await obj.create(**callback.response.get("results"))
     if isinstance(obj, list) and obj:
         obj = obj[0]
     return obj
 
 
 async def internal_fetch_all(
-    obj: AbstractModel, request: dict, bulk: bool = False
+    obj: AbstractModel, request: dict, bulk: bool = False, log_creation: bool = True
 ) -> List[AbstractModel]:
     """
     Fetch all known instances of the concrete object from the API.
 
     .. NOTE:: Concrete objects are added to cache on creation.
 
     :param obj: :ref:`AbstractModel`
         An abstract model.
     :param request: dict
         The request to pass into a Callback.
     :param bulk: bool
         Whether to generate objects in bulk (Defaults to False).
+    :param log_creation: bool
+        Whether to log the creation.
     :return: List[:ref:`AbstractModel`]
         Returns a list of abstract models.
     """
     callback = CallBack(request=request)
     await outer.client.add_and_wait(callback)
 
     if not callback.response.get("results"):
@@ -58,15 +60,15 @@
         if not bulk:
             data = [
                 await obj.create(**info)
                 for info in callback.response["results"].values()
             ]
         else:
             data = await obj.create_bulk(list(callback.response["results"].values()))
-        if outer.client.logger:
+        if outer.client.logger and log_creation:
             outer.client.logger.info(f"Finished creating/fetching all cache for {obj.__name__} in "
                                      f"{perf_counter() - start}s")
         return data
     except Exception as e:
         raise FailedObjectCreation(callback)
```

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/biasgame.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/biasgame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/bloodtype.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/bloodtype.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/callback.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/callback.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/channel.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/channel.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/client.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/client.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/company.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/company.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/date.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/date.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/difficulty.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/difficulty.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/display.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/display.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/eightball.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/eightball.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/fandom.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/fandom.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/group.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/group.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/groupalias.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/groupalias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/guessinggame.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guessinggame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/guild.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/guild.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/interactions.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/interactions.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/language.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/language.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/location.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/location.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/media.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/media.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/name.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/name.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/notification.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/notification.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/person.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/person.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/personalias.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/personalias.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/position.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/position.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/preloadcache.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/preloadcache.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/reactionrolemessages.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reactionrolemessages.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/reminder.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/reminder.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,18 @@
         """
         return await internal_fetch(
             Reminder,
             request={"route": "reminder/$remind_id", "remind_id": remind_id, "method": "GET"},
         )
 
     @staticmethod
-    async def fetch_all():
+    async def fetch_all(log_creation=True):
         """Fetch all reminders.
 
         .. NOTE::: Reminders objects are added to cache on creation.
         """
         return await internal_fetch_all(
-            obj=Reminder, request={"route": "reminder/", "method": "GET"}
+            obj=Reminder, request={"route": "reminder/", "method": "GET"}, log_creation=log_creation
         )
 
 
 _reminders: Dict[int, Reminder] = dict()
```

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/social.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/social.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/subscription.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/subscription.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tag.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tag.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tiktokaccount.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tiktokaccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/timeline.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/timeline.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/tweet.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/tweet.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/twitchaccount.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitchaccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/twitteraccount.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/twitteraccount.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/unscramblegame.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/unscramblegame.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/user.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/user.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper/models/userstatus.py` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper/models/userstatus.py`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/PKG-INFO` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IreneAPIWrapper
-Version: 2.3.5
+Version: 2.3.6
 Summary: A wrapper for Irene's API and connects with a websocket connection.
 Home-page: https://github.com/MujyKun/IreneAPIWrapper
 Author: MujyKun
 Author-email: mujy@irenebot.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IreneAPIWrapper-2.3.5/IreneAPIWrapper.egg-info/SOURCES.txt` & `IreneAPIWrapper-2.3.6/IreneAPIWrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IreneAPIWrapper-2.3.5/PKG-INFO` & `IreneAPIWrapper-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IreneAPIWrapper
-Version: 2.3.5
+Version: 2.3.6
 Summary: A wrapper for Irene's API and connects with a websocket connection.
 Home-page: https://github.com/MujyKun/IreneAPIWrapper
 Author: MujyKun
 Author-email: mujy@irenebot.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IreneAPIWrapper-2.3.5/pyproject.toml` & `IreneAPIWrapper-2.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "IreneAPIWrapper"
-version = "2.3.5"
+version = "2.3.6"
 description = "The Wrapper for the Websocket and REST API of Irene."
 authors = ["MujyKun <mujy@irenebot.com>"]
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
 ]
```

### Comparing `IreneAPIWrapper-2.3.5/setup.py` & `IreneAPIWrapper-2.3.6/setup.py`

 * *Files identical despite different names*

