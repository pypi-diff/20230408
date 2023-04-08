# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.2.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.1.tar` & `nonebot_plugin_l4d2_server-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.1/LICENSE
--rw-r--r--   0        0        0    20158 2023-04-03 20:20:36.574468 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     4897 2023-03-26 04:49:59.448001 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     4856 2023-04-03 20:13:13.878383 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1666 2023-03-06 09:04:41.376881 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     5829 2023-03-01 12:23:49.342774 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html
--rw-r--r--   0        0        0     6206 2023-03-05 16:25:01.648005 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6417 2023-02-27 15:03:03.981712 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1595 2023-03-02 15:28:44.743644 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9110 2023-03-09 03:44:26.265121 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3891 2023-03-27 06:41:16.031721 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3447 2023-03-18 17:24:53.495140 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-03 20:05:30.225988 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10404 2023-03-26 05:16:08.141654 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     3431 2023-04-01 15:46:38.537804 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     5227 2023-04-01 04:26:08.217691 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    17566 2023-04-01 15:50:42.713700 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2188 2023-02-14 16:07:15.000000 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8803 2023-03-25 16:41:28.201956 nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1512 2023-04-03 20:22:56.127020 nonebot_plugin_l4d2_server-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    10854 2023-04-03 20:20:26.673950 nonebot_plugin_l4d2_server-0.4.1/README.md
--rw-r--r--   0        0        0    12648 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.1/setup.py
--rw-r--r--   0        0        0    12624 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.2/LICENSE
+-rw-r--r--   0        0        0    16800 2023-04-08 18:21:31.335607 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8079 2023-04-08 18:33:45.829557 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     4965 2023-04-08 18:09:47.583660 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1666 2023-03-06 09:04:41.376881 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     5829 2023-03-01 12:23:49.342774 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html
+-rw-r--r--   0        0        0     6206 2023-03-05 16:25:01.648005 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6417 2023-02-27 15:03:03.981712 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1595 2023-03-02 15:28:44.743644 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0     9110 2023-03-09 03:44:26.265121 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3891 2023-03-27 06:41:16.031721 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-08 18:08:59.052656 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10656 2023-04-08 15:58:37.818041 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     3423 2023-04-08 11:56:34.551084 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/config.py
+-rw-r--r--   0        0        0     6395 2023-04-08 18:36:15.718548 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2188 2023-02-14 16:07:15.000000 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8205 2023-04-08 18:24:13.271797 nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1485 2023-04-08 18:36:26.349581 nonebot_plugin_l4d2_server-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    11067 2023-04-08 18:35:22.067066 nonebot_plugin_l4d2_server-0.4.2/README.md
+-rw-r--r--   0        0        0    12829 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.2/setup.py
+-rw-r--r--   0        0        0    12732 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/LICENSE` & `nonebot_plugin_l4d2_server-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,43 +10,46 @@
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
+from typing import Tuple,Union,List
+from time import sleep
+
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg,RawCommand,CommandStart
+from nonebot import get_driver, require
+from nonebot.plugin import PluginMetadata
 
-from typing import Tuple,Union,List
-from time import sleep
-import asyncio
 
 from .config import *
 from .utils import *
 from .command import *
 from .l4d2_image.steam import url_to_byte,url_to_byte_name
-from nonebot.plugin import PluginMetadata
+
 from .l4d2_data import sq_L4D2
-from nonebot import get_driver, require
+
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 
 from .txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
-# from .l4d2_web import web,webUI
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
+from .l4d2_web import web,webUI
+
 driver = get_driver()
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Umamusume-Agnes-Digital <Z735803792@163.com>",
@@ -56,173 +59,168 @@
 
 """相当于启动就检查数据库"""
 
 
 @up.handle()
 async def _(matcher:Matcher,event: NoticeEvent):
     args = event.dict()
-    map_path = Path(l4_file[CHECK_FILE],vpk_path)
     if args['notice_type'] != 'offline_file':
         matcher.set_arg('txt',args)
-    else:
+        return
+    l4_file_path = l4_file[CHECK_FILE]
+    map_path = Path(l4_file_path, vpk_path)
     # 检查下载路径是否存在
-    # logger.info('检查下载路径是否存在')
-        l4_file_path = l4_file[CHECK_FILE]
-        # 检查下载路径是否存在
-        logger.info(l4_file_path)
-        if not Path(l4_file_path).exists():
-            await up.finish("你填写的路径不存在辣")
-        if not Path(map_path).exists():
-            await up.finish("这个路径并不是求生服务器的路径，请再看看罢")
-            # args = event.dict()
-        # if args['notice_type'] != 'offline_file':  # 群聊值响应超管
-        #     return
-        url = args['file']['url']
-        name: str = args['file']['name']
-        # user_id = txt['user_id']
-        # 如果不符合格式则忽略
-        await up.send('已收到文件，开始下载')
-        sleep(1)   # 等待一秒防止因为文件名获取出现BUG
-        vpk_files = await updown_l4d2_vpk(map_path,name,url)
-        if vpk_files:
-            logger.info('检查到新增文件')
-            mes = "解压成功，新增以下几个vpk文件"
-        else:
-            mes = "你可能上传了相同的文件，或者解压失败了捏"
-                
-        await up.finish(mes_list(mes,vpk_files))
+    if not Path(l4_file_path).exists():
+        await matcher.finish("你填写的路径不存在辣")
+        return
+    if not Path(map_path).exists():
+        await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
+        return
+    url = args['file']['url']
+    name: str = args['file']['name']
+    # 如果不符合格式则忽略
+    await up.send('已收到文件，开始下载')
+    sleep(1)   # 等待一秒防止因为文件名获取出现BUG
+    vpk_files = await updown_l4d2_vpk(map_path,name,url)
+    if vpk_files:
+        mes = "解压成功，新增以下几个vpk文件"
+        await matcher.finish(mes_list(mes,vpk_files))
+    else:
+        await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
+
 
 
-@up.got("is_sure",prompt="请选择上传位置（输入阿拉伯数字)")    
+@up.got("is_sure", prompt="请选择上传位置（输入阿拉伯数字)")    
 async def _(matcher: Matcher):
     args = matcher.get_arg('txt')
-    map_path = Path(l4_file[CHECK_FILE],vpk_path)
-    sleep(1)
     if not args:
         await matcher.finish('获取文件出错辣，再试一次吧')
-    # args = txt.dict()
+
     is_sure = str(matcher.get_arg('is_sure')).strip()
     if not is_sure.isdigit():
         await matcher.finish('已取消上传')
     file_number = len(l4_file)
     is_sure = int(is_sure)
     if is_sure > file_number or is_sure <= 0:
         await matcher.finish('没有该序号')
     l4_file_path = l4_file[is_sure - 1]
-    
+
+    map_path = Path(l4_file_path, vpk_path)
+
     # 检查下载路径是否存在
-    logger.info(l4_file_path)
     if not Path(l4_file_path).exists():
-        await up.finish("你填写的路径不存在辣")
-    if not Path(map_path).exists():
-        await up.finish("这个路径并不是求生服务器的路径，请再看看罢")
-    # args = event.dict()
-    # if args['notice_type'] != 'offline_file':  # 群聊值响应超管
+        await matcher.finish("你填写的路径不存在辣")
+    if not map_path.exists():
+        await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
+
     url = args['file']['url']
-    name: str = args['file']['name']
-    # user_id = args['user_id']
+    name = args['file']['name']
     # 如果不符合格式则忽略
     if not name.endswith(file_format):
         return
-    await up.send('已收到文件，开始下载')
+
+    await matcher.send('已收到文件，开始下载')
     sleep(1)   # 等待一秒防止因为文件名获取出现BUG
-    vpk_files = await updown_l4d2_vpk(Path(l4_file_path,vpk_path),name,url)
+    vpk_files = await updown_l4d2_vpk(map_path, name, url)
+
     if vpk_files:
         logger.info('检查到新增文件')
         mes = "解压成功，新增以下几个vpk文件"
-    elif vpk_files == None:
-        await up.finish('文件错误')
+    elif vpk_files is None:
+        await matcher.finish('文件错误')
     else:
         mes = "你可能上传了相同的文件，或者解压失败了捏"
-    await up.finish(mes_list(mes,vpk_files))
+
+    await matcher.finish(mes_list(mes, vpk_files))
+
     
 @find_vpk.handle()
