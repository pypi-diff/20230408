# Comparing `tmp/binance_data_exporter-0.2.2.tar.gz` & `tmp/binance_data_exporter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_data_exporter-0.2.2.tar", last modified: Sat Apr  8 14:41:15 2023, max compression
+gzip compressed data, was "binance_data_exporter-0.2.3.tar", last modified: Sat Apr  8 16:09:52 2023, max compression
```

## Comparing `binance_data_exporter-0.2.2.tar` & `binance_data_exporter-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:41:15.029141 binance_data_exporter-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-08 14:41:15.029141 binance_data_exporter-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-08 14:41:04.000000 binance_data_exporter-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:41:15.029141 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-08 14:41:14.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-08 14:41:15.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:41:14.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 14:41:14.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-08 14:41:14.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:41:14.000000 binance_data_exporter-0.2.2/binance_data_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:41:15.029141 binance_data_exporter-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-08 14:41:13.000000 binance_data_exporter-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.189442 binance_data_exporter-0.2.3/
+-rw-rw-rw-   0        0        0       32 2023-04-08 16:07:11.000000 binance_data_exporter-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:09:52.188459 binance_data_exporter-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4308 2023-04-08 14:33:42.000000 binance_data_exporter-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.104440 binance_data_exporter-0.2.3/binance_data_exporter/
+-rw-rw-rw-   0        0        0        0 2023-04-08 16:08:49.000000 binance_data_exporter-0.2.3/binance_data_exporter/__init__.py
+-rw-rw-rw-   0        0        0     9242 2023-04-08 14:37:53.000000 binance_data_exporter-0.2.3/binance_data_exporter/binance_data_exporter.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.181452 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-08 16:09:52.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 16:09:52.189442 binance_data_exporter-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-08 16:09:38.000000 binance_data_exporter-0.2.3/setup.py
```

### Comparing `binance_data_exporter-0.2.2/PKG-INFO` & `binance_data_exporter-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-Metadata-Version: 2.1
-Name: binance_data_exporter
-Version: 0.2.2
-Summary: A tool for exporting in JSON the historical data of a symbol from Binance
-Author: zestones
-Author-email: idrissbenguezzou@gmail.com
-Description-Content-Type: text/markdown
-
-# Binance API Data Exporter
-
-This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
-
-## Installation
-
-1. Install it via pip by running the following command in your terminal:
-````bash
-pip install binance-data-exporter
-````
-2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
-
-3. Clone the project repository from GitHub by running the following command in your terminal:
-````bash
-git clone git@github.com:zestones/Binance-Data-Exporter.git
-````
-
-## Usage
-
-To run the script, use the following command:
-
-````bash
-python binance_data_exporter.py [OPTIONS]
-````
-
-Bellow the list of available options you can use to customize the request to the Binance API:
-
-| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
-|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
-| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
-| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
-| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
-| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
-| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
-| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
-| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
-
-
-> **NOTE** 
-> 
-> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
-> - If the end-time is not specified the date of the day will be choosed by default.
-> - If you dont provide parameters, the script will use the default values specified.
-### Examples
-
-To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
-
-````bash
-python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
-````
-
-You can customize the parameters to retrieve data as you wish.
-
-
-## Dependencies
-
-The script requires the following dependencies:
-
-- requests
-- colorama
-- tabulate
-
-You can install the dependencies using the following command:
-
-````bash
-pip install -r requirements.txt
-````	
-
-
-## Output
-
-The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
-
-where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
-
-## API Limits and Maximum Number of Requests
-
-Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
-
-It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
-
-## Binance API Documentation
-For more information on the Binance API, you can refer to the official documentation at:
-
-https://binance-docs.github.io/apidocs/spot/en/
+Metadata-Version: 2.1
+Name: binance_data_exporter
+Version: 0.2.3
+Summary: A tool for exporting in JSON the historical data of a symbol from Binance
+Author: zestones
+Author-email: idrissbenguezzou@gmail.com
+Description-Content-Type: text/markdown
+
+# Binance API Data Exporter
+
+This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
+
+## Installation
+
+1. Install it via pip by running the following command in your terminal:
+````bash
+pip install binance-data-exporter
+````
+2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
+
+3. Clone the project repository from GitHub by running the following command in your terminal:
+````bash
+git clone git@github.com:zestones/Binance-Data-Exporter.git
+````
+
+## Usage
+
+To run the script, use the following command:
+
+````bash
+python binance_data_exporter.py [OPTIONS]
+````
+
+Bellow the list of available options you can use to customize the request to the Binance API:
+
+| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
+|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
+| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
+| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
+| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
+| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
+| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
+| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
+| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
+
+
+> **NOTE** 
+> 
+> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
+> - If the end-time is not specified the date of the day will be choosed by default.
+> - If you dont provide parameters, the script will use the default values specified.
+### Examples
+
+To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
+
+````bash
+python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
+````
+
+You can customize the parameters to retrieve data as you wish.
+
+
+## Dependencies
+
+The script requires the following dependencies:
+
+- requests
+- colorama
+- tabulate
+
+You can install the dependencies using the following command:
+
+````bash
+pip install -r requirements.txt
+````	
+
+
+## Output
+
+The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
+
+where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
+
+## API Limits and Maximum Number of Requests
+
+Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
+
+It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
+
+## Binance API Documentation
+For more information on the Binance API, you can refer to the official documentation at:
+
+https://binance-docs.github.io/apidocs/spot/en/
```

### Comparing `binance_data_exporter-0.2.2/README.md` & `binance_data_exporter-0.2.3/binance_data_exporter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,93 @@
-# Binance API Data Exporter
-
-This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
-
-## Installation
-
-1. Install it via pip by running the following command in your terminal:
-````bash
-pip install binance-data-exporter
-````
-2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
-
-3. Clone the project repository from GitHub by running the following command in your terminal:
-````bash
-git clone git@github.com:zestones/Binance-Data-Exporter.git
-````
-
-## Usage
-
-To run the script, use the following command:
-
-````bash
-python binance_data_exporter.py [OPTIONS]
-````
-
-Bellow the list of available options you can use to customize the request to the Binance API:
-
-| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
-|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
-| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
-| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
-| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
-| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
-| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
-| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
-| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
-
-
-> **NOTE** 
-> 
-> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
-> - If the end-time is not specified the date of the day will be choosed by default.
-> - If you dont provide parameters, the script will use the default values specified.
-### Examples
-
-To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
-
-````bash
-python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
-````
-
-You can customize the parameters to retrieve data as you wish.
-
-
-## Dependencies
-
-The script requires the following dependencies:
-
-- requests
-- colorama
-- tabulate
-
-You can install the dependencies using the following command:
-
-````bash
-pip install -r requirements.txt
-````	
-
-
-## Output
-
-The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
-
-where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
-
-## API Limits and Maximum Number of Requests
-
-Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
-
-It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
-
-## Binance API Documentation
-For more information on the Binance API, you can refer to the official documentation at:
-
-https://binance-docs.github.io/apidocs/spot/en/
+Metadata-Version: 2.1
+Name: binance-data-exporter
+Version: 0.2.3
+Summary: A tool for exporting in JSON the historical data of a symbol from Binance
+Author: zestones
+Author-email: idrissbenguezzou@gmail.com
+Description-Content-Type: text/markdown
+
+# Binance API Data Exporter
+
+This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
+
+## Installation
+
+1. Install it via pip by running the following command in your terminal:
+````bash
+pip install binance-data-exporter
+````
+2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
+
+3. Clone the project repository from GitHub by running the following command in your terminal:
+````bash
+git clone git@github.com:zestones/Binance-Data-Exporter.git
+````
+
+## Usage
+
+To run the script, use the following command:
+
+````bash
+python binance_data_exporter.py [OPTIONS]
+````
+
+Bellow the list of available options you can use to customize the request to the Binance API:
+
+| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
+|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
+| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
+| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
+| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
+| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
+| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
+| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
+| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
+
+
+> **NOTE** 
+> 
+> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
+> - If the end-time is not specified the date of the day will be choosed by default.
+> - If you dont provide parameters, the script will use the default values specified.
+### Examples
+
+To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
+
+````bash
+python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
+````
+
+You can customize the parameters to retrieve data as you wish.
+
+
+## Dependencies
+
+The script requires the following dependencies:
+
+- requests
+- colorama
+- tabulate
+
+You can install the dependencies using the following command:
+
+````bash
+pip install -r requirements.txt
+````	
+
+
+## Output
+
+The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
+
+where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
+
+## API Limits and Maximum Number of Requests
+
+Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
+
+It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
+
+## Binance API Documentation
+For more information on the Binance API, you can refer to the official documentation at:
+
+https://binance-docs.github.io/apidocs/spot/en/
```

### Comparing `binance_data_exporter-0.2.2/binance_data_exporter.egg-info/PKG-INFO` & `binance_data_exporter-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,85 @@
-Metadata-Version: 2.1
-Name: binance-data-exporter
-Version: 0.2.2
-Summary: A tool for exporting in JSON the historical data of a symbol from Binance
-Author: zestones
-Author-email: idrissbenguezzou@gmail.com
-Description-Content-Type: text/markdown
-
-# Binance API Data Exporter
-
-This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
-
-## Installation
-
-1. Install it via pip by running the following command in your terminal:
-````bash
-pip install binance-data-exporter
-````
-2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
-
-3. Clone the project repository from GitHub by running the following command in your terminal:
-````bash
-git clone git@github.com:zestones/Binance-Data-Exporter.git
-````
-
-## Usage
-
-To run the script, use the following command:
-
-````bash
-python binance_data_exporter.py [OPTIONS]
-````
-
-Bellow the list of available options you can use to customize the request to the Binance API:
-
-| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
-|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
-| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
-| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
-| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
-| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
-| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
-| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
-| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
-
-
-> **NOTE** 
-> 
-> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
-> - If the end-time is not specified the date of the day will be choosed by default.
-> - If you dont provide parameters, the script will use the default values specified.
-### Examples
-
-To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
-
-````bash
-python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
-````
-
-You can customize the parameters to retrieve data as you wish.
-
-
-## Dependencies
-
-The script requires the following dependencies:
-
-- requests
-- colorama
-- tabulate
-
-You can install the dependencies using the following command:
-
-````bash
-pip install -r requirements.txt
-````	
-
-
-## Output
-
-The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
-
-where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
-
-## API Limits and Maximum Number of Requests
-
-Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
-
-It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
-
-## Binance API Documentation
-For more information on the Binance API, you can refer to the official documentation at:
-
-https://binance-docs.github.io/apidocs/spot/en/
+# Binance API Data Exporter
+
+This Python script allows you to retrieve historical data from Binance API and export it to a JSON file. The data can be retrieved for any specified symbol (e.g. BTCUSDT) and interval (e.g. 1m, 1h, 1d) for a given period of time.
+
+## Installation
+
+1. Install it via pip by running the following command in your terminal:
+````bash
+pip install binance-data-exporter
+````
+2. Check out the project on PyPI at https://pypi.org/project/binance-data-exporter/.
+
+3. Clone the project repository from GitHub by running the following command in your terminal:
+````bash
+git clone git@github.com:zestones/Binance-Data-Exporter.git
+````
+
+## Usage
+
+To run the script, use the following command:
+
+````bash
+python binance_data_exporter.py [OPTIONS]
+````
+
+Bellow the list of available options you can use to customize the request to the Binance API:
+
+| **Option**          | **Description**                   | **Possible Values**               | **Default Value** 	|
+|-------------------	|----------------------------------	|---------------------------------	|:-----------------:	|
+| `-h`,<br> `--help`          	| Show the help message and exit  	|                          	|                   	|	
+| `-i`,<br> `--interval`      	| The interval of the data                                                 	| 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h, 1d, 3d, 1w, 1M 	|        `1d`       	|
+| `-p`,<br> `--pair`          	| The pair of coin (refer to the binance symbol list)                      	| BTCUSDT, ETHUSDT, etc                                         	|     `BTCUSDT`     	|
+| `-l`,<br> `--limit`         	| The limit of the data per request  	| 1, 2, ..., 1000 (Should be integer)                           	|       `500`       	|
+| `-s`,<br> `--start-time`    	| The start time of the data                                               	| YYYY_MM_DD                                                    	|        None       	|
+| `-e`,<br> `--end-time`      	| The end time of the data                                                 	| YYYY_MM_DD                                                    	|      `TODAY`      	|
+| `-o`,<br> `--output-folder` 	| The folder where the data will be exported                               	| Path                                                          	|      `./data`     	|
+
+
+> **NOTE** 
+> 
+> - If you don't specify a start time for your request, it will use the earliest available data for the requested time interval.
+> - If the end-time is not specified the date of the day will be choosed by default.
+> - If you dont provide parameters, the script will use the default values specified.
+### Examples
+
+To retrieve data for ETHUSDT from 2018-01-15 to 2018-01-16 with an interval of 1 hour, a limit of 10, and export the data to `./data/eth_usdt/`, use the following command:
+
+````bash
+python binance_data_exporter.py -l 10 -i 1h -p ETHUSDT -s 2018_01_15 -e 2018_01_16 -o ./data/eth_usdt/
+````
+
+You can customize the parameters to retrieve data as you wish.
+
+
+## Dependencies
+
+The script requires the following dependencies:
+
+- requests
+- colorama
+- tabulate
+
+You can install the dependencies using the following command:
+
+````bash
+pip install -r requirements.txt
+````	
+
+
+## Output
+
+The script exports the retrieved data as a JSON file in the `OUTPUT_FOLDER` specified in the configuration. The filename of the JSON file is in the following format: **symbol**\_**start-date**\_to\_**end-date**\_**interval**.json
+
+where `start_date` and `end_date` are the start and end dates of the data retrieved, respectively and ``interval`` is the interval between each data point.
+
+## API Limits and Maximum Number of Requests
+
+Please note that Binance API has certain limits on the number of requests that can be made within a specific time frame. 
+
+It is important to be mindful of these limits when making requests to avoid being disconnected or banned. Make sure to not exceed the number of requests allowed by the API, when configuring the `limit` and `interval` parameters in the script.
+
+## Binance API Documentation
+For more information on the Binance API, you can refer to the official documentation at:
+
+https://binance-docs.github.io/apidocs/spot/en/
```

