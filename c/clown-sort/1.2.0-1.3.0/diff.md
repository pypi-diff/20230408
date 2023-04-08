# Comparing `tmp/clown_sort-1.2.0.tar.gz` & `tmp/clown_sort-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.2.0.tar", max compression
+gzip compressed data, was "clown_sort-1.3.0.tar", max compression
```

## Comparing `clown_sort-1.2.0.tar` & `clown_sort-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1324 2023-04-03 20:19:04.170920 clown_sort-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.2.0/LICENSE
--rw-r--r--   0        0        0     6703 2023-03-21 17:32:52.245778 clown_sort-1.2.0/README.md
--rw-r--r--   0        0        0     3243 2023-03-01 08:49:45.644326 clown_sort-1.2.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     6380 2023-03-25 04:04:50.951504 clown_sort-1.2.0/clown_sort/config.py
--rw-r--r--   0        0        0     6946 2023-03-21 17:01:06.731825 clown_sort-1.2.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4090 2023-03-25 04:05:46.024955 clown_sort-1.2.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0      811 2023-03-01 06:48:04.940218 clown_sort-1.2.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0     8678 2023-03-25 02:16:44.968934 clown_sort-1.2.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3109 2023-02-27 05:37:46.609295 clown_sort-1.2.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     5286 2023-04-03 20:18:34.176472 clown_sort-1.2.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3098 2023-03-22 05:52:50.032785 clown_sort-1.2.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.2.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.2.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.2.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-02-22 15:45:18.161513 clown_sort-1.2.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     2725 2023-02-27 12:32:42.820775 clown_sort-1.2.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      167 2023-02-20 21:09:37.440942 clown_sort-1.2.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1441 2023-04-03 20:19:04.177253 clown_sort-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8107 1970-01-01 00:00:00.000000 clown_sort-1.2.0/setup.py
--rw-r--r--   0        0        0     7951 1970-01-01 00:00:00.000000 clown_sort-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-04-08 19:53:14.230615 clown_sort-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6799 2023-04-07 00:33:31.752002 clown_sort-1.3.0/README.md
+-rw-r--r--   0        0        0     3243 2023-03-01 08:49:45.644326 clown_sort-1.3.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     6481 2023-04-07 00:35:30.510105 clown_sort-1.3.0/clown_sort/config.py
+-rw-r--r--   0        0        0     7607 2023-04-07 00:25:54.119824 clown_sort-1.3.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4090 2023-03-25 04:05:46.024955 clown_sort-1.3.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0      811 2023-03-01 06:48:04.940218 clown_sort-1.3.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0     9023 2023-04-07 00:36:43.260639 clown_sort-1.3.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3109 2023-02-27 05:37:46.609295 clown_sort-1.3.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     5392 2023-04-07 17:58:30.359470 clown_sort-1.3.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3343 2023-04-07 00:34:34.095790 clown_sort-1.3.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-02-22 15:45:18.161513 clown_sort-1.3.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     2725 2023-02-27 12:32:42.820775 clown_sort-1.3.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      167 2023-02-20 21:09:37.440942 clown_sort-1.3.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1441 2023-04-08 19:53:08.440362 clown_sort-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 clown_sort-1.3.0/setup.py
+-rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 clown_sort-1.3.0/PKG-INFO
```

### Comparing `clown_sort-1.2.0/CHANGELOG.md` & `clown_sort-1.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # NEXT RELEASE
 
-# 1.2.0
+## 1.3.0
+* Ask for confirmation before overwriting files (`--yes-overwrite` option to skip the check)
+* Check if image's extracted text is already in the filename (important if rescanning)
+
+## 1.2.0
 * `--only-if-match` option
 * New crypto sort rules
 
 ## 1.1.0
 * Filenames for retweets
 * New crypto sort rules
```

### Comparing `clown_sort-1.2.0/LICENSE` & `clown_sort-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/README.md` & `clown_sort-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 The default is for the tool to run in "dry run" mode, meaning it doesn't actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**
 
 While every effort has been made to use Python's cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
