# Comparing `tmp/360monitoringcli-1.0.8.tar.gz` & `tmp/360monitoringcli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "360monitoringcli-1.0.8.tar", last modified: Mon Feb 13 09:48:07 2023, max compression
+gzip compressed data, was "360monitoringcli-1.0.9.tar", last modified: Thu Feb 16 09:55:27 2023, max compression
```

## Comparing `360monitoringcli-1.0.8.tar` & `360monitoringcli-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:48:07.760376 360monitoringcli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/360monitoring-example.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:48:07.756376 360monitoringcli-1.0.8/360monitoringcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-13 09:48:07.000000 360monitoringcli-1.0.8/360monitoringcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-02-13 09:48:07.760376 360monitoringcli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:48:07.760376 360monitoringcli-1.0.8/cli360monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:48:07.760376 360monitoringcli-1.0.8/cli360monitoring/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/bcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6207 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10427 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/servers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10236 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/statistics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3585 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/lib/usertokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17727 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/cli360monitoring/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 09:48:07.760376 360monitoringcli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-13 09:47:57.000000 360monitoringcli-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:27.645772 360monitoringcli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/360monitoring-example.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:27.641772 360monitoringcli-1.0.9/360monitoringcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-16 09:55:27.000000 360monitoringcli-1.0.9/360monitoringcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-02-16 09:55:27.645772 360monitoringcli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:27.641772 360monitoringcli-1.0.9/cli360monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:27.645772 360monitoringcli-1.0.9/cli360monitoring/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/bcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6222 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11990 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/servers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10924 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/statistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/lib/usertokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17966 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/cli360monitoring/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 09:55:27.645772 360monitoringcli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-16 09:55:16.000000 360monitoringcli-1.0.9/setup.py
```

### Comparing `360monitoringcli-1.0.8/360monitoringcli.egg-info/PKG-INFO` & `360monitoringcli-1.0.9/360monitoringcli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 360monitoringcli
-Version: 1.0.8
+Version: 1.0.9
 Summary: 360 Monitoring CLI
 Home-page: https://github.com/plesk/360monitoring-cli
 Author: Jan Loeffler
 Author-email: jan.loeffler@webpros.com
 Maintainer: Jan Loeffler
 Maintainer-email: jan.loeffler@webpros.com
 License: MIT
@@ -58,15 +58,15 @@
 
 ### Test 360 Monitoring CLI for specific staging version
 
  To test a package from staging you can simply deploy a docker container:
 
     $ docker run -it --rm ubuntu /bin/bash
     $ apt-get update && apt-get install -y python3 && apt-get install -y pip
-    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.7"
+    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.9"
 
 ### For developement, install required Python modules
 
  * To test the code locally, install the Python modules "requests", "configparser", "argparse" and "prettytable"
  * Create an alias for "360monitoring=./monitoring.py"
 
     $ pip install requests
@@ -85,15 +85,18 @@
     $ ./test_cli.sh "360monitoring"
 ## Usage
 
     $ 360monitoring --help                        display general help
     $ 360monitoring config save --api-key KEY     configure API KEY to connect to 360 Monitoring account
     $ 360monitoring statistics                    display all assets of your account
     $ 360monitoring servers list                  display all monitored servers
+    $ 360monitoring servers list --issues         display monitored servers with issues only
+    $ 360monitoring servers list --tag cpanel     display only servers with tag "cpanel"
     $ 360monitoring sites list                    display all monitored sites
+    $ 360monitoring sites list --issues           display monitored sites with issues only
     $ 360monitoring contacts list                 display all contacts
     $ 360monitoring usertokens list               display user tokens
     $ 360monitoring config print                  display your current settings and where those are stored
 
     $ 360monitoring sites add --url domain.tld    start monitoring a new website
     $ 360monitoring servers update --name cpanel123.hoster.com --tag production   tag a specific server
```

### Comparing `360monitoringcli-1.0.8/360monitoringcli.egg-info/SOURCES.txt` & `360monitoringcli-1.0.9/360monitoringcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `360monitoringcli-1.0.8/LICENSE` & `360monitoringcli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `360monitoringcli-1.0.8/PKG-INFO` & `360monitoringcli-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 360monitoringcli
-Version: 1.0.8
+Version: 1.0.9
 Summary: 360 Monitoring CLI
 Home-page: https://github.com/plesk/360monitoring-cli
 Author: Jan Loeffler
 Author-email: jan.loeffler@webpros.com
 Maintainer: Jan Loeffler
 Maintainer-email: jan.loeffler@webpros.com
 License: MIT
