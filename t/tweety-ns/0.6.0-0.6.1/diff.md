# Comparing `tmp/tweety-ns-0.6.0.tar.gz` & `tmp/tweety-ns-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.6.0.tar", last modified: Mon Apr  3 16:27:15 2023, max compression
+gzip compressed data, was "tweety-ns-0.6.1.tar", last modified: Sat Apr  8 16:41:00 2023, max compression
```

## Comparing `tweety-ns-0.6.0.tar` & `tweety-ns-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-03 16:27:15.177344 tweety-ns-0.6.0/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-03 16:27:15.177635 tweety-ns-0.6.0/PKG-INFO
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      302 2022-10-22 17:49:03.000000 tweety-ns-0.6.0/README.md
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-0.6.0/pyproject.toml
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      671 2023-04-03 16:27:15.178781 tweety-ns-0.6.0/setup.cfg
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      767 2023-04-03 16:27:05.000000 tweety-ns-0.6.0/setup.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-03 16:27:15.149176 tweety-ns-0.6.0/src/
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-03 16:27:15.163336 tweety-ns-0.6.0/src/tweety/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       54 2023-02-16 05:38:51.000000 tweety-ns-0.6.0/src/tweety/__init__.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     7599 2023-02-17 05:07:11.000000 tweety-ns-0.6.0/src/tweety/bot.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    14631 2023-03-25 06:51:19.000000 tweety-ns-0.6.0/src/tweety/builder.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    18861 2023-02-16 11:46:04.000000 tweety-ns-0.6.0/src/tweety/exceptions_.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      282 2022-03-04 06:53:48.000000 tweety-ns-0.6.0/src/tweety/filters.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     2261 2023-04-03 14:41:39.000000 tweety-ns-0.6.0/src/tweety/http.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-03 16:27:15.169199 tweety-ns-0.6.0/src/tweety/types/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       58 2023-03-12 12:43:32.000000 tweety-ns-0.6.0/src/tweety/types/__init__.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     4906 2023-04-03 14:44:27.000000 tweety-ns-0.6.0/src/tweety/types/search.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    31246 2023-04-03 14:44:45.000000 tweety-ns-0.6.0/src/tweety/types/twDataTypes.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     3271 2023-04-03 14:44:51.000000 tweety-ns-0.6.0/src/tweety/types/usertweet.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       96 2023-03-13 06:35:02.000000 tweety-ns-0.6.0/src/tweety/utils.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-03 16:27:15.176081 tweety-ns-0.6.0/src/tweety_ns.egg-info/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-03 16:27:15.000000 tweety-ns-0.6.0/src/tweety_ns.egg-info/PKG-INFO
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      495 2023-04-03 16:27:15.000000 tweety-ns-0.6.0/src/tweety_ns.egg-info/SOURCES.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        1 2023-04-03 16:27:15.000000 tweety-ns-0.6.0/src/tweety_ns.egg-info/dependency_links.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       40 2023-04-03 16:27:15.000000 tweety-ns-0.6.0/src/tweety_ns.egg-info/requires.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        7 2023-04-03 16:27:15.000000 tweety-ns-0.6.0/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.881770 tweety-ns-0.6.1/
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-08 16:41:00.882073 tweety-ns-0.6.1/PKG-INFO
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      302 2022-10-22 17:49:03.000000 tweety-ns-0.6.1/README.md
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-0.6.1/pyproject.toml
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      671 2023-04-08 16:41:00.883072 tweety-ns-0.6.1/setup.cfg
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      767 2023-04-08 16:40:37.000000 tweety-ns-0.6.1/setup.py
+drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.851381 tweety-ns-0.6.1/src/
+drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.866647 tweety-ns-0.6.1/src/tweety/
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       54 2023-04-08 16:39:18.000000 tweety-ns-0.6.1/src/tweety/__init__.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     7599 2023-02-17 05:07:11.000000 tweety-ns-0.6.1/src/tweety/bot.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    14608 2023-04-08 16:31:32.000000 tweety-ns-0.6.1/src/tweety/builder.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    18861 2023-02-16 11:46:04.000000 tweety-ns-0.6.1/src/tweety/exceptions_.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      282 2022-03-04 06:53:48.000000 tweety-ns-0.6.1/src/tweety/filters.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     2261 2023-04-03 14:41:39.000000 tweety-ns-0.6.1/src/tweety/http.py
+drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.873328 tweety-ns-0.6.1/src/tweety/types/
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       58 2023-03-12 12:43:32.000000 tweety-ns-0.6.1/src/tweety/types/__init__.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     4906 2023-04-03 14:44:27.000000 tweety-ns-0.6.1/src/tweety/types/search.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    31494 2023-04-08 16:37:09.000000 tweety-ns-0.6.1/src/tweety/types/twDataTypes.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     3271 2023-04-03 14:44:51.000000 tweety-ns-0.6.1/src/tweety/types/usertweet.py
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       96 2023-03-13 06:35:02.000000 tweety-ns-0.6.1/src/tweety/utils.py
+drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.880563 tweety-ns-0.6.1/src/tweety_ns.egg-info/
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/PKG-INFO
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      495 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        1 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       40 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/requires.txt
+-rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        7 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.6.0/PKG-INFO` & `tweety-ns-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.6.0
+Version: 0.6.1
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-0.6.0/setup.cfg` & `tweety-ns-0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 0.6.0
+version = 0.6.1
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety-ns-0.6.0/setup.py` & `tweety-ns-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types'],
-    version='0.6.0',
+    version='0.6.1',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-0.6.0/src/tweety/bot.py` & `tweety-ns-0.6.1/src/tweety/bot.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.6.0/src/tweety/builder.py` & `tweety-ns-0.6.1/src/tweety/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     URL_GUEST_TOKEN = "https://api.twitter.com/1.1/guest/activate.json"
     URL_API_INIT = "https://twitter.com/i/api/1.1/branch/init.json"
     URL_USER_BY_SCREEN_NAME = "https://api.twitter.com/graphql/rePnxwe9LZ51nQ7Sn_xN_A/UserByScreenName"
     URL_USER_TWEETS = "https://twitter.com/i/api/graphql/OXXUyHfKYZ-xLx4NcL9-_Q/UserTweets"
     URL_USER_TWEETS_WITH_REPLIES = "https://twitter.com/i/api/graphql/nrdle2catTyGnTyj1Qa7wA/UserTweetsAndReplies"
     URL_TRENDS = "https://twitter.com/i/api/2/guide.json"
     URL_SEARCH = "https://twitter.com/i/api/2/search/adaptive.json"
