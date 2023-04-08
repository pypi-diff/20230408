# Comparing `tmp/bovine-0.0.8.tar.gz` & `tmp/bovine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.0.8.tar", max compression
+gzip compressed data, was "bovine-0.0.9.tar", max compression
```

## Comparing `bovine-0.0.8.tar` & `bovine-0.0.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     5744 2023-03-25 08:45:05.838742 bovine-0.0.8/README.md
--rw-r--r--   0        0        0     1572 2023-03-24 15:43:02.258186 bovine-0.0.8/bovine/__init__.py
--rw-r--r--   0        0        0      135 2023-03-09 14:15:03.990325 bovine-0.0.8/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      433 2023-03-24 17:38:21.495829 bovine-0.0.8/bovine/activitypub/activity_factory.py
--rw-r--r--   0        0        0     5213 2023-03-24 17:31:31.844569 bovine-0.0.8/bovine/activitypub/actor.py
--rw-r--r--   0        0        0     2258 2023-03-24 15:50:13.824440 bovine-0.0.8/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      429 2023-03-20 10:43:54.377726 bovine-0.0.8/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0      549 2023-03-19 16:16:18.865574 bovine-0.0.8/bovine/activitypub/object_factory.py
--rw-r--r--   0        0        0     3159 2023-03-24 17:38:21.571829 bovine-0.0.8/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      500 2023-02-04 17:51:50.746650 bovine-0.0.8/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0      778 2023-03-09 14:15:03.990325 bovine-0.0.8/bovine/activitystreams/activities/__init__.py
--rw-r--r--   0        0        0      597 2023-03-09 14:15:03.990325 bovine-0.0.8/bovine/activitystreams/activities/accept_builder.py
--rw-r--r--   0        0        0     1456 2023-02-01 09:02:28.507153 bovine-0.0.8/bovine/activitystreams/activities/create_builder.py
--rw-r--r--   0        0        0      735 2023-03-10 14:37:48.405572 bovine-0.0.8/bovine/activitystreams/activities/delete_builder.py
--rw-r--r--   0        0        0      509 2023-02-01 10:42:10.659202 bovine-0.0.8/bovine/activitystreams/activities/follow_builder.py
--rw-r--r--   0        0        0     1040 2023-03-10 14:37:54.201636 bovine-0.0.8/bovine/activitystreams/activities/like_builder.py
--rw-r--r--   0        0        0      387 2023-01-17 14:01:43.244742 bovine-0.0.8/bovine/activitystreams/activities/test_accept_builder.py
--rw-r--r--   0        0        0      917 2023-03-10 14:36:42.507038 bovine-0.0.8/bovine/activitystreams/activities/test_create_builder.py
--rw-r--r--   0        0        0      259 2023-01-31 08:42:22.041274 bovine-0.0.8/bovine/activitystreams/activities/test_delete_builder.py
--rw-r--r--   0        0        0      379 2023-01-31 08:41:47.244847 bovine-0.0.8/bovine/activitystreams/activities/test_follow_builder.py
--rw-r--r--   0        0        0      409 2023-03-09 14:15:03.990325 bovine-0.0.8/bovine/activitystreams/activities/test_like_builder.py
--rw-r--r--   0        0        0      299 2023-03-09 14:15:03.990325 bovine-0.0.8/bovine/activitystreams/activities/undo_builder.py
--rw-r--r--   0        0        0     3329 2023-03-10 14:36:37.496150 bovine-0.0.8/bovine/activitystreams/actor_builder.py
--rw-r--r--   0        0        0      155 2023-01-31 08:42:22.041274 bovine-0.0.8/bovine/activitystreams/common/__init__.py
--rw-r--r--   0        0        0      944 2023-01-31 08:42:22.041274 bovine-0.0.8/bovine/activitystreams/common/context_builder.py
--rw-r--r--   0        0        0     1357 2023-01-31 08:42:22.041274 bovine-0.0.8/bovine/activitystreams/common/test_context_builder.py
--rw-r--r--   0        0        0      307 2023-03-19 16:16:18.853573 bovine-0.0.8/bovine/activitystreams/objects/__init__.py
--rw-r--r--   0        0        0      235 2023-03-19 16:16:18.865574 bovine-0.0.8/bovine/activitystreams/objects/note_builder.py
--rw-r--r--   0        0        0     3794 2023-03-23 18:13:46.605395 bovine-0.0.8/bovine/activitystreams/objects/object_builder.py
--rw-r--r--   0        0        0     2157 2023-03-19 16:16:18.853573 bovine-0.0.8/bovine/activitystreams/objects/test_note_builder.py
--rw-r--r--   0        0        0      163 2023-01-31 08:42:22.041274 bovine-0.0.8/bovine/activitystreams/objects/test_tombstone_builder.py
--rw-r--r--   0        0        0      344 2023-03-10 14:37:20.402249 bovine-0.0.8/bovine/activitystreams/objects/tombstone_builder.py
--rw-r--r--   0        0        0     1021 2023-02-05 10:08:43.390300 bovine-0.0.8/bovine/activitystreams/ordered_collection_builder.py
--rw-r--r--   0        0        0      971 2023-02-04 15:54:46.460872 bovine-0.0.8/bovine/activitystreams/ordered_collection_page_builder.py
--rw-r--r--   0        0        0     1615 2023-03-10 14:36:40.235525 bovine-0.0.8/bovine/activitystreams/test_actor_builder.py
--rw-r--r--   0        0        0     1165 2023-02-04 15:45:55.208330 bovine-0.0.8/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      907 2023-02-04 15:55:05.840941 bovine-0.0.8/bovine/activitystreams/test_ordered_collection_page_builder.py
--rw-r--r--   0        0        0     1177 2023-03-21 16:59:50.049501 bovine-0.0.8/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0      787 2023-03-20 09:55:30.800090 bovine-0.0.8/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     1593 2023-03-19 16:16:18.805573 bovine-0.0.8/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0        0 2023-02-01 11:25:23.677425 bovine-0.0.8/bovine/clients/__init__.py
--rw-r--r--   0        0        0       83 2023-03-19 16:16:18.853573 bovine-0.0.8/bovine/clients/consts.py
--rw-r--r--   0        0        0     1034 2023-03-10 14:34:42.596286 bovine-0.0.8/bovine/clients/event_source.py
--rw-r--r--   0        0        0     1493 2023-03-24 15:30:34.358765 bovine-0.0.8/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3159 2023-03-24 17:31:32.720575 bovine-0.0.8/bovine/clients/moo_auth_client.py
--rw-r--r--   0        0        0     1399 2023-03-10 11:13:25.612108 bovine-0.0.8/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     3261 2023-03-10 14:34:56.587254 bovine-0.0.8/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     1074 2023-03-24 14:58:19.852389 bovine-0.0.8/bovine/clients/signed_http_client.py
--rw-r--r--   0        0        0      638 2023-03-24 17:38:21.503829 bovine-0.0.8/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      304 2023-03-10 15:13:34.129037 bovine-0.0.8/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1159 2023-03-10 14:35:33.299257 bovine-0.0.8/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      576 2023-03-24 14:59:03.816692 bovine-0.0.8/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0      282 2023-03-09 14:15:03.994325 bovine-0.0.8/bovine/test_types.py
--rw-r--r--   0        0        0     1832 2023-03-09 14:15:03.994325 bovine-0.0.8/bovine/types.py
--rw-r--r--   0        0        0     1045 2023-02-01 11:31:34.017446 bovine-0.0.8/bovine/utils/__init__.py
--rw-r--r--   0        0        0     1966 2023-03-24 17:38:21.551829 bovine-0.0.8/bovine/utils/crypto/__init__.py
--rw-r--r--   0        0        0     2175 2023-03-24 15:33:41.584599 bovine-0.0.8/bovine/utils/crypto/did_key.py
--rw-r--r--   0        0        0     1028 2023-03-24 17:38:21.519829 bovine-0.0.8/bovine/utils/crypto/test_crypto.py
--rw-r--r--   0        0        0     1339 2023-03-24 17:38:21.527829 bovine-0.0.8/bovine/utils/crypto/test_did_key.py
--rw-r--r--   0        0        0      519 2023-01-24 19:32:45.881784 bovine-0.0.8/bovine/utils/date.py
--rw-r--r--   0        0        0     1955 2023-03-24 14:26:06.295997 bovine-0.0.8/bovine/utils/http_signature.py
--rw-r--r--   0        0        0      186 2023-03-10 11:19:46.071642 bovine-0.0.8/bovine/utils/parse.py
--rw-r--r--   0        0        0     2715 2023-03-19 16:16:18.853573 bovine-0.0.8/bovine/utils/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-02-10 10:31:09.425518 bovine-0.0.8/bovine/utils/signature_parser.py
--rw-r--r--   0        0        0      181 2023-02-01 10:42:08.771183 bovine-0.0.8/bovine/utils/test.py
--rw-r--r--   0        0        0      737 2023-02-01 11:30:58.697070 bovine-0.0.8/bovine/utils/test_date.py
--rw-r--r--   0        0        0     2979 2023-03-19 16:16:18.825573 bovine-0.0.8/bovine/utils/test_http_signature.py
--rw-r--r--   0        0        0      457 2023-03-10 11:08:29.021486 bovine-0.0.8/bovine/utils/test_parse.py
--rw-r--r--   0        0        0     1207 2023-02-10 10:31:31.613742 bovine-0.0.8/bovine/utils/test_signature_parser.py
--rw-r--r--   0        0        0       22 2023-03-25 08:46:37.676348 bovine-0.0.8/bovine/version.py
--rw-r--r--   0        0        0      939 2023-03-25 08:46:29.560210 bovine-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6969 1970-01-01 00:00:00.000000 bovine-0.0.8/setup.py
--rw-r--r--   0        0        0     6581 1970-01-01 00:00:00.000000 bovine-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9040 2023-03-25 10:32:01.307672 bovine-0.0.9/README.md
+-rw-r--r--   0        0        0     1611 2023-03-25 10:38:12.803581 bovine-0.0.9/bovine/__init__.py
+-rw-r--r--   0        0        0      135 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      433 2023-03-25 10:43:18.023969 bovine-0.0.9/bovine/activitypub/activity_factory.py
+-rw-r--r--   0        0        0     5213 2023-03-25 10:37:33.475555 bovine-0.0.9/bovine/activitypub/actor.py
+-rw-r--r--   0        0        0     2258 2023-03-24 15:50:13.824440 bovine-0.0.9/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      429 2023-03-20 10:43:54.377726 bovine-0.0.9/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0      582 2023-03-25 10:39:52.167675 bovine-0.0.9/bovine/activitypub/object_factory.py
+-rw-r--r--   0        0        0     3159 2023-03-25 10:43:18.083969 bovine-0.0.9/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      500 2023-02-04 17:51:50.746650 bovine-0.0.9/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/__init__.py
+-rw-r--r--   0        0        0      597 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/accept_builder.py
+-rw-r--r--   0        0        0     1456 2023-02-01 09:02:28.507153 bovine-0.0.9/bovine/activitystreams/activities/create_builder.py
+-rw-r--r--   0        0        0      735 2023-03-10 14:37:48.405572 bovine-0.0.9/bovine/activitystreams/activities/delete_builder.py
+-rw-r--r--   0        0        0      509 2023-02-01 10:42:10.659202 bovine-0.0.9/bovine/activitystreams/activities/follow_builder.py
+-rw-r--r--   0        0        0     1040 2023-03-10 14:37:54.201636 bovine-0.0.9/bovine/activitystreams/activities/like_builder.py
+-rw-r--r--   0        0        0      387 2023-01-17 14:01:43.244742 bovine-0.0.9/bovine/activitystreams/activities/test_accept_builder.py
+-rw-r--r--   0        0        0      917 2023-03-10 14:36:42.507038 bovine-0.0.9/bovine/activitystreams/activities/test_create_builder.py
+-rw-r--r--   0        0        0      259 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/activities/test_delete_builder.py
+-rw-r--r--   0        0        0      379 2023-01-31 08:41:47.244847 bovine-0.0.9/bovine/activitystreams/activities/test_follow_builder.py
+-rw-r--r--   0        0        0      409 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/test_like_builder.py
+-rw-r--r--   0        0        0      299 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/undo_builder.py
+-rw-r--r--   0        0        0     3329 2023-03-10 14:36:37.496150 bovine-0.0.9/bovine/activitystreams/actor_builder.py
+-rw-r--r--   0        0        0      155 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/__init__.py
+-rw-r--r--   0        0        0      944 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/context_builder.py
+-rw-r--r--   0        0        0     1357 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/test_context_builder.py
+-rw-r--r--   0        0        0      307 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/activitystreams/objects/__init__.py
+-rw-r--r--   0        0        0      235 2023-03-19 16:16:18.865574 bovine-0.0.9/bovine/activitystreams/objects/note_builder.py
+-rw-r--r--   0        0        0     3794 2023-03-23 18:13:46.605395 bovine-0.0.9/bovine/activitystreams/objects/object_builder.py
+-rw-r--r--   0        0        0     2157 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/activitystreams/objects/test_note_builder.py
+-rw-r--r--   0        0        0      163 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/objects/test_tombstone_builder.py
+-rw-r--r--   0        0        0      344 2023-03-10 14:37:20.402249 bovine-0.0.9/bovine/activitystreams/objects/tombstone_builder.py
+-rw-r--r--   0        0        0     1021 2023-02-05 10:08:43.390300 bovine-0.0.9/bovine/activitystreams/ordered_collection_builder.py
+-rw-r--r--   0        0        0      971 2023-02-04 15:54:46.460872 bovine-0.0.9/bovine/activitystreams/ordered_collection_page_builder.py
+-rw-r--r--   0        0        0     1615 2023-03-10 14:36:40.235525 bovine-0.0.9/bovine/activitystreams/test_actor_builder.py
+-rw-r--r--   0        0        0     1165 2023-02-04 15:45:55.208330 bovine-0.0.9/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      907 2023-02-04 15:55:05.840941 bovine-0.0.9/bovine/activitystreams/test_ordered_collection_page_builder.py
+-rw-r--r--   0        0        0     1177 2023-03-21 16:59:50.049501 bovine-0.0.9/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0      787 2023-03-20 09:55:30.800090 bovine-0.0.9/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     1593 2023-03-19 16:16:18.805573 bovine-0.0.9/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0        0 2023-02-01 11:25:23.677425 bovine-0.0.9/bovine/clients/__init__.py
+-rw-r--r--   0        0        0       83 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1034 2023-03-10 14:34:42.596286 bovine-0.0.9/bovine/clients/event_source.py
+-rw-r--r--   0        0        0     1493 2023-03-24 15:30:34.358765 bovine-0.0.9/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3159 2023-03-24 17:31:32.720575 bovine-0.0.9/bovine/clients/moo_auth_client.py
+-rw-r--r--   0        0        0     1399 2023-03-10 11:13:25.612108 bovine-0.0.9/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     3261 2023-03-10 14:34:56.587254 bovine-0.0.9/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     1074 2023-03-24 14:58:19.852389 bovine-0.0.9/bovine/clients/signed_http_client.py
+-rw-r--r--   0        0        0      638 2023-03-25 10:43:18.023969 bovine-0.0.9/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      304 2023-03-10 15:13:34.129037 bovine-0.0.9/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1159 2023-03-10 14:35:33.299257 bovine-0.0.9/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      576 2023-03-24 14:59:03.816692 bovine-0.0.9/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0      282 2023-03-09 14:15:03.994325 bovine-0.0.9/bovine/test_types.py
+-rw-r--r--   0        0        0     1832 2023-03-09 14:15:03.994325 bovine-0.0.9/bovine/types.py
+-rw-r--r--   0        0        0     1045 2023-02-01 11:31:34.017446 bovine-0.0.9/bovine/utils/__init__.py
+-rw-r--r--   0        0        0     1966 2023-03-25 10:43:18.055969 bovine-0.0.9/bovine/utils/crypto/__init__.py
+-rw-r--r--   0        0        0     2175 2023-03-24 15:33:41.584599 bovine-0.0.9/bovine/utils/crypto/did_key.py
+-rw-r--r--   0        0        0     1028 2023-03-25 10:43:18.035969 bovine-0.0.9/bovine/utils/crypto/test_crypto.py
+-rw-r--r--   0        0        0     1339 2023-03-25 10:43:18.043969 bovine-0.0.9/bovine/utils/crypto/test_did_key.py
+-rw-r--r--   0        0        0      519 2023-01-24 19:32:45.881784 bovine-0.0.9/bovine/utils/date.py
+-rw-r--r--   0        0        0     1955 2023-03-24 14:26:06.295997 bovine-0.0.9/bovine/utils/http_signature.py
+-rw-r--r--   0        0        0      186 2023-03-10 11:19:46.071642 bovine-0.0.9/bovine/utils/parse.py
+-rw-r--r--   0        0        0     2715 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/utils/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-02-10 10:31:09.425518 bovine-0.0.9/bovine/utils/signature_parser.py
+-rw-r--r--   0        0        0      181 2023-02-01 10:42:08.771183 bovine-0.0.9/bovine/utils/test.py
+-rw-r--r--   0        0        0      737 2023-02-01 11:30:58.697070 bovine-0.0.9/bovine/utils/test_date.py
+-rw-r--r--   0        0        0     2979 2023-03-19 16:16:18.825573 bovine-0.0.9/bovine/utils/test_http_signature.py
+-rw-r--r--   0        0        0      457 2023-03-10 11:08:29.021486 bovine-0.0.9/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0     1207 2023-02-10 10:31:31.613742 bovine-0.0.9/bovine/utils/test_signature_parser.py
+-rw-r--r--   0        0        0       22 2023-03-25 10:40:50.823746 bovine-0.0.9/bovine/version.py
+-rw-r--r--   0        0        0      932 2023-03-25 10:40:37.763729 bovine-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 bovine-0.0.9/setup.py
+-rw-r--r--   0        0        0     9872 1970-01-01 00:00:00.000000 bovine-0.0.9/PKG-INFO
```

### Comparing `bovine-0.0.8/bovine/__init__.py` & `bovine-0.0.9/bovine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 from .activitypub.actor import ActivityPubActor
 
 
 class BovineActor(ActivityPubActor):
     def __init__(self, config):
         self.config = config