@@ -58,15 +58,15 @@
 
 ### Test 360 Monitoring CLI for specific staging version
 
  To test a package from staging you can simply deploy a docker container:
 
     $ docker run -it --rm ubuntu /bin/bash
     $ apt-get update && apt-get install -y python3 && apt-get install -y pip
-    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.7"
+    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.9"
 
 ### For developement, install required Python modules
 
  * To test the code locally, install the Python modules "requests", "configparser", "argparse" and "prettytable"
  * Create an alias for "360monitoring=./monitoring.py"
 
     $ pip install requests
@@ -85,15 +85,18 @@
     $ ./test_cli.sh "360monitoring"
 ## Usage
 
     $ 360monitoring --help                        display general help
     $ 360monitoring config save --api-key KEY     configure API KEY to connect to 360 Monitoring account
     $ 360monitoring statistics                    display all assets of your account
     $ 360monitoring servers list                  display all monitored servers
+    $ 360monitoring servers list --issues         display monitored servers with issues only
+    $ 360monitoring servers list --tag cpanel     display only servers with tag "cpanel"
     $ 360monitoring sites list                    display all monitored sites
+    $ 360monitoring sites list --issues           display monitored sites with issues only
     $ 360monitoring contacts list                 display all contacts
     $ 360monitoring usertokens list               display user tokens
     $ 360monitoring config print                  display your current settings and where those are stored
 
     $ 360monitoring sites add --url domain.tld    start monitoring a new website
     $ 360monitoring servers update --name cpanel123.hoster.com --tag production   tag a specific server
```

### Comparing `360monitoringcli-1.0.8/README.md` & `360monitoringcli-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 ### Test 360 Monitoring CLI for specific staging version
 
  To test a package from staging you can simply deploy a docker container:
 
     $ docker run -it --rm ubuntu /bin/bash
     $ apt-get update && apt-get install -y python3 && apt-get install -y pip
-    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.7"
+    $ pip install -i https://test.pypi.org/simple/ --force-reinstall -v "360monitoringcli==1.0.9"
 
 ### For developement, install required Python modules
 
  * To test the code locally, install the Python modules "requests", "configparser", "argparse" and "prettytable"
  * Create an alias for "360monitoring=./monitoring.py"
 
     $ pip install requests
@@ -58,15 +58,18 @@
     $ ./test_cli.sh "360monitoring"
 ## Usage
 
     $ 360monitoring --help                        display general help
     $ 360monitoring config save --api-key KEY     configure API KEY to connect to 360 Monitoring account
     $ 360monitoring statistics                    display all assets of your account
     $ 360monitoring servers list                  display all monitored servers
+    $ 360monitoring servers list --issues         display monitored servers with issues only
+    $ 360monitoring servers list --tag cpanel     display only servers with tag "cpanel"
     $ 360monitoring sites list                    display all monitored sites