-async def _(bot:Bot,event: MessageEvent):
+async def _(bot:Bot,event: MessageEvent,matcher: Matcher):
     name_vpk = []
     map_path = Path(l4_file[CHECK_FILE],vpk_path)
     name_vpk = get_vpk(name_vpk,map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ''
     msg = mes_list(msg,name_vpk).replace(" ","")
     
-    await find_vpk.finish(mode_txt_to_img(mes,msg))
+    await matcher.finish(mode_txt_to_img(mes,msg))
 
 @del_vpk.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num",args)
 
 @del_vpk.got("num",prompt="你要删除第几个序号的地图(阿拉伯数字)")
-async def _(tag:int = ArgPlainText("num")):
+async def _(matcher: Matcher,tag:int = ArgPlainText("num")):
     map_path = Path(l4_file[CHECK_FILE],vpk_path)
     vpk_name = del_map(tag,map_path)
-    await del_vpk.finish('已删除地图：' + vpk_name)
+    await matcher.finish('已删除地图：' + vpk_name)
     
 @rename_vpk.handle()
-async def _(matched: Tuple[int,str, str] = RegexGroup(),):
+async def _(matcher:Matcher,matched: Tuple[int,str, str] = RegexGroup(),):
     num,useless,rename = matched
     map_path = Path(l4_file[CHECK_FILE],vpk_path)
     logger.info('检查是否名字是.vpk后缀')
     if not rename.endswith('.vpk'):
         rename = rename + '.vpk'
     logger.info('尝试改名')
     try:
         map_name = rename_map(num,rename,map_path)
         if map_name:
-            await rename_vpk.finish('改名成功\n原名:'+ map_name +'\n新名称:' + rename)
+            await matcher.finish('改名成功\n原名:'+ map_name +'\n新名称:' + rename)
     except ValueError:
-        await rename_vpk.finish('参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称')
+        await matcher.finish('参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称')
         
 @anne_player.handle()
-async def _(event:MessageEvent,args:Message = CommandArg()):
+async def _(matcher:Matcher,event:MessageEvent,args:Message = CommandArg()):
     name = args.extract_plain_text()
     name = name.strip()
     at = await get_message_at(event.json())
     usr_id = at_to_usrid(at)
     if usr_id == None:
         usr_id = event.user_id
     # 没有参数则从db里找数据
     msg = await search_anne(name,usr_id)
     if type(msg)==str:
-        await anne_player.finish(msg)
+        await matcher.finish(msg)
     else:
-        await anne_player.finish(MessageSegment.image(msg)) 
+        await matcher.finish(MessageSegment.image(msg)) 
     
 @anne_bind.handle()
-async def _(event:MessageEvent,args:Message = CommandArg()):
+async def _(matcher:Matcher,event:MessageEvent,args:Message = CommandArg()):
     tag = args.extract_plain_text()
     tag = tag.strip()
     if tag=="" or tag.isspace():
-        await anne_bind.finish("虚空绑定?")
+        await matcher.finish("虚空绑定?")
     usr_id = str(event.user_id)
     nickname = event.sender.card or event.sender.nickname
     msg = await bind_steam(usr_id,tag,nickname)
-    await anne_bind.finish(msg)
+    await matcher.finish(msg)
 
 @del_bind.handle()
-async def _(event:MessageEvent):
+async def _(matcher:Matcher,event:MessageEvent):
     usr_id = event.user_id
-    await del_bind.finish(name_exist(usr_id))
+    await matcher.finish(name_exist(usr_id))
 
 @rcon_to_server.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("command",args)
 
 @rcon_to_server.got("command",prompt="请输入向服务器发送的指令")
-async def _(tag:str = ArgPlainText("command")):
+async def _(matcher:Matcher,tag:str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     if l4_image:
-        await rcon_to_server.finish(mode_txt_to_img('服务器返回',msg))
+        await matcher.finish(mode_txt_to_img('服务器返回',msg))
     else:
-        await rcon_to_server.finish(msg,reply_message = True)
+        await matcher.finish(msg,reply_message = True)
         
 
 # 连续rcon连接
 # @connect_rcon.handle()
 # async def _(State:T_State,args:Message = CommandArg()):
 #     msg = args.extract_plain_text()
     # client = RCONClient(l4_host[CHECK_FILE], l4_port[CHECK_FILE], l4_rcon[CHECK_FILE])
@@ -237,72 +235,72 @@
     # client:RCONClient = State['client']
 
     # await client.close()
     # await connect_rcon.finish('聊天结束...')
         
         
 @check_path.handle()
-async def _(args:Message = CommandArg()):
+async def _(matcher:Matcher,args:Message = CommandArg()):
     global CHECK_FILE
     msg = args.extract_plain_text()
     if msg.startswith('切换'):
         msg_number = int(''.join(msg.replace('切换', ' ').split()))
         if msg_number > len(l4_file) or msg_number < 0:
-            await check_path.send('没有这个序号的路径呐')
+            await matcher.send('没有这个序号的路径呐')
         else:
             CHECK_FILE = msg_number - 1
             now_path = l4_file[CHECK_FILE]
-            await check_path.send(f'已经切换路径为\n{str(CHECK_FILE+1)}、{now_path}')
+            await matcher.send(f'已经切换路径为\n{str(CHECK_FILE+1)}、{now_path}')
     else: 
         now_path = l4_file[CHECK_FILE]
-        await check_path.send(f'当前的路径为\n{str(CHECK_FILE+1)}、{now_path}')
+        await matcher.send(f'当前的路径为\n{str(CHECK_FILE+1)}、{now_path}')
         
         
 @queries.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("ip",args)
 
 @queries.got("ip",prompt="请输入ip,格式如中括号内【127.0.0.1】【114.51.49.19:1810】")
-async def _(tag:str = ArgPlainText("ip")):
+async def _(matcher:Matcher,tag:str = ArgPlainText("ip")):
     ip = split_maohao(tag)
     msg = await queries_server(ip)
-    await queries.finish(msg)
+    await matcher.finish(msg)
     
 
 @add_queries.handle()
-async def _(event:GroupMessageEvent,args:Message = CommandArg()):
+async def _(matcher:Matcher,event:GroupMessageEvent,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg)==0:
-        await add_queries.finish('请在该指令后加入参数，例如【114.51.49.19:1810】')
+        await matcher.finish('请在该指令后加入参数，例如【114.51.49.19:1810】')
     [host,port] = split_maohao(msg)
     group_id = event.group_id
     msg = await add_ip(group_id,host,port)
-    await add_queries.finish(msg)
+    await matcher.finish(msg)
 
 @del_queries.handle()
 async def _(event:GroupMessageEvent,matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if not msg.isdigit():
-        await del_queries.finish('请输入正确的序号数字')
+        await matcher.finish('请输入正确的序号数字')
     group_id = event.group_id
     msg = await del_ip(group_id,msg)
-    await del_queries.finish(msg)
+    await matcher.finish(msg)
    
 @show_queries.handle()
-async def _(event:GroupMessageEvent):
+async def _(matcher:Matcher,event:GroupMessageEvent):
     group_id = event.group_id
     msg = await show_ip(group_id)
     if not msg:
-        await show_queries.finish("当前没有启动的服务器捏")
+        await matcher.finish("当前没有启动的服务器捏")
     if type(msg) == str:
-        await show_queries.finish(msg)
+        await matcher.finish(msg)
     else:
-        await show_queries.finish(MessageSegment.image(msg))
+        await matcher.finish(MessageSegment.image(msg))
 
 @join_server.handle()
 async def _(args:Message = CommandArg()):
     msg = args.extract_plain_text()
     url = await get_number_url(msg)
     await join_server.finish(url)
     
@@ -310,18 +308,18 @@
 @up_workshop.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("ip",args)
     
 @up_workshop.got("ip",prompt="请输入创意工坊网址或者物品id")
-async def _(state:T_State,tag:str = ArgPlainText("ip")):
+async def _(matcher:Matcher,state:T_State,tag:str = ArgPlainText("ip")):
     msg = await workshop_msg(tag)
     if not msg:
-        await up_workshop.finish('没有这个物品捏')
+        await matcher.finish('没有这个物品捏')
     elif type(msg) == dict:
         pic = await url_to_byte(msg['图片地址'])
         message = ''
         for item,value in msg.items():
             if item in ['图片地址','下载地址','细节']:
                 continue
             message += item + ':' + value + '\n'
@@ -345,47 +343,47 @@
     is_sure = str(state["is_sure"])
     if is_sure == 'yes':
         data_dict:Union[dict,List[dict]] = state['dic']
         if type(data_dict) == dict:
             logger.info('开始上传')
             data_file = await url_to_byte(data_dict['下载地址'])
             file_name = data_dict['名字']+ '.vpk'
-            await up_workshop.send('获取地址成功，尝试上传')
+            await matcher.send('获取地址成功，尝试上传')
             await upload_file(bot, event, data_file, file_name)
         else:
             logger.info('开始上传')
             for data_one in data_dict:
                 data_file = await url_to_byte(data_one['下载地址'])
                 await all_zip_to_one
             file_name = data_one['名字']+ '.vpk'
             await upload_file(bot, event, data_file, file_name)
     else:
-        await up_workshop.finish('已取消上传')
+        await matcher.finish('已取消上传')
     
 
 
 @updata.handle()
-async def _(args:Message = CommandArg()):
+async def _(matcher:Matcher,args:Message = CommandArg()):
     """更新"""
     msg = args.extract_plain_text()
     if not msg:
         load_josn()
         reload_ip()
-        await updata.finish('已更新缓存数据')
+        await matcher.finish('已更新缓存数据')
     else:
         message = await write_json(msg)
-        await updata.finish(message)
+        await matcher.finish(message)
   
 
             
 @vtf_make.handle()
 async def _(matcher:Matcher,state:T_State,args:Message = CommandArg()):
     msg:str = args.extract_plain_text()
     if msg not in ['拉伸','填充','覆盖','']:
-        await vtf_make.finish('错误的图片处理方式')
+        await matcher.finish('错误的图片处理方式')
     if msg == '':
         msg = '拉伸'
     state['way'] = msg
     logger.info('方式',msg)
     
 @vtf_make.got("image",prompt="请发送喷漆图片")
 async def _(bot:Bot,event:MessageEvent,state:T_State,tag = Arg("image")):
@@ -400,142 +398,60 @@
     usr_id = event.user_id
     file_name:str = str(usr_id) + '.vtf'
     await upload_file(bot, event, img_bytes, file_name)
 
 
 
 @smx_file.handle()
-async def _():
+async def _(matcher:Matcher,):
     smx_path = Path(l4_file[CHECK_FILE],"left4dead2/addons/sourcemod/plugins")
     smx_list = []
     name_smx = get_vpk(smx_list,smx_path,file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ''
     msg = mes_list(msg,name_smx).replace(" ","")
-    await find_vpk.finish(mode_txt_to_img(mes,msg))
+    await matcher.finish(mode_txt_to_img(mes,msg))
     
 @search_api.handle()
-async def _(state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
+async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
     msg:str = args.extract_plain_text()
     # if msg.startswith('代码'):
         # 建图代码返回三方图信息
-    data = await seach_map(msg,l4_qq,l4_key)
+    data = seach_map(msg,l4_qq,l4_key)
     # else:
     if type(data) == str:
-        await search_api.finish(data)
+        await matcher.finish(data)
     else:
         state['maps'] = data
-        await search_api.send(await map_dict_to_str(data))
+        await matcher.send(await map_dict_to_str(data))
         
 @search_api.got("is_sure",prompt='如果需要上传，请发送 "yes"')    
-async def _(bot:Bot,event:GroupMessageEvent,state:T_State):
+async def _(matcher:Matcher,bot:Bot,event:GroupMessageEvent,state:T_State):
     is_sure = str(state["is_sure"])
     if is_sure == 'yes':
         data_dict:dict = state['maps'][0]
         if type(data_dict) == dict:
             logger.info('开始上传')
             if l4_only:
                 data_file,file_name = await url_to_byte_name(data_dict['url'],'htp')
             else:
                 data_file,file_name = await url_to_byte_name(data_dict['url'])
             if data_file:
-                await search_api.send('获取地址成功，尝试上传')
+                await matcher.send('获取地址成功，尝试上传')
                 await upload_file(bot, event, data_file, file_name)
             else:
                 await search_api.send('出错了，原因是下载链接不存在')
         else:
             logger.info('开始上传')
             for data_one in data_dict:
                 data_file,file_name = await url_to_byte_name(data_one['url'])
                 await all_zip_to_one
                 await upload_file(bot, event, data_file, file_name)
     else:
-        await search_api.finish('已取消上传')
-        
-
-@driver.on_startup
-async def _():
-    global ALL_HOST
-    global ANNE_IP
-    if l4_tag == None:
-        pass
-    else:
-        ALL_HOST.update(await seach_map(l4_tag,l4_qq,l4_key,'ip'))
-        def count_ips(ip_dict:dict):
-            for key, value in ip_dict.items():
-                if key == 'error_':
-                    continue
-                count = len(value)
-                logger.info(f'已加载：{key} | {count}个')
-                if key == '云':
-                    ANNE_IP = {key:value}
-        count_ips(ALL_HOST)
-        ip_anne_list=[] 
-        try:
-            ips = ALL_HOST['云']
-            ip_anne_list = []
-            for one_ip in ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_anne_list.append((one_ip['id'],host,port))
-        except KeyError:
-            pass
-    get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
-    @get_ip.handle()
-    async def _(start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg(),):
-        if start:
-            command.replace(start,'')
-        if command == 'anne':
-            command = '云'
-        msg:str = args.extract_plain_text()
-        if not msg:
-            # 以图片输出全部当前
-            this_ips = ALL_HOST[command]
-            ip_list = []
-            for one_ip in this_ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_list.append((one_ip['id'],host,port))
-            img = await qq_ip_queries_pic(ip_list)
-            if img:
-                await get_ip.finish(MessageSegment.image(img)) 
-            else:
-                await get_ip.finish("服务器无响应")
-        else:
-            if not msg[0].isdigit():
-                if any(mode in msg for mode in gamemode_list):
-                    pass
-                else:
-                    return
-            message = await json_server_to_tag_dict(command,msg)
-            if len(message) == 0:
-                # 关键词不匹配，忽略
-                return
-            ip = str(message['ip'])
-            logger.info(ip)
-            try:
-                msg= await get_anne_server_ip(ip)
-                await get_ip.finish(msg)
-            except (OSError,asyncio.exceptions.TimeoutError):
-                await get_ip.finish('服务器无响应')
-                
-    @tan_jian.handle()
-    async def _(event:MessageEvent):
-        await tan_jian.send('正在寻找牢房...')
-        msg = await get_tan_jian(ip_anne_list,1)
-        await tan_jian.finish(msg)  
+        await matcher.finish('已取消上传')
         
-    @prison.handle()
-    async def _(event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,2)
-        await tan_jian.finish(msg)
 
-    @open_prison.handle()
-    async def _(event:MessageEvent):
-
-        msg = await get_tan_jian(ip_anne_list,3)
-        await tan_jian.finish(msg)
-    
-            
 @driver.on_shutdown
 async def close_db():
     """关闭数据库"""
     sq_L4D2._close()
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,167 +138,174 @@
 00000890: 6e66 6967 2e6c 345f 6b65 790d 0a65 7863  nfig.l4_key..exc
 000008a0: 6570 743a 0d0a 2020 2020 6c34 5f6b 6579  ept:..    l4_key
 000008b0: 3a73 7472 203d 2022 220d 0a0d 0a74 7279  :str = ""....try
 000008c0: 3a0d 0a20 2020 206c 345f 7461 673a 6c69  :..    l4_tag:li
 000008d0: 7374 203d 2064 7269 7665 722e 636f 6e66  st = driver.conf
 000008e0: 6967 2e6c 345f 7461 670d 0a65 7863 6570  ig.l4_tag..excep
 000008f0: 743a 0d0a 2020 2020 6c34 5f74 6167 203d  t:..    l4_tag =
-00000900: 204e 6f6e 650d 0a23 20e5 bcba e588 b6e8   None..# .......
-00000910: bdac 6c69 7374 0d0a 6966 2074 7970 6528  ..list..if type(
-00000920: 6c34 5f74 6167 2920 3d3d 2073 7472 206f  l4_tag) == str o
-00000930: 7220 6c69 7374 3a0d 0a20 2020 206c 345f  r list:..    l4_
-00000940: 6c69 7374 203d 205b 6c34 5f66 696c 652c  list = [l4_file,
-00000950: 206c 345f 7374 6561 6d69 642c 206c 345f   l4_steamid, l4_
-00000960: 686f 7374 2c20 6c34 5f70 6f72 742c 206c  host, l4_port, l
-00000970: 345f 7263 6f6e 2c20 6c34 5f6d 6173 7465  4_rcon, l4_maste
-00000980: 722c 6c34 5f74 6167 5d0d 0a20 2020 206c  r,l4_tag]..    l
-00000990: 345f 6c69 7374 203d 205b 6173 742e 6c69  4_list = [ast.li
-000009a0: 7465 7261 6c5f 6576 616c 2869 2920 6966  teral_eval(i) if
-000009b0: 2069 7369 6e73 7461 6e63 6528 692c 2073   isinstance(i, s
-000009c0: 7472 2920 656c 7365 2069 2066 6f72 2069  tr) else i for i
-000009d0: 2069 6e20 6c34 5f6c 6973 745d 0d0a 2020   in l4_list]..  
-000009e0: 2020 6c34 5f66 696c 652c 206c 345f 7374    l4_file, l4_st
-000009f0: 6561 6d69 642c 206c 345f 686f 7374 2c20  eamid, l4_host, 
-00000a00: 6c34 5f70 6f72 742c 206c 345f 7263 6f6e  l4_port, l4_rcon
-00000a10: 2c20 6c34 5f6d 6173 7465 722c 206c 345f  , l4_master, l4_
-00000a20: 7461 673d 206c 345f 6c69 7374 0d0a 656c  tag= l4_list..el
-00000a30: 7365 3a0d 0a20 2020 206c 345f 6c69 7374  se:..    l4_list
-00000a40: 203d 205b 6c34 5f66 696c 652c 206c 345f   = [l4_file, l4_
-00000a50: 7374 6561 6d69 642c 206c 345f 686f 7374  steamid, l4_host
-00000a60: 2c20 6c34 5f70 6f72 742c 206c 345f 7263  , l4_port, l4_rc
-00000a70: 6f6e 2c20 6c34 5f6d 6173 7465 725d 0d0a  on, l4_master]..
-00000a80: 2020 2020 6c34 5f6c 6973 7420 3d20 5b61      l4_list = [a
-00000a90: 7374 2e6c 6974 6572 616c 5f65 7661 6c28  st.literal_eval(
-00000aa0: 6929 2069 6620 6973 696e 7374 616e 6365  i) if isinstance
-00000ab0: 2869 2c20 7374 7229 2065 6c73 6520 6920  (i, str) else i 
-00000ac0: 666f 7220 6920 696e 206c 345f 6c69 7374  for i in l4_list
-00000ad0: 5d0d 0a20 2020 206c 345f 6669 6c65 2c20  ]..    l4_file, 
-00000ae0: 6c34 5f73 7465 616d 6964 2c20 6c34 5f68  l4_steamid, l4_h
-00000af0: 6f73 742c 206c 345f 706f 7274 2c20 6c34  ost, l4_port, l4
-00000b00: 5f72 636f 6e2c 206c 345f 6d61 7374 6572  _rcon, l4_master
-00000b10: 3d20 6c34 5f6c 6973 7420 2020 2020 2020  = l4_list       
-00000b20: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00000b30: 0a27 2727 0d0a e59c b0e5 9bbe e8b7 afe5  .'''............
-00000b40: be84 0d0a 2727 270d 0a76 706b 5f70 6174  ....'''..vpk_pat
-00000b50: 6820 3d20 226c 6566 7434 6465 6164 322f  h = "left4dead2/
-00000b60: 6164 646f 6e73 220d 0a23 206d 6170 5f70  addons"..# map_p
-00000b70: 6174 6820 3d20 5061 7468 286c 345f 6669  ath = Path(l4_fi
-00000b80: 6c65 5b43 4845 434b 5f46 494c 455d 2c76  le[CHECK_FILE],v
-00000b90: 706b 5f70 6174 6829 0d0a 2320 6c34 5f66  pk_path)..# l4_f
-00000ba0: 696c 655f 6f6e 6520 3d20 6c34 5f66 696c  ile_one = l4_fil
-00000bb0: 655b 4348 4543 4b5f 4649 4c45 5d0d 0a23  e[CHECK_FILE]..#
-00000bc0: 206c 345f 686f 7374 5f6f 6e65 203d 206c   l4_host_one = l
-00000bd0: 345f 686f 7374 5b43 4845 434b 5f46 494c  4_host[CHECK_FIL
-00000be0: 455d 0d0a 2320 6c34 5f70 6f72 745f 6f6e  E]..# l4_port_on
-00000bf0: 6520 3d20 696e 7428 6c34 5f70 6f72 745b  e = int(l4_port[
-00000c00: 4348 4543 4b5f 4649 4c45 5d29 0d0a 2320  CHECK_FILE])..# 
-00000c10: 6c34 5f72 636f 6e5f 6f6e 6520 3d20 6c34  l4_rcon_one = l4
-00000c20: 5f72 636f 6e5b 4348 4543 4b5f 4649 4c45  _rcon[CHECK_FILE
-00000c30: 5d0d 0a23 2064 6566 206c 6f61 645f 636f  ]..# def load_co
-00000c40: 6e66 6967 2829 3a0d 0a23 2020 2020 2023  nfig():..#     #
-00000c50: 20e6 9687 e4bb b6e8 b7af e5be 840d 0a23   ..............#
-00000c60: 2020 2020 2067 6c6f 6261 6c20 6d61 705f       global map_
-00000c70: 7061 7468 2c6c 345f 6669 6c65 5f6f 6e65  path,l4_file_one
-00000c80: 2c6c 345f 686f 7374 5f6f 6e65 2c6c 345f  ,l4_host_one,l4_
-00000c90: 706f 7274 5f6f 6e65 2c6c 345f 7263 6f6e  port_one,l4_rcon
-00000ca0: 5f6f 6e65 0d0a 2320 2020 2020 6d61 705f  _one..#     map_
-00000cb0: 7061 7468 203d 2050 6174 6828 6c34 5f66  path = Path(l4_f
-00000cc0: 696c 655b 4348 4543 4b5f 4649 4c45 5d2c  ile[CHECK_FILE],
-00000cd0: 7670 6b5f 7061 7468 290d 0a23 2020 2020  vpk_path)..#    
-00000ce0: 206c 345f 6669 6c65 5f6f 6e65 203d 206c   l4_file_one = l
-00000cf0: 345f 6669 6c65 5b43 4845 434b 5f46 494c  4_file[CHECK_FIL
-00000d00: 455d 0d0a 2320 2020 2020 6c34 5f68 6f73  E]..#     l4_hos
-00000d10: 745f 6f6e 6520 3d20 6c34 5f68 6f73 745b  t_one = l4_host[
-00000d20: 4348 4543 4b5f 4649 4c45 5d0d 0a23 2020  CHECK_FILE]..#  
-00000d30: 2020 206c 345f 706f 7274 5f6f 6e65 203d     l4_port_one =
-00000d40: 2069 6e74 286c 345f 706f 7274 5b43 4845   int(l4_port[CHE
-00000d50: 434b 5f46 494c 455d 290d 0a23 2020 2020  CK_FILE])..#    
-00000d60: 206c 345f 7263 6f6e 5f6f 6e65 203d 206c   l4_rcon_one = l
-00000d70: 345f 7263 6f6e 5b43 4845 434b 5f46 494c  4_rcon[CHECK_FIL
-00000d80: 455d 0d0a 0d0a 0d0a 504c 4159 4552 5344  E]......PLAYERSD
-00000d90: 4154 4120 3d20 5061 7468 2829 202f 2022  ATA = Path() / "
-00000da0: 6461 7461 2f4c 3444 322f 696d 6167 652f  data/L4D2/image/
-00000db0: 706c 6179 6572 7322 0d0a 2222 22e7 94a8  players".."""...
-00000dc0: e688 b7e6 95b0 e68d aee8 b7af e5be 8422  ..............."
-00000dd0: 2222 0d0a 5445 5854 5f50 4154 4820 3d20  ""..TEXT_PATH = 
-00000de0: 5061 7468 285f 5f66 696c 655f 5f29 2e70  Path(__file__).p
-00000df0: 6172 656e 7420 2f20 2764 6174 612f 4c34  arent / 'data/L4
-00000e00: 4432 2f69 6d61 6765 270d 0a22 2222 e59b  D2/image'.."""..
-00000e10: bee7 8987 e5ad 98e5 82a8 e8b7 afe5 be84  ................
-00000e20: 2222 220d 0a54 4558 545f 5850 4154 4820  """..TEXT_XPATH 
-00000e30: 3d20 5061 7468 2829 202f 2027 6461 7461  = Path() / 'data
-00000e40: 2f4c 3444 322f 696d 6167 6527 0d0a 2222  /L4D2/image'..""
-00000e50: 22e5 8685 e7bd aee5 9bbe e789 87e8 b7af  "...............
-00000e60: e5be 8422 2222 0d0a 0d0a 0d0a 0d0a 504c  ..."""........PL
-00000e70: 4159 4552 5344 4154 4120 3d20 5061 7468  AYERSDATA = Path
-00000e80: 2829 202f 2022 6461 7461 2f4c 3444 322f  () / "data/L4D2/
-00000e90: 7371 6c22 0d0a 2222 22e6 95b0 e68d aee5  sql"..""".......
-00000ea0: ba93 e8b7 afe5 be84 2222 220d 0a44 4154  ........"""..DAT
-00000eb0: 4153 514c 4954 4520 3d20 5061 7468 2829  ASQLITE = Path()
-00000ec0: 2e70 6172 656e 7420 2f20 2264 6174 612f  .parent / "data/
-00000ed0: 4c34 4432 2f73 716c 2f4c 3444 322e 6462  L4D2/sql/L4D2.db
-00000ee0: 220d 0a22 2222 e695 b0e6 8dae e5ba 93ef  ".."""..........
-00000ef0: bc81 2222 2220 200d 0a0d 0a74 6162 6c65  .."""  ....table
-00000f00: 5f64 6174 6120 3d20 5b22 4c34 6432 5f70  _data = ["L4d2_p
-00000f10: 6c61 7965 7273 222c 224c 3444 325f 7365  layers","L4D2_se
-00000f20: 7276 6572 225d 0d0a 2222 22e6 95b0 e68d  rver"]..""".....
-00000f30: aee5 ba93 e8a1 a822 2222 0d0a 4c34 6432  ......."""..L4d2
-00000f40: 5f70 6c61 7965 7273 5f74 6167 203d 205b  _players_tag = [
-00000f50: 2771 7127 2c20 276e 6963 6b6e 616d 6527  'qq', 'nickname'
-00000f60: 2c20 2773 7465 616d 6964 275d 0d0a 2222  , 'steamid']..""
-00000f70: 22e6 95b0 e68d aee5 ba93 e8a1 a831 2222  "............1""
-00000f80: 220d 0a4c 3464 325f 7365 7276 6572 5f74  "..L4d2_server_t
-00000f90: 6167 203d 205b 2769 6427 2c27 7171 6772  ag = ['id','qqgr
-00000fa0: 6f75 7027 2c20 2768 6f73 7427 2c20 2770  oup', 'host', 'p
-00000fb0: 6f72 7427 2c20 2772 636f 6e27 5d0d 0a22  ort', 'rcon'].."
-00000fc0: 2222 e695 b0e6 8dae e5ba 93e8 a1a8 3222  ""............2"
-00000fd0: 2222 0d0a 4c34 6432 5f49 4e54 4547 4552  ""..L4d2_INTEGER
-00000fe0: 203d 205b 2769 6427 2c27 7171 272c 2771   = ['id','qq','q
-00000ff0: 7167 726f 7570 272c 2770 6f72 7427 5d0d  qgroup','port'].
-00001000: 0a22 2222 494e 4954 4547 4552 e79a 84e8  ."""INITEGER....
-00001010: a1a8 e5a4 b422 2222 0d0a 4c34 6432 5f54  ....."""..L4d2_T
-00001020: 4558 5420 3d20 5b27 6e69 636b 6e61 6d65  EXT = ['nickname
-00001030: 272c 2773 7465 616d 6964 272c 2768 6f73  ','steamid','hos
-00001040: 7427 2c27 7263 6f6e 272c 2770 6174 6827  t','rcon','path'
-00001050: 5d0d 0a22 2222 5445 5854 e79a 84e8 a1a8  ].."""TEXT......
-00001060: e5a4 b422 2222 0d0a 4c34 6432 5f42 4f4f  ..."""..L4d2_BOO
-00001070: 4c45 414e 203d 205b 2775 7365 275d 0d0a  LEAN = ['use']..
-00001080: 2222 2242 4f4f 4c45 414e e79a 84e8 a1a8  """BOOLEAN......
-00001090: e5a4 b422 2222 0d0a 0d0a 7461 626c 6573  ..."""....tables
-000010a0: 5f63 6f6c 756d 6e73 203d 207b 0d0a 2020  _columns = {..  
-000010b0: 2020 7461 626c 655f 6461 7461 5b30 5d3a    table_data[0]:
-000010c0: 4c34 6432 5f70 6c61 7965 7273 5f74 6167  L4d2_players_tag
-000010d0: 2c0d 0a20 2020 2074 6162 6c65 5f64 6174  ,..    table_dat
-000010e0: 615b 315d 3a4c 3464 325f 7365 7276 6572  a[1]:L4d2_server
-000010f0: 5f74 6167 0d0a 7d0d 0a0d 0a23 20e6 b182  _tag..}....# ...
-00001100: e794 9f61 6e6e 65e6 9c8d e58a a1e5 99a8  ...anne.........
-00001110: 0d0a 616e 6e65 5f75 726c 203d 2022 6874  ..anne_url = "ht
-00001120: 7470 733a 2f2f 7365 7276 6572 2e74 7279  tps://server.try
-00001130: 6765 6b2e 636f 6d2f 220d 0a0d 0a67 616d  gek.com/"....gam
-00001140: 656d 6f64 655f 6c69 7374 203d 205b 0d0a  emode_list = [..
-00001150: 2020 2020 27e6 8898 e5bd b927 2c0d 0a20      '......',.. 
-00001160: 2020 2027 e5a4 9ae7 89b9 272c 0d0a 2020     '......',..  
-00001170: 2020 27e5 8699 e4b8 9327 2c0d 0a20 2020    '......',..   
-00001180: 2027 616e 6e65 272c 0d0a 2020 2020 27e8   'anne',..    '.
-00001190: 8daf e68a 9727 2c0d 0a20 2020 2027 e58c  .....',..    '..
-000011a0: 85e6 8a97 272c 0d0a 2020 2020 27e7 bb9d  ....',..    '...
-000011b0: e5a2 8327 2c0d 0a20 2020 2027 e6ad bbe4  ...',..    '....
-000011c0: b893 272c 0d0a 2020 2020 2761 7374 272c  ..',..    'ast',
-000011d0: 0d0a 2020 2020 27e6 b885 e981 93e5 a4ab  ..    '.........
-000011e0: 272c 0d0a 5d0d 0a0d 0a23 20e7 b3bb e7bb  ',..]....# .....
-000011f0: 9f0d 0a69 6620 706c 6174 666f 726d 2e73  ...if platform.s
-00001200: 7973 7465 6d28 2920 3d3d 2027 5769 6e64  ystem() == 'Wind
-00001210: 6f77 7327 3a0d 0a20 2020 2073 7973 7465  ows':..    syste
-00001220: 6d73 3a73 7472 203d 2027 7769 6e27 0d0a  ms:str = 'win'..
-00001230: 656c 6966 2070 6c61 7466 6f72 6d2e 7379  elif platform.sy
-00001240: 7374 656d 2829 203d 3d20 274c 696e 7578  stem() == 'Linux
-00001250: 273a 0d0a 2020 2020 7379 7374 656d 733a  ':..    systems:
-00001260: 7374 7220 3d20 276c 696e 7578 270d 0a65  str = 'linux'..e
-00001270: 6c73 653a 0d0a 2020 2020 7379 7374 656d  lse:..    system
-00001280: 733a 7374 7220 3d20 276f 7468 6572 7327  s:str = 'others'
-00001290: 0d0a 414e 4e45 5f49 5020 3d20 7b7d 0d0a  ..ANNE_IP = {}..
-000012a0: 0d0a 7472 793a 0d0a 2020 2020 6f73 2e72  ..try:..    os.r
-000012b0: 656d 6f76 6528 5061 7468 2829 2e70 6172  emove(Path().par
-000012c0: 656e 742e 6a6f 696e 7061 7468 2827 6461  ent.joinpath('da
-000012d0: 7461 2f4c 3444 322f 6c34 6432 2e79 6d6c  ta/L4D2/l4d2.yml
-000012e0: 2729 290d 0a65 7863 6570 743a 0d0a 2020  '))..except:..  
-000012f0: 2020 7061 7373 0d0a                        pass..
+00000900: 204e 6f6e 650d 0a0d 0a74 7279 3a0d 0a20   None....try:.. 
+00000910: 2020 206c 345f 7765 623a 626f 6f6c 203d     l4_web:bool =
+00000920: 2064 7269 7665 722e 636f 6e66 6967 2e6c   driver.config.l
+00000930: 345f 7765 620d 0a65 7863 6570 743a 0d0a  4_web..except:..
+00000940: 2020 2020 6c34 5f77 6562 3a62 6f6f 6c20      l4_web:bool 
+00000950: 3d20 5472 7565 0d0a 2020 2020 0d0a 2320  = True..    ..# 
+00000960: e5bc bae5 88b6 e8bd ac6c 6973 740d 0a69  .........list..i
+00000970: 6620 7479 7065 286c 345f 7461 6729 203d  f type(l4_tag) =
+00000980: 3d20 7374 7220 6f72 206c 6973 743a 0d0a  = str or list:..
+00000990: 2020 2020 6c34 5f6c 6973 7420 3d20 5b6c      l4_list = [l
+000009a0: 345f 6669 6c65 2c20 6c34 5f73 7465 616d  4_file, l4_steam
+000009b0: 6964 2c20 6c34 5f68 6f73 742c 206c 345f  id, l4_host, l4_
+000009c0: 706f 7274 2c20 6c34 5f72 636f 6e2c 206c  port, l4_rcon, l
+000009d0: 345f 6d61 7374 6572 2c6c 345f 7461 675d  4_master,l4_tag]
+000009e0: 0d0a 2020 2020 6c34 5f6c 6973 7420 3d20  ..    l4_list = 
+000009f0: 5b61 7374 2e6c 6974 6572 616c 5f65 7661  [ast.literal_eva
+00000a00: 6c28 6929 2069 6620 6973 696e 7374 616e  l(i) if isinstan
+00000a10: 6365 2869 2c20 7374 7229 2065 6c73 6520  ce(i, str) else 
+00000a20: 6920 666f 7220 6920 696e 206c 345f 6c69  i for i in l4_li
+00000a30: 7374 5d0d 0a20 2020 206c 345f 6669 6c65  st]..    l4_file
+00000a40: 2c20 6c34 5f73 7465 616d 6964 2c20 6c34  , l4_steamid, l4
+00000a50: 5f68 6f73 742c 206c 345f 706f 7274 2c20  _host, l4_port, 
+00000a60: 6c34 5f72 636f 6e2c 206c 345f 6d61 7374  l4_rcon, l4_mast
+00000a70: 6572 2c20 6c34 5f74 6167 3d20 6c34 5f6c  er, l4_tag= l4_l
+00000a80: 6973 740d 0a65 6c73 653a 0d0a 2020 2020  ist..else:..    
+00000a90: 6c34 5f6c 6973 7420 3d20 5b6c 345f 6669  l4_list = [l4_fi
+00000aa0: 6c65 2c20 6c34 5f73 7465 616d 6964 2c20  le, l4_steamid, 
+00000ab0: 6c34 5f68 6f73 742c 206c 345f 706f 7274  l4_host, l4_port
+00000ac0: 2c20 6c34 5f72 636f 6e2c 206c 345f 6d61  , l4_rcon, l4_ma
+00000ad0: 7374 6572 5d0d 0a20 2020 206c 345f 6c69  ster]..    l4_li
+00000ae0: 7374 203d 205b 6173 742e 6c69 7465 7261  st = [ast.litera
+00000af0: 6c5f 6576 616c 2869 2920 6966 2069 7369  l_eval(i) if isi
+00000b00: 6e73 7461 6e63 6528 692c 2073 7472 2920  nstance(i, str) 
+00000b10: 656c 7365 2069 2066 6f72 2069 2069 6e20  else i for i in 
+00000b20: 6c34 5f6c 6973 745d 0d0a 2020 2020 6c34  l4_list]..    l4
+00000b30: 5f66 696c 652c 206c 345f 7374 6561 6d69  _file, l4_steami
+00000b40: 642c 206c 345f 686f 7374 2c20 6c34 5f70  d, l4_host, l4_p
+00000b50: 6f72 742c 206c 345f 7263 6f6e 2c20 6c34  ort, l4_rcon, l4
+00000b60: 5f6d 6173 7465 723d 206c 345f 6c69 7374  _master= l4_list
+00000b70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00000b80: 2020 2020 2020 0d0a 2727 270d 0ae5 9cb0        ..'''.....
+00000b90: e59b bee8 b7af e5be 840d 0a27 2727 0d0a  ...........'''..
+00000ba0: 7670 6b5f 7061 7468 203d 2022 6c65 6674  vpk_path = "left
+00000bb0: 3464 6561 6432 2f61 6464 6f6e 7322 0d0a  4dead2/addons"..
+00000bc0: 2320 6d61 705f 7061 7468 203d 2050 6174  # map_path = Pat
+00000bd0: 6828 6c34 5f66 696c 655b 4348 4543 4b5f  h(l4_file[CHECK_
+00000be0: 4649 4c45 5d2c 7670 6b5f 7061 7468 290d  FILE],vpk_path).
+00000bf0: 0a23 206c 345f 6669 6c65 5f6f 6e65 203d  .# l4_file_one =
+00000c00: 206c 345f 6669 6c65 5b43 4845 434b 5f46   l4_file[CHECK_F
+00000c10: 494c 455d 0d0a 2320 6c34 5f68 6f73 745f  ILE]..# l4_host_
+00000c20: 6f6e 6520 3d20 6c34 5f68 6f73 745b 4348  one = l4_host[CH
+00000c30: 4543 4b5f 4649 4c45 5d0d 0a23 206c 345f  ECK_FILE]..# l4_
+00000c40: 706f 7274 5f6f 6e65 203d 2069 6e74 286c  port_one = int(l
+00000c50: 345f 706f 7274 5b43 4845 434b 5f46 494c  4_port[CHECK_FIL
+00000c60: 455d 290d 0a23 206c 345f 7263 6f6e 5f6f  E])..# l4_rcon_o
+00000c70: 6e65 203d 206c 345f 7263 6f6e 5b43 4845  ne = l4_rcon[CHE
+00000c80: 434b 5f46 494c 455d 0d0a 2320 6465 6620  CK_FILE]..# def 
+00000c90: 6c6f 6164 5f63 6f6e 6669 6728 293a 0d0a  load_config():..
+00000ca0: 2320 2020 2020 2320 e696 87e4 bbb6 e8b7  #     # ........
+00000cb0: afe5 be84 0d0a 2320 2020 2020 676c 6f62  ......#     glob
+00000cc0: 616c 206d 6170 5f70 6174 682c 6c34 5f66  al map_path,l4_f
+00000cd0: 696c 655f 6f6e 652c 6c34 5f68 6f73 745f  ile_one,l4_host_
+00000ce0: 6f6e 652c 6c34 5f70 6f72 745f 6f6e 652c  one,l4_port_one,
+00000cf0: 6c34 5f72 636f 6e5f 6f6e 650d 0a23 2020  l4_rcon_one..#  
+00000d00: 2020 206d 6170 5f70 6174 6820 3d20 5061     map_path = Pa
+00000d10: 7468 286c 345f 6669 6c65 5b43 4845 434b  th(l4_file[CHECK
+00000d20: 5f46 494c 455d 2c76 706b 5f70 6174 6829  _FILE],vpk_path)
+00000d30: 0d0a 2320 2020 2020 6c34 5f66 696c 655f  ..#     l4_file_
+00000d40: 6f6e 6520 3d20 6c34 5f66 696c 655b 4348  one = l4_file[CH
+00000d50: 4543 4b5f 4649 4c45 5d0d 0a23 2020 2020  ECK_FILE]..#    
+00000d60: 206c 345f 686f 7374 5f6f 6e65 203d 206c   l4_host_one = l
+00000d70: 345f 686f 7374 5b43 4845 434b 5f46 494c  4_host[CHECK_FIL
+00000d80: 455d 0d0a 2320 2020 2020 6c34 5f70 6f72  E]..#     l4_por
+00000d90: 745f 6f6e 6520 3d20 696e 7428 6c34 5f70  t_one = int(l4_p
+00000da0: 6f72 745b 4348 4543 4b5f 4649 4c45 5d29  ort[CHECK_FILE])
+00000db0: 0d0a 2320 2020 2020 6c34 5f72 636f 6e5f  ..#     l4_rcon_
+00000dc0: 6f6e 6520 3d20 6c34 5f72 636f 6e5b 4348  one = l4_rcon[CH
+00000dd0: 4543 4b5f 4649 4c45 5d0d 0a0d 0a0d 0a50  ECK_FILE]......P
+00000de0: 4c41 5945 5253 4441 5441 203d 2050 6174  LAYERSDATA = Pat
+00000df0: 6828 2920 2f20 2264 6174 612f 4c34 4432  h() / "data/L4D2
+00000e00: 2f69 6d61 6765 2f70 6c61 7965 7273 220d  /image/players".
+00000e10: 0a22 2222 e794 a8e6 88b7 e695 b0e6 8dae  ."""............
+00000e20: e8b7 afe5 be84 2222 220d 0a54 4558 545f  ......"""..TEXT_
+00000e30: 5041 5448 203d 2050 6174 6828 5f5f 6669  PATH = Path(__fi
+00000e40: 6c65 5f5f 292e 7061 7265 6e74 202f 2027  le__).parent / '
+00000e50: 6461 7461 2f4c 3444 322f 696d 6167 6527  data/L4D2/image'
+00000e60: 0d0a 2222 22e5 9bbe e789 87e5 ad98 e582  .."""...........
+00000e70: a8e8 b7af e5be 8422 2222 0d0a 5445 5854  ......."""..TEXT
+00000e80: 5f58 5041 5448 203d 2050 6174 6828 2920  _XPATH = Path() 
+00000e90: 2f20 2764 6174 612f 4c34 4432 2f69 6d61  / 'data/L4D2/ima
+00000ea0: 6765 270d 0a22 2222 e586 85e7 bdae e59b  ge'.."""........
+00000eb0: bee7 8987 e8b7 afe5 be84 2222 220d 0a0d  .........."""...
+00000ec0: 0a0d 0a0d 0a50 4c41 5945 5253 4441 5441  .....PLAYERSDATA
+00000ed0: 203d 2050 6174 6828 2920 2f20 2264 6174   = Path() / "dat
+00000ee0: 612f 4c34 4432 2f73 716c 220d 0a22 2222  a/L4D2/sql".."""
+00000ef0: e695 b0e6 8dae e5ba 93e8 b7af e5be 8422  ..............."
+00000f00: 2222 0d0a 4441 5441 5351 4c49 5445 203d  ""..DATASQLITE =
+00000f10: 2050 6174 6828 292e 7061 7265 6e74 202f   Path().parent /
+00000f20: 2022 6461 7461 2f4c 3444 322f 7371 6c2f   "data/L4D2/sql/
+00000f30: 4c34 4432 2e64 6222 0d0a 2222 22e6 95b0  L4D2.db".."""...
+00000f40: e68d aee5 ba93 efbc 8122 2222 2020 0d0a  ........."""  ..
+00000f50: 0d0a 7461 626c 655f 6461 7461 203d 205b  ..table_data = [
+00000f60: 224c 3464 325f 706c 6179 6572 7322 2c22  "L4d2_players","
+00000f70: 4c34 4432 5f73 6572 7665 7222 5d0d 0a22  L4D2_server"].."
+00000f80: 2222 e695 b0e6 8dae e5ba 93e8 a1a8 2222  ""............""
+00000f90: 220d 0a4c 3464 325f 706c 6179 6572 735f  "..L4d2_players_
+00000fa0: 7461 6720 3d20 5b27 7171 272c 2027 6e69  tag = ['qq', 'ni
+00000fb0: 636b 6e61 6d65 272c 2027 7374 6561 6d69  ckname', 'steami
+00000fc0: 6427 5d0d 0a22 2222 e695 b0e6 8dae e5ba  d'].."""........
+00000fd0: 93e8 a1a8 3122 2222 0d0a 4c34 6432 5f73  ....1"""..L4d2_s
+00000fe0: 6572 7665 725f 7461 6720 3d20 5b27 6964  erver_tag = ['id
+00000ff0: 272c 2771 7167 726f 7570 272c 2027 686f  ','qqgroup', 'ho
+00001000: 7374 272c 2027 706f 7274 272c 2027 7263  st', 'port', 'rc
+00001010: 6f6e 275d 0d0a 2222 22e6 95b0 e68d aee5  on']..""".......
+00001020: ba93 e8a1 a832 2222 220d 0a4c 3464 325f  .....2"""..L4d2_
+00001030: 494e 5445 4745 5220 3d20 5b27 6964 272c  INTEGER = ['id',
+00001040: 2771 7127 2c27 7171 6772 6f75 7027 2c27  'qq','qqgroup','
+00001050: 706f 7274 275d 0d0a 2222 2249 4e49 5445  port'].."""INITE
+00001060: 4745 52e7 9a84 e8a1 a8e5 a4b4 2222 220d  GER.........""".
+00001070: 0a4c 3464 325f 5445 5854 203d 205b 276e  .L4d2_TEXT = ['n
+00001080: 6963 6b6e 616d 6527 2c27 7374 6561 6d69  ickname','steami
+00001090: 6427 2c27 686f 7374 272c 2772 636f 6e27  d','host','rcon'
+000010a0: 2c27 7061 7468 275d 0d0a 2222 2254 4558  ,'path'].."""TEX
+000010b0: 54e7 9a84 e8a1 a8e5 a4b4 2222 220d 0a4c  T........."""..L
+000010c0: 3464 325f 424f 4f4c 4541 4e20 3d20 5b27  4d2_BOOLEAN = ['
+000010d0: 7573 6527 5d0d 0a22 2222 424f 4f4c 4541  use'].."""BOOLEA
+000010e0: 4ee7 9a84 e8a1 a8e5 a4b4 2222 220d 0a0d  N........."""...
+000010f0: 0a74 6162 6c65 735f 636f 6c75 6d6e 7320  .tables_columns 
+00001100: 3d20 7b0d 0a20 2020 2074 6162 6c65 5f64  = {..    table_d
+00001110: 6174 615b 305d 3a4c 3464 325f 706c 6179  ata[0]:L4d2_play
+00001120: 6572 735f 7461 672c 0d0a 2020 2020 7461  ers_tag,..    ta
+00001130: 626c 655f 6461 7461 5b31 5d3a 4c34 6432  ble_data[1]:L4d2
+00001140: 5f73 6572 7665 725f 7461 670d 0a7d 0d0a  _server_tag..}..
+00001150: 0d0a 2320 e6b1 82e7 949f 616e 6e65 e69c  ..# ......anne..
+00001160: 8de5 8aa1 e599 a80d 0a61 6e6e 655f 7572  .........anne_ur
+00001170: 6c20 3d20 2268 7474 7073 3a2f 2f73 6572  l = "https://ser
+00001180: 7665 722e 7472 7967 656b 2e63 6f6d 2f22  ver.trygek.com/"
+00001190: 0d0a 0d0a 6761 6d65 6d6f 6465 5f6c 6973  ....gamemode_lis
+000011a0: 7420 3d20 5b0d 0a20 2020 2027 e688 98e5  t = [..    '....
+000011b0: bdb9 272c 0d0a 2020 2020 27e5 a49a e789  ..',..    '.....
+000011c0: b927 2c0d 0a20 2020 2027 e586 99e4 b893  .',..    '......
+000011d0: 272c 0d0a 2020 2020 2761 6e6e 6527 2c0d  ',..    'anne',.
+000011e0: 0a20 2020 2027 e88d afe6 8a97 272c 0d0a  .    '......',..
+000011f0: 2020 2020 27e5 8c85 e68a 9727 2c0d 0a20      '......',.. 
+00001200: 2020 2027 e7bb 9de5 a283 272c 0d0a 2020     '......',..  
+00001210: 2020 27e6 adbb e4b8 9327 2c0d 0a20 2020    '......',..   
+00001220: 2027 6173 7427 2c0d 0a20 2020 2027 e6b8   'ast',..    '..
+00001230: 85e9 8193 e5a4 ab27 2c0d 0a5d 0d0a 0d0a  .......',..]....
+00001240: 2320 e7b3 bbe7 bb9f 0d0a 6966 2070 6c61  # ........if pla
+00001250: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
+00001260: 3d20 2757 696e 646f 7773 273a 0d0a 2020  = 'Windows':..  
+00001270: 2020 7379 7374 656d 733a 7374 7220 3d20    systems:str = 
+00001280: 2777 696e 270d 0a65 6c69 6620 706c 6174  'win'..elif plat
+00001290: 666f 726d 2e73 7973 7465 6d28 2920 3d3d  form.system() ==
+000012a0: 2027 4c69 6e75 7827 3a0d 0a20 2020 2073   'Linux':..    s
+000012b0: 7973 7465 6d73 3a73 7472 203d 2027 6c69  ystems:str = 'li
+000012c0: 6e75 7827 0d0a 656c 7365 3a0d 0a20 2020  nux'..else:..   
+000012d0: 2073 7973 7465 6d73 3a73 7472 203d 2027   systems:str = '
+000012e0: 6f74 6865 7273 270d 0a41 4e4e 455f 4950  others'..ANNE_IP
+000012f0: 203d 207b 7d0d 0a0d 0a74 7279 3a0d 0a20   = {}....try:.. 
+00001300: 2020 206f 732e 7265 6d6f 7665 2850 6174     os.remove(Pat
+00001310: 6828 292e 7061 7265 6e74 2e6a 6f69 6e70  h().parent.joinp
+00001320: 6174 6828 2764 6174 612f 4c34 4432 2f6c  ath('data/L4D2/l
+00001330: 3464 322e 796d 6c27 2929 0d0a 6578 6365  4d2.yml'))..exce
+00001340: 7074 3a0d 0a20 2020 2070 6173 730d 0a20  pt:..    pass.. 
+00001350: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001360: 2020 2020 20
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     msg:a2s.SourceInfo = await a2s.ainfo((ip,port))
     # message_dict = await l4d2.server(ip,port,times=5)
     msg_dict['folder'] =  msg.folder
     msg_dict['name'] =  msg.server_name
     msg_dict['map_'] =  msg.map_name
     msg_dict['players'] =  msg.player_count
     msg_dict['max_players'] =  msg.max_players
+    msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
     msg_dict['ip'] = str(ip) + ':' +str(port)
     msg_dict['ping'] = f"{msg.ping*1000:.0f}ms"
     if msg_dict['players'] < msg_dict['max_players']:
         msg_dict['enabled'] = True
     else:
         msg_dict['enabled'] = False
     return msg_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,44 +47,56 @@
     for i in msg:
         number,qqgroup,host,port = i
         msg2 = await player_queries(host,port)
         msg1 = await queries(host,port)
         messsage += '序号、'+ str(number) + '\n' + msg1 + msg2 + '--------------------\n'
     return messsage
             
-async def qq_ip_queries_pic(msg: list):
+            
+async def qq_ip_querie(msg: list):
     msg_list = []
-    pic = None
     tasks = []  # 用来保存异步任务
     if msg != []:
         for i in msg:
             try:
                 number, host, port = i
+                qqgroup = ''
             except ValueError:
                 number, qqgroup, host, port = i
             finally:
                 # 将异步任务添加到任务列表中
-                tasks.append(asyncio.create_task(process_message(number, host, port, msg_list)))
+                tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup)))
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
         msg_list = sorted(msg_list, key=lambda x: x['number'])
-        pic = await server_ip_pic(msg_list)
-    if pic is None:
-        return None
+        result = {'msg_list': msg_list}
+    else:
+        result = {}
+    return result
+
+
+async def qq_ip_queries_pic(msg: list):
+    result = await qq_ip_querie(msg)
+    if 'msg_list' in result:
+        pic = await server_ip_pic(result['msg_list'])
+    else:
+        pic = None
     return pic
+            
 
 
 
-async def process_message(number, host, port, msg_list):
+async def process_message(number, host, port, msg_list:list,qqgroup = ''):
     try:
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
-        msg1.update({'Players':msg2})
-        msg1.update({'number':number})
+        msg1.update({'Players':msg2,'number':number,})
+        if qqgroup:
+            msg1.update({'tag':qqgroup})
         msg_list.append(msg1)
     except errors:
         pass  # 忽略异常，继续下一次循环
 
 
     
 async def get_tan_jian(msg:List[tuple],mode:int):
@@ -196,73 +208,69 @@
 
 def split_maohao(msg:str) -> list:
     """分割大小写冒号"""
     msg:list = re.split(":|：",msg.strip())
     mse = [msg[0],msg[-1]] if msg[0] != msg[-1] else [msg[0],20715]
     return mse
 
-async def write_json(data_str:str):
-    """添加数据或者删除数据
+async def write_json(data_str: str):
+    """
+    添加数据或者删除数据
      - 【求生更新 添加 腐竹 ip 模式 序号】
      - 【求生更新 添加 腐竹 ip 模式】
      - 【求生更新 删除 腐竹 序号】
     """
-    data_list = data_str.split(' ')
+    data_list = data_str.split()
     logger.info(data_list)
-    if data_list[0]=="添加":
+    if data_list[0] == "添加":
         add_server = {}
         server_dict = ALL_HOST.get(data_list[1], {})
         if not server_dict:
             logger.info('新建分支')
             ALL_HOST[data_list[1]] = []
-        for key,value in ALL_HOST.items():
+        for key, value in ALL_HOST.items():
             if data_list[1] == key:
-                ids = []
+                ids = [server['id'] for server in value]
                 # 序号
                 if len(data_list) == 4:
-                    data_num:int = 1
-                    for server in value:
-                        ids.append(str(server['id']))
-                    while data_num in ids:
-                        data_num += 1
-                    data_id = str(data_num)
-                    add_server.update({'id':data_num})
-                if len(data_list) == 5:
-                    for server in value:
-                        ids.append(str(server['id']))
-                    if data_list[4].isdigit():
-                        if data_list[4] not in ids:
-                            data_id = data_list[4]
-                            add_server.update({'id':int(data_id)})
-                        else:
-                            return '该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】'
-                    else:
+                    data_num = max(ids, default=0) + 1
+                    add_server.update({'id': data_num})
+                elif len(data_list) == 5:
+                    if not data_list[4].isdigit():
                         return '序号应该为大于0的正整数，请输入【求生更新 添加 腐竹 ip 模式 序号】'
+                    data_num = int(data_list[4])
+                    if data_num in ids:
+                        return '该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】'
+                    add_server.update({'id': data_num})
+                else:
+                    return '输入参数错误，请输入【求生更新 添加 腐竹 ip 模式 序号】或【求生更新 添加 腐竹 ip 模式】'
                 # 模式，ip
-                add_server.update({'version':data_list[3]})
                 try:
-                    host,port = split_maohao(data_list[2])
-                    add_server.update({'host':host,'port':port})
+                    host, port = split_maohao(data_list[2])
+                    add_server.update({'host': host, 'port': port})
                 except KeyError:
                     return 'ip格式不正确【114.11.4.514:9191】'
+                add_server.update({'version': data_list[3]})
                 value.append(add_server)
-                ALL_HOST.update({key:value})
-                with open('data/L4D2/l4d2.json', "r", encoding="utf8") as f_new:
+                ALL_HOST[key] = value
+                with open('data/L4D2/l4d2.json', 'w', encoding='utf8') as f_new:
                     json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
-                return f'添加成功，指令为{key}{data_id}'
+                return f'添加成功，指令为{key}{data_num}'
             
-    elif data_list[0]=="删除":
-        for key,value in ALL_HOST.items():
-            value:List[dict]
+    elif data_list[0] == "删除":
+        for key, value in ALL_HOST.items():
             if data_list[1] == key:
-                for server in value:
-                    if int(data_list[2]) == server['id']:
-                        value.remove(server)
+                try:
+                    data_num = int(data_list[2])
+                except ValueError:
+                    return '序号应该为大于0的正整数，请输入【求生更新 删除 腐竹 序号】'
+                for i, server in enumerate(value):
+                    if data_num == server['id']:
+                        value.pop(i)
                         if not value:
                             ALL_HOST.pop(key)
-                        else:
-                            ALL_HOST[key] = value
-                        with open('data/L4D2/l4d2.json', "r", encoding="utf8") as f_new:
+                        with open('data/L4D2/l4d2.json', 'w', encoding='utf8') as f_new:
                             json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
                         return '删除成功喵'
                 return '序号不正确，请输入【求生更新 删除 腐竹 序号】'
-        return '腐竹名不存在，请输入【求生更新 删除 腐竹 序号】'    
+        return '腐竹名不存在，请输入【求生更新 删除 腐竹 序号】'   
+
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/config.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pydantic import BaseModel
 from typing import List, Dict
 from pathlib import Path
 
 from pydantic import BaseModel, Field
-
-from nonebot import get_driver, logger
+from nonebot import logger
 from ruamel import yaml
 
 
 CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 class L4d2GroupConfig(BaseModel):
@@ -77,8 +76,9 @@
                 Dumper=yaml.RoundTripDumper,
                 allow_unicode=True)
             
 config_manager = L4d2ConfigManager()
 
 class UserModel(BaseModel):
     username: str
-    password: str
+    password: str
+
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 from jose import jwt
 from nonebot import get_bot, get_app
 
 from pathlib import Path
 
 
 from nonebot import get_driver, logger
-from ruamel import yaml
 from .config import *
+from ..config import *
+from ..utils import split_maohao
+from ..l4d2_queries.qqgroup import qq_ip_querie
 CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
+
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 
 from .webUI import login_page, admin_app
 
 requestAdaptor = '''
@@ -60,15 +63,15 @@
 
 
 @driver.on_startup
 async def init_web():
     if not config_manager.config.total_enable:
         return
     app: FastAPI = get_app()
-
+    logger.success('成功加载网页控制台')
     @app.post('/l4d2/api/login', response_class=JSONResponse)
     async def login(user: UserModel):
         if user.username != config_manager.config.web_username or user.password != config_manager.config.web_password:
             return {
                 'status': -100,
                 'msg':    '登录失败，请确认用户ID和密码无误'
             }
@@ -119,15 +122,42 @@
             config['member_list'] = member_list
             return config
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
             }
-
+            
+    @app.get('/l4d2/api/get_chat_contexts', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_chat_context():
+        try:
+            from ..command import ALL_HOST
+            this_ips = ALL_HOST
+            print(ALL_HOST)
+            ip_lists = []
+            for ip_list, v in this_ips.items():
+                for d in v:
+                    host, port = split_maohao(d['ip'])
+                    ip_lists.append((d['id'], ip_list, host, port))
+            data_dict = await qq_ip_querie(ip_lists)
+            data_list = data_dict['msg_list']
+            print(data_list)
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': {
+                    'items': data_list,
+                    'total': len(data_list),
+                }
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
 
 
     @app.get('/l4d2', response_class=RedirectResponse)
     async def redirect_page():
         return RedirectResponse('/l4d2/login')
 
     @app.get('/l4d2/login', response_class=HTMLResponse)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from amis import ColumnList, AmisList, ActionType, TableCRUD, TableColumn
-from amis import Dialog, PageSchema, Switch, InputNumber, InputTag, Action, App
-from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper,Combo,CRUD
-from amis import LevelEnum, Select, InputArray, Alert, Tpl, Flex
+from amis import  ActionType, TableCRUD, TableColumn
+from amis import  PageSchema, Switch, InputNumber, InputTag, Action, App
+from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
+from amis import LevelEnum, Select,  Alert, Tpl, Flex
 
 
 from ..config import NICKNAME
 
 logo = Html(html='''
 <p align="center">
     <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server">
@@ -101,149 +101,68 @@
 
 message_table = TableCRUD(
     mode='table',
     title='',
     syncLocation=False,
     api='/l4d2/api/get_chat_messages',
     interval=12000,
-    headerToolbar=[ActionType.Ajax(label='删除所有聊天记录',
-                                    level=LevelEnum.warning,
-                                    confirmText='确定要删除所有聊天记录吗？',
-                                    api='put:/l4d2/api/delete_all?type=message')],
-    itemActions=[ActionType.Ajax(tooltip='禁用',
-                                icon='fa fa-ban text-danger',
-                                confirmText='禁用该聊天记录相关的学习内容和回复',
-                                api='put:/l4d2/api/ban_chat?type=message&id=${id}'),
-                ActionType.Ajax(tooltip='删除',
-                                icon='fa fa-times text-danger',
-                                confirmText='删除该条聊天记录',
-                                api='delete:/l4d2/api/delete_chat?type=message&id=${id}')
-                ],
     footable=True,
     columns=[TableColumn(label='序号', name='message_id'),
             TableColumn(label='服务器ip', name='group_id', searchable=True),
             TableColumn(label='服务器端口', name='user_id', searchable=True),
             TableColumn(type='tpl', tpl='${raw_message|truncate:20}', label='rcon密码',
                         name='message',
                         searchable=True, popOver={'mode':      'dialog', 'title': '消息全文',
                                                     'className': 'break-all',
                                                     'body':      {'type': 'tpl',
                                                                 'tpl':  '${raw_message}'}}),
             TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='时间',
                         name='time', sortable=True)
             ])
-answer_table = TableCRUD(
-    mode='table',
-    syncLocation=False,
-    footable=True,
-    api='/l4d2/api/get_chat_answers',
-    interval=12000,
-    headerToolbar=[ActionType.Ajax(label='删除所有已学习的回复',
-                                   level=LevelEnum.warning,
-                                   confirmText='确定要删除所有已学习的回复吗？',
-                                   api='put:/l4d2/api/delete_all?type=answer')],
-    itemActions=[ActionType.Ajax(tooltip='禁用',
-                                 icon='fa fa-ban text-danger',
-                                 confirmText='禁用并删除该已学回复',
-                                 api='put:/l4d2/api/ban_chat?type=answer&id=${id}'),
-                 ActionType.Ajax(tooltip='删除',
-                                 icon='fa fa-times text-danger',
-                                 confirmText='仅删除该已学回复，不会禁用，所以依然能继续学',
-                                 api='delete:/l4d2/api/delete_chat?type=answer&id=${id}')],
-    columns=[TableColumn(label='ID', name='id', visible=False),
-             TableColumn(label='群ID', name='group_id', searchable=True),
-             TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词', name='keywords',
-                         searchable=True, popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                   'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-             TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='最后学习时间', name='time',
-                         sortable=True),
-             TableColumn(label='次数', name='count', sortable=True),
-             ColumnList(label='完整消息', name='messages', breakpoint='*', source='${messages}',
-                        listItem=AmisList.Item(body={'name': 'msg'}))
-             ])
-answer_table_on_context = TableCRUD(
-    mode='table',
-    syncLocation=False,
-    footable=True,
-    api='/l4d2/api/get_chat_answers?context_id=${id}&page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}',
-    interval=12000,
-    headerToolbar=[ActionType.Ajax(label='删除该内容所有回复',
-                                   level=LevelEnum.warning,
-                                   confirmText='确定要删除该条内容已学习的回复吗？',
-                                   api='put:/l4d2/api/delete_all?type=answer&id=${id}')],
-    itemActions=[ActionType.Ajax(tooltip='禁用',
-                                 icon='fa fa-ban text-danger',
-                                 confirmText='禁用并删除该已学回复',
-                                 api='put:/l4d2/api/ban_chat?type=answer&id=${id}'),
-                 ActionType.Ajax(tooltip='删除',
-                                 icon='fa fa-times text-danger',
-                                 confirmText='仅删除该已学回复，但不禁用，依然能继续学',
-                                 api='delete:/l4d2/api/delete_chat?type=answer&id=${id}')],
-    columns=[TableColumn(label='ID', name='id', visible=False),
-             TableColumn(label='群ID', name='group_id'),
-             TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词', name='keywords',
-                         searchable=True, popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                   'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-             TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='最后学习时间', name='time',
-                         sortable=True),
-             TableColumn(label='次数', name='count', sortable=True),
-             ColumnList(label='完整消息', name='messages', breakpoint='*', source='${messages}',
-                        listItem=AmisList.Item(body={'name': 'msg'}))
-             ])
+
 context_table = TableCRUD(mode='table',
                           title='',
                           syncLocation=False,
                           api='/l4d2/api/get_chat_contexts',
-                          interval=12000,
-                          headerToolbar=[ActionType.Ajax(label='删除所有学习内容',
-                                                         level=LevelEnum.warning,
-                                                         confirmText='确定要删除所有已学习的内容吗？',
-                                                         api='put:/l4d2/api/delete_all?type=context')],
-                          itemActions=[ActionType.Dialog(tooltip='回复列表',
-                                                         icon='fa fa-book text-info',
-                                                         dialog=Dialog(title='回复列表',
-                                                                       size='lg',
-                                                                       body=answer_table_on_context)),
-                                       ActionType.Ajax(tooltip='禁用',
-                                                       icon='fa fa-ban text-danger',
-                                                       confirmText='禁用并删除该学习的内容及其所有回复',
-                                                       api='put:/l4d2/api/ban_chat?type=context&id=${id}'),
-                                       ActionType.Ajax(tooltip='删除',
-                                                       icon='fa fa-times text-danger',
-                                                       confirmText='仅删除该学习的内容及其所有回复，但不禁用，依然能继续学',
-                                                       api='delete:/l4d2/api/delete_chat?type=context&id=${id}')
-                                       ],
+                          interval=60000,
                           footable=True,
-                          columns=[TableColumn(label='ID', name='id', visible=False),
-                                   TableColumn(type='tpl', tpl='${keywords|truncate:20}', label='内容/关键词',
-                                               name='keywords', searchable=True,
-                                               popOver={'mode': 'dialog', 'title': '内容全文', 'className': 'break-all',
-                                                        'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
-                                   TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-                                               label='最后学习时间', name='time', sortable=True),
-                                   TableColumn(label='已学次数', name='count', sortable=True),
-                                   ])
+                          itemActions=[ActionType.Url(
+                                tooltip='加入游戏',
+                                icon='fa fa-gamepad',
+                                confirmText = "加入steam://connect/"+'${ip}',
+                                url= "steam://connect/"+'${ip}',
+                                # url= "http://"+'${ip}',
+                                blank= True
+                                 ),
+                            ],
+                          columns = [
+                                    TableColumn(label='服主', name='tag', searchable=True),
+                                    TableColumn(label='名称', name='name', searchable=True),
+                                    TableColumn(label='地图', name='map_', searchable=True),
+                                    TableColumn(label='玩家', name='rank_players', searchable=True),
+                                    TableColumn(label='延迟', name='ping', searchable=True),
+                                    TableColumn(label='IP 地址', name='ip', searchable=True),
+                                    ])
 
 message_page = PageSchema(url='/messages', icon='fa fa-comments', label='本地服务器管理',
                           schema=Page(title='本地服务器管理', body=[
                               Alert(level=LevelEnum.info,
                                     className='white-space-pre-wrap',
                                     body=(f'此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n'
-                                        #   '· 点击"禁用"可以将某条聊天记录进行禁用，这样其相关的学习就会列入禁用列表。\n'
-                                        #   '· 点击"删除"可以删除某条记录，但不会影响它的学习。\n'
+
                                           f'· 功能暂未完善')),
                               message_table]))
 context_page = PageSchema(url='/contexts', icon='fa fa-comment', label='远程服务器查询',
                           schema=Page(title='远程服务器查询',
                                       body=[Alert(level=LevelEnum.info,
                                                   className='white-space-pre-wrap',
                                                   body=(f'此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n'
                                                         # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
                                                         # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
-                                                        '· 点击"删除"可以删除该学习，让它重新开始学习这句话。')),
+                                                        f'· 功能暂未完善')),
                                             context_table]))
 
 database_page = PageSchema(label='数据库', icon='fa fa-database',
                            children=[message_page, context_page])
 config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
                          schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
                                      body=[global_config_form, group_select, group_config_form]))
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-from amis import ColumnList, AmisList, ActionType, TableCRUD, TableColumn from
-amis import Dialog, PageSchema, Switch, InputNumber, InputTag, Action, App from
-amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal,
-Remark, Html, Page, AmisAPI, Wrapper,Combo,CRUD from amis import LevelEnum,
-Select, InputArray, Alert, Tpl, Flex from ..config import NICKNAME logo = Html
-(html='''
+from amis import ActionType, TableCRUD, TableColumn from amis import
+PageSchema, Switch, InputNumber, InputTag, Action, App from amis import Form,
+InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page,
+AmisAPI, Wrapper from amis import LevelEnum, Select, Alert, Tpl, Flex from
+..config import NICKNAME logo = Html(html='''
                                 [Learning-Chat]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
 ''') login_api = AmisAPI( url='/l4d2/api/login', method='post', adaptor=''' if
 (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
@@ -59,116 +58,52 @@
 content='å ä½ç¬¦è¯æ¡')), ], actions=[Action(label='ä¿å­',
 level=LevelEnum.success, type='submit'), ActionType.Ajax
 ( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
 confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/l4d2/api/
 chat_group_config?group_id=all' ), Action(label='éç½®',
 level=LevelEnum.warning, type='reset')] ) message_table = TableCRUD
 ( mode='table', title='', syncLocation=False, api='/l4d2/api/
-get_chat_messages', interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤ææèå¤©è®°å½', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤ææèå¤©è®°å½åï¼', api='put:/l4d2/api/
-delete_all?type=message')], itemActions=[ActionType.Ajax(tooltip='ç¦ç¨',
-icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨è¯¥èå¤©è®°å½ç¸å³çå­¦ä¹ åå®¹ååå¤', api='put:/
-l4d2/api/ban_chat?type=message&id=${id}'), ActionType.Ajax(tooltip='å é¤',
-icon='fa fa-times text-danger', confirmText='å é¤è¯¥æ¡èå¤©è®°å½',
-api='delete:/l4d2/api/delete_chat?type=message&id=${id}') ], footable=True,
-columns=[TableColumn(label='åºå·', name='message_id'), TableColumn
-(label='æå¡å¨ip', name='group_id', searchable=True), TableColumn
-(label='æå¡å¨ç«¯å£', name='user_id', searchable=True), TableColumn
-(type='tpl', tpl='${raw_message|truncate:20}', label='rconå¯ç ',
-name='message', searchable=True, popOver={'mode': 'dialog', 'title':
-'æ¶æ¯å¨æ', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
-{raw_message}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:
-mm\\:ss}', label='æ¶é´', name='time', sortable=True) ]) answer_table =
-TableCRUD( mode='table', syncLocation=False, footable=True, api='/l4d2/api/
-get_chat_answers', interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤ææå·²å­¦ä¹ çåå¤', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå¤åï¼', api='put:/l4d2/
-api/delete_all?type=answer')], itemActions=[ActionType.Ajax(tooltip='ç¦ç¨',
-icon='fa fa-ban text-danger', confirmText='ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤',
-api='put:/l4d2/api/ban_chat?type=answer&id=${id}'), ActionType.Ajax
-(tooltip='å é¤', icon='fa fa-times text-danger',
-confirmText='ä»å é¤è¯¥å·²å­¦åå¤ï¼ä¸ä¼ç¦ç¨ï¼æä»¥ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/l4d2/api/delete_chat?type=answer&id=${id}')], columns=[TableColumn
-(label='ID', name='id', visible=False), TableColumn(label='ç¾¤ID',
-name='group_id', searchable=True), TableColumn(type='tpl', tpl='$
-{keywords|truncate:20}', label='åå®¹/å³é®è¯', name='keywords',
-searchable=True, popOver={'mode': 'dialog', 'title': 'åå®¹å¨æ',
-'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '${keywords}'}}),
+get_chat_messages', interval=12000, footable=True, columns=[TableColumn
+(label='åºå·', name='message_id'), TableColumn(label='æå¡å¨ip',
+name='group_id', searchable=True), TableColumn(label='æå¡å¨ç«¯å£',
+name='user_id', searchable=True), TableColumn(type='tpl', tpl='$
+{raw_message|truncate:20}', label='rconå¯ç ', name='message',
+searchable=True, popOver={'mode': 'dialog', 'title': 'æ¶æ¯å¨æ',
+'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '${raw_message}'}}),
 TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-label='æåå­¦ä¹ æ¶é´', name='time', sortable=True), TableColumn
-(label='æ¬¡æ°', name='count', sortable=True), ColumnList(label='å®æ´æ¶æ¯',
-name='messages', breakpoint='*', source='${messages}', listItem=AmisList.Item
-(body={'name': 'msg'})) ]) answer_table_on_context = TableCRUD( mode='table',
-syncLocation=False, footable=True, api='/l4d2/api/get_chat_answers?context_id=$
-{id}&page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}',
-interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤è¯¥åå®¹ææåå¤', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤è¯¥æ¡åå®¹å·²å­¦ä¹ çåå¤åï¼', api='put:/
-l4d2/api/delete_all?type=answer&id=${id}')], itemActions=[ActionType.Ajax
-(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨å¹¶å é¤è¯¥å·²å­¦åå¤', api='put:/l4d2/api/
-ban_chat?type=answer&id=${id}'), ActionType.Ajax(tooltip='å é¤', icon='fa fa-
-times text-danger',
-confirmText='ä»å é¤è¯¥å·²å­¦åå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/l4d2/api/delete_chat?type=answer&id=${id}')], columns=[TableColumn
-(label='ID', name='id', visible=False), TableColumn(label='ç¾¤ID',
-name='group_id'), TableColumn(type='tpl', tpl='${keywords|truncate:20}',
-label='åå®¹/å³é®è¯', name='keywords', searchable=True, popOver={'mode':
-'dialog', 'title': 'åå®¹å¨æ', 'className': 'break-all', 'body': {'type':
-'tpl', 'tpl': '${keywords}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-
-MM-DD HH\\:mm\\:ss}', label='æåå­¦ä¹ æ¶é´', name='time', sortable=True),
-TableColumn(label='æ¬¡æ°', name='count', sortable=True), ColumnList
-(label='å®æ´æ¶æ¯', name='messages', breakpoint='*', source='${messages}',
-listItem=AmisList.Item(body={'name': 'msg'})) ]) context_table = TableCRUD
+label='æ¶é´', name='time', sortable=True) ]) context_table = TableCRUD
 (mode='table', title='', syncLocation=False, api='/l4d2/api/get_chat_contexts',
-interval=12000, headerToolbar=[ActionType.Ajax
-(label='å é¤ææå­¦ä¹ åå®¹', level=LevelEnum.warning,
-confirmText='ç¡®å®è¦å é¤ææå·²å­¦ä¹ çåå®¹åï¼', api='put:/l4d2/
-api/delete_all?type=context')], itemActions=[ActionType.Dialog
-(tooltip='åå¤åè¡¨', icon='fa fa-book text-info', dialog=Dialog
-(title='åå¤åè¡¨', size='lg', body=answer_table_on_context)),
-ActionType.Ajax(tooltip='ç¦ç¨', icon='fa fa-ban text-danger',
-confirmText='ç¦ç¨å¹¶å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤', api='put:/
-l4d2/api/ban_chat?type=context&id=${id}'), ActionType.Ajax(tooltip='å é¤',
-icon='fa fa-times text-danger',
-confirmText='ä»å é¤è¯¥å­¦ä¹ çåå®¹åå¶ææåå¤ï¼ä½ä¸ç¦ç¨ï¼ä¾ç¶è½ç»§ç»­å­¦',
-api='delete:/l4d2/api/delete_chat?type=context&id=${id}') ], footable=True,
-columns=[TableColumn(label='ID', name='id', visible=False), TableColumn
-(type='tpl', tpl='${keywords|truncate:20}', label='åå®¹/å³é®è¯',
-name='keywords', searchable=True, popOver={'mode': 'dialog', 'title':
-'åå®¹å¨æ', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
-{keywords}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:
-ss}', label='æåå­¦ä¹ æ¶é´', name='time', sortable=True), TableColumn
-(label='å·²å­¦æ¬¡æ°', name='count', sortable=True), ]) message_page =
-PageSchema(url='/messages', icon='fa fa-comments',
-label='æ¬å°æå¡å¨ç®¡ç', schema=Page(title='æ¬å°æå¡å¨ç®¡ç', body=
-[ Alert(level=LevelEnum.info, className='white-space-pre-wrap', body=
-(f'æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n' #
-'Â·
-ç¹å»"ç¦ç¨"å¯ä»¥å°ææ¡èå¤©è®°å½è¿è¡ç¦ç¨ï¼è¿æ ·å¶ç¸å³çå­¦ä¹ å°±ä¼åå¥ç¦ç¨åè¡¨ã\n'
-# 'Â·
-ç¹å»"å é¤"å¯ä»¥å é¤ææ¡è®°å½ï¼ä½ä¸ä¼å½±åå®çå­¦ä¹ ã\n' f'Â·
+interval=60000, footable=True, itemActions=[ActionType.Url
+( tooltip='å å¥æ¸¸æ', icon='fa fa-gamepad', confirmText = "å å¥steam://
+connect/"+'${ip}', url= "steam://connect/"+'${ip}', # url= "http://"+'${ip}',
+blank= True ), ], columns = [ TableColumn(label='æä¸»', name='tag',
+searchable=True), TableColumn(label='åç§°', name='name', searchable=True),
+TableColumn(label='å°å¾', name='map_', searchable=True), TableColumn
+(label='ç©å®¶', name='rank_players', searchable=True), TableColumn
+(label='å»¶è¿', name='ping', searchable=True), TableColumn(label='IP å°å',
+name='ip', searchable=True), ]) message_page = PageSchema(url='/messages',
+icon='fa fa-comments', label='æ¬å°æå¡å¨ç®¡ç', schema=Page
+(title='æ¬å°æå¡å¨ç®¡ç', body=[ Alert(level=LevelEnum.info,
+className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n' f'Â·
 åè½ææªå®å')), message_table])) context_page = PageSchema(url='/
 contexts', icon='fa fa-comment', label='è¿ç¨æå¡å¨æ¥è¯¢', schema=Page
 (title='è¿ç¨æå¡å¨æ¥è¯¢', body=[Alert(level=LevelEnum.info,
 className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
 {NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n' # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
-'Â·
-ç¹å»"å é¤"å¯ä»¥å é¤è¯¥å­¦ä¹ ï¼è®©å®éæ°å¼å§å­¦ä¹ è¿å¥è¯ã')),
-context_table])) database_page = PageSchema(label='æ°æ®åº', icon='fa fa-
-database', children=[message_page, context_page]) config_page = PageSchema
-(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='éç½®',
-schema=Page(title='éç½®', initApi='/l4d2/api/get_group_list', body=
-[global_config_form, group_select, group_config_form])) chat_page = PageSchema
-(label='æ±çä¹è·¯', icon='fa fa-wechat (alias)', children=[config_page,
-database_page]) github_logo = Tpl(className='w-full', tpl='
+f'Â· åè½ææªå®å')), context_table])) database_page = PageSchema
+(label='æ°æ®åº', icon='fa fa-database', children=[message_page,
+context_page]) config_page = PageSchema(url='/configs', isDefaultPage=True,
+icon='fa fa-wrench', label='éç½®', schema=Page(title='éç½®', initApi='/
+l4d2/api/get_group_list', body=[global_config_form, group_select,
+group_config_form])) chat_page = PageSchema(label='æ±çä¹è·¯', icon='fa fa-
+wechat (alias)', children=[config_page, database_page]) github_logo = Tpl
+(className='w-full', tpl='
 ') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
 items=[github_logo]) admin_app = App(brandName='L4d2-Server', logo='https://
 raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/
 main/image/logo.png', header=header, pages=[{ 'children': [config_page,
 database_page] }], footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
 ')
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.1/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.4.2/nonebot_plugin_l4d2_server/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,77 +14,75 @@
 from .l4d2_queries import queries,player_queries
 from .l4d2_queries.qqgroup import *
 from .l4d2_server.workshop import workshop_to_dict
 from .l4d2_image.steam import url_to_byte
 import tempfile
 import random
 
-async def get_file(url:str,down_file:Path):
+
+
+async def get_file(url: str, down_file: Path):
     '''
     下载指定Url到指定位置
     '''
     try:
         if l4_only:
             maps = await url_to_byte(url)
         else:
             maps = httpx.get(url).content
         logger.info('已获取文件，尝试新建文件并写入')
-        with open(down_file ,'wb') as mfile:
+        with open(down_file, 'wb') as mfile:
             mfile.write(maps)
-            logger.info('下载成功')
-            mes ='文件已下载,正在解压'
+        logger.info('下载成功')
+        return '文件已下载，正在解压'
     except Exception as e:
         logger.info(f"文件获取不到/已损坏:原因是{e}")
-        mes = None
-    return mes
+        return None
+
 
-def get_vpk(vpk_list:list,path,file_:str = '.vpk'):
+def get_vpk(path: Path, file_: str = '.vpk') -> List[str]:
     '''
     获取所有vpk文件
     '''
-    for file in os.listdir(path):
-        if file.endswith(file_):
-            vpk_list.append(file)
-    return vpk_list
+    return [file for file in os.listdir(path) if file.endswith(file_)]
+
 
-def mes_list(mes:str,name_list:list):
-    n = 0
+def mes_list(mes: str, name_list: List[str]) -> str:
     if name_list:
-        for i in name_list:
-            n += 1
-            mes += "\n" + str(n) + "、" + i
+        for idx, name in enumerate(name_list):
+            mes += f'\n{idx+1}、{name}'
     return mes
 
 
 
-def del_map(num,map_path):
+
+def del_map(num: int, map_path: Path) -> str:
     '''
     删除指定的地图
     '''
-    vpk_list = []
-    map = get_vpk(vpk_list,map_path)
-    map_name = map[int(num)-1]
-    del_file = Path(map_path,map_name)
+    map = get_vpk(map_path)
+    map_name = map[num - 1]
+    del_file = map_path / map_name
     os.remove(del_file)
     return map_name
 
-def rename_map(num,rename,map_path):
+
+def rename_map(num: int, rename: str, map_path: Path) -> str:
     '''
     改名指定的地图
     '''
-    vpk_list = []
-    name = str(rename)
-    map = get_vpk(vpk_list,map_path)
-    map_name = map[int(num)-1]
-    old_file = Path(map_path,map_name)
-    new_file = Path(map_path,name)
-    os.rename(old_file,new_file)
+    map = get_vpk(map_path)
+    map_name = map[num - 1]
+    old_file = map_path / map_name
+    new_file = map_path / rename
+    os.rename(old_file, new_file)
     logger.info('改名成功')
     return map_name
 
+
 def text_to_png(msg: str) -> bytes:
     """文字转png"""
     return txt_to_img(msg)
 
 
 
 def solve(msg:str):
@@ -104,54 +102,35 @@
     return await write_player(id,msg,nickname)
 
 def name_exist(id:str):
     """删除绑定信息"""
     return del_player(id)
 
 async def get_message_at(data: str) -> list:
-    '''
-    获取at列表
-    :param data: event.json()
-    抄的groupmate_waifu
-    '''
-    qq_list = []
     data = json.loads(data)
-    try:
-        for msg in data['message']:
-            if msg['type'] == 'at':
-                qq_list.append(int(msg['data']['qq']))
-        return qq_list
-    except Exception:
-        return []
+    return [int(msg['data']['qq']) for msg in data['message'] if msg['type'] == 'at']
+
     
 
 def at_to_usrid(at):
-    """at对象变qqid否则返回usr_id"""
-    if at != []:
-        at:str = at[0]
-        usr_id:str = at
-        return usr_id
-    else:
-        return None
+    return at[0] if at else None
+
 
-async def command_server(msg:str):
-    """rcon控制台返回信息"""
+async def rcon_command(rcon, cmd):
+    return await rcon_server(rcon, cmd.strip())
+
+async def command_server(msg: str):
     rcon = await read_server_cfg_rcon()
-    l4_host_ = l4_host[CHECK_FILE]
-    l4_port_ = l4_port[CHECK_FILE]
-    logger.info([msg,l4_host_,l4_port_,rcon])
-    msg = await rcon_server(rcon,msg)
-    logger.info(msg)
-    if len(msg)==0:
+    msg = await rcon_command(rcon, msg)
+    if not msg:
         msg = '你可能发送了一个无用指令，或者换图导致服务器无响应'
-    if msg.startswith('Unknown command'):
-        msg = msg.replace('Unknown command','').strip()
-        msg = '无效指令：' + msg
-    msg = msg.strip()
-    return msg
+    elif msg.startswith('Unknown command'):
+        msg = '无效指令：' + msg.replace('Unknown command', '').strip()
+    return msg.strip().replace('\n', '')
+
 
 
 
 async def queries_server(msg:list) -> str:
     """查询ip返回信息"""
     print(msg)
     ip = msg[0]
@@ -254,39 +233,39 @@
      - 1、先匹配腐竹
      - 2、再匹配模式、没有参数则从直接匹配最上面的
      - 3、匹配数字（几服），没有参数则从结果里随机返回一个
     """
     data_dict = {}
     data_list = []
     msg = msg.replace(' ','')
-    n = 0
     # 腐竹循环
     for tag,value in ALL_HOST.items():
         value:List[dict]  
         if tag == key:
             data_dict.update({'server':tag})
-            n = 1
-            if msg == '':
+            if not msg:
                 # 腐竹
                 data_dict.update(random.choice(value))
             elif msg.isdigit():
                 logger.info("腐竹 + 序号")
                 for server in value:
                     if msg == str(server['id']):
                         data_dict.update(server)
+                        break
             else:
                 logger.info("腐竹 + 模式 + 序号")
                 for server in value:
                     if msg.startswith(server['version']):
-                        n = 2
                         data_list.append(server)
                         msg_id = msg[len(server['version']):]
                         if msg_id == str(server['id']):
-                            n = 3
                             data_dict.update(server)
-                if n == 2:
+                            break
+                else:
                     # 腐竹 + 模式
                     data_dict.update(random.choice(data_list))
+
     logger.info(data_dict)
     return data_dict
 
 
+
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/pyproject.toml` & `nonebot_plugin_l4d2_server-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.1"
-description = "L4D2 server related operations plugin for NoneBot"
+version = "0.4.2"
+description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
 classifiers = [
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_htmlrender = "^0.2.0.1"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
 asyncio = ">=3.4.3"
 jinja2 = ">=3.0.0"
@@ -36,15 +36,14 @@
 rcon = "^2.1.0"
 pillow = "^9.3.0"
 aiohttp = "^3.8.3"
 pyunpack = "^0.3.0"
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
-"ruamel.yaml" = "^0.17.21"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
 pandas = ">=1.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/README.md` & `nonebot_plugin_l4d2_server-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,22 @@
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
 
 <h2 id="gn">如何获取key</h2>
 
 为了使得ip不被滥用，我采取这种方式管理。
+
+这并不影响正常使用，如果不需要可以忽略
+
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
-        l4_tag = ['呆呆','橘']   # 这里是内置可以查询的服的list对象
-        l4_key = ''             # 这里是获取的key，是13个字符组成的字符串
+        l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
+        l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
 
 
 ## 🚑  提交自己的服务器？
 
 **本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
 
@@ -94,26 +97,32 @@
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
 | 云 | anne电信服云服 | 东 | 25
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
 | 橘 | 橘希实香的小窝 | 橘希实香 | 13
 | 竹 | 竹烨 | 竹烨oО柠檬茶 | 9
 | 音理 | 星空列车与白的旅行 | 音理 | 3
-| 尤 | 尤尤 | 晓音 | 2
-| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 1
+| 尤 | 尤尤 | 晓音 | 3
+| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
 
+### 0.4.2--2022.4.9
+
+ - 修复响应开头匹配出现的重大bug
+ - 启用web端
+ - web使用yaml管理，未来可能删除env配置
+
 ### 0.4.1--2022.3
 
  - 修复rar压缩包命名错误
  - 更新了tag的参数读取方式
  - 确定了传文件私聊比群聊快速
  - 修复了电信服计算错误
```

#### html2text {}

```diff
@@ -16,35 +16,38 @@
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
 ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
-[ç¹å»è¿éå ç¾¤](https://jq.qq.com/
-?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
+è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
+(https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
-l4_key = '' # è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
+l4_key = 'qwertyuiopasdfg' #
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
 æäº¤èªå·±çæå¡å¨ï¼
 **æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
 **é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
 ***** ð é»è®¤æå¡å¨ *****
 ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
-2 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 1 | ææ |
+3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.1--2022.3 -
+## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.2--2022.4.9 -
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
 ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/setup.py` & `nonebot_plugin_l4d2_server-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,27 @@
  'pandas>=1.5.2',
  'patool>=1.12,<2.0',
  'pillow>=9.3.0,<10.0.0',
  'python-a2s>=1.3.0,<2.0.0',
  'pyunpack>=0.3.0,<0.4.0',
  'rarfile>=4.0,<5.0',
  'rcon>=2.1.0,<3.0.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
  'srctools>=2.3.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.1',
-    'description': 'L4D2 server related operations plugin for NoneBot',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']\n    l4_file = [\'/home/ubuntu/l4d2/coop\']\n    l4_host = [\'127.0.0.1\']\n    l4_port = [\'20715\']\n    l4_rcon = [\'1145149191810\']\n    l4_font = \'simsun.ttc\'\n    l4_only = True\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://umamusume-agnes-digital.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']   # 这里是内置可以查询的服的list对象\n        l4_key = \'\'             # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 25\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 13\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 2\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 1\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-Digital)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Umamusume-Agnes-Digital/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
+    'version': '0.4.2',
+    'description': 'L4D2 server related operations plugin for NoneBot2',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']\n    l4_file = [\'/home/ubuntu/l4d2/coop\']\n    l4_host = [\'127.0.0.1\']\n    l4_port = [\'20715\']\n    l4_rcon = [\'1145149191810\']\n    l4_font = \'simsun.ttc\'\n    l4_only = True\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://umamusume-agnes-digital.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 25\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 13\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-Digital)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Umamusume-Agnes-Digital/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -10,18 +10,17 @@
 ['aiohttp>=3.8.3,<4.0.0', 'amis-python>=1.0.6,<2.0.0', 'asyncio>=3.4.3',
 'beautifulsoup4>=4.8.0', 'httpx>=0.23.3,<0.24.0', 'jieba>=0.42.1,<0.43.0',
 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc3,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
 'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
 a2s>=1.3.0,<2.0.0', 'pyunpack>=0.3.0,<0.4.0', 'rarfile>=4.0,<5.0',
-'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0', 'srctools>=2.3.9,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-l4d2-server', 'version': '0.4.1',
-'description': 'L4D2 server related operations plugin for NoneBot',
-'long_description': '
+'rcon>=2.1.0,<3.0.0', 'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name':
+'nonebot-plugin-l4d2-server', 'version': '0.4.2', 'description': 'L4D2 server
+related operations plugin for NoneBot2', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
          \n\n# nonebot_plugin_l4d2_server\n_â¨Nonebot & Left 4 Dead 2
                               serveræä½â¨_\n
@@ -39,34 +38,36 @@
 ***** ä¸»è¦åè½ *****
 \n\n- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
 åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)\n\n\n
 ***** å¦ä½è·åkey *****
-\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n
+\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n\nè¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥\n\n
 [ç¹å»è¿éå ç¾¤](https://jq.qq.com/
 ?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ\nå¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼\n\n
 l4_tag = [\'åå\',\'æ©\'] #
-è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡\n l4_key = \'\' #
+è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡\n l4_key = \'qwertyuiopasdfg\' #
 è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n\n\n## ð
 æäº¤èªå·±çæå¡å¨ï¼\n\n**æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**\n\n**é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**\n\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n\n
 {\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
 27031"\n }\n ]\n }\n\n
 ***** ð é»è®¤æå¡å¨ *****
 \nç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸»\n\n|
 æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3\n| äº | anneçµä¿¡æäºæ | ä¸
 | 25\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
 | 9\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
-æé³ | 2\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 1\n| ææ |
+æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
-15\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n\n### 0.4.1--2022.3\n\n -
+15\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n\n### 0.4.2--2022.4.9\n\n -
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n -
 ä¿®å¤raråç¼©åå½åéè¯¯\n - æ´æ°äºtagçåæ°è¯»åæ¹å¼\n -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n -
 ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n -
 æ°å¢webæ§å¶å°\n - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n - éåææ¡£\n -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n -
 æ°å¢ä¸æ¹ä¸è½½ç½ç\n - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯\n -
@@ -160,8 +161,8 @@
 - webæ§å¶å°çåæ³æ¥èªäºä»\n- [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè\n- åå -
 æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n', 'author': 'Agnes_Digital',
 'author_email': 'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'https://github.com/Umamusume-Agnes-Digital/
 nonebot_plugin_l4d2_server', 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.7,<4.0', } setup(**setup_kwargs)
+'>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.1/PKG-INFO` & `nonebot_plugin_l4d2_server-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.4.1
-Summary: L4D2 server related operations plugin for NoneBot
+Version: 0.4.2
+Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +36,14 @@
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: srctools (>=2.3.9,<3.0.0)
 Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
@@ -104,19 +102,22 @@
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
 
 <h2 id="gn">如何获取key</h2>
 
 为了使得ip不被滥用，我采取这种方式管理。
+
+这并不影响正常使用，如果不需要可以忽略
+
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
-        l4_tag = ['呆呆','橘']   # 这里是内置可以查询的服的list对象
-        l4_key = ''             # 这里是获取的key，是13个字符组成的字符串
+        l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
+        l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
 
 
 ## 🚑  提交自己的服务器？
 
 **本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
 
@@ -142,26 +143,32 @@
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
 | 云 | anne电信服云服 | 东 | 25
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
 | 橘 | 橘希实香的小窝 | 橘希实香 | 13
 | 竹 | 竹烨 | 竹烨oО柠檬茶 | 9
 | 音理 | 星空列车与白的旅行 | 音理 | 3
-| 尤 | 尤尤 | 晓音 | 2
-| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 1
+| 尤 | 尤尤 | 晓音 | 3
+| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
 
+### 0.4.2--2022.4.9
+
+ - 修复响应开头匹配出现的重大bug
+ - 启用web端
+ - web使用yaml管理，未来可能删除env配置
+
 ### 0.4.1--2022.3
 
  - 修复rar压缩包命名错误
  - 更新了tag的参数读取方式
  - 确定了传文件私聊比群聊快速
  - 修复了电信服计算错误
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.1 Summary:
-L4D2 server related operations plugin for NoneBot Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.2 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
-Z735803792@163.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
+Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: amis-python
-(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: beautifulsoup4
-(>=4.8.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: jieba
-(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Requires-
-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
-nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-
+Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-
+Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2
+(>=2.0.0rc3,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
 nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
 patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
 python-a2s (>=1.3.0,<2.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-
 Dist: rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
-ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/
-nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
+srctools (>=2.3.9,<3.0.0) Project-URL: Repository, https://github.com/
+Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server Description-Content-Type:
+text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
@@ -44,35 +43,38 @@
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
 ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
-[ç¹å»è¿éå ç¾¤](https://jq.qq.com/
-?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
+è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
+(https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
-l4_key = '' # è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
+l4_key = 'qwertyuiopasdfg' #
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ## ð
 æäº¤èªå·±çæå¡å¨ï¼
 **æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
 **é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
 ***** ð é»è®¤æå¡å¨ *****
 ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
-2 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 1 | ææ |
+3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.1--2022.3 -
+## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.2--2022.4.9 -
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
 ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
```