-        super().__init__()  # self.config["account_url"])
+        super().__init__()
 
     async def init(self, session=None):
         self.session = session
         if session is None:
             self.session = aiohttp.ClientSession()
 
         if self._has_moo_auth():
             await self.with_host_and_ed25519_private_key(
                 self.config["host"], self.config["private_key"], session=self.session
             )
         elif self._has_http_signature():
+            self.actor_id = self.config["account_url"]
             self.with_http_signature(
                 self.config["public_key_url"],
                 self.config["private_key"],
                 session=self.session,
             )
         else:
             raise Exception("No known authorization method available")
@@ -33,15 +34,15 @@
         await self.init()
         return self
 
     async def __aexit__(self, *args):
         await self.session.close()
 
     def _has_http_signature(self):
-        return self._has_keys(["public_key_url", "private_key"])
+        return self._has_keys(["account_url", "public_key_url", "private_key"])
 
     def _has_moo_auth(self):
         return self._has_keys(["host", "private_key"])
 
     def _has_keys(self, key_list):
         for key in key_list:
             if key not in self.config:
```

### Comparing `bovine-0.0.8/bovine/activitypub/actor.py` & `bovine-0.0.9/bovine/activitypub/actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitypub/collection_helper.py` & `bovine-0.0.9/bovine/activitypub/collection_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitypub/object_factory.py` & `bovine-0.0.9/bovine/activitypub/object_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class ObjectFactory:
     def __init__(self, actor_information):
         self.information = actor_information
 
     def note(self, text):
         return NoteBuilder(
-            self.information["id"], text, followers=self.information["followers"]
+            self.information["id"], text, followers=self.information.get("followers")
         )
 
     def article(self):
         return ObjectBuilder(
-            "Article", self.information["id"], followers=self.information["followers"]
+            "Article",
+            self.information["id"],
+            followers=self.information.get("followers"),
         )
