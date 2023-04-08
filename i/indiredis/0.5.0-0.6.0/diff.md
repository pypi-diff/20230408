# Comparing `tmp/indiredis-0.5.0.tar.gz` & `tmp/indiredis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indiredis-0.5.0.tar", last modified: Sun Mar 12 19:25:11 2023, max compression
+gzip compressed data, was "indiredis-0.6.0.tar", last modified: Sat Apr  8 16:38:38 2023, max compression
```

## Comparing `indiredis-0.5.0.tar` & `indiredis-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,17 @@
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.535728 indiredis-0.5.0/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     1056 2023-03-09 20:41:53.000000 indiredis-0.5.0/LICENSE
--rw-rw-r--   0 bernard   (1000) bernard   (1000)       41 2023-03-09 20:41:53.000000 indiredis-0.5.0/MANIFEST.in
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     3502 2023-03-12 19:25:11.535728 indiredis-0.5.0/PKG-INFO
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     2587 2023-03-09 20:41:53.000000 indiredis-0.5.0/README.md
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.527728 indiredis-0.5.0/indiredis/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)    17855 2023-03-12 18:40:42.000000 indiredis-0.5.0/indiredis/__init__.py
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     3310 2023-03-11 17:14:36.000000 indiredis-0.5.0/indiredis/__main__.py
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.527728 indiredis-0.5.0/indiredis/indiredis/
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.531728 indiredis-0.5.0/indiredis/indiredis/data/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)    13939 2023-03-10 12:21:24.000000 indiredis-0.5.0/indiredis/indiredis/data/defaults.json
--rw-rw-r--   0 bernard   (1000) bernard   (1000)    64480 2023-03-10 22:48:31.000000 indiredis-0.5.0/indiredis/indiredis/data/project.json
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.531728 indiredis-0.5.0/indiredis/indiredis/data/textblocks_json/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     3008 2023-03-10 22:48:31.000000 indiredis-0.5.0/indiredis/indiredis/data/textblocks_json/en.json
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.527728 indiredis-0.5.0/indiredis/indiredis/static/
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.531728 indiredis-0.5.0/indiredis/indiredis/static/css/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     1524 2023-03-09 20:41:53.000000 indiredis-0.5.0/indiredis/indiredis/static/css/w3-theme-ski.css
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.531728 indiredis-0.5.0/indiredis/indiredis/static/images/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)      712 2023-03-09 20:41:53.000000 indiredis-0.5.0/indiredis/indiredis/static/images/logo.svg
--rw-rw-r--   0 bernard   (1000) bernard   (1000)      513 2023-03-09 20:41:53.000000 indiredis-0.5.0/indiredis/indiredis/static/images/logo_icon16.svg
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.535728 indiredis-0.5.0/indiredis/webcode/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)        0 2023-03-09 20:41:53.000000 indiredis-0.5.0/indiredis/webcode/__init__.py
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     1505 2023-03-11 17:09:55.000000 indiredis-0.5.0/indiredis/webcode/authenticate.py
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     1846 2023-03-10 15:01:26.000000 indiredis-0.5.0/indiredis/webcode/blobs.py
--rw-rw-r--   0 bernard   (1000) bernard   (1000)    52352 2023-03-11 14:57:14.000000 indiredis-0.5.0/indiredis/webcode/devices.py
--rw-rw-r--   0 bernard   (1000) bernard   (1000)    20618 2023-03-09 20:41:53.000000 indiredis-0.5.0/indiredis/webcode/setvalues.py
-drwxrwxr-x   0 bernard   (1000) bernard   (1000)        0 2023-03-12 19:25:11.531728 indiredis-0.5.0/indiredis.egg-info/
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     3502 2023-03-12 19:25:11.000000 indiredis-0.5.0/indiredis.egg-info/PKG-INFO
--rw-rw-r--   0 bernard   (1000) bernard   (1000)      664 2023-03-12 19:25:11.000000 indiredis-0.5.0/indiredis.egg-info/SOURCES.txt
--rw-rw-r--   0 bernard   (1000) bernard   (1000)        1 2023-03-12 19:25:11.000000 indiredis-0.5.0/indiredis.egg-info/dependency_links.txt
--rw-rw-r--   0 bernard   (1000) bernard   (1000)       41 2023-03-12 19:25:11.000000 indiredis-0.5.0/indiredis.egg-info/requires.txt
--rw-rw-r--   0 bernard   (1000) bernard   (1000)       10 2023-03-12 19:25:11.000000 indiredis-0.5.0/indiredis.egg-info/top_level.txt
--rw-rw-r--   0 bernard   (1000) bernard   (1000)       38 2023-03-12 19:25:11.535728 indiredis-0.5.0/setup.cfg
--rw-rw-r--   0 bernard   (1000) bernard   (1000)     1299 2023-03-10 15:17:37.000000 indiredis-0.5.0/setup.py
+-rw-r--r--   0        0        0     1056 2023-01-08 14:22:55.619352 indiredis-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3029 2023-04-07 21:50:40.093339 indiredis-0.6.0/README.md
+-rw-r--r--   0        0        0    27523 2023-04-07 21:39:09.514020 indiredis-0.6.0/indiredis/__init__.py
+-rw-r--r--   0        0        0     3310 2023-04-07 20:33:19.729769 indiredis-0.6.0/indiredis/__main__.py
+-rw-r--r--   0        0        0    13939 2023-03-17 15:56:20.966801 indiredis-0.6.0/indiredis/indiredis/data/defaults.json
+-rw-r--r--   0        0        0    64481 2023-04-07 20:34:39.214839 indiredis-0.6.0/indiredis/indiredis/data/project.json
+-rw-r--r--   0        0        0     3008 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/indiredis/data/textblocks_json/en.json
+-rw-r--r--   0        0        0     1524 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/css/w3-theme-ski.css
+-rw-r--r--   0        0        0      712 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/images/logo.svg
+-rw-r--r--   0        0        0      513 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/indiredis/static/images/logo_icon16.svg
+-rw-r--r--   0        0        0        0 2023-01-08 14:22:55.631352 indiredis-0.6.0/indiredis/webcode/__init__.py
+-rw-r--r--   0        0        0     1505 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/authenticate.py
+-rw-r--r--   0        0        0     1846 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/blobs.py
+-rw-r--r--   0        0        0    52352 2023-03-17 15:56:20.970802 indiredis-0.6.0/indiredis/webcode/devices.py
+-rw-r--r--   0        0        0    20618 2023-01-08 14:44:11.760425 indiredis-0.6.0/indiredis/webcode/setvalues.py
+-rw-r--r--   0        0        0     1000 2023-04-07 20:51:10.300544 indiredis-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 indiredis-0.6.0/PKG-INFO
```

### Comparing `indiredis-0.5.0/LICENSE` & `indiredis-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/PKG-INFO` & `indiredis-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: indiredis
-Version: 0.5.0
+Version: 0.6.0
 Summary: An INDI web client for general Instrument control. If the package is run, it provides a web service for controlling instruments. If imported, it provides functions which can be adapted to your own web server.