+(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)
+
 ### Custom Sorting Rules
 The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
```

### Comparing `clown_sort-1.2.0/clown_sort/__init__.py` & `clown_sort-1.3.0/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/config.py` & `clown_sort-1.3.0/clown_sort/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     dry_run: bool = True
     manual_sort: bool = False
     only_if_match: bool = False
     leave_in_place: bool = False
     screenshots_only: bool = True
     delete_originals: bool = False
     rescan_sorted: bool = False
+    yes_overwrite: bool = False
     sort_rules: List[SortRule] = []
     filename_regex: re.Pattern
 
     @classmethod
     def configure(cls):
         """Parse arguments and configure."""
         if '--version' in sys.argv:
@@ -66,14 +67,15 @@
         destination_dir = Path(args.destination_dir or args.screenshots_dir).expanduser()
         Config.set_directories(screenshots_dir, destination_dir, rules_csvs)
         Config.filename_regex = re.compile(args.filename_regex)
         Config.leave_in_place = True if args.leave_in_place else False
         Config.only_if_match = True if args.only_if_match else False
         Config.delete_originals = True if args.delete_originals else False
         Config.rescan_sorted = True if args.rescan_sorted else False
+        Config.yes_overwrite = True if args.yes_overwrite else False
 
         if Config.leave_in_place and Config.delete_originals:
             Console().print("--leave-in-place and --delete-originals are mutually exclusive.", style='red')
             sys.exit()
 
         if args.show_rules:
             Console().print(cls._rules_table())
```

### Comparing `clown_sort-1.2.0/clown_sort/filename_extractor.py` & `clown_sort-1.3.0/clown_sort/filename_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     re.DOTALL | re.MULTILINE | re.IGNORECASE
 )
 
 REVEDDIT_REGEX = re.compile('Reveddit Real.?Time')
 SUBREDDIT_REGEX = re.compile('/r/(?P<subreddit>\\w+)|\\sse(lf|ir)\\.(?P<subreddit2>\\w+)')
 DUNE_ANALYTICS_REGEX = re.compile('Query results (.*) @\\w+')
 RETWEETED_REGEX = re.compile('(.*) Retweeted')
+MIN_LENGTH_FOR_DUPE_CHECK = 9
 
 
 class FilenameExtractor:
     def __init__(self, image_file: 'ImageFile') -> None:
         self.image_file = image_file
         self.text: Optional[str] = image_file.extracted_text()
         self.basename_length: int = len(image_file.basename)
@@ -46,44 +47,48 @@
         self.author: Optional[str] = None
         self.reply_to_account: Optional[str] = None
 
     def filename(self) -> str:
         """Examine self.text and decide on an appropriate filename."""
         if self.text is None:
             return self.image_file.basename
-        elif DUNE_ANALYTICS_REGEX.search(self.text):
+
+        if DUNE_ANALYTICS_REGEX.search(self.text):
             dune_match = DUNE_ANALYTICS_REGEX.search(self.text)
             query_title = self._strip_bad_chars(dune_match.group(1))
-            return 'Dune Analytics "' + query_title + '" ' + self.image_file.basename
+            filename_str = 'Dune Analytics "' + query_title + '" '
+            new_filename = filename_str + self.image_file.basename
         elif self._is_tweet() or self._is_reddit():
             if self._is_tweet():
                 filename_str = self._filename_str_for_tweet()
             else:
                 filename_str = self._filename_str_for_reddit()
 
             filename = f"{filename_str} {self.image_file.basename_without_ext}"
             filename = filename[0:-1] if filename.endswith('.') else filename
-            return filename + self.image_file.extname
+            new_filename = filename + self.image_file.extname
         elif self._is_reveddit():
-            filename = 'Reveddit '
+            filename_str = 'Reveddit '
             subreddit_match = SUBREDDIT_REGEX.search(self.text)
 
             if subreddit_match is not None:
-                filename += 'r_' + (subreddit_match.group('subreddit') or subreddit_match.group('subreddit2')) + ' '
+                filename_str += 'r_' + (subreddit_match.group('subreddit') or subreddit_match.group('subreddit2')) + ' '
 