```

### Comparing `bovine-0.0.8/bovine/activitypub/test_actor.py` & `bovine-0.0.9/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/__init__.py` & `bovine-0.0.9/bovine/activitystreams/activities/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/accept_builder.py` & `bovine-0.0.9/bovine/activitystreams/activities/accept_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/create_builder.py` & `bovine-0.0.9/bovine/activitystreams/activities/create_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/delete_builder.py` & `bovine-0.0.9/bovine/activitystreams/activities/delete_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/like_builder.py` & `bovine-0.0.9/bovine/activitystreams/activities/like_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/activities/test_create_builder.py` & `bovine-0.0.9/bovine/activitystreams/activities/test_create_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/actor_builder.py` & `bovine-0.0.9/bovine/activitystreams/actor_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/common/context_builder.py` & `bovine-0.0.9/bovine/activitystreams/common/context_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/common/test_context_builder.py` & `bovine-0.0.9/bovine/activitystreams/common/test_context_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/objects/object_builder.py` & `bovine-0.0.9/bovine/activitystreams/objects/object_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/objects/test_note_builder.py` & `bovine-0.0.9/bovine/activitystreams/objects/test_note_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/ordered_collection_builder.py` & `bovine-0.0.9/bovine/activitystreams/ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/ordered_collection_page_builder.py` & `bovine-0.0.9/bovine/activitystreams/ordered_collection_page_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/test_actor_builder.py` & `bovine-0.0.9/bovine/activitystreams/test_actor_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.0.9/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/test_ordered_collection_page_builder.py` & `bovine-0.0.9/bovine/activitystreams/test_ordered_collection_page_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/utils/__init__.py` & `bovine-0.0.9/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/utils/print.py` & `bovine-0.0.9/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/activitystreams/utils/test_utils.py` & `bovine-0.0.9/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/event_source.py` & `bovine-0.0.9/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/lookup_account.py` & `bovine-0.0.9/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/moo_auth_client.py` & `bovine-0.0.9/bovine/clients/moo_auth_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/nodeinfo.py` & `bovine-0.0.9/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/signed_http.py` & `bovine-0.0.9/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/signed_http_client.py` & `bovine-0.0.9/bovine/clients/signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/test_lookup_account.py` & `bovine-0.0.9/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/test_signed_http.py` & `bovine-0.0.9/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/clients/test_signed_http_client.py` & `bovine-0.0.9/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/types.py` & `bovine-0.0.9/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/__init__.py` & `bovine-0.0.9/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/crypto/__init__.py` & `bovine-0.0.9/bovine/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/crypto/did_key.py` & `bovine-0.0.9/bovine/utils/crypto/did_key.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/crypto/test_crypto.py` & `bovine-0.0.9/bovine/utils/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/crypto/test_did_key.py` & `bovine-0.0.9/bovine/utils/crypto/test_did_key.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/date.py` & `bovine-0.0.9/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/http_signature.py` & `bovine-0.0.9/bovine/utils/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/signature_checker.py` & `bovine-0.0.9/bovine/utils/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/signature_parser.py` & `bovine-0.0.9/bovine/utils/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/test_date.py` & `bovine-0.0.9/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/test_http_signature.py` & `bovine-0.0.9/bovine/utils/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/bovine/utils/test_signature_parser.py` & `bovine-0.0.9/bovine/utils/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.8/pyproject.toml` & `bovine-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bovine"
-version = "0.0.8"
+version = "0.0.9"
 description = "Core functionality of bovine needed to build client to server applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