-Home-page: https://github.com/bernie-skipole/indi
-Author: Bernard Czenkusz
-Author-email: bernie@skipole.co.uk
-License: UNKNOWN
-Keywords: indi client astronomy instrument
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Keywords: indi,client,astronomy,instrument
+Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: skipole>=5.5.2
+Requires-Dist: indi-mr>=0.2.3
+Requires-Dist: paho-mqtt>=1.5.1
+Requires-Dist: redis>=3.5.3
+Requires-Dist: waitress>=1.4.4
+Project-URL: Documentation, https://indiredis.readthedocs.io
+Project-URL: Source, https://github.com/bernie-skipole/indi
 
 # indiredis
 
+
 This Python3 package provides an INDI web client for general Instrument control.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-The package does not include indiserver or drivers, but is compatable with them.
+The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client (or other INDI clients), can connect to this port and using an XML based protocol, control the connected instruments.
+
+Though the INDI protocol is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
+
+If this indiredis package is imported it provides functions for running a web client connected to either: an INDI server port; an MQTT server; or directly to INDI instrument drivers.
 
-Though INDI is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
+If indiredis is run with the python -m option, then the web client is started and connects to an INDI server port.
 
-The package can be imported, or run directly with the python -m option.
+This web client uses a redis database to hold instrument values, so a redis instance is needed, generally running on the same host as indiredis.
 
-For example:
+ For example:
 