-    URL_TWEET_DETAILS = "https://api.twitter.com/graphql/NNiD2K-nEYUfXlMwGCocMQ/TweetDetail"
+    URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/1oIoGPTOJN2mSjbbXlQifA/TweetDetail"
 
     def __init__(self, profile_url):
         self.username = profile_url.split("/")[-1] if profile_url else None
         self.user_id = None
         self.guest_token = None
 
     def _get_headers(self):
@@ -206,11 +206,11 @@
             params['cursor'] = cursor
 
         return self._build(self.URL_SEARCH, urlencode(params))
 
     @return_with_headers
     def tweet_detail(self, tweet_id):
         params = {
-            'variables': f'{{"focalTweetId":"{tweet_id}","with_rux_injections":false,"includePromotedContent":true,"withCommunity":true,"withQuickPromoteEligibilityTweetFields":true,"withBirdwatchNotes":false,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
-            'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
+            'variables': f'{{"focalTweetId":"{tweet_id}","with_rux_injections":false,"includePromotedContent":true,"withCommunity":true,"withQuickPromoteEligibilityTweetFields":true,"withBirdwatchNotes":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withVoice":true,"withV2Timeline":true}}',
+            'features': '{"blue_business_profile_image_shape_enabled":false,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"longform_notetweets_richtext_consumption_enabled":false,"responsive_web_enhance_cards_enabled":false}',
         }
         return self._build(self.URL_TWEET_DETAILS, urlencode(params))
```

### Comparing `tweety-ns-0.6.0/src/tweety/exceptions_.py` & `tweety-ns-0.6.1/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.6.0/src/tweety/http.py` & `tweety-ns-0.6.1/src/tweety/http.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.6.0/src/tweety/types/search.py` & `tweety-ns-0.6.1/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.6.0/src/tweety/types/twDataTypes.py` & `tweety-ns-0.6.1/src/tweety/types/twDataTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
+import warnings
 from dateutil import parser
 import openpyxl
 import dateutil
 
 try:
     import wget
