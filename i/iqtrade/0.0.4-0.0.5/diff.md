# Comparing `tmp/iqtrade-0.0.4-py3-none-any.whl.zip` & `tmp/iqtrade-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12103 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 21-Aug-27 01:02 iqtrade/__init__.py
--rw-r--r--  2.0 unx    52703 b- defN 21-Aug-27 01:02 iqtrade/api.py
--rw-rw-rw-  2.0 unx     1067 b- defN 21-Aug-27 06:16 iqtrade-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1141 b- defN 21-Aug-27 06:16 iqtrade-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Aug-27 06:16 iqtrade-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 21-Aug-27 06:16 iqtrade-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 21-Aug-27 06:16 iqtrade-0.0.4.dist-info/RECORD
-7 files, 55541 bytes uncompressed, 11165 bytes compressed:  79.9%
+Zip file size: 12142 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 20:32 iqtrade/__init__.py
+-rw-r--r--  2.0 unx    52937 b- defN 23-Apr-08 20:01 iqtrade/api.py
+-rw-rw-rw-  2.0 unx     1067 b- defN 23-Apr-08 20:32 iqtrade-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1104 b- defN 23-Apr-08 20:32 iqtrade-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 20:32 iqtrade-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 20:32 iqtrade-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 23-Apr-08 20:32 iqtrade-0.0.5.dist-info/RECORD
+7 files, 55738 bytes uncompressed, 11204 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: iqtrade/__init__.py
 Comment: 
 
 Filename: iqtrade/api.py
 Comment: 
 
-Filename: iqtrade-0.0.4.dist-info/LICENSE
+Filename: iqtrade-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: iqtrade-0.0.4.dist-info/METADATA
+Filename: iqtrade-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: iqtrade-0.0.4.dist-info/WHEEL
+Filename: iqtrade-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: iqtrade-0.0.4.dist-info/top_level.txt
+Filename: iqtrade-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: iqtrade-0.0.4.dist-info/RECORD
+Filename: iqtrade-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqtrade/api.py