-Your host should have a redis server running, typically with instruments connected by appropriate drivers and indiserver. For example, in one terminal, run:
+Your host typically has instruments connected by appropriate drivers and indiserver. For example, in one terminal, run:
 
 > indiserver -v indi_simulator_telescope indi_simulator_ccd
 
 Usage of this client is then:
 
 > python3 -m indiredis /path/to/blobfolder
 
-
 The directory /path/to/blobfolder should be a path to a directory of your choice, where BLOB's (Binary Large Objects), such as images will be stored, it will be created if it does not exist. Then connecting with a browser to http://localhost:8000 should enable you to view and control the connected instruments.
 
 For further usage information, including setting ports and hosts, try:
 
 > python3 -m indiredis --help
 
 
@@ -72,22 +76,16 @@
 
 skipole - framework used to build the web pages.
 
 waitress - Python web server.
 
 redis - Python redis client.
 
-## Security
-
-Only open communications are defined in this package, security and authentication are not considered.
+paho-mqtt - Python mqtt client.
 
-The web service provided here does not apply any authentication.
 
 ## Documentation
 
 If the package is imported into your own scripts, it provides functions which can be adapted to your own web server. Detailed information is available at:
 
 https://indiredis.readthedocs.io
 
-
-
-
```

### Comparing `indiredis-0.5.0/README.md` & `indiredis-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # indiredis
 
+
 This Python3 package provides an INDI web client for general Instrument control.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-The package does not include indiserver or drivers, but is compatable with them.
+The package does not include indiserver or drivers, but is compatable with them, indiserver is an application (debian package indi-bin) which runs instrument drivers, and listens on port 7624. This client (or other INDI clients), can connect to this port and using an XML based protocol, control the connected instruments.
+
+Though the INDI protocol is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
 
-Though INDI is generally used for astronomical instruments, it can work with any instrument if appropriate INDI drivers are available.
+If this indiredis package is imported it provides functions for running a web client connected to either: an INDI server port; an MQTT server; or directly to INDI instrument drivers.
 
-The package can be imported, or run directly with the python -m option.
+If indiredis is run with the python -m option, then the web client is started and connects to an INDI server port.
 
-For example:
+This web client uses a redis database to hold instrument values, so a redis instance is needed, generally running on the same host as indiredis.
 
-Your host should have a redis server running, typically with instruments connected by appropriate drivers and indiserver. For example, in one terminal, run:
+ For example:
+
+Your host typically has instruments connected by appropriate drivers and indiserver. For example, in one terminal, run:
 
 > indiserver -v indi_simulator_telescope indi_simulator_ccd
 
 Usage of this client is then:
 
 > python3 -m indiredis /path/to/blobfolder
 
-
 The directory /path/to/blobfolder should be a path to a directory of your choice, where BLOB's (Binary Large Objects), such as images will be stored, it will be created if it does not exist. Then connecting with a browser to http://localhost:8000 should enable you to view and control the connected instruments.
 
 For further usage information, including setting ports and hosts, try:
 
 > python3 -m indiredis --help
 
 
@@ -52,20 +56,15 @@
 
 skipole - framework used to build the web pages.
 
 waitress - Python web server.
 
 redis - Python redis client.
 
-## Security
+paho-mqtt - Python mqtt client.
 
-Only open communications are defined in this package, security and authentication are not considered.
-
-The web service provided here does not apply any authentication.
 
 ## Documentation
 
 If the package is imported into your own scripts, it provides functions which can be adapted to your own web server. Detailed information is available at:
 
 https://indiredis.readthedocs.io
-
-
```

### Comparing `indiredis-0.5.0/indiredis/__init__.py` & `indiredis-0.6.0/indiredis/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 Running indiredis with the python3 -m option, imports and runs the indi-mr function
 inditoredis, and creates a wsgi web application with the function make_wsgi_app().
 
 Finally it serves the web application with the Python waitress web server.
 
 Instead of running this indiredis package, you could import it, and then run
 make_wsgi_app() in your own script with your preferred web server.
-""" 
+"""
 
 
-import os, sys, pathlib, time, configparser, hashlib, threading
+import os, sys, pathlib, time, configparser, hashlib, threading, json
 
 from datetime import datetime
 
 from waitress import serve
 
-from skipole import WSGIApplication, use_submit_list, skis, ServeFile
+from skipole import WSGIApplication, use_submit_list, skis, ServeFile, set_debug
 
