# Comparing `tmp/bittrade_binance_websocket-0.1.3.tar.gz` & `tmp/bittrade_binance_websocket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_binance_websocket-0.1.3.tar", max compression
+gzip compressed data, was "bittrade_binance_websocket-0.1.4.tar", max compression
```

## Comparing `bittrade_binance_websocket-0.1.3.tar` & `bittrade_binance_websocket-0.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     4374 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/README.md
--rw-r--r--   0        0        0       23 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/__init__.py
--rw-r--r--   0        0        0      169 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/__init__.py
--rw-r--r--   0        0        0     1349 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/book_ticker.py
--rw-r--r--   0        0        0     1310 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/depth.py
--rw-r--r--   0        0        0      238 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/message.py
--rw-r--r--   0        0        0      437 2023-03-24 23:50:23.045002 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     2150 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/subscribe.py
--rw-r--r--   0        0        0      387 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/__init__.py
--rw-r--r--   0        0        0      984 2023-03-24 23:35:26.931887 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0     3531 2023-03-25 04:52:58.088547 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/generic.py
--rw-r--r--   0        0        0     2622 2023-04-03 09:03:45.595389 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/http.py
--rw-r--r--   0        0        0     1020 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/private.py
--rw-r--r--   0        0        0     2843 2023-03-25 04:14:51.250991 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/private_user_stream.py
--rw-r--r--   0        0        0      866 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/public_stream.py
--rw-r--r--   0        0        0     3556 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/reconnect.py
--rw-r--r--   0        0        0        0 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/__init__.py
--rw-r--r--   0        0        0     3411 2023-04-04 09:07:47.233373 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/add_order.py
--rw-r--r--   0        0        0     4603 2023-04-04 09:07:47.233373 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/cancel_order.py
--rw-r--r--   0        0        0     1222 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/ping.py
--rw-r--r--   0        0        0     1955 2023-03-26 02:56:38.197385 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/request_response.py
--rw-r--r--   0        0        0     1160 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/time.py
--rw-r--r--   0        0        0      109 2023-03-24 08:39:47.489037 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/framework/__init__.py
--rw-r--r--   0        0        0     7382 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/framework/framework.py
--rw-r--r--   0        0        0        0 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      628 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/json.py
--rw-r--r--   0        0        0      710 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/listen.py
--rw-r--r--   0        0        0      500 2023-03-24 23:27:41.885480 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/__init__.py
--rw-r--r--   0        0        0      200 2023-03-26 05:50:49.880376 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/accounts.py
--rw-r--r--   0        0        0       76 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/contingency_type.py
--rw-r--r--   0        0        0      705 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/endpoints.py
--rw-r--r--   0        0        0     1351 2023-03-26 02:22:12.004073 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0     3353 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/framework.py
--rw-r--r--   0        0        0      430 2023-03-24 23:31:12.793597 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/message.py
--rw-r--r--   0        0        0      404 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/oco_list_status.py
--rw-r--r--   0        0        0     5416 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/order.py
--rw-r--r--   0        0        0      951 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/order_status.py
--rw-r--r--   0        0        0      316 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/permission.py
--rw-r--r--   0        0        0      170 2023-04-04 09:07:47.233373 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/private.py
--rw-r--r--   0        0        0      441 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/request.py
--rw-r--r--   0        0        0      280 2023-03-29 01:15:49.390328 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/response_message.py
--rw-r--r--   0        0        0       15 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0       85 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/get_time.py
--rw-r--r--   0        0        0       91 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/listen_key.py
--rw-r--r--   0        0        0      595 2023-03-29 01:15:49.390328 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/margin_account.py
--rw-r--r--   0        0        0       98 2023-03-25 08:43:55.036423 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0      254 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/symbol_status.py
--rw-r--r--   0        0        0       14 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/operators/__init__.py
--rw-r--r--   0        0        0      721 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/operators/orderbook/__init__.py
--rw-r--r--   0        0        0      696 2023-03-24 23:50:03.044230 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/operators/stream/response_messages.py
--rw-r--r--   0        0        0        0 2023-03-24 01:54:38.772479 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/__init__.py
--rw-r--r--   0        0        0      642 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/cancel_order.py
--rw-r--r--   0        0        0      639 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/create_order.py
--rw-r--r--   0        0        0      724 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/current_open_orders.py
--rw-r--r--   0        0        0      533 2023-03-26 06:02:52.776601 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/get_time.py
--rw-r--r--   0        0        0     1167 2023-03-26 06:02:58.536601 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/http_factory_decorator.py
--rw-r--r--   0        0        0     2485 2023-03-26 06:10:58.443293 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/listen_key.py
--rw-r--r--   0        0        0      680 2023-03-29 01:15:49.390328 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/query_margin_account.py
--rw-r--r--   0        0        0      718 2023-03-29 01:15:49.390328 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/query_margin_fee_data.py
--rw-r--r--   0        0        0     1241 2023-04-03 06:54:20.052428 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/symbol_orders_cancel.py
--rw-r--r--   0        0        0      669 2023-03-25 08:43:32.174867 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0     3824 2023-03-29 01:24:13.423136 bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/sign.py
--rw-r--r--   0        0        0     1760 2023-04-05 05:52:59.030067 bittrade_binance_websocket-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.3/setup.py
--rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.1.4/README.md
+-rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/__init__.py
+-rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/__init__.py
+-rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/book_ticker.py
+-rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/depth.py
+-rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/message.py
+-rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/__init__.py
+-rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0     3531 2023-03-26 22:59:27.837091 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2622 2023-03-26 22:59:27.837264 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/http.py
+-rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/private.py
+-rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/private_user_stream.py
+-rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/public_stream.py
+-rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/__init__.py
+-rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/add_order.py
+-rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/cancel_order.py
+-rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/ping.py
+-rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/request_response.py
+-rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/time.py
+-rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/framework/__init__.py
+-rw-r--r--   0        0        0     7382 2023-04-01 05:20:35.503250 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/framework/framework.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/json.py
+-rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/listen.py
+-rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/accounts.py
+-rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/contingency_type.py
+-rw-r--r--   0        0        0      705 2023-04-01 05:21:43.540430 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/endpoints.py
+-rw-r--r--   0        0        0     1351 2023-03-26 22:59:27.838662 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0     3353 2023-04-01 05:14:48.687793 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/framework.py
+-rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/message.py
+-rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/oco_list_status.py
+-rw-r--r--   0        0        0     5878 2023-04-08 09:51:07.675078 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/order.py
+-rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/order_status.py
+-rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/permission.py
+-rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/private.py
+-rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/request.py
+-rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/response_message.py
+-rw-r--r--   0        0        0       15 2023-03-07 05:38:31.457289 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/get_time.py
+-rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/listen_key.py
+-rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/margin_account.py
+-rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/symbol_status.py
+-rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/operators/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/operators/orderbook/__init__.py
+-rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/operators/stream/response_messages.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-01 04:56:33.596498 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/cancel_order.py
+-rw-r--r--   0        0        0      639 2023-04-01 04:56:55.000215 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/create_order.py
+-rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/current_open_orders.py
+-rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/get_time.py
+-rw-r--r--   0        0        0     1167 2023-03-24 09:56:30.849712 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/http_factory_decorator.py
+-rw-r--r--   0        0        0     2485 2023-03-26 22:59:27.840684 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/listen_key.py
+-rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/query_margin_account.py
+-rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/query_margin_fee_data.py
+-rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/symbol_orders_cancel.py
+-rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0     3824 2023-03-30 09:47:19.704651 bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/sign.py
+-rw-r--r--   0        0        0     1761 2023-04-08 20:13:14.080328 bittrade_binance_websocket-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.4/setup.py
+-rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.4/PKG-INFO
```

### Comparing `bittrade_binance_websocket-0.1.3/README.md` & `bittrade_binance_websocket-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-# Binance Websocket
-
-[NOT RELEASED] This is very much a work in progress, despite being on pypi.
-Most things might be wrongly documented; API **will** change
-
-## Features
-
-- Reconnect with incremental backoff 
-- Respond to ping
-- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API
-- ... but provides more info than a simple request/response; 
-  for instance, `add_order` goes through each stage submitted->pending->open or canceled, 
-  emitting a notification at each stage
-
-## Installing
-
-`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`
-
-## General considerations
-
-### Observables/Reactivex
-
-The whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).
-
-Though Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.
-
-For simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below
-
-### Concurrency
-
-Internally the library uses threads.
-For your main program you don't have to worry about threads; you can block the main thread.
-
-## Getting started
-
-### Connect to the public feeds
-
-```python
-from bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker
-from bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only
-
-# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method
-socket_connection = public_websocket_connection()
-# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…
-messages = socket_connection.pipe(
-    keep_messages_only(),
-)
-socket_connection.pipe(
-    filter_new_socket_only(),
-    subscribe_ticker('USDT/USD', messages)
-).subscribe(
-    print, print, print  # you can do anything with the messages; here we simply print them out
-)
-socket_connection.connect()
-```
-
-_(This script is complete, it should run "as is")_
-
-
-## Logging
-
-We use Python's standard logging.
-You can modify what logs you see as follows:
-
-```
-logging.getLogger('bittrade_huobi_websocket').addHandler(logging.StreamHandler())
-```
-
-In addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`
-
-To view a full, timestamped history of the socket exchanges use
-
-```
-handler = FileHandler("logs/raw_socket.log")
-handler.setLevel(DEBUG)
-logger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")
-formatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")
-handler.setFormatter(formatter)
-logger.addHandler(handler)
-handler = FileHandler("logs/raw_socket.log")
-handler.setLevel(DEBUG)
-logger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")
-formatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")
-handler.setFormatter(formatter)
-logger.addHandler(handler)
-```
-
-## Private feeds
-
-Similar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.
-
-This means that you'll need to implement the signature token yourself. The library never has access to your API secret.
-
-See `examples/sign.py` for an example of implementation but it is generally as simple as:
-
-```python
-authenticated_sockets = connection.pipe(
-    filter_new_socket_only(),
-    operators.map(add_token),
-    operators.share(),
-)
-```
-
-# Development guidelines
-
-## `*_http` methods
-
-REST functions over http should be suffixed with `_http` e.g. `get_book_http`.
-They should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.
-
-Where possible models should be defined to describe the *raw* result and *parsed result* if available/useful.
-
-Reactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.
-
+# Binance Websocket
+
+[NOT RELEASED] This is very much a work in progress, despite being on pypi.
+Most things might be wrongly documented; API **will** change
+
+## Features
+
+- Reconnect with incremental backoff 
+- Respond to ping
+- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API
+- ... but provides more info than a simple request/response; 
+  for instance, `add_order` goes through each stage submitted->pending->open or canceled, 
+  emitting a notification at each stage
+
+## Installing
+
+`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`
+
+## General considerations
+
+### Observables/Reactivex
+
+The whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).
+
+Though Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.
+
+For simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below
+
+### Concurrency
+
+Internally the library uses threads.
+For your main program you don't have to worry about threads; you can block the main thread.
+
+## Getting started
+
+### Connect to the public feeds
+
+```python
+from bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker
+from bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only
+
+# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method
+socket_connection = public_websocket_connection()
+# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…
+messages = socket_connection.pipe(
+    keep_messages_only(),
+)
+socket_connection.pipe(
+    filter_new_socket_only(),
+    subscribe_ticker('USDT/USD', messages)
+).subscribe(
+    print, print, print  # you can do anything with the messages; here we simply print them out
+)
+socket_connection.connect()
+```
+
+_(This script is complete, it should run "as is")_
+
+
+## Logging
+
+We use Python's standard logging.
+You can modify what logs you see as follows:
+
+```
+logging.getLogger('bittrade_huobi_websocket').addHandler(logging.StreamHandler())
+```
+
+In addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`
+
+To view a full, timestamped history of the socket exchanges use
+
+```
+handler = FileHandler("logs/raw_socket.log")
+handler.setLevel(DEBUG)
+logger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")
+formatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")
+handler.setFormatter(formatter)
+logger.addHandler(handler)
+handler = FileHandler("logs/raw_socket.log")
+handler.setLevel(DEBUG)
+logger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")
+formatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")
+handler.setFormatter(formatter)
+logger.addHandler(handler)
+```
+
+## Private feeds
+
+Similar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.
+
+This means that you'll need to implement the signature token yourself. The library never has access to your API secret.
+
+See `examples/sign.py` for an example of implementation but it is generally as simple as:
+
+```python
+authenticated_sockets = connection.pipe(
+    filter_new_socket_only(),
+    operators.map(add_token),
+    operators.share(),
+)
+```
+
+# Development guidelines
+
+## `*_http` methods
+
+REST functions over http should be suffixed with `_http` e.g. `get_book_http`.
+They should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.
+
+Where possible models should be defined to describe the *raw* result and *parsed result* if available/useful.
+
+Reactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.
+
 Any operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.