-            return filename + self.image_file.basename
+            new_filename = filename_str + self.image_file.basename
         else:
-            filename = self._build_filename(
-                self.image_file.basename_without_ext,
-                self.text[0:self.available_char_count]
-            )
-            return filename + self.image_file.extname
+            filename_str = self.text[0:self.available_char_count]
+            new_filename = self._build_filename(self.image_file.basename_without_ext, filename_str)
+            new_filename += self.image_file.extname
+
+        # If we already seem to have scanned the file then just return the filename
+        if self._is_text_already_in_filename(filename_str):
+            log.warning(f"'{filename_str}' already appears in filename, not renaming.")
+            return self.image_file.basename
 
-    def _first_line(self) -> str:
-        return self.text.split('\n')[0]
+        return new_filename
 
     def _is_tweet(self) -> bool:
         """Return true if the text looks like a tweet."""
         return TWEET_REGEX.search(self.text) is not None and '@crypto_oracle' not in self.text
 
     def _is_retweet(self) -> bool:
         """Return true if the text looks like a retweet."""
@@ -163,7 +168,14 @@
         body = self._strip_bad_chars(body)
         body = body[0:self.available_char_count - len(filename_text) - 2].strip()
         return f'{filename_text} - "{body}"'.replace('  ', ' ')
 
     def _strip_bad_chars(self, text: str) -> str:
         """Remove chars that don't work well in filenames"""
         return re.sub('[^0-9a-zA-Z@.?_:\'" ()]+', '_', text)
+
+    def _is_text_already_in_filename(self, filename_str: str) -> bool:
+        """Check if the extracted text is already in the filename"""
+        return filename_str[0:100] in self.image_file.basename and len(filename_str) > MIN_LENGTH_FOR_DUPE_CHECK
+
+    def _first_line(self) -> str:
+        return self.text.split('\n')[0]
```

### Comparing `clown_sort-1.2.0/clown_sort/files/image_file.py` & `clown_sort-1.3.0/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/files/pdf_file.py` & `clown_sort-1.3.0/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/files/sortable_file.py` & `clown_sort-1.3.0/clown_sort/files/sortable_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os import path, remove
 from pathlib import Path
 from typing import List, Optional, Union
 
 from exiftool import ExifToolHelper
 from rich.console import Console, ConsoleOptions, RenderResult
 from rich.panel import Panel
+from rich.prompt import Confirm
 from rich.text import Text
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
 from clown_sort.util.filesystem_helper import copy_file_creation_time
 from clown_sort.util.logging import log
 from clown_sort.util.rich_helper import (bullet_text, indented_bullet, console,
@@ -68,14 +69,22 @@
                 destination_dir = Config.sorted_screenshots_dir.joinpath(folder)
 
                 if not destination_dir.is_dir() and not Config.dry_run:
                     log.info(f"Creating subdirectory '{destination_dir}'...")
                     destination_dir.mkdir()
 
             destination_path = self.sort_destination_path(folder)
+
+            if destination_path.exists():
+                console.print(f"\nFile '{destination_path.name}' already exists in '{folder}/'!", style='blink')
+
+                if not (Config.yes_overwrite or Confirm.ask(f"Overwrite?")):
+                    console.print("Skipping...")
+                    continue
+
             self._paths_of_sorted_copies.append(destination_path)
             self.copy_file_to_sorted_dir(destination_path)
 
         if Config.leave_in_place:
             console.print(bullet_text(Text('Leaving in place...', style='dim')))
             return
```

### Comparing `clown_sort-1.2.0/clown_sort/sort_selector.py` & `clown_sort-1.3.0/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.3.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 1mdb,1mdb|jho[-_\s]*low|Victor[-_\s]*Hoo
 3ac,3ac|Three[-_\s]*Arrows[-_\s]*Capital|su[-_\s]*zhu|zhu[-_\s]*su|kyle[-_\s]*davies
 A16Z,a16z|andreessen|packym|arianna[-_\s1]*simpson
 Aave,aave
 AAX,\baax
 Arbitrum,Arbitrum|[$#]ARB\b
 Art,occult
-Avalanche,Avax|avalanche
-Banks,\$CUBI|Customers[-_\s]*Ban(k|corp)|SEBA[^a-z]|MCB\b|MCBankNY|Metropolitan[-_\s]*Community|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank
+Avalanche,\bAvax|avalanche
+Banks,\$CUBI|Customers[-_\s]*Ban(k|corp)|SEBA[^a-z]|MCB\b|MCBankNY|Metropolitan[-_\s]*Community|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group
 Bankless,Bankless
 Binary Options,binary[-_\s]*options
-Binance,binance|biconomy|bnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD
+Binance,binance|biconomy|bnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD|\boztures|Kaiser[-_\s]*Ng
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bitmain,Bitmain
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s]*Lai
 Bitzlato,Bitzlato
 Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna
@@ -80,24 +80,25 @@
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s]*Cotten
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,\$RIOT|Riot[-\s_]*Block
 Safemoon,Safemoon
+Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s]*Bank|Signet
 Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
 Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|[\s#]SEN[^\w]|Rebecca[-_\s]*Rettig
 Solana,Solana|Serum
 TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
 Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|bitfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT
 Tornado Cash,tornado\s*cash
 Transactive Systems UAB,Transactive
-Tron,\stron\s|tron(block|\s*)?chain|trondao
+Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s]*sacks|\bthiel\b|sequoia|founders[-_\s]*fund
 Voyager,voyager
 Wallet Addresses BCH,bitcoincash:q.*\b
 Wallet Addresses Bitcoin,(bc1|[13])[a-zA-HJ-NP-Z0–9]{25,39}\b
 Wallet Addresses Cardano,addr1[a-z0–9]+\b
```

### Comparing `clown_sort-1.2.0/clown_sort/util/argument_parser.py` & `clown_sort-1.3.0/clown_sort/util/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
                     metavar='RULES_FILE.CSV',
                     help=f"sorting rules can be supplied more than once (use string '{CRYPTO}' to use the defaults)")
 
 parser.add_argument('-f', '--filename-regex',
                     help='filename regular expression',
                     default=DEFAULT_FILENAME_REGEX.pattern)
 
+parser.add_argument('-y', '--yes-overwrite', action='store_true',
+                    help='skip confirmation prompt and always overwrite if a file with the same name already exists',
+                    default=DEFAULT_FILENAME_REGEX.pattern)
+
 parser.add_argument('--rescan-sorted', action='store_true',
                     help="rescan already sorted files (useful if you updated your sorting rules)")
 
 parser.add_argument('--delete-originals', action='store_true',
                     help="don't preserve the original screenshots in the Processed/ folder")
 
 parser.add_argument('--show-rules', action='store_true',
```

### Comparing `clown_sort-1.2.0/clown_sort/util/constants.py` & `clown_sort-1.3.0/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.3.0/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/clown_sort/util/rich_helper.py` & `clown_sort-1.3.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.2.0/pyproject.toml` & `clown_sort-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.2.0"
+version = "1.3.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.2.0/setup.py` & `clown_sort-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 entry_points = \
 {'console_scripts': ['set_screenshot_timestamps = '
                      'clown_sort:set_screenshot_timestamps',
                      'sort_screenshots = clown_sort:sort_screenshots']}
 
 setup_kwargs = {
     'name': 'clown-sort',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'Sort screenshots based on rules or through individual review.',
-    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests. Only requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
+    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests. Only requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
     'author': 'Michel de Cryptadamus',
     'author_email': 'michel@cryptadamus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michelcrypt4d4mus/clown_sort',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clown_sort-1.2.0/PKG-INFO` & `clown_sort-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.2.0
+Version: 1.3.0
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -111,14 +111,16 @@
 The default is for the tool to run in "dry run" mode, meaning it doesn't actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**
 
 While every effort has been made to use Python's cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
+(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)
+
 ### Custom Sorting Rules
 The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
```