-from indi_mr import tools, inditoredis, indi_server, redis_server
+from indi_mr import tools, inditoredis, indi_server, redis_server, mqtttoredis, mqtt_server, driverstoredis
 
 PROJECTFILES = os.path.dirname(os.path.realpath(__file__))
 PROJECT = 'indiredis'
 
 
 def _start_call(called_ident, skicall):
     "When a call is initially received this function is called."
@@ -80,21 +80,21 @@
 def _submit_data(skicall):
     "This function is called when a Responder wishes to submit data for processing in some manner"
     return
 
 
 def _end_call(page_ident, page_type, skicall):
     """This function is called at the end of a call prior to filling the returned page with skicall.page_data"""
-    if ('authenticate' in skicall.call_data) and skicall.call_data['authenticate']:
+    if skicall.call_data.get('authenticate'):
         # a user has logged in, set a cookie
         return skicall.call_data['authenticate']
-    if ('logout' in skicall.call_data) and skicall.call_data['logout']:
+    if skicall.call_data.get('logout'):
         # a user has been logged out, set an invalid cookie in the client
         return "xxxxxxxx"
-        
+
     if "status" in skicall.call_data:
         # display a modal status message
         skicall.page_data["status", "para_text"] = skicall.call_data["status"]
         skicall.page_data["status", "hide"] = False
 
     # set device and group into a string to be sent as ident_data
         # with two checksums
@@ -133,15 +133,15 @@
     score = rconn.zscore(rediskey, receivedcookie)
     # if this cookie has a score of None, it does not exist
     if not score:
         return False
     # cookie exist, update its score - which is the unix timestamp
     rconn.zadd(rediskey, {receivedcookie:time.time()}, xx=True)
     return True
-    
+
 
 
 def make_wsgi_app(redisserver, blob_folder='', url="/", hashedpassword=""):
     """Create a wsgi application which can be served by a WSGI compatable web server.
     Reads and writes to redis stores created by indi-mr
 
     :param redisserver: Named Tuple providing the redis server parameters
@@ -154,15 +154,15 @@
     :type hashedpassword: String
     :return: A WSGI callable application
     :rtype: skipole.WSGIApplication
     """
 
     if blob_folder:
         blob_folder = pathlib.Path(blob_folder).expanduser().resolve()