```

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/book_ticker.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/depth.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/depth.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/channels/subscribe.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/channels/subscribe.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/connection_operators.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/generic.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/http.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/private.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/private_user_stream.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/private_user_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/public_stream.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/public_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/connection/reconnect.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/add_order.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/add_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/cancel_order.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/ping.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/ping.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/request_response.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/events/time.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/events/time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/framework/framework.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/framework/framework.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/filters/kind.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/filters/kind.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/json.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/messages/listen.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/messages/listen.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/endpoints.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/enhanced_websocket.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/framework.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/framework.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/order.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,27 @@
     recvWindow: Optional[int] = None
     is_margin: Optional[bool] = False
     isIsolated: Optional[bool] = None
 
     def to_dict(self):
         as_dict = dataclasses.asdict(self)
         del as_dict["is_margin"]
-        if not self.is_margin:
+        if self.is_margin:
+            as_dict["isIsolated"] = "TRUE" if self.isIsolated else "FALSE"
+        else:
             del as_dict["isIsolated"]
+        for key in (
+            "newOrderRespType",
+            "selfTradePreventionMode",
+            "side",
+            "type",
+            "timeInForce",
+        ):
+            if enum_value := getattr(self, key, None):
+                as_dict[key] = enum_value.value
         return as_dict
 
 
 @dataclasses.dataclass
 class PlaceOrderResponse:
     symbol: str
     orderId: int
@@ -116,14 +127,16 @@
     isIsolated: Optional[bool] = None
 
     def to_dict(self):
         as_dict = dataclasses.asdict(self)
         del as_dict["is_margin"]
         if self.is_margin:
             as_dict["isIsolated"] = "TRUE" if self.isIsolated else "FALSE"
+        else:
+            del as_dict["isIsolated"]
         return as_dict
 
 
 @dataclasses.dataclass
 class SymbolOrdersCancelRequest:
     symbol: str
     recvWindow: Optional[int] = None
@@ -131,14 +144,16 @@
     isIsolated: Optional[bool] = None
 
     def to_dict(self):
         as_dict = dataclasses.asdict(self)
         del as_dict["is_margin"]
         if self.is_margin:
             as_dict["isIsolated"] = "TRUE" if self.isIsolated else "FALSE"
+        else:
+            del as_dict["isIsolated"]
         return as_dict
 
 
 @dataclasses.dataclass
 class MarginSymbolOrdersRequest:
     symbol: str
     isIsolated: bool = False
```

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/order_status.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/order_status.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/models/rest/margin_account.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/models/rest/margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/operators/orderbook/__init__.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/operators/orderbook/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Callable, Any
-from reactivex import operators, Observable
-
-
-def map_bids_only() -> Callable[[Observable[dict]], Observable[list[tuple[float, ...]]]]:
-    return operators.map(lambda x: x["bids"])
-
-
-def map_asks_only() -> Callable[[Observable[dict]], Observable[list[tuple[float, ...]]]]:
-    return operators.map(lambda x: x["asks"])
-
-def _best_price(x: list[tuple[float, ...]]):
-    return x[0][0]
-
-def map_top_prices() -> Callable[[Observable[Any]], Observable[tuple[float, float]]]:
-    return operators.map(lambda x: (_best_price(x["bids"]), _best_price(x["asks"])))
-
-def map_best_price() -> Callable[[Observable[list[tuple[float, ...]]]], Observable[float]]:
-    return operators.map(_best_price)
+from typing import Callable, Any
+from reactivex import operators, Observable
+
+
+def map_bids_only() -> Callable[[Observable[dict]], Observable[list[tuple[float, ...]]]]:
+    return operators.map(lambda x: x["bids"])
+
+
+def map_asks_only() -> Callable[[Observable[dict]], Observable[list[tuple[float, ...]]]]:
+    return operators.map(lambda x: x["asks"])
+
+def _best_price(x: list[tuple[float, ...]]):
+    return x[0][0]
+
+def map_top_prices() -> Callable[[Observable[Any]], Observable[tuple[float, float]]]:
+    return operators.map(lambda x: (_best_price(x["bids"]), _best_price(x["asks"])))
+
+def map_best_price() -> Callable[[Observable[list[tuple[float, ...]]]], Observable[float]]:
+    return operators.map(_best_price)
```

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/operators/stream/response_messages.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/operators/stream/response_messages.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/cancel_order.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/create_order.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/current_open_orders.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/current_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/get_time.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/get_time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/http_factory_decorator.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/http_factory_decorator.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/listen_key.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/listen_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/query_margin_account.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/query_margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/query_margin_fee_data.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/query_margin_fee_data.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/symbol_orders_cancel.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/symbol_orders_cancel.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/rest/symbol_price_ticker.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/rest/symbol_price_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/bittrade_binance_websocket/sign.py` & `bittrade_binance_websocket-0.1.4/bittrade_binance_websocket/sign.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.3/pyproject.toml` & `bittrade_binance_websocket-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-binance-websocket"
-version = "0.1.3"
+version = "0.1.4"
 description = "Reactive Websocket for Binance"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 license = "MIT"
 classifiers = [
@@ -50,14 +50,15 @@
 
 
 
 
 
 
 
+
 
 [tool.poetry.group.rich.dependencies]
 fire = "^0.5.0"
 rich = "^13.3.1"
 
 [tool.black]
 line-length = 88
```

### Comparing `bittrade_binance_websocket-0.1.3/setup.py` & `bittrade_binance_websocket-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.4.2,<2.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'bittrade-binance-websocket',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Reactive Websocket for Binance',
     'long_description': '# Binance Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff \n- Respond to ping\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_huobi_websocket\').addHandler(logging.StreamHandler())\n```\n\nIn addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`\n\nTo view a full, timestamped history of the socket exchanges use\n\n```\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nThis means that you\'ll need to implement the signature token yourself. The library never has access to your API secret.\n\nSee `examples/sign.py` for an example of implementation but it is generally as simple as:\n\n```python\nauthenticated_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n# Development guidelines\n\n## `*_http` methods\n\nREST functions over http should be suffixed with `_http` e.g. `get_book_http`.\nThey should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.\n\nWhere possible models should be defined to describe the *raw* result and *parsed result* if available/useful.\n\nReactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.\n\nAny operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-binance-websocket',
```

### Comparing `bittrade_binance_websocket-0.1.3/PKG-INFO` & `bittrade_binance_websocket-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-binance-websocket
-Version: 0.1.3
+Version: 0.1.4
 Summary: Reactive Websocket for Binance
 Home-page: https://github.com/TechSpaceAsia/bittrade-binance-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