+    $ 360monitoring sites list --issues           display monitored sites with issues only
     $ 360monitoring contacts list                 display all contacts
     $ 360monitoring usertokens list               display user tokens
     $ 360monitoring config print                  display your current settings and where those are stored
 
     $ 360monitoring sites add --url domain.tld    start monitoring a new website
     $ 360monitoring servers update --name cpanel123.hoster.com --tag production   tag a specific server
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/config.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/config.py`

 * *Files identical despite different names*

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/contacts.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/contacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,21 +149,21 @@
             if self.config.hide_ids:
                 self.table.del_column('ID')
             print(self.table)
 
     def print(self, contact):
         """Print the data of the specified contact"""
 
+        if (self.format == 'json'):
+            print(json.dumps(contact, indent=4))
+            return
+
         id = contact['id']
         name = contact['name']
         email = contact['email'] if 'email' in contact else ''
         phone = contact['phonenumber'] if 'phonenumber' in contact else ''
         method = contact['method'] if 'method' in contact else ''
 
-        if (self.format == 'table'):
-            self.table.add_row([id, name, email, phone, method])
-
-        elif (self.format == 'csv'):
+        if (self.format == 'csv'):
             print(f"{id};{name};{email};{phone};{method}")
-
         else:
-            print(json.dumps(contact, indent=4))
+            self.table.add_row([id, name, email, phone, method])
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/servers.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,45 +72,72 @@
         if response.status_code == 200:
             print('Updated tags of server', serverId, 'to', tags)
             return True
         else:
             printError('Failed to update server', serverId, 'with response code:', response.status_code)
             return False
 
-    def list(self, tags):
+    def list(self, issuesOnly: bool, tags):
         """Iterate through list of server monitors and print details"""
 
         if self.fetchData():
             self.printHeader()
 
             # Iterate through list of monitors and print urls, etc.
             for server in self.servers:
                 if len(tags) == 0:
-                    self.print(server)
+                    if (not issuesOnly) or self.hasIssue(server):
+                        self.print(server)
                 elif 'tags' in server:
                     match = True
                     for tag in tags:
                         if not tag in server['tags']:
                             match = False
                             break
                     if match:
-                        self.print(server)
+                        if (not issuesOnly) or self.hasIssue(server):
+                            self.print(server)
 
             self.printFooter()
 
     def setTags(self, pattern: str, tags):
         """Set the tags for the server specified with pattern. Pattern can be either the server ID or its name"""
 
         if pattern and len(tags) > 0 and self.fetchData():
             for server in self.servers:
                 if pattern == server['id'] or pattern in server['name']:
                     return self.update(server['id'], tags)
 
         printWarn('No server with given pattern found: ' + pattern)
 
+    def hasIssue(self, server):
+        """Return True if the specified server has some issue by having a value outside of the expected threshold specified in config file"""
+
+        cpu_usage_percent = server['summary']['cpu_usage_percent'] if 'summary' in server else 0
+        mem_usage_percent = server['summary']['mem_usage_percent'] if 'summary' in server else 0
+        disk_usage_percent = server['summary']['disk_usage_percent'] if 'summary' in server else 0
+
+        if cpu_usage_percent >= float(self.config.threshold_cpu_usage) \
+            or mem_usage_percent >= float(self.config.threshold_mem_usage) \
+            or disk_usage_percent >= float(self.config.threshold_disk_usage):
+            return True
+
+        last_data = server['last_data']
+        if 'df' in last_data:
+            for disk in last_data['df']:
+                free_disk_space = disk['free_bytes']
+                used_disk_space = disk['used_bytes']
+                total_disk_space = free_disk_space + used_disk_space
+                free_disk_space_percent = free_disk_space / total_disk_space * 100
+
+                if free_disk_space_percent <= float(self.config.threshold_free_diskspace):
+                    return True
+
+        return False
+
     def printHeader(self):
         """Print CSV if CSV format requested"""
 
         if (self.format == 'csv'):
             print('id;server name;ip address;status;os;cpu usage %;mem usage %;disk usage %;free disk space;tags')
 
         self.sum_cpu_usage = 0
@@ -161,30 +188,40 @@
             print("\n".join(list_of_table_lines[:-(result_lines + 1)]))
             print(horizontal_line)
             print("\n".join(list_of_table_lines[-(result_lines + 1):]))
 
     def print(self, server):
         """Print the data of the specified server monitor"""
 
+        if (self.format == 'json'):
+            print(json.dumps(server, indent=4))
+            return
+
         id = server['id']
         name = server['name']
         os = server['os'] if 'os' in server else ''
         agent_version = server['agent_version'] if 'agent_version' in server else ''
         status = server['status'] if 'status' in server else ''
         last_data = server['last_data']
         uptime_seconds = last_data['uptime']['seconds'] if 'uptime' in last_data else 0
         cores = last_data['cores'] if 'cores' in last_data else 0
         memory_used = last_data['memory']['used'] if 'memory' in last_data else 0
         memory_free = last_data['memory']['free'] if 'memory' in last_data else 0
         memory_available = last_data['memory']['available'] if 'memory' in last_data else 0
         memory_total = last_data['memory']['total'] if 'memory' in last_data else 0
         connecting_ip = server['connecting_ip'] if 'connecting_ip' in server else ''
-        ip_address = server['ip_whois']['ip'] if 'ip_whois' in server else ''
-        ip_country = server['ip_whois']['country'] if 'ip_whois' in server else ''
-        ip_hoster = server['ip_whois']['org'] if 'ip_whois' in server else ''
+        if 'ip_whois' in server:
+            ip_whois = server['ip_whois']
+            ip_address = ip_whois['ip'] if 'ip' in ip_whois else ''
+            ip_country = ip_whois['country'] if 'country' in ip_whois else ''
+            ip_hoster = ip_whois['org'] if 'org' in ip_whois else ''
+        else:
+            ip_address = ''
+            ip_country = ''
+            ip_hoster = ''
         cpu_usage_percent = server['summary']['cpu_usage_percent'] if 'summary' in server else 0
         mem_usage_percent = server['summary']['mem_usage_percent'] if 'summary' in server else 0
         disk_usage_percent = server['summary']['disk_usage_percent'] if 'summary' in server else 0
 
         self.sum_cpu_usage = self.sum_cpu_usage + cpu_usage_percent
         self.sum_mem_usage = self.sum_mem_usage + mem_usage_percent
         self.sum_disk_usage = self.sum_disk_usage + disk_usage_percent
@@ -227,15 +264,11 @@
                     disk_info += ', '
 
                 if free_disk_space_percent <= float(self.config.threshold_free_diskspace):
                     disk_info += f"{bcolors.FAIL}" + "{:.0f}".format(free_disk_space_percent) + "% free on " + mount + f"{bcolors.ENDC}"
                 else:
                     disk_info += "{:.0f}".format(free_disk_space_percent) + "% free on " + mount
 
-        if (self.format == 'table'):
-            self.table.add_row([id, name, ip_address, status, os, cpu_usage_percent_text, mem_usage_percent_text, disk_usage_percent_text, disk_info, tags])
-
-        elif (self.format == 'csv'):
+        if (self.format == 'csv'):
             print(f"{id};{name};{ip_address};{status};{os};{cpu_usage_percent};{mem_usage_percent};{disk_usage_percent};{disk_info};{tags}")
-
         else:
-            print(json.dumps(server, indent=4))
+            self.table.add_row([id, name, ip_address, status, os, cpu_usage_percent_text, mem_usage_percent_text, disk_usage_percent_text, disk_info, tags])
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/sites.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/sites.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,30 +51,32 @@
             self.monitors = response.json()['monitors']
             return True
         else:
             printError('An error occurred:', response.status_code)
             self.monitors = None
             return False
 
-    def list(self, id: str = '', url: str = '', name: str = '', location: str = '', pattern: str = ''):
+    def list(self, id: str = '', url: str = '', name: str = '', location: str = '', pattern: str = '', issuesOnly: bool = False):
         """Iterate through list of web monitors and print details"""
 
         if self.fetchData():
             self.printHeader()
 
             for monitor in self.monitors:
                 if (id or url or name or location or pattern):
                     if (id and monitor['id'] == id) \
                         or (url and monitor['url'] == url) \
                         or (name and 'name' in monitor and monitor['name'] == name) \
                         or (location and location in monitor['monitor']['name']) \
                         or (pattern and pattern in monitor['url']):
-                        self.print(monitor)
+                        if (not issuesOnly) or self.hasIssue(monitor):
+                            self.print(monitor)
                 else:
-                    self.print(monitor)
+                    if (not issuesOnly) or self.hasIssue(monitor):
+                        self.print(monitor)
 
             self.printFooter()
 
     def add(self, url: str, protocol: str = 'https', name: str = '', force: bool = False):
         """Add a monitor for the given URL"""
 
         if url and self.fetchData():
@@ -163,14 +165,26 @@
                     else:
                         printError('Failed to remove site monitor', curr_url, '[', curr_id, '] with response code:', response.status_code)
                         return False
 
         if removed == 0:
             printWarn('No monitors with given pattern found: id=' + id, 'url=', url, 'name=' + name, 'location=' + location, 'pattern=' + pattern)
 
+    def hasIssue(self, monitor):
+        """Return True if the specified monitor has some issue by having a value outside of the expected threshold specified in config file"""
+
+        if float(monitor['uptime_percentage']) <= float(self.config.threshold_uptime):
+            return True
+
+        if 'last_check' in monitor and 'ttfb' in monitor['last_check']:
+            if float(monitor['last_check']['ttfb']) >= float(self.config.threshold_ttfb):
+                return True
+
+        return False
+
     def printHeader(self):
         """Print CSV header if CSV format requested"""
 
         if (self.format == 'csv'):
             print('id;url;name;code;status;status_message;uptime_percentage;ttfb;location')
 
         self.sum_uptime = 0
@@ -214,14 +228,18 @@
             print("\n".join(list_of_table_lines[:-(result_lines + 1)]))
             print(horizontal_line)
             print("\n".join(list_of_table_lines[-(result_lines + 1):]))
 
     def print(self, monitor):
         """Print the data of the specified web monitor"""
 
+        if (self.format == 'json'):
+            print(json.dumps(monitor, indent=4))
+            return
+
         id = monitor['id']
         url = monitor['url']
         name = monitor['name'] if 'name' in monitor else ''
         code = monitor['code'] if 'code' in monitor else ''
         status = monitor['status'] if 'status' in monitor else ''
         status_message = monitor['status_message'] if 'status_message' in monitor else ''
         location = monitor['monitor']['name']
@@ -231,28 +249,23 @@
             ttfb = float(monitor['last_check']['ttfb'])
             self.sum_uptime = self.sum_uptime + uptime_percentage
             self.sum_ttfb = self.sum_ttfb + ttfb
             self.num_monitors = self.num_monitors + 1
         else:
             ttfb = -1
 
-        if (self.format == 'table'):
-
+        if (self.format == 'csv'):
+            print(f"{id};{url};{name};{code};{status};{status_message};{uptime_percentage}%;{ttfb};{location}")
+        else:
             if uptime_percentage <= float(self.config.threshold_uptime):
                 uptime_percentage_text = f"{bcolors.FAIL}" + "{:.4f}".format(uptime_percentage) + f"{bcolors.ENDC}"
             else:
                 uptime_percentage_text = "{:.4f}".format(uptime_percentage)
 
             if ttfb >= float(self.config.threshold_ttfb):
                 ttfb_text = f"{bcolors.FAIL}" + "{:.2f}".format(ttfb) + f"{bcolors.ENDC}"
             elif ttfb != -1:
                 ttfb_text = "{:.2f}".format(ttfb)
             else:
                 ttfb_text = f"{bcolors.FAIL}n/a{bcolors.ENDC}"
 
             self.table.add_row([id, url, status_message, uptime_percentage_text, ttfb_text, location])
-
-        elif (self.format == 'csv'):
-            print(f"{id};{url};{name};{code};{status};{status_message};{uptime_percentage}%;{ttfb};{location}")
-
-        else:
-            print(json.dumps(monitor, indent=4))
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/statistics.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,12 +117,11 @@
 
         if (self.format == 'table'):
             print(self.table)
 
     def printAsset(self, asset: str, value):
         """Print the data of the specified web monitor"""
 
-        if (self.format == 'table'):
-            self.table.add_row([value, asset])
-
-        elif (self.format == 'csv'):
+        if (self.format == 'csv'):
             print(f"{asset};{value}")
+        else:
+            self.table.add_row([value, asset])
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/lib/usertokens.py` & `360monitoringcli-1.0.9/cli360monitoring/lib/usertokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,17 @@
         """Print table if table format requested"""
         if (self.format == 'table'):
             print(self.table)
 
     def print(self, usertoken):
         """Print the data of the specified usertoken"""
 
-        token = usertoken['token']
+        if (self.format == 'json'):
+            print(json.dumps(usertoken, indent=4))
+            return
 
-        if (self.format == 'table'):
-            self.table.add_row([token])
+        token = usertoken['token']
 
-        elif (self.format == 'csv'):
+        if (self.format == 'csv'):
             print(f"{token}")
-
         else:
-            print(json.dumps(usertoken, indent=4))
+            self.table.add_row([token])
```

