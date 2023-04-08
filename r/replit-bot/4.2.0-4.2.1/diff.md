# Comparing `tmp/replit-bot-4.2.0.tar.gz` & `tmp/replit-bot-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.0.tar", max compression
+gzip compressed data, was "replit-bot-4.2.1.tar", max compression
```

## Comparing `replit-bot-4.2.0.tar` & `replit-bot-4.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.0/LICENSE
--rw-r--r--   0        0        0      822 2023-04-01 17:19:47.164610 replit-bot-4.2.0/pyproject.toml
--rw-r--r--   0        0        0    26572 2023-04-01 17:19:58.116582 replit-bot-4.2.0/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50124 2023-04-01 17:19:09.880707 replit-bot-4.2.0/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.0/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.0/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-01 17:19:52.160598 replit-bot-4.2.0/replit_bot/__init__.py
--rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.0/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.0/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.0/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.0/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.0/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.0/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.0/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.0/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.0/replit_bot/queries.js
--rw-r--r--   0        0        0    64976 2023-04-01 17:18:23.964826 replit-bot-4.2.0/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.0/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.0/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.0/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.0/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.0/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.0/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      823 2023-04-01 17:20:00.060322 replit-bot-4.2.0/setup.py
--rw-r--r--   0        0        0      674 2023-04-01 17:20:00.060796 replit-bot-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.1/LICENSE
+-rw-r--r--   0        0        0      822 2023-04-08 20:28:37.000575 replit-bot-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0    30264 2023-04-08 20:28:31.236583 replit-bot-4.2.1/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50124 2023-04-01 19:33:20.331864 replit-bot-4.2.1/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.1/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.1/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-08 20:28:39.816571 replit-bot-4.2.1/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.1/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.1/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.1/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.1/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.1/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.1/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.1/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.1/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.1/replit_bot/queries.js
+-rw-r--r--   0        0        0    65893 2023-04-08 20:14:29.965727 replit-bot-4.2.1/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.1/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.1/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.1/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.1/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.1/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.1/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      823 2023-04-08 20:28:43.812679 replit-bot-4.2.1/setup.py
+-rw-r--r--   0        0        0      674 2023-04-08 20:28:43.813094 replit-bot-4.2.1/PKG-INFO
```

### Comparing `replit-bot-4.2.0/LICENSE` & `replit-bot-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/pyproject.toml` & `replit-bot-4.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.0"
+version = "4.2.1"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.6.1,<4.0.0"
 # replit db I think I can't remember lol
```

### Comparing `replit-bot-4.2.0/replit_bot/AsyncBot.py` & `replit-bot-4.2.1/replit_bot/AsyncBot.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,33 +121,40 @@
             await ctx.reply(__current)
 
         async def __default_call_when_followed(ctx, person) -> None:
             logger.info(
                 f"{green}[FILE] BOT.py{end}\n{green}[INFO]{end} @{person.username} followed bot"
             )
 
+        async def __default_when_invited_to_repl(ctx) -> None:
+            return await ctx.reply(
+                "Hello @everyone ! Thanks for inviting me to this repl"
+            )
+
         self.commands = {
             "help": {
                 "call": help_function,
                 "desc": "See commands",
                 "name": "help",
                 "thread": False,
                 "params": {"command": Param(required=False, default="None")},
             }
         }
         self.doc_html = None  # deadlock for if html generated || stores html
         self._call_when_followed = __default_call_when_followed
         self._default = __current_default
         self._not_all_required_params_specified = __not_included_params
+        self._when_invited_to_repl = __default_when_invited_to_repl
         self.token = token
         self.bio = bio
         self.prefix = prefix
         self.alias = {}
         self.listeners = {}
         self.threads_ = []
+        self.multiplayer_repls = []
 
     def command(
         self, name: str, thread: bool = False, desc: str = None, alias: List[str] = []
     ):
         """takes in args"""
         name = name.lower()
         if not name.replace("-", "").isalnum():