```diff
@@ -58,38 +58,39 @@
     SoleProprietorship = 7
     Family = 8
     JointAndInformalTrust = 9
     Institution = 10
 
     @staticmethod
     def from_string(account_type: str) -> ClientAccountType:
-        if account_type == "Individual":
+        account_type = account_type.replace(" ", "").lower()
+        if account_type == "individual":
             return ClientAccountType.Individual
-        elif account_type == "Joint":
+        elif account_type == "joint":
             return ClientAccountType.Joint
-        elif account_type == "Informal Trust":
+        elif account_type == "informaltrust":
             return ClientAccountType.InformalTrust
-        elif account_type == "Corporation":
+        elif account_type == "corporation":
             return ClientAccountType.Corporation
-        elif account_type == "Investment Club":
+        elif account_type == "investmentclub":
             return ClientAccountType.InvestmentClub
-        elif account_type == "Formal Trust":
+        elif account_type == "formaltrust":
             return ClientAccountType.FormalTrust
-        elif account_type == "Partnership":
+        elif account_type == "partnership":
             return ClientAccountType.Partnership
-        elif account_type == "Sole Proprietorship":
+        elif account_type == "soleproprietorship":
             return ClientAccountType.SoleProprietorship
-        elif account_type == "Family":
+        elif account_type == "family":
             return ClientAccountType.Family
-        elif account_type == "Joint and Informal Trust":
+        elif account_type == "jointandinformaltrust":
             return ClientAccountType.JointAndInformalTrust
-        elif account_type == "Institution":
+        elif account_type == "institution":
             return ClientAccountType.Institution
         else:
-            raise ValueError("account_type")
+            raise ValueError('Unknown account_type "' + account_type + '"')  # pragma: no cover
 
 
 class TickType(Enum):
     Up = 0
     Down = 1
     Equal = 2
 
@@ -261,15 +262,15 @@
 
     def get_account_number(account_id: Union[str, AccountInfo]) -> str:
         if isinstance(account_id, str):
             return account_id
         elif isinstance(account_id, AccountInfo):
             return account_id.number
         else:
-            raise TypeError("Invalid type for 'account_id'")
+            raise TypeError("Invalid type for 'account_id'")  # pragma: no cover
 
 
 class AccountActivity:
     def __init__(self, iq_data: dict[str, Any]):
         self.trade_date: dt = dt.fromisoformat(iq_data["tradeDate"])
         self.transaction_date: dt = dt.fromisoformat(iq_data["transactionDate"])
         self.settlement_date: dt = dt.fromisoformat(iq_data["settlementDate"])
@@ -282,15 +283,15 @@
         self.price: float = iq_data["price"]
         self.gross_amount: float = iq_data["grossAmount"]
         self.commission: float = iq_data["commission"]
         self.net_amount: float = iq_data["netAmount"]
         self.activity_type: str = iq_data["type"]
 
     def __str__(self) -> str:  # pragma: no cover
-        return (
+        return str(
             self.activity_type
             + " "
             + self.action
             + " "
             + f"{self.quantity:.2f}"
             + " "
             + self.ticker
@@ -439,15 +440,15 @@
         self.industry_sector: str = iq_data["industrySector"]
         self.industry_group: str = iq_data["industryGroup"]
         self.industry_subgroup: str = iq_data["industrySubgroup"]
 
     def get_display_name(self) -> str:  # pragma: no cover
         if isinstance(self.option_expiry_date, dt):
             if self.option_root:
-                return (
+                return str(
                     self.option_root
                     + " "
                     + self.option_expiry_date.strftime("%d %b %Y")
                     + " "
                     + f"{self.option_strike_price:.2f}"
                     + " "
                     + self.option_type.name
@@ -549,15 +550,15 @@
             price = f"{self.limit_price:,.2f}% TrlLimit {self.stop_price:,.2f}% TrlStop"
         elif self.order_type == OrderType.TrailStopLimitInDollar:
             price = f"{self.limit_price:,.2f} TrlLimit {self.stop_price:,.2f} TrlStop"
         elif self.order_type == OrderType.LimitOnOpen:
             price = f"{self.limit_price:,.2f} LimitOnOpen"
         elif self.order_type == OrderType.LimitOnClose:
             price = f"{self.limit_price:,.2f} LimitOnClose"
-        return (
+        return str(
             self.side.name
             + " "
             + str(self.total_quantity)
             + " "
             + self.ticker
             + " "
             + self.strategy_type.name
@@ -822,24 +823,24 @@
         self.volume: int = iq_data["volume"]
         self.vwap: Optional[int] = None
         if "VWAP" in iq_data:
             self.vwap = iq_data["VWAP"]
 
 
 class QuestradeIQ:
-    def __init__(self, config: Union[str, dict[str, Any]] = "secrets.json", safe_config: bool = True):
+    def __init__(self, config: Union[str, dict[str, Any]] = "secrets.json", save_config: bool = True):
         """Constructor
 
         Parameters
         ----------
         config : Union[str, dict], optional
             Config filename or dictionary.
                 If a dict, key/value pairs for configuration, by default "secrets.json"
         """
-        self._should_save_config = safe_config
+        self._should_save_config = save_config
         if isinstance(config, str):
             self._config_filename = config
             with open(self._config_filename, "r") as infile:
                 self._config = json.load(infile)
         elif isinstance(config, dict):
             self._config_filename = ""
             self._config = config.copy()  # make a copy here to not modify the caller's dict
@@ -865,15 +866,15 @@
 
     def get_access_token_type(self) -> str:
         return self._token_type
 
     def get_api_url(self) -> urllib.parse.ParseResult:
         if self._api_url is not None:
             return self._api_url
-        raise AttributeError("'api_url' is None")
+        raise AttributeError("'api_url' is None")  # pragma: no cover
 
     def _save_config(self) -> None:
         assert "iq_refresh_token" in self._config
         if self._config_filename != "" and self._should_save_config:
             with open(self._config_filename, "w") as outfile:
                 json.dump(self._config, outfile, indent=4)
 
@@ -1053,15 +1054,15 @@
             query["startTime"] = start_time.isoformat()
         if end_time is not None:
             if not isinstance(end_time, dt):
                 raise TypeError("Type of 'end_time' must be datetime")
             query["endTime"] = end_time.isoformat()
         if state_filter:
             if not isinstance(state_filter, OrderStateFilter):
-                raise TypeError("Type of 'state_filter' must be OrderStateFilter")
+                raise TypeError("Type of 'state_filter' must be OrderStateFilter")  # pragma: no cover
             query["stateFilter"] = state_filter.name
         response = self._make_request(f"accounts/{AccountInfo.get_account_number(account_id)}/orders", params=query)
         if "orders" not in response:
             raise RuntimeError("Invalid respose received")
         return [Order(order) for order in response["orders"]]
 
     def get_order(self, account_id: Union[str, AccountInfo], orderId: Union[str, int]) -> list[Order]:
@@ -1362,15 +1363,15 @@
         query = {
             "startTime": start_time.isoformat(),
             "endTime": end_time.isoformat(),
             "interval": interval.name,
         }
         response = self._make_request(f"markets/candles/{id}", params=query)
         if "candles" not in response:
-            raise RuntimeError("Invalid respose received")
+            raise RuntimeError("Invalid respose received")  # pragma: no cover
         return response["candles"] if raw_data else [Candle(candle) for candle in response["candles"]]
 
     def setup_streaming_notifications(self, socket_mode: SocketMode) -> int:
         """Retrieves the port number used for notification streaming.
 
         Args:
             socket_mode: Either RawSocket or WebSocket.
@@ -1380,15 +1381,15 @@
 
         See Also:
             https://www.questrade.com/api/documentation/streaming
         """
         query = {"mode": socket_mode.name}
         response = self._make_request("notifications", params=query)
         if "streamPort" not in response:
-            raise RuntimeError("Invalid respose received")
+            raise RuntimeError("Invalid respose received")  # pragma: no cover
         return int(response["streamPort"])
 
     def setup_streaming_quotes(self, ids: list[int], socket_mode: SocketMode) -> int:
         """Retrieves the port number used for L1 quote streaming.
 
         Args:
             ids: List of symbol ids to stream.
@@ -1399,9 +1400,9 @@
 
         See Also:
             https://www.questrade.com/api/documentation/streaming
         """
         query = {"ids": ",".join([str(id) for id in ids]), "stream": "true", "mode": socket_mode.name}
         response = self._make_request("markets/quotes", params=query)
         if "streamPort" not in response:
-            raise RuntimeError("Invalid respose received")
+            raise RuntimeError("Invalid respose received")  # pragma: no cover
         return int(response["streamPort"])
```

## Comparing `iqtrade-0.0.4.dist-info/LICENSE` & `iqtrade-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iqtrade-0.0.4.dist-info/METADATA` & `iqtrade-0.0.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: iqtrade
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper around Questrade IQ API
 Home-page: https://github.com/jpflouret/iqtrade
 Author: JP Flouret
 Author-email: jpflouret@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 [![Build Status](https://travis-ci.com/jpflouret/iqtrade.svg?branch=main)](https://travis-ci.com/jpflouret/iqtrade)
 [![PyPI](https://img.shields.io/pypi/v/iqtrade)](https://pypi.org/project/iqtrade/)
@@ -28,9 +26,7 @@
 pip install iqtrade
 ```
 
 ## Disclaimer
 
 This project is not affiliated with Questrade Wealth Management Inc., Questrade,
 Inc., or any members of the Questrade Group of Companies or its affiliates.
-
-
```