### Comparing `360monitoringcli-1.0.8/cli360monitoring/monitoring.py` & `360monitoringcli-1.0.9/cli360monitoring/monitoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .lib.config import Config
 from .lib.contacts import Contacts
 from .lib.servers import Servers
 from .lib.sites import Sites
 from .lib.usertokens import UserTokens
 from .lib.statistics import Statistics
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 cfg = Config(__version__)
 cli = argparse.ArgumentParser(prog='360monitoring', description='CLI for 360 Monitoring')
 cli_subcommands = dict()
 
 def check_columns(columns):
     """Show or hide columns in ASCII table view"""
@@ -83,29 +83,29 @@
 def servers_add(args):
     """Sub command for servers add"""
     usertokens = UserTokens(cfg)
     token = usertokens.token()
     if not token:
         print('First create a user token by executing:')
         print()
-        print('360monitoring usertokens --create')
-        print('360monitoring usertokens --list')
+        print('360monitoring usertokens create')
+        print('360monitoring usertokens list')
         print()
         token = '[YOUR_USER_TOKEN]'
 
     print('Please login via SSH to each of the servers you would like to add and execute the following command:')
     print()
     print('wget -q -N monitoring.platform360.io/agent360.sh && bash agent360.sh', token)
 
 def servers_list(args):
     """Sub command for servers list"""
     check_columns(args.columns)
     servers = Servers(cfg)
     servers.format = args.output