@@ -192,14 +199,17 @@
 
     def default(self, func):
         self._default = func
 
     def fallback_param_not_included_case(self, func):
         self._not_all_required_params_specified = func
 
+    def when_invited_to_repl(self, func):
+        self._when_invited_to_repl = func
+
     async def parse_command(self, command: str):
         """parses command
 
         @Example-Bot /say message:hi!
         ->
         {
             "options": {
@@ -357,14 +367,16 @@
 
             else:
                 links.docs = None
 
             @flask_app.route("/<command>/<user>/<choice>/<rand_chars>")
             def _parse_button_commands(command, user, choice, rand_chars):
                 global _started_buttons
+                if rand_chars[-1] == ")":
+                    rand_chars = rand_chars[:-1]
                 if request.headers["X-Replit-User-Name"] == "":
                     return render_template_string(
                         TEMPLATE,
                         html='<center><div><script authed="location.reload()" src="https://auth.util.repl.co/script.js"></script></div></center>',
                     )
                 if (
                     command in _started_buttons
@@ -396,15 +408,18 @@
             __typename = getattr(notif, "__typename")
             if __typename == "WarningNotification":
                 logger.critical(
                     f"{red}[FILE] BOT.py{end}\n{red}[INFO]{end} bot has been warned"
                 )
             elif __typename == "NewFollowerNotification":
                 await self._call_when_followed(self, notif.creator)
-            elif getattr(notif, "comment", False):
+            elif (
+                __typename == "MentionedInComment" or __typename == "MentionedInPost"
+            ) and getattr(notif, "comment", False):
+                notif.comment.notif_type = __typename
                 notif.comment.author = notif.comment.user
                 notif.comment.author.mention = "@" + notif.comment.author.username
                 notif.comment.Image = lambda url, caption="": f"![{caption}]({url})"
                 notif.comment.Link = lambda text, url: f"[{text}]({url})"
                 for i in dir(self):
                     if not i.startswith("__") and not i.endswith("__"):
                         setattr(notif.comment, i, getattr(self, i))
@@ -526,14 +541,15 @@
                 await self.gql(
                     "markMessageAsSeen",
                     {"replId": repl_annotations["id"], "anchorId": anchor["id"]},
                 )
 
                 class CurrentCtx:
                     def __init__(self):
+                        self.notif_type = "AnnotationNotification"
                         self.repl_id = repl_annotations["id"]
                         self.anchor_id = anchor["id"]
 
                     async def reply(self, body) -> None:
                         return await self.gql(
                             "createChatMessage",
                             vars={
@@ -625,14 +641,80 @@
                         )
                         await self._not_all_required_params_specified(ctx)
                 elif "command" in parsed_json and valid_first:
                     logger.info(
                         f"{green}[FILE] BOT.py{end}\n{green}[INFO]{end} logging command\n\t{blue}[SUMMARY]{end} unsuccessful: {red}Invalid command{end}.\n\t{purple}[EXTRA]{end} Requested command: {parsed_json['command']}"
                     )
                     await self._default(ctx)
+            elif __typename == "MultiplayerInvitedNotification":
+                url = notif.__dict__["url"]
+                res = await self.gql("getReplAnnotations", {"url": url})
+                repl_annotations = res["repl"]
+                if repl_annotations is None:
+                    return
+                anchor = list(
+                    filter(
+                        lambda x: x["isGeneral"], repl_annotations["annotationAnchors"]
+                    )
+                )
+                if len(anchor) > 0:
+                    anchor = anchor[0]
+                else:
+                    anchor = {"id": None}
+                super_self = self
+
+                class CurrentCtx:
+                    def __init__(self):
+                        self.notif_type = "MultiplayerInvitedNotification"
+                        self.repl_url = url
+                        self.repl_id = repl_annotations["id"]
+                        self.anchor_id = anchor["id"]
+                        self.super_self = super_self
+
+                    async def reply(self, body) -> None:
+                        if self.anchor_id:
+                            return await self.super_self.gql(
+                                "createChatMessage",
+                                vars={
+                                    "replId": self.repl_id,
+                                    "anchorId": self.anchor_id,
+                                    "annotationMessage": {
+                                        "id": str(uuid.uuid4()),
+                                        "text": body,
+                                    },
+                                },
+                            )
+                        else:
+
+                            self.anchor_id = await self.super_self.gql(
+                                "chatInit",
+                                {
+                                    "annotationAnchor": {
+                                        "id": str(uuid.uuid4()),
+                                        "replId": self.repl_id,
+                                        "isGeneral": True,
+                                        "isResolved": False,
+                                    },
+                                    "annotationMessage": {
+                                        "id": str(uuid.uuid4()),
+                                        "text": body,
+                                        "mentions": [],
+                                    },
+                                },
+                            )
+
+                ctx = CurrentCtx()
+                for i in dir(self):
+                    if not i.startswith("__") and not i.endswith("__"):
+                        setattr(ctx, i, getattr(self, i))
+                logger.info(
+                    f"{green}[FILE] BOT.py{end}\n{green}[INFO]{end} got invited to repl {url}"
+                )
+                self.multiplayer_repls.append(ctx)
+                await self._when_invited_to_repl(ctx)
 
         if flask_app is not None:
             Thread(
                 target=serve,
                 kwargs={"app": flask_app, "host": "0.0.0.0", "port": 8080},
                 daemon=daemon,
             ).start()
```

### Comparing `replit-bot-4.2.0/replit_bot/AsyncClient.py` & `replit-bot-4.2.1/replit_bot/AsyncClient.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.1/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/LICENSE` & `replit-bot-4.2.1/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/bot.py` & `replit-bot-4.2.1/replit_bot/bot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/client.py` & `replit-bot-4.2.1/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/html_default_templates.py` & `replit-bot-4.2.1/replit_bot/html_default_templates.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/param.py` & `replit-bot-4.2.1/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/post_ql.py` & `replit-bot-4.2.1/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/queries.js` & `replit-bot-4.2.1/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/queries.py` & `replit-bot-4.2.1/replit_bot/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,56 @@
     "getBountiesQuery": "query BountiesPageSearch($input: BountySearchInput!) {\n  bountySearch(input: $input) {\n    __typename\n    ... on BountySearchConnection {\n      items {\n        ...BountyCard\n        __typename\n      }\n      pageInfo {\n        hasNextPage\n        nextCursor\n        __typename\n      }\n      __typename\n    }\n    ... on UserError {\n      message\n      __typename\n    }\n    ... on UnauthorizedError {\n      message\n      __typename\n    }\n  }\n}\n\nfragment BountyCard on Bounty {\n  id\n  title\n  descriptionPreview\n  cycles\n  deadline\n  status\n  slug\n  solverPayout\n  timeCreated\n  applicationCount\n  solver {\n    id\n    username\n    image\n    url\n    __typename\n  }\n  user {\n    id\n    username\n    image\n    url\n    __typename\n  }\n  __typename\n}\n",
     "tipQuery": 'query TipRepl($id: String!) {\n  repl(id: $id) {\n    ... on Repl {\n      user {\n        ... on User {\n          id\n          ...TipSurfaceOwnerFragment\n          __typename\n        }\n        __typename\n      }\n      ...TipReplFragment\n      ...TopTipperReplLeaderboard\n      __typename\n    }\n    __typename\n  }\n  currentUser {\n    id\n    ...IsTippingAvailableForSender\n    __typename\n  }\n}\n\nfragment TipSurfaceOwnerFragment on User {\n  id\n  username\n  ...IsTippingAvailableForRecipient\n  __typename\n}\n\nfragment IsTippingAvailableForRecipient on User {\n  id\n  hasPrivacyRole\n  isVerified\n  isGated: gate(feature: "flag-tip-repl")\n  __typename\n}\n\nfragment TipReplFragment on Repl {\n  id\n  slug\n  user {\n    id\n    __typename\n  }\n  totalCyclesTips\n  currentUserTotalTips\n  __typename\n}\n\nfragment TopTipperReplLeaderboard on Repl {\n  id\n  topTippers {\n    ...TopTippersFragment\n    __typename\n  }\n  __typename\n}\n\nfragment TopTippersFragment on TipperUser {\n  user {\n    id\n    username\n    url\n    image\n    __typename\n  }\n  totalCyclesTipped\n  __typename\n}\n\nfragment IsTippingAvailableForSender on CurrentUser {\n  id\n  hasPrivacyRole\n  isVerified\n  __typename\n}\n',
     "reportUser": "mutation ReportUser($reportedUserId: Int, $reason: String!) {\n  createBoardReport(reportedUserId: $reportedUserId, reason: $reason) {\n    __typename\n    id\n    reportedUser {\n      id\n      __typename\n    }\n  }\n}\n",
     "changeBanner": "mutation CoverImageUpdate($input: SetUserCoverImageInput!) {\n  setUserCoverImage(input: $input) {\n    ... on CurrentUser {\n      id\n      ...CoverImageCurrentUser\n      __typename\n    }\n    __typename\n  }\n}\n\nfragment CoverImageCurrentUser on CurrentUser {\n  id\n  coverImage {\n    url\n    offsetY\n    __typename\n  }\n  __typename\n}\n",
     "createChatMessage": "mutation ThreadComment($replId: String!, $anchorId: String!, $annotationMessage: AnnotationMessageInput!, $highlight: AnnotationHighlightInput) {createAnnotationMessage(replId: $replId, anchorId: $anchorId, annotationMessage: $annotationMessage, highlight: $highlight) {...on AnnotationAnchor {id} ...on UserError {message}}}",
     "markMessageAsSeen": "mutation MarkMessagesSeen($replId: String!, $threadId: String) {markMessagesAsSeen(replId: $replId, threadId: $threadId) {...on AnnotationMessageList {messages {id anchor {id}}} ...on UserError {message}}}",
     "getReplAnnotations": "query Repl($url: String, $id: String) {repl(url: $url, id: $id) {...on Repl {id annotationAnchors {id isGeneral messages {id seen anchor {id} user {username bio} content {...on TextMessageContentType {text}}}}}}}",
+    "chatInit": """mutation CreateAnnotationAnchor($annotationAnchor: AnnotationAnchorInput!, $annotationMessage: AnnotationMessageInput, $highlight: AnnotationHighlightInput) {
+  createAnnotationAnchor(
+    annotationAnchor: $annotationAnchor
+    annotationMessage: $annotationMessage
+    highlight: $highlight
+  ) {
+    ... on UserError {
+      message
+      __typename
+    }
+    ... on AnnotationAnchor {
+      id
+      path
+      isResolved
+      isGeneral
+      messages {
+        id
+        user {
+          id
+          username
+        }
+        anchor {
+          id
+        }
+        timeCreated
+        content {
+          ... on TextMessageContentType {
+            text
+          }
+          ... on PreviewMessageContentType {
+            preview
+          }
+          ... on StatusMessageContentType {
+            status
+          }
+          __typename
+        }
+      }
+    }
+    __typename
+  }
+}""",
 }
 
 """
 import { GraphQL } from '@rayhanadev/replit-gql';
 import gql from 'graphql-tag';
 import * as fs from 'fs';
 const client = GraphQL()
```

### Comparing `replit-bot-4.2.0/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.1/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/replit_bot/utils/lines.py` & `replit-bot-4.2.1/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.0/setup.py` & `replit-bot-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'pyee>=9.0.4,<10.0.0',
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.0',
+    'version': '4.2.1',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.0/PKG-INFO` & `replit-bot-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.0
+Version: 4.2.1
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