-        
+
     # The web service needs a redis connection, available in tools
     rconn = tools.open_redis(redisserver)
     # and pass parameters in proj_data, note that resdiskey will be the key used to store cookies, created
     # as users log in
     proj_data = {"rconn":rconn,
                  "redisserver":redisserver,
                  "rediskey":redisserver.keyprefix + 'cookies',
@@ -181,59 +181,96 @@
         skisurl = url + "lib"
     else:
         skisurl = url + "/lib"
 
     skis_application = skis.makeapp()
     application.add_project(skis_application, url=skisurl)
 
+    #set_debug(True)
+
     return application
-    
+
 
 # The function confighelper helps generate a config file which should look like:
 
 #  [WEB]
 #  # Set this to the folder where Blobs will be stored
 #  blob_folder = path/to/blob/folder
 #  # Set this to a hashed password string which will be required to access the
 #  # web pages, or do not include this parameter if no password is required
 #  hashedpassword = hash-of-password
 #  # web service host and port
 #  host = localhost
 #  port = 8000
 #
+#  # only one of the following [INDI], [MQTT] or [DRIVERS] should
+#  # be given. They are mutually exclusive.
+#
 #  [INDI]
 #  # indi server host and port
 #  ihost = localhost
 #  iport = 7624
 #
+#  [MQTT]
+#  # mqtt server host, port and client id
+#  mhost = localhost
+#  mport = 1883
+#  mqtt_id = indi_client01
+#  # mqtt topics
+#  to_indi_topic = to_indi
+#  from_indi_topic = from_indi
+#  snoop_control_topic = snoop_control
+#  snoop_data_topic = snoop_data
+#
+#  [MQTT.SUBSCRIBE_LIST]
+#  # A list of remote mqtt_id's to subscribe to, for example
+#  indi_drivers01
+#  indi_drivers02
+#
+#  [DRIVERS]
+#  # a list of drivers, for example
+#  indi_simulator_telescope
+#  indi_simulator_ccd
+#
 #  [REDIS]
 #  # redis server host and port
 #  rhost = localhost
 #  rport = 6379
 #  # Prefix applied to redis keys
 #  prefix = indi_
 #  # Redis channel used to publish data to indiserver
 #  toindipub = to_indi
-#  # Redis channel on which data is published from indiserver 
+#  # Redis channel on which data is published from indiserver
 #  fromindipub = from_indi
 
 
 
 def confighelper(path):
     """This generates a config file and is normally run in the python REPL,
     path should be the path of the file you wish to make, and should not
     already exist. You will be asked a series of questions and then the
     file will be generated.
-       
+
     :param path: path of the file to be generated
     :type path: String
     """
-    
+
     hp = "localhost:8000"
     ihp = "localhost:7624"
+    ihost = ""
+    mhp = "localhost:1883"
+    mhost = ""
+    mqtt_id = "indi_client01"
+    newmid = ""
+    to_topic = 'to_indi'
+    from_topic = 'from_indi'
+    control_topic = 'snoop_control'
+    data_topic = 'snoop_data'
+    remote_ids = set()
+    drivers = set()
     rhp = "localhost:6379"
     prefix = "indi_"
     toindipub = "to_indi"
     fromindipub = "from_indi"
 
     # the path should be to a directory which exits, but not an existing file
 
@@ -261,33 +298,136 @@
         except:
             print("Invalid web host:port")
             continue
         print("Value set at : " + newhp + "\n")
         q = input("OK (y/n)?")
         if q == "y" or q == "Y":
             break
-        
-    while True:
-        print("\nType in the host and port of the indi service to connect to,\nas colon separated host:number")
-        newihp = input("Currently : " + ihp + "\nEnter to accept, or input new value>")
-        if not newihp:
-            newihp = ihp
-        if ":" not in newihp:
-            print("Invalid indi host:port")
-            continue
-        try:
-            ihost,iport = newihp.split(":")
-            iport = int(iport)
-        except:
-            print("Invalid indi host:port")
-            continue
-        print("Value set at : " + newihp + "\n")
-        q = input("OK (y/n)?")
+
+    print("\nYou can specify one of the following three:")
+    print("The host:port of an INDI server (which itself connects to instruments and drivers).")
+    print("Or\nThe host:port of an MQTT server (which connect to instruments using the indi-mr package).")
+    print("Or\nA list of indi drivers, which in turn connect to instruments.\n")
+    q = input("Do you wish to connect to an INDI server (y/n)?")
+    if q == "y" or q == "Y":
+        while True:
+            print("\nType in the host and port of the indi service to connect to,\nas colon separated host:number")
+            newihp = input("Currently : " + ihp + "\nEnter to accept, or input new value>")
+            if not newihp:
+                newihp = ihp
+            if ":" not in newihp:
+                print("Invalid indi host:port")
+                continue
+            try:
+                ihost,iport = newihp.split(":")
+                iport = int(iport)
+            except:
+                print("Invalid indi host:port")
+                continue
+            print("Value set at : " + newihp + "\n")
+            q = input("OK (y/n)?")
+            if q == "y" or q == "Y":
+                break
+    else:
+        # Not indi server, could be mqtt or drivers
+        q = input("\nDo you wish to connect to an MQTT server (y/n)?")
         if q == "y" or q == "Y":
-            break
+            while True:
+                print("\nType in the host and port of the mqtt service to connect to,\nas colon separated host:number")
+                newmhp = input("Currently : " + mhp + "\nEnter to accept, or input new value>")
+                if not newmhp:
+                    newmhp = mhp
+                if ":" not in newmhp:
+                    print("Invalid mqtt host:port")
+                    continue
+                try:
+                    mhost,mport = newmhp.split(":")
+                    mport = int(mport)
+                except:
+                    print("Invalid mqtt host:port")
+                    continue
+                print("Value set at : " + newmhp + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            while True:
+                print("\nType in a string which will be the MQTT client ID.\nThis should be unique if there are multiple MQTT clients.")
+                newmid = input("Currently : " + mqtt_id + "\nEnter to accept, or input new string>")
+                if not newmid:
+                    newmid = mqtt_id
+                print("String set at : " + newmid + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            while True:
+                print("\nType in a string which will be the MQTT topic communicating to drivers.")
+                to_indi_topic = input("Currently : " + to_topic + "\nEnter to accept, or input new string>")
+                if not to_indi_topic:
+                    to_indi_topic = to_topic
+                print("String set at : " + to_indi_topic + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            while True:
+                print("\nType in a string which will be the MQTT topic communicating to the client.")
+                from_indi_topic = input("Currently : " + from_topic + "\nEnter to accept, or input new string>")
+                if not from_indi_topic:
+                    from_indi_topic = from_topic
+                print("String set at : " + from_indi_topic + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            while True:
+                print("\nType in a string which will be the MQTT topic used for driver snoop control.")
+                snoop_control_topic = input("Currently : " + control_topic + "\nEnter to accept, or input new string>")
+                if not snoop_control_topic:
+                    snoop_control_topic = control_topic
+                print("String set at : " + snoop_control_topic + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            while True:
+                print("\nType in a string which will be the MQTT topic used for driver snoop data.")
+                snoop_data_topic = input("Currently : " + data_topic + "\nEnter to accept, or input new string>")
+                if not snoop_data_topic:
+                    snoop_data_topic = data_topic
+                print("String set at : " + snoop_data_topic + "\n")
+                q = input("OK (y/n)?")
+                if q == "y" or q == "Y":
+                    break
+            print("/nDo you want to list the remote driver mqtt id's to which this client connects?")
+            print("If not then the client will connect (subscribe) to all mqtt id's")
+            q = input("List mqtt id's to subscribe to (y/n)?")
+            if q == "y" or q == "Y":
+                # fill section MQTT.SUBSCRIBE_LIST
+                print("\nType an id string and Enter, you will then be prompted for the next id.")
+                print("Continue adding id's, and then just press Enter without input to finish.")
+                while True:
+                    idstring = input("mqtt_id : ")
+                    idstring = idstring.strip(" \"\'")
+                    if not idstring:
+                        break
+                    remote_ids.add(dstring)
+        else:
+            # neither indi nor mqtt servers, therfore should be drivers
+            q = input("\nDo you wish to define one or more drivers (y/n)?")
+            if q != "y" and q != "Y":
+                print("No other options are available. Exiting without creating config file")
+                sys.exit(0)
+            print("\nType a driver string and Enter, you will then be prompted for the next driver.")
+            print("Continue adding drivers, and then just press Enter without input to finish.")
+            while True:
+                dstring = input("Driver : ")
+                dstring = dstring.strip(" \"\'")
+                if not dstring:
+                    break
+                drivers.add(dstring)
+            if not drivers:
+                print("No drivers specified, no other options are available. Exiting without creating config file")
+                sys.exit(0)
 
     while True:
         print("\nType in the host and port of the redis service to connect to,\nas colon separated host:number")
         newrhp = input("Currently : " + rhp + "\nEnter to accept, or input new value>")
         if not newrhp:
             newrhp = rhp
         if ":" not in newrhp:
@@ -362,34 +502,56 @@
         sys.exit(0)
 
     if password:
         hashedpassword = hashlib.sha512( password.encode('utf-8') ).hexdigest()
         hashedpasswordkey = 'hashedpassword'
     else:
         hashedpassword = None
-        hashedpasswordkey = '# hashedpassword'
-        
+        hashedpasswordkey = '# hashedpassword ='
+
 
     config = configparser.ConfigParser(allow_no_value=True)
 
     config['WEB'] =        { "# Set this to the folder where Blobs will be stored": None,
                              'blob_folder': blob_folder,
                              "# Set this to a hashed password string which will be required to access the": None,
                              "# web pages, or do not include this parameter if no password is required": None,
                              hashedpasswordkey: hashedpassword,
                              '# web service host and port': None,
                              'host': host,
                              'port': port
                            }
-                             
 
-    config['INDI'] =       { '# indi server host and port': None,
+    if ihost:
+        config['INDI'] =   { '# indi server host and port': None,
                              'ihost': ihost,
                              'iport': iport
                            }
+    elif mhost:
+        config['MQTT'] =   { '# mqtt server host, port and client id': None,
+                             'mhost': mhost,
+                             'mport': mport,
+                             'mqtt_id': newmid,
+                             '# mqtt topics': None,
+                             'to_indi_topic': to_indi_topic,
+                             'from_indi_topic': from_indi_topic,
+                             'snoop_control_topic': snoop_control_topic,
+                             'snoop_data_topic': snoop_data_topic
+                           }
+        if remote_ids:
+            iddict = { "# A list of remote mqtt_id's to subscribe to, for example": None }
+            for ids in remote_ids:
+                iddict[ids] = None
+            config['MQTT.SUBSCRIBE_LIST'] = iddict
+
+    elif drivers:
+        driverdict = { '# a list of drivers': None }
+        for driver in drivers:
+            driverdict[driver] = None
+        config['DRIVERS'] = driverdict
 
     config['REDIS'] =      { '# redis server host and port': None,
                              'rhost': rhost,
                              'rport': rport,
                              '# Prefix applied to redis keys': None,
                              'prefix': newprefix,
                              '# Redis channel used to publish data to indiserver': None,
@@ -404,66 +566,100 @@
 
     print(f"File {configfile} has been created")
     sys.exit(0)
 
 
 def _read_config(configfile):
     "Reads the configfile and returns dictionary of parameters"
-    config = configparser.ConfigParser()
+    config = configparser.ConfigParser(allow_no_value=True)
     config.read(configfile)
     configdict = {}
+    if 'WEB' not in config:
+        print("ERROR: The config file does not include a WEB section.")
+        sys.exit(1)
     webparams = config['WEB']
     configdict['blob_folder'] = webparams['blob_folder']
     configdict['hashedpassword'] = webparams.get('hashedpassword', '')
     configdict['host'] = webparams.get('host', 'localhost')
     configdict['port'] = webparams.getint('port', 8000)
-    indiparams = config['INDI']
-    configdict['ihost'] = indiparams.get('ihost', 'localhost')
-    configdict['iport'] = indiparams.getint('iport', 7624)
+    if 'INDI' in config:
+        indiparams = config['INDI']
+        configdict['ihost'] = indiparams.get('ihost', 'localhost')
+        configdict['iport'] = indiparams.getint('iport', 7624)
+    elif 'MQTT' in config:
+        mqttparams = config['MQTT']
+        configdict['mhost'] = mqttparams.get('mhost', 'localhost')
+        configdict['mport'] = mqttparams.getint('mport', 1883)
+        configdict['mqtt_id'] = mqttparams.get('mqtt_id', 'indi_client01')
+        configdict['to_indi_topic'] = mqttparams.get('to_indi_topic', 'to_indi')
+        configdict['from_indi_topic'] = mqttparams.get('from_indi_topic', 'from_indi')
+        configdict['snoop_control_topic'] = mqttparams.get('snoop_control_topic', 'snoop_control')
+        configdict['snoop_data_topic'] = mqttparams.get('snoop_data_topic', 'snoop_data')
+        if 'MQTT.SUBSCRIBE_LIST' in config:
+            subscribe_list = config['MQTT.SUBSCRIBE_LIST']
+            configdict['subscribe_list'] = list(subscribe_list.keys())
+        else:
+            configdict['subscribe_list'] = []
+    elif 'DRIVERS' in config:
+        drivers = config['DRIVERS']
+        configdict['drivers'] = list(drivers.keys())
+        if not configdict['drivers']:
+            print("ERROR: No drivers given under DRIVERS.")
+            sys.exit(1)
+    else:
+        print("ERROR: No INDI, MQTT or DRIVERS section in the config file.")
+        sys.exit(1)
+    if 'REDIS' not in config:
+        print("ERROR: The config file does not include a REDIS section.")
+        sys.exit(1)
     redisparams = config['REDIS']
     configdict['rhost'] = redisparams.get('rhost', 'localhost')
     configdict['rport'] = redisparams.getint('rport', 6379)
     configdict['prefix'] = redisparams.get('prefix', 'indi_')
     configdict['toindipub'] = redisparams.get('toindipub', 'to_indi')
     configdict['fromindipub'] = redisparams.get('fromindipub', 'from_indi')
     return configdict
-    
+
 
 def runclient(configfile):
     """Blocking call, which given the path to a config reads the
-    parameters and runs the web client 
+    parameters and runs the web client
 
     :param configfile: path to the config file
     :type configfile: String
     """
-    
+
     configfile = os.path.abspath(os.path.expanduser(configfile))
     if not os.path.isfile(configfile):
         print("The configuration file has not been found")
         sys.exit(1)
 
     configdict = _read_config(configfile)
 
-    # define the hosts/ports where servers are listenning, these functions return named tuples
-    # which are required as arguments to inditoredis() and to make_wsgi_app()
-
-    indi_host = indi_server(host=configdict["ihost"], port=configdict["iport"])
     redis_host = redis_server(host=configdict["rhost"], port=configdict["rport"],
                               db=0, password='',
                               keyprefix=configdict['prefix'],
                               to_indi_channel=configdict['toindipub'],
                               from_indi_channel=configdict['fromindipub'])
 
     # create a wsgi application
     application = make_wsgi_app(redis_host, configdict['blob_folder'], url='/', hashedpassword=configdict['hashedpassword'])
 
     # serve the application with the python waitress web server in another thread
     webapp = threading.Thread(target=serve, args=(application,), kwargs={'host':configdict['host'], 'port':configdict['port']})
     webapp.start()
 
-    # and start the blocking function inditoredis
-    inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=configdict['blob_folder'])
-
-
-
-
-
+    if "ihost" in configdict:
+        indi_host = indi_server(host=configdict["ihost"], port=configdict["iport"])
+        # start the blocking function inditoredis
+        inditoredis(indi_host, redis_host, log_lengths={}, blob_folder=configdict['blob_folder'])
+    elif "mhost" in configdict:
+        mqtt_host = mqtt_server(host=configdict["mhost"], port=configdict["mport"],
+                                to_indi_topic = configdict['to_indi_topic'],
+                                from_indi_topic = configdict['from_indi_topic'],
+                                snoop_control_topic = configdict['snoop_control_topic'],
+                                snoop_data_topic = configdict['snoop_data_topic'] )
+        # start the blocking function mqtttoredis
+        mqtttoredis(configdict['mqtt_id'], mqtt_host, redis_host, subscribe_list=configdict['subscribe_list'], blob_folder=configdict['blob_folder'])
+    elif "drivers" in configdict:
+        # start the blocking function driverstoredis
+        driverstoredis(configdict['drivers'], redis_host, blob_folder=configdict['blob_folder'])
```

### Comparing `indiredis-0.5.0/indiredis/__main__.py` & `indiredis-0.6.0/indiredis/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # in this example the web server 'waitress' is used
 
 from waitress import serve
 
 from . import make_wsgi_app
 
 
-version = "0.5.0"
+version = "0.6.0"
 
 if __name__ == "__main__":
 
 
     parser = argparse.ArgumentParser(usage="python3 -m indiredis [options] blobdirectorypath",
         description="INDI web client communicating to indiserver and saving data to redis and to a BLOB directory.")
     parser.add_argument("blobdirectorypath", help="Path of the directory where BLOB's will be set")
```

### Comparing `indiredis-0.5.0/indiredis/indiredis/data/defaults.json` & `indiredis-0.6.0/indiredis/indiredis/data/defaults.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/indiredis/data/project.json` & `indiredis-0.6.0/indiredis/indiredis/data/project.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.6.0'"}*

```diff
@@ -4317,9 +4317,9 @@
         "skipolelogo": 3001,
         "url_not_found": 2080,
         "validate_error": 2010,
         "w3_css": "skis,w3_css",
         "w3_theme_ski_css": 1008
     },
     "url": "/",
-    "version": "0.5.0"
+    "version": "0.6.0"
 }
```

### Comparing `indiredis-0.5.0/indiredis/indiredis/data/textblocks_json/en.json` & `indiredis-0.6.0/indiredis/indiredis/data/textblocks_json/en.json`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/indiredis/static/css/w3-theme-ski.css` & `indiredis-0.6.0/indiredis/indiredis/static/css/w3-theme-ski.css`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/indiredis/static/images/logo.svg` & `indiredis-0.6.0/indiredis/indiredis/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/indiredis/static/images/logo_icon16.svg` & `indiredis-0.6.0/indiredis/indiredis/static/images/logo_icon16.svg`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/webcode/authenticate.py` & `indiredis-0.6.0/indiredis/webcode/authenticate.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/webcode/blobs.py` & `indiredis-0.6.0/indiredis/webcode/blobs.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/webcode/devices.py` & `indiredis-0.6.0/indiredis/webcode/devices.py`

 * *Files identical despite different names*

### Comparing `indiredis-0.5.0/indiredis/webcode/setvalues.py` & `indiredis-0.6.0/indiredis/webcode/setvalues.py`

 * *Files identical despite different names*