-    servers.list(args.tag)
+    servers.list(args.issues, args.tag)
 
 def servers_remove(args):
     """Sub command for servers remove"""
     print("Please login via SSH to each of the servers you would like to remove.")
     print("First stop the monitoring agent by running \"service agent360 stop\" then run \"pip3 uninstall agent360\". After 15 minutes you are able to remove the server.")
 
 def servers_update(args):
@@ -142,15 +142,15 @@
         print('You need to specify at least a name with --name [name]')
 
 def sites_list(args):
     """Sub command for sites list"""
     check_columns(args.columns)
     sites = Sites(cfg)
     sites.format = args.output
-    sites.list(id=args.id, url=args.url, name=args.name, location=args.location, pattern=args.pattern)
+    sites.list(id=args.id, url=args.url, name=args.name, location=args.location, pattern=args.pattern, issuesOnly=args.issues)
 
 def sites_remove(args):
     """Sub command for sites remove"""
     sites = Sites(cfg)
     sites.remove(id=args.id, url=args.url, name=args.name, location=args.location, pattern=args.pattern)
 
 def sites(args):
@@ -245,14 +245,15 @@
     cli_servers_add.set_defaults(func=servers_add)
 
     cli_servers_list = cli_servers_subparsers.add_parser('list', help='list monitored servers')
     cli_servers_list.set_defaults(func=servers_list)
     cli_servers_list.add_argument('--id', nargs='?', default='', metavar='id', help='update server with given ID')
     cli_servers_list.add_argument('--name', nargs='?', default='', metavar='name', help='update server with given name')
     cli_servers_list.add_argument('--tag', nargs='*', default='', metavar='tag', help='only list servers matching these tags')