-    import warnings
 except ModuleNotFoundError:
     warnings.warn(' "wget" not found in system ,you will not be able to download the medias')
 WORKBOOK_HEADERS = ['Created on', 'author', 'is_retweet', 'is_reply', 'tweet_id', 'tweet_body', 'language', 'likes',
                     'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
 
 
 def deprecated(func):
@@ -124,15 +124,16 @@
         text = self._get_tweet_text(original_tweet, is_retweet)
         is_quoted = self._is_quoted(original_tweet)
         quoted_tweet = self._get_quoted_tweet(is_quoted)
         is_reply = self._is_reply(original_tweet)
         is_sensitive = self._is_sensitive(original_tweet)
         reply_counts = self._get_reply_counts(original_tweet)
         quote_counts = self._get_quote_counts(original_tweet)
-        replied_to = self.__replied_to = self._get_reply_to(is_reply, original_tweet, )
+        replied_to = self.__replied_to = self._get_reply_to(is_reply, original_tweet)
+        bookmark_count = self._get_bookmark_count(original_tweet)
         vibe = self._get_vibe()
         views = self._get_views()
 
         return {
             "created_on": created_on,
             "author": author,
             "is_quoted": is_quoted,
@@ -156,14 +157,15 @@
             "media": self._get_tweet_media(original_tweet),
             "user_mentions": self._get_tweet_mentions(original_tweet),
             "urls": self._get_tweet_urls(original_tweet),
             "hashtags": self._get_tweet_hashtags(original_tweet),
             "symbols": self._get_tweet_symbols(original_tweet),
             "views": views,
             "reply_to": replied_to,
+            "bookmark_count": bookmark_count,
             "threads": [],
             "comments": []
         }
 
     def _get_id(self):
         if self.__raw_tweet.get("rest_id"):
             return self.__raw_tweet['rest_id']
@@ -201,19 +203,20 @@
                         if not self.__replied_to or self.__replied_to.id != tweet['rest_id']:
                             self.__formatted_tweet['threads' if tweetType == "SelfThread" else 'comments'].append(
                                 Tweet(None, tweet, self.http))
                     except KeyError as e:
                         pass
 
     def _get_quoted_tweet(self, is_quoted):
+        raw_tweet = None
         if is_quoted:
             raw_response = self.__raw_response
-            raw_tweet = None
             if self.__raw_tweet.get("quoted_status_result"):
                 raw_tweet = self.__raw_tweet['quoted_status_result']['result']
+                return Tweet(raw_response, raw_tweet, self.http)
             try:
                 if not raw_tweet and self.__raw_tweet.get("legacy"):
                     raw_tweet = self.__raw_tweet['legacy']['retweeted_status_result']['result']['quoted_status_result']['result']
                     return Tweet(raw_response, raw_tweet, self.http)
             except:
                 return None
 
@@ -342,14 +345,18 @@
 
         if not original_tweet['entities'].get("user_mentions"):
             return []
 
         return [ShortUser(user) for user in original_tweet['entities']['user_mentions']]
 
     @staticmethod
+    def _get_bookmark_count(original_tweet):
+        return original_tweet.get("bookmark_count", None)
+
+    @staticmethod
     def _get_tweet_urls(original_tweet):
         if not original_tweet.get("entities"):
             return []
 
         if not original_tweet['entities'].get("urls"):
             return []
 
@@ -586,21 +593,19 @@
             date = user["created_at"]
 
         return parser.parse(date) if date else None
 
     @staticmethod
     def _get_key(user, key):
         keyValue = None
-        print(user)
         if user.get("legacy"):
             keyValue = user['legacy'].get(key)
 
         if not keyValue and user.get(key):
             keyValue = user[key]
-        print(keyValue)
 
         return keyValue
 
 
 class Trends:
     def __init__(self, trends_dict):
         self.__dictionary = trends_dict
@@ -771,8 +776,7 @@
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
     def __repr__(self):
         return f"Coordinates(latitude={self.latitude}, longitude={self.longitude})"
 
-
```

### Comparing `tweety-ns-0.6.0/src/tweety/types/usertweet.py` & `tweety-ns-0.6.1/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.6.0/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.6.1/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.6.0
+Version: 0.6.1
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