-license = "../LICENSE"
+license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine"}]
 repository = "https://codeberg.org/helge/bovine"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
```

### Comparing `bovine-0.0.8/setup.py` & `bovine-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,17 +22,17 @@
  'cryptography>=39.0.0,<40.0.0',
  'multiformats>=0.2.1,<0.3.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'tomli>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bovine',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Core functionality of bovine needed to build client to server applications',
-    'long_description': '# Bovine\n\nThis package contains two essential parts of bovine. First\nit defines `BovineActor`, which contains all the necessities\nto write ActivityPub Clients. Furthermore, this package contains\nthe cryptographic routines to verify HTTP signatures.\n\nFurthermore, the folder `examples` contains a few examples on\nhow `BovineActor` can be used. The cryptographic routines\nare used in `bovine_fedi` to verify signatures.\n\n## Example: Make a post aka Faking at being a Server\n\nWhile [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.\n\nWithout having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.\n\n__FIXME!!!__\n\nStuff needed:\n\n- Generate Keys\n- Webfinger\n- Actor object\n- How to deploy\n- How to post\n\n## Using BovineActor\n\nOne can import it via `from bovine import BovineActor`. Then one can either use it via:\n\n```python\nasync with BovineActor(config) as actor:\n    ...\n# or\nactor = BovineActor(config)\nawait actor.init()\n```\n\nHere the config object can be present in two variants. First it can contain the keys `host` and `private_key`, where `host` is the domain the ActivityPub Actor is on and `private_key` is a mutlicodec encoded Ed25519 key, whose corresponding did-key has been added to the Actor. In this case [Moo-Auth-1](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation) will be used. The second variant is to use [HTTP Signatures](https://docs.joinmastodon.org/spec/security/#http), where the keys `account_url`, `public_key_url`, and `private_key` need to be present. Alternatively, to passing a config object, one can use `BovineActor.from_file(path_to_toml_file)`.\n\n### Making a post\n\nBovineActor contains two factories to create [ActivityStreams Objects](https://www.w3.org/TR/activitystreams-vocabulary/#object-types) and [ActivityStreams Activities](https://www.w3.org/TR/activitystreams-vocabulary/#activity-types). One can obtain them by running\n\n```python\nactivity_factory, object_factory = actor.factories\n```\n\nThe simplest usage example is a create wrapping a note, that looks like:\n\n```python\nactivity_factory, object_factory = actor.factories\nnote = object_factory.note("Hello").as_public().build()\ncreate = activity_factory.create(note).build()\n```\n\nThe result should be the something equivalent to the json\n\n```json\n{\n  "@context": "https://www.w3.org/ns/activitystreams",\n  "type": "Create",\n  "actor": "https://domain/actor",\n  "object": {\n    "attributedTo": "https://domain/actor",\n    "type": "Note",\n    "content": "Hello",\n    "published": "2023-03-25T08:12:32Z",\n    "to": "as:Public",\n    "cc": "https://domain/followers_collection"\n  },\n  "published": "2023-03-25T08:12:32Z",\n  "to": "as:Public",\n  "cc": "https://domain/followers_collection"\n}\n```\n\nThe details depend on the used actor and will likely contain superfluous elements until the creation process is improved. We can now send this activity to our outbox using\n\n```python\nawait actor.send_to_outbox(create)\n```\n\n__Note__: This is different from what we did in the first example, where we used `await actor.post(inbox, create)`. The difference is that in the first example, we faked being a server, now we are actually using Client To Server.\n\n### The inbox and outbox\n\nBy running\n\n```python\ninbox = await actor.inbox()\noutbox = await actor.outbox()\n```\n\none can obtain `CollectionHelper` objects. These are meant to make it easier to interact with collection objects. In the simplest use case, one can use\n\n```python\nawait inbox.next_item()\n```\n\nto get the items from the inbox one after the other. It is also possible to print a summary of all elements that have been fetched from the inbox using `await inbox.summary()`. Finally, it is possible to iterate over the inbox via\n\n```python\nasync for item in inbox.iterate(max_number=3):\n    do_something(item)\n```\n\n### Proxying elements\n\nWe have already seen the difference between using `post` directly to an inbox and posting to the actor\'s outbox using `send_to_outbox`. A similar pattern applies to fetching objects. Both of these commands often have a similar result\n\n```python\nawait actor.get(object_id)\nawait actor.proxy_element(object_id)\n```\n\nHowever, they do different things:\n\n- The first `actor.get` sends a webrequest to the server `object_id` is on and retrieves it\n- The second `actor.proxy_element` sends a request to the actor\'s server for the object. This request is then either answered from the server\'s object store or by the server fetching the object. The cache behavior is up to the server. Depending of the evolution of `proxyUrl` of an Actor, more options might be added here.\n\nAs most servers don\'t support Moo-Auth-1, using `proxy_element` is the only way to obtain foreign objects, when using it.\n\n### Event Source\n\nThe event source is demonstrated in `examples/sse.py`. First, the event source will be specified in a [FEP](https://codeberg.org/fediverse/fep) to come. It provides a way to receive updates from the server, whenever a new element is added to the inbox or outbox. The basic usage is\n\n```python\nevent_source = await actor.event_source()\nasync for event in event_source:\n    if event and event.data:\n        data = json.loads(event.data)\n        do_something(data)\n```\n\nIf you plan on writing long running applications, the event source does not automatically reconnect, so you will need to implement this. [mechanical_bull](https://codeberg.org/helge/mechanical_bull) uses the event source in this way.\n',
+    'long_description': '# Bovine\n\nThis package contains two essential parts of bovine. First\nit defines `BovineActor`, which contains all the necessities\nto write ActivityPub Clients. Furthermore, this package contains\nthe cryptographic routines to verify HTTP signatures.\n\nFurthermore, the folder `examples` contains a few examples on\nhow `BovineActor` can be used. The cryptographic routines\nare used in `bovine_fedi` to verify signatures.\n\n## Example: Make a post aka Faking at being a Server\n\nWhile [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.\n\nWithout having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.\n\nThe stub server is given by the following snippet. One should note that it just answers with predefined json from a config file, that hasn\'t been generated yet. One could easily replace it with serving static files. See also [the Mastodon Blog](https://blog.joinmastodon.org/2018/06/how-to-implement-a-basic-activitypub-server/) for a similar implementation.\n\n```python\nimport tomli\nimport json\nfrom quart import Quart\n\napp = Quart(__name__)\n\nwith open("server.toml", "rb") as fp:\n    config = tomli.load(fp)\n\n@app.get("/.well-known/webfinger")\nasync def webfinger():\n    return json.loads(config["webfinger"])\n\n\n@app.get("/actor")\nasync def actor():\n    return json.loads(config["actor"])\n\nif __name__ == "__main__":\n    app.run()\n```\n\nThe following script generates the config files. You will have to adapt the `hostname` variable and be able to serve the entire thing through https.\n\n```python\nimport bovine\nimport tomli_w\nimport json\n\nhostname = "bovine-demo.mymath.rocks"\n\npublic_key, private_key = bovine.utils.crypto.generate_public_private_key()\nactor_url = f"https://{hostname}/actor"\nactor = (\n    bovine.activitystreams.build_actor("actor")\n    .with_account_url(actor_url)\n    .with_public_key(public_key)\n)\n\nwebfinger = {\n    "subject": f"acct:actor@{hostname}",\n    "links": [\n        {\n            "href": actor_url,\n            "rel": "self",\n            "type": "application/activity+json",\n        }\n    ],\n}\n\nserver_config = {"actor": json.dumps(actor.build()), "webfinger": json.dumps(webfinger)}\n\nactor_config = {\n    "account_url": actor_url,\n    "public_key_url": f"{actor_url}#main-key",\n    "private_key": private_key,\n}\n\nwith open("server.toml", "wb") as fp:\n    tomli_w.dump(server_config, fp)\n\nwith open("bovine.toml", "wb") as fp:\n    tomli_w.dump(actor_config, fp)\n```\n\nYou can now access the urls, which are in my case [https://bovine-demo.mymath.rocks/actor](https://bovine-demo.mymath.rocks/actor) and [https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks](https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks). Using this, we can now lookup the fediverse handle `actor@bovine-demo.mymath.rocks` on most FediVerse applications.\n\nYou can now send a post via the following code snippet:\n\n```python\nimport asyncio\n\nfrom uuid import uuid4\nfrom bovine import BovineActor\n\ntarget_account = "https://mas.to/users/themilkman"\ntarget_inbox = "https://mas.to/users/themilkman/inbox"\n\n\nasync def run():\n    async with BovineActor.from_file("bovine.toml") as actor:\n        activity_factory, object_factory = actor.factories\n        note = (\n            object_factory.note("Hello")\n            .add_to(target_account)\n            .with_mention(target_account)\n            .build()\n        )\n        note["id"] = actor.actor_id + "/" + str(uuid4())\n        create = activity_factory.create(note).build()\n        create["id"] = actor.actor_id + "/" + str(uuid4())\n\n        await actor.post(target_inbox, create)\n\n\nasyncio.run(run())\n```\n\nA few comments are in order:\n\n- The id needs to be set on the Note and Create in order to be compatible with Mastodon. When using proper Client To Server as below, it is superfluous\n- The form of adding the `target_account` to both to and mention causes it to be a direct message.\n- Normally, you would look up the inbox from the target account.\n\n## Using BovineActor\n\nOne can import it via `from bovine import BovineActor`. Then one can either use it via:\n\n```python\nasync with BovineActor(config) as actor:\n    ...\n# or\nactor = BovineActor(config)\nawait actor.init()\n```\n\nHere the config object can be present in two variants. First it can contain the keys `host` and `private_key`, where `host` is the domain the ActivityPub Actor is on and `private_key` is a mutlicodec encoded Ed25519 key, whose corresponding did-key has been added to the Actor. In this case [Moo-Auth-1](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation) will be used. The second variant is to use [HTTP Signatures](https://docs.joinmastodon.org/spec/security/#http), where the keys `account_url`, `public_key_url`, and `private_key` need to be present. Alternatively, to passing a config object, one can use `BovineActor.from_file(path_to_toml_file)`.\n\n### Making a post\n\nBovineActor contains two factories to create [ActivityStreams Objects](https://www.w3.org/TR/activitystreams-vocabulary/#object-types) and [ActivityStreams Activities](https://www.w3.org/TR/activitystreams-vocabulary/#activity-types). One can obtain them by running\n\n```python\nactivity_factory, object_factory = actor.factories\n```\n\nThe simplest usage example is a create wrapping a note, that looks like:\n\n```python\nactivity_factory, object_factory = actor.factories\nnote = object_factory.note("Hello").as_public().build()\ncreate = activity_factory.create(note).build()\n```\n\nThe result should be the something equivalent to the json\n\n```json\n{\n  "@context": "https://www.w3.org/ns/activitystreams",\n  "type": "Create",\n  "actor": "https://domain/actor",\n  "object": {\n    "attributedTo": "https://domain/actor",\n    "type": "Note",\n    "content": "Hello",\n    "published": "2023-03-25T08:12:32Z",\n    "to": "as:Public",\n    "cc": "https://domain/followers_collection"\n  },\n  "published": "2023-03-25T08:12:32Z",\n  "to": "as:Public",\n  "cc": "https://domain/followers_collection"\n}\n```\n\nThe details depend on the used actor and will likely contain superfluous elements until the creation process is improved. We can now send this activity to our outbox using\n\n```python\nawait actor.send_to_outbox(create)\n```\n\n__Note__: This is different from what we did in the first example, where we used `await actor.post(inbox, create)`. The difference is that in the first example, we faked being a server, now we are actually using Client To Server.\n\n### The inbox and outbox\n\nBy running\n\n```python\ninbox = await actor.inbox()\noutbox = await actor.outbox()\n```\n\none can obtain `CollectionHelper` objects. These are meant to make it easier to interact with collection objects. In the simplest use case, one can use\n\n```python\nawait inbox.next_item()\n```\n\nto get the items from the inbox one after the other. It is also possible to print a summary of all elements that have been fetched from the inbox using `await inbox.summary()`. Finally, it is possible to iterate over the inbox via\n\n```python\nasync for item in inbox.iterate(max_number=3):\n    do_something(item)\n```\n\n### Proxying elements\n\nWe have already seen the difference between using `post` directly to an inbox and posting to the actor\'s outbox using `send_to_outbox`. A similar pattern applies to fetching objects. Both of these commands often have a similar result\n\n```python\nawait actor.get(object_id)\nawait actor.proxy_element(object_id)\n```\n\nHowever, they do different things:\n\n- The first `actor.get` sends a webrequest to the server `object_id` is on and retrieves it\n- The second `actor.proxy_element` sends a request to the actor\'s server for the object. This request is then either answered from the server\'s object store or by the server fetching the object. The cache behavior is up to the server. Depending of the evolution of `proxyUrl` of an Actor, more options might be added here.\n\nAs most servers don\'t support Moo-Auth-1, using `proxy_element` is the only way to obtain foreign objects, when using it.\n\n### Event Source\n\nThe event source is demonstrated in `examples/sse.py`. First, the event source will be specified in a [FEP](https://codeberg.org/fediverse/fep) to come. It provides a way to receive updates from the server, whenever a new element is added to the inbox or outbox. The basic usage is\n\n```python\nevent_source = await actor.event_source()\nasync for event in event_source:\n    if event and event.data:\n        data = json.loads(event.data)\n        do_something(data)\n```\n\nIf you plan on writing long running applications, the event source does not automatically reconnect, so you will need to implement this. [mechanical_bull](https://codeberg.org/helge/mechanical_bull) uses the event source in this way.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/helge/bovine',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bovine-0.0.8/PKG-INFO` & `bovine-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: bovine
-Version: 0.0.8
-Summary: Core functionality of bovine needed to build client to server applications
-Home-page: https://codeberg.org/helge/bovine
-License: ../LICENSE
-Author: Helge
-Author-email: helge.krueger@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: bleach (>=6.0.0,<7.0.0)
-Requires-Dist: cryptography (>=39.0.0,<40.0.0)
-Requires-Dist: multiformats (>=0.2.1,<0.3.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://codeberg.org/helge/bovine
-Description-Content-Type: text/markdown
-
 # Bovine
 
 This package contains two essential parts of bovine. First
 it defines `BovineActor`, which contains all the necessities
 to write ActivityPub Clients. Furthermore, this package contains
 the cryptographic routines to verify HTTP signatures.
 
@@ -33,23 +11,120 @@
 
 ## Example: Make a post aka Faking at being a Server
 
 While [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.
 
 Without having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.
 
-__FIXME!!!__
+The stub server is given by the following snippet. One should note that it just answers with predefined json from a config file, that hasn't been generated yet. One could easily replace it with serving static files. See also [the Mastodon Blog](https://blog.joinmastodon.org/2018/06/how-to-implement-a-basic-activitypub-server/) for a similar implementation.
+
+```python
+import tomli
+import json
+from quart import Quart
+
+app = Quart(__name__)
+
+with open("server.toml", "rb") as fp:
+    config = tomli.load(fp)
+
+@app.get("/.well-known/webfinger")
+async def webfinger():
+    return json.loads(config["webfinger"])
+
+
+@app.get("/actor")
+async def actor():
+    return json.loads(config["actor"])
+
+if __name__ == "__main__":
+    app.run()
+```
+
+The following script generates the config files. You will have to adapt the `hostname` variable and be able to serve the entire thing through https.
+
+```python
+import bovine
+import tomli_w
+import json
+
+hostname = "bovine-demo.mymath.rocks"
+
+public_key, private_key = bovine.utils.crypto.generate_public_private_key()
+actor_url = f"https://{hostname}/actor"
+actor = (
+    bovine.activitystreams.build_actor("actor")
+    .with_account_url(actor_url)
+    .with_public_key(public_key)
+)
+
+webfinger = {
+    "subject": f"acct:actor@{hostname}",
+    "links": [
+        {
+            "href": actor_url,
+            "rel": "self",
+            "type": "application/activity+json",
+        }
+    ],
+}
+
+server_config = {"actor": json.dumps(actor.build()), "webfinger": json.dumps(webfinger)}
 
-Stuff needed:
+actor_config = {
+    "account_url": actor_url,
+    "public_key_url": f"{actor_url}#main-key",
+    "private_key": private_key,
+}
+
+with open("server.toml", "wb") as fp:
+    tomli_w.dump(server_config, fp)
+
+with open("bovine.toml", "wb") as fp:
+    tomli_w.dump(actor_config, fp)
+```
+
+You can now access the urls, which are in my case [https://bovine-demo.mymath.rocks/actor](https://bovine-demo.mymath.rocks/actor) and [https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks](https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks). Using this, we can now lookup the fediverse handle `actor@bovine-demo.mymath.rocks` on most FediVerse applications.
+
+You can now send a post via the following code snippet:
+
+```python
+import asyncio
+
+from uuid import uuid4
+from bovine import BovineActor
 
-- Generate Keys
-- Webfinger
-- Actor object
-- How to deploy
-- How to post
+target_account = "https://mas.to/users/themilkman"
+target_inbox = "https://mas.to/users/themilkman/inbox"
+
+
+async def run():
+    async with BovineActor.from_file("bovine.toml") as actor:
+        activity_factory, object_factory = actor.factories
+        note = (
+            object_factory.note("Hello")
+            .add_to(target_account)
+            .with_mention(target_account)
+            .build()
+        )
+        note["id"] = actor.actor_id + "/" + str(uuid4())
+        create = activity_factory.create(note).build()
+        create["id"] = actor.actor_id + "/" + str(uuid4())
+
+        await actor.post(target_inbox, create)
+
+
+asyncio.run(run())
+```
+
+A few comments are in order:
+
+- The id needs to be set on the Note and Create in order to be compatible with Mastodon. When using proper Client To Server as below, it is superfluous
+- The form of adding the `target_account` to both to and mention causes it to be a direct message.
+- Normally, you would look up the inbox from the target account.
 
 ## Using BovineActor
 
 One can import it via `from bovine import BovineActor`. Then one can either use it via:
 
 ```python
 async with BovineActor(config) as actor:
@@ -153,8 +228,7 @@
 async for event in event_source:
     if event and event.data:
         data = json.loads(event.data)
         do_something(data)
 ```
 
 If you plan on writing long running applications, the event source does not automatically reconnect, so you will need to implement this. [mechanical_bull](https://codeberg.org/helge/mechanical_bull) uses the event source in this way.
-
```