+    cli_servers_list.add_argument('--issues', action='store_true', help='show only servers with issues')
 
     cli_servers_list.add_argument('--output', choices=['json', 'csv', 'table'], default='table', help='output format for the data')
     cli_servers_list.add_argument('--json', action='store_const', const='json', dest='output', help='print data in JSON format')
     cli_servers_list.add_argument('--csv', action='store_const', const='csv', dest='output', help='print data in CSV format')
     cli_servers_list.add_argument('--table', action='store_const', const='table', dest='output', help='print data as ASCII table')
     cli_servers_list.add_argument('--columns', nargs='*', default='', metavar='columns', help='Specify columns to print in table view or remove columns with 0 as prefix e.g. "0id"')
 
@@ -283,14 +284,15 @@
     cli_sites_list = cli_sites_subparsers.add_parser('list', help='list sites')
     cli_sites_list.set_defaults(func=sites_list)
     cli_sites_list.add_argument('--id', nargs='?', default='', metavar='id', help='list site with given ID')
     cli_sites_list.add_argument('--url', nargs='?', default='', metavar='url', help='list site with given url')
     cli_sites_list.add_argument('--name', nargs='?', default='', metavar='name', help='list site with given name')
     cli_sites_list.add_argument('--location', nargs='?', default='', metavar='location', help='list sites monitored from given location')
     cli_sites_list.add_argument('--pattern', nargs='?', default='', metavar='pattern', help='list sites with pattern included in URL')
+    cli_sites_list.add_argument('--issues', action='store_true', help='show only sites with issues')
 
     cli_sites_list.add_argument('--output', choices=['json', 'csv', 'table'], default='table', help='output format for the data')
     cli_sites_list.add_argument('--json', action='store_const', const='json', dest='output', help='print data in JSON format')
     cli_sites_list.add_argument('--csv', action='store_const', const='csv', dest='output', help='print data in CSV format')
     cli_sites_list.add_argument('--table', action='store_const', const='table', dest='output', help='print data as ASCII table')
     cli_sites_list.add_argument('--columns', nargs='*', default='', metavar='columns', help='Specify columns to print in table view or remove columns with 0 as prefix e.g. "0id"')
```

### Comparing `360monitoringcli-1.0.8/setup.py` & `360monitoringcli-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 readme = open(os.path.join(here, 'README.md')).read()
 install_requires = ['configparser', 'prettytable', 'requests']
 
 setuptools.setup(
     name='360monitoringcli',
-    version='1.0.8',
+    version='1.0.9',
     description='360 Monitoring CLI',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/plesk/360monitoring-cli',
     author='Jan Loeffler',
     author_email='jan.loeffler@webpros.com',
     maintainer='Jan Loeffler',
```

