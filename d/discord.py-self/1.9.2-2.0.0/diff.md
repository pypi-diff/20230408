# Comparing `tmp/discord.py-self-1.9.2.tar.gz` & `tmp/discord.py-self-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord.py-self-1.9.2.tar", last modified: Wed Mar  2 01:56:37 2022, max compression
+gzip compressed data, was "discord.py-self-2.0.0.tar", last modified: Fri Apr  7 22:39:10 2023, max compression
```

## Comparing `discord.py-self-1.9.2.tar` & `discord.py-self-2.0.0.tar`

### file list

```diff
@@ -1,84 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.814586 discord.py-self-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-03-02 01:56:37.814586 discord.py-self-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.810587 discord.py-self-1.9.2/discord/
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9871 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46366 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)    23607 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    11425 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (121)    13768 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/backoff.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.810587 discord.py-self-1.9.2/discord/bin/
--rw-r--r--   0 runner    (1001) docker     (121)   441856 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/bin/libopus-0.x64.dll
--rw-r--r--   0 runner    (1001) docker     (121)   366080 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/bin/libopus-0.x86.dll
--rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/calls.py
--rw-r--r--   0 runner    (1001) docker     (121)    47301 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)    47991 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8222 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/colour.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/context_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    18073 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/embeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7615 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)    15812 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     5787 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.802586 discord.py-self-1.9.2/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.814586 discord.py-self-1.9.2/discord/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    36170 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)    15832 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (121)    12279 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    28937 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9275 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (121)    70598 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    25312 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    48469 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.814586 discord.py-self-1.9.2/discord/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)    16936 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)    31495 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    83537 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/guild_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)    47172 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     7149 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/integrations.py
--rw-r--r--   0 runner    (1001) docker     (121)    15909 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (121)    18156 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)    30908 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/member.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/mentions.py
--rw-r--r--   0 runner    (1001) docker     (121)    57755 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/object.py
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/oggparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    13540 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/opus.py
--rw-r--r--   0 runner    (1001) docker     (121)     5916 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/partial_emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)    20579 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    23104 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6398 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/relationship.py
--rw-r--r--   0 runner    (1001) docker     (121)    11981 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    48489 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/state.py
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (121)     6903 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/template.py
--rw-r--r--   0 runner    (1001) docker     (121)    40444 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    18973 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22766 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/voice_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    38520 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)     8607 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/discord/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 01:56:37.810587 discord.py-self-1.9.2/discord.py_self.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-03-02 01:56:37.000000 discord.py-self-1.9.2/discord.py_self.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-03-02 01:56:37.000000 discord.py-self-1.9.2/discord.py_self.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 01:56:37.000000 discord.py-self-1.9.2/discord.py_self.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-02 01:56:37.000000 discord.py-self-1.9.2/discord.py_self.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-02 01:56:37.000000 discord.py-self-1.9.2/discord.py_self.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-02 01:56:37.814586 discord.py-self-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-03-02 01:56:24.000000 discord.py-self-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.547421 discord.py-self-2.0.0/
+-rw-rw-rw-   0        0        0     1102 2022-03-23 14:03:55.000000 discord.py-self-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      116 2022-03-23 14:03:55.000000 discord.py-self-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5811 2023-04-07 22:39:10.546421 discord.py-self-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4533 2023-04-07 22:38:09.000000 discord.py-self-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.456111 discord.py-self-2.0.0/discord/
+-rw-rw-rw-   0        0        0     2436 2023-04-07 22:24:27.000000 discord.py-self-2.0.0/discord/__init__.py
+-rw-rw-rw-   0        0        0    10965 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/__main__.py
+-rw-rw-rw-   0        0        0    81997 2023-04-07 22:11:15.000000 discord.py-self-2.0.0/discord/abc.py
+-rw-rw-rw-   0        0        0    35249 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/activity.py
+-rw-rw-rw-   0        0        0     4272 2023-03-26 00:11:34.000000 discord.py-self-2.0.0/discord/affinity.py
+-rw-rw-rw-   0        0        0   124457 2023-04-07 01:26:12.000000 discord.py-self-2.0.0/discord/application.py
+-rw-rw-rw-   0        0        0    20104 2023-04-07 16:46:37.000000 discord.py-self-2.0.0/discord/asset.py
+-rw-rw-rw-   0        0        0    31379 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    24248 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/automod.py
+-rw-rw-rw-   0        0        0     3859 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/backoff.py
+-rw-rw-rw-   0        0        0    12634 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/billing.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.471278 discord.py-self-2.0.0/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0    16172 2023-04-05 21:40:09.000000 discord.py-self-2.0.0/discord/calls.py
+-rw-rw-rw-   0        0        0   135095 2023-04-05 22:11:46.000000 discord.py-self-2.0.0/discord/channel.py
+-rw-rw-rw-   0        0        0   155071 2023-04-07 15:22:18.000000 discord.py-self-2.0.0/discord/client.py
+-rw-rw-rw-   0        0        0    14681 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/colour.py
+-rw-rw-rw-   0        0        0    32936 2023-03-26 02:11:45.000000 discord.py-self-2.0.0/discord/commands.py
+-rw-rw-rw-   0        0        0    17498 2023-04-01 14:35:35.000000 discord.py-self-2.0.0/discord/components.py
+-rw-rw-rw-   0        0        0    11516 2023-02-15 22:20:22.000000 discord.py-self-2.0.0/discord/connections.py
+-rw-rw-rw-   0        0        0     3124 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/context_managers.py
+-rw-rw-rw-   0        0        0    23041 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/embeds.py
+-rw-rw-rw-   0        0        0     9463 2023-04-02 01:59:00.000000 discord.py-self-2.0.0/discord/emoji.py
+-rw-rw-rw-   0        0        0    23239 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/entitlements.py
+-rw-rw-rw-   0        0        0    38120 2023-04-05 01:54:27.000000 discord.py-self-2.0.0/discord/enums.py
+-rw-rw-rw-   0        0        0     8247 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.303080 discord.py-self-2.0.0/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.493982 discord.py-self-2.0.0/discord/ext/commands/
+-rw-rw-rw-   0        0        0      435 2022-04-29 00:38:09.000000 discord.py-self-2.0.0/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    43826 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    18691 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    18484 2023-04-03 03:00:03.000000 discord.py-self-2.0.0/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    46230 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    13738 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89505 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36755 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    23016 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    58954 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0     8647 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6443 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.494980 discord.py-self-2.0.0/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    29990 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5816 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/file.py
+-rw-rw-rw-   0        0        0    76908 2023-04-05 22:09:05.000000 discord.py-self-2.0.0/discord/flags.py
+-rw-rw-rw-   0        0        0    39923 2023-03-29 23:39:54.000000 discord.py-self-2.0.0/discord/gateway.py
+-rw-rw-rw-   0        0        0   168357 2023-04-07 15:25:26.000000 discord.py-self-2.0.0/discord/guild.py
+-rw-rw-rw-   0        0        0    10816 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/guild_premium.py
+-rw-rw-rw-   0        0        0     3529 2022-04-29 00:38:09.000000 discord.py-self-2.0.0/discord/handlers.py
+-rw-rw-rw-   0        0        0   177759 2023-04-07 01:31:43.000000 discord.py-self-2.0.0/discord/http.py
+-rw-rw-rw-   0        0        0    12512 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/integrations.py
+-rw-rw-rw-   0        0        0     7790 2023-03-28 01:51:53.000000 discord.py-self-2.0.0/discord/interactions.py
+-rw-rw-rw-   0        0        0    26660 2023-04-05 21:40:55.000000 discord.py-self-2.0.0/discord/invite.py
+-rw-rw-rw-   0        0        0     9503 2023-03-26 02:12:05.000000 discord.py-self-2.0.0/discord/library.py
+-rw-rw-rw-   0        0        0    43501 2023-04-07 22:16:10.000000 discord.py-self-2.0.0/discord/member.py
+-rw-rw-rw-   0        0        0     5743 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/mentions.py
+-rw-rw-rw-   0        0        0    85298 2023-04-03 03:00:03.000000 discord.py-self-2.0.0/discord/message.py
+-rw-rw-rw-   0        0        0     4655 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/metadata.py
+-rw-rw-rw-   0        0        0     1531 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/mixins.py
+-rw-rw-rw-   0        0        0     4534 2023-03-26 02:11:28.000000 discord.py-self-2.0.0/discord/modal.py
+-rw-rw-rw-   0        0        0     3812 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/object.py
+-rw-rw-rw-   0        0        0     3763 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15533 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/opus.py
+-rw-rw-rw-   0        0        0     9165 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    10693 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/payments.py
+-rw-rw-rw-   0        0        0    30168 2023-04-03 02:56:36.000000 discord.py-self-2.0.0/discord/permissions.py
+-rw-rw-rw-   0        0        0    27217 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/player.py
+-rw-rw-rw-   0        0        0    16128 2023-04-07 15:23:12.000000 discord.py-self-2.0.0/discord/profile.py
+-rw-rw-rw-   0        0        0    10463 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/promotions.py
+-rw-rw-rw-   0        0        0        0 2022-04-29 00:31:12.000000 discord.py-self-2.0.0/discord/py.typed
+-rw-rw-rw-   0        0        0    12430 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8482 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/reaction.py
+-rw-rw-rw-   0        0        0    10742 2023-03-25 00:41:05.000000 discord.py-self-2.0.0/discord/relationship.py
+-rw-rw-rw-   0        0        0    24102 2023-04-03 02:58:06.000000 discord.py-self-2.0.0/discord/role.py
+-rw-rw-rw-   0        0        0    24244 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    98360 2023-04-05 21:42:06.000000 discord.py-self-2.0.0/discord/settings.py
+-rw-rw-rw-   0        0        0     6848 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/stage_instance.py
+-rw-rw-rw-   0        0        0   120924 2023-04-07 01:05:10.000000 discord.py-self-2.0.0/discord/state.py
+-rw-rw-rw-   0        0        0    17642 2023-04-03 02:56:26.000000 discord.py-self-2.0.0/discord/sticker.py
+-rw-rw-rw-   0        0        0    93140 2023-03-26 02:12:03.000000 discord.py-self-2.0.0/discord/store.py
+-rw-rw-rw-   0        0        0    30116 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/subscriptions.py
+-rw-rw-rw-   0        0        0    19286 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/team.py
+-rw-rw-rw-   0        0        0     9691 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/template.py
+-rw-rw-rw-   0        0        0    34125 2023-03-30 00:08:56.000000 discord.py-self-2.0.0/discord/threads.py
+-rw-rw-rw-   0        0        0     7454 2023-04-03 00:02:40.000000 discord.py-self-2.0.0/discord/tracking.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.543248 discord.py-self-2.0.0/discord/types/
+-rw-rw-rw-   0        0        0      159 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2836 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/activity.py
+-rw-rw-rw-   0        0        0     7631 2023-04-07 01:26:24.000000 discord.py-self-2.0.0/discord/types/application.py
+-rw-rw-rw-   0        0        0     8193 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4141 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/automod.py
+-rw-rw-rw-   0        0        0     2493 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/types/billing.py
+-rw-rw-rw-   0        0        0     5126 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/channel.py
+-rw-rw-rw-   0        0        0     5805 2022-04-29 00:38:09.000000 discord.py-self-2.0.0/discord/types/command.py
+-rw-rw-rw-   0        0        0     2548 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/components.py
+-rw-rw-rw-   0        0        0     2419 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1718 2023-03-25 21:24:16.000000 discord.py-self-2.0.0/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     3327 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/types/entitlements.py
+-rw-rw-rw-   0        0        0    12841 2023-04-07 00:55:58.000000 discord.py-self-2.0.0/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5168 2023-04-02 01:46:21.000000 discord.py-self-2.0.0/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2419 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7070 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2813 2023-03-26 02:12:02.000000 discord.py-self-2.0.0/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1647 2023-03-26 02:12:01.000000 discord.py-self-2.0.0/discord/types/library.py
+-rw-rw-rw-   0        0        0     2051 2023-04-07 01:21:27.000000 discord.py-self-2.0.0/discord/types/member.py
+-rw-rw-rw-   0        0        0     4338 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/message.py
+-rw-rw-rw-   0        0        0     2285 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/types/payments.py
+-rw-rw-rw-   0        0        0     2668 2023-04-07 01:26:46.000000 discord.py-self-2.0.0/discord/types/profile.py
+-rw-rw-rw-   0        0        0     2526 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/types/promotions.py
+-rw-rw-rw-   0        0        0     1799 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/types/role.py
+-rw-rw-rw-   0        0        0     3412 2022-04-29 00:38:09.000000 discord.py-self-2.0.0/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1210 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2343 2023-04-03 02:56:26.000000 discord.py-self-2.0.0/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     5078 2023-03-26 02:12:01.000000 discord.py-self-2.0.0/discord/types/store.py
+-rw-rw-rw-   0        0        0     4653 2023-03-26 00:08:25.000000 discord.py-self-2.0.0/discord/types/subscriptions.py
+-rw-rw-rw-   0        0        0     2025 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/discord/types/team.py
+-rw-rw-rw-   0        0        0     1658 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/template.py
+-rw-rw-rw-   0        0        0     2569 2023-03-30 00:44:12.000000 discord.py-self-2.0.0/discord/types/threads.py
+-rw-rw-rw-   0        0        0     3841 2023-04-07 01:32:10.000000 discord.py-self-2.0.0/discord/types/user.py
+-rw-rw-rw-   0        0        0     2415 2023-03-30 00:14:09.000000 discord.py-self-2.0.0/discord/types/voice.py
+-rw-rw-rw-   0        0        0     2045 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1500 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1948 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/types/widget.py
+-rw-rw-rw-   0        0        0    35630 2023-04-07 22:20:06.000000 discord.py-self-2.0.0/discord/user.py
+-rw-rw-rw-   0        0        0    50402 2023-04-07 16:08:24.000000 discord.py-self-2.0.0/discord/utils.py
+-rw-rw-rw-   0        0        0    26268 2023-04-02 00:06:34.000000 discord.py-self-2.0.0/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.545252 discord.py-self-2.0.0/discord/webhook/
+-rw-rw-rw-   0        0        0      195 2022-04-29 00:09:50.000000 discord.py-self-2.0.0/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    61821 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    43801 2023-04-03 00:52:21.000000 discord.py-self-2.0.0/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7603 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10420 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-07 22:39:10.461624 discord.py-self-2.0.0/discord.py_self.egg-info/
+-rw-rw-rw-   0        0        0     5811 2023-04-07 22:39:09.000000 discord.py-self-2.0.0/discord.py_self.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-04-07 22:39:09.000000 discord.py-self-2.0.0/discord.py_self.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 22:39:09.000000 discord.py-self-2.0.0/discord.py_self.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      351 2023-04-07 22:39:09.000000 discord.py-self-2.0.0/discord.py_self.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-07 22:39:09.000000 discord.py-self-2.0.0/discord.py_self.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      902 2023-02-02 23:33:44.000000 discord.py-self-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       41 2023-03-25 00:46:42.000000 discord.py-self-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 22:39:10.547421 discord.py-self-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3218 2023-03-29 00:55:31.000000 discord.py-self-2.0.0/setup.py
```

### Comparing `discord.py-self-1.9.2/LICENSE` & `discord.py-self-2.0.0/discord/types/snowflake.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from typing import List, Union
+
+Snowflake = Union[str, int]
+SnowflakeList = List[Snowflake]
```

### Comparing `discord.py-self-1.9.2/discord/abc.py` & `discord.py-self-2.0.0/discord/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1288 +1,1622 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import abc
-import sys
-import copy
-import asyncio
-
-from .iterators import HistoryIterator
-from .context_managers import Typing
-from .enums import ChannelType
-from .errors import InvalidArgument, ClientException
-from .mentions import AllowedMentions
-from .permissions import PermissionOverwrite, Permissions
-from .role import Role
-from .invite import Invite
-from .file import File
-from .voice_client import VoiceClient, VoiceProtocol
-from . import utils
-
-class _Undefined:
-    def __repr__(self):
-        return 'see-below'
-
-_undefined = _Undefined()
-
-class Snowflake(metaclass=abc.ABCMeta):
-    """An ABC that details the common operations on a Discord model.
-
-    Almost all :ref:`Discord models <discord_api_models>` meet this
-    abstract base class.
-
-    If you want to create a snowflake on your own, consider using
-    :class:`.Object`.
-
-    Attributes
-    -----------
-    id: :class:`int`
-        The model's unique ID.
-    """
-    __slots__ = ()
-
-    @property
-    @abc.abstractmethod
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the model's creation time as a naive datetime in UTC."""
-        raise NotImplementedError
-
-    @classmethod
-    def __subclasshook__(cls, C):
-        if cls is Snowflake:
-            mro = C.__mro__
-            for attr in ('created_at', 'id'):
-                for base in mro:
-                    if attr in base.__dict__:
-                        break
-                else:
-                    return NotImplemented
-            return True
-        return NotImplemented
-
-class User(metaclass=abc.ABCMeta):
-    """An ABC that details the common operations on a Discord user.
-
-    The following implement this ABC:
-
-    - :class:`~discord.User`
-    - :class:`~discord.ClientUser`
-    - :class:`~discord.Member`
-
-    This ABC must also implement :class:`~discord.abc.Snowflake`.
-
-    Attributes
-    -----------
-    name: :class:`str`
-        The user's username.
-    discriminator: :class:`str`
-        The user's discriminator.
-    avatar: Optional[:class:`str`]
-        The avatar hash the user has.
-    bot: :class:`bool`
-        If the user is a bot account.
-    """
-    __slots__ = ()
-
-    @property
-    @abc.abstractmethod
-    def display_name(self):
-        """:class:`str`: Returns the user's display name."""
-        raise NotImplementedError
-
-    @property
-    @abc.abstractmethod
-    def mention(self):
-        """:class:`str`: Returns a string that allows you to mention the given user."""
-        raise NotImplementedError
-
-    @classmethod
-    def __subclasshook__(cls, C):
-        if cls is User:
-            if Snowflake.__subclasshook__(C) is NotImplemented:
-                return NotImplemented
-
-            mro = C.__mro__
-            for attr in ('display_name', 'mention', 'name', 'avatar', 'discriminator', 'bot'):
-                for base in mro:
-                    if attr in base.__dict__:
-                        break
-                else:
-                    return NotImplemented
-            return True
-        return NotImplemented
-
-class PrivateChannel(metaclass=abc.ABCMeta):
-    """An ABC that details the common operations on a private Discord channel.
-
-    The following implement this ABC:
-
-    - :class:`~discord.DMChannel`
-    - :class:`~discord.GroupChannel`
-
-    This ABC must also implement :class:`~discord.abc.Snowflake`.
-
-    Attributes
-    -----------
-    me: :class:`~discord.ClientUser`
-        The user presenting yourself.
-    """
-    __slots__ = ()
-
-    @classmethod
-    def __subclasshook__(cls, C):
-        if cls is PrivateChannel:
-            if Snowflake.__subclasshook__(C) is NotImplemented:
-                return NotImplemented
-
-            mro = C.__mro__
-            for base in mro:
-                if 'me' in base.__dict__:
-                    return True
-            return NotImplemented
-        return NotImplemented
-
-class _Overwrites:
-    __slots__ = ('id', 'allow', 'deny', 'type')
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop('id')
-        self.allow = int(kwargs.pop('allow_new', 0))
-        self.deny = int(kwargs.pop('deny_new', 0))
-        self.type = sys.intern(kwargs.pop('type'))
-
-    def _asdict(self):
-        return {
-            'id': self.id,
-            'allow': str(self.allow),
-            'deny': str(self.deny),
-            'type': self.type,
-        }
-
-class GuildChannel:
-    """An ABC that details the common operations on a Discord guild channel.
-
-    The following implement this ABC:
-
-    - :class:`~discord.TextChannel`
-    - :class:`~discord.VoiceChannel`
-    - :class:`~discord.CategoryChannel`
-    - :class:`~discord.StageChannel`
-
-    This ABC must also implement :class:`~discord.abc.Snowflake`.
-
-    Attributes
-    -----------
-    name: :class:`str`
-        The channel name.
-    guild: :class:`~discord.Guild`
-        The guild the channel belongs to.
-    position: :class:`int`
-        The position in the channel list. This is a number that starts at 0.
-        e.g. the top channel is position 0.
-    """
-    __slots__ = ()
-
-    def __str__(self):
-        return self.name
-
-    @property
-    def _sorting_bucket(self):
-        raise NotImplementedError
-
-    async def _move(self, position, parent_id=None, lock_permissions=False):
-        if position < 0:
-            raise InvalidArgument('Channel position cannot be less than 0.')
-
-        http = self._state.http
-        bucket = self._sorting_bucket
-        channels = [c for c in self.guild.channels if c._sorting_bucket == bucket]
-
-        channels.sort(key=lambda c: c.position)
-
-        try:
-            # remove ourselves from the channel list
-            channels.remove(self)
-        except ValueError:
-            # not there somehow lol
-            return
-        else:
-            index = next((i for i, c in enumerate(channels) if c.position >= position), len(channels))
-            # add ourselves at our designated position
-            channels.insert(index, self)
-
-        payload = []
-        for index, c in enumerate(channels):
-            d = {'id': c.id, 'position': index}
-            if parent_id is not _undefined and c.id == self.id:
-                d.update(parent_id=parent_id, lock_permissions=lock_permissions)
-            payload.append(d)
-
-        await http.bulk_channel_update(self.guild.id, payload)
-        self.position = position
-        if parent_id is not _undefined:
-            self.category_id = int(parent_id) if parent_id else None
-
-    async def _edit(self, options):
-        try:
-            parent = options.pop('category')
-        except KeyError:
-            parent_id = _undefined
-        else:
-            parent_id = parent and parent.id
-
-        try:
-            options['rate_limit_per_user'] = options.pop('slowmode_delay')
-        except KeyError:
-            pass
-
-        try:
-            rtc_region = options.pop('rtc_region')
-        except KeyError:
-            pass
-        else:
-            options['rtc_region'] = None if rtc_region is None else str(rtc_region)
-
-        lock_permissions = options.pop('sync_permissions', False)
-
-        try:
-            position = options.pop('position')
-        except KeyError:
-            if parent_id is not _undefined:
-                if lock_permissions:
-                    category = self.guild.get_channel(parent_id)
-                    options['permission_overwrites'] = [c._asdict() for c in category._overwrites]
-                options['parent_id'] = parent_id
-            elif lock_permissions and self.category_id is not None:
-                # if we're syncing permissions on a pre-existing channel category without changing it
-                # we need to update the permissions to point to the pre-existing category
-                category = self.guild.get_channel(self.category_id)
-                options['permission_overwrites'] = [c._asdict() for c in category._overwrites]
-        else:
-            await self._move(position, parent_id=parent_id, lock_permissions=lock_permissions)
-
-        overwrites = options.get('overwrites', None)
-        if overwrites is not None:
-            perms = []
-            for target, perm in overwrites.items():
-                if not isinstance(perm, PermissionOverwrite):
-                    raise InvalidArgument('Expected PermissionOverwrite received {0.__name__}'.format(type(perm)))
-
-                allow, deny = perm.pair()
-                payload = {
-                    'allow': allow.value,
-                    'deny': deny.value,
-                    'id': target.id
-                }
-
-                if isinstance(target, Role):
-                    payload['type'] = 'role'
-                else:
-                    payload['type'] = 'member'
-
-                perms.append(payload)
-            options['permission_overwrites'] = perms
-
-        try:
-            ch_type = options['type']
-        except KeyError:
-            pass
-        else:
-            if not isinstance(ch_type, ChannelType):
-                raise InvalidArgument('type field must be of type ChannelType')
-            options['type'] = ch_type.value
-
-        if options:
-            data = await self._state.http.edit_channel(self.id, **options)
-            self._update(self.guild, data)
-
-    def _fill_overwrites(self, data):
-        self._overwrites = []
-        everyone_index = 0
-        everyone_id = self.guild.id
-
-        for index, overridden in enumerate(data.get('permission_overwrites', [])):
-            overridden_id = int(overridden.pop('id'))
-            self._overwrites.append(_Overwrites(id=overridden_id, **overridden))
-
-            if overridden['type'] == 'member':
-                continue
-
-            if overridden_id == everyone_id:
-                # the @everyone role is not guaranteed to be the first one
-                # in the list of permission overwrites, however the permission
-                # resolution code kind of requires that it is the first one in
-                # the list since it is special. So we need the index so we can
-                # swap it to be the first one.
-                everyone_index = index
-
-        # do the swap
-        tmp = self._overwrites
-        if tmp:
-            tmp[everyone_index], tmp[0] = tmp[0], tmp[everyone_index]
-
-    @property
-    def changed_roles(self):
-        """List[:class:`~discord.Role`]: Returns a list of roles that have been overridden from
-        their default values in the :attr:`~discord.Guild.roles` attribute."""
-        ret = []
-        g = self.guild
-        for overwrite in filter(lambda o: o.type == 'role', self._overwrites):
-            role = g.get_role(overwrite.id)
-            if role is None:
-                continue
-
-            role = copy.copy(role)
-            role.permissions.handle_overwrite(overwrite.allow, overwrite.deny)
-            ret.append(role)
-        return ret
-
-    @property
-    def mention(self):
-        """:class:`str`: The string that allows you to mention the channel."""
-        return '<#%s>' % self.id
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the channel's creation time in UTC."""
-        return utils.snowflake_time(self.id)
-
-    def overwrites_for(self, obj):
-        """Returns the channel-specific overwrites for a member or a role.
-
-        Parameters
-        -----------
-        obj: Union[:class:`~discord.Role`, :class:`~discord.abc.User`]
-            The role or user denoting
-            whose overwrite to get.
-
-        Returns
-        ---------
-        :class:`~discord.PermissionOverwrite`
-            The permission overwrites for this object.
-        """
-
-        if isinstance(obj, User):
-            predicate = lambda p: p.type == 'member'
-        elif isinstance(obj, Role):
-            predicate = lambda p: p.type == 'role'
-        else:
-            predicate = lambda p: True
-
-        for overwrite in filter(predicate, self._overwrites):
-            if overwrite.id == obj.id:
-                allow = Permissions(overwrite.allow)
-                deny = Permissions(overwrite.deny)
-                return PermissionOverwrite.from_pair(allow, deny)
-
-        return PermissionOverwrite()
-
-    @property
-    def overwrites(self):
-        """Returns all of the channel's overwrites.
-
-        This is returned as a dictionary where the key contains the target which
-        can be either a :class:`~discord.Role` or a :class:`~discord.Member` and the value is the
-        overwrite as a :class:`~discord.PermissionOverwrite`.
-
-        Returns
-        --------
-        Mapping[Union[:class:`~discord.Role`, :class:`~discord.Member`], :class:`~discord.PermissionOverwrite`]
-            The channel's permission overwrites.
-        """
-        ret = {}
-        for ow in self._overwrites:
-            allow = Permissions(ow.allow)
-            deny = Permissions(ow.deny)
-            overwrite = PermissionOverwrite.from_pair(allow, deny)
-
-            if ow.type == 'role':
-                target = self.guild.get_role(ow.id)
-            elif ow.type == 'member':
-                target = self.guild.get_member(ow.id)
-
-            # TODO: There is potential data loss here in the non-chunked
-            # case, i.e. target is None because get_member returned nothing.
-            # This can be fixed with a slight breaking change to the return type,
-            # i.e. adding discord.Object to the list of it
-            # However, for now this is an acceptable compromise.
-            if target is not None:
-                ret[target] = overwrite
-        return ret
-
-    @property
-    def category(self):
-        """Optional[:class:`~discord.CategoryChannel`]: The category this channel belongs to.
-
-        If there is no category then this is ``None``.
-        """
-        return self.guild.get_channel(self.category_id)
-
-    @property
-    def permissions_synced(self):
-        """:class:`bool`: Whether or not the permissions for this channel are synced with the
-        category it belongs to.
-
-        If there is no category then this is ``False``.
-
-        .. versionadded:: 1.3
-        """
-        category = self.guild.get_channel(self.category_id)
-        return bool(category and category.overwrites == self.overwrites)
-
-    def permissions_for(self, member):
-        """Handles permission resolution for the current :class:`~discord.Member`.
-
-        This function takes into consideration the following cases:
-
-        - Guild owner
-        - Guild roles
-        - Channel overrides
-        - Member overrides
-
-        Parameters
-        ----------
-        member: :class:`~discord.Member`
-            The member to resolve permissions for.
-
-        Returns
-        -------
-        :class:`~discord.Permissions`
-            The resolved permissions for the member.
-        """
-
-        # The current cases can be explained as:
-        # Guild owner get all permissions -- no questions asked. Otherwise...
-        # The @everyone role gets the first application.
-        # After that, the applied roles that the user has in the channel
-        # (or otherwise) are then OR'd together.
-        # After the role permissions are resolved, the member permissions
-        # have to take into effect.
-        # After all that is done.. you have to do the following:
-
-        # If manage permissions is True, then all permissions are set to True.
-
-        # The operation first takes into consideration the denied
-        # and then the allowed.
-
-        if self.guild.owner_id == member.id:
-            return Permissions.all()
-
-        default = self.guild.default_role
-        base = Permissions(default.permissions.value)
-        roles = member._roles
-        get_role = self.guild.get_role
-
-        # Apply guild roles that the member has.
-        for role_id in roles:
-            role = get_role(role_id)
-            if role is not None:
-                base.value |= role._permissions
-
-        # Guild-wide Administrator -> True for everything
-        # Bypass all channel-specific overrides
-        if base.administrator:
-            return Permissions.all()
-
-        # Apply @everyone allow/deny first since it's special
-        try:
-            maybe_everyone = self._overwrites[0]
-            if maybe_everyone.id == self.guild.id:
-                base.handle_overwrite(allow=maybe_everyone.allow, deny=maybe_everyone.deny)
-                remaining_overwrites = self._overwrites[1:]
-            else:
-                remaining_overwrites = self._overwrites
-        except IndexError:
-            remaining_overwrites = self._overwrites
-
-        denies = 0
-        allows = 0
-
-        # Apply channel specific role permission overwrites
-        for overwrite in remaining_overwrites:
-            if overwrite.type == 'role' and roles.has(overwrite.id):
-                denies |= overwrite.deny
-                allows |= overwrite.allow
-
-        base.handle_overwrite(allow=allows, deny=denies)
-
-        # Apply member specific permission overwrites
-        for overwrite in remaining_overwrites:
-            if overwrite.type == 'member' and overwrite.id == member.id:
-                base.handle_overwrite(allow=overwrite.allow, deny=overwrite.deny)
-                break
-
-        # if you can't send a message in a channel then you can't have certain
-        # permissions as well
-        if not base.send_messages:
-            base.send_tts_messages = False
-            base.mention_everyone = False
-            base.embed_links = False
-            base.attach_files = False
-
-        # if you can't read a channel then you have no permissions there
-        if not base.read_messages:
-            denied = Permissions.all_channel()
-            base.value &= ~denied.value
-
-        return base
-
-    async def delete(self):
-        """|coro|
-
-        Deletes the channel.
-
-        You must have :attr:`~Permissions.manage_channels` permission to use this.
-
-        Raises
-        -------
-        ~discord.Forbidden
-            You do not have proper permissions to delete the channel.
-        ~discord.NotFound
-            The channel was not found or was already deleted.
-        ~discord.HTTPException
-            Deleting the channel failed.
-        """
-        await self._state.http.delete_channel(self.id)
-
-    async def set_permissions(self, target, *, overwrite=_undefined, **permissions):
-        r"""|coro|
-
-        Sets the channel specific permission overwrites for a target in the
-        channel.
-
-        The ``target`` parameter should either be a :class:`~discord.Member` or a
-        :class:`~discord.Role` that belongs to guild.
-
-        The ``overwrite`` parameter, if given, must either be ``None`` or
-        :class:`~discord.PermissionOverwrite`. For convenience, you can pass in
-        keyword arguments denoting :class:`~discord.Permissions` attributes. If this is
-        done, then you cannot mix the keyword arguments with the ``overwrite``
-        parameter.
-
-        If the ``overwrite`` parameter is ``None``, then the permission
-        overwrites are deleted.
-
-        You must have the :attr:`~Permissions.manage_roles` permission to use this.
-
-        Examples
-        ----------
-
-        Setting allow and deny: ::
-
-            await message.channel.set_permissions(message.author, read_messages=True,
-                                                                  send_messages=False)
-
-        Deleting overwrites ::
-
-            await channel.set_permissions(member, overwrite=None)
-
-        Using :class:`~discord.PermissionOverwrite` ::
-
-            overwrite = discord.PermissionOverwrite()
-            overwrite.send_messages = False
-            overwrite.read_messages = True
-            await channel.set_permissions(member, overwrite=overwrite)
-
-        Parameters
-        -----------
-        target: Union[:class:`~discord.Member`, :class:`~discord.Role`]
-            The member or role to overwrite permissions for.
-        overwrite: Optional[:class:`~discord.PermissionOverwrite`]
-            The permissions to allow and deny to the target, or ``None`` to
-            delete the overwrite.
-        \*\*permissions
-            A keyword argument list of permissions to set for ease of use.
-            Cannot be mixed with ``overwrite``.
-
-        Raises
-        -------
-        ~discord.Forbidden
-            You do not have permissions to edit channel specific permissions.
-        ~discord.HTTPException
-            Editing channel specific permissions failed.
-        ~discord.NotFound
-            The role or member being edited is not part of the guild.
-        ~discord.InvalidArgument
-            The overwrite parameter invalid or the target type was not
-            :class:`~discord.Role` or :class:`~discord.Member`.
-        """
-
-        http = self._state.http
-
-        if isinstance(target, User):
-            perm_type = 'member'
-        elif isinstance(target, Role):
-            perm_type = 'role'
-        else:
-            raise InvalidArgument('target parameter must be either Member or Role')
-
-        if isinstance(overwrite, _Undefined):
-            if len(permissions) == 0:
-                raise InvalidArgument('No overwrite provided.')
-            try:
-                overwrite = PermissionOverwrite(**permissions)
-            except (ValueError, TypeError):
-                raise InvalidArgument('Invalid permissions given to keyword arguments.')
-        else:
-            if len(permissions) > 0:
-                raise InvalidArgument('Cannot mix overwrite and keyword arguments.')
-
-        # TODO: wait for event
-
-        if overwrite is None:
-            await http.delete_channel_permissions(self.id, target.id)
-        elif isinstance(overwrite, PermissionOverwrite):
-            (allow, deny) = overwrite.pair()
-            await http.edit_channel_permissions(self.id, target.id, allow.value, deny.value, perm_type)
-        else:
-            raise InvalidArgument('Invalid overwrite type provided.')
-
-    async def _clone_impl(self, base_attrs, *, name=None):
-        base_attrs['permission_overwrites'] = [
-            x._asdict() for x in self._overwrites
-        ]
-        base_attrs['parent_id'] = self.category_id
-        base_attrs['name'] = name or self.name
-        guild_id = self.guild.id
-        cls = self.__class__
-        data = await self._state.http.create_channel(guild_id, self.type.value, **base_attrs)
-        obj = cls(state=self._state, guild=self.guild, data=data)
-
-        # temporarily add it to the cache
-        self.guild._channels[obj.id] = obj
-        return obj
-
-    async def clone(self, *, name=None):
-        """|coro|
-
-        Clones this channel. This creates a channel with the same properties
-        as this channel.
-
-        You must have the :attr:`~discord.Permissions.manage_channels` permission to
-        do this.
-
-        .. versionadded:: 1.1
-
-        Parameters
-        ------------
-        name: Optional[:class:`str`]
-            The name of the new channel. If not provided, defaults to this
-            channel name.
-
-        Raises
-        -------
-        ~discord.Forbidden
-            You do not have the proper permissions to create this channel.
-        ~discord.HTTPException
-            Creating the channel failed.
-
-        Returns
-        --------
-        :class:`.abc.GuildChannel`
-            The channel that was created.
-        """
-        raise NotImplementedError
-
-    async def move(self, **kwargs):
-        """|coro|
-
-        A rich interface to help move a channel relative to other channels.
-
-        If exact position movement is required, :meth:`edit` should be used instead.
-
-        You must have the :attr:`~discord.Permissions.manage_channels` permission to
-        do this.
-
-        .. note::
-
-            Voice channels will always be sorted below text channels.
-            This is a Discord limitation.
-
-        .. versionadded:: 1.7
-
-        Parameters
-        ------------
-        beginning: :class:`bool`
-            Whether to move the channel to the beginning of the
-            channel list (or category if given).
-            This is mutually exclusive with ``end``, ``before``, and ``after``.
-        end: :class:`bool`
-            Whether to move the channel to the end of the
-            channel list (or category if given).
-            This is mutually exclusive with ``beginning``, ``before``, and ``after``.
-        before: :class:`~discord.abc.Snowflake`
-            The channel that should be before our current channel.
-            This is mutually exclusive with ``beginning``, ``end``, and ``after``.
-        after: :class:`~discord.abc.Snowflake`
-            The channel that should be after our current channel.
-            This is mutually exclusive with ``beginning``, ``end``, and ``before``.
-        offset: :class:`int`
-            The number of channels to offset the move by. For example,
-            an offset of ``2`` with ``beginning=True`` would move
-            it 2 after the beginning. A positive number moves it below
-            while a negative number moves it above. Note that this
-            number is relative and computed after the ``beginning``,
-            ``end``, ``before``, and ``after`` parameters.
-        category: Optional[:class:`~discord.abc.Snowflake`]
-            The category to move this channel under.
-            If ``None`` is given then it moves it out of the category.
-            This parameter is ignored if moving a category channel.
-        sync_permissions: :class:`bool`
-            Whether to sync the permissions with the category (if given).
-
-        Raises
-        -------
-        InvalidArgument
-            An invalid position was given or a bad mix of arguments were passed.
-        Forbidden
-            You do not have permissions to move the channel.
-        HTTPException
-            Moving the channel failed.
-        """
-
-        if not kwargs:
-            return
-
-        beginning, end = kwargs.get('beginning'), kwargs.get('end')
-        before, after = kwargs.get('before'), kwargs.get('after')
-        offset = kwargs.get('offset', 0)
-        if sum(bool(a) for a in (beginning, end, before, after)) > 1:
-            raise InvalidArgument('Only one of [before, after, end, beginning] can be used.')
-
-        bucket = self._sorting_bucket
-        parent_id = kwargs.get('category', ...)
-        if parent_id not in (..., None):
-            parent_id = parent_id.id
-            channels = [
-                ch
-                for ch in self.guild.channels
-                if ch._sorting_bucket == bucket
-                and ch.category_id == parent_id
-            ]
-        else:
-            channels = [
-                ch
-                for ch in self.guild.channels
-                if ch._sorting_bucket == bucket
-                and ch.category_id == self.category_id
-            ]
-
-        channels.sort(key=lambda c: (c.position, c.id))
-
-        try:
-            # Try to remove ourselves from the channel list
-            channels.remove(self)
-        except ValueError:
-            # If we're not there then it's probably due to not being in the category
-            pass
-
-        index = None
-        if beginning:
-            index = 0
-        elif end:
-            index = len(channels)
-        elif before:
-            index = next((i for i, c in enumerate(channels) if c.id == before.id), None)
-        elif after:
-            index = next((i + 1 for i, c in enumerate(channels) if c.id == after.id), None)
-
-        if index is None:
-            raise InvalidArgument('Could not resolve appropriate move position')
-
-        channels.insert(max((index + offset), 0), self)
-        payload = []
-        lock_permissions = kwargs.get('sync_permissions', False)
-        for index, channel in enumerate(channels):
-            d = { 'id': channel.id, 'position': index }
-            if parent_id is not ... and channel.id == self.id:
-                d.update(parent_id=parent_id, lock_permissions=lock_permissions)
-            payload.append(d)
-
-        await self._state.http.bulk_channel_update(self.guild.id, payload)
-
-    async def create_invite(self, **fields):
-        """|coro|
-
-        Creates an instant invite from a text or voice channel.
-
-        You must have the :attr:`~Permissions.create_instant_invite` permission to
-        do this.
-
-        Parameters
-        ------------
-        max_age: :class:`int`
-            How long the invite should last in seconds. If it's 0 then the invite
-            doesn't expire. Defaults to ``0``.
-        max_uses: :class:`int`
-            How many uses the invite could be used for. If it's 0 then there
-            are unlimited uses. Defaults to ``0``.
-        temporary: :class:`bool`
-            Denotes that the invite grants temporary membership
-            (i.e. they get kicked after they disconnect). Defaults to ``False``.
-        unique: :class:`bool`
-            Indicates if a unique invite URL should be created. Defaults to True.
-            If this is set to ``False`` then it will return a previously created
-            invite.
-        validate: Unknown
-            Purpose is unknown.
-
-            .. versionadded:: 1.9
-        target_type: :class:`int`
-            Used to create application invites.
-
-            .. versionadded:: 1.9
-        target_application_id: :class:`int`
-            ID of the application.
-
-            .. versionadded:: 1.9
-
-        Raises
-        -------
-        ~discord.HTTPException
-            Invite creation failed.
-
-        ~discord.NotFound
-            The channel that was passed is a category or an invalid channel.
-
-        Returns
-        --------
-        :class:`~discord.Invite`
-            The invite that was created.
-        """
-
-        data = await self._state.http.create_invite(self.id, **fields)
-        return Invite.from_incomplete(data=data, state=self._state)
-
-    async def invites(self):
-        """|coro|
-
-        Returns a list of all active instant invites from this channel.
-
-        You must have :attr:`~Permissions.manage_channels` to get this information.
-
-        Raises
-        -------
-        ~discord.Forbidden
-            You do not have proper permissions to get the information.
-        ~discord.HTTPException
-            An error occurred while fetching the information.
-
-        Returns
-        -------
-        List[:class:`~discord.Invite`]
-            The list of invites that are currently active.
-        """
-
-        state = self._state
-        data = await state.http.invites_from_channel(self.id)
-        result = []
-
-        for invite in data:
-            invite['channel'] = self
-            invite['guild'] = self.guild
-            result.append(Invite(state=state, data=invite))
-
-        return result
-
-class Messageable(metaclass=abc.ABCMeta):
-    """An ABC that details the common operations on a model that can send messages.
-
-    The following implement this ABC:
-
-    - :class:`~discord.TextChannel`
-    - :class:`~discord.DMChannel`
-    - :class:`~discord.GroupChannel`
-    - :class:`~discord.User`
-    - :class:`~discord.Member`
-    - :class:`~discord.ext.commands.Context`
-    """
-
-    __slots__ = ()
-
-    @abc.abstractmethod
-    async def _get_channel(self):
-        raise NotImplementedError
-
-    async def send(self, content=None, *, tts=False, embed=None, file=None,
-                                          files=None, delete_after=None, nonce=None,
-                                          allowed_mentions=None, reference=None,
-                                          mention_author=None):
-        """|coro|
-
-        Sends a message to the destination with the content given.
-
-        The content must be a type that can convert to a string through ``str(content)``.
-        If the content is set to ``None`` (the default), then the ``embed`` parameter must
-        be provided.
-
-        To upload a single file, the ``file`` parameter should be used with a
-        single :class:`~discord.File` object. To upload multiple files, the ``files``
-        parameter should be used with a :class:`list` of :class:`~discord.File` objects.
-        **Specifying both parameters will lead to an exception**.
-
-        If the ``embed`` parameter is provided, it must be of type :class:`~discord.Embed` and
-        it must be a rich embed type.
-
-        Parameters
-        ------------
-        content: :class:`str`
-            The content of the message to send.
-        tts: :class:`bool`
-            Indicates if the message should be sent using text-to-speech.
-        embed: :class:`~discord.Embed`
-            The rich embed for the content.
-        file: :class:`~discord.File`
-            The file to upload.
-        files: List[:class:`~discord.File`]
-            A list of files to upload. Must be a maximum of 10.
-        nonce: :class:`int`
-            The nonce to use for sending this message. If the message was successfully sent,
-            then the message will have a nonce with this value.
-        delete_after: :class:`float`
-            If provided, the number of seconds to wait in the background
-            before deleting the message we just sent. If the deletion fails,
-            then it is silently ignored.
-        allowed_mentions: :class:`~discord.AllowedMentions`
-            Controls the mentions being processed in this message. If this is
-            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
-            The merging behaviour only overrides attributes that have been explicitly passed
-            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
-            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
-            are used instead.
-
-            .. versionadded:: 1.4
-
-        reference: Union[:class:`~discord.Message`, :class:`~discord.MessageReference`]
-            A reference to the :class:`~discord.Message` to which you are replying, this can be created using
-            :meth:`~discord.Message.to_reference` or passed directly as a :class:`~discord.Message`. You can control
-            whether this mentions the author of the referenced message using the :attr:`~discord.AllowedMentions.replied_user`
-            attribute of ``allowed_mentions`` or by setting ``mention_author``.
-
-            .. versionadded:: 1.6
-
-        mention_author: Optional[:class:`bool`]
-            If set, overrides the :attr:`~discord.AllowedMentions.replied_user` attribute of ``allowed_mentions``.
-
-            .. versionadded:: 1.6
-
-        Raises
-        --------
-        ~discord.HTTPException
-            Sending the message failed.
-        ~discord.Forbidden
-            You do not have the proper permissions to send the message.
-        ~discord.InvalidArgument
-            The ``files`` list is not of the appropriate size,
-            you specified both ``file`` and ``files``,
-            or the ``reference`` object is not a :class:`~discord.Message`
-            or :class:`~discord.MessageReference`.
-
-        Returns
-        ---------
-        :class:`~discord.Message`
-            The message that was sent.
-        """
-
-        channel = await self._get_channel()
-        state = self._state
-        content = str(content) if content is not None else None
-        if embed is not None:
-            embed = embed.to_dict()
-
-        if allowed_mentions is not None:
-            if state.allowed_mentions is not None:
-                allowed_mentions = state.allowed_mentions.merge(allowed_mentions).to_dict()
-            else:
-                allowed_mentions = allowed_mentions.to_dict()
-        else:
-            allowed_mentions = state.allowed_mentions and state.allowed_mentions.to_dict()
-
-        if mention_author is not None:
-            allowed_mentions = allowed_mentions or AllowedMentions().to_dict()
-            allowed_mentions['replied_user'] = bool(mention_author)
-
-        if reference is not None:
-            try:
-                reference = reference.to_message_reference_dict()
-            except AttributeError:
-                raise InvalidArgument('reference parameter must be Message or MessageReference') from None
-
-        if file is not None and files is not None:
-            raise InvalidArgument('cannot pass both file and files parameter to send()')
-
-        if file is not None:
-            if not isinstance(file, File):
-                raise InvalidArgument('file parameter must be File')
-
-            try:
-                data = await state.http.send_files(channel.id, files=[file], allowed_mentions=allowed_mentions,
-                                                   content=content, tts=tts, embed=embed, nonce=nonce,
-                                                   message_reference=reference)
-            finally:
-                file.close()
-
-        elif files is not None:
-            if len(files) > 10:
-                raise InvalidArgument('files parameter must be a list of up to 10 elements')
-            elif not all(isinstance(file, File) for file in files):
-                raise InvalidArgument('files parameter must be a list of File')
-
-            try:
-                data = await state.http.send_files(channel.id, files=files, content=content, tts=tts,
-                                                   embed=embed, nonce=nonce, allowed_mentions=allowed_mentions,
-                                                   message_reference=reference)
-            finally:
-                for f in files:
-                    f.close()
-        else:
-            data = await state.http.send_message(channel.id, content, tts=tts, embed=embed,
-                                                                      nonce=nonce, allowed_mentions=allowed_mentions,
-                                                                      message_reference=reference)
-
-        ret = state.create_message(channel=channel, data=data)
-        if delete_after is not None:
-            await ret.delete(delay=delete_after)
-        return ret
-
-    async def trigger_typing(self):
-        """|coro|
-
-        Triggers a *typing* indicator to the destination.
-
-        *Typing* indicator will go away after 10 seconds, or after a message is sent.
-        """
-
-        channel = await self._get_channel()
-        await self._state.http.send_typing(channel.id)
-
-    def typing(self):
-        """Returns a context manager that allows you to type for an indefinite period of time.
-
-        This is useful for denoting long computations in your bot.
-
-        .. note::
-
-            This is both a regular context manager and an async context manager.
-            This means that both ``with`` and ``async with`` work with this.
-
-        Example Usage: ::
-
-            async with channel.typing():
-                # do expensive stuff here
-                await channel.send('done!')
-
-        """
-        return Typing(self)
-
-    async def fetch_message(self, id):
-        """|coro|
-
-        Retrieves a single :class:`~discord.Message` from the destination.
-
-        Parameters
-        ------------
-        id: :class:`int`
-            The message ID to look for.
-
-        Raises
-        --------
-        ~discord.NotFound
-            The specified message was not found.
-        ~discord.Forbidden
-            You do not have the permissions required to get a message.
-        ~discord.HTTPException
-            Retrieving the message failed.
-
-        Returns
-        --------
-        :class:`~discord.Message`
-            The message asked for.
-        """
-
-        channel = await self._get_channel()
-        data = await self._state.http.get_message(channel.id, id)
-        return self._state.create_message(channel=channel, data=data)
-
-    async def pins(self):
-        """|coro|
-
-        Retrieves all messages that are currently pinned in the channel.
-
-        .. note::
-
-            Due to a limitation with the Discord API, the :class:`.Message`
-            objects returned by this method do not contain complete
-            :attr:`.Message.reactions` data.
-
-        Raises
-        -------
-        ~discord.HTTPException
-            Retrieving the pinned messages failed.
-
-        Returns
-        --------
-        List[:class:`~discord.Message`]
-            The messages that are currently pinned.
-        """
-
-        channel = await self._get_channel()
-        state = self._state
-        data = await state.http.pins_from(channel.id)
-        return [state.create_message(channel=channel, data=m) for m in data]
-
-    def history(self, *, limit=100, before=None, after=None, around=None, oldest_first=None):
-        """Returns an :class:`~discord.AsyncIterator` that enables receiving the destination's message history.
-
-        You must have :attr:`~Permissions.read_message_history` permissions to use this.
-
-        Examples
-        ---------
-
-        Usage ::
-
-            counter = 0
-            async for message in channel.history(limit=200):
-                if message.author == client.user:
-                    counter += 1
-
-        Flattening into a list: ::
-
-            messages = await channel.history(limit=123).flatten()
-            # messages is now a list of Message...
-
-        All parameters are optional.
-
-        Parameters
-        -----------
-        limit: Optional[:class:`int`]
-            The number of messages to retrieve.
-            If ``None``, retrieves every message in the channel. Note, however,
-            that this would make it a slow operation.
-        before: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
-            Retrieve messages before this date or message.
-            If a date is provided it must be a timezone-naive datetime representing UTC time.
-        after: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
-            Retrieve messages after this date or message.
-            If a date is provided it must be a timezone-naive datetime representing UTC time.
-        around: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
-            Retrieve messages around this date or message.
-            If a date is provided it must be a timezone-naive datetime representing UTC time.
-            When using this argument, the maximum limit is 101. Note that if the limit is an
-            even number then this will return at most limit + 1 messages.
-        oldest_first: Optional[:class:`bool`]
-            If set to ``True``, return messages in oldest->newest order. Defaults to ``True`` if
-            ``after`` is specified, otherwise ``False``.
-
-        Raises
-        ------
-        ~discord.Forbidden
-            You do not have permissions to get channel message history.
-        ~discord.HTTPException
-            The request to get message history failed.
-
-        Yields
-        -------
-        :class:`~discord.Message`
-            The message with the message data parsed.
-        """
-        return HistoryIterator(self, limit=limit, before=before, after=after, around=around, oldest_first=oldest_first)
-
-class Connectable(metaclass=abc.ABCMeta):
-    """An ABC that details the common operations on a channel that can
-    connect to a voice server.
-
-    The following implement this ABC:
-
-    - :class:`~discord.VoiceChannel`
-    """
-    __slots__ = ()
-
-    @abc.abstractmethod
-    def _get_voice_client_key(self):
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def _get_voice_state_pair(self):
-        raise NotImplementedError
-
-    async def connect(self, *, timeout=60.0, reconnect=True, cls=VoiceClient):
-        """|coro|
-
-        Connects to voice and creates a :class:`VoiceClient` to establish
-        your connection to the voice server.
-
-        Parameters
-        -----------
-        timeout: :class:`float`
-            The timeout in seconds to wait for the voice endpoint.
-        reconnect: :class:`bool`
-            Whether the bot should automatically attempt
-            a reconnect if a part of the handshake fails
-            or the gateway goes down.
-        cls: Type[:class:`VoiceProtocol`]
-            A type that subclasses :class:`~discord.VoiceProtocol` to connect with.
-            Defaults to :class:`~discord.VoiceClient`.
-
-        Raises
-        -------
-        asyncio.TimeoutError
-            Could not connect to the voice channel in time.
-        ~discord.ClientException
-            You are already connected to a voice channel.
-        ~discord.opus.OpusNotLoaded
-            The opus library has not been loaded.
-
-        Returns
-        --------
-        :class:`~discord.VoiceProtocol`
-            A voice client that is fully connected to the voice server.
-        """
-
-        key_id, _ = self._get_voice_client_key()
-        state = self._state
-
-        if state._get_voice_client(key_id):
-            raise ClientException('Already connected to a voice channel.')
-
-        client = state._get_client()
-        voice = cls(client, self)
-
-        if not isinstance(voice, VoiceProtocol):
-            raise TypeError('Type must meet VoiceProtocol abstract base class.')
-
-        state._add_voice_client(key_id, voice)
-
-        try:
-            await voice.connect(timeout=timeout, reconnect=reconnect)
-        except asyncio.TimeoutError:
-            try:
-                await voice.disconnect(force=True)
-            except Exception:
-                # we don't care if disconnect failed because connection failed
-                pass
-            raise # re-raise
-
-        return voice
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+import array
+import asyncio
+from typing import (
+    Any,
+    AsyncIterable,
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Collection,
+    Coroutine,
+    Dict,
+    ForwardRef,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Literal,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Protocol,
+    Set,
+    Sequence,
+    SupportsIndex,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+    TYPE_CHECKING,
+)
+import collections
+import unicodedata
+from base64 import b64encode
+from bisect import bisect_left
+import datetime
+import functools
+from inspect import isawaitable as _isawaitable, signature as _signature
+from operator import attrgetter
+from urllib.parse import urlencode
+import json
+import logging
+import os
+import random
+import re
+import string
+import sys
+from threading import Timer
+import types
+import warnings
+import logging
+
+import yarl
+
+try:
+    import orjson  # type: ignore
+except ModuleNotFoundError:
+    HAS_ORJSON = False
+else:
+    HAS_ORJSON = True
+
+from .enums import Locale, try_enum
+
+
+__all__ = (
+    'oauth_url',
+    'snowflake_time',
+    'time_snowflake',
+    'find',
+    'get',
+    'sleep_until',
+    'utcnow',
+    'remove_markdown',
+    'escape_markdown',
+    'escape_mentions',
+    'maybe_coroutine',
+    'as_chunks',
+    'format_dt',
+    'set_target',
+    'MISSING',
+    'setup_logging',
+)
+
+DISCORD_EPOCH = 1420070400000
+
+_log = logging.getLogger(__name__)
+
+
+class _MissingSentinel:
+    __slots__ = ()
+
+    def __eq__(self, other):
+        return False
+
+    def __bool__(self):
+        return False
+
+    def __hash__(self):
+        return 0
+
+    def __repr__(self):
+        return '...'
+
+
+MISSING: Any = _MissingSentinel()
+
+
+class _cached_property:
+    def __init__(self, function):
+        self.function = function
+        self.__doc__ = getattr(function, '__doc__')
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+
+        value = self.function(instance)
+        setattr(instance, self.function.__name__, value)
+
+        return value
+
+
+if TYPE_CHECKING:
+    from aiohttp import ClientSession
+    from functools import cached_property as cached_property
+
+    from typing_extensions import ParamSpec, Self, TypeGuard
+
+    from .permissions import Permissions
+    from .abc import Messageable, Snowflake
+    from .invite import Invite
+    from .message import Message
+    from .template import Template
+    from .commands import ApplicationCommand
+    from .entitlements import Gift
+
+    class _RequestLike(Protocol):
+        headers: Mapping[str, Any]
+
+    P = ParamSpec('P')
+
+    MaybeAwaitableFunc = Callable[P, 'MaybeAwaitable[T]']
+
+    _SnowflakeListBase = array.array[int]
+
+else:
+    cached_property = _cached_property
+    _SnowflakeListBase = array.array
+
+
+T = TypeVar('T')
+T_co = TypeVar('T_co', covariant=True)
+_Iter = Union[Iterable[T], AsyncIterable[T]]
+Coro = Coroutine[Any, Any, T]
+MaybeAwaitable = Union[T, Awaitable[T]]
+
+
+class CachedSlotProperty(Generic[T, T_co]):
+    def __init__(self, name: str, function: Callable[[T], T_co]) -> None:
+        self.name = name
+        self.function = function
+        self.__doc__ = getattr(function, '__doc__')
+
+    @overload
+    def __get__(self, instance: None, owner: Type[T]) -> CachedSlotProperty[T, T_co]:
+        ...
+
+    @overload
+    def __get__(self, instance: T, owner: Type[T]) -> T_co:
+        ...
+
+    def __get__(self, instance: Optional[T], owner: Type[T]) -> Any:
+        if instance is None:
+            return self
+
+        try:
+            return getattr(instance, self.name)
+        except AttributeError:
+            value = self.function(instance)
+            setattr(instance, self.name, value)
+            return value
+
+
+class classproperty(Generic[T_co]):
+    def __init__(self, fget: Callable[[Any], T_co]) -> None:
+        self.fget = fget
+
+    def __get__(self, instance: Optional[Any], owner: Type[Any]) -> T_co:
+        return self.fget(owner)
+
+    def __set__(self, instance: Optional[Any], value: Any) -> None:
+        raise AttributeError('cannot set attribute')
+
+
+def cached_slot_property(name: str) -> Callable[[Callable[[T], T_co]], CachedSlotProperty[T, T_co]]:
+    def decorator(func: Callable[[T], T_co]) -> CachedSlotProperty[T, T_co]:
+        return CachedSlotProperty(name, func)
+
+    return decorator
+
+
+class SequenceProxy(Sequence[T_co]):
+    """A proxy of a sequence that only creates a copy when necessary."""
+
+    def __init__(self, proxied: Collection[T_co], *, sorted: bool = False):
+        self.__proxied: Collection[T_co] = proxied
+        self.__sorted: bool = sorted
+
+    @cached_property
+    def __copied(self) -> List[T_co]:
+        if self.__sorted:
+            # The type checker thinks the variance is wrong, probably due to the comparison requirements
+            self.__proxied = sorted(self.__proxied)  # type: ignore
+        else:
+            self.__proxied = list(self.__proxied)
+        return self.__proxied
+
+    def __repr__(self) -> str:
+        return f"SequenceProxy({self.__proxied!r})"
+
+    @overload
+    def __getitem__(self, idx: SupportsIndex) -> T_co:
+        ...
+
+    @overload
+    def __getitem__(self, idx: slice) -> List[T_co]:
+        ...
+
+    def __getitem__(self, idx: Union[SupportsIndex, slice]) -> Union[T_co, List[T_co]]:
+        return self.__copied[idx]
+
+    def __len__(self) -> int:
+        return len(self.__proxied)
+
+    def __contains__(self, item: Any) -> bool:
+        return item in self.__copied
+
+    def __iter__(self) -> Iterator[T_co]:
+        return iter(self.__copied)
+
+    def __reversed__(self) -> Iterator[T_co]:
+        return reversed(self.__copied)
+
+    def index(self, value: Any, *args: Any, **kwargs: Any) -> int:
+        return self.__copied.index(value, *args, **kwargs)
+
+    def count(self, value: Any) -> int:
+        return self.__copied.count(value)
+
+
+@overload
+def parse_time(timestamp: None) -> None:
+    ...
+
+
+@overload
+def parse_time(timestamp: str) -> datetime.datetime:
+    ...
+
+
+@overload
+def parse_time(timestamp: Optional[str]) -> Optional[datetime.datetime]:
+    ...
+
+
+def parse_time(timestamp: Optional[str]) -> Optional[datetime.datetime]:
+    if timestamp:
+        return datetime.datetime.fromisoformat(timestamp)
+    return None
+
+
+@overload
+def parse_date(date: None) -> None:
+    ...
+
+
+@overload
+def parse_date(date: str) -> datetime.date:
+    ...
+
+
+@overload
+def parse_date(date: Optional[str]) -> Optional[datetime.date]:
+    ...
+
+
+def parse_date(date: Optional[str]) -> Optional[datetime.date]:
+    if date:
+        return parse_time(date).date()
+    return None
+
+
+@overload
+def parse_timestamp(timestamp: None) -> None:
+    ...
+
+
+@overload
+def parse_timestamp(timestamp: float) -> datetime.datetime:
+    ...
+
+
+@overload
+def parse_timestamp(timestamp: Optional[float]) -> Optional[datetime.datetime]:
+    ...
+
+
+def parse_timestamp(timestamp: Optional[float]) -> Optional[datetime.datetime]:
+    if timestamp:
+        return datetime.datetime.fromtimestamp(timestamp / 1000.0, tz=datetime.timezone.utc)
+
+
+def copy_doc(original: Callable[..., Any]) -> Callable[[T], T]:
+    def decorator(overridden: T) -> T:
+        overridden.__doc__ = original.__doc__
+        overridden.__signature__ = _signature(original)  # type: ignore
+        return overridden
+
+    return decorator
+
+
+def deprecated(instead: Optional[str] = None) -> Callable[[Callable[P, T]], Callable[P, T]]:
+    def actual_decorator(func: Callable[P, T]) -> Callable[P, T]:
+        @functools.wraps(func)
+        def decorated(*args: P.args, **kwargs: P.kwargs) -> T:
+            warnings.simplefilter('always', DeprecationWarning)  # turn off filter
+            if instead:
+                fmt = "{0.__name__} is deprecated, use {1} instead."
+            else:
+                fmt = '{0.__name__} is deprecated.'
+
+            warnings.warn(fmt.format(func, instead), stacklevel=3, category=DeprecationWarning)
+            warnings.simplefilter('default', DeprecationWarning)  # reset filter
+            return func(*args, **kwargs)
+
+        return decorated
+
+    return actual_decorator
+
+
+def oauth_url(
+    client_id: Union[int, str],
+    *,
+    permissions: Permissions = MISSING,
+    guild: Snowflake = MISSING,
+    redirect_uri: str = MISSING,
+    scopes: Iterable[str] = MISSING,
+    disable_guild_select: bool = False,
+    state: str = MISSING,
+) -> str:
+    """A helper function that returns the OAuth2 URL for inviting a bot
+    into guilds.
+
+    .. versionchanged:: 2.0
+
+        ``permissions``, ``guild``, ``redirect_uri``, ``scopes`` and ``state`` parameters
+        are now keyword-only.
+
+    Parameters
+    -----------
+    client_id: Union[:class:`int`, :class:`str`]
+        The client ID for the bot.
+    permissions: :class:`~discord.Permissions`
+        The permissions you're requesting. If not given then you won't be requesting any
+        permissions.
+    guild: :class:`~discord.abc.Snowflake`
+        The guild to pre-select in the authorization screen, if available.
+    redirect_uri: :class:`str`
+        An optional valid redirect URI.
+    scopes: Iterable[:class:`str`]
+        An optional valid list of scopes. Defaults to ``('bot', 'applications.commands')``.
+
+        .. versionadded:: 1.7
+    disable_guild_select: :class:`bool`
+        Whether to disallow the user from changing the guild dropdown.
+
+        .. versionadded:: 2.0
+    state: :class:`str`
+        The state to return after the authorization.
+
+        .. versionadded:: 2.0
+
+    Returns
+    --------
+    :class:`str`
+        The OAuth2 URL for inviting the bot into guilds.
+    """
+    url = f'https://discord.com/oauth2/authorize?client_id={client_id}'
+    url += '&scope=' + '+'.join(scopes or ('bot', 'applications.commands'))
+    if permissions is not MISSING:
+        url += f'&permissions={permissions.value}'
+    if guild is not MISSING:
+        url += f'&guild_id={guild.id}'
+    if disable_guild_select:
+        url += '&disable_guild_select=true'
+    if redirect_uri is not MISSING:
+        url += '&response_type=code&' + urlencode({'redirect_uri': redirect_uri})
+    if state is not MISSING:
+        url += f'&{urlencode({"state": state})}'
+    return url
+
+
+def snowflake_time(id: int, /) -> datetime.datetime:
+    """Returns the creation time of the given snowflake.
+
+    .. versionchanged:: 2.0
+        The ``id`` parameter is now positional-only.
+
+    Parameters
+    -----------
+    id: :class:`int`
+        The snowflake ID.
+
+    Returns
+    --------
+    :class:`datetime.datetime`
+        An aware datetime in UTC representing the creation time of the snowflake.
+    """
+    timestamp = ((id >> 22) + DISCORD_EPOCH) / 1000
+    return datetime.datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc)
+
+
+def time_snowflake(dt: datetime.datetime, /, *, high: bool = False) -> int:
+    """Returns a numeric snowflake pretending to be created at the given date.
+
+    When using as the lower end of a range, use ``time_snowflake(dt, high=False) - 1``
+    to be inclusive, ``high=True`` to be exclusive.
+
+    When using as the higher end of a range, use ``time_snowflake(dt, high=True) + 1``
+    to be inclusive, ``high=False`` to be exclusive.
+
+    .. versionchanged:: 2.0
+        The ``high`` parameter is now keyword-only and the ``dt`` parameter is now
+        positional-only.
+
+    Parameters
+    -----------
+    dt: :class:`datetime.datetime`
+        A datetime object to convert to a snowflake.
+        If naive, the timezone is assumed to be local time.
+    high: :class:`bool`
+        Whether or not to set the lower 22 bit to high or low.
+
+    Returns
+    --------
+    :class:`int`
+        The snowflake representing the time given.
+    """
+    discord_millis = int(dt.timestamp() * 1000 - DISCORD_EPOCH)
+    return (discord_millis << 22) + (2**22 - 1 if high else 0)
+
+
+def _find(predicate: Callable[[T], Any], iterable: Iterable[T], /) -> Optional[T]:
+    return next((element for element in iterable if predicate(element)), None)
+
+
+async def _afind(predicate: Callable[[T], Any], iterable: AsyncIterable[T], /) -> Optional[T]:
+    async for element in iterable:
+        if predicate(element):
+            return element
+
+    return None
+
+
+@overload
+def find(predicate: Callable[[T], Any], iterable: AsyncIterable[T], /) -> Coro[Optional[T]]:
+    ...
+
+
+@overload
+def find(predicate: Callable[[T], Any], iterable: Iterable[T], /) -> Optional[T]:
+    ...
+
+
+def find(predicate: Callable[[T], Any], iterable: _Iter[T], /) -> Union[Optional[T], Coro[Optional[T]]]:
+    r"""A helper to return the first element found in the sequence
+    that meets the predicate. For example: ::
+
+        member = discord.utils.find(lambda m: m.name == 'Mighty', channel.guild.members)
+
+    would find the first :class:`~discord.Member` whose name is 'Mighty' and return it.
+    If an entry is not found, then ``None`` is returned.
+
+    This is different from :func:`py:filter` due to the fact it stops the moment it finds
+    a valid entry.
+
+    .. versionchanged:: 2.0
+
+        Both parameters are now positional-only.
+
+    .. versionchanged:: 2.0
+
+        The ``iterable`` parameter supports :term:`asynchronous iterable`\s.
+
+    Parameters
+    -----------
+    predicate
+        A function that returns a boolean-like result.
+    iterable: Union[:class:`collections.abc.Iterable`, :class:`collections.abc.AsyncIterable`]
+        The iterable to search through. Using a :class:`collections.abc.AsyncIterable`,
+        makes this function return a :term:`coroutine`.
+    """
+
+    return (
+        _afind(predicate, iterable)  # type: ignore
+        if hasattr(iterable, '__aiter__')  # isinstance(iterable, collections.abc.AsyncIterable) is too slow
+        else _find(predicate, iterable)  # type: ignore
+    )
+
+
+def _get(iterable: Iterable[T], /, **attrs: Any) -> Optional[T]:
+    # global -> local
+    _all = all
+    attrget = attrgetter
+
+    # Special case the single element call
+    if len(attrs) == 1:
+        k, v = attrs.popitem()
+        pred = attrget(k.replace('__', '.'))
+        return next((elem for elem in iterable if pred(elem) == v), None)
+
+    converted = [(attrget(attr.replace('__', '.')), value) for attr, value in attrs.items()]
+    for elem in iterable:
+        if _all(pred(elem) == value for pred, value in converted):
+            return elem
+    return None
+
+
+async def _aget(iterable: AsyncIterable[T], /, **attrs: Any) -> Optional[T]:
+    # global -> local
+    _all = all
+    attrget = attrgetter
+
+    # Special case the single element call
+    if len(attrs) == 1:
+        k, v = attrs.popitem()
+        pred = attrget(k.replace('__', '.'))
+        async for elem in iterable:
+            if pred(elem) == v:
+                return elem
+        return None
+
+    converted = [(attrget(attr.replace('__', '.')), value) for attr, value in attrs.items()]
+
+    async for elem in iterable:
+        if _all(pred(elem) == value for pred, value in converted):
+            return elem
+    return None
+
+
+@overload
+def get(iterable: AsyncIterable[T], /, **attrs: Any) -> Coro[Optional[T]]:
+    ...
+
+
+@overload
+def get(iterable: Iterable[T], /, **attrs: Any) -> Optional[T]:
+    ...
+
+
+def get(iterable: _Iter[T], /, **attrs: Any) -> Union[Optional[T], Coro[Optional[T]]]:
+    r"""A helper that returns the first element in the iterable that meets
+    all the traits passed in ``attrs``. This is an alternative for
+    :func:`~discord.utils.find`.
+
+    When multiple attributes are specified, they are checked using
+    logical AND, not logical OR. Meaning they have to meet every
+    attribute passed in and not one of them.
+
+    To have a nested attribute search (i.e. search by ``x.y``) then
+    pass in ``x__y`` as the keyword argument.
+
+    If nothing is found that matches the attributes passed, then
+    ``None`` is returned.
+
+    .. versionchanged:: 2.0
+
+        The ``iterable`` parameter is now positional-only.
+
+    .. versionchanged:: 2.0
+
+        The ``iterable`` parameter supports :term:`asynchronous iterable`\s.
+
+    Examples
+    ---------
+
+    Basic usage:
+
+    .. code-block:: python3
+
+        member = discord.utils.get(message.guild.members, name='Foo')
+
+    Multiple attribute matching:
+
+    .. code-block:: python3
+
+        channel = discord.utils.get(guild.voice_channels, name='Foo', bitrate=64000)
+
+    Nested attribute matching:
+
+    .. code-block:: python3
+
+        channel = discord.utils.get(client.get_all_channels(), guild__name='Cool', name='general')
+
+    Async iterables:
+
+    .. code-block:: python3
+
+        msg = await discord.utils.get(channel.history(), author__name='Dave')
+
+    Parameters
+    -----------
+    iterable: Union[:class:`collections.abc.Iterable`, :class:`collections.abc.AsyncIterable`]
+        The iterable to search through. Using a :class:`collections.abc.AsyncIterable`,
+        makes this function return a :term:`coroutine`.
+    \*\*attrs
+        Keyword arguments that denote attributes to search with.
+    """
+
+    return (
+        _aget(iterable, **attrs)  # type: ignore
+        if hasattr(iterable, '__aiter__')  # isinstance(iterable, collections.abc.AsyncIterable) is too slow
+        else _get(iterable, **attrs)  # type: ignore
+    )
+
+
+def _unique(iterable: Iterable[T]) -> List[T]:
+    return [x for x in dict.fromkeys(iterable)]
+
+
+def _get_as_snowflake(data: Any, key: str) -> Optional[int]:
+    try:
+        value = data[key]
+    except KeyError:
+        return None
+    else:
+        return value and int(value)
+
+
+def _ocast(value: Any, type: Any):
+    if value is MISSING:
+        return MISSING
+    return type(value)
+
+
+def _get_mime_type_for_image(data: bytes, with_video: bool = False, fallback: bool = False) -> str:
+    if data.startswith(b'\x89\x50\x4E\x47\x0D\x0A\x1A\x0A'):
+        return 'image/png'
+    elif data[0:3] == b'\xff\xd8\xff' or data[6:10] in (b'JFIF', b'Exif'):
+        return 'image/jpeg'
+    elif data.startswith((b'\x47\x49\x46\x38\x37\x61', b'\x47\x49\x46\x38\x39\x61')):
+        return 'image/gif'
+    elif data.startswith(b'RIFF') and data[8:12] == b'WEBP':
+        return 'image/webp'
+    elif data.startswith(b'\x66\x74\x79\x70\x69\x73\x6F\x6D') and with_video:
+        return 'video/mp4'
+    else:
+        if fallback:
+            return 'application/octet-stream'
+        raise ValueError('Unsupported image type given')
+
+
+def _get_extension_for_mime_type(mime_type: str) -> str:
+    if mime_type == 'image/png':
+        return 'png'
+    elif mime_type == 'image/jpeg':
+        return 'jpg'
+    elif mime_type == 'image/gif':
+        return 'gif'
+    elif mime_type == 'video/mp4':
+        return 'mp4'
+    else:
+        return 'webp'
+
+
+def _bytes_to_base64_data(data: bytes) -> str:
+    fmt = 'data:{mime};base64,{data}'
+    mime = _get_mime_type_for_image(data, fallback=True)
+    b64 = b64encode(data).decode('ascii')
+    return fmt.format(mime=mime, data=b64)
+
+
+def _is_submodule(parent: str, child: str) -> bool:
+    return parent == child or child.startswith(parent + '.')
+
+
+def _handle_metadata(obj):
+    try:
+        return dict(obj)
+    except Exception:
+        raise TypeError(f'Type {obj.__class__.__name__} is not JSON serializable')
+
+
+if HAS_ORJSON:
+
+    def _to_json(obj: Any) -> str:
+        return orjson.dumps(obj, default=_handle_metadata).decode('utf-8')
+
+    _from_json = orjson.loads  # type: ignore
+
+else:
+
+    def _to_json(obj: Any) -> str:
+        return json.dumps(obj, separators=(',', ':'), ensure_ascii=True, default=_handle_metadata)
+
+    _from_json = json.loads
+
+
+def _parse_ratelimit_header(request: Any, *, use_clock: bool = False) -> float:
+    reset_after: Optional[str] = request.headers.get('X-Ratelimit-Reset-After')
+    if use_clock or not reset_after:
+        utc = datetime.timezone.utc
+        now = datetime.datetime.now(utc)
+        reset = datetime.datetime.fromtimestamp(float(request.headers['X-Ratelimit-Reset']), utc)
+        return (reset - now).total_seconds()
+    else:
+        return float(reset_after)
+
+
+async def maybe_coroutine(f: MaybeAwaitableFunc[P, T], *args: P.args, **kwargs: P.kwargs) -> T:
+    r"""|coro|
+
+    A helper function that will await the result of a function if it's a coroutine
+    or return the result if it's not.
+
+    This is useful for functions that may or may not be coroutines.
+
+    .. versionadded:: 2.0
+
+    Parameters
+    -----------
+    f: Callable[..., Any]
+        The function or coroutine to call.
+    \*args
+        The arguments to pass to the function.
+    \*\*kwargs
+        The keyword arguments to pass to the function.
+
+    Returns
+    --------
+    Any
+        The result of the function or coroutine.
+    """
+
+    value = f(*args, **kwargs)
+    if _isawaitable(value):
+        return await value
+    else:
+        return value  # type: ignore
+
+
+async def async_all(
+    gen: Iterable[Union[T, Awaitable[T]]],
+    *,
+    check: Callable[[Union[T, Awaitable[T]]], TypeGuard[Awaitable[T]]] = _isawaitable,
+) -> bool:
+    for elem in gen:
+        if check(elem):
+            elem = await elem
+        if not elem:
+            return False
+    return True
+
+
+async def sane_wait_for(futures: Iterable[Awaitable[T]], *, timeout: Optional[float]) -> Set[asyncio.Task[T]]:
+    ensured = [asyncio.ensure_future(fut) for fut in futures]
+    done, pending = await asyncio.wait(ensured, timeout=timeout, return_when=asyncio.ALL_COMPLETED)
+
+    if len(pending) != 0:
+        raise asyncio.TimeoutError()
+
+    return done
+
+
+def get_slots(cls: Type[Any]) -> Iterator[str]:
+    for mro in reversed(cls.__mro__):
+        try:
+            yield from mro.__slots__  # type: ignore
+        except AttributeError:
+            continue
+
+
+def compute_timedelta(dt: datetime.datetime) -> float:
+    if dt.tzinfo is None:
+        dt = dt.astimezone()
+    now = datetime.datetime.now(datetime.timezone.utc)
+    return max((dt - now).total_seconds(), 0)
+
+
+@overload
+async def sleep_until(when: datetime.datetime, result: T) -> T:
+    ...
+
+
+@overload
+async def sleep_until(when: datetime.datetime) -> None:
+    ...
+
+
+async def sleep_until(when: datetime.datetime, result: Optional[T] = None) -> Optional[T]:
+    """|coro|
+
+    Sleep until a specified time.
+
+    If the time supplied is in the past this function will yield instantly.
+
+    .. versionadded:: 1.3
+
+    Parameters
+    -----------
+    when: :class:`datetime.datetime`
+        The timestamp in which to sleep until. If the datetime is naive then
+        it is assumed to be local time.
+    result: Any
+        If provided is returned to the caller when the coroutine completes.
+    """
+    delta = compute_timedelta(when)
+    return await asyncio.sleep(delta, result)
+
+
+def utcnow() -> datetime.datetime:
+    """A helper function to return an aware UTC datetime representing the current time.
+
+    This should be preferred to :meth:`datetime.datetime.utcnow` since it is an aware
+    datetime, compared to the naive datetime in the standard library.
+
+    .. versionadded:: 2.0
+
+    Returns
+    --------
+    :class:`datetime.datetime`
+        The current aware datetime in UTC.
+    """
+    return datetime.datetime.now(datetime.timezone.utc)
+
+
+def valid_icon_size(size: int) -> bool:
+    """Icons must be power of 2 within [16, 4096]."""
+    ADDITIONAL_SIZES = (20, 22, 24, 28, 40, 44, 48, 56, 60, 80, 96, 100, 160, 240, 300, 320, 480, 600, 640, 1280, 1536, 3072)
+    return (not size & (size - 1) and 4096 >= size >= 16) or size in ADDITIONAL_SIZES
+
+
+class SnowflakeList(_SnowflakeListBase):
+    """Internal data storage class to efficiently store a list of snowflakes.
+
+    This should have the following characteristics:
+
+    - Low memory usage
+    - O(n) iteration (obviously)
+    - O(n log n) initial creation if data is unsorted
+    - O(log n) search and indexing
+    - O(n) insertion
+    """
+
+    __slots__ = ()
+
+    if TYPE_CHECKING:
+
+        def __init__(self, data: Iterable[int], *, is_sorted: bool = False):
+            ...
+
+    def __new__(cls, data: Iterable[int], *, is_sorted: bool = False) -> Self:
+        return array.array.__new__(cls, 'Q', data if is_sorted else sorted(data))  # type: ignore
+
+    def add(self, element: int) -> None:
+        i = bisect_left(self, element)
+        self.insert(i, element)
+
+    def get(self, element: int) -> Optional[int]:
+        i = bisect_left(self, element)
+        return self[i] if i != len(self) and self[i] == element else None
+
+    def has(self, element: int) -> bool:
+        i = bisect_left(self, element)
+        return i != len(self) and self[i] == element
+
+
+_IS_ASCII = re.compile(r'^[\x00-\x7f]+$')
+
+
+def _string_width(string: str, *, _IS_ASCII=_IS_ASCII) -> int:
+    """Returns string's width."""
+    match = _IS_ASCII.match(string)
+    if match:
+        return match.endpos
+
+    UNICODE_WIDE_CHAR_TYPE = 'WFA'
+    func = unicodedata.east_asian_width
+    return sum(2 if func(char) in UNICODE_WIDE_CHAR_TYPE else 1 for char in string)
+
+
+class ResolvedInvite(NamedTuple):
+    code: str
+    event: Optional[int]
+
+
+def resolve_invite(invite: Union[Invite, str]) -> ResolvedInvite:
+    """Resolves an invite from a :class:`~discord.Invite`, URL or code.
+
+    .. versionchanged:: 2.0
+        Now returns a :class:`.ResolvedInvite` instead of a
+        :class:`str`.
+
+    Parameters
+    -----------
+    invite: Union[:class:`~discord.Invite`, :class:`str`]
+        The invite.
+
+    Returns
+    --------
+    :class:`.ResolvedInvite`
+        A data class containing the invite code and the event ID.
+    """
+    from .invite import Invite  # circular import
+
+    if isinstance(invite, Invite):
+        return ResolvedInvite(invite.code, invite.scheduled_event_id)
+    else:
+        rx = r'(?:https?\:\/\/)?discord(?:\.gg|(?:app)?\.com\/invite)\/[^/]+'
+        m = re.match(rx, invite)
+
+        if m:
+            url = yarl.URL(invite)
+            code = url.parts[-1]
+            event_id = url.query.get('event')
+
+            return ResolvedInvite(code, int(event_id) if event_id else None)
+    return ResolvedInvite(invite, None)
+
+
+def resolve_template(code: Union[Template, str]) -> str:
+    """
+    Resolves a template code from a :class:`~discord.Template`, URL or code.
+
+    .. versionadded:: 1.4
+
+    Parameters
+    -----------
+    code: Union[:class:`~discord.Template`, :class:`str`]
+        The code.
+
+    Returns
+    --------
+    :class:`str`
+        The template code.
+    """
+    from .template import Template  # circular import
+
+    if isinstance(code, Template):
+        return code.code
+    else:
+        rx = r'(?:https?\:\/\/)?discord(?:\.new|(?:app)?\.com\/template)\/(.+)'
+        m = re.match(rx, code)
+        if m:
+            return m.group(1)
+    return code
+
+
+def resolve_gift(code: Union[Gift, str]) -> str:
+    """
+    Resolves a gift code from a :class:`~discord.Gift`, URL or code.
+
+    .. versionadded:: 2.0
+
+    Parameters
+    -----------
+    code: Union[:class:`~discord.Gift`, :class:`str`]
+        The code.
+
+    Returns
+    --------
+    :class:`str`
+        The gift code.
+    """
+    from .entitlements import Gift  # circular import
+
+    if isinstance(code, Gift):
+        return code.code
+    else:
+        rx = r'(?:https?\:\/\/)?(?:discord(?:app)?\.com\/(?:gifts|billing\/promotions)|promos\.discord\.gg|discord.gift)\/(.+)'
+        m = re.match(rx, code)
+        if m:
+            return m.group(1)
+    return code
+
+
+_MARKDOWN_ESCAPE_SUBREGEX = '|'.join(r'\{0}(?=([\s\S]*((?<!\{0})\{0})))'.format(c) for c in ('*', '`', '_', '~', '|'))
+
+_MARKDOWN_ESCAPE_COMMON = r'^>(?:>>)?\s|\[.+\]\(.+\)'
+
+_MARKDOWN_ESCAPE_REGEX = re.compile(fr'(?P<markdown>{_MARKDOWN_ESCAPE_SUBREGEX}|{_MARKDOWN_ESCAPE_COMMON})', re.MULTILINE)
+
+_URL_REGEX = r'(?P<url><[^: >]+:\/[^ >]+>|(?:https?|steam):\/\/[^\s<]+[^<.,:;\"\'\]\s])'
+
+_MARKDOWN_STOCK_REGEX = fr'(?P<markdown>[_\\~|\*`]|{_MARKDOWN_ESCAPE_COMMON})'
+
+
+def remove_markdown(text: str, *, ignore_links: bool = True) -> str:
+    """A helper function that removes markdown characters.
+
+    .. versionadded:: 1.7
+
+    .. note::
+            This function is not markdown aware and may remove meaning from the original text. For example,
+            if the input contains ``10 * 5`` then it will be converted into ``10  5``.
+
+    Parameters
+    -----------
+    text: :class:`str`
+        The text to remove markdown from.
+    ignore_links: :class:`bool`
+        Whether to leave links alone when removing markdown. For example,
+        if a URL in the text contains characters such as ``_`` then it will
+        be left alone. Defaults to ``True``.
+
+    Returns
+    --------
+    :class:`str`
+        The text with the markdown special characters removed.
+    """
+
+    def replacement(match):
+        groupdict = match.groupdict()
+        return groupdict.get('url', '')
+
+    regex = _MARKDOWN_STOCK_REGEX
+    if ignore_links:
+        regex = f'(?:{_URL_REGEX}|{regex})'
+    return re.sub(regex, replacement, text, 0, re.MULTILINE)
+
+
+def escape_markdown(text: str, *, as_needed: bool = False, ignore_links: bool = True) -> str:
+    r"""A helper function that escapes Discord's markdown.
+
+    Parameters
+    -----------
+    text: :class:`str`
+        The text to escape markdown from.
+    as_needed: :class:`bool`
+        Whether to escape the markdown characters as needed. This
+        means that it does not escape extraneous characters if it's
+        not necessary, e.g. ``**hello**`` is escaped into ``\*\*hello**``
+        instead of ``\*\*hello\*\*``. Note however that this can open
+        you up to some clever syntax abuse. Defaults to ``False``.
+    ignore_links: :class:`bool`
+        Whether to leave links alone when escaping markdown. For example,
+        if a URL in the text contains characters such as ``_`` then it will
+        be left alone. This option is not supported with ``as_needed``.
+        Defaults to ``True``.
+
+    Returns
+    --------
+    :class:`str`
+        The text with the markdown special characters escaped with a slash.
+    """
+
+    if not as_needed:
+
+        def replacement(match):
+            groupdict = match.groupdict()
+            is_url = groupdict.get('url')
+            if is_url:
+                return is_url
+            return '\\' + groupdict['markdown']
+
+        regex = _MARKDOWN_STOCK_REGEX
+        if ignore_links:
+            regex = f'(?:{_URL_REGEX}|{regex})'
+        return re.sub(regex, replacement, text, 0, re.MULTILINE)
+    else:
+        text = re.sub(r'\\', r'\\\\', text)
+        return _MARKDOWN_ESCAPE_REGEX.sub(r'\\\1', text)
+
+
+def escape_mentions(text: str) -> str:
+    """A helper function that escapes everyone, here, role, and user mentions.
+
+    .. note::
+
+        This does not include channel mentions.
+
+    .. note::
+
+        For more granular control over what mentions should be escaped
+        within messages, refer to the :class:`~discord.AllowedMentions`
+        class.
+
+    Parameters
+    -----------
+    text: :class:`str`
+        The text to escape mentions from.
+
+    Returns
+    --------
+    :class:`str`
+        The text with the mentions removed.
+    """
+    return re.sub(r'@(everyone|here|[!&]?[0-9]{17,20})', '@\u200b\\1', text)
+
+
+def _chunk(iterator: Iterable[T], max_size: int) -> Iterator[List[T]]:
+    ret = []
+    n = 0
+    for item in iterator:
+        ret.append(item)
+        n += 1
+        if n == max_size:
+            yield ret
+            ret = []
+            n = 0
+    if ret:
+        yield ret
+
+
+async def _achunk(iterator: AsyncIterable[T], max_size: int) -> AsyncIterator[List[T]]:
+    ret = []
+    n = 0
+    async for item in iterator:
+        ret.append(item)
+        n += 1
+        if n == max_size:
+            yield ret
+            ret = []
+            n = 0
+    if ret:
+        yield ret
+
+
+@overload
+def as_chunks(iterator: AsyncIterable[T], max_size: int) -> AsyncIterator[List[T]]:
+    ...
+
+
+@overload
+def as_chunks(iterator: Iterable[T], max_size: int) -> Iterator[List[T]]:
+    ...
+
+
+def as_chunks(iterator: _Iter[T], max_size: int) -> _Iter[List[T]]:
+    """A helper function that collects an iterator into chunks of a given size.
+
+    .. versionadded:: 2.0
+
+    Parameters
+    ----------
+    iterator: Union[:class:`collections.abc.Iterable`, :class:`collections.abc.AsyncIterable`]
+        The iterator to chunk, can be sync or async.
+    max_size: :class:`int`
+        The maximum chunk size.
+
+
+    .. warning::
+
+        The last chunk collected may not be as large as ``max_size``.
+
+    Returns
+    --------
+    Union[:class:`Iterator`, :class:`AsyncIterator`]
+        A new iterator which yields chunks of a given size.
+    """
+    if max_size <= 0:
+        raise ValueError('Chunk sizes must be greater than 0.')
+
+    if isinstance(iterator, AsyncIterable):
+        return _achunk(iterator, max_size)
+    return _chunk(iterator, max_size)
+
+
+PY_310 = sys.version_info >= (3, 10)
+
+
+def flatten_literal_params(parameters: Iterable[Any]) -> Tuple[Any, ...]:
+    params = []
+    literal_cls = type(Literal[0])
+    for p in parameters:
+        if isinstance(p, literal_cls):
+            params.extend(p.__args__)
+        else:
+            params.append(p)
+    return tuple(params)
+
+
+def normalise_optional_params(parameters: Iterable[Any]) -> Tuple[Any, ...]:
+    none_cls = type(None)
+    return tuple(p for p in parameters if p is not none_cls) + (none_cls,)
+
+
+def evaluate_annotation(
+    tp: Any,
+    globals: Dict[str, Any],
+    locals: Dict[str, Any],
+    cache: Dict[str, Any],
+    *,
+    implicit_str: bool = True,
+) -> Any:
+    if isinstance(tp, ForwardRef):
+        tp = tp.__forward_arg__
+        # ForwardRefs always evaluate their internals
+        implicit_str = True
+
+    if implicit_str and isinstance(tp, str):
+        if tp in cache:
+            return cache[tp]
+        evaluated = evaluate_annotation(eval(tp, globals, locals), globals, locals, cache)
+        cache[tp] = evaluated
+        return evaluated
+
+    if hasattr(tp, '__metadata__'):
+        # Annotated[X, Y] can access Y via __metadata__
+        metadata = tp.__metadata__[0]
+        return evaluate_annotation(metadata, globals, locals, cache)
+
+    if hasattr(tp, '__args__'):
+        implicit_str = True
+        is_literal = False
+        args = tp.__args__
+        if not hasattr(tp, '__origin__'):
+            if PY_310 and tp.__class__ is types.UnionType:  # type: ignore
+                converted = Union[args]  # type: ignore
+                return evaluate_annotation(converted, globals, locals, cache)
+
+            return tp
+        if tp.__origin__ is Union:
+            try:
+                if args.index(type(None)) != len(args) - 1:
+                    args = normalise_optional_params(tp.__args__)
+            except ValueError:
+                pass
+        if tp.__origin__ is Literal:
+            if not PY_310:
+                args = flatten_literal_params(tp.__args__)
+            implicit_str = False
+            is_literal = True
+
+        evaluated_args = tuple(evaluate_annotation(arg, globals, locals, cache, implicit_str=implicit_str) for arg in args)
+
+        if is_literal and not all(isinstance(x, (str, int, bool, type(None))) for x in evaluated_args):
+            raise TypeError('Literal arguments must be of type str, int, bool, or NoneType.')
+
+        try:
+            return tp.copy_with(evaluated_args)
+        except AttributeError:
+            return tp.__origin__[evaluated_args]
+
+    return tp
+
+
+def resolve_annotation(
+    annotation: Any,
+    globalns: Dict[str, Any],
+    localns: Optional[Dict[str, Any]],
+    cache: Optional[Dict[str, Any]],
+) -> Any:
+    if annotation is None:
+        return type(None)
+    if isinstance(annotation, str):
+        annotation = ForwardRef(annotation)
+
+    locals = globalns if localns is None else localns
+    if cache is None:
+        cache = {}
+    return evaluate_annotation(annotation, globalns, locals, cache)
+
+
+def is_inside_class(func: Callable[..., Any]) -> bool:
+    # For methods defined in a class, the qualname has a dotted path
+    # denoting which class it belongs to. So, e.g. for A.foo the qualname
+    # would be A.foo while a global foo() would just be foo.
+    #
+    # Unfortunately, for nested functions this breaks. So inside an outer
+    # function named outer, those two would end up having a qualname with
+    # outer.<locals>.A.foo and outer.<locals>.foo
+
+    if func.__qualname__ == func.__name__:
+        return False
+    (remaining, _, _) = func.__qualname__.rpartition('.')
+    return not remaining.endswith('<locals>')
+
+
+TimestampStyle = Literal['f', 'F', 'd', 'D', 't', 'T', 'R']
+
+
+def format_dt(dt: datetime.datetime, /, style: Optional[TimestampStyle] = None) -> str:
+    """A helper function to format a :class:`datetime.datetime` for presentation within Discord.
+
+    This allows for a locale-independent way of presenting data using Discord specific Markdown.
+
+    +-------------+----------------------------+-----------------+
+    |    Style    |       Example Output       |   Description   |
+    +=============+============================+=================+
+    | t           | 22:57                      | Short Time      |
+    +-------------+----------------------------+-----------------+
+    | T           | 22:57:58                   | Long Time       |
+    +-------------+----------------------------+-----------------+
+    | d           | 17/05/2016                 | Short Date      |
+    +-------------+----------------------------+-----------------+
+    | D           | 17 May 2016                | Long Date       |
+    +-------------+----------------------------+-----------------+
+    | f (default) | 17 May 2016 22:57          | Short Date Time |
+    +-------------+----------------------------+-----------------+
+    | F           | Tuesday, 17 May 2016 22:57 | Long Date Time  |
+    +-------------+----------------------------+-----------------+
+    | R           | 5 years ago                | Relative Time   |
+    +-------------+----------------------------+-----------------+
+
+    Note that the exact output depends on the user's locale setting in the client. The example output
+    presented is using the ``en-GB`` locale.
+
+    .. versionadded:: 2.0
+
+    Parameters
+    -----------
+    dt: :class:`datetime.datetime`
+        The datetime to format.
+    style: :class:`str`
+        The style to format the datetime with.
+
+    Returns
+    --------
+    :class:`str`
+        The formatted string.
+    """
+    if style is None:
+        return f'<t:{int(dt.timestamp())}>'
+    return f'<t:{int(dt.timestamp())}:{style}>'
+
+
+def set_target(
+    items: Iterable[ApplicationCommand],
+    *,
+    channel: Optional[Messageable] = MISSING,
+    message: Optional[Message] = MISSING,
+    user: Optional[Snowflake] = MISSING,
+) -> None:
+    """A helper function to set the target for a list of items.
+
+    This is used to set the target for a list of application commands.
+
+    Suppresses all AttributeErrors so you can pass multiple types of commands and
+    not worry about which elements support which parameter.
+
+    Parameters
+    -----------
+    items: Iterable[:class:`.abc.ApplicationCommand`]
+        A list of items to set the target for.
+    channel: Optional[:class:`.abc.Messageable`]
+        The channel to target.
+    message: Optional[:class:`.Message`]
+        The message to target.
+    user: Optional[:class:`~discord.abc.Snowflake`]
+        The user to target.
+    """
+    attrs = {}
+    if channel is not MISSING:
+        attrs['target_channel'] = channel
+    if message is not MISSING:
+        attrs['target_message'] = message
+    if user is not MISSING:
+        attrs['target_user'] = user
+
+    for item in items:
+        for k, v in attrs.items():
+            try:
+                setattr(item, k, v)
+            except AttributeError:
+                pass
+
+
+def _generate_session_id() -> str:
+    return ''.join(random.choices(string.ascii_letters + string.digits, k=16))
+
+
+def _generate_nonce() -> str:
+    return str(time_snowflake(utcnow()))
+
+
+def _parse_localizations(data: Any, key: str) -> tuple[Any, dict]:
+    values = data.get(key)
+    values = values if isinstance(values, dict) else {'default': values}
+    string = values['default']
+    localizations = {
+        try_enum(Locale, k): v for k, v in (values.get('localizations', data.get(f'{key}_localizations')) or {}).items()
+    }
+    return string, localizations
+
+
+class ExpiringString(collections.UserString):
+    def __init__(self, data: str, timeout: int) -> None:
+        super().__init__(data)
+        self._timer: Timer = Timer(timeout, self._destruct)
+        self._timer.start()
+
+    def _update(self, data: str, timeout: int) -> None:
+        try:
+            self._timer.cancel()
+        except:
+            pass
+        self.data = data
+        self._timer: Timer = Timer(timeout, self._destruct)
+        self._timer.start()
+
+    def _destruct(self) -> None:
+        self.data = ''
+
+    def destroy(self) -> None:
+        self._destruct()
+        self._timer.cancel()
+
+
+async def _get_info(session: ClientSession) -> Tuple[Dict[str, Any], str]:
+    for _ in range(3):
+        try:
+            async with session.post('https://cordapi.dolfi.es/api/v2/properties/web', timeout=5) as resp:
+                json = await resp.json()
+                return json['properties'], json['encoded']
+        except Exception:
+            continue
+
+    _log.warning('Info API down. Falling back to manual fetching...')
+    ua = await _get_user_agent(session)
+    bn = await _get_build_number(session)
+    bv = _get_browser_version(ua)
+
+    properties = {
+        'os': 'Windows',
+        'browser': 'Chrome',
+        'device': '',
+        'browser_user_agent': ua,
+        'browser_version': bv,
+        'os_version': '10',
+        'referrer': '',
+        'referring_domain': '',
+        'referrer_current': '',
+        'referring_domain_current': '',
+        'release_channel': 'stable',
+        'system_locale': 'en-US',
+        'client_build_number': bn,
+        'client_event_source': None,
+        'design_id': 0,
+    }
+    return properties, b64encode(_to_json(properties).encode()).decode('utf-8')
+
+
+async def _get_build_number(session: ClientSession) -> int:  # Thank you Discord-S.C.U.M
+    """Fetches client build number"""
+    try:
+        login_page_request = await session.get('https://discord.com/login', timeout=7)
+        login_page = await login_page_request.text()
+        build_url = 'https://discord.com/assets/' + re.compile(r'assets/+([a-z0-9]+)\.js').findall(login_page)[-2] + '.js'
+        build_request = await session.get(build_url, timeout=7)
+        build_file = await build_request.text()
+        build_index = build_file.find('buildNumber') + 24
+        return int(build_file[build_index : build_index + 6])
+    except asyncio.TimeoutError:
+        _log.critical('Could not fetch client build number. Falling back to hardcoded value...')
+        return 9999
+
+
+async def _get_user_agent(session: ClientSession) -> str:
+    """Fetches the latest Windows 10/Chrome user-agent."""
+    try:
+        request = await session.request('GET', 'https://jnrbsn.github.io/user-agents/user-agents.json', timeout=7)
+        response = json.loads(await request.text())
+        return response[0]
+    except asyncio.TimeoutError:
+        _log.critical('Could not fetch user-agent. Falling back to hardcoded value...')
+        return (
+            'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
+        )
+
+
+def _get_browser_version(user_agent: str) -> str:
+    """Fetches the latest Windows 10/Chrome version."""
+    return user_agent.split('Chrome/')[1].split()[0]
+
+
+def is_docker() -> bool:
+    path = '/proc/self/cgroup'
+    return os.path.exists('/.dockerenv') or (os.path.isfile(path) and any('docker' in line for line in open(path)))
+
+
+def stream_supports_colour(stream: Any) -> bool:
+    # Pycharm and Vscode support colour in their inbuilt editors
+    if 'PYCHARM_HOSTED' in os.environ or os.environ.get('TERM_PROGRAM') == 'vscode':
+        return True
+
+    is_a_tty = hasattr(stream, 'isatty') and stream.isatty()
+    if sys.platform != 'win32':
+        # Docker does not consistently have a tty attached to it
+        return is_a_tty or is_docker()
+
+    # ANSICON checks for things like ConEmu
+    # WT_SESSION checks if this is Windows Terminal
+    return is_a_tty and ('ANSICON' in os.environ or 'WT_SESSION' in os.environ)
+
+
+class _ColourFormatter(logging.Formatter):
+
+    # ANSI codes are a bit weird to decipher if you're unfamiliar with them, so here's a refresher
+    # It starts off with a format like \x1b[XXXm where XXX is a semicolon separated list of commands
+    # The important ones here relate to colour.
+    # 30-37 are black, red, green, yellow, blue, magenta, cyan and white in that order
+    # 40-47 are the same except for the background
+    # 90-97 are the same but "bright" foreground
+    # 100-107 are the same as the bright ones but for the background.
+    # 1 means bold, 2 means dim, 0 means reset, and 4 means underline.
+
+    LEVEL_COLOURS = [
+        (logging.DEBUG, '\x1b[40;1m'),
+        (logging.INFO, '\x1b[34;1m'),
+        (logging.WARNING, '\x1b[33;1m'),
+        (logging.ERROR, '\x1b[31m'),
+        (logging.CRITICAL, '\x1b[41m'),
+    ]
+
+    FORMATS = {
+        level: logging.Formatter(
+            f'\x1b[30;1m%(asctime)s\x1b[0m {colour}%(levelname)-8s\x1b[0m \x1b[35m%(name)s\x1b[0m %(message)s',
+            '%Y-%m-%d %H:%M:%S',
+        )
+        for level, colour in LEVEL_COLOURS
+    }
+
+    def format(self, record):
+        formatter = self.FORMATS.get(record.levelno)
+        if formatter is None:
+            formatter = self.FORMATS[logging.DEBUG]
+
+        # Override the traceback to always print in red
+        if record.exc_info:
+            text = formatter.formatException(record.exc_info)
+            record.exc_text = f'\x1b[31m{text}\x1b[0m'
+
+        output = formatter.format(record)
+
+        # Remove the cache layer
+        record.exc_text = None
+        return output
+
+
+def setup_logging(
+    *,
+    handler: logging.Handler = MISSING,
+    formatter: logging.Formatter = MISSING,
+    level: int = MISSING,
+    root: bool = True,
+) -> None:
+    """A helper function to setup logging.
+
+    This is superficially similar to :func:`logging.basicConfig` but
+    uses different defaults and a colour formatter if the stream can
+    display colour.
+
+    This is used by the :class:`~discord.Client` to set up logging
+    if ``log_handler`` is not ``None``.
+
+    .. versionadded:: 2.0
+
+    Parameters
+    -----------
+    handler: :class:`logging.Handler`
+        The log handler to use for the library's logger.
+
+        The default log handler if not provided is :class:`logging.StreamHandler`.
+    formatter: :class:`logging.Formatter`
+        The formatter to use with the given log handler. If not provided then it
+        defaults to a colour based logging formatter (if available). If colour
+        is not available then a simple logging formatter is provided.
+    level: :class:`int`
+        The default log level for the library's logger. Defaults to ``logging.INFO``.
+    root: :class:`bool`
+        Whether to set up the root logger rather than the library logger.
+        Unlike the default for :class:`~discord.Client`, this defaults to ``True``.
+    """
+
+    if level is MISSING:
+        level = logging.INFO
+
+    if handler is MISSING:
+        handler = logging.StreamHandler()
+
+    if formatter is MISSING:
+        if isinstance(handler, logging.StreamHandler) and stream_supports_colour(handler.stream):
+            formatter = _ColourFormatter()
+        else:
+            dt_fmt = '%Y-%m-%d %H:%M:%S'
+            formatter = logging.Formatter('[{asctime}] [{levelname:<8}] {name}: {message}', dt_fmt, style='{')
+
+    if root:
+        logger = logging.getLogger()
+    else:
+        library, _, _ = __name__.partition('.')
+        logger = logging.getLogger(library)
+
+    handler.setFormatter(formatter)
+    logger.setLevel(level)
+    logger.addHandler(handler)
```

### Comparing `discord.py-self-1.9.2/discord/backoff.py` & `discord.py-self-2.0.0/discord/backoff.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,108 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import time
-import random
-
-class ExponentialBackoff:
-    """An implementation of the exponential backoff algorithm
-
-    Provides a convenient interface to implement an exponential backoff
-    for reconnecting or retrying transmissions in a distributed network.
-
-    Once instantiated, the delay method will return the next interval to
-    wait for when retrying a connection or transmission.  The maximum
-    delay increases exponentially with each retry up to a maximum of
-    2^10 * base, and is reset if no more attempts are needed in a period
-    of 2^11 * base seconds.
-
-    Parameters
-    ----------
-    base: :class:`int`
-        The base delay in seconds. The first retry-delay will be up to
-        this many seconds.
-    integral: :class:`bool`
-        Set to ``True`` if whole periods of base is desirable, otherwise any
-        number in between may be returned.
-    """
-
-    def __init__(self, base=1, *, integral=False):
-        self._base = base
-
-        self._exp = 0
-        self._max = 10
-        self._reset_time = base * 2 ** 11
-        self._last_invocation = time.monotonic()
-
-        # Use our own random instance to avoid messing with global one
-        rand = random.Random()
-        rand.seed()
-
-        self._randfunc = rand.randrange if integral else rand.uniform
-
-    def delay(self):
-        """Compute the next delay
-
-        Returns the next delay to wait according to the exponential
-        backoff algorithm.  This is a value between 0 and base * 2^exp
-        where exponent starts off at 1 and is incremented at every
-        invocation of this method up to a maximum of 10.
-
-        If a period of more than base * 2^11 has passed since the last
-        retry, the exponent is reset to 1.
-        """
-        invocation = time.monotonic()
-        interval = invocation - self._last_invocation
-        self._last_invocation = invocation
-
-        if interval > self._reset_time:
-            self._exp = 0
-
-        self._exp = min(self._exp + 1, self._max)
-        return self._randfunc(0, self._base * 2 ** self._exp)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+
+import time
+import random
+from typing import Callable, Generic, Literal, TypeVar, overload, Union
+
+T = TypeVar('T', bool, Literal[True], Literal[False])
+
+# fmt: off
+__all__ = (
+    'ExponentialBackoff',
+)
+# fmt: on
+
+
+class ExponentialBackoff(Generic[T]):
+    """An implementation of the exponential backoff algorithm
+
+    Provides a convenient interface to implement an exponential backoff
+    for reconnecting or retrying transmissions in a distributed network.
+
+    Once instantiated, the delay method will return the next interval to
+    wait for when retrying a connection or transmission.  The maximum
+    delay increases exponentially with each retry up to a maximum of
+    2^10 * base, and is reset if no more attempts are needed in a period
+    of 2^11 * base seconds.
+
+    Parameters
+    ----------
+    base: :class:`int`
+        The base delay in seconds. The first retry-delay will be up to
+        this many seconds.
+    integral: :class:`bool`
+        Set to ``True`` if whole periods of base is desirable, otherwise any
+        number in between may be returned.
+    """
+
+    def __init__(self, base: int = 1, *, integral: T = False):
+        self._base: int = base
+
+        self._exp: int = 0
+        self._max: int = 10
+        self._reset_time: int = base * 2**11
+        self._last_invocation: float = time.monotonic()
+
+        # Use our own random instance to avoid messing with global one
+        rand = random.Random()
+        rand.seed()
+
+        self._randfunc: Callable[..., Union[int, float]] = rand.randrange if integral else rand.uniform
+
+    @overload
+    def delay(self: ExponentialBackoff[Literal[False]]) -> float:
+        ...
+
+    @overload
+    def delay(self: ExponentialBackoff[Literal[True]]) -> int:
+        ...
+
+    @overload
+    def delay(self: ExponentialBackoff[bool]) -> Union[int, float]:
+        ...
+
+    def delay(self) -> Union[int, float]:
+        """Compute the next delay
+
+        Returns the next delay to wait according to the exponential
+        backoff algorithm.  This is a value between 0 and base * 2^exp
+        where exponent starts off at 1 and is incremented at every
+        invocation of this method up to a maximum of 10.
+
+        If a period of more than base * 2^11 has passed since the last
+        retry, the exponent is reset to 1.
+        """
+        invocation = time.monotonic()
+        interval = invocation - self._last_invocation
+        self._last_invocation = invocation
+
+        if interval > self._reset_time:
+            self._exp = 0
+
+        self._exp = min(self._exp + 1, self._max)
+        return self._randfunc(0, self._base * 2**self._exp)
```

### Comparing `discord.py-self-1.9.2/discord/bin/libopus-0.x64.dll` & `discord.py-self-2.0.0/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discord.py-self-1.9.2/discord/bin/libopus-0.x86.dll` & `discord.py-self-2.0.0/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discord.py-self-1.9.2/discord/emoji.py` & `discord.py-self-2.0.0/discord/emoji.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,280 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .asset import Asset
-from . import utils
-from .partial_emoji import _EmojiTag
-from .user import User
-
-class Emoji(_EmojiTag):
-    """Represents a custom emoji.
-
-    Depending on the way this object was created, some of the attributes can
-    have a value of ``None``.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two emoji are the same.
-
-        .. describe:: x != y
-
-            Checks if two emoji are not the same.
-
-        .. describe:: hash(x)
-
-            Return the emoji's hash.
-
-        .. describe:: iter(x)
-
-            Returns an iterator of ``(field, value)`` pairs. This allows this class
-            to be used as an iterable in list/dict/etc constructions.
-
-        .. describe:: str(x)
-
-            Returns the emoji rendered for discord.
-
-    Attributes
-    -----------
-    name: :class:`str`
-        The name of the emoji.
-    id: :class:`int`
-        The emoji's ID.
-    require_colons: :class:`bool`
-        If colons are required to use this emoji in the client (:PJSalt: vs PJSalt).
-    animated: :class:`bool`
-        Whether an emoji is animated or not.
-    managed: :class:`bool`
-        If this emoji is managed by a Twitch integration.
-    guild_id: :class:`int`
-        The guild ID the emoji belongs to.
-    available: :class:`bool`
-        Whether the emoji is available for use.
-    user: Optional[:class:`User`]
-        The user that created the emoji. This can only be retrieved using :meth:`Guild.fetch_emoji` and
-        having the :attr:`~Permissions.manage_emojis` permission.
-    """
-    __slots__ = ('require_colons', 'animated', 'managed', 'id', 'name', '_roles', 'guild_id',
-                 '_state', 'user', 'available')
-
-    def __init__(self, *, guild, state, data):
-        self.guild_id = guild.id
-        self._state = state
-        self._from_data(data)
-
-    def _from_data(self, emoji):
-        self.require_colons = emoji['require_colons']
-        self.managed = emoji['managed']
-        self.id = int(emoji['id'])
-        self.name = emoji['name']
-        self.animated = emoji.get('animated', False)
-        self.available = emoji.get('available', True)
-        self._roles = utils.SnowflakeList(map(int, emoji.get('roles', [])))
-        user = emoji.get('user')
-        self.user = User(state=self._state, data=user) if user else None
-
-    def _iterator(self):
-        for attr in self.__slots__:
-            if attr[0] != '_':
-                value = getattr(self, attr, None)
-                if value is not None:
-                    yield (attr, value)
-
-    def __iter__(self):
-        return self._iterator()
-
-    def __str__(self):
-        if self.animated:
-            return '<a:{0.name}:{0.id}>'.format(self)
-        return "<:{0.name}:{0.id}>".format(self)
-
-    def __repr__(self):
-        return '<Emoji id={0.id} name={0.name!r} animated={0.animated} managed={0.managed}>'.format(self)
-
-    def __eq__(self, other):
-        return isinstance(other, _EmojiTag) and self.id == other.id
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
-        return self.id >> 22
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the emoji's creation time in UTC."""
-        return utils.snowflake_time(self.id)
-
-    @property
-    def url(self):
-        """:class:`Asset`: Returns the asset of the emoji.
-
-        This is equivalent to calling :meth:`url_as` with
-        the default parameters (i.e. png/gif detection).
-        """
-        return self.url_as(format=None)
-
-    @property
-    def roles(self):
-        """List[:class:`Role`]: A :class:`list` of roles that is allowed to use this emoji.
-
-        If roles is empty, the emoji is unrestricted.
-        """
-        guild = self.guild
-        if guild is None:
-            return []
-
-        return [role for role in guild.roles if self._roles.has(role.id)]
-
-    @property
-    def guild(self):
-        """:class:`Guild`: The guild this emoji belongs to."""
-        return self._state._get_guild(self.guild_id)
-
-
-    def url_as(self, *, format=None, static_format="png"):
-        """Returns an :class:`Asset` for the emoji's url.
-
-        The format must be one of 'webp', 'jpeg', 'jpg', 'png' or 'gif'.
-        'gif' is only valid for animated emojis.
-
-        .. versionadded:: 1.6
-
-        Parameters
-        -----------
-        format: Optional[:class:`str`]
-            The format to attempt to convert the emojis to.
-            If the format is ``None``, then it is automatically
-            detected as either 'gif' or static_format, depending on whether the
-            emoji is animated or not.
-        static_format: Optional[:class:`str`]
-            Format to attempt to convert only non-animated emoji's to.
-            Defaults to 'png'
-
-        Raises
-        -------
-        InvalidArgument
-            Bad image format passed to ``format`` or ``static_format``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_emoji(self._state, self, format=format, static_format=static_format)
-
-
-    def is_usable(self):
-        """:class:`bool`: Whether the bot can use this emoji.
-
-        .. versionadded:: 1.3
-        """
-        if not self.available:
-            return False
-        if not self._roles:
-            return True
-        emoji_roles, my_roles = self._roles, self.guild.me._roles
-        return any(my_roles.has(role_id) for role_id in emoji_roles)
-
-    async def delete(self):
-        """|coro|
-
-        Deletes the custom emoji.
-
-        You must have :attr:`~Permissions.manage_emojis` permission to
-        do this.
-
-        Raises
-        -------
-        Forbidden
-            You are not allowed to delete emojis.
-        HTTPException
-            An error occurred deleting the emoji.
-        """
-
-        await self._state.http.delete_custom_emoji(self.guild.id, self.id)
-
-    async def edit(self, *, name=None):
-        r"""|coro|
-
-        Edits the custom emoji.
-
-        You must have :attr:`~Permissions.manage_emojis` permission to
-        do this.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The new emoji name.
-
-        Raises
-        -------
-        Forbidden
-            You are not allowed to edit emojis.
-        HTTPException
-            An error occurred editing the emoji.
-        """
-
-        name = name or self.name
-        await self._state.http.edit_custom_emoji(self.guild.id, self.id, name=name)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+from typing import Any, Collection, Iterator, List, Optional, TYPE_CHECKING, Tuple
+
+from .asset import Asset, AssetMixin
+from .utils import SnowflakeList, snowflake_time, MISSING
+from .partial_emoji import _EmojiTag, PartialEmoji
+from .user import User
+
+# fmt: off
+__all__ = (
+    'Emoji',
+)
+# fmt: on
+
+if TYPE_CHECKING:
+    from .types.emoji import Emoji as EmojiPayload
+    from .guild import Guild
+    from .state import ConnectionState
+    from .abc import Snowflake
+    from .role import Role
+    from datetime import datetime
+
+
+class Emoji(_EmojiTag, AssetMixin):
+    """Represents a custom emoji.
+
+    Depending on the way this object was created, some of the attributes can
+    have a value of ``None``.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two emoji are the same.
+
+        .. describe:: x != y
+
+            Checks if two emoji are not the same.
+
+        .. describe:: hash(x)
+
+            Return the emoji's hash.
+
+        .. describe:: iter(x)
+
+            Returns an iterator of ``(field, value)`` pairs. This allows this class
+            to be used as an iterable in list/dict/etc constructions.
+
+        .. describe:: str(x)
+
+            Returns the emoji rendered for discord.
+
+    Attributes
+    -----------
+    name: :class:`str`
+        The name of the emoji.
+    id: :class:`int`
+        The emoji's ID.
+    require_colons: :class:`bool`
+        If colons are required to use this emoji in the client (:PJSalt: vs PJSalt).
+    animated: :class:`bool`
+        Whether an emoji is animated or not.
+    managed: :class:`bool`
+        If this emoji is managed by a Twitch integration.
+    guild_id: :class:`int`
+        The guild ID the emoji belongs to.
+    available: :class:`bool`
+        Whether the emoji is available for use.
+    user: Optional[:class:`User`]
+        The user that created the emoji. This can only be retrieved using :meth:`Guild.fetch_emoji` and
+        having :attr:`~Permissions.manage_emojis`.
+    """
+
+    __slots__: Tuple[str, ...] = (
+        'require_colons',
+        'animated',
+        'managed',
+        'id',
+        'name',
+        '_roles',
+        'guild_id',
+        '_state',
+        'user',
+        'available',
+    )
+
+    def __init__(self, *, guild: Guild, state: ConnectionState, data: EmojiPayload):
+        self.guild_id: int = guild.id
+        self._state: ConnectionState = state
+        self._from_data(data)
+
+    def _from_data(self, emoji: EmojiPayload):
+        self.require_colons: bool = emoji.get('require_colons', False)
+        self.managed: bool = emoji.get('managed', False)
+        self.id: int = int(emoji['id'])  # type: ignore # This won't be None for full emoji objects.
+        self.name: str = emoji['name']  # type: ignore # This won't be None for full emoji objects.
+        self.animated: bool = emoji.get('animated', False)
+        self.available: bool = emoji.get('available', True)
+        self._roles: SnowflakeList = SnowflakeList(map(int, emoji.get('roles', [])))
+        user = emoji.get('user')
+        self.user: Optional[User] = User(state=self._state, data=user) if user else None
+
+    def _to_partial(self) -> PartialEmoji:
+        return PartialEmoji(name=self.name, animated=self.animated, id=self.id)
+
+    def __iter__(self) -> Iterator[Tuple[str, Any]]:
+        for attr in self.__slots__:
+            if attr[0] != '_':
+                value = getattr(self, attr, None)
+                if value is not None:
+                    yield (attr, value)
+
+    def __str__(self) -> str:
+        if self.animated:
+            return f'<a:{self.name}:{self.id}>'
+        return f'<:{self.name}:{self.id}>'
+
+    def __repr__(self) -> str:
+        return f'<Emoji id={self.id} name={self.name!r} animated={self.animated} managed={self.managed}>'
+
+    def __eq__(self, other: object) -> bool:
+        return isinstance(other, _EmojiTag) and self.id == other.id
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
+    def __hash__(self) -> int:
+        return self.id >> 22
+
+    @property
+    def created_at(self) -> datetime:
+        """:class:`datetime.datetime`: Returns the emoji's creation time in UTC."""
+        return snowflake_time(self.id)
+
+    @property
+    def url(self) -> str:
+        """:class:`str`: Returns the URL of the emoji."""
+        fmt = 'gif' if self.animated else 'png'
+        return f'{Asset.BASE}/emojis/{self.id}.{fmt}'
+
+    @property
+    def roles(self) -> List[Role]:
+        """List[:class:`Role`]: A :class:`list` of roles that is allowed to use this emoji.
+
+        If roles is empty, the emoji is unrestricted.
+        """
+        guild = self.guild
+        if guild is None:
+            return []
+
+        return [role for role in guild.roles if self._roles.has(role.id)]
+
+    @property
+    def guild(self) -> Optional[Guild]:
+        """:class:`Guild`: The guild this emoji belongs to."""
+        return self._state._get_guild(self.guild_id)
+
+    def is_usable(self) -> bool:
+        """:class:`bool`: Whether the bot can use this emoji.
+
+        .. versionadded:: 1.3
+        """
+        if not self.available or not self.guild or self.guild.unavailable:
+            return False
+        if not self._roles:
+            return True
+        emoji_roles, my_roles = self._roles, self.guild.me._roles  # type: ignore # Should just error ATP
+        return any(my_roles.has(role_id) for role_id in emoji_roles)
+
+    async def delete(self, *, reason: Optional[str] = None) -> None:
+        """|coro|
+
+        Deletes the custom emoji.
+
+        You must have :attr:`~Permissions.manage_emojis` to do this.
+
+        Parameters
+        -----------
+        reason: Optional[:class:`str`]
+            The reason for deleting this emoji. Shows up on the audit log.
+
+        Raises
+        -------
+        Forbidden
+            You are not allowed to delete emojis.
+        HTTPException
+            An error occurred deleting the emoji.
+        """
+
+        await self._state.http.delete_custom_emoji(self.guild_id, self.id, reason=reason)
+
+    async def edit(
+        self, *, name: str = MISSING, roles: Collection[Snowflake] = MISSING, reason: Optional[str] = None
+    ) -> Emoji:
+        r"""|coro|
+
+        Edits the custom emoji.
+
+        You must have :attr:`~Permissions.manage_emojis` to do this.
+
+        .. versionchanged:: 2.0
+            The newly updated emoji is returned.
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The new emoji name.
+        roles: List[:class:`~discord.abc.Snowflake`]
+            A list of roles that can use this emoji. An empty list can be passed to make it available to everyone.
+        reason: Optional[:class:`str`]
+            The reason for editing this emoji. Shows up on the audit log.
+
+        Raises
+        -------
+        Forbidden
+            You are not allowed to edit emojis.
+        HTTPException
+            An error occurred editing the emoji.
+
+        Returns
+        --------
+        :class:`Emoji`
+            The newly updated emoji.
+        """
+
+        payload = {}
+        if name is not MISSING:
+            payload['name'] = name
+        if roles is not MISSING:
+            payload['roles'] = [role.id for role in roles]
+
+        data = await self._state.http.edit_custom_emoji(self.guild_id, self.id, payload=payload, reason=reason)
+        return Emoji(guild=self.guild, data=data, state=self._state)  # type: ignore # If guild is None, the http request would have failed
+
+    async def fetch_guild(self):
+        """|coro|
+
+        Retrieves the guild this emoji belongs to.
+
+        Raises
+        ------
+        NotFound
+            The guild this emoji belongs to is not public.
+        HTTPException
+            An error occurred while fetching the guild.
+
+        Returns
+        -------
+        :class:`Guild`
+            The guild this emoji belongs to.
+        """
+        from .guild import Guild  # Circular import
+
+        state = self._state
+        data = await state.http.get_emoji_guild(self.id)
+        return Guild(state=state, data=data)
```

### Comparing `discord.py-self-1.9.2/discord/ext/commands/_types.py` & `discord.py-self-2.0.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-# This is merely a tag type to avoid circular import issues.
-# Yes, this is a terrible solution but ultimately it is the only solution.
-class _BaseCommand:
-    __slots__ = ()
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

### Comparing `discord.py-self-1.9.2/discord/ext/commands/bot.py` & `discord.py-self-2.0.0/discord/ext/commands/bot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1052 +1,1293 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import asyncio
-import collections
-import inspect
-import importlib.util
-import sys
-import traceback
-import types
-
-import discord
-
-from .core import GroupMixin
-from .view import StringView
-from .context import Context
-from . import errors
-from .help import HelpCommand, DefaultHelpCommand
-from .cog import Cog
-
-def when_mentioned(bot, msg):
-    """A callable that implements a command prefix equivalent to being mentioned.
-
-    These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
-    """
-    return [bot.user.mention + ' ', '<@!%s> ' % bot.user.id]
-
-def when_mentioned_or(*prefixes):
-    """A callable that implements when mentioned or other prefixes provided.
-
-    These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
-
-    Example
-    --------
-
-    .. code-block:: python3
-
-        bot = commands.Bot(command_prefix=commands.when_mentioned_or('!'))
-
-
-    .. note::
-
-        This callable returns another callable, so if this is done inside a custom
-        callable, you must call the returned callable, for example:
-
-        .. code-block:: python3
-
-            async def get_prefix(bot, message):
-                extras = await prefixes_for(message.guild) # returns a list
-                return commands.when_mentioned_or(*extras)(bot, message)
-
-
-    See Also
-    ----------
-    :func:`.when_mentioned`
-    """
-    def inner(bot, msg):
-        r = list(prefixes)
-        r = when_mentioned(bot, msg) + r
-        return r
-
-    return inner
-
-def _is_submodule(parent, child):
-    return parent == child or child.startswith(parent + ".")
-
-class _DefaultRepr:
-    def __repr__(self):
-        return '<default-help-command>'
-
-_default = _DefaultRepr()
-
-class BotBase(GroupMixin):
-    def __init__(self, command_prefix, help_command=_default, description=None, **options):
-        super().__init__(**options)
-        self.command_prefix = command_prefix
-        self.extra_events = {}
-        self.__cogs = {}
-        self.__extensions = {}
-        self._checks = []
-        self._check_once = []
-        self._before_invoke = None
-        self._after_invoke = None
-        self._help_command = None
-        self.description = inspect.cleandoc(description) if description else ''
-        self.owner_id = options.get('owner_id')
-        self.owner_ids = options.get('owner_ids', set())
-        self.strip_after_prefix = options.get('strip_after_prefix', False)
-
-        if self.owner_id and self.owner_ids:
-            raise TypeError('Both owner_id and owner_ids are set.')
-
-        if self.owner_ids and not isinstance(self.owner_ids, collections.abc.Collection):
-            raise TypeError('owner_ids must be a collection not {0.__class__!r}'.format(self.owner_ids))
-
-        self_bot = options.get('self_bot', False)
-        user_bot = options.get('user_bot', False)
-
-        if self_bot and user_bot:
-            raise TypeError('Both self_bot and user_bot are set.')
-
-        if self_bot:
-            self._skip_check = lambda x, y: x != y
-        elif user_bot:
-            self._skip_check = lambda x, y: False
-        else:
-            self._skip_check = lambda x, y: x == y
-
-        if help_command is _default:
-            self.help_command = DefaultHelpCommand()
-        else:
-            self.help_command = help_command
-
-    # internal helpers
-
-    def dispatch(self, event_name, *args, **kwargs):
-        super().dispatch(event_name, *args, **kwargs)
-        ev = 'on_' + event_name
-        for event in self.extra_events.get(ev, []):
-            self._schedule_event(event, ev, *args, **kwargs)
-
-    async def close(self):
-        for extension in tuple(self.__extensions):
-            try:
-                self.unload_extension(extension)
-            except Exception:
-                pass
-
-        for cog in tuple(self.__cogs):
-            try:
-                self.remove_cog(cog)
-            except Exception:
-                pass
-
-        await super().close()
-
-    async def on_command_error(self, context, exception):
-        """|coro|
-
-        The default command error handler provided by the bot.
-
-        By default this prints to :data:`sys.stderr` however it could be
-        overridden to have a different implementation.
-
-        This only fires if you do not specify any listeners for command error.
-        """
-        if self.extra_events.get('on_command_error', None):
-            return
-
-        if hasattr(context.command, 'on_error'):
-            return
-
-        cog = context.cog
-        if cog and Cog._get_overridden_method(cog.cog_command_error) is not None:
-            return
-
-        print('Ignoring exception in command {}:'.format(context.command), file=sys.stderr)
-        traceback.print_exception(type(exception), exception, exception.__traceback__, file=sys.stderr)
-
-    # global check registration
-
-    def check(self, func):
-        r"""A decorator that adds a global check to the bot.
-
-        A global check is similar to a :func:`.check` that is applied
-        on a per command basis except it is run before any command checks
-        have been verified and applies to every command the bot has.
-
-        .. note::
-
-            This function can either be a regular function or a coroutine.
-
-        Similar to a command :func:`.check`\, this takes a single parameter
-        of type :class:`.Context` and can only raise exceptions inherited from
-        :exc:`.CommandError`.
-
-        Example
-        ---------
-
-        .. code-block:: python3
-
-            @bot.check
-            def check_commands(ctx):
-                return ctx.command.qualified_name in allowed_commands
-
-        """
-        self.add_check(func)
-        return func
-
-    def add_check(self, func, *, call_once=False):
-        """Adds a global check to the bot.
-
-        This is the non-decorator interface to :meth:`.check`
-        and :meth:`.check_once`.
-
-        Parameters
-        -----------
-        func
-            The function that was used as a global check.
-        call_once: :class:`bool`
-            If the function should only be called once per
-            :meth:`.Command.invoke` call.
-        """
-
-        if call_once:
-            self._check_once.append(func)
-        else:
-            self._checks.append(func)
-
-    def remove_check(self, func, *, call_once=False):
-        """Removes a global check from the bot.
-
-        This function is idempotent and will not raise an exception
-        if the function is not in the global checks.
-
-        Parameters
-        -----------
-        func
-            The function to remove from the global checks.
-        call_once: :class:`bool`
-            If the function was added with ``call_once=True`` in
-            the :meth:`.Bot.add_check` call or using :meth:`.check_once`.
-        """
-        l = self._check_once if call_once else self._checks
-
-        try:
-            l.remove(func)
-        except ValueError:
-            pass
-
-    def check_once(self, func):
-        r"""A decorator that adds a "call once" global check to the bot.
-
-        Unlike regular global checks, this one is called only once
-        per :meth:`.Command.invoke` call.
-
-        Regular global checks are called whenever a command is called
-        or :meth:`.Command.can_run` is called. This type of check
-        bypasses that and ensures that it's called only once, even inside
-        the default help command.
-
-        .. note::
-
-            When using this function the :class:`.Context` sent to a group subcommand
-            may only parse the parent command and not the subcommands due to it
-            being invoked once per :meth:`.Bot.invoke` call.
-
-        .. note::
-
-            This function can either be a regular function or a coroutine.
-
-        Similar to a command :func:`.check`\, this takes a single parameter
-        of type :class:`.Context` and can only raise exceptions inherited from
-        :exc:`.CommandError`.
-
-        Example
-        ---------
-
-        .. code-block:: python3
-
-            @bot.check_once
-            def whitelist(ctx):
-                return ctx.message.author.id in my_whitelist
-
-        """
-        self.add_check(func, call_once=True)
-        return func
-
-    async def can_run(self, ctx, *, call_once=False):
-        data = self._check_once if call_once else self._checks
-
-        if len(data) == 0:
-            return True
-
-        return await discord.utils.async_all(f(ctx) for f in data)
-
-    async def is_owner(self, user):
-        """|coro|
-
-        Checks if a :class:`~discord.User` or :class:`~discord.Member` is the owner of
-        this bot.
-
-        Parameters
-        -----------
-        user: :class:`.abc.User`
-            The user to check for.
-
-        Raises
-        -------
-        AttributeError
-            Owners aren't set.
-
-        Returns
-        --------
-        :class:`bool`
-            Whether the user is the owner.
-        """
-
-        if self.owner_id:
-            return user.id == self.owner_id
-        elif self.owner_ids:
-            return user.id in self.owner_ids
-        else:
-            raise AttributeError('Owners aren\'t set.')
-
-    def before_invoke(self, coro):
-        """A decorator that registers a coroutine as a pre-invoke hook.
-
-        A pre-invoke hook is called directly before the command is
-        called. This makes it a useful function to set up database
-        connections or any type of set up required.
-
-        This pre-invoke hook takes a sole parameter, a :class:`.Context`.
-
-        .. note::
-
-            The :meth:`~.Bot.before_invoke` and :meth:`~.Bot.after_invoke` hooks are
-            only called if all checks and argument parsing procedures pass
-            without error. If any check or argument parsing procedures fail
-            then the hooks are not called.
-
-        Parameters
-        -----------
-        coro: :ref:`coroutine <coroutine>`
-            The coroutine to register as the pre-invoke hook.
-
-        Raises
-        -------
-        TypeError
-            The coroutine passed is not actually a coroutine.
-        """
-        if not asyncio.iscoroutinefunction(coro):
-            raise TypeError('The pre-invoke hook must be a coroutine.')
-
-        self._before_invoke = coro
-        return coro
-
-    def after_invoke(self, coro):
-        r"""A decorator that registers a coroutine as a post-invoke hook.
-
-        A post-invoke hook is called directly after the command is
-        called. This makes it a useful function to clean-up database
-        connections or any type of clean up required.
-
-        This post-invoke hook takes a sole parameter, a :class:`.Context`.
-
-        .. note::
-
-            Similar to :meth:`~.Bot.before_invoke`\, this is not called unless
-            checks and argument parsing procedures succeed. This hook is,
-            however, **always** called regardless of the internal command
-            callback raising an error (i.e. :exc:`.CommandInvokeError`\).
-            This makes it ideal for clean-up scenarios.
-
-        Parameters
-        -----------
-        coro: :ref:`coroutine <coroutine>`
-            The coroutine to register as the post-invoke hook.
-
-        Raises
-        -------
-        TypeError
-            The coroutine passed is not actually a coroutine.
-        """
-        if not asyncio.iscoroutinefunction(coro):
-            raise TypeError('The post-invoke hook must be a coroutine.')
-
-        self._after_invoke = coro
-        return coro
-
-    # listener registration
-
-    def add_listener(self, func, name=None):
-        """The non decorator alternative to :meth:`.listen`.
-
-        Parameters
-        -----------
-        func: :ref:`coroutine <coroutine>`
-            The function to call.
-        name: Optional[:class:`str`]
-            The name of the event to listen for. Defaults to ``func.__name__``.
-
-        Example
-        --------
-
-        .. code-block:: python3
-
-            async def on_ready(): pass
-            async def my_message(message): pass
-
-            bot.add_listener(on_ready)
-            bot.add_listener(my_message, 'on_message')
-
-        """
-        name = func.__name__ if name is None else name
-
-        if not asyncio.iscoroutinefunction(func):
-            raise TypeError('Listeners must be coroutines')
-
-        if name in self.extra_events:
-            self.extra_events[name].append(func)
-        else:
-            self.extra_events[name] = [func]
-
-    def remove_listener(self, func, name=None):
-        """Removes a listener from the pool of listeners.
-
-        Parameters
-        -----------
-        func
-            The function that was used as a listener to remove.
-        name: :class:`str`
-            The name of the event we want to remove. Defaults to
-            ``func.__name__``.
-        """
-
-        name = func.__name__ if name is None else name
-
-        if name in self.extra_events:
-            try:
-                self.extra_events[name].remove(func)
-            except ValueError:
-                pass
-
-    def listen(self, name=None):
-        """A decorator that registers another function as an external
-        event listener. Basically this allows you to listen to multiple
-        events from different places e.g. such as :func:`.on_ready`
-
-        The functions being listened to must be a :ref:`coroutine <coroutine>`.
-
-        Example
-        --------
-
-        .. code-block:: python3
-
-            @bot.listen()
-            async def on_message(message):
-                print('one')
-
-            # in some other file...
-
-            @bot.listen('on_message')
-            async def my_message(message):
-                print('two')
-
-        Would print one and two in an unspecified order.
-
-        Raises
-        -------
-        TypeError
-            The function being listened to is not a coroutine.
-        """
-
-        def decorator(func):
-            self.add_listener(func, name)
-            return func
-
-        return decorator
-
-    # cogs
-
-    def add_cog(self, cog):
-        """Adds a "cog" to the bot.
-
-        A cog is a class that has its own event listeners and commands.
-
-        Parameters
-        -----------
-        cog: :class:`.Cog`
-            The cog to register to the bot.
-
-        Raises
-        -------
-        TypeError
-            The cog does not inherit from :class:`.Cog`.
-        CommandError
-            An error happened during loading.
-        """
-
-        if not isinstance(cog, Cog):
-            raise TypeError('cogs must derive from Cog')
-
-        cog = cog._inject(self)
-        self.__cogs[cog.__cog_name__] = cog
-
-    def get_cog(self, name):
-        """Gets the cog instance requested.
-
-        If the cog is not found, ``None`` is returned instead.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The name of the cog you are requesting.
-            This is equivalent to the name passed via keyword
-            argument in class creation or the class name if unspecified.
-
-        Returns
-        --------
-        Optional[:class:`Cog`]
-            The cog that was requested. If not found, returns ``None``.
-        """
-        return self.__cogs.get(name)
-
-    def remove_cog(self, name):
-        """Removes a cog from the bot.
-
-        All registered commands and event listeners that the
-        cog has registered will be removed as well.
-
-        If no cog is found then this method has no effect.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The name of the cog to remove.
-        """
-
-        cog = self.__cogs.pop(name, None)
-        if cog is None:
-            return
-
-        help_command = self._help_command
-        if help_command and help_command.cog is cog:
-            help_command.cog = None
-        cog._eject(self)
-
-    @property
-    def cogs(self):
-        """Mapping[:class:`str`, :class:`Cog`]: A read-only mapping of cog name to cog."""
-        return types.MappingProxyType(self.__cogs)
-
-    # extensions
-
-    def _remove_module_references(self, name):
-        # find all references to the module
-        # remove the cogs registered from the module
-        for cogname, cog in self.__cogs.copy().items():
-            if _is_submodule(name, cog.__module__):
-                self.remove_cog(cogname)
-
-        # remove all the commands from the module
-        for cmd in self.all_commands.copy().values():
-            if cmd.module is not None and _is_submodule(name, cmd.module):
-                if isinstance(cmd, GroupMixin):
-                    cmd.recursively_remove_all_commands()
-                self.remove_command(cmd.name)
-
-        # remove all the listeners from the module
-        for event_list in self.extra_events.copy().values():
-            remove = []
-            for index, event in enumerate(event_list):
-                if event.__module__ is not None and _is_submodule(name, event.__module__):
-                    remove.append(index)
-
-            for index in reversed(remove):
-                del event_list[index]
-
-    def _call_module_finalizers(self, lib, key):
-        try:
-            func = getattr(lib, 'teardown')
-        except AttributeError:
-            pass
-        else:
-            try:
-                func(self)
-            except Exception:
-                pass
-        finally:
-            self.__extensions.pop(key, None)
-            sys.modules.pop(key, None)
-            name = lib.__name__
-            for module in list(sys.modules.keys()):
-                if _is_submodule(name, module):
-                    del sys.modules[module]
-
-    def _load_from_module_spec(self, spec, key):
-        # precondition: key not in self.__extensions
-        lib = importlib.util.module_from_spec(spec)
-        sys.modules[key] = lib
-        try:
-            spec.loader.exec_module(lib)
-        except Exception as e:
-            del sys.modules[key]
-            raise errors.ExtensionFailed(key, e) from e
-
-        try:
-            setup = getattr(lib, 'setup')
-        except AttributeError:
-            del sys.modules[key]
-            raise errors.NoEntryPointError(key)
-
-        try:
-            setup(self)
-        except Exception as e:
-            del sys.modules[key]
-            self._remove_module_references(lib.__name__)
-            self._call_module_finalizers(lib, key)
-            raise errors.ExtensionFailed(key, e) from e
-        else:
-            self.__extensions[key] = lib
-
-    def _resolve_name(self, name, package):
-        try:
-            return importlib.util.resolve_name(name, package)
-        except ImportError:
-            raise errors.ExtensionNotFound(name)
-
-    def load_extension(self, name, *, package=None):
-        """Loads an extension.
-
-        An extension is a python module that contains commands, cogs, or
-        listeners.
-
-        An extension must have a global function, ``setup`` defined as
-        the entry point on what to do when the extension is loaded. This entry
-        point must have a single argument, the ``bot``.
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The extension name to load. It must be dot separated like
-            regular Python imports if accessing a sub-module. e.g.
-            ``foo.test`` if you want to import ``foo/test.py``.
-        package: Optional[:class:`str`]
-            The package name to resolve relative imports with.
-            This is required when loading an extension using a relative path, e.g ``.foo.test``.
-            Defaults to ``None``.
-
-            .. versionadded:: 1.7
-
-        Raises
-        --------
-        ExtensionNotFound
-            The extension could not be imported.
-            This is also raised if the name of the extension could not
-            be resolved using the provided ``package`` parameter.
-        ExtensionAlreadyLoaded
-            The extension is already loaded.
-        NoEntryPointError
-            The extension does not have a setup function.
-        ExtensionFailed
-            The extension or its setup function had an execution error.
-        """
-
-        name = self._resolve_name(name, package)
-        if name in self.__extensions:
-            raise errors.ExtensionAlreadyLoaded(name)
-
-        spec = importlib.util.find_spec(name)
-        if spec is None:
-            raise errors.ExtensionNotFound(name)
-
-        self._load_from_module_spec(spec, name)
-
-    def unload_extension(self, name, *, package=None):
-        """Unloads an extension.
-
-        When the extension is unloaded, all commands, listeners, and cogs are
-        removed from the bot and the module is un-imported.
-
-        The extension can provide an optional global function, ``teardown``,
-        to do miscellaneous clean-up if necessary. This function takes a single
-        parameter, the ``bot``, similar to ``setup`` from
-        :meth:`~.Bot.load_extension`.
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The extension name to unload. It must be dot separated like
-            regular Python imports if accessing a sub-module. e.g.
-            ``foo.test`` if you want to import ``foo/test.py``.
-        package: Optional[:class:`str`]
-            The package name to resolve relative imports with.
-            This is required when unloading an extension using a relative path, e.g ``.foo.test``.
-            Defaults to ``None``.
-
-            .. versionadded:: 1.7
-
-        Raises
-        -------
-        ExtensionNotFound
-            The name of the extension could not
-            be resolved using the provided ``package`` parameter.
-        ExtensionNotLoaded
-            The extension was not loaded.
-        """
-
-        name = self._resolve_name(name, package)
-        lib = self.__extensions.get(name)
-        if lib is None:
-            raise errors.ExtensionNotLoaded(name)
-
-        self._remove_module_references(lib.__name__)
-        self._call_module_finalizers(lib, name)
-
-    def reload_extension(self, name, *, package=None):
-        """Atomically reloads an extension.
-
-        This replaces the extension with the same extension, only refreshed. This is
-        equivalent to a :meth:`unload_extension` followed by a :meth:`load_extension`
-        except done in an atomic way. That is, if an operation fails mid-reload then
-        the bot will roll-back to the prior working state.
-
-        Parameters
-        ------------
-        name: :class:`str`
-            The extension name to reload. It must be dot separated like
-            regular Python imports if accessing a sub-module. e.g.
-            ``foo.test`` if you want to import ``foo/test.py``.
-        package: Optional[:class:`str`]
-            The package name to resolve relative imports with.
-            This is required when reloading an extension using a relative path, e.g ``.foo.test``.
-            Defaults to ``None``.
-
-            .. versionadded:: 1.7
-
-        Raises
-        -------
-        ExtensionNotLoaded
-            The extension was not loaded.
-        ExtensionNotFound
-            The extension could not be imported.
-            This is also raised if the name of the extension could not
-            be resolved using the provided ``package`` parameter.
-        NoEntryPointError
-            The extension does not have a setup function.
-        ExtensionFailed
-            The extension setup function had an execution error.
-        """
-
-        name = self._resolve_name(name, package)
-        lib = self.__extensions.get(name)
-        if lib is None:
-            raise errors.ExtensionNotLoaded(name)
-
-        # get the previous module states from sys modules
-        modules = {
-            name: module
-            for name, module in sys.modules.items()
-            if _is_submodule(lib.__name__, name)
-        }
-
-        try:
-            # Unload and then load the module...
-            self._remove_module_references(lib.__name__)
-            self._call_module_finalizers(lib, name)
-            self.load_extension(name)
-        except Exception:
-            # if the load failed, the remnants should have been
-            # cleaned from the load_extension function call
-            # so let's load it from our old compiled library.
-            lib.setup(self)
-            self.__extensions[name] = lib
-
-            # revert sys.modules back to normal and raise back to caller
-            sys.modules.update(modules)
-            raise
-
-    @property
-    def extensions(self):
-        """Mapping[:class:`str`, :class:`py:types.ModuleType`]: A read-only mapping of extension name to extension."""
-        return types.MappingProxyType(self.__extensions)
-
-    # help command stuff
-
-    @property
-    def help_command(self):
-        return self._help_command
-
-    @help_command.setter
-    def help_command(self, value):
-        if value is not None:
-            if not isinstance(value, HelpCommand):
-                raise TypeError('help_command must be a subclass of HelpCommand')
-            if self._help_command is not None:
-                self._help_command._remove_from_bot(self)
-            self._help_command = value
-            value._add_to_bot(self)
-        elif self._help_command is not None:
-            self._help_command._remove_from_bot(self)
-            self._help_command = None
-        else:
-            self._help_command = None
-
-    # command processing
-
-    async def get_prefix(self, message):
-        """|coro|
-
-        Retrieves the prefix the bot is listening to
-        with the message as a context.
-
-        Parameters
-        -----------
-        message: :class:`discord.Message`
-            The message context to get the prefix of.
-
-        Returns
-        --------
-        Union[List[:class:`str`], :class:`str`]
-            A list of prefixes or a single prefix that the bot is
-            listening for.
-        """
-        prefix = ret = self.command_prefix
-        if callable(prefix):
-            ret = await discord.utils.maybe_coroutine(prefix, self, message)
-
-        if not isinstance(ret, str):
-            try:
-                ret = list(ret)
-            except TypeError:
-                # It's possible that a generator raised this exception.  Don't
-                # replace it with our own error if that's the case.
-                if isinstance(ret, collections.abc.Iterable):
-                    raise
-
-                raise TypeError("command_prefix must be plain string, iterable of strings, or callable "
-                                "returning either of these, not {}".format(ret.__class__.__name__))
-
-            if not ret:
-                raise ValueError("Iterable command_prefix must contain at least one prefix")
-
-        return ret
-
-    async def get_context(self, message, *, cls=Context):
-        r"""|coro|
-
-        Returns the invocation context from the message.
-
-        This is a more low-level counter-part for :meth:`.process_commands`
-        to allow users more fine grained control over the processing.
-
-        The returned context is not guaranteed to be a valid invocation
-        context, :attr:`.Context.valid` must be checked to make sure it is.
-        If the context is not valid then it is not a valid candidate to be
-        invoked under :meth:`~.Bot.invoke`.
-
-        Parameters
-        -----------
-        message: :class:`discord.Message`
-            The message to get the invocation context from.
-        cls
-            The factory class that will be used to create the context.
-            By default, this is :class:`.Context`. Should a custom
-            class be provided, it must be similar enough to :class:`.Context`\'s
-            interface.
-
-        Returns
-        --------
-        :class:`.Context`
-            The invocation context. The type of this can change via the
-            ``cls`` parameter.
-        """
-
-        view = StringView(message.content)
-        ctx = cls(prefix=None, view=view, bot=self, message=message)
-
-        if self._skip_check(message.author.id, self.user.id):
-            return ctx
-
-        prefix = await self.get_prefix(message)
-        invoked_prefix = prefix
-
-        if isinstance(prefix, str):
-            if not view.skip_string(prefix):
-                return ctx
-        else:
-            try:
-                # if the context class' __init__ consumes something from the view this
-                # will be wrong.  That seems unreasonable though.
-                if message.content.startswith(tuple(prefix)):
-                    invoked_prefix = discord.utils.find(view.skip_string, prefix)
-                else:
-                    return ctx
-
-            except TypeError:
-                if not isinstance(prefix, list):
-                    raise TypeError("get_prefix must return either a string or a list of string, "
-                                    "not {}".format(prefix.__class__.__name__))
-
-                # It's possible a bad command_prefix got us here.
-                for value in prefix:
-                    if not isinstance(value, str):
-                        raise TypeError("Iterable command_prefix or list returned from get_prefix must "
-                                        "contain only strings, not {}".format(value.__class__.__name__))
-
-                # Getting here shouldn't happen
-                raise
-
-        if self.strip_after_prefix:
-            view.skip_ws()
-
-        invoker = view.get_word()
-        ctx.invoked_with = invoker
-        ctx.prefix = invoked_prefix
-        ctx.command = self.all_commands.get(invoker)
-        return ctx
-
-    async def invoke(self, ctx):
-        """|coro|
-
-        Invokes the command given under the invocation context and
-        handles all the internal event dispatch mechanisms.
-
-        Parameters
-        -----------
-        ctx: :class:`.Context`
-            The invocation context to invoke.
-        """
-        if ctx.command is not None:
-            self.dispatch('command', ctx)
-            try:
-                if await self.can_run(ctx, call_once=True):
-                    await ctx.command.invoke(ctx)
-                else:
-                    raise errors.CheckFailure('The global check once functions failed.')
-            except errors.CommandError as exc:
-                await ctx.command.dispatch_error(ctx, exc)
-            else:
-                self.dispatch('command_completion', ctx)
-        elif ctx.invoked_with:
-            exc = errors.CommandNotFound('Command "{}" is not found'.format(ctx.invoked_with))
-            self.dispatch('command_error', ctx, exc)
-
-    async def process_commands(self, message):
-        """|coro|
-
-        This function processes the commands that have been registered
-        to the bot and other groups. Without this coroutine, none of the
-        commands will be triggered.
-
-        By default, this coroutine is called inside the :func:`.on_message`
-        event. If you choose to override the :func:`.on_message` event, then
-        you should invoke this coroutine as well.
-
-        This is built using other low level tools, and is equivalent to a
-        call to :meth:`~.Bot.get_context` followed by a call to :meth:`~.Bot.invoke`.
-
-        This also checks if the message's author is a bot and doesn't
-        call :meth:`~.Bot.get_context` or :meth:`~.Bot.invoke` if so.
-
-        Parameters
-        -----------
-        message: :class:`discord.Message`
-            The message to process commands for.
-        """
-        if message.author.bot:
-            return
-
-        ctx = await self.get_context(message)
-        await self.invoke(ctx)
-
-    async def on_message(self, message):
-        await self.process_commands(message)
-
-class Bot(BotBase, discord.Client):
-    """Represents a discord bot.
-
-    This class is a subclass of :class:`discord.Client` and as a result
-    anything that you can do with a :class:`discord.Client` you can do with
-    this bot.
-
-    This class also subclasses :class:`.GroupMixin` to provide the functionality
-    to manage commands.
-
-    Attributes
-    -----------
-    command_prefix
-        The command prefix is what the message content must contain initially
-        to have a command invoked. This prefix could either be a string to
-        indicate what the prefix should be, or a callable that takes in the bot
-        as its first parameter and :class:`discord.Message` as its second
-        parameter and returns the prefix. This is to facilitate "dynamic"
-        command prefixes. This callable can be either a regular function or
-        a coroutine.
-
-        An empty string as the prefix always matches, enabling prefix-less
-        command invocation. While this may be useful in DMs it should be avoided
-        in servers, as it's likely to cause performance issues and unintended
-        command invocations.
-
-        The command prefix could also be an iterable of strings indicating that
-        multiple checks for the prefix should be used and the first one to
-        match will be the invocation prefix. You can get this prefix via
-        :attr:`.Context.prefix`. To avoid confusion empty iterables are not
-        allowed.
-
-        .. note::
-
-            When passing multiple prefixes be careful to not pass a prefix
-            that matches a longer prefix occurring later in the sequence.  For
-            example, if the command prefix is ``('!', '!?')``  the ``'!?'``
-            prefix will never be matched to any message as the previous one
-            matches messages starting with ``!?``. This is especially important
-            when passing an empty string, it should always be last as no prefix
-            after it will be matched.
-    case_insensitive: :class:`bool`
-        Whether the commands should be case insensitive. Defaults to ``False``. This
-        attribute does not carry over to groups. You must set it to every group if
-        you require group commands to be case insensitive as well.
-    description: :class:`str`
-        The content prefixed into the default help message.
-    self_bot: :class:`bool`
-        If ``True``, the bot will only listen to commands invoked by itself rather
-        than ignoring itself. If ``False`` (the default) then the bot will ignore
-        itself. This cannot be changed once initialised.
-    help_command: Optional[:class:`.HelpCommand`]
-        The help command implementation to use. This can be dynamically
-        set at runtime. To remove the help command pass ``None``. For more
-        information on implementing a help command, see :ref:`ext_commands_help_command`.
-    owner_id: Optional[:class:`int`]
-        The user ID that owns the bot. If this is not set and is then queried via
-        :meth:`.is_owner` then it will error.
-    owner_ids: Optional[Collection[:class:`int`]]
-        The user IDs that owns the bot. This is similar to :attr:`owner_id`.
-        For performance reasons it is recommended to use a :class:`set`
-        for the collection. You cannot set both ``owner_id`` and ``owner_ids``.
-
-        .. versionadded:: 1.3
-    strip_after_prefix: :class:`bool`
-        Whether to strip whitespace characters after encountering the command
-        prefix. This allows for ``!   hello`` and ``!hello`` to both work if
-        the ``command_prefix`` is set to ``!``. Defaults to ``False``.
-
-        .. versionadded:: 1.7
-    """
-    pass
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+
+import asyncio
+import collections
+import collections.abc
+import inspect
+import importlib.util
+import sys
+import logging
+import types
+from typing import (
+    Any,
+    Callable,
+    Mapping,
+    List,
+    Dict,
+    TYPE_CHECKING,
+    Optional,
+    TypeVar,
+    Type,
+    Union,
+    Iterable,
+    Collection,
+    overload,
+)
+
+import discord
+from discord.utils import MISSING, _is_submodule
+
+from .core import GroupMixin
+from .view import StringView
+from .context import Context
+from . import errors
+from .help import HelpCommand, DefaultHelpCommand
+from .cog import Cog
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    import importlib.machinery
+
+    from discord.message import Message
+    from discord.abc import User
+    from ._types import (
+        _Bot,
+        BotT,
+        UserCheck,
+        CoroFunc,
+        ContextT,
+        MaybeAwaitableFunc,
+    )
+
+    _Prefix = Union[Iterable[str], str]
+    _PrefixCallable = MaybeAwaitableFunc[[BotT, Message], _Prefix]
+    PrefixType = Union[_Prefix, _PrefixCallable[BotT]]
+
+__all__ = (
+    'when_mentioned',
+    'when_mentioned_or',
+    'Bot',
+)
+
+T = TypeVar('T')
+CFT = TypeVar('CFT', bound='CoroFunc')
+
+_log = logging.getLogger(__name__)
+
+
+def when_mentioned(bot: _Bot, msg: Message, /) -> List[str]:
+    """A callable that implements a command prefix equivalent to being mentioned.
+
+    These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
+
+        .. versionchanged:: 2.0
+
+            ``bot`` and ``msg`` parameters are now positional-only.
+    """
+    # bot.user will never be None when this is called
+    return [f'<@{bot.user.id}> ', f'<@!{bot.user.id}> ']  # type: ignore
+
+
+def when_mentioned_or(*prefixes: str) -> Callable[[_Bot, Message], List[str]]:
+    """A callable that implements when mentioned or other prefixes provided.
+
+    These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
+
+    Example
+    --------
+
+    .. code-block:: python3
+
+        bot = commands.Bot(command_prefix=commands.when_mentioned_or('!'))
+
+
+    .. note::
+
+        This callable returns another callable, so if this is done inside a custom
+        callable, you must call the returned callable, for example:
+
+        .. code-block:: python3
+
+            async def get_prefix(bot, message):
+                extras = await prefixes_for(message.guild) # returns a list
+                return commands.when_mentioned_or(*extras)(bot, message)
+
+
+    See Also
+    ----------
+    :func:`.when_mentioned`
+    """
+
+    def inner(bot, msg):
+        r = list(prefixes)
+        r = when_mentioned(bot, msg) + r
+        return r
+
+    return inner
+
+
+class _DefaultRepr:
+    def __repr__(self):
+        return '<default-help-command>'
+
+
+_default: Any = _DefaultRepr()
+
+
+class BotBase(GroupMixin[None]):
+    def __init__(
+        self,
+        command_prefix: PrefixType[BotT],
+        help_command: Optional[HelpCommand] = _default,
+        description: Optional[str] = None,
+        **options: Any,
+    ) -> None:
+        super().__init__(**options)
+        self.command_prefix: PrefixType[BotT] = command_prefix
+        self.extra_events: Dict[str, List[CoroFunc]] = {}
+        self.__cogs: Dict[str, Cog] = {}
+        self.__extensions: Dict[str, types.ModuleType] = {}
+        self._checks: List[UserCheck] = []
+        self._check_once: List[UserCheck] = []
+        self._before_invoke: Optional[CoroFunc] = None
+        self._after_invoke: Optional[CoroFunc] = None
+        self._help_command: Optional[HelpCommand] = None
+        self.description: str = inspect.cleandoc(description) if description else ''
+        self.owner_id: Optional[int] = options.get('owner_id')
+        self.owner_ids: Optional[Collection[int]] = options.get('owner_ids', set())
+        self.strip_after_prefix: bool = options.get('strip_after_prefix', False)
+
+        if self.owner_id and self.owner_ids:
+            raise TypeError('Both owner_id and owner_ids are set')
+
+        if self.owner_ids and not isinstance(self.owner_ids, collections.abc.Collection):
+            raise TypeError(f'owner_ids must be a collection not {self.owner_ids.__class__!r}')
+
+        self_bot = options.get('self_bot', False)
+        user_bot = options.get('user_bot', False)
+
+        if self_bot and user_bot:
+            raise TypeError('Both self_bot and user_bot are set')
+
+        if self_bot:
+            self._skip_check = lambda x, y: x != y
+        elif user_bot:
+            self._skip_check = lambda *_: False
+        else:
+            self._skip_check = lambda x, y: x == y
+
+        if help_command is _default:
+            self.help_command = DefaultHelpCommand()
+        else:
+            self.help_command = help_command
+
+    # internal helpers
+
+    def dispatch(self, event_name: str, /, *args: Any, **kwargs: Any) -> None:
+        # super() will resolve to Client
+        super().dispatch(event_name, *args, **kwargs)  # type: ignore
+        ev = 'on_' + event_name
+        for event in self.extra_events.get(ev, []):
+            self._schedule_event(event, ev, *args, **kwargs)  # type: ignore
+
+    @discord.utils.copy_doc(discord.Client.close)
+    async def close(self) -> None:
+        for extension in tuple(self.__extensions):
+            try:
+                await self.unload_extension(extension)
+            except Exception:
+                pass
+
+        for cog in tuple(self.__cogs):
+            try:
+                await self.remove_cog(cog)
+            except Exception:
+                pass
+
+        await super().close()  # type: ignore
+
+    async def on_command_error(self, context: Context[BotT], exception: errors.CommandError, /) -> None:
+        """|coro|
+
+        The default command error handler provided by the bot.
+
+        By default this logs to the library logger, however it could be
+        overridden to have a different implementation.
+
+        This only fires if you do not specify any listeners for command error.
+
+        .. versionchanged:: 2.0
+
+            ``context`` and ``exception`` parameters are now positional-only.
+            Instead of writing to ``sys.stderr`` this now uses the library logger.
+        """
+        if self.extra_events.get('on_command_error', None):
+            return
+
+        command = context.command
+        if command and command.has_error_handler():
+            return
+
+        cog = context.cog
+        if cog and cog.has_error_handler():
+            return
+
+        _log.error('Ignoring exception in command %s', command, exc_info=exception)
+
+    # global check registration
+
+    def check(self, func: T, /) -> T:
+        r"""A decorator that adds a global check to the bot.
+
+        A global check is similar to a :func:`.check` that is applied
+        on a per command basis except it is run before any command checks
+        have been verified and applies to every command the bot has.
+
+        .. note::
+
+            This function can either be a regular function or a coroutine.
+
+        Similar to a command :func:`.check`\, this takes a single parameter
+        of type :class:`.Context` and can only raise exceptions inherited from
+        :exc:`.CommandError`.
+
+        Example
+        ---------
+
+        .. code-block:: python3
+
+            @bot.check
+            def check_commands(ctx):
+                return ctx.command.qualified_name in allowed_commands
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+        """
+        # T was used instead of Check to ensure the type matches on return
+        self.add_check(func)  # type: ignore
+        return func
+
+    def add_check(self, func: UserCheck[ContextT], /, *, call_once: bool = False) -> None:
+        """Adds a global check to the bot.
+
+        This is the non-decorator interface to :meth:`.check`
+        and :meth:`.check_once`.
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        func
+            The function that was used as a global check.
+        call_once: :class:`bool`
+            If the function should only be called once per
+            :meth:`.invoke` call.
+        """
+
+        if call_once:
+            self._check_once.append(func)
+        else:
+            self._checks.append(func)
+
+    def remove_check(self, func: UserCheck[ContextT], /, *, call_once: bool = False) -> None:
+        """Removes a global check from the bot.
+
+        This function is idempotent and will not raise an exception
+        if the function is not in the global checks.
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        func
+            The function to remove from the global checks.
+        call_once: :class:`bool`
+            If the function was added with ``call_once=True`` in
+            the :meth:`.Bot.add_check` call or using :meth:`.check_once`.
+        """
+        l = self._check_once if call_once else self._checks
+
+        try:
+            l.remove(func)
+        except ValueError:
+            pass
+
+    def check_once(self, func: CFT, /) -> CFT:
+        r"""A decorator that adds a "call once" global check to the bot.
+
+        Unlike regular global checks, this one is called only once
+        per :meth:`.invoke` call.
+
+        Regular global checks are called whenever a command is called
+        or :meth:`.Command.can_run` is called. This type of check
+        bypasses that and ensures that it's called only once, even inside
+        the default help command.
+
+        .. note::
+
+            When using this function the :class:`.Context` sent to a group subcommand
+            may only parse the parent command and not the subcommands due to it
+            being invoked once per :meth:`.Bot.invoke` call.
+
+        .. note::
+
+            This function can either be a regular function or a coroutine.
+
+        Similar to a command :func:`.check`\, this takes a single parameter
+        of type :class:`.Context` and can only raise exceptions inherited from
+        :exc:`.CommandError`.
+
+        Example
+        ---------
+
+        .. code-block:: python3
+
+            @bot.check_once
+            def whitelist(ctx):
+                return ctx.message.author.id in my_whitelist
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        """
+        self.add_check(func, call_once=True)
+        return func
+
+    async def can_run(self, ctx: Context[BotT], /, *, call_once: bool = False) -> bool:
+        data = self._check_once if call_once else self._checks
+
+        if len(data) == 0:
+            return True
+
+        return await discord.utils.async_all(f(ctx) for f in data)
+
+    async def is_owner(self, user: User, /) -> bool:
+        """|coro|
+
+        Checks if a :class:`~discord.User` or :class:`~discord.Member` is the owner of
+        this bot.
+
+        .. versionchanged:: 2.0
+            ``user`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        user: :class:`.abc.User`
+            The user to check for.
+
+        Raises
+        -------
+        AttributeError
+            Owners aren't set.
+
+        Returns
+        --------
+        :class:`bool`
+            Whether the user is the owner.
+        """
+        if self.owner_id:
+            return user.id == self.owner_id
+        elif self.owner_ids:
+            return user.id in self.owner_ids
+        else:
+            raise AttributeError('Owners aren\'t set.')
+
+    def before_invoke(self, coro: CFT, /) -> CFT:
+        """A decorator that registers a coroutine as a pre-invoke hook.
+
+        A pre-invoke hook is called directly before the command is
+        called. This makes it a useful function to set up database
+        connections or any type of set up required.
+
+        This pre-invoke hook takes a sole parameter, a :class:`.Context`.
+
+        .. note::
+
+            The :meth:`~.Bot.before_invoke` and :meth:`~.Bot.after_invoke` hooks are
+            only called if all checks and argument parsing procedures pass
+            without error. If any check or argument parsing procedures fail
+            then the hooks are not called.
+
+        .. versionchanged:: 2.0
+
+            ``coro`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        coro: :ref:`coroutine <coroutine>`
+            The coroutine to register as the pre-invoke hook.
+
+        Raises
+        -------
+        TypeError
+            The coroutine passed is not actually a coroutine.
+        """
+        if not asyncio.iscoroutinefunction(coro):
+            raise TypeError('The pre-invoke hook must be a coroutine.')
+
+        self._before_invoke = coro
+        return coro
+
+    def after_invoke(self, coro: CFT, /) -> CFT:
+        r"""A decorator that registers a coroutine as a post-invoke hook.
+
+        A post-invoke hook is called directly after the command is
+        called. This makes it a useful function to clean-up database
+        connections or any type of clean up required.
+
+        This post-invoke hook takes a sole parameter, a :class:`.Context`.
+
+        .. note::
+
+            Similar to :meth:`~.Bot.before_invoke`\, this is not called unless
+            checks and argument parsing procedures succeed. This hook is,
+            however, **always** called regardless of the internal command
+            callback raising an error (i.e. :exc:`.CommandInvokeError`\).
+            This makes it ideal for clean-up scenarios.
+
+        .. versionchanged:: 2.0
+
+            ``coro`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        coro: :ref:`coroutine <coroutine>`
+            The coroutine to register as the post-invoke hook.
+
+        Raises
+        -------
+        TypeError
+            The coroutine passed is not actually a coroutine.
+        """
+        if not asyncio.iscoroutinefunction(coro):
+            raise TypeError('The post-invoke hook must be a coroutine.')
+
+        self._after_invoke = coro
+        return coro
+
+    # listener registration
+
+    def add_listener(self, func: CoroFunc, /, name: str = MISSING) -> None:
+        """The non decorator alternative to :meth:`.listen`.
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        func: :ref:`coroutine <coroutine>`
+            The function to call.
+        name: :class:`str`
+            The name of the event to listen for. Defaults to ``func.__name__``.
+
+        Example
+        --------
+
+        .. code-block:: python3
+
+            async def on_ready(): pass
+            async def my_message(message): pass
+
+            bot.add_listener(on_ready)
+            bot.add_listener(my_message, 'on_message')
+
+        """
+        name = func.__name__ if name is MISSING else name
+
+        if not asyncio.iscoroutinefunction(func):
+            raise TypeError('Listeners must be coroutines')
+
+        if name in self.extra_events:
+            self.extra_events[name].append(func)
+        else:
+            self.extra_events[name] = [func]
+
+    def remove_listener(self, func: CoroFunc, /, name: str = MISSING) -> None:
+        """Removes a listener from the pool of listeners.
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        func
+            The function that was used as a listener to remove.
+        name: :class:`str`
+            The name of the event we want to remove. Defaults to
+            ``func.__name__``.
+        """
+
+        name = func.__name__ if name is MISSING else name
+
+        if name in self.extra_events:
+            try:
+                self.extra_events[name].remove(func)
+            except ValueError:
+                pass
+
+    def listen(self, name: str = MISSING) -> Callable[[CFT], CFT]:
+        """A decorator that registers another function as an external
+        event listener. Basically this allows you to listen to multiple
+        events from different places e.g. such as :func:`.on_ready`
+
+        The functions being listened to must be a :ref:`coroutine <coroutine>`.
+
+        Example
+        --------
+
+        .. code-block:: python3
+
+            @bot.listen()
+            async def on_message(message):
+                print('one')
+
+            # in some other file...
+
+            @bot.listen('on_message')
+            async def my_message(message):
+                print('two')
+
+        Would print one and two in an unspecified order.
+
+        Raises
+        -------
+        TypeError
+            The function being listened to is not a coroutine.
+        """
+
+        def decorator(func: CFT) -> CFT:
+            self.add_listener(func, name)
+            return func
+
+        return decorator
+
+    # cogs
+
+    async def add_cog(
+        self,
+        cog: Cog,
+        /,
+        *,
+        override: bool = False,
+    ) -> None:
+        """|coro|
+
+        Adds a "cog" to the bot.
+
+        A cog is a class that has its own event listeners and commands.
+
+        .. note::
+
+            Exceptions raised inside a :class:`.Cog`'s :meth:`~.Cog.cog_load` method will be
+            propagated to the caller.
+
+        .. versionchanged:: 2.0
+
+            :exc:`.ClientException` is raised when a cog with the same name
+            is already loaded.
+
+        .. versionchanged:: 2.0
+
+            ``cog`` parameter is now positional-only.
+
+        .. versionchanged:: 2.0
+
+            This method is now a :term:`coroutine`.
+
+        Parameters
+        -----------
+        cog: :class:`.Cog`
+            The cog to register to the bot.
+        override: :class:`bool`
+            If a previously loaded cog with the same name should be ejected
+            instead of raising an error.
+
+            .. versionadded:: 2.0
+
+        Raises
+        -------
+        TypeError
+            The cog does not inherit from :class:`.Cog`.
+        CommandError
+            An error happened during loading.
+        ClientException
+            A cog with the same name is already loaded.
+        """
+
+        if not isinstance(cog, Cog):
+            raise TypeError('cogs must derive from Cog')
+
+        cog_name = cog.__cog_name__
+        existing = self.__cogs.get(cog_name)
+
+        if existing is not None:
+            if not override:
+                raise discord.ClientException(f'Cog named {cog_name!r} already loaded')
+            await self.remove_cog(cog_name)
+
+        cog = await cog._inject(self, override=override)
+        self.__cogs[cog_name] = cog
+
+    def get_cog(self, name: str, /) -> Optional[Cog]:
+        """Gets the cog instance requested.
+
+        If the cog is not found, ``None`` is returned instead.
+
+        .. versionchanged:: 2.0
+
+            ``name`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the cog you are requesting.
+            This is equivalent to the name passed via keyword
+            argument in class creation or the class name if unspecified.
+
+        Returns
+        --------
+        Optional[:class:`Cog`]
+            The cog that was requested. If not found, returns ``None``.
+        """
+        return self.__cogs.get(name)
+
+    async def remove_cog(
+        self,
+        name: str,
+        /,
+    ) -> Optional[Cog]:
+        """|coro|
+
+        Removes a cog from the bot and returns it.
+
+        All registered commands and event listeners that the
+        cog has registered will be removed as well.
+
+        If no cog is found then this method has no effect.
+
+        .. versionchanged:: 2.0
+
+            ``name`` parameter is now positional-only.
+
+        .. versionchanged:: 2.0
+
+            This method is now a :term:`coroutine`.
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the cog to remove.
+
+        Returns
+        -------
+        Optional[:class:`.Cog`]
+             The cog that was removed. ``None`` if not found.
+        """
+
+        cog = self.__cogs.pop(name, None)
+        if cog is None:
+            return
+
+        help_command = self._help_command
+        if help_command and help_command.cog is cog:
+            help_command.cog = None
+
+        await cog._eject(self)
+
+        return cog
+
+    @property
+    def cogs(self) -> Mapping[str, Cog]:
+        """Mapping[:class:`str`, :class:`Cog`]: A read-only mapping of cog name to cog."""
+        return types.MappingProxyType(self.__cogs)
+
+    # extensions
+
+    async def _remove_module_references(self, name: str) -> None:
+        # find all references to the module
+        # remove the cogs registered from the module
+        for cogname, cog in self.__cogs.copy().items():
+            if _is_submodule(name, cog.__module__):
+                await self.remove_cog(cogname)
+
+        # remove all the commands from the module
+        for cmd in self.all_commands.copy().values():
+            if cmd.module is not None and _is_submodule(name, cmd.module):
+                if isinstance(cmd, GroupMixin):
+                    cmd.recursively_remove_all_commands()
+                self.remove_command(cmd.name)
+
+        # remove all the listeners from the module
+        for event_list in self.extra_events.copy().values():
+            remove = []
+            for index, event in enumerate(event_list):
+                if event.__module__ is not None and _is_submodule(name, event.__module__):
+                    remove.append(index)
+
+            for index in reversed(remove):
+                del event_list[index]
+
+    async def _call_module_finalizers(self, lib: types.ModuleType, key: str) -> None:
+        try:
+            func = getattr(lib, 'teardown')
+        except AttributeError:
+            pass
+        else:
+            try:
+                await func(self)
+            except Exception:
+                pass
+        finally:
+            self.__extensions.pop(key, None)
+            sys.modules.pop(key, None)
+            name = lib.__name__
+            for module in list(sys.modules.keys()):
+                if _is_submodule(name, module):
+                    del sys.modules[module]
+
+    async def _load_from_module_spec(self, spec: importlib.machinery.ModuleSpec, key: str) -> None:
+        # precondition: key not in self.__extensions
+        lib = importlib.util.module_from_spec(spec)
+        sys.modules[key] = lib
+        try:
+            spec.loader.exec_module(lib)  # type: ignore
+        except Exception as e:
+            del sys.modules[key]
+            raise errors.ExtensionFailed(key, e) from e
+
+        try:
+            setup = getattr(lib, 'setup')
+        except AttributeError:
+            del sys.modules[key]
+            raise errors.NoEntryPointError(key)
+
+        try:
+            await setup(self)
+        except Exception as e:
+            del sys.modules[key]
+            await self._remove_module_references(lib.__name__)
+            await self._call_module_finalizers(lib, key)
+            raise errors.ExtensionFailed(key, e) from e
+        else:
+            self.__extensions[key] = lib
+
+    def _resolve_name(self, name: str, package: Optional[str]) -> str:
+        try:
+            return importlib.util.resolve_name(name, package)
+        except ImportError:
+            raise errors.ExtensionNotFound(name)
+
+    async def load_extension(self, name: str, *, package: Optional[str] = None) -> None:
+        """|coro|
+
+        Loads an extension.
+
+        An extension is a python module that contains commands, cogs, or
+        listeners.
+
+        An extension must have a global function, ``setup`` defined as
+        the entry point on what to do when the extension is loaded. This entry
+        point must have a single argument, the ``bot``.
+
+        .. versionchanged:: 2.0
+
+            This method is now a :term:`coroutine`.
+
+        Parameters
+        ------------
+        name: :class:`str`
+            The extension name to load. It must be dot separated like
+            regular Python imports if accessing a sub-module. e.g.
+            ``foo.test`` if you want to import ``foo/test.py``.
+        package: Optional[:class:`str`]
+            The package name to resolve relative imports with.
+            This is required when loading an extension using a relative path, e.g ``.foo.test``.
+            Defaults to ``None``.
+
+            .. versionadded:: 1.7
+
+        Raises
+        --------
+        ExtensionNotFound
+            The extension could not be imported.
+            This is also raised if the name of the extension could not
+            be resolved using the provided ``package`` parameter.
+        ExtensionAlreadyLoaded
+            The extension is already loaded.
+        NoEntryPointError
+            The extension does not have a setup function.
+        ExtensionFailed
+            The extension or its setup function had an execution error.
+        """
+
+        name = self._resolve_name(name, package)
+        if name in self.__extensions:
+            raise errors.ExtensionAlreadyLoaded(name)
+
+        spec = importlib.util.find_spec(name)
+        if spec is None:
+            raise errors.ExtensionNotFound(name)
+
+        await self._load_from_module_spec(spec, name)
+
+    async def unload_extension(self, name: str, *, package: Optional[str] = None) -> None:
+        """|coro|
+
+        Unloads an extension.
+
+        When the extension is unloaded, all commands, listeners, and cogs are
+        removed from the bot and the module is un-imported.
+
+        The extension can provide an optional global function, ``teardown``,
+        to do miscellaneous clean-up if necessary. This function takes a single
+        parameter, the ``bot``, similar to ``setup`` from
+        :meth:`~.Bot.load_extension`.
+
+        .. versionchanged:: 2.0
+
+            This method is now a :term:`coroutine`.
+
+        Parameters
+        ------------
+        name: :class:`str`
+            The extension name to unload. It must be dot separated like
+            regular Python imports if accessing a sub-module. e.g.
+            ``foo.test`` if you want to import ``foo/test.py``.
+        package: Optional[:class:`str`]
+            The package name to resolve relative imports with.
+            This is required when unloading an extension using a relative path, e.g ``.foo.test``.
+            Defaults to ``None``.
+
+            .. versionadded:: 1.7
+
+        Raises
+        -------
+        ExtensionNotFound
+            The name of the extension could not
+            be resolved using the provided ``package`` parameter.
+        ExtensionNotLoaded
+            The extension was not loaded.
+        """
+
+        name = self._resolve_name(name, package)
+        lib = self.__extensions.get(name)
+        if lib is None:
+            raise errors.ExtensionNotLoaded(name)
+
+        await self._remove_module_references(lib.__name__)
+        await self._call_module_finalizers(lib, name)
+
+    async def reload_extension(self, name: str, *, package: Optional[str] = None) -> None:
+        """|coro|
+
+        Atomically reloads an extension.
+
+        This replaces the extension with the same extension, only refreshed. This is
+        equivalent to a :meth:`unload_extension` followed by a :meth:`load_extension`
+        except done in an atomic way. That is, if an operation fails mid-reload then
+        the bot will roll-back to the prior working state.
+
+        Parameters
+        ------------
+        name: :class:`str`
+            The extension name to reload. It must be dot separated like
+            regular Python imports if accessing a sub-module. e.g.
+            ``foo.test`` if you want to import ``foo/test.py``.
+        package: Optional[:class:`str`]
+            The package name to resolve relative imports with.
+            This is required when reloading an extension using a relative path, e.g ``.foo.test``.
+            Defaults to ``None``.
+
+            .. versionadded:: 1.7
+
+        Raises
+        -------
+        ExtensionNotLoaded
+            The extension was not loaded.
+        ExtensionNotFound
+            The extension could not be imported.
+            This is also raised if the name of the extension could not
+            be resolved using the provided ``package`` parameter.
+        NoEntryPointError
+            The extension does not have a setup function.
+        ExtensionFailed
+            The extension setup function had an execution error.
+        """
+
+        name = self._resolve_name(name, package)
+        lib = self.__extensions.get(name)
+        if lib is None:
+            raise errors.ExtensionNotLoaded(name)
+
+        # get the previous module states from sys modules
+        # fmt: off
+        modules = {
+            name: module
+            for name, module in sys.modules.items()
+            if _is_submodule(lib.__name__, name)
+        }
+        # fmt: on
+
+        try:
+            # Unload and then load the module...
+            await self._remove_module_references(lib.__name__)
+            await self._call_module_finalizers(lib, name)
+            await self.load_extension(name)
+        except Exception:
+            # if the load failed, the remnants should have been
+            # cleaned from the load_extension function call
+            # so let's load it from our old compiled library.
+            await lib.setup(self)
+            self.__extensions[name] = lib
+
+            # revert sys.modules back to normal and raise back to caller
+            sys.modules.update(modules)
+            raise
+
+    @property
+    def extensions(self) -> Mapping[str, types.ModuleType]:
+        """Mapping[:class:`str`, :class:`py:types.ModuleType`]: A read-only mapping of extension name to extension."""
+        return types.MappingProxyType(self.__extensions)
+
+    # help command stuff
+
+    @property
+    def help_command(self) -> Optional[HelpCommand]:
+        return self._help_command
+
+    @help_command.setter
+    def help_command(self, value: Optional[HelpCommand]) -> None:
+        if value is not None:
+            if not isinstance(value, HelpCommand):
+                raise TypeError('help_command must be a subclass of HelpCommand')
+            if self._help_command is not None:
+                self._help_command._remove_from_bot(self)
+            self._help_command = value
+            value._add_to_bot(self)
+        elif self._help_command is not None:
+            self._help_command._remove_from_bot(self)
+            self._help_command = None
+        else:
+            self._help_command = None
+
+    # command processing
+
+    async def get_prefix(self, message: Message, /) -> Union[List[str], str]:
+        """|coro|
+
+        Retrieves the prefix the bot is listening to
+        with the message as a context.
+
+        .. versionchanged:: 2.0
+
+            ``message`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        message: :class:`discord.Message`
+            The message context to get the prefix of.
+
+        Returns
+        --------
+        Union[List[:class:`str`], :class:`str`]
+            A list of prefixes or a single prefix that the bot is
+            listening for.
+        """
+        prefix = ret = self.command_prefix
+
+        if callable(prefix):
+            # self will be a Bot or AutoShardedBot
+            ret = await discord.utils.maybe_coroutine(prefix, self, message)  # type: ignore
+
+        if not isinstance(ret, str):
+            try:
+                ret = list(ret)  # type: ignore
+            except TypeError:
+                # It's possible that a generator raised this exception.  Don't
+                # replace it with our own error if that's the case.
+                if isinstance(ret, collections.abc.Iterable):
+                    raise
+
+                raise TypeError(
+                    "command_prefix must be plain string, iterable of strings, or callable "
+                    f"returning either of these, not {ret.__class__.__name__}"
+                )
+
+        return ret
+
+    @overload
+    async def get_context(
+        self,
+        message: Message,
+        /,
+    ) -> Context[Self]:  # type: ignore
+        ...
+
+    @overload
+    async def get_context(
+        self,
+        message: Message,
+        /,
+        *,
+        cls: Type[ContextT] = ...,
+    ) -> ContextT:
+        ...
+
+    async def get_context(
+        self,
+        message: Message,
+        /,
+        *,
+        cls: Type[ContextT] = MISSING,
+    ) -> Any:
+        r"""|coro|
+
+        Returns the invocation context from the message.
+
+        This is a more low-level counter-part for :meth:`.process_commands`
+        to allow users more fine grained control over the processing.
+
+        The returned context is not guaranteed to be a valid invocation
+        context, :attr:`.Context.valid` must be checked to make sure it is.
+        If the context is not valid then it is not a valid candidate to be
+        invoked under :meth:`~.Bot.invoke`.
+
+        .. versionchanged:: 2.0
+
+            ``message`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        message: :class:`discord.Message`
+            The message to get the invocation context from.
+        cls
+            The factory class that will be used to create the context.
+            By default, this is :class:`.Context`. Should a custom
+            class be provided, it must be similar enough to :class:`.Context`\'s
+            interface.
+
+        Returns
+        --------
+        :class:`.Context`
+            The invocation context. The type of this can change via the
+            ``cls`` parameter.
+        """
+        if cls is MISSING:
+            cls = Context  # type: ignore
+
+        view = StringView(message.content)
+        ctx = cls(prefix=None, view=view, bot=self, message=message)
+
+        if self._skip_check(message.author.id, self.user.id):  # type: ignore
+            return ctx
+
+        prefix = await self.get_prefix(message)
+        invoked_prefix = prefix
+
+        if isinstance(prefix, str):
+            if not view.skip_string(prefix):
+                return ctx
+        else:
+            try:
+                # if the context class' __init__ consumes something from the view this
+                # will be wrong.  That seems unreasonable though.
+                if message.content.startswith(tuple(prefix)):
+                    invoked_prefix = discord.utils.find(view.skip_string, prefix)
+                else:
+                    return ctx
+
+            except TypeError:
+                if not isinstance(prefix, list):
+                    raise TypeError(
+                        "get_prefix must return either a string or a list of string, " f"not {prefix.__class__.__name__}"
+                    )
+
+                # It's possible a bad command_prefix got us here.
+                for value in prefix:
+                    if not isinstance(value, str):
+                        raise TypeError(
+                            "Iterable command_prefix or list returned from get_prefix must "
+                            f"contain only strings, not {value.__class__.__name__}"
+                        )
+
+                # Getting here shouldn't happen
+                raise
+
+        if self.strip_after_prefix:
+            view.skip_ws()
+
+        invoker = view.get_word()
+        ctx.invoked_with = invoker
+        # type-checker fails to narrow invoked_prefix type.
+        ctx.prefix = invoked_prefix  # type: ignore
+        ctx.command = self.all_commands.get(invoker)
+        return ctx
+
+    async def invoke(self, ctx: Context[BotT], /) -> None:
+        """|coro|
+
+        Invokes the command given under the invocation context and
+        handles all the internal event dispatch mechanisms.
+
+        .. versionchanged:: 2.0
+
+            ``ctx`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        ctx: :class:`.Context`
+            The invocation context to invoke.
+        """
+        if ctx.command is not None:
+            self.dispatch('command', ctx)
+            try:
+                if await self.can_run(ctx, call_once=True):
+                    await ctx.command.invoke(ctx)
+                else:
+                    raise errors.CheckFailure('The global check once functions failed.')
+            except errors.CommandError as exc:
+                await ctx.command.dispatch_error(ctx, exc)
+            else:
+                self.dispatch('command_completion', ctx)
+        elif ctx.invoked_with:
+            exc = errors.CommandNotFound(f'Command "{ctx.invoked_with}" is not found')
+            self.dispatch('command_error', ctx, exc)
+
+    async def process_commands(self, message: Message, /) -> None:
+        """|coro|
+
+        This function processes the commands that have been registered
+        to the bot and other groups. Without this coroutine, none of the
+        commands will be triggered.
+
+        By default, this coroutine is called inside the :func:`.on_message`
+        event. If you choose to override the :func:`.on_message` event, then
+        you should invoke this coroutine as well.
+
+        This is built using other low level tools, and is equivalent to a
+        call to :meth:`~.Bot.get_context` followed by a call to :meth:`~.Bot.invoke`.
+
+        This also checks if the message's author is a bot and doesn't
+        call :meth:`~.Bot.get_context` or :meth:`~.Bot.invoke` if so.
+
+        .. versionchanged:: 2.0
+
+            ``message`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        message: :class:`discord.Message`
+            The message to process commands for.
+        """
+        if message.author.bot:
+            return
+
+        ctx = await self.get_context(message)
+        # the type of the invocation context's bot attribute will be correct
+        await self.invoke(ctx)  # type: ignore
+
+    async def on_message(self, message: Message, /) -> None:
+        await self.process_commands(message)
+
+
+class Bot(BotBase, discord.Client):
+    """Represents a Discord bot.
+
+    This class is a subclass of :class:`discord.Client` and as a result
+    anything that you can do with a :class:`discord.Client` you can do with
+    this bot.
+
+    This class also subclasses :class:`.GroupMixin` to provide the functionality
+    to manage commands.
+
+    .. container:: operations
+
+        .. describe:: async with x
+
+            Asynchronously initialises the bot and automatically cleans up.
+
+            .. versionadded:: 2.0
+
+    Attributes
+    -----------
+    command_prefix
+        The command prefix is what the message content must contain initially
+        to have a command invoked. This prefix could either be a string to
+        indicate what the prefix should be, or a callable that takes in the bot
+        as its first parameter and :class:`discord.Message` as its second
+        parameter and returns the prefix. This is to facilitate "dynamic"
+        command prefixes. This callable can be either a regular function or
+        a coroutine.
+
+        An empty string as the prefix always matches, enabling prefix-less
+        command invocation. While this may be useful in DMs it should be avoided
+        in servers, as it's likely to cause performance issues and unintended
+        command invocations.
+
+        The command prefix could also be an iterable of strings indicating that
+        multiple checks for the prefix should be used and the first one to
+        match will be the invocation prefix. You can get this prefix via
+        :attr:`.Context.prefix`.
+
+        .. note::
+
+            When passing multiple prefixes be careful to not pass a prefix
+            that matches a longer prefix occurring later in the sequence.  For
+            example, if the command prefix is ``('!', '!?')``  the ``'!?'``
+            prefix will never be matched to any message as the previous one
+            matches messages starting with ``!?``. This is especially important
+            when passing an empty string, it should always be last as no prefix
+            after it will be matched.
+    case_insensitive: :class:`bool`
+        Whether the commands should be case insensitive. Defaults to ``False``. This
+        attribute does not carry over to groups. You must set it to every group if
+        you require group commands to be case insensitive as well.
+    description: :class:`str`
+        The content prefixed into the default help message.
+    help_command: Optional[:class:`.HelpCommand`]
+        The help command implementation to use. This can be dynamically
+        set at runtime. To remove the help command pass ``None``. For more
+        information on implementing a help command, see :ref:`ext_commands_help_command`.
+    owner_id: Optional[:class:`int`]
+        The user ID that owns the bot. If this is not set and is then queried via
+        :meth:`.is_owner` then it will error.
+    owner_ids: Optional[Collection[:class:`int`]]
+        The user IDs that owns the bot. This is similar to :attr:`owner_id`.
+        If this is not set and and is then queried via :meth:`.is_owner` then it will error.
+        For performance reasons it is recommended to use a :class:`set`
+        for the collection. You cannot set both ``owner_id`` and ``owner_ids``.
+
+        .. versionadded:: 1.3
+    strip_after_prefix: :class:`bool`
+        Whether to strip whitespace characters after encountering the command
+        prefix. This allows for ``!   hello`` and ``!hello`` to both work if
+        the ``command_prefix`` is set to ``!``. Defaults to ``False``.
+
+        .. versionadded:: 1.7
+    """
+
+    pass
```

### Comparing `discord.py-self-1.9.2/discord/ext/commands/help.py` & `discord.py-self-2.0.0/discord/ext/commands/help.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1342 +1,1568 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import itertools
-import copy
-import functools
-import re
-import discord.utils
-
-from .core import Group, Command
-from .errors import CommandError
-
-__all__ = (
-    'Paginator',
-    'HelpCommand',
-    'DefaultHelpCommand',
-    'MinimalHelpCommand',
-)
-
-# help -> shows info of bot on top/bottom and lists subcommands
-# help command -> shows detailed info of command
-# help command <subcommand chain> -> same as above
-
-# <description>
-
-# <command signature with aliases>
-
-# <long doc>
-
-# Cog:
-#   <command> <shortdoc>
-#   <command> <shortdoc>
-# Other Cog:
-#   <command> <shortdoc>
-# No Category:
-#   <command> <shortdoc>
-
-# Type <prefix>help command for more info on a command.
-# You can also type <prefix>help category for more info on a category.
-
-class Paginator:
-    """A class that aids in paginating code blocks for Discord messages.
-
-    .. container:: operations
-
-        .. describe:: len(x)
-
-            Returns the total number of characters in the paginator.
-
-    Attributes
-    -----------
-    prefix: :class:`str`
-        The prefix inserted to every page. e.g. three backticks.
-    suffix: :class:`str`
-        The suffix appended at the end of every page. e.g. three backticks.
-    max_size: :class:`int`
-        The maximum amount of codepoints allowed in a page.
-    linesep: :class:`str`
-        The character string inserted between lines. e.g. a newline character.
-            .. versionadded:: 1.7
-    """
-    def __init__(self, prefix='```', suffix='```', max_size=2000, linesep='\n'):
-        self.prefix = prefix
-        self.suffix = suffix
-        self.max_size = max_size
-        self.linesep = linesep
-        self.clear()
-
-    def clear(self):
-        """Clears the paginator to have no pages."""
-        if self.prefix is not None:
-            self._current_page = [self.prefix]
-            self._count = len(self.prefix) + self._linesep_len # prefix + newline
-        else:
-            self._current_page = []
-            self._count = 0
-        self._pages = []
-
-    @property
-    def _prefix_len(self):
-        return len(self.prefix) if self.prefix else 0
-
-    @property
-    def _suffix_len(self):
-        return len(self.suffix) if self.suffix else 0
-
-    @property
-    def _linesep_len(self):
-        return len(self.linesep)
-
-    def add_line(self, line='', *, empty=False):
-        """Adds a line to the current page.
-
-        If the line exceeds the :attr:`max_size` then an exception
-        is raised.
-
-        Parameters
-        -----------
-        line: :class:`str`
-            The line to add.
-        empty: :class:`bool`
-            Indicates if another empty line should be added.
-
-        Raises
-        ------
-        RuntimeError
-            The line was too big for the current :attr:`max_size`.
-        """
-        max_page_size = self.max_size - self._prefix_len - self._suffix_len - 2 * self._linesep_len
-        if len(line) > max_page_size:
-            raise RuntimeError('Line exceeds maximum page size %s' % (max_page_size))
-
-        if self._count + len(line) + self._linesep_len > self.max_size - self._suffix_len:
-            self.close_page()
-
-        self._count += len(line) + self._linesep_len
-        self._current_page.append(line)
-
-        if empty:
-            self._current_page.append('')
-            self._count += self._linesep_len
-
-    def close_page(self):
-        """Prematurely terminate a page."""
-        if self.suffix is not None:
-            self._current_page.append(self.suffix)
-        self._pages.append(self.linesep.join(self._current_page))
-
-        if self.prefix is not None:
-            self._current_page = [self.prefix]
-            self._count = len(self.prefix) + self._linesep_len # prefix + linesep
-        else:
-            self._current_page = []
-            self._count = 0
-
-    def __len__(self):
-        total = sum(len(p) for p in self._pages)
-        return total + self._count
-
-    @property
-    def pages(self):
-        """List[:class:`str`]: Returns the rendered list of pages."""
-        # we have more than just the prefix in our current page
-        if len(self._current_page) > (0 if self.prefix is None else 1):
-            self.close_page()
-        return self._pages
-
-    def __repr__(self):
-        fmt = '<Paginator prefix: {0.prefix!r} suffix: {0.suffix!r} linesep: {0.linesep!r} max_size: {0.max_size} count: {0._count}>'
-        return fmt.format(self)
-
-def _not_overriden(f):
-    f.__help_command_not_overriden__ = True
-    return f
-
-class _HelpCommandImpl(Command):
-    def __init__(self, inject, *args, **kwargs):
-        super().__init__(inject.command_callback, *args, **kwargs)
-        self._original = inject
-        self._injected = inject
-
-    async def prepare(self, ctx):
-        self._injected = injected = self._original.copy()
-        injected.context = ctx
-        self.callback = injected.command_callback
-
-        on_error = injected.on_help_command_error
-        if not hasattr(on_error, '__help_command_not_overriden__'):
-            if self.cog is not None:
-                self.on_error = self._on_error_cog_implementation
-            else:
-                self.on_error = on_error
-
-        await super().prepare(ctx)
-
-    async def _parse_arguments(self, ctx):
-        # Make the parser think we don't have a cog so it doesn't
-        # inject the parameter into `ctx.args`.
-        original_cog = self.cog
-        self.cog = None
-        try:
-            await super()._parse_arguments(ctx)
-        finally:
-            self.cog = original_cog
-
-    async def _on_error_cog_implementation(self, dummy, ctx, error):
-        await self._injected.on_help_command_error(ctx, error)
-
-    @property
-    def clean_params(self):
-        result = self.params.copy()
-        try:
-            result.popitem(last=False)
-        except Exception:
-            raise ValueError('Missing context parameter') from None
-        else:
-            return result
-
-    def _inject_into_cog(self, cog):
-        # Warning: hacky
-
-        # Make the cog think that get_commands returns this command
-        # as well if we inject it without modifying __cog_commands__
-        # since that's used for the injection and ejection of cogs.
-        def wrapped_get_commands(*, _original=cog.get_commands):
-            ret = _original()
-            ret.append(self)
-            return ret
-
-        # Ditto here
-        def wrapped_walk_commands(*, _original=cog.walk_commands):
-            yield from _original()
-            yield self
-
-        functools.update_wrapper(wrapped_get_commands, cog.get_commands)
-        functools.update_wrapper(wrapped_walk_commands, cog.walk_commands)
-        cog.get_commands = wrapped_get_commands
-        cog.walk_commands = wrapped_walk_commands
-        self.cog = cog
-
-    def _eject_cog(self):
-        if self.cog is None:
-            return
-
-        # revert back into their original methods
-        cog = self.cog
-        cog.get_commands = cog.get_commands.__wrapped__
-        cog.walk_commands = cog.walk_commands.__wrapped__
-        self.cog = None
-
-class HelpCommand:
-    r"""The base implementation for help command formatting.
-
-    .. note::
-
-        Internally instances of this class are deep copied every time
-        the command itself is invoked to prevent a race condition
-        mentioned in :issue:`2123`.
-
-        This means that relying on the state of this class to be
-        the same between command invocations would not work as expected.
-
-    Attributes
-    ------------
-    context: Optional[:class:`Context`]
-        The context that invoked this help formatter. This is generally set after
-        the help command assigned, :func:`command_callback`\, has been called.
-    show_hidden: :class:`bool`
-        Specifies if hidden commands should be shown in the output.
-        Defaults to ``False``.
-    verify_checks: Optional[:class:`bool`]
-        Specifies if commands should have their :attr:`.Command.checks` called
-        and verified. If ``True``, always calls :attr:`.Commands.checks`.
-        If ``None``, only calls :attr:`.Commands.checks` in a guild setting.
-        If ``False``, never calls :attr:`.Commands.checks`. Defaults to ``True``.
-
-        .. versionchanged:: 1.7
-    command_attrs: :class:`dict`
-        A dictionary of options to pass in for the construction of the help command.
-        This allows you to change the command behaviour without actually changing
-        the implementation of the command. The attributes will be the same as the
-        ones passed in the :class:`.Command` constructor.
-    """
-
-    MENTION_TRANSFORMS = {
-        '@everyone': '@\u200beveryone',
-        '@here': '@\u200bhere',
-        r'<@!?[0-9]{17,22}>': '@deleted-user',
-        r'<@&[0-9]{17,22}>': '@deleted-role'
-    }
-
-    MENTION_PATTERN = re.compile('|'.join(MENTION_TRANSFORMS.keys()))
-
-    def __new__(cls, *args, **kwargs):
-        # To prevent race conditions of a single instance while also allowing
-        # for settings to be passed the original arguments passed must be assigned
-        # to allow for easier copies (which will be made when the help command is actually called)
-        # see issue 2123
-        self = super().__new__(cls)
-
-        # Shallow copies cannot be used in this case since it is not unusual to pass
-        # instances that need state, e.g. Paginator or what have you into the function
-        # The keys can be safely copied as-is since they're 99.99% certain of being
-        # string keys
-        deepcopy = copy.deepcopy
-        self.__original_kwargs__ = {
-            k: deepcopy(v)
-            for k, v in kwargs.items()
-        }
-        self.__original_args__ = deepcopy(args)
-        return self
-
-    def __init__(self, **options):
-        self.show_hidden = options.pop('show_hidden', False)
-        self.verify_checks = options.pop('verify_checks', True)
-        self.command_attrs = attrs = options.pop('command_attrs', {})
-        attrs.setdefault('name', 'help')
-        attrs.setdefault('help', 'Shows this message')
-        self.context = None
-        self._command_impl = _HelpCommandImpl(self, **self.command_attrs)
-
-    def copy(self):
-        obj = self.__class__(*self.__original_args__, **self.__original_kwargs__)
-        obj._command_impl = self._command_impl
-        return obj
-
-    def _add_to_bot(self, bot):
-        command = _HelpCommandImpl(self, **self.command_attrs)
-        bot.add_command(command)
-        self._command_impl = command
-
-    def _remove_from_bot(self, bot):
-        bot.remove_command(self._command_impl.name)
-        self._command_impl._eject_cog()
-
-    def add_check(self, func):
-        """
-        Adds a check to the help command.
-
-        .. versionadded:: 1.4
-
-        Parameters
-        ----------
-        func
-            The function that will be used as a check.
-        """
-
-        self._command_impl.add_check(func)
-
-    def remove_check(self, func):
-        """
-        Removes a check from the help command.
-
-        This function is idempotent and will not raise an exception if
-        the function is not in the command's checks.
-
-        .. versionadded:: 1.4
-
-        Parameters
-        ----------
-        func
-            The function to remove from the checks.
-        """
-
-        self._command_impl.remove_check(func)
-
-    def get_bot_mapping(self):
-        """Retrieves the bot mapping passed to :meth:`send_bot_help`."""
-        bot = self.context.bot
-        mapping = {
-            cog: cog.get_commands()
-            for cog in bot.cogs.values()
-        }
-        mapping[None] = [c for c in bot.commands if c.cog is None]
-        return mapping
-
-    @property
-    def clean_prefix(self):
-        """:class:`str`: The cleaned up invoke prefix. i.e. mentions are ``@name`` instead of ``<@id>``."""
-        user = self.context.guild.me if self.context.guild else self.context.bot.user
-        # this breaks if the prefix mention is not the bot itself but I
-        # consider this to be an *incredibly* strange use case. I'd rather go
-        # for this common use case rather than waste performance for the
-        # odd one.
-        pattern = re.compile(r"<@!?%s>" % user.id)
-        return pattern.sub("@%s" % user.display_name.replace('\\', r'\\'), self.context.prefix)
-
-    @property
-    def invoked_with(self):
-        """Similar to :attr:`Context.invoked_with` except properly handles
-        the case where :meth:`Context.send_help` is used.
-
-        If the help command was used regularly then this returns
-        the :attr:`Context.invoked_with` attribute. Otherwise, if
-        it the help command was called using :meth:`Context.send_help`
-        then it returns the internal command name of the help command.
-
-        Returns
-        ---------
-        :class:`str`
-            The command name that triggered this invocation.
-        """
-        command_name = self._command_impl.name
-        ctx = self.context
-        if ctx is None or ctx.command is None or ctx.command.qualified_name != command_name:
-            return command_name
-        return ctx.invoked_with
-
-    def get_command_signature(self, command):
-        """Retrieves the signature portion of the help page.
-
-        Parameters
-        ------------
-        command: :class:`Command`
-            The command to get the signature of.
-
-        Returns
-        --------
-        :class:`str`
-            The signature for the command.
-        """
-
-        parent = command.parent
-        entries = []
-        while parent is not None:
-            if not parent.signature or parent.invoke_without_command:
-                entries.append(parent.name)
-            else:
-                entries.append(parent.name + ' ' + parent.signature)
-            parent = parent.parent
-        parent_sig = ' '.join(reversed(entries))
-
-        if len(command.aliases) > 0:
-            aliases = '|'.join(command.aliases)
-            fmt = '[%s|%s]' % (command.name, aliases)
-            if parent_sig:
-                fmt = parent_sig + ' ' + fmt
-            alias = fmt
-        else:
-            alias = command.name if not parent_sig else parent_sig + ' ' + command.name
-
-        return '%s%s %s' % (self.clean_prefix, alias, command.signature)
-
-    def remove_mentions(self, string):
-        """Removes mentions from the string to prevent abuse.
-
-        This includes ``@everyone``, ``@here``, member mentions and role mentions.
-
-        Returns
-        -------
-        :class:`str`
-            The string with mentions removed.
-        """
-
-        def replace(obj, *, transforms=self.MENTION_TRANSFORMS):
-            return transforms.get(obj.group(0), '@invalid')
-
-        return self.MENTION_PATTERN.sub(replace, string)
-
-    @property
-    def cog(self):
-        """A property for retrieving or setting the cog for the help command.
-
-        When a cog is set for the help command, it is as-if the help command
-        belongs to that cog. All cog special methods will apply to the help
-        command and it will be automatically unset on unload.
-
-        To unbind the cog from the help command, you can set it to ``None``.
-
-        Returns
-        --------
-        Optional[:class:`Cog`]
-            The cog that is currently set for the help command.
-        """
-        return self._command_impl.cog
-
-    @cog.setter
-    def cog(self, cog):
-        # Remove whatever cog is currently valid, if any
-        self._command_impl._eject_cog()
-
-        # If a new cog is set then inject it.
-        if cog is not None:
-            self._command_impl._inject_into_cog(cog)
-
-    def command_not_found(self, string):
-        """|maybecoro|
-
-        A method called when a command is not found in the help command.
-        This is useful to override for i18n.
-
-        Defaults to ``No command called {0} found.``
-
-        Parameters
-        ------------
-        string: :class:`str`
-            The string that contains the invalid command. Note that this has
-            had mentions removed to prevent abuse.
-
-        Returns
-        ---------
-        :class:`str`
-            The string to use when a command has not been found.
-        """
-        return 'No command called "{}" found.'.format(string)
-
-    def subcommand_not_found(self, command, string):
-        """|maybecoro|
-
-        A method called when a command did not have a subcommand requested in the help command.
-        This is useful to override for i18n.
-
-        Defaults to either:
-
-        - ``'Command "{command.qualified_name}" has no subcommands.'``
-            - If there is no subcommand in the ``command`` parameter.
-        - ``'Command "{command.qualified_name}" has no subcommand named {string}'``
-            - If the ``command`` parameter has subcommands but not one named ``string``.
-
-        Parameters
-        ------------
-        command: :class:`Command`
-            The command that did not have the subcommand requested.
-        string: :class:`str`
-            The string that contains the invalid subcommand. Note that this has
-            had mentions removed to prevent abuse.
-
-        Returns
-        ---------
-        :class:`str`
-            The string to use when the command did not have the subcommand requested.
-        """
-        if isinstance(command, Group) and len(command.all_commands) > 0:
-            return 'Command "{0.qualified_name}" has no subcommand named {1}'.format(command, string)
-        return 'Command "{0.qualified_name}" has no subcommands.'.format(command)
-
-    async def filter_commands(self, commands, *, sort=False, key=None):
-        """|coro|
-
-        Returns a filtered list of commands and optionally sorts them.
-
-        This takes into account the :attr:`verify_checks` and :attr:`show_hidden`
-        attributes.
-
-        Parameters
-        ------------
-        commands: Iterable[:class:`Command`]
-            An iterable of commands that are getting filtered.
-        sort: :class:`bool`
-            Whether to sort the result.
-        key: Optional[Callable[:class:`Command`, Any]]
-            An optional key function to pass to :func:`py:sorted` that
-            takes a :class:`Command` as its sole parameter. If ``sort`` is
-            passed as ``True`` then this will default as the command name.
-
-        Returns
-        ---------
-        List[:class:`Command`]
-            A list of commands that passed the filter.
-        """
-
-        if sort and key is None:
-            key = lambda c: c.name
-
-        iterator = commands if self.show_hidden else filter(lambda c: not c.hidden, commands)
-
-        if self.verify_checks is False:
-            # if we do not need to verify the checks then we can just
-            # run it straight through normally without using await.
-            return sorted(iterator, key=key) if sort else list(iterator)
-
-        if self.verify_checks is None and not self.context.guild:
-            # if verify_checks is None and we're in a DM, don't verify
-            return sorted(iterator, key=key) if sort else list(iterator)
-
-        # if we're here then we need to check every command if it can run
-        async def predicate(cmd):
-            try:
-                return await cmd.can_run(self.context)
-            except CommandError:
-                return False
-
-        ret = []
-        for cmd in iterator:
-            valid = await predicate(cmd)
-            if valid:
-                ret.append(cmd)
-
-        if sort:
-            ret.sort(key=key)
-        return ret
-
-    def get_max_size(self, commands):
-        """Returns the largest name length of the specified command list.
-
-        Parameters
-        ------------
-        commands: Sequence[:class:`Command`]
-            A sequence of commands to check for the largest size.
-
-        Returns
-        --------
-        :class:`int`
-            The maximum width of the commands.
-        """
-
-        as_lengths = (
-            discord.utils._string_width(c.name)
-            for c in commands
-        )
-        return max(as_lengths, default=0)
-
-    def get_destination(self):
-        """Returns the :class:`~discord.abc.Messageable` where the help command will be output.
-
-        You can override this method to customise the behaviour.
-
-        By default this returns the context's channel.
-
-        Returns
-        -------
-        :class:`.abc.Messageable`
-            The destination where the help command will be output.
-        """
-        return self.context.channel
-
-    async def send_error_message(self, error):
-        """|coro|
-
-        Handles the implementation when an error happens in the help command.
-        For example, the result of :meth:`command_not_found` or
-        :meth:`command_has_no_subcommand_found` will be passed here.
-
-        You can override this method to customise the behaviour.
-
-        By default, this sends the error message to the destination
-        specified by :meth:`get_destination`.
-
-        .. note::
-
-            You can access the invocation context with :attr:`HelpCommand.context`.
-
-        Parameters
-        ------------
-        error: :class:`str`
-            The error message to display to the user. Note that this has
-            had mentions removed to prevent abuse.
-        """
-        destination = self.get_destination()
-        await destination.send(error)
-
-    @_not_overriden
-    async def on_help_command_error(self, ctx, error):
-        """|coro|
-
-        The help command's error handler, as specified by :ref:`ext_commands_error_handler`.
-
-        Useful to override if you need some specific behaviour when the error handler
-        is called.
-
-        By default this method does nothing and just propagates to the default
-        error handlers.
-
-        Parameters
-        ------------
-        ctx: :class:`Context`
-            The invocation context.
-        error: :class:`CommandError`
-            The error that was raised.
-        """
-        pass
-
-    async def send_bot_help(self, mapping):
-        """|coro|
-
-        Handles the implementation of the bot command page in the help command.
-        This function is called when the help command is called with no arguments.
-
-        It should be noted that this method does not return anything -- rather the
-        actual message sending should be done inside this method. Well behaved subclasses
-        should use :meth:`get_destination` to know where to send, as this is a customisation
-        point for other users.
-
-        You can override this method to customise the behaviour.
-
-        .. note::
-
-            You can access the invocation context with :attr:`HelpCommand.context`.
-
-            Also, the commands in the mapping are not filtered. To do the filtering
-            you will have to call :meth:`filter_commands` yourself.
-
-        Parameters
-        ------------
-        mapping: Mapping[Optional[:class:`Cog`], List[:class:`Command`]]
-            A mapping of cogs to commands that have been requested by the user for help.
-            The key of the mapping is the :class:`~.commands.Cog` that the command belongs to, or
-            ``None`` if there isn't one, and the value is a list of commands that belongs to that cog.
-        """
-        return None
-
-    async def send_cog_help(self, cog):
-        """|coro|
-
-        Handles the implementation of the cog page in the help command.
-        This function is called when the help command is called with a cog as the argument.
-
-        It should be noted that this method does not return anything -- rather the
-        actual message sending should be done inside this method. Well behaved subclasses
-        should use :meth:`get_destination` to know where to send, as this is a customisation
-        point for other users.
-
-        You can override this method to customise the behaviour.
-
-        .. note::
-
-            You can access the invocation context with :attr:`HelpCommand.context`.
-
-            To get the commands that belong to this cog see :meth:`Cog.get_commands`.
-            The commands returned not filtered. To do the filtering you will have to call
-            :meth:`filter_commands` yourself.
-
-        Parameters
-        -----------
-        cog: :class:`Cog`
-            The cog that was requested for help.
-        """
-        return None
-
-    async def send_group_help(self, group):
-        """|coro|
-
-        Handles the implementation of the group page in the help command.
-        This function is called when the help command is called with a group as the argument.
-
-        It should be noted that this method does not return anything -- rather the
-        actual message sending should be done inside this method. Well behaved subclasses
-        should use :meth:`get_destination` to know where to send, as this is a customisation
-        point for other users.
-
-        You can override this method to customise the behaviour.
-
-        .. note::
-
-            You can access the invocation context with :attr:`HelpCommand.context`.
-
-            To get the commands that belong to this group without aliases see
-            :attr:`Group.commands`. The commands returned not filtered. To do the
-            filtering you will have to call :meth:`filter_commands` yourself.
-
-        Parameters
-        -----------
-        group: :class:`Group`
-            The group that was requested for help.
-        """
-        return None
-
-    async def send_command_help(self, command):
-        """|coro|
-
-        Handles the implementation of the single command page in the help command.
-
-        It should be noted that this method does not return anything -- rather the
-        actual message sending should be done inside this method. Well behaved subclasses
-        should use :meth:`get_destination` to know where to send, as this is a customisation
-        point for other users.
-
-        You can override this method to customise the behaviour.
-
-        .. note::
-
-            You can access the invocation context with :attr:`HelpCommand.context`.
-
-        .. admonition:: Showing Help
-            :class: helpful
-
-            There are certain attributes and methods that are helpful for a help command
-            to show such as the following:
-
-            - :attr:`Command.help`
-            - :attr:`Command.brief`
-            - :attr:`Command.short_doc`
-            - :attr:`Command.description`
-            - :meth:`get_command_signature`
-
-            There are more than just these attributes but feel free to play around with
-            these to help you get started to get the output that you want.
-
-        Parameters
-        -----------
-        command: :class:`Command`
-            The command that was requested for help.
-        """
-        return None
-
-    async def prepare_help_command(self, ctx, command=None):
-        """|coro|
-
-        A low level method that can be used to prepare the help command
-        before it does anything. For example, if you need to prepare
-        some state in your subclass before the command does its processing
-        then this would be the place to do it.
-
-        The default implementation does nothing.
-
-        .. note::
-
-            This is called *inside* the help command callback body. So all
-            the usual rules that happen inside apply here as well.
-
-        Parameters
-        -----------
-        ctx: :class:`Context`
-            The invocation context.
-        command: Optional[:class:`str`]
-            The argument passed to the help command.
-        """
-        pass
-
-    async def command_callback(self, ctx, *, command=None):
-        """|coro|
-
-        The actual implementation of the help command.
-
-        It is not recommended to override this method and instead change
-        the behaviour through the methods that actually get dispatched.
-
-        - :meth:`send_bot_help`
-        - :meth:`send_cog_help`
-        - :meth:`send_group_help`
-        - :meth:`send_command_help`
-        - :meth:`get_destination`
-        - :meth:`command_not_found`
-        - :meth:`subcommand_not_found`
-        - :meth:`send_error_message`
-        - :meth:`on_help_command_error`
-        - :meth:`prepare_help_command`
-        """
-        await self.prepare_help_command(ctx, command)
-        bot = ctx.bot
-
-        if command is None:
-            mapping = self.get_bot_mapping()
-            return await self.send_bot_help(mapping)
-
-        # Check if it's a cog
-        cog = bot.get_cog(command)
-        if cog is not None:
-            return await self.send_cog_help(cog)
-
-        maybe_coro = discord.utils.maybe_coroutine
-
-        # If it's not a cog then it's a command.
-        # Since we want to have detailed errors when someone
-        # passes an invalid subcommand, we need to walk through
-        # the command group chain ourselves.
-        keys = command.split(' ')
-        cmd = bot.all_commands.get(keys[0])
-        if cmd is None:
-            string = await maybe_coro(self.command_not_found, self.remove_mentions(keys[0]))
-            return await self.send_error_message(string)
-
-        for key in keys[1:]:
-            try:
-                found = cmd.all_commands.get(key)
-            except AttributeError:
-                string = await maybe_coro(self.subcommand_not_found, cmd, self.remove_mentions(key))
-                return await self.send_error_message(string)
-            else:
-                if found is None:
-                    string = await maybe_coro(self.subcommand_not_found, cmd, self.remove_mentions(key))
-                    return await self.send_error_message(string)
-                cmd = found
-
-        if isinstance(cmd, Group):
-            return await self.send_group_help(cmd)
-        else:
-            return await self.send_command_help(cmd)
-
-class DefaultHelpCommand(HelpCommand):
-    """The implementation of the default help command.
-
-    This inherits from :class:`HelpCommand`.
-
-    It extends it with the following attributes.
-
-    Attributes
-    ------------
-    width: :class:`int`
-        The maximum number of characters that fit in a line.
-        Defaults to 80.
-    sort_commands: :class:`bool`
-        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
-    dm_help: Optional[:class:`bool`]
-        A tribool that indicates if the help command should DM the user instead of
-        sending it to the channel it received it from. If the boolean is set to
-        ``True``, then all help output is DM'd. If ``False``, none of the help
-        output is DM'd. If ``None``, then the bot will only DM when the help
-        message becomes too long (dictated by more than :attr:`dm_help_threshold` characters).
-        Defaults to ``False``.
-    dm_help_threshold: Optional[:class:`int`]
-        The number of characters the paginator must accumulate before getting DM'd to the
-        user if :attr:`dm_help` is set to ``None``. Defaults to 1000.
-    indent: :class:`int`
-        How much to indent the commands from a heading. Defaults to ``2``.
-    commands_heading: :class:`str`
-        The command list's heading string used when the help command is invoked with a category name.
-        Useful for i18n. Defaults to ``"Commands:"``
-    no_category: :class:`str`
-        The string used when there is a command which does not belong to any category(cog).
-        Useful for i18n. Defaults to ``"No Category"``
-    paginator: :class:`Paginator`
-        The paginator used to paginate the help command output.
-    """
-
-    def __init__(self, **options):
-        self.width = options.pop('width', 80)
-        self.indent = options.pop('indent', 2)
-        self.sort_commands = options.pop('sort_commands', True)
-        self.dm_help = options.pop('dm_help', False)
-        self.dm_help_threshold = options.pop('dm_help_threshold', 1000)
-        self.commands_heading = options.pop('commands_heading', "Commands:")
-        self.no_category = options.pop('no_category', 'No Category')
-        self.paginator = options.pop('paginator', None)
-
-        if self.paginator is None:
-            self.paginator = Paginator()
-
-        super().__init__(**options)
-
-    def shorten_text(self, text):
-        """:class:`str`: Shortens text to fit into the :attr:`width`."""
-        if len(text) > self.width:
-            return text[:self.width - 3] + '...'
-        return text
-
-    def get_ending_note(self):
-        """:class:`str`: Returns help command's ending note. This is mainly useful to override for i18n purposes."""
-        command_name = self.invoked_with
-        return "Type {0}{1} command for more info on a command.\n" \
-               "You can also type {0}{1} category for more info on a category.".format(self.clean_prefix, command_name)
-
-    def add_indented_commands(self, commands, *, heading, max_size=None):
-        """Indents a list of commands after the specified heading.
-
-        The formatting is added to the :attr:`paginator`.
-
-        The default implementation is the command name indented by
-        :attr:`indent` spaces, padded to ``max_size`` followed by
-        the command's :attr:`Command.short_doc` and then shortened
-        to fit into the :attr:`width`.
-
-        Parameters
-        -----------
-        commands: Sequence[:class:`Command`]
-            A list of commands to indent for output.
-        heading: :class:`str`
-            The heading to add to the output. This is only added
-            if the list of commands is greater than 0.
-        max_size: Optional[:class:`int`]
-            The max size to use for the gap between indents.
-            If unspecified, calls :meth:`get_max_size` on the
-            commands parameter.
-        """
-
-        if not commands:
-            return
-
-        self.paginator.add_line(heading)
-        max_size = max_size or self.get_max_size(commands)
-
-        get_width = discord.utils._string_width
-        for command in commands:
-            name = command.name
-            width = max_size - (get_width(name) - len(name))
-            entry = '{0}{1:<{width}} {2}'.format(self.indent * ' ', name, command.short_doc, width=width)
-            self.paginator.add_line(self.shorten_text(entry))
-
-    async def send_pages(self):
-        """A helper utility to send the page output from :attr:`paginator` to the destination."""
-        destination = self.get_destination()
-        for page in self.paginator.pages:
-            await destination.send(page)
-
-    def add_command_formatting(self, command):
-        """A utility function to format the non-indented block of commands and groups.
-
-        Parameters
-        ------------
-        command: :class:`Command`
-            The command to format.
-        """
-
-        if command.description:
-            self.paginator.add_line(command.description, empty=True)
-
-        signature = self.get_command_signature(command)
-        self.paginator.add_line(signature, empty=True)
-
-        if command.help:
-            try:
-                self.paginator.add_line(command.help, empty=True)
-            except RuntimeError:
-                for line in command.help.splitlines():
-                    self.paginator.add_line(line)
-                self.paginator.add_line()
-
-    def get_destination(self):
-        ctx = self.context
-        if self.dm_help is True:
-            return ctx.author
-        elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
-            return ctx.author
-        else:
-            return ctx.channel
-
-    async def prepare_help_command(self, ctx, command):
-        self.paginator.clear()
-        await super().prepare_help_command(ctx, command)
-
-    async def send_bot_help(self, mapping):
-        ctx = self.context
-        bot = ctx.bot
-
-        if bot.description:
-            # <description> portion
-            self.paginator.add_line(bot.description, empty=True)
-
-        no_category = '\u200b{0.no_category}:'.format(self)
-        def get_category(command, *, no_category=no_category):
-            cog = command.cog
-            return cog.qualified_name + ':' if cog is not None else no_category
-
-        filtered = await self.filter_commands(bot.commands, sort=True, key=get_category)
-        max_size = self.get_max_size(filtered)
-        to_iterate = itertools.groupby(filtered, key=get_category)
-
-        # Now we can add the commands to the page.
-        for category, commands in to_iterate:
-            commands = sorted(commands, key=lambda c: c.name) if self.sort_commands else list(commands)
-            self.add_indented_commands(commands, heading=category, max_size=max_size)
-
-        note = self.get_ending_note()
-        if note:
-            self.paginator.add_line()
-            self.paginator.add_line(note)
-
-        await self.send_pages()
-
-    async def send_command_help(self, command):
-        self.add_command_formatting(command)
-        self.paginator.close_page()
-        await self.send_pages()
-
-    async def send_group_help(self, group):
-        self.add_command_formatting(group)
-
-        filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
-        self.add_indented_commands(filtered, heading=self.commands_heading)
-
-        if filtered:
-            note = self.get_ending_note()
-            if note:
-                self.paginator.add_line()
-                self.paginator.add_line(note)
-
-        await self.send_pages()
-
-    async def send_cog_help(self, cog):
-        if cog.description:
-            self.paginator.add_line(cog.description, empty=True)
-
-        filtered = await self.filter_commands(cog.get_commands(), sort=self.sort_commands)
-        self.add_indented_commands(filtered, heading=self.commands_heading)
-
-        note = self.get_ending_note()
-        if note:
-            self.paginator.add_line()
-            self.paginator.add_line(note)
-
-        await self.send_pages()
-
-class MinimalHelpCommand(HelpCommand):
-    """An implementation of a help command with minimal output.
-
-    This inherits from :class:`HelpCommand`.
-
-    Attributes
-    ------------
-    sort_commands: :class:`bool`
-        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
-    commands_heading: :class:`str`
-        The command list's heading string used when the help command is invoked with a category name.
-        Useful for i18n. Defaults to ``"Commands"``
-    aliases_heading: :class:`str`
-        The alias list's heading string used to list the aliases of the command. Useful for i18n.
-        Defaults to ``"Aliases:"``.
-    dm_help: Optional[:class:`bool`]
-        A tribool that indicates if the help command should DM the user instead of
-        sending it to the channel it received it from. If the boolean is set to
-        ``True``, then all help output is DM'd. If ``False``, none of the help
-        output is DM'd. If ``None``, then the bot will only DM when the help
-        message becomes too long (dictated by more than :attr:`dm_help_threshold` characters).
-        Defaults to ``False``.
-    dm_help_threshold: Optional[:class:`int`]
-        The number of characters the paginator must accumulate before getting DM'd to the
-        user if :attr:`dm_help` is set to ``None``. Defaults to 1000.
-    no_category: :class:`str`
-        The string used when there is a command which does not belong to any category(cog).
-        Useful for i18n. Defaults to ``"No Category"``
-    paginator: :class:`Paginator`
-        The paginator used to paginate the help command output.
-    """
-
-    def __init__(self, **options):
-        self.sort_commands = options.pop('sort_commands', True)
-        self.commands_heading = options.pop('commands_heading', "Commands")
-        self.dm_help = options.pop('dm_help', False)
-        self.dm_help_threshold = options.pop('dm_help_threshold', 1000)
-        self.aliases_heading = options.pop('aliases_heading', "Aliases:")
-        self.no_category = options.pop('no_category', 'No Category')
-        self.paginator = options.pop('paginator', None)
-
-        if self.paginator is None:
-            self.paginator = Paginator(suffix=None, prefix=None)
-
-        super().__init__(**options)
-
-    async def send_pages(self):
-        """A helper utility to send the page output from :attr:`paginator` to the destination."""
-        destination = self.get_destination()
-        for page in self.paginator.pages:
-            await destination.send(page)
-
-    def get_opening_note(self):
-        """Returns help command's opening note. This is mainly useful to override for i18n purposes.
-
-        The default implementation returns ::
-
-            Use `{prefix}{command_name} [command]` for more info on a command.
-            You can also use `{prefix}{command_name} [category]` for more info on a category.
-
-        Returns
-        -------
-        :class:`str`
-            The help command opening note.
-        """
-        command_name = self.invoked_with
-        return "Use `{0}{1} [command]` for more info on a command.\n" \
-               "You can also use `{0}{1} [category]` for more info on a category.".format(self.clean_prefix, command_name)
-
-    def get_command_signature(self, command):
-        return '%s%s %s' % (self.clean_prefix, command.qualified_name, command.signature)
-
-    def get_ending_note(self):
-        """Return the help command's ending note. This is mainly useful to override for i18n purposes.
-
-        The default implementation does nothing.
-
-        Returns
-        -------
-        :class:`str`
-            The help command ending note.
-        """
-        return None
-
-    def add_bot_commands_formatting(self, commands, heading):
-        """Adds the minified bot heading with commands to the output.
-
-        The formatting should be added to the :attr:`paginator`.
-
-        The default implementation is a bold underline heading followed
-        by commands separated by an EN SPACE (U+2002) in the next line.
-
-        Parameters
-        -----------
-        commands: Sequence[:class:`Command`]
-            A list of commands that belong to the heading.
-        heading: :class:`str`
-            The heading to add to the line.
-        """
-        if commands:
-            # U+2002 Middle Dot
-            joined = '\u2002'.join(c.name for c in commands)
-            self.paginator.add_line('__**%s**__' % heading)
-            self.paginator.add_line(joined)
-
-    def add_subcommand_formatting(self, command):
-        """Adds formatting information on a subcommand.
-
-        The formatting should be added to the :attr:`paginator`.
-
-        The default implementation is the prefix and the :attr:`Command.qualified_name`
-        optionally followed by an En dash and the command's :attr:`Command.short_doc`.
-
-        Parameters
-        -----------
-        command: :class:`Command`
-            The command to show information of.
-        """
-        fmt = '{0}{1} \N{EN DASH} {2}' if command.short_doc else '{0}{1}'
-        self.paginator.add_line(fmt.format(self.clean_prefix, command.qualified_name, command.short_doc))
-
-    def add_aliases_formatting(self, aliases):
-        """Adds the formatting information on a command's aliases.
-
-        The formatting should be added to the :attr:`paginator`.
-
-        The default implementation is the :attr:`aliases_heading` bolded
-        followed by a comma separated list of aliases.
-
-        This is not called if there are no aliases to format.
-
-        Parameters
-        -----------
-        aliases: Sequence[:class:`str`]
-            A list of aliases to format.
-        """
-        self.paginator.add_line('**%s** %s' % (self.aliases_heading, ', '.join(aliases)), empty=True)
-
-    def add_command_formatting(self, command):
-        """A utility function to format commands and groups.
-
-        Parameters
-        ------------
-        command: :class:`Command`
-            The command to format.
-        """
-
-        if command.description:
-            self.paginator.add_line(command.description, empty=True)
-
-        signature = self.get_command_signature(command)
-        if command.aliases:
-            self.paginator.add_line(signature)
-            self.add_aliases_formatting(command.aliases)
-        else:
-            self.paginator.add_line(signature, empty=True)
-
-        if command.help:
-            try:
-                self.paginator.add_line(command.help, empty=True)
-            except RuntimeError:
-                for line in command.help.splitlines():
-                    self.paginator.add_line(line)
-                self.paginator.add_line()
-
-    def get_destination(self):
-        ctx = self.context
-        if self.dm_help is True:
-            return ctx.author
-        elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
-            return ctx.author
-        else:
-            return ctx.channel
-
-    async def prepare_help_command(self, ctx, command):
-        self.paginator.clear()
-        await super().prepare_help_command(ctx, command)
-
-    async def send_bot_help(self, mapping):
-        ctx = self.context
-        bot = ctx.bot
-
-        if bot.description:
-            self.paginator.add_line(bot.description, empty=True)
-
-        note = self.get_opening_note()
-        if note:
-            self.paginator.add_line(note, empty=True)
-
-        no_category = '\u200b{0.no_category}'.format(self)
-        def get_category(command, *, no_category=no_category):
-            cog = command.cog
-            return cog.qualified_name if cog is not None else no_category
-
-        filtered = await self.filter_commands(bot.commands, sort=True, key=get_category)
-        to_iterate = itertools.groupby(filtered, key=get_category)
-
-        for category, commands in to_iterate:
-            commands = sorted(commands, key=lambda c: c.name) if self.sort_commands else list(commands)
-            self.add_bot_commands_formatting(commands, category)
-
-        note = self.get_ending_note()
-        if note:
-            self.paginator.add_line()
-            self.paginator.add_line(note)
-
-        await self.send_pages()
-
-    async def send_cog_help(self, cog):
-        bot = self.context.bot
-        if bot.description:
-            self.paginator.add_line(bot.description, empty=True)
-
-        note = self.get_opening_note()
-        if note:
-            self.paginator.add_line(note, empty=True)
-
-        if cog.description:
-            self.paginator.add_line(cog.description, empty=True)
-
-        filtered = await self.filter_commands(cog.get_commands(), sort=self.sort_commands)
-        if filtered:
-            self.paginator.add_line('**%s %s**' % (cog.qualified_name, self.commands_heading))
-            for command in filtered:
-                self.add_subcommand_formatting(command)
-
-            note = self.get_ending_note()
-            if note:
-                self.paginator.add_line()
-                self.paginator.add_line(note)
-
-        await self.send_pages()
-
-    async def send_group_help(self, group):
-        self.add_command_formatting(group)
-
-        filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
-        if filtered:
-            note = self.get_opening_note()
-            if note:
-                self.paginator.add_line(note, empty=True)
-
-            self.paginator.add_line('**%s**' % self.commands_heading)
-            for command in filtered:
-                self.add_subcommand_formatting(command)
-
-            note = self.get_ending_note()
-            if note:
-                self.paginator.add_line()
-                self.paginator.add_line(note)
-
-        await self.send_pages()
-
-    async def send_command_help(self, command):
-        self.add_command_formatting(command)
-        self.paginator.close_page()
-        await self.send_pages()
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import itertools
+import copy
+import functools
+import re
+
+from typing import (
+    TYPE_CHECKING,
+    Optional,
+    Generator,
+    List,
+    TypeVar,
+    Callable,
+    Any,
+    Dict,
+    Tuple,
+    Iterable,
+    Sequence,
+    Mapping,
+)
+
+import discord.utils
+from discord.utils import MISSING
+
+from .core import Group, Command, get_signature_parameters
+from .errors import CommandError
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    import discord.abc
+
+    from .bot import BotBase
+    from .context import Context
+    from .cog import Cog
+    from .parameters import Parameter
+
+    from ._types import (
+        UserCheck,
+        BotT,
+        _Bot,
+    )
+
+__all__ = (
+    'Paginator',
+    'HelpCommand',
+    'DefaultHelpCommand',
+    'MinimalHelpCommand',
+)
+
+FuncT = TypeVar('FuncT', bound=Callable[..., Any])
+
+# help -> shows info of bot on top/bottom and lists subcommands
+# help command -> shows detailed info of command
+# help command <subcommand chain> -> same as above
+
+# <description>
+
+# <command signature with aliases>
+
+# <long doc>
+
+# Cog:
+#   <command> <shortdoc>
+#   <command> <shortdoc>
+# Other Cog:
+#   <command> <shortdoc>
+# No Category:
+#   <command> <shortdoc>
+
+# Type <prefix>help command for more info on a command.
+# You can also type <prefix>help category for more info on a category.
+
+
+class Paginator:
+    """A class that aids in paginating code blocks for Discord messages.
+
+    .. container:: operations
+
+        .. describe:: len(x)
+
+            Returns the total number of characters in the paginator.
+
+    Attributes
+    -----------
+    prefix: Optional[:class:`str`]
+        The prefix inserted to every page. e.g. three backticks, if any.
+    suffix: Optional[:class:`str`]
+        The suffix appended at the end of every page. e.g. three backticks, if any.
+    max_size: :class:`int`
+        The maximum amount of codepoints allowed in a page.
+    linesep: :class:`str`
+        The character string inserted between lines. e.g. a newline character.
+            .. versionadded:: 1.7
+    """
+
+    def __init__(
+        self, prefix: Optional[str] = '```', suffix: Optional[str] = '```', max_size: int = 2000, linesep: str = '\n'
+    ) -> None:
+        self.prefix: Optional[str] = prefix
+        self.suffix: Optional[str] = suffix
+        self.max_size: int = max_size
+        self.linesep: str = linesep
+        self.clear()
+
+    def clear(self) -> None:
+        """Clears the paginator to have no pages."""
+        if self.prefix is not None:
+            self._current_page: List[str] = [self.prefix]
+            self._count: int = len(self.prefix) + self._linesep_len  # prefix + newline
+        else:
+            self._current_page = []
+            self._count = 0
+        self._pages: List[str] = []
+
+    @property
+    def _prefix_len(self) -> int:
+        return len(self.prefix) if self.prefix else 0
+
+    @property
+    def _suffix_len(self) -> int:
+        return len(self.suffix) if self.suffix else 0
+
+    @property
+    def _linesep_len(self) -> int:
+        return len(self.linesep)
+
+    def add_line(self, line: str = '', *, empty: bool = False) -> None:
+        """Adds a line to the current page.
+
+        If the line exceeds the :attr:`max_size` then an exception
+        is raised.
+
+        Parameters
+        -----------
+        line: :class:`str`
+            The line to add.
+        empty: :class:`bool`
+            Indicates if another empty line should be added.
+
+        Raises
+        ------
+        RuntimeError
+            The line was too big for the current :attr:`max_size`.
+        """
+        max_page_size = self.max_size - self._prefix_len - self._suffix_len - 2 * self._linesep_len
+        if len(line) > max_page_size:
+            raise RuntimeError(f'Line exceeds maximum page size {max_page_size}')
+
+        if self._count + len(line) + self._linesep_len > self.max_size - self._suffix_len:
+            self.close_page()
+
+        self._count += len(line) + self._linesep_len
+        self._current_page.append(line)
+
+        if empty:
+            self._current_page.append('')
+            self._count += self._linesep_len
+
+    def close_page(self) -> None:
+        """Prematurely terminate a page."""
+        if self.suffix is not None:
+            self._current_page.append(self.suffix)
+        self._pages.append(self.linesep.join(self._current_page))
+
+        if self.prefix is not None:
+            self._current_page = [self.prefix]
+            self._count = len(self.prefix) + self._linesep_len  # prefix + linesep
+        else:
+            self._current_page = []
+            self._count = 0
+
+    def __len__(self) -> int:
+        total = sum(len(p) for p in self._pages)
+        return total + self._count
+
+    @property
+    def pages(self) -> List[str]:
+        """List[:class:`str`]: Returns the rendered list of pages."""
+        # we have more than just the prefix in our current page
+        if len(self._current_page) > (0 if self.prefix is None else 1):
+            self.close_page()
+        return self._pages
+
+    def __repr__(self) -> str:
+        fmt = '<Paginator prefix: {0.prefix!r} suffix: {0.suffix!r} linesep: {0.linesep!r} max_size: {0.max_size} count: {0._count}>'
+        return fmt.format(self)
+
+
+def _not_overridden(f: FuncT) -> FuncT:
+    f.__help_command_not_overridden__ = True
+    return f
+
+
+class _HelpCommandImpl(Command):
+    def __init__(self, inject: HelpCommand, *args: Any, **kwargs: Any) -> None:
+        super().__init__(inject.command_callback, *args, **kwargs)
+        self._original: HelpCommand = inject
+        self._injected: HelpCommand = inject
+        self.params: Dict[str, Parameter] = get_signature_parameters(inject.command_callback, globals(), skip_parameters=1)
+
+    async def prepare(self, ctx: Context[Any]) -> None:
+        self._injected = injected = self._original.copy()
+        injected.context = ctx
+        self.callback = injected.command_callback
+        self.params = get_signature_parameters(injected.command_callback, globals(), skip_parameters=1)
+
+        on_error = injected.on_help_command_error
+        if not hasattr(on_error, '__help_command_not_overridden__'):
+            if self.cog is not None:
+                self.on_error = self._on_error_cog_implementation
+            else:
+                self.on_error = on_error
+
+        await super().prepare(ctx)
+
+    async def _parse_arguments(self, ctx: Context[BotT]) -> None:
+        # Make the parser think we don't have a cog so it doesn't
+        # inject the parameter into `ctx.args`.
+        original_cog = self.cog
+        self.cog = None
+        try:
+            await super()._parse_arguments(ctx)
+        finally:
+            self.cog = original_cog
+
+    async def _on_error_cog_implementation(self, _, ctx: Context[BotT], error: CommandError) -> None:
+        await self._injected.on_help_command_error(ctx, error)
+
+    def _inject_into_cog(self, cog: Cog) -> None:
+        # Warning: hacky
+
+        # Make the cog think that get_commands returns this command
+        # as well if we inject it without modifying __cog_commands__
+        # since that's used for the injection and ejection of cogs.
+        def wrapped_get_commands(
+            *, _original: Callable[[], List[Command[Any, ..., Any]]] = cog.get_commands
+        ) -> List[Command[Any, ..., Any]]:
+            ret = _original()
+            ret.append(self)
+            return ret
+
+        # Ditto here
+        def wrapped_walk_commands(
+            *, _original: Callable[[], Generator[Command[Any, ..., Any], None, None]] = cog.walk_commands
+        ):
+            yield from _original()
+            yield self
+
+        functools.update_wrapper(wrapped_get_commands, cog.get_commands)
+        functools.update_wrapper(wrapped_walk_commands, cog.walk_commands)
+        cog.get_commands = wrapped_get_commands
+        cog.walk_commands = wrapped_walk_commands
+        self.cog = cog
+
+    def _eject_cog(self) -> None:
+        if self.cog is None:
+            return
+
+        # revert back into their original methods
+        cog = self.cog
+        cog.get_commands = cog.get_commands.__wrapped__
+        cog.walk_commands = cog.walk_commands.__wrapped__
+        self.cog = None
+
+
+class HelpCommand:
+    r"""The base implementation for help command formatting.
+
+    .. note::
+
+        Internally instances of this class are deep copied every time
+        the command itself is invoked to prevent a race condition
+        mentioned in :issue:`2123`.
+
+        This means that relying on the state of this class to be
+        the same between command invocations would not work as expected.
+
+    Attributes
+    ------------
+    context: Optional[:class:`Context`]
+        The context that invoked this help formatter. This is generally set after
+        the help command assigned, :func:`command_callback`\, has been called.
+    show_hidden: :class:`bool`
+        Specifies if hidden commands should be shown in the output.
+        Defaults to ``False``.
+    verify_checks: Optional[:class:`bool`]
+        Specifies if commands should have their :attr:`.Command.checks` called
+        and verified. If ``True``, always calls :attr:`.Command.checks`.
+        If ``None``, only calls :attr:`.Command.checks` in a guild setting.
+        If ``False``, never calls :attr:`.Command.checks`. Defaults to ``True``.
+
+        .. versionchanged:: 1.7
+    command_attrs: :class:`dict`
+        A dictionary of options to pass in for the construction of the help command.
+        This allows you to change the command behaviour without actually changing
+        the implementation of the command. The attributes will be the same as the
+        ones passed in the :class:`.Command` constructor.
+    """
+
+    MENTION_TRANSFORMS = {
+        '@everyone': '@\u200beveryone',
+        '@here': '@\u200bhere',
+        r'<@!?[0-9]{17,22}>': '@deleted-user',
+        r'<@&[0-9]{17,22}>': '@deleted-role',
+    }
+
+    MENTION_PATTERN = re.compile('|'.join(MENTION_TRANSFORMS.keys()))
+
+    if TYPE_CHECKING:
+        __original_kwargs__: Dict[str, Any]
+        __original_args__: Tuple[Any, ...]
+
+    def __new__(cls, *args: Any, **kwargs: Any) -> Self:
+        # To prevent race conditions of a single instance while also allowing
+        # for settings to be passed the original arguments passed must be assigned
+        # to allow for easier copies (which will be made when the help command is actually called)
+        # see issue 2123
+        self = super().__new__(cls)
+
+        # Shallow copies cannot be used in this case since it is not unusual to pass
+        # instances that need state, e.g. Paginator or what have you into the function
+        # The keys can be safely copied as-is since they're 99.99% certain of being
+        # string keys
+        deepcopy = copy.deepcopy
+        self.__original_kwargs__ = {k: deepcopy(v) for k, v in kwargs.items()}
+        self.__original_args__ = deepcopy(args)
+        return self
+
+    def __init__(self, **options: Any) -> None:
+        self.show_hidden: bool = options.pop('show_hidden', False)
+        self.verify_checks: bool = options.pop('verify_checks', True)
+        self.command_attrs: Dict[str, Any]
+        self.command_attrs = attrs = options.pop('command_attrs', {})
+        attrs.setdefault('name', 'help')
+        attrs.setdefault('help', 'Shows this message')
+        self.context: Context[_Bot] = MISSING
+        self._command_impl = _HelpCommandImpl(self, **self.command_attrs)
+
+    def copy(self) -> Self:
+        obj = self.__class__(*self.__original_args__, **self.__original_kwargs__)
+        obj._command_impl = self._command_impl
+        return obj
+
+    def _add_to_bot(self, bot: BotBase) -> None:
+        command = _HelpCommandImpl(self, **self.command_attrs)
+        bot.add_command(command)
+        self._command_impl = command
+
+    def _remove_from_bot(self, bot: BotBase) -> None:
+        bot.remove_command(self._command_impl.name)
+        self._command_impl._eject_cog()
+
+    def add_check(self, func: UserCheck[Context[Any]], /) -> None:
+        """
+        Adds a check to the help command.
+
+        .. versionadded:: 1.4
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        ----------
+        func
+            The function that will be used as a check.
+        """
+
+        self._command_impl.add_check(func)
+
+    def remove_check(self, func: UserCheck[Context[Any]], /) -> None:
+        """
+        Removes a check from the help command.
+
+        This function is idempotent and will not raise an exception if
+        the function is not in the command's checks.
+
+        .. versionadded:: 1.4
+
+        .. versionchanged:: 2.0
+
+            ``func`` parameter is now positional-only.
+
+        Parameters
+        ----------
+        func
+            The function to remove from the checks.
+        """
+
+        self._command_impl.remove_check(func)
+
+    def get_bot_mapping(self) -> Dict[Optional[Cog], List[Command[Any, ..., Any]]]:
+        """Retrieves the bot mapping passed to :meth:`send_bot_help`."""
+        bot = self.context.bot
+        mapping: Dict[Optional[Cog], List[Command[Any, ..., Any]]] = {cog: cog.get_commands() for cog in bot.cogs.values()}
+        mapping[None] = [c for c in bot.commands if c.cog is None]
+        return mapping
+
+    @property
+    def invoked_with(self) -> Optional[str]:
+        """Similar to :attr:`Context.invoked_with` except properly handles
+        the case where :meth:`Context.send_help` is used.
+
+        If the help command was used regularly then this returns
+        the :attr:`Context.invoked_with` attribute. Otherwise, if
+        it the help command was called using :meth:`Context.send_help`
+        then it returns the internal command name of the help command.
+
+        Returns
+        ---------
+        Optional[:class:`str`]
+            The command name that triggered this invocation.
+        """
+        command_name = self._command_impl.name
+        ctx = self.context
+        if ctx is MISSING or ctx.command is None or ctx.command.qualified_name != command_name:
+            return command_name
+        return ctx.invoked_with
+
+    def get_command_signature(self, command: Command[Any, ..., Any], /) -> str:
+        """Retrieves the signature portion of the help page.
+
+        .. versionchanged:: 2.0
+
+            ``command`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        command: :class:`Command`
+            The command to get the signature of.
+
+        Returns
+        --------
+        :class:`str`
+            The signature for the command.
+        """
+        parent: Optional[Group[Any, ..., Any]] = command.parent  # type: ignore # the parent will be a Group
+        entries = []
+        while parent is not None:
+            if not parent.signature or parent.invoke_without_command:
+                entries.append(parent.name)
+            else:
+                entries.append(parent.name + ' ' + parent.signature)
+            parent = parent.parent  # type: ignore
+        parent_sig = ' '.join(reversed(entries))
+
+        if len(command.aliases) > 0:
+            aliases = '|'.join(command.aliases)
+            fmt = f'[{command.name}|{aliases}]'
+            if parent_sig:
+                fmt = parent_sig + ' ' + fmt
+            alias = fmt
+        else:
+            alias = command.name if not parent_sig else parent_sig + ' ' + command.name
+
+        return f'{self.context.clean_prefix}{alias} {command.signature}'
+
+    def remove_mentions(self, string: str, /) -> str:
+        """Removes mentions from the string to prevent abuse.
+
+        This includes ``@everyone``, ``@here``, member mentions and role mentions.
+
+        .. versionchanged:: 2.0
+
+            ``string`` parameter is now positional-only.
+
+        Returns
+        -------
+        :class:`str`
+            The string with mentions removed.
+        """
+
+        def replace(obj: re.Match, *, transforms: Dict[str, str] = self.MENTION_TRANSFORMS) -> str:
+            return transforms.get(obj.group(0), '@invalid')
+
+        return self.MENTION_PATTERN.sub(replace, string)
+
+    @property
+    def cog(self) -> Optional[Cog]:
+        """A property for retrieving or setting the cog for the help command.
+
+        When a cog is set for the help command, it is as-if the help command
+        belongs to that cog. All cog special methods will apply to the help
+        command and it will be automatically unset on unload.
+
+        To unbind the cog from the help command, you can set it to ``None``.
+
+        Returns
+        --------
+        Optional[:class:`Cog`]
+            The cog that is currently set for the help command.
+        """
+        return self._command_impl.cog
+
+    @cog.setter
+    def cog(self, cog: Optional[Cog]) -> None:
+        # Remove whatever cog is currently valid, if any
+        self._command_impl._eject_cog()
+
+        # If a new cog is set then inject it.
+        if cog is not None:
+            self._command_impl._inject_into_cog(cog)
+
+    def command_not_found(self, string: str, /) -> str:
+        """|maybecoro|
+
+        A method called when a command is not found in the help command.
+        This is useful to override for i18n.
+
+        Defaults to ``No command called {0} found.``
+
+        .. versionchanged:: 2.0
+
+            ``string`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        string: :class:`str`
+            The string that contains the invalid command. Note that this has
+            had mentions removed to prevent abuse.
+
+        Returns
+        ---------
+        :class:`str`
+            The string to use when a command has not been found.
+        """
+        return f'No command called "{string}" found.'
+
+    def subcommand_not_found(self, command: Command[Any, ..., Any], string: str, /) -> str:
+        """|maybecoro|
+
+        A method called when a command did not have a subcommand requested in the help command.
+        This is useful to override for i18n.
+
+        Defaults to either:
+
+        - ``'Command "{command.qualified_name}" has no subcommands.'``
+            - If there is no subcommand in the ``command`` parameter.
+        - ``'Command "{command.qualified_name}" has no subcommand named {string}'``
+            - If the ``command`` parameter has subcommands but not one named ``string``.
+
+        .. versionchanged:: 2.0
+
+            ``command`` and ``string`` parameters are now positional-only.
+
+        Parameters
+        ------------
+        command: :class:`Command`
+            The command that did not have the subcommand requested.
+        string: :class:`str`
+            The string that contains the invalid subcommand. Note that this has
+            had mentions removed to prevent abuse.
+
+        Returns
+        ---------
+        :class:`str`
+            The string to use when the command did not have the subcommand requested.
+        """
+        if isinstance(command, Group) and len(command.all_commands) > 0:
+            return f'Command "{command.qualified_name}" has no subcommand named {string}'
+        return f'Command "{command.qualified_name}" has no subcommands.'
+
+    async def filter_commands(
+        self,
+        commands: Iterable[Command[Any, ..., Any]],
+        /,
+        *,
+        sort: bool = False,
+        key: Optional[Callable[[Command[Any, ..., Any]], Any]] = None,
+    ) -> List[Command[Any, ..., Any]]:
+        """|coro|
+
+        Returns a filtered list of commands and optionally sorts them.
+
+        This takes into account the :attr:`verify_checks` and :attr:`show_hidden`
+        attributes.
+
+        .. versionchanged:: 2.0
+
+            ``commands`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        commands: Iterable[:class:`Command`]
+            An iterable of commands that are getting filtered.
+        sort: :class:`bool`
+            Whether to sort the result.
+        key: Optional[Callable[[:class:`Command`], Any]]
+            An optional key function to pass to :func:`py:sorted` that
+            takes a :class:`Command` as its sole parameter. If ``sort`` is
+            passed as ``True`` then this will default as the command name.
+
+        Returns
+        ---------
+        List[:class:`Command`]
+            A list of commands that passed the filter.
+        """
+
+        if sort and key is None:
+            key = lambda c: c.name
+
+        iterator = commands if self.show_hidden else filter(lambda c: not c.hidden, commands)
+
+        if self.verify_checks is False:
+            # if we do not need to verify the checks then we can just
+            # run it straight through normally without using await.
+            return sorted(iterator, key=key) if sort else list(iterator)  # type: ignore # the key shouldn't be None
+
+        if self.verify_checks is None and not self.context.guild:
+            # if verify_checks is None and we're in a DM, don't verify
+            return sorted(iterator, key=key) if sort else list(iterator)  # type: ignore
+
+        # if we're here then we need to check every command if it can run
+        async def predicate(cmd: Command[Any, ..., Any]) -> bool:
+            try:
+                return await cmd.can_run(self.context)
+            except CommandError:
+                return False
+
+        ret = []
+        for cmd in iterator:
+            valid = await predicate(cmd)
+            if valid:
+                ret.append(cmd)
+
+        if sort:
+            ret.sort(key=key)
+        return ret
+
+    def get_max_size(self, commands: Sequence[Command[Any, ..., Any]], /) -> int:
+        """Returns the largest name length of the specified command list.
+
+        .. versionchanged:: 2.0
+
+            ``commands`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        commands: Sequence[:class:`Command`]
+            A sequence of commands to check for the largest size.
+
+        Returns
+        --------
+        :class:`int`
+            The maximum width of the commands.
+        """
+
+        as_lengths = (discord.utils._string_width(c.name) for c in commands)
+        return max(as_lengths, default=0)
+
+    def get_destination(self) -> discord.abc.MessageableChannel:
+        """Returns the :class:`~discord.abc.Messageable` where the help command will be output.
+
+        You can override this method to customise the behaviour.
+
+        By default this returns the context's channel.
+
+        Returns
+        -------
+        :class:`.abc.Messageable`
+            The destination where the help command will be output.
+        """
+        return self.context.channel
+
+    async def send_error_message(self, error: str, /) -> None:
+        """|coro|
+
+        Handles the implementation when an error happens in the help command.
+        For example, the result of :meth:`command_not_found` will be passed here.
+
+        You can override this method to customise the behaviour.
+
+        By default, this sends the error message to the destination
+        specified by :meth:`get_destination`.
+
+        .. note::
+
+            You can access the invocation context with :attr:`HelpCommand.context`.
+
+        .. versionchanged:: 2.0
+
+            ``error`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        error: :class:`str`
+            The error message to display to the user. Note that this has
+            had mentions removed to prevent abuse.
+        """
+        destination = self.get_destination()
+        await destination.send(error)
+
+    @_not_overridden
+    async def on_help_command_error(self, ctx: Context[BotT], error: CommandError, /) -> None:
+        """|coro|
+
+        The help command's error handler, as specified by :ref:`ext_commands_error_handler`.
+
+        Useful to override if you need some specific behaviour when the error handler
+        is called.
+
+        By default this method does nothing and just propagates to the default
+        error handlers.
+
+        .. versionchanged:: 2.0
+
+            ``ctx`` and ``error`` parameters are now positional-only.
+
+        Parameters
+        ------------
+        ctx: :class:`Context`
+            The invocation context.
+        error: :class:`CommandError`
+            The error that was raised.
+        """
+        pass
+
+    async def send_bot_help(self, mapping: Mapping[Optional[Cog], List[Command[Any, ..., Any]]], /) -> None:
+        """|coro|
+
+        Handles the implementation of the bot command page in the help command.
+        This function is called when the help command is called with no arguments.
+
+        It should be noted that this method does not return anything -- rather the
+        actual message sending should be done inside this method. Well behaved subclasses
+        should use :meth:`get_destination` to know where to send, as this is a customisation
+        point for other users.
+
+        You can override this method to customise the behaviour.
+
+        .. note::
+
+            You can access the invocation context with :attr:`HelpCommand.context`.
+
+            Also, the commands in the mapping are not filtered. To do the filtering
+            you will have to call :meth:`filter_commands` yourself.
+
+        .. versionchanged:: 2.0
+
+            ``mapping`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        mapping: Mapping[Optional[:class:`Cog`], List[:class:`Command`]]
+            A mapping of cogs to commands that have been requested by the user for help.
+            The key of the mapping is the :class:`~.commands.Cog` that the command belongs to, or
+            ``None`` if there isn't one, and the value is a list of commands that belongs to that cog.
+        """
+        return None
+
+    async def send_cog_help(self, cog: Cog, /) -> None:
+        """|coro|
+
+        Handles the implementation of the cog page in the help command.
+        This function is called when the help command is called with a cog as the argument.
+
+        It should be noted that this method does not return anything -- rather the
+        actual message sending should be done inside this method. Well behaved subclasses
+        should use :meth:`get_destination` to know where to send, as this is a customisation
+        point for other users.
+
+        You can override this method to customise the behaviour.
+
+        .. note::
+
+            You can access the invocation context with :attr:`HelpCommand.context`.
+
+            To get the commands that belong to this cog see :meth:`Cog.get_commands`.
+            The commands returned not filtered. To do the filtering you will have to call
+            :meth:`filter_commands` yourself.
+
+        .. versionchanged:: 2.0
+
+            ``cog`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        cog: :class:`Cog`
+            The cog that was requested for help.
+        """
+        return None
+
+    async def send_group_help(self, group: Group[Any, ..., Any], /) -> None:
+        """|coro|
+
+        Handles the implementation of the group page in the help command.
+        This function is called when the help command is called with a group as the argument.
+
+        It should be noted that this method does not return anything -- rather the
+        actual message sending should be done inside this method. Well behaved subclasses
+        should use :meth:`get_destination` to know where to send, as this is a customisation
+        point for other users.
+
+        You can override this method to customise the behaviour.
+
+        .. note::
+
+            You can access the invocation context with :attr:`HelpCommand.context`.
+
+            To get the commands that belong to this group without aliases see
+            :attr:`Group.commands`. The commands returned not filtered. To do the
+            filtering you will have to call :meth:`filter_commands` yourself.
+
+        .. versionchanged:: 2.0
+
+            ``group`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        group: :class:`Group`
+            The group that was requested for help.
+        """
+        return None
+
+    async def send_command_help(self, command: Command[Any, ..., Any], /) -> None:
+        """|coro|
+
+        Handles the implementation of the single command page in the help command.
+
+        It should be noted that this method does not return anything -- rather the
+        actual message sending should be done inside this method. Well behaved subclasses
+        should use :meth:`get_destination` to know where to send, as this is a customisation
+        point for other users.
+
+        You can override this method to customise the behaviour.
+
+        .. note::
+
+            You can access the invocation context with :attr:`HelpCommand.context`.
+
+        .. admonition:: Showing Help
+            :class: helpful
+
+            There are certain attributes and methods that are helpful for a help command
+            to show such as the following:
+
+            - :attr:`Command.help`
+            - :attr:`Command.brief`
+            - :attr:`Command.short_doc`
+            - :attr:`Command.description`
+            - :meth:`get_command_signature`
+
+            There are more than just these attributes but feel free to play around with
+            these to help you get started to get the output that you want.
+
+        .. versionchanged:: 2.0
+
+            ``command`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        command: :class:`Command`
+            The command that was requested for help.
+        """
+        return None
+
+    async def prepare_help_command(self, ctx: Context[BotT], command: Optional[str] = None, /) -> None:
+        """|coro|
+
+        A low level method that can be used to prepare the help command
+        before it does anything. For example, if you need to prepare
+        some state in your subclass before the command does its processing
+        then this would be the place to do it.
+
+        The default implementation does nothing.
+
+        .. note::
+
+            This is called *inside* the help command callback body. So all
+            the usual rules that happen inside apply here as well.
+
+        .. versionchanged:: 2.0
+
+            ``ctx`` and ``command`` parameters are now positional-only.
+
+        Parameters
+        -----------
+        ctx: :class:`Context`
+            The invocation context.
+        command: Optional[:class:`str`]
+            The argument passed to the help command.
+        """
+        pass
+
+    async def command_callback(self, ctx: Context[BotT], /, *, command: Optional[str] = None) -> None:
+        """|coro|
+
+        The actual implementation of the help command.
+
+        It is not recommended to override this method and instead change
+        the behaviour through the methods that actually get dispatched.
+
+        - :meth:`send_bot_help`
+        - :meth:`send_cog_help`
+        - :meth:`send_group_help`
+        - :meth:`send_command_help`
+        - :meth:`get_destination`
+        - :meth:`command_not_found`
+        - :meth:`subcommand_not_found`
+        - :meth:`send_error_message`
+        - :meth:`on_help_command_error`
+        - :meth:`prepare_help_command`
+
+        .. versionchanged:: 2.0
+
+            ``ctx`` parameter is now positional-only.
+        """
+        await self.prepare_help_command(ctx, command)
+
+        bot = ctx.bot
+
+        if command is None:
+            mapping = self.get_bot_mapping()
+            return await self.send_bot_help(mapping)
+
+        # Check if it's a cog
+        cog = bot.get_cog(command)
+        if cog is not None:
+            return await self.send_cog_help(cog)
+
+        maybe_coro = discord.utils.maybe_coroutine
+
+        # If it's not a cog then it's a command.
+        # Since we want to have detailed errors when someone
+        # passes an invalid subcommand, we need to walk through
+        # the command group chain ourselves.
+        keys = command.split(' ')
+        cmd = bot.all_commands.get(keys[0])
+        if cmd is None:
+            string = await maybe_coro(self.command_not_found, self.remove_mentions(keys[0]))
+            return await self.send_error_message(string)
+
+        for key in keys[1:]:
+            try:
+                found = cmd.all_commands.get(key)  # type: ignore
+            except AttributeError:
+                string = await maybe_coro(self.subcommand_not_found, cmd, self.remove_mentions(key))
+                return await self.send_error_message(string)
+            else:
+                if found is None:
+                    string = await maybe_coro(self.subcommand_not_found, cmd, self.remove_mentions(key))
+                    return await self.send_error_message(string)
+                cmd = found
+
+        if isinstance(cmd, Group):
+            return await self.send_group_help(cmd)
+        else:
+            return await self.send_command_help(cmd)
+
+
+class DefaultHelpCommand(HelpCommand):
+    """The implementation of the default help command.
+
+    This inherits from :class:`HelpCommand`.
+
+    It extends it with the following attributes.
+
+    Attributes
+    ------------
+    width: :class:`int`
+        The maximum number of characters that fit in a line.
+        Defaults to 80.
+    sort_commands: :class:`bool`
+        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
+    dm_help: Optional[:class:`bool`]
+        A tribool that indicates if the help command should DM the user instead of
+        sending it to the channel it received it from. If the boolean is set to
+        ``True``, then all help output is DM'd. If ``False``, none of the help
+        output is DM'd. If ``None``, then the bot will only DM when the help
+        message becomes too long (dictated by more than :attr:`dm_help_threshold` characters).
+        Defaults to ``False``.
+    dm_help_threshold: Optional[:class:`int`]
+        The number of characters the paginator must accumulate before getting DM'd to the
+        user if :attr:`dm_help` is set to ``None``. Defaults to 1000.
+    indent: :class:`int`
+        How much to indent the commands from a heading. Defaults to ``2``.
+    arguments_heading: :class:`str`
+        The arguments list's heading string used when the help command is invoked with a command name.
+        Useful for i18n. Defaults to ``"Arguments:"``.
+        Shown when :attr:`.show_parameter_descriptions` is ``True``.
+
+        .. versionadded:: 2.0
+    show_parameter_descriptions: :class:`bool`
+        Whether to show the parameter descriptions. Defaults to ``True``.
+        Setting this to ``False`` will revert to showing the :attr:`~.commands.Command.signature` instead.
+
+        .. versionadded:: 2.0
+    commands_heading: :class:`str`
+        The command list's heading string used when the help command is invoked with a category name.
+        Useful for i18n. Defaults to ``"Commands:"``
+    default_argument_description: :class:`str`
+        The default argument description string used when the argument's :attr:`~.commands.Parameter.description` is ``None``.
+        Useful for i18n. Defaults to ``"No description given."``
+
+        .. versionadded:: 2.0
+    no_category: :class:`str`
+        The string used when there is a command which does not belong to any category(cog).
+        Useful for i18n. Defaults to ``"No Category"``
+    paginator: :class:`Paginator`
+        The paginator used to paginate the help command output.
+    """
+
+    def __init__(self, **options: Any) -> None:
+        self.width: int = options.pop('width', 80)
+        self.indent: int = options.pop('indent', 2)
+        self.sort_commands: bool = options.pop('sort_commands', True)
+        self.dm_help: bool = options.pop('dm_help', False)
+        self.dm_help_threshold: int = options.pop('dm_help_threshold', 1000)
+        self.arguments_heading: str = options.pop('arguments_heading', "Arguments:")
+        self.commands_heading: str = options.pop('commands_heading', 'Commands:')
+        self.default_argument_description: str = options.pop('default_argument_description', 'No description given')
+        self.no_category: str = options.pop('no_category', 'No Category')
+        self.paginator: Paginator = options.pop('paginator', None)
+        self.show_parameter_descriptions: bool = options.pop('show_parameter_descriptions', True)
+
+        if self.paginator is None:
+            self.paginator: Paginator = Paginator()
+
+        super().__init__(**options)
+
+    def shorten_text(self, text: str, /) -> str:
+        """:class:`str`: Shortens text to fit into the :attr:`width`.
+
+        .. versionchanged:: 2.0
+
+            ``text`` parameter is now positional-only.
+        """
+        if len(text) > self.width:
+            return text[: self.width - 3].rstrip() + '...'
+        return text
+
+    def get_ending_note(self) -> str:
+        """:class:`str`: Returns help command's ending note. This is mainly useful to override for i18n purposes."""
+        command_name = self.invoked_with
+        return (
+            f'Type {self.context.clean_prefix}{command_name} command for more info on a command.\n'
+            f'You can also type {self.context.clean_prefix}{command_name} category for more info on a category.'
+        )
+
+    def get_command_signature(self, command: Command[Any, ..., Any], /) -> str:
+        """Retrieves the signature portion of the help page.
+
+        Calls :meth:`~.HelpCommand.get_command_signature` if :attr:`show_parameter_descriptions` is ``False``
+        else returns a modified signature where the command parameters are not shown.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        ------------
+        command: :class:`Command`
+            The command to get the signature of.
+
+        Returns
+        --------
+        :class:`str`
+            The signature for the command.
+        """
+        if not self.show_parameter_descriptions:
+            return super().get_command_signature(command)
+
+        name = command.name
+        if len(command.aliases) > 0:
+            aliases = '|'.join(command.aliases)
+            name = f'[{command.name}|{aliases}]'
+
+        return f'{self.context.clean_prefix}{name}'
+
+    def add_indented_commands(
+        self, commands: Sequence[Command[Any, ..., Any]], /, *, heading: str, max_size: Optional[int] = None
+    ) -> None:
+        """Indents a list of commands after the specified heading.
+
+        The formatting is added to the :attr:`paginator`.
+
+        The default implementation is the command name indented by
+        :attr:`indent` spaces, padded to ``max_size`` followed by
+        the command's :attr:`Command.short_doc` and then shortened
+        to fit into the :attr:`width`.
+
+        .. versionchanged:: 2.0
+            ``commands`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        commands: Sequence[:class:`Command`]
+            A list of commands to indent for output.
+        heading: :class:`str`
+            The heading to add to the output. This is only added
+            if the list of commands is greater than 0.
+        max_size: Optional[:class:`int`]
+            The max size to use for the gap between indents.
+            If unspecified, calls :meth:`~HelpCommand.get_max_size` on the
+            commands parameter.
+        """
+
+        if not commands:
+            return
+
+        self.paginator.add_line(heading)
+        max_size = max_size or self.get_max_size(commands)
+
+        get_width = discord.utils._string_width
+        for command in commands:
+            name = command.name
+            width = max_size - (get_width(name) - len(name))
+            entry = f'{self.indent * " "}{name:<{width}} {command.short_doc}'
+            self.paginator.add_line(self.shorten_text(entry))
+
+    def add_command_arguments(self, command: Command[Any, ..., Any], /) -> None:
+        """Indents a list of command arguments after the :attr:`.arguments_heading`.
+
+        The default implementation is the argument :attr:`~.commands.Parameter.name` indented by
+        :attr:`indent` spaces, padded to ``max_size`` using :meth:`~HelpCommand.get_max_size`
+        followed by the argument's :attr:`~.commands.Parameter.description` or
+        :attr:`.default_argument_description` and then shortened
+        to fit into the :attr:`width` and then :attr:`~.commands.Parameter.displayed_default`
+        between () if one is present after that.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        -----------
+        command: :class:`Command`
+            The command to list the arguments for.
+        """
+        arguments = command.clean_params.values()
+        if not arguments:
+            return
+
+        self.paginator.add_line(self.arguments_heading)
+        max_size = self.get_max_size(arguments)  # type: ignore # not a command
+
+        get_width = discord.utils._string_width
+        for argument in arguments:
+            name = argument.name
+            width = max_size - (get_width(name) - len(name))
+            entry = f'{self.indent * " "}{name:<{width}} {argument.description or self.default_argument_description}'
+            # we do not want to shorten the default value, if any.
+            entry = self.shorten_text(entry)
+            if argument.displayed_default is not None:
+                entry += f' (default: {argument.displayed_default})'
+
+            self.paginator.add_line(entry)
+
+    async def send_pages(self) -> None:
+        """|coro|
+
+        A helper utility to send the page output from :attr:`paginator` to the destination.
+        """
+        destination = self.get_destination()
+        for page in self.paginator.pages:
+            await destination.send(page)
+
+    def add_command_formatting(self, command: Command[Any, ..., Any], /) -> None:
+        """A utility function to format the non-indented block of commands and groups.
+
+        .. versionchanged:: 2.0
+
+            ``command`` parameter is now positional-only.
+
+        .. versionchanged:: 2.0
+            :meth:`.add_command_arguments` is now called if :attr:`.show_parameter_descriptions` is ``True``.
+
+        Parameters
+        ------------
+        command: :class:`Command`
+            The command to format.
+        """
+
+        if command.description:
+            self.paginator.add_line(command.description, empty=True)
+
+        signature = self.get_command_signature(command)
+        self.paginator.add_line(signature, empty=True)
+
+        if command.help:
+            try:
+                self.paginator.add_line(command.help, empty=True)
+            except RuntimeError:
+                for line in command.help.splitlines():
+                    self.paginator.add_line(line)
+                self.paginator.add_line()
+
+        if self.show_parameter_descriptions:
+            self.add_command_arguments(command)
+
+    def get_destination(self) -> discord.abc.Messageable:
+        ctx = self.context
+        if self.dm_help is True:
+            return ctx.author
+        elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
+            return ctx.author
+        else:
+            return ctx.channel
+
+    async def prepare_help_command(self, ctx: Context[BotT], command: Optional[str], /) -> None:
+        self.paginator.clear()
+        await super().prepare_help_command(ctx, command)
+
+    async def send_bot_help(self, mapping: Mapping[Optional[Cog], List[Command[Any, ..., Any]]], /) -> None:
+        ctx = self.context
+        bot = ctx.bot
+
+        if bot.description:
+            # <description> portion
+            self.paginator.add_line(bot.description, empty=True)
+
+        no_category = f'\u200b{self.no_category}:'
+
+        def get_category(command, *, no_category=no_category):
+            cog = command.cog
+            return cog.qualified_name + ':' if cog is not None else no_category
+
+        filtered = await self.filter_commands(bot.commands, sort=True, key=get_category)
+        max_size = self.get_max_size(filtered)
+        to_iterate = itertools.groupby(filtered, key=get_category)
+
+        # Now we can add the commands to the page.
+        for category, commands in to_iterate:
+            commands = sorted(commands, key=lambda c: c.name) if self.sort_commands else list(commands)
+            self.add_indented_commands(commands, heading=category, max_size=max_size)
+
+        note = self.get_ending_note()
+        if note:
+            self.paginator.add_line()
+            self.paginator.add_line(note)
+
+        await self.send_pages()
+
+    async def send_command_help(self, command: Command[Any, ..., Any], /) -> None:
+        self.add_command_formatting(command)
+        self.paginator.close_page()
+        await self.send_pages()
+
+    async def send_group_help(self, group: Group[Any, ..., Any], /) -> None:
+        self.add_command_formatting(group)
+
+        filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
+        self.add_indented_commands(filtered, heading=self.commands_heading)
+
+        if filtered:
+            note = self.get_ending_note()
+            if note:
+                self.paginator.add_line()
+                self.paginator.add_line(note)
+
+        await self.send_pages()
+
+    async def send_cog_help(self, cog: Cog, /) -> None:
+        if cog.description:
+            self.paginator.add_line(cog.description, empty=True)
+
+        filtered = await self.filter_commands(cog.get_commands(), sort=self.sort_commands)
+        self.add_indented_commands(filtered, heading=self.commands_heading)
+
+        note = self.get_ending_note()
+        if note:
+            self.paginator.add_line()
+            self.paginator.add_line(note)
+
+        await self.send_pages()
+
+
+class MinimalHelpCommand(HelpCommand):
+    """An implementation of a help command with minimal output.
+
+    This inherits from :class:`HelpCommand`.
+
+    Attributes
+    ------------
+    sort_commands: :class:`bool`
+        Whether to sort the commands in the output alphabetically. Defaults to ``True``.
+    commands_heading: :class:`str`
+        The command list's heading string used when the help command is invoked with a category name.
+        Useful for i18n. Defaults to ``"Commands"``
+    aliases_heading: :class:`str`
+        The alias list's heading string used to list the aliases of the command. Useful for i18n.
+        Defaults to ``"Aliases:"``.
+    dm_help: Optional[:class:`bool`]
+        A tribool that indicates if the help command should DM the user instead of
+        sending it to the channel it received it from. If the boolean is set to
+        ``True``, then all help output is DM'd. If ``False``, none of the help
+        output is DM'd. If ``None``, then the bot will only DM when the help
+        message becomes too long (dictated by more than :attr:`dm_help_threshold` characters).
+        Defaults to ``False``.
+    dm_help_threshold: Optional[:class:`int`]
+        The number of characters the paginator must accumulate before getting DM'd to the
+        user if :attr:`dm_help` is set to ``None``. Defaults to 1000.
+    no_category: :class:`str`
+        The string used when there is a command which does not belong to any category(cog).
+        Useful for i18n. Defaults to ``"No Category"``
+    paginator: :class:`Paginator`
+        The paginator used to paginate the help command output.
+    """
+
+    def __init__(self, **options: Any) -> None:
+        self.sort_commands: bool = options.pop('sort_commands', True)
+        self.commands_heading: str = options.pop('commands_heading', 'Commands')
+        self.dm_help: bool = options.pop('dm_help', False)
+        self.dm_help_threshold: int = options.pop('dm_help_threshold', 1000)
+        self.aliases_heading: str = options.pop('aliases_heading', 'Aliases:')
+        self.no_category: str = options.pop('no_category', 'No Category')
+        self.paginator: Paginator = options.pop('paginator', None)
+
+        if self.paginator is None:
+            self.paginator: Paginator = Paginator(suffix=None, prefix=None)
+
+        super().__init__(**options)
+
+    async def send_pages(self) -> None:
+        """|coro|
+
+        A helper utility to send the page output from :attr:`paginator` to the destination.
+        """
+        destination = self.get_destination()
+        for page in self.paginator.pages:
+            await destination.send(page)
+
+    def get_opening_note(self) -> str:
+        """Returns help command's opening note. This is mainly useful to override for i18n purposes.
+
+        The default implementation returns ::
+
+            Use `{prefix}{command_name} [command]` for more info on a command.
+            You can also use `{prefix}{command_name} [category]` for more info on a category.
+
+        Returns
+        -------
+        :class:`str`
+            The help command opening note.
+        """
+        command_name = self.invoked_with
+        return (
+            f'Use `{self.context.clean_prefix}{command_name} [command]` for more info on a command.\n'
+            f'You can also use `{self.context.clean_prefix}{command_name} [category]` for more info on a category.'
+        )
+
+    def get_command_signature(self, command: Command[Any, ..., Any], /) -> str:
+        return f'{self.context.clean_prefix}{command.qualified_name} {command.signature}'
+
+    def get_ending_note(self) -> str:
+        """Return the help command's ending note. This is mainly useful to override for i18n purposes.
+
+        The default implementation does nothing.
+
+        Returns
+        -------
+        :class:`str`
+            The help command ending note.
+        """
+        return ''
+
+    def add_bot_commands_formatting(self, commands: Sequence[Command[Any, ..., Any]], heading: str, /) -> None:
+        """Adds the minified bot heading with commands to the output.
+
+        The formatting should be added to the :attr:`paginator`.
+
+        The default implementation is a bold underline heading followed
+        by commands separated by an EN SPACE (U+2002) in the next line.
+
+        .. versionchanged:: 2.0
+
+            ``commands`` and ``heading`` parameters are now positional-only.
+
+        Parameters
+        -----------
+        commands: Sequence[:class:`Command`]
+            A list of commands that belong to the heading.
+        heading: :class:`str`
+            The heading to add to the line.
+        """
+        if commands:
+            # U+2002 Middle Dot
+            joined = '\u2002'.join(c.name for c in commands)
+            self.paginator.add_line(f'__**{heading}**__')
+            self.paginator.add_line(joined)
+
+    def add_subcommand_formatting(self, command: Command[Any, ..., Any], /) -> None:
+        """Adds formatting information on a subcommand.
+
+        The formatting should be added to the :attr:`paginator`.
+
+        The default implementation is the prefix and the :attr:`Command.qualified_name`
+        optionally followed by an En dash and the command's :attr:`Command.short_doc`.
+
+        .. versionchanged:: 2.0
+
+            ``command`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        command: :class:`Command`
+            The command to show information of.
+        """
+        fmt = '{0}{1} \N{EN DASH} {2}' if command.short_doc else '{0}{1}'
+        self.paginator.add_line(fmt.format(self.context.clean_prefix, command.qualified_name, command.short_doc))
+
+    def add_aliases_formatting(self, aliases: Sequence[str], /) -> None:
+        """Adds the formatting information on a command's aliases.
+
+        The formatting should be added to the :attr:`paginator`.
+
+        The default implementation is the :attr:`aliases_heading` bolded
+        followed by a comma separated list of aliases.
+
+        This is not called if there are no aliases to format.
+
+        .. versionchanged:: 2.0
+
+            ``aliases`` parameter is now positional-only.
+
+        Parameters
+        -----------
+        aliases: Sequence[:class:`str`]
+            A list of aliases to format.
+        """
+        self.paginator.add_line(f'**{self.aliases_heading}** {", ".join(aliases)}', empty=True)
+
+    def add_command_formatting(self, command: Command[Any, ..., Any], /) -> None:
+        """A utility function to format commands and groups.
+
+        .. versionchanged:: 2.0
+
+            ``command`` parameter is now positional-only.
+
+        Parameters
+        ------------
+        command: :class:`Command`
+            The command to format.
+        """
+
+        if command.description:
+            self.paginator.add_line(command.description, empty=True)
+
+        signature = self.get_command_signature(command)
+        if command.aliases:
+            self.paginator.add_line(signature)
+            self.add_aliases_formatting(command.aliases)
+        else:
+            self.paginator.add_line(signature, empty=True)
+
+        if command.help:
+            try:
+                self.paginator.add_line(command.help, empty=True)
+            except RuntimeError:
+                for line in command.help.splitlines():
+                    self.paginator.add_line(line)
+                self.paginator.add_line()
+
+    def get_destination(self) -> discord.abc.Messageable:
+        ctx = self.context
+        if self.dm_help is True:
+            return ctx.author
+        elif self.dm_help is None and len(self.paginator) > self.dm_help_threshold:
+            return ctx.author
+        else:
+            return ctx.channel
+
+    async def prepare_help_command(self, ctx: Context[BotT], command: Optional[str], /) -> None:
+        self.paginator.clear()
+        await super().prepare_help_command(ctx, command)
+
+    async def send_bot_help(self, mapping: Mapping[Optional[Cog], List[Command[Any, ..., Any]]], /) -> None:
+        ctx = self.context
+        bot = ctx.bot
+
+        if bot.description:
+            self.paginator.add_line(bot.description, empty=True)
+
+        note = self.get_opening_note()
+        if note:
+            self.paginator.add_line(note, empty=True)
+
+        no_category = f'\u200b{self.no_category}'
+
+        def get_category(command: Command[Any, ..., Any], *, no_category: str = no_category) -> str:
+            cog = command.cog
+            return cog.qualified_name if cog is not None else no_category
+
+        filtered = await self.filter_commands(bot.commands, sort=True, key=get_category)
+        to_iterate = itertools.groupby(filtered, key=get_category)
+
+        for category, commands in to_iterate:
+            commands = sorted(commands, key=lambda c: c.name) if self.sort_commands else list(commands)
+            self.add_bot_commands_formatting(commands, category)
+
+        note = self.get_ending_note()
+        if note:
+            self.paginator.add_line()
+            self.paginator.add_line(note)
+
+        await self.send_pages()
+
+    async def send_cog_help(self, cog: Cog, /) -> None:
+        bot = self.context.bot
+        if bot.description:
+            self.paginator.add_line(bot.description, empty=True)
+
+        note = self.get_opening_note()
+        if note:
+            self.paginator.add_line(note, empty=True)
+
+        if cog.description:
+            self.paginator.add_line(cog.description, empty=True)
+
+        filtered = await self.filter_commands(cog.get_commands(), sort=self.sort_commands)
+        if filtered:
+            self.paginator.add_line(f'**{cog.qualified_name} {self.commands_heading}**')
+            for command in filtered:
+                self.add_subcommand_formatting(command)
+
+            note = self.get_ending_note()
+            if note:
+                self.paginator.add_line()
+                self.paginator.add_line(note)
+
+        await self.send_pages()
+
+    async def send_group_help(self, group: Group[Any, ..., Any], /) -> None:
+        self.add_command_formatting(group)
+
+        filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
+        if filtered:
+            note = self.get_opening_note()
+            if note:
+                self.paginator.add_line(note, empty=True)
+
+            self.paginator.add_line(f'**{self.commands_heading}**')
+            for command in filtered:
+                self.add_subcommand_formatting(command)
+
+            note = self.get_ending_note()
+            if note:
+                self.paginator.add_line()
+                self.paginator.add_line(note)
+
+        await self.send_pages()
+
+    async def send_command_help(self, command: Command[Any, ..., Any], /) -> None:
+        self.add_command_formatting(command)
+        self.paginator.close_page()
+        await self.send_pages()
```

### Comparing `discord.py-self-1.9.2/discord/ext/commands/view.py` & `discord.py-self-2.0.0/discord/ext/commands/view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,194 +1,196 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .errors import UnexpectedQuoteError, InvalidEndOfQuotedStringError, ExpectedClosingQuoteError
-
-# map from opening quotes to closing quotes
-_quotes = {
-    '"': '"',
-    "‘": "’",
-    "‚": "‛",
-    "“": "”",
-    "„": "‟",
-    "⹂": "⹂",
-    "「": "」",
-    "『": "』",
-    "〝": "〞",
-    "﹁": "﹂",
-    "﹃": "﹄",
-    "＂": "＂",
-    "｢": "｣",
-    "«": "»",
-    "‹": "›",
-    "《": "》",
-    "〈": "〉",
-}
-_all_quotes = set(_quotes.keys()) | set(_quotes.values())
-
-class StringView:
-    def __init__(self, buffer):
-        self.index = 0
-        self.buffer = buffer
-        self.end = len(buffer)
-        self.previous = 0
-
-    @property
-    def current(self):
-        return None if self.eof else self.buffer[self.index]
-
-    @property
-    def eof(self):
-        return self.index >= self.end
-
-    def undo(self):
-        self.index = self.previous
-
-    def skip_ws(self):
-        pos = 0
-        while not self.eof:
-            try:
-                current = self.buffer[self.index + pos]
-                if not current.isspace():
-                    break
-                pos += 1
-            except IndexError:
-                break
-
-        self.previous = self.index
-        self.index += pos
-        return self.previous != self.index
-
-    def skip_string(self, string):
-        strlen = len(string)
-        if self.buffer[self.index:self.index + strlen] == string:
-            self.previous = self.index
-            self.index += strlen
-            return True
-        return False
-
-    def read_rest(self):
-        result = self.buffer[self.index:]
-        self.previous = self.index
-        self.index = self.end
-        return result
-
-    def read(self, n):
-        result = self.buffer[self.index:self.index + n]
-        self.previous = self.index
-        self.index += n
-        return result
-
-    def get(self):
-        try:
-            result = self.buffer[self.index + 1]
-        except IndexError:
-            result = None
-
-        self.previous = self.index
-        self.index += 1
-        return result
-
-    def get_word(self):
-        pos = 0
-        while not self.eof:
-            try:
-                current = self.buffer[self.index + pos]
-                if current.isspace():
-                    break
-                pos += 1
-            except IndexError:
-                break
-        self.previous = self.index
-        result = self.buffer[self.index:self.index + pos]
-        self.index += pos
-        return result
-
-    def get_quoted_word(self):
-        current = self.current
-        if current is None:
-            return None
-
-        close_quote = _quotes.get(current)
-        is_quoted = bool(close_quote)
-        if is_quoted:
-            result = []
-            _escaped_quotes = (current, close_quote)
-        else:
-            result = [current]
-            _escaped_quotes = _all_quotes
-
-        while not self.eof:
-            current = self.get()
-            if not current:
-                if is_quoted:
-                    # unexpected EOF
-                    raise ExpectedClosingQuoteError(close_quote)
-                return ''.join(result)
-
-            # currently we accept strings in the format of "hello world"
-            # to embed a quote inside the string you must escape it: "a \"world\""
-            if current == '\\':
-                next_char = self.get()
-                if not next_char:
-                    # string ends with \ and no character after it
-                    if is_quoted:
-                        # if we're quoted then we're expecting a closing quote
-                        raise ExpectedClosingQuoteError(close_quote)
-                    # if we aren't then we just let it through
-                    return ''.join(result)
-
-                if next_char in _escaped_quotes:
-                    # escaped quote
-                    result.append(next_char)
-                else:
-                    # different escape character, ignore it
-                    self.undo()
-                    result.append(current)
-                continue
-
-            if not is_quoted and current in _all_quotes:
-                # we aren't quoted
-                raise UnexpectedQuoteError(current)
-
-            # closing quote
-            if is_quoted and current == close_quote:
-                next_char = self.get()
-                valid_eof = not next_char or next_char.isspace()
-                if not valid_eof:
-                    raise InvalidEndOfQuotedStringError(next_char)
-
-                # we're quoted so it's okay
-                return ''.join(result)
-
-            if current.isspace() and not is_quoted:
-                # end of word found
-                return ''.join(result)
-
-            result.append(current)
-
-
-    def __repr__(self):
-        return '<StringView pos: {0.index} prev: {0.previous} end: {0.end} eof: {0.eof}>'.format(self)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import Optional
+
+from .errors import UnexpectedQuoteError, InvalidEndOfQuotedStringError, ExpectedClosingQuoteError
+
+# map from opening quotes to closing quotes
+_quotes = {
+    '"': '"',
+    "‘": "’",
+    "‚": "‛",
+    "“": "”",
+    "„": "‟",
+    "⹂": "⹂",
+    "「": "」",
+    "『": "』",
+    "〝": "〞",
+    "﹁": "﹂",
+    "﹃": "﹄",
+    "＂": "＂",
+    "｢": "｣",
+    "«": "»",
+    "‹": "›",
+    "《": "》",
+    "〈": "〉",
+}
+_all_quotes = set(_quotes.keys()) | set(_quotes.values())
+
+
+class StringView:
+    def __init__(self, buffer: str) -> None:
+        self.index: int = 0
+        self.buffer: str = buffer
+        self.end: int = len(buffer)
+        self.previous = 0
+
+    @property
+    def current(self) -> Optional[str]:
+        return None if self.eof else self.buffer[self.index]
+
+    @property
+    def eof(self) -> bool:
+        return self.index >= self.end
+
+    def undo(self) -> None:
+        self.index = self.previous
+
+    def skip_ws(self) -> bool:
+        pos = 0
+        while not self.eof:
+            try:
+                current = self.buffer[self.index + pos]
+                if not current.isspace():
+                    break
+                pos += 1
+            except IndexError:
+                break
+
+        self.previous = self.index
+        self.index += pos
+        return self.previous != self.index
+
+    def skip_string(self, string: str) -> bool:
+        strlen = len(string)
+        if self.buffer[self.index : self.index + strlen] == string:
+            self.previous = self.index
+            self.index += strlen
+            return True
+        return False
+
+    def read_rest(self) -> str:
+        result = self.buffer[self.index :]
+        self.previous = self.index
+        self.index = self.end
+        return result
+
+    def read(self, n: int) -> str:
+        result = self.buffer[self.index : self.index + n]
+        self.previous = self.index
+        self.index += n
+        return result
+
+    def get(self) -> Optional[str]:
+        try:
+            result = self.buffer[self.index + 1]
+        except IndexError:
+            result = None
+
+        self.previous = self.index
+        self.index += 1
+        return result
+
+    def get_word(self) -> str:
+        pos = 0
+        while not self.eof:
+            try:
+                current = self.buffer[self.index + pos]
+                if current.isspace():
+                    break
+                pos += 1
+            except IndexError:
+                break
+        self.previous: int = self.index
+        result = self.buffer[self.index : self.index + pos]
+        self.index += pos
+        return result
+
+    def get_quoted_word(self) -> Optional[str]:
+        current = self.current
+        if current is None:
+            return None
+
+        close_quote = _quotes.get(current)
+        is_quoted = bool(close_quote)
+        if is_quoted:
+            result = []
+            _escaped_quotes = (current, close_quote)
+        else:
+            result = [current]
+            _escaped_quotes = _all_quotes
+
+        while not self.eof:
+            current = self.get()
+            if not current:
+                if is_quoted:
+                    # unexpected EOF
+                    raise ExpectedClosingQuoteError(close_quote)
+                return ''.join(result)
+
+            # currently we accept strings in the format of "hello world"
+            # to embed a quote inside the string you must escape it: "a \"world\""
+            if current == '\\':
+                next_char = self.get()
+                if not next_char:
+                    # string ends with \ and no character after it
+                    if is_quoted:
+                        # if we're quoted then we're expecting a closing quote
+                        raise ExpectedClosingQuoteError(close_quote)
+                    # if we aren't then we just let it through
+                    return ''.join(result)
+
+                if next_char in _escaped_quotes:
+                    # escaped quote
+                    result.append(next_char)
+                else:
+                    # different escape character, ignore it
+                    self.undo()
+                    result.append(current)
+                continue
+
+            if not is_quoted and current in _all_quotes:
+                # we aren't quoted
+                raise UnexpectedQuoteError(current)
+
+            # closing quote
+            if is_quoted and current == close_quote:
+                next_char = self.get()
+                valid_eof = not next_char or next_char.isspace()
+                if not valid_eof:
+                    raise InvalidEndOfQuotedStringError(next_char)  # type: ignore # this will always be a string
+
+                # we're quoted so it's okay
+                return ''.join(result)
+
+            if current.isspace() and not is_quoted:
+                # end of word found
+                return ''.join(result)
+
+            result.append(current)
+
+    def __repr__(self) -> str:
+        return f'<StringView pos: {self.index} prev: {self.previous} end: {self.end} eof: {self.eof}>'
```

### Comparing `discord.py-self-1.9.2/discord/guild.py` & `discord.py-self-2.0.0/discord/abc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,2445 +1,2277 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import asyncio
-from datetime import datetime, timedelta
-import copy
-from collections import namedtuple
-import logging
-from math import ceil
-
-from . import utils
-from .role import Role
-from .member import Member, VoiceState
-from .emoji import Emoji
-from .errors import InvalidData
-from .permissions import PermissionOverwrite
-from .colour import Colour
-from .errors import InvalidArgument, ClientException
-from .channel import *
-from .enums import VoiceRegion, ChannelType, try_enum, VerificationLevel, ContentFilter, NotificationLevel
-from .mixins import Hashable
-from .user import User
-from .invite import Invite
-from .iterators import AuditLogIterator
-from .widget import Widget
-from .asset import Asset
-from .flags import SystemChannelFlags
-from .integrations import Integration
-
-
-BanEntry = namedtuple('BanEntry', 'reason user')
-_GuildLimit = namedtuple('_GuildLimit', 'emoji bitrate filesize')
-log = logging.getLogger(__name__)
-
-class Guild(Hashable):
-    """Represents a Discord guild.
-
-    This is referred to as a "server" in the official Discord UI.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two guilds are equal.
-
-        .. describe:: x != y
-
-            Checks if two guilds are not equal.
-
-        .. describe:: hash(x)
-
-            Returns the guild's hash.
-
-        .. describe:: str(x)
-
-            Returns the guild's name.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The guild name.
-    emojis: Tuple[:class:`Emoji`, ...]
-        All emojis that the guild owns.
-    region: :class:`VoiceRegion`
-        The region the guild belongs on. There is a chance that the region
-        will be a :class:`str` if the value is not recognised by the enumerator.
-    afk_timeout: :class:`int`
-        The timeout to get sent to the AFK channel.
-    afk_channel: Optional[:class:`VoiceChannel`]
-        The channel that denotes the AFK channel. ``None`` if it doesn't exist.
-    icon: Optional[:class:`str`]
-        The guild's icon.
-    id: :class:`int`
-        The guild's ID.
-    owner_id: :class:`int`
-        The guild owner's ID. Use :attr:`Guild.owner` instead.
-    unavailable: :class:`bool`
-        Indicates if the guild is unavailable. If this is ``True`` then the
-        reliability of other attributes outside of :attr:`Guild.id` is slim and they might
-        all be ``None``. It is best to not do anything with the guild if it is unavailable.
-
-        Check the :func:`on_guild_unavailable` and :func:`on_guild_available` events.
-    max_presences: Optional[:class:`int`]
-        The maximum amount of presences for the guild.
-    max_members: Optional[:class:`int`]
-        The maximum amount of members for the guild.
-
-        .. note::
-
-            This attribute is only available via :meth:`.Client.fetch_guild`.
-    max_video_channel_users: Optional[:class:`int`]
-        The maximum amount of users in a video channel.
-
-        .. versionadded:: 1.4
-    banner: Optional[:class:`str`]
-        The guild's banner.
-    description: Optional[:class:`str`]
-        The guild's description.
-    mfa_level: :class:`int`
-        Indicates the guild's two factor authorisation level. If this value is 0 then
-        the guild does not require 2FA for their administrative members. If the value is
-        1 then they do.
-    verification_level: :class:`VerificationLevel`
-        The guild's verification level.
-    explicit_content_filter: :class:`ContentFilter`
-        The guild's explicit content filter.
-    default_notifications: :class:`NotificationLevel`
-        The guild's notification settings.
-    features: List[:class:`str`]
-        A list of features that the guild has. They are currently as follows:
-
-        - ``VIP_REGIONS``: Guild has VIP voice regions
-        - ``VANITY_URL``: Guild can have a vanity invite URL (e.g. discord.gg/discord-api)
-        - ``INVITE_SPLASH``: Guild's invite page can have a special splash.
-        - ``VERIFIED``: Guild is a verified server.
-        - ``PARTNERED``: Guild is a partnered server.
-        - ``MORE_EMOJI``: Guild is allowed to have more than 50 custom emoji.
-        - ``DISCOVERABLE``: Guild shows up in Server Discovery.
-        - ``FEATURABLE``: Guild is able to be featured in Server Discovery.
-        - ``COMMUNITY``: Guild is a community server.
-        - ``COMMERCE``: Guild can sell things using store channels.
-        - ``PUBLIC``: Guild is a public guild.
-        - ``NEWS``: Guild can create news channels.
-        - ``BANNER``: Guild can upload and use a banner (i.e. :meth:`banner_url`).
-        - ``ANIMATED_ICON``: Guild can upload an animated icon.
-        - ``PUBLIC_DISABLED``: Guild cannot be public.
-        - ``WELCOME_SCREEN_ENABLED``: Guild has enabled the welcome screen
-        - ``MEMBER_VERIFICATION_GATE_ENABLED``: Guild has Membership Screening enabled.
-        - ``PREVIEW_ENABLED``: Guild can be viewed before being accepted via Membership Screening.
-
-    splash: Optional[:class:`str`]
-        The guild's invite splash.
-    premium_tier: :class:`int`
-        The premium tier for this guild. Corresponds to "Nitro Server" in the official UI.
-        The number goes from 0 to 3 inclusive.
-    premium_subscription_count: :class:`int`
-        The number of "boosts" this guild currently has.
-    preferred_locale: Optional[:class:`str`]
-        The preferred locale for the guild. Used when filtering Server Discovery
-        results to a specific language.
-    discovery_splash: :class:`str`
-        The guild's discovery splash.
-
-        .. versionadded:: 1.3
-    """
-
-    __slots__ = ('afk_timeout', 'afk_channel', '_members', '_channels', 'icon',
-                 'name', 'id', 'unavailable', 'banner', 'region', '_state',
-                 '_roles', '_member_count', '_large',
-                 'owner_id', 'mfa_level', 'emojis', 'features',
-                 'verification_level', 'explicit_content_filter', 'splash',
-                 '_voice_states', '_system_channel_id', 'default_notifications',
-                 'description', 'max_presences', 'max_members', 'max_video_channel_users',
-                 'premium_tier', 'premium_subscription_count', '_system_channel_flags',
-                 'preferred_locale', 'discovery_splash', '_rules_channel_id',
-                 '_public_updates_channel_id', '_online_count', '_subscribing')
-
-    _PREMIUM_GUILD_LIMITS = {
-        None: _GuildLimit(emoji=50, bitrate=96e3, filesize=8388608),
-        0: _GuildLimit(emoji=50, bitrate=96e3, filesize=8388608),
-        1: _GuildLimit(emoji=100, bitrate=128e3, filesize=8388608),
-        2: _GuildLimit(emoji=150, bitrate=256e3, filesize=52428800),
-        3: _GuildLimit(emoji=250, bitrate=384e3, filesize=104857600),
-    }
-
-    def __init__(self, *, data, state):
-        self._roles = {}
-        self._channels = {}
-        self._members = {}
-        self._voice_states = {}
-        self._state = state
-        self._from_data(data)
-
-    def _add_channel(self, channel):
-        self._channels[channel.id] = channel
-
-    def _remove_channel(self, channel):
-        self._channels.pop(channel.id, None)
-
-    def _voice_state_for(self, user_id):
-        return self._voice_states.get(user_id)
-
-    def _add_member(self, member):
-        self._members[member.id] = member
-
-    def _remove_member(self, member):
-        self._members.pop(member.id, None)
-
-    def __str__(self):
-        return self.name or ''
-
-    def __repr__(self):
-        attrs = (
-            'id', 'name', 'chunked'
-        )
-        resolved = ['%s=%r' % (attr, getattr(self, attr)) for attr in attrs]
-        resolved.append('member_count=%r' % getattr(self, '_member_count', None))
-        return '<Guild %s>' % ' '.join(resolved)
-
-    def _update_voice_state(self, data, channel_id):
-        user_id = int(data['user_id'])
-        channel = self.get_channel(channel_id)
-        try:
-            # check if we should remove the voice state from cache
-            if channel is None:
-                after = self._voice_states.pop(user_id)
-            else:
-                after = self._voice_states[user_id]
-
-            before = copy.copy(after)
-            after._update(data, channel)
-        except KeyError:
-            # if we're here then we're getting added into the cache
-            after = VoiceState(data=data, channel=channel)
-            before = VoiceState(data=data, channel=None)
-            self._voice_states[user_id] = after
-
-        member = self.get_member(user_id)
-        if member is None:
-            try:
-                member = Member(data=data['member'], state=self._state, guild=self)
-            except KeyError:
-                member = None
-
-        return member, before, after
-
-    def _add_role(self, role):
-        # roles get added to the bottom (position 1, pos 0 is @everyone)
-        # so since self.roles has the @everyone role, we can't increment
-        # its position because it's stuck at position 0. Luckily x += False
-        # is equivalent to adding 0. So we cast the position to a bool and
-        # increment it.
-        for r in self._roles.values():
-            r.position += (not r.is_default())
-
-        self._roles[role.id] = role
-
-    def _remove_role(self, role_id):
-        # this raises KeyError if it fails..
-        role = self._roles.pop(role_id)
-
-        # since it didn't, we can change the positions now
-        # basically the same as above except we only decrement
-        # the position if we're above the role we deleted.
-        for r in self._roles.values():
-            r.position -= r.position > role.position
-
-        return role
-
-    def _from_data(self, guild):
-        member_count = guild.get('member_count')
-        if member_count is not None:
-            self._member_count = member_count
-
-        self.name = guild.get('name')
-        self.region = try_enum(VoiceRegion, guild.get('region'))
-        self.verification_level = try_enum(VerificationLevel, guild.get('verification_level'))
-        self.default_notifications = try_enum(NotificationLevel, guild.get('default_message_notifications'))
-        self.explicit_content_filter = try_enum(ContentFilter, guild.get('explicit_content_filter', 0))
-        self.afk_timeout = guild.get('afk_timeout')
-        self.icon = guild.get('icon')
-        self.banner = guild.get('banner')
-        self.unavailable = guild.get('unavailable', False)
-        self.id = int(guild['id'])
-
-        state = self._state # speed up attribute access
-
-        for r in guild.get('roles', []):
-            role = Role(guild=self, data=r, state=state)
-            self._roles[role.id] = role
-
-        for c in guild.get('channels', []):
-            factory, ch_type = _channel_factory(c['type'])
-            if factory:
-                self._add_channel(factory(guild=self, data=c, state=state))
-
-        self.mfa_level = guild.get('mfa_level')
-        self.emojis = tuple(map(lambda d: state.store_emoji(self, d), guild.get('emojis', [])))
-        self.features = guild.get('features', [])
-        self.splash = guild.get('splash')
-        self._system_channel_id = utils._get_as_snowflake(guild, 'system_channel_id')
-        self.description = guild.get('description')
-        self.max_presences = guild.get('max_presences')
-        self.max_members = guild.get('max_members')
-        self.max_video_channel_users = guild.get('max_video_channel_users')
-        self.premium_tier = guild.get('premium_tier', 0)
-        self.premium_subscription_count = guild.get('premium_subscription_count') or 0
-        self._system_channel_flags = guild.get('system_channel_flags', 0)
-        self.preferred_locale = guild.get('preferred_locale')
-        self.discovery_splash = guild.get('discovery_splash')
-        self._rules_channel_id = utils._get_as_snowflake(guild, 'rules_channel_id')
-        self._public_updates_channel_id = utils._get_as_snowflake(guild, 'public_updates_channel_id')
-        self._online_count = guild.get('online_count')
-
-        for mdata in guild.get('merged_members', []):
-            try:
-                member = Member(data=mdata, guild=self, state=state)
-            except KeyError:
-                continue
-            self._add_member(member)
-
-        empty_tuple = tuple()
-        for presence in guild.get('merged_presences', []):
-            user_id = int(presence['user_id'])
-            member = self.get_member(user_id)
-            if member is not None:
-                member._presence_update(presence, empty_tuple)
-
-        _large = None if member_count is None else member_count >= 250
-        self._large = guild.get('large', _large)
-
-        self.owner_id = utils._get_as_snowflake(guild, 'owner_id')
-        self.afk_channel = self.get_channel(utils._get_as_snowflake(guild, 'afk_channel_id'))
-
-        for obj in guild.get('voice_states', []):
-            self._update_voice_state(obj, int(obj['channel_id']))
-
-    async def subscribe(self, delay=0.25, op_ranges=None, ticket=None, max_online=None):
-        """|coro|
-
-        Abuses the member sidebar to scrape all members*.
-
-        *Discord doesn't provide offline members for "large" guilds.
-        *If a guild doesn't have a channel (of any type) @everyone can view,
-        the subscribing currently fails. In the future, it'll pick the next
-        most-used role and look for a channel that role can view.
-
-        You can only request members from the sidebar in 100 member ranges, and
-        you can only specify up to 2 ranges per request.
-
-        This is a websocket operation and can be extremely slow.
-
-        Parameters
-        -----------
-        delay: Union[:class:`int`, :class:`float`]
-            Amount of time (in seconds) to wait before requesting the next 2 ranges.
-            Note: By default, we wait for the GUILD_MEMBER_LIST_UPDATE to arrive before
-            continuing. However, those arrive extremely fast so we need to add an extra
-            delay to try to avoid rate-limits.
-
-        Returns
-        --------
-        :class:`bool`
-            Whether the subscribing was successful.
-
-        .. versionadded:: 1.9
-        """
-
-        self._subscribing = True
-
-        if ticket:
-            await ticket.acquire()
-
-        state = self._state
-        ws = state._get_websocket()
-
-        def cleanup(*, successful):
-            if ticket:
-                ticket.release()
-            if successful:
-                self._subscribing = False
-            else:
-                del self._subscribing
-
-        def get_channel():
-            for channel in self.channels:
-                perms = channel.overwrites_for(self.default_role)
-                if perms.view_channel is None:
-                    perms = self.default_role.permissions
-                if perms.view_channel:
-                    return channel.id
-            return # TODO: Check for a "member" role and do the above
-
-        def get_ranges():
-            online = ceil(self._online_count / 100.0) * 100
-            ranges = []
-            for i in range(1, int(online / 100) + 1):
-                min = i * 100
-                max = min + 99
-                ranges.append([min, max])
-            return ranges
-
-        def get_current_ranges(ranges):
-            try:
-                current = [[0, 99]]
-                current.append(ranges.pop(0))
-                try:
-                    current.append(ranges.pop(0))
-                except IndexError:
-                    pass
-                return current
-            except:
-                return
-
-        channel_id = get_channel()
-        if not channel_id:
-            log.warn('Guild %s subscribing failed (no channels available).' % self.id)
-            cleanup(successful=False)
-            return False
-
-        def predicate(data):
-            if int(data['guild_id']) == self.id:
-                return any((opdata.get('range') in ranges_to_send for opdata in data.get('ops', [])))
-
-        log.debug("Subscribing to [[0, 99]] ranges for guild %s." % self.id)
-        ranges_to_send = [[0, 99]]
-        await ws.request_lazy_guild(self.id, channels={channel_id: ranges_to_send})
-
-        try:
-            await asyncio.wait_for(ws.wait_for('GUILD_MEMBER_LIST_UPDATE', predicate), timeout=60)
-        except asyncio.TimeoutError:
-            log.debug('Guild %s timed out waiting for subscribes.' % self.id)
-            cleanup(successful=False)
-            return False
-
-        for r in ranges_to_send:
-            if self._online_count in range(r[0], r[1]) or self.online_count < r[1]:
-                cleanup(successful=True)
-                return True
-
-        if max_online:
-            if self.online_count > max_online:
-                cleanup(successful=False)
-                return False
-
-        ranges = op_ranges or get_ranges()
-        if not ranges:
-            log.warn('Guild %s subscribing failed (could not fetch ranges).' % self.id)
-            cleanup(successful=False)
-            return False
-
-        while self._subscribing:
-            ranges_to_send = get_current_ranges(ranges)
-
-            if not ranges_to_send:
-                cleanup(successful=True)
-                return True
-
-            log.debug("Subscribing to %s ranges for guild %s." % (ranges_to_send, self.id))
-            await ws.request_lazy_guild(self.id, channels={channel_id: ranges_to_send})
-
-            try:
-                await asyncio.wait_for(ws.wait_for('GUILD_MEMBER_LIST_UPDATE', predicate), timeout=45)
-            except asyncio.TimeoutError:
-                log.debug('Guild %s timed out waiting for subscribes.' % self.id)
-                r = ranges_to_send[-1]
-                if self._online_count in range(r[0], r[1]) or self.online_count < r[1]:
-                    cleanup(successful=True)
-                    return True
-                else:
-                    cleanup(successful=False)
-                    return False
-
-            await asyncio.sleep(delay)
-
-            for r in ranges_to_send:
-                if ((self._online_count in range(r[0], r[1]) or self._online_count < r[1]) and self.large) or \
-                ((self._member_count in range(r[0], r[1]) or self._member_count < r[1]) and not self.large):
-                    cleanup(successful=True)
-                    return True
-
-    @property
-    def channels(self):
-        """List[:class:`abc.GuildChannel`]: A list of channels that belongs to this guild."""
-        return list(self._channels.values())
-
-    @property
-    def large(self):
-        """:class:`bool`: Indicates if the guild is a 'large' guild.
-
-        A large guild is defined as having more than ``large_threshold`` count
-        members, which for this library is set to the maximum of 250.
-        """
-        if self._large is None:
-            try:
-                return self._member_count >= 250
-            except AttributeError:
-                return len(self._members) >= 250
-        return self._large
-
-    @property
-    def voice_channels(self):
-        """List[:class:`VoiceChannel`]: A list of voice channels that belongs to this guild.
-
-        This is sorted by the position and are in UI order from top to bottom.
-        """
-        r = [ch for ch in self._channels.values() if isinstance(ch, VoiceChannel)]
-        r.sort(key=lambda c: (c.position, c.id))
-        return r
-
-    @property
-    def stage_channels(self):
-        """List[:class:`StageChannel`]: A list of voice channels that belongs to this guild.
-
-        .. versionadded:: 1.7
-
-        This is sorted by the position and are in UI order from top to bottom.
-        """
-        r = [ch for ch in self._channels.values() if isinstance(ch, StageChannel)]
-        r.sort(key=lambda c: (c.position, c.id))
-        return r
-
-    @property
-    def me(self):
-        """:class:`Member`: Similar to :attr:`Client.user` except an instance of :class:`Member`.
-        This is essentially used to get the member version of yourself.
-        """
-        self_id = self._state.user.id
-        return self.get_member(self_id)
-
-    @property
-    def voice_client(self):
-        """Optional[:class:`VoiceProtocol`]: Returns the :class:`VoiceProtocol` associated with this guild, if any."""
-        return self._state._get_voice_client(self.id)
-
-    @property
-    def text_channels(self):
-        """List[:class:`TextChannel`]: A list of text channels that belongs to this guild.
-
-        This is sorted by the position and are in UI order from top to bottom.
-        """
-        r = [ch for ch in self._channels.values() if isinstance(ch, TextChannel)]
-        r.sort(key=lambda c: (c.position, c.id))
-        return r
-
-    @property
-    def categories(self):
-        """List[:class:`CategoryChannel`]: A list of categories that belongs to this guild.
-
-        This is sorted by the position and are in UI order from top to bottom.
-        """
-        r = [ch for ch in self._channels.values() if isinstance(ch, CategoryChannel)]
-        r.sort(key=lambda c: (c.position, c.id))
-        return r
-
-    def by_category(self):
-        """Returns every :class:`CategoryChannel` and their associated channels.
-
-        These channels and categories are sorted in the official Discord UI order.
-
-        If the channels do not have a category, then the first element of the tuple is
-        ``None``.
-
-        Returns
-        --------
-        List[Tuple[Optional[:class:`CategoryChannel`], List[:class:`abc.GuildChannel`]]]:
-            The categories and their associated channels.
-        """
-        grouped = {}
-        for channel in self._channels.values():
-            if isinstance(channel, CategoryChannel):
-                grouped.setdefault(channel.id, [])
-                continue
-
-            try:
-                grouped[channel.category_id].append(channel)
-            except KeyError:
-                grouped[channel.category_id] = [channel]
-
-        def key(t):
-            k, v = t
-            return ((k.position, k.id) if k else (-1, -1), v)
-
-        _get = self._channels.get
-        as_list = [(_get(k), v) for k, v in grouped.items()]
-        as_list.sort(key=key)
-        for _, channels in as_list:
-            channels.sort(key=lambda c: (c._sorting_bucket, c.position, c.id))
-        return as_list
-
-    def get_channel(self, channel_id):
-        """Returns a channel with the given ID.
-
-        Parameters
-        -----------
-        channel_id: :class:`int`
-            The ID to search for.
-
-        Returns
-        --------
-        Optional[:class:`.abc.GuildChannel`]
-            The returned channel or ``None`` if not found.
-        """
-        return self._channels.get(channel_id)
-
-    @property
-    def system_channel(self):
-        """Optional[:class:`TextChannel`]: Returns the guild's channel used for system messages.
-
-        If no channel is set, then this returns ``None``.
-        """
-        channel_id = self._system_channel_id
-        return channel_id and self._channels.get(channel_id)
-
-    @property
-    def system_channel_flags(self):
-        """:class:`SystemChannelFlags`: Returns the guild's system channel settings."""
-        return SystemChannelFlags._from_value(self._system_channel_flags)
-
-    @property
-    def rules_channel(self):
-        """Optional[:class:`TextChannel`]: Return's the guild's channel used for the rules.
-        The guild must be a Community guild.
-
-        If no channel is set, then this returns ``None``.
-
-        .. versionadded:: 1.3
-        """
-        channel_id = self._rules_channel_id
-        return channel_id and self._channels.get(channel_id)
-
-    @property
-    def public_updates_channel(self):
-        """Optional[:class:`TextChannel`]: Return's the guild's channel where admins and
-        moderators of the guilds receive notices from Discord. The guild must be a
-        Community guild.
-
-        If no channel is set, then this returns ``None``.
-
-        .. versionadded:: 1.4
-        """
-        channel_id = self._public_updates_channel_id
-        return channel_id and self._channels.get(channel_id)
-
-    @property
-    def emoji_limit(self):
-        """:class:`int`: The maximum number of emoji slots this guild has."""
-        more_emoji = 200 if 'MORE_EMOJI' in self.features else 50
-        return max(more_emoji, self._PREMIUM_GUILD_LIMITS[self.premium_tier].emoji)
-
-    @property
-    def bitrate_limit(self):
-        """:class:`float`: The maximum bitrate for voice channels this guild can have."""
-        vip_guild = self._PREMIUM_GUILD_LIMITS[1].bitrate if 'VIP_REGIONS' in self.features else 96e3
-        return max(vip_guild, self._PREMIUM_GUILD_LIMITS[self.premium_tier].bitrate)
-
-    @property
-    def filesize_limit(self):
-        """:class:`int`: The maximum number of bytes files can have when uploaded to this guild."""
-        return self._PREMIUM_GUILD_LIMITS[self.premium_tier].filesize
-
-    @property
-    def members(self):
-        """List[:class:`Member`]: A list of members that belong to this guild."""
-        return list(self._members.values())
-
-    def get_member(self, user_id):
-        """Returns a member with the given ID.
-
-        Parameters
-        -----------
-        user_id: :class:`int`
-            The ID to search for.
-
-        Returns
-        --------
-        Optional[:class:`Member`]
-            The member or ``None`` if not found.
-        """
-        return self._members.get(user_id)
-
-    @property
-    def premium_subscribers(self):
-        """List[:class:`Member`]: A list of members who have "boosted" this guild."""
-        return [member for member in self.members if member.premium_since is not None]
-
-    @property
-    def roles(self):
-        """List[:class:`Role`]: Returns a :class:`list` of the guild's roles in hierarchy order.
-
-        The first element of this list will be the lowest role in the
-        hierarchy.
-        """
-        return sorted(self._roles.values())
-
-    def get_role(self, role_id):
-        """Returns a role with the given ID.
-
-        Parameters
-        -----------
-        role_id: :class:`int`
-            The ID to search for.
-
-        Returns
-        --------
-        Optional[:class:`Role`]
-            The role or ``None`` if not found.
-        """
-        return self._roles.get(role_id)
-
-    @property
-    def default_role(self):
-        """:class:`Role`: Gets the @everyone role that all members have by default."""
-        return self.get_role(self.id)
-
-    @property
-    def premium_subscriber_role(self):
-        """Optional[:class:`Role`]: Gets the premium subscriber role, AKA "boost" role, in this guild.
-
-        .. versionadded:: 1.6
-        """
-        for role in self._roles.values():
-            if role.is_premium_subscriber():
-                return role
-        return None
-
-    @property
-    def owner(self):
-        """Optional[:class:`Member`]: The member that owns the guild."""
-        return self.get_member(self.owner_id)
-
-    @property
-    def icon_url(self):
-        """:class:`Asset`: Returns the guild's icon asset."""
-        return self.icon_url_as()
-
-    def is_icon_animated(self):
-        """:class:`bool`: Returns True if the guild has an animated icon."""
-        return bool(self.icon and self.icon.startswith('a_'))
-
-    def icon_url_as(self, *, format=None, static_format='webp', size=1024):
-        """Returns an :class:`Asset` for the guild's icon.
-
-        The format must be one of 'webp', 'jpeg', 'jpg', 'png' or 'gif', and
-        'gif' is only valid for animated avatars. The size must be a power of 2
-        between 16 and 4096.
-
-        Parameters
-        -----------
-        format: Optional[:class:`str`]
-            The format to attempt to convert the icon to.
-            If the format is ``None``, then it is automatically
-            detected into either 'gif' or static_format depending on the
-            icon being animated or not.
-        static_format: Optional[:class:`str`]
-            Format to attempt to convert only non-animated icons to.
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_icon(self._state, self, format=format, static_format=static_format, size=size)
-
-    @property
-    def banner_url(self):
-        """:class:`Asset`: Returns the guild's banner asset."""
-        return self.banner_url_as()
-
-    def banner_url_as(self, *, format='webp', size=2048):
-        """Returns an :class:`Asset` for the guild's banner.
-
-        The format must be one of 'webp', 'jpeg', or 'png'. The
-        size must be a power of 2 between 16 and 4096.
-
-        Parameters
-        -----------
-        format: :class:`str`
-            The format to attempt to convert the banner to.
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_image(self._state, self.id, self.banner, 'banners', format=format, size=size)
-
-    @property
-    def splash_url(self):
-        """:class:`Asset`: Returns the guild's invite splash asset."""
-        return self.splash_url_as()
-
-    def splash_url_as(self, *, format='webp', size=2048):
-        """Returns an :class:`Asset` for the guild's invite splash.
-
-        The format must be one of 'webp', 'jpeg', 'jpg', or 'png'. The
-        size must be a power of 2 between 16 and 4096.
-
-        Parameters
-        -----------
-        format: :class:`str`
-            The format to attempt to convert the splash to.
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_image(self._state, self.id, self.splash, 'splashes', format=format, size=size)
-
-    @property
-    def discovery_splash_url(self):
-        """:class:`Asset`: Returns the guild's discovery splash asset.
-
-        .. versionadded:: 1.3
-        """
-        return self.discovery_splash_url_as()
-
-    def discovery_splash_url_as(self, *, format='webp', size=2048):
-        """Returns an :class:`Asset` for the guild's discovery splash.
-
-        The format must be one of 'webp', 'jpeg', 'jpg', or 'png'. The
-        size must be a power of 2 between 16 and 4096.
-
-        .. versionadded:: 1.3
-
-        Parameters
-        -----------
-        format: :class:`str`
-            The format to attempt to convert the splash to.
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_image(self._state, self.id, self.discovery_splash, 'discovery-splashes', format=format, size=size)
-
-    @property
-    def member_count(self):
-        """:class:`int`: Returns the true member count regardless of it being loaded fully or not."""
-        return self._member_count
-
-    @property
-    def online_count(self):
-        """:class:`int`: Returns the online member count. This only exists after the first GUILD_MEMBER_LIST_UPDATE."""
-        return self._online_count
-
-    @property
-    def chunked(self):
-        """:class:`bool`: Returns a boolean indicating if the guild is "chunked".
-
-        A chunked guild means that :attr:`member_count` is equal to the
-        number of members stored in the internal :attr:`members` cache.
-
-        If this value returns ``False``, then you should request for
-        offline members.
-        """
-        count = getattr(self, '_member_count', None)
-        if count is None:
-            return False
-        return count == len(self._members)
-
-    @property
-    def subscribed(self):
-        """:class:`bool`: Returns a boolean indicating if the guild is "subscribed".
-
-        A subscribed guild means that opcode 14s have been sent for every range
-        available. Note that every 100 new members, a new one has to be sent.
-
-        .. versionadded:: 1.9
-        """
-        try:
-            return not self._subscribing
-        except:
-            return False
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the guild's creation time in UTC."""
-        return utils.snowflake_time(self.id)
-
-    def get_member_named(self, name):
-        """Returns the first member found that matches the name provided.
-
-        The name can have an optional discriminator argument, e.g. "Jake#0001"
-        or "Jake" will both do the lookup. However the former will give a more
-        precise result. Note that the discriminator must have all 4 digits
-        for this to work.
-
-        If a nickname is passed, then it is looked up via the nickname. Note
-        however, that a nickname + discriminator combo will not lookup the nickname
-        but rather the username + discriminator combo due to nickname + discriminator
-        not being unique.
-
-        If no member is found, ``None`` is returned.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The name of the member to lookup with an optional discriminator.
-
-        Returns
-        --------
-        Optional[:class:`Member`]
-            The member in this guild with the associated name. If not found
-            then ``None`` is returned.
-        """
-
-        result = None
-        members = self.members
-        if len(name) > 5 and name[-5] == '#':
-            # The 5 length is checking to see if #0000 is in the string,
-            # as a#0000 has a length of 6, the minimum for a potential
-            # discriminator lookup.
-            potential_discriminator = name[-4:]
-
-            # do the actual lookup and return if found
-            # if it isn't found then we'll do a full name lookup below.
-            result = utils.get(members, name=name[:-5], discriminator=potential_discriminator)
-            if result is not None:
-                return result
-
-        def pred(m):
-            return m.nick == name or m.name == name
-
-        return utils.find(pred, members)
-
-    def _create_channel(self, name, overwrites, channel_type, category=None, **options):
-        if overwrites is None:
-            overwrites = {}
-        elif not isinstance(overwrites, dict):
-            raise InvalidArgument('overwrites parameter expects a dict.')
-
-        perms = []
-        for target, perm in overwrites.items():
-            if not isinstance(perm, PermissionOverwrite):
-                raise InvalidArgument('Expected PermissionOverwrite received {0.__name__}'.format(type(perm)))
-
-            allow, deny = perm.pair()
-            payload = {
-                'allow': allow.value,
-                'deny': deny.value,
-                'id': target.id
-            }
-
-            if isinstance(target, Role):
-                payload['type'] = 'role'
-            else:
-                payload['type'] = 'member'
-
-            perms.append(payload)
-
-        try:
-            options['rate_limit_per_user'] = options.pop('slowmode_delay')
-        except KeyError:
-            pass
-
-        try:
-            rtc_region = options.pop('rtc_region')
-        except KeyError:
-            pass
-        else:
-            options['rtc_region'] = None if rtc_region is None else str(rtc_region)
-
-        parent_id = category.id if category else None
-        return self._state.http.create_channel(self.id, channel_type.value, name=name, parent_id=parent_id,
-                                               permission_overwrites=perms, **options)
-
-    async def create_text_channel(self, name, *, overwrites=None, category=None, **options):
-        """|coro|
-
-        Creates a :class:`TextChannel` for the guild.
-
-        Note that you need the :attr:`~Permissions.manage_channels` permission
-        to create the channel.
-
-        The ``overwrites`` parameter can be used to create a 'secret'
-        channel upon creation. This parameter expects a :class:`dict` of
-        overwrites with the target (either a :class:`Member` or a :class:`Role`)
-        as the key and a :class:`PermissionOverwrite` as the value.
-
-        .. note::
-
-            Creating a channel of a specified position will not update the position of
-            other channels to follow suit. A follow-up call to :meth:`~TextChannel.edit`
-            will be required to update the position of the channel in the channel list.
-
-        Examples
-        ----------
-
-        Creating a basic channel:
-
-        .. code-block:: python3
-
-            channel = await guild.create_text_channel('cool-channel')
-
-        Creating a "secret" channel:
-
-        .. code-block:: python3
-
-            overwrites = {
-                guild.default_role: discord.PermissionOverwrite(read_messages=False),
-                guild.me: discord.PermissionOverwrite(read_messages=True)
-            }
-
-            channel = await guild.create_text_channel('secret', overwrites=overwrites)
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The channel's name.
-        overwrites
-            A :class:`dict` of target (either a role or a member) to
-            :class:`PermissionOverwrite` to apply upon creation of a channel.
-            Useful for creating secret channels.
-        category: Optional[:class:`CategoryChannel`]
-            The category to place the newly created channel under.
-            The permissions will be automatically synced to category if no
-            overwrites are provided.
-        position: :class:`int`
-            The position in the channel list. This is a number that starts
-            at 0. e.g. the top channel is position 0.
-        topic: Optional[:class:`str`]
-            The new channel's topic.
-        slowmode_delay: :class:`int`
-            Specifies the slowmode rate limit for user in this channel, in seconds.
-            The maximum value possible is `21600`.
-        nsfw: :class:`bool`
-            To mark the channel as NSFW or not.
-        reason: Optional[:class:`str`]
-            The reason for creating this channel. Shows up on the audit log.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to create this channel.
-        HTTPException
-            Creating the channel failed.
-        InvalidArgument
-            The permission overwrite information is not in proper form.
-
-        Returns
-        -------
-        :class:`TextChannel`
-            The channel that was just created.
-        """
-        data = await self._create_channel(name, overwrites, ChannelType.text, category, **options)
-        channel = TextChannel(state=self._state, guild=self, data=data)
-
-        # Temporarily add to the cache
-        self._channels[channel.id] = channel
-        return channel
-
-    async def create_voice_channel(self, name, *, overwrites=None, category=None, **options):
-        """|coro|
-
-        This is similar to :meth:`create_text_channel` except makes a :class:`VoiceChannel` instead, in addition
-        to having the following new parameters.
-
-        Parameters
-        -----------
-        bitrate: :class:`int`
-            The channel's preferred audio bitrate in bits per second.
-        user_limit: :class:`int`
-            The channel's limit for number of members that can be in a voice channel.
-        rtc_region: Optional[:class:`VoiceRegion`]
-            The region for the voice channel's voice communication.
-            A value of ``None`` indicates automatic voice region detection.
-
-            .. versionadded:: 1.7
-
-        Raises
-        ------
-        Forbidden
-            You do not have the proper permissions to create this channel.
-        HTTPException
-            Creating the channel failed.
-        InvalidArgument
-            The permission overwrite information is not in proper form.
-
-        Returns
-        -------
-        :class:`VoiceChannel`
-            The channel that was just created.
-        """
-        data = await self._create_channel(name, overwrites, ChannelType.voice, category, **options)
-        channel = VoiceChannel(state=self._state, guild=self, data=data)
-
-        # temporarily add to the cache
-        self._channels[channel.id] = channel
-        return channel
-
-    async def create_stage_channel(self, name, *, topic=None, category=None, overwrites=None, position=None):
-        """|coro|
-
-        This is similar to :meth:`create_text_channel` except makes a :class:`StageChannel` instead.
-
-        .. note::
-
-            The ``slowmode_delay`` and ``nsfw`` parameters are not supported in this function.
-
-        .. versionadded:: 1.7
-
-        Raises
-        ------
-        Forbidden
-            You do not have the proper permissions to create this channel.
-        HTTPException
-            Creating the channel failed.
-        InvalidArgument
-            The permission overwrite information is not in proper form.
-
-        Returns
-        -------
-        :class:`StageChannel`
-            The channel that was just created.
-        """
-        data = await self._create_channel(name, overwrites, ChannelType.stage_voice, category, position=position, topic=topic)
-        channel = StageChannel(state=self._state, guild=self, data=data)
-
-        # temporarily add to the cache
-        self._channels[channel.id] = channel
-        return channel
-
-    async def create_category(self, name, *, overwrites=None, position=None):
-        """|coro|
-
-        Same as :meth:`create_text_channel` except makes a :class:`CategoryChannel` instead.
-
-        .. note::
-
-            The ``category`` parameter is not supported in this function since categories
-            cannot have categories.
-
-        Raises
-        ------
-        Forbidden
-            You do not have the proper permissions to create this channel.
-        HTTPException
-            Creating the channel failed.
-        InvalidArgument
-            The permission overwrite information is not in proper form.
-
-        Returns
-        -------
-        :class:`CategoryChannel`
-            The channel that was just created.
-        """
-        data = await self._create_channel(name, overwrites, ChannelType.category, position=position)
-        channel = CategoryChannel(state=self._state, guild=self, data=data)
-
-        # temporarily add to the cache
-        self._channels[channel.id] = channel
-        return channel
-
-    create_category_channel = create_category
-
-    async def leave(self):
-        """|coro|
-
-        Leaves the guild.
-
-        .. note::
-
-            You cannot leave a guild that you own, you must delete it instead
-            via :meth:`delete`.
-
-        Raises
-        --------
-        HTTPException
-            Leaving the guild failed.
-        """
-        await self._state.http.leave_guild(self.id)
-
-    async def delete(self):
-        """|coro|
-
-        Deletes the guild. You must be the guild owner to delete the
-        guild.
-
-        Raises
-        --------
-        HTTPException
-            Deleting the guild failed.
-        Forbidden
-            You do not have permissions to delete the guild.
-        """
-
-        await self._state.http.delete_guild(self.id)
-
-    async def edit(self, **fields):
-        """|coro|
-
-        Edits the guild.
-
-        You must have the :attr:`~Permissions.manage_guild` permission
-        to edit the guild.
-
-        .. versionchanged:: 1.4
-            The `rules_channel` and `public_updates_channel` keyword-only parameters were added.
-
-        Parameters
-        ----------
-        name: :class:`str`
-            The new name of the guild.
-        description: :class:`str`
-            The new description of the guild. This is only available to guilds that
-            contain ``COMMUNITY`` in :attr:`Guild.features`.
-        icon: :class:`bytes`
-            A :term:`py:bytes-like object` representing the icon. Only PNG/JPEG is supported.
-            GIF is only available to guilds that contain ``ANIMATED_ICON`` in :attr:`Guild.features`.
-            Could be ``None`` to denote removal of the icon.
-        banner: :class:`bytes`
-            A :term:`py:bytes-like object` representing the banner.
-            Could be ``None`` to denote removal of the banner.
-        splash: :class:`bytes`
-            A :term:`py:bytes-like object` representing the invite splash.
-            Only PNG/JPEG supported. Could be ``None`` to denote removing the
-            splash. This is only available to guilds that contain ``INVITE_SPLASH``
-            in :attr:`Guild.features`.
-        region: :class:`VoiceRegion`
-            The new region for the guild's voice communication.
-        afk_channel: Optional[:class:`VoiceChannel`]
-            The new channel that is the AFK channel. Could be ``None`` for no AFK channel.
-        afk_timeout: :class:`int`
-            The number of seconds until someone is moved to the AFK channel.
-        owner: :class:`Member`
-            The new owner of the guild to transfer ownership to. Note that you must
-            be owner of the guild to do this.
-        verification_level: :class:`VerificationLevel`
-            The new verification level for the guild.
-        default_notifications: :class:`NotificationLevel`
-            The new default notification level for the guild.
-        explicit_content_filter: :class:`ContentFilter`
-            The new explicit content filter for the guild.
-        vanity_code: :class:`str`
-            The new vanity code for the guild.
-        system_channel: Optional[:class:`TextChannel`]
-            The new channel that is used for the system channel. Could be ``None`` for no system channel.
-        system_channel_flags: :class:`SystemChannelFlags`
-            The new system channel settings to use with the new system channel.
-        preferred_locale: :class:`str`
-            The new preferred locale for the guild. Used as the primary language in the guild.
-            If set, this must be an ISO 639 code, e.g. ``en-US`` or ``ja`` or ``zh-CN``.
-        rules_channel: Optional[:class:`TextChannel`]
-            The new channel that is used for rules. This is only available to
-            guilds that contain ``PUBLIC`` in :attr:`Guild.features`. Could be ``None`` for no rules
-            channel.
-        public_updates_channel: Optional[:class:`TextChannel`]
-            The new channel that is used for public updates from Discord. This is only available to
-            guilds that contain ``PUBLIC`` in :attr:`Guild.features`. Could be ``None`` for no
-            public updates channel.
-        features: List[:class:`str`]
-            The guild features. This is used to enable community. Make sure to pass the full list of
-            features (including the ones the guild already has).
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to edit the guild.
-        HTTPException
-            Editing the guild failed.
-        InvalidArgument
-            The image format passed in to ``icon`` is invalid. It must be
-            PNG or JPG. This is also raised if you are not the owner of the
-            guild and request an ownership transfer.
-        """
-
-        http = self._state.http
-
-        try:
-            icon_bytes = fields['icon']
-        except KeyError:
-            icon = self.icon
-        else:
-            if icon_bytes is not None:
-                icon = utils._bytes_to_base64_data(icon_bytes)
-            else:
-                icon = None
-
-        try:
-            banner_bytes = fields['banner']
-        except KeyError:
-            banner = self.banner
-        else:
-            if banner_bytes is not None:
-                banner = utils._bytes_to_base64_data(banner_bytes)
-            else:
-                banner = None
-
-        try:
-            vanity_code = fields['vanity_code']
-        except KeyError:
-            pass
-        else:
-            await http.change_vanity_code(self.id, vanity_code)
-
-        try:
-            splash_bytes = fields['splash']
-        except KeyError:
-            splash = self.splash
-        else:
-            if splash_bytes is not None:
-                splash = utils._bytes_to_base64_data(splash_bytes)
-            else:
-                splash = None
-
-        fields['icon'] = icon
-        fields['banner'] = banner
-        fields['splash'] = splash
-
-        fields['name'] = fields.get('name', self.name)
-        fields['description'] = fields.get('description', self.description)
-        fields['afk_timeout'] = fields.get('afk_timeout', self.afk_timeout)
-        fields['features'] = fields.get('features', self.features)
-
-        try:
-            default_message_notifications = fields.pop('default_notifications')
-        except KeyError:
-            default_message_notifications = self.default_notifications
-        else:
-            if not isinstance(default_message_notifications, NotificationLevel):
-                raise InvalidArgument('default_notifications field must be of type NotificationLevel')
-            fields['default_message_notifications'] = default_message_notifications.value
-
-        try:
-            afk_channel = fields.pop('afk_channel')
-        except KeyError:
-            afk_channel = self.afk_channel
-        else:
-            if afk_channel is None:
-                fields['afk_channel_id'] = afk_channel
-            else:
-                fields['afk_channel_id'] = afk_channel.id
-
-        try:
-            system_channel = fields.pop('system_channel')
-        except KeyError:
-            system_channel = self.system_channel
-        else:
-            if system_channel is None:
-                fields['system_channel_id'] = system_channel
-            else:
-                fields['system_channel_id'] = system_channel.id
-
-        if 'owner' in fields:
-            if self.owner_id != self._state.self_id:
-                raise InvalidArgument('To transfer ownership you must be the owner of the guild.')
-
-            fields['owner_id'] = fields['owner'].id
-
-        if 'region' in fields:
-            fields['region'] = str(fields['region'])
-        else:
-            fields['region'] = str(self.region)
-
-        level = fields.get('verification_level', self.verification_level)
-        if not isinstance(level, VerificationLevel):
-            raise InvalidArgument('verification_level field must be of type VerificationLevel')
-
-        fields['verification_level'] = level.value
-
-        explicit_content_filter = fields.get('explicit_content_filter', self.explicit_content_filter)
-        if not isinstance(explicit_content_filter, ContentFilter):
-            raise InvalidArgument('explicit_content_filter field must be of type ContentFilter')
-
-        fields['explicit_content_filter'] = explicit_content_filter.value
-
-        system_channel_flags = fields.get('system_channel_flags', self.system_channel_flags)
-        if not isinstance(system_channel_flags, SystemChannelFlags):
-            raise InvalidArgument('system_channel_flags field must be of type SystemChannelFlags')
-
-        fields['system_channel_flags'] = system_channel_flags.value
-
-        try:
-            rules_channel = fields.pop('rules_channel')
-        except KeyError:
-            pass
-        else:
-            if rules_channel is None:
-                fields['rules_channel_id'] = rules_channel
-            else:
-                fields['rules_channel_id'] = rules_channel.id
-
-        try:
-            public_updates_channel = fields.pop('public_updates_channel')
-        except KeyError:
-            public_updates_channel = self.public_updates_channel
-        else:
-            if public_updates_channel is None:
-                fields['public_updates_channel_id'] = public_updates_channel
-            else:
-                fields['public_updates_channel_id'] = public_updates_channel.id
-
-        await http.edit_guild(self.id, **fields)
-
-    async def fetch_channels(self):
-        """|coro|
-
-        Retrieves all :class:`abc.GuildChannel` that the guild has.
-
-        .. note::
-
-            This method is an API call. For general usage, consider :attr:`channels` instead.
-
-        .. versionadded:: 1.2
-
-        Raises
-        -------
-        InvalidData
-            An unknown channel type was received from Discord.
-        HTTPException
-            Retrieving the channels failed.
-
-        Returns
-        -------
-        List[:class:`abc.GuildChannel`]
-            All channels in the guild.
-        """
-        data = await self._state.http.get_all_guild_channels(self.id)
-
-        def convert(d):
-            factory, ch_type = _channel_factory(d['type'])
-            if factory is None:
-                raise InvalidData('Unknown channel type {type} for channel ID {id}.'.format_map(d))
-
-            channel = factory(guild=self, state=self._state, data=d)
-            return channel
-
-        return [convert(d) for d in data]
-
-    async def fetch_member(self, member_id):
-        """|coro|
-
-        Retrieves a :class:`Member` from a guild ID, and a member ID.
-
-        .. note::
-
-            This method is an API call. If you have member cache enabled, consider :meth:`get_member` instead.
-
-        Parameters
-        -----------
-        member_id: :class:`int`
-            The member's ID to fetch from.
-
-        Raises
-        -------
-        Forbidden
-            You do not have access to the guild.
-        HTTPException
-            Fetching the member failed.
-
-        Returns
-        --------
-        :class:`Member`
-            The member from the member ID.
-        """
-        data = await self._state.http.get_member(self.id, member_id)
-        return Member(data=data, state=self._state, guild=self)
-
-    async def fetch_ban(self, user):
-        """|coro|
-
-        Retrieves the :class:`BanEntry` for a user.
-
-        You must have the :attr:`~Permissions.ban_members` permission
-        to get this information.
-
-        Parameters
-        -----------
-        user: :class:`abc.Snowflake`
-            The user to get ban information from.
-
-        Raises
-        ------
-        Forbidden
-            You do not have proper permissions to get the information.
-        NotFound
-            This user is not banned.
-        HTTPException
-            An error occurred while fetching the information.
-
-        Returns
-        -------
-        :class:`BanEntry`
-            The :class:`BanEntry` object for the specified user.
-        """
-        data = await self._state.http.get_ban(self.id, user.id)
-        return BanEntry(
-            user=User(state=self._state, data=data['user']),
-            reason=data['reason']
-        )
-
-    async def bans(self):
-        """|coro|
-
-        Retrieves all the users that are banned from the guild as a :class:`list` of :class:`BanEntry`.
-
-        You must have the :attr:`~Permissions.ban_members` permission
-        to get this information.
-
-        Raises
-        -------
-        Forbidden
-            You do not have proper permissions to get the information.
-        HTTPException
-            An error occurred while fetching the information.
-
-        Returns
-        --------
-        List[:class:`BanEntry`]
-            A list of :class:`BanEntry` objects.
-        """
-
-        data = await self._state.http.get_bans(self.id)
-        return [BanEntry(user=User(state=self._state, data=e['user']),
-                         reason=e['reason'])
-                for e in data]
-
-    async def prune_members(self, *, days, compute_prune_count=True, roles=None):
-        r"""|coro|
-
-        Prunes the guild from its inactive members.
-
-        The inactive members are denoted if they have not logged on in
-        ``days`` number of days and they have no roles.
-
-        You must have the :attr:`~Permissions.kick_members` permission
-        to use this.
-
-        To check how many members you would prune without actually pruning,
-        see the :meth:`estimate_pruned_members` function.
-
-        To prune members that have specific roles see the ``roles`` parameter.
-
-        .. versionchanged:: 1.4
-            The ``roles`` keyword-only parameter was added.
-
-        Parameters
-        -----------
-        days: :class:`int`
-            The number of days before counting as inactive.
-        compute_prune_count: :class:`bool`
-            Whether to compute the prune count. This defaults to ``True``
-            which makes it prone to timeouts in very large guilds. In order
-            to prevent timeouts, you must set this to ``False``. If this is
-            set to ``False``\, then this function will always return ``None``.
-        roles: Optional[List[:class:`abc.Snowflake`]]
-            A list of :class:`abc.Snowflake` that represent roles to include in the pruning process. If a member
-            has a role that is not specified, they'll be excluded.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to prune members.
-        HTTPException
-            An error occurred while pruning members.
-        InvalidArgument
-            An integer was not passed for ``days``.
-
-        Returns
-        ---------
-        Optional[:class:`int`]
-            The number of members pruned. If ``compute_prune_count`` is ``False``
-            then this returns ``None``.
-        """
-
-        if not isinstance(days, int):
-            raise InvalidArgument('Expected int for ``days``, received {0.__class__.__name__} instead.'.format(days))
-
-        if roles:
-            roles = [str(role.id) for role in roles]
-
-        data = await self._state.http.prune_members(self.id, days, compute_prune_count=compute_prune_count, roles=roles)
-        return data['pruned']
-
-    async def templates(self):
-        """|coro|
-
-        Gets the list of templates from this guild.
-
-        Requires :attr:`~.Permissions.manage_guild` permissions.
-
-        .. versionadded:: 1.7
-
-        Raises
-        -------
-        Forbidden
-            You don't have permissions to get the templates.
-
-        Returns
-        --------
-        List[:class:`Template`]
-            The templates for this guild.
-        """
-        from .template import Template
-        data = await self._state.http.guild_templates(self.id)
-        return [Template(data=d, state=self._state) for d in data]
-
-    async def webhooks(self):
-        """|coro|
-
-        Gets the list of webhooks from this guild.
-
-        Requires :attr:`~.Permissions.manage_webhooks` permissions.
-
-        Raises
-        -------
-        Forbidden
-            You don't have permissions to get the webhooks.
-
-        Returns
-        --------
-        List[:class:`Webhook`]
-            The webhooks for this guild.
-        """
-
-        from .webhook import Webhook
-        data = await self._state.http.guild_webhooks(self.id)
-        return [Webhook.from_state(d, state=self._state) for d in data]
-
-    async def estimate_pruned_members(self, *, days, roles=None):
-        """|coro|
-
-        Similar to :meth:`prune_members` except instead of actually
-        pruning members, it returns how many members it would prune
-        from the guild had it been called.
-
-        Parameters
-        -----------
-        days: :class:`int`
-            The number of days before counting as inactive.
-        roles: Optional[List[:class:`abc.Snowflake`]]
-            A list of :class:`abc.Snowflake` that represent roles to include in the estimate. If a member
-            has a role that is not specified, they'll be excluded.
-
-            .. versionadded:: 1.7
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to prune members.
-        HTTPException
-            An error occurred while fetching the prune members estimate.
-        InvalidArgument
-            An integer was not passed for ``days``.
-
-        Returns
-        ---------
-        :class:`int`
-            The number of members estimated to be pruned.
-        """
-
-        if not isinstance(days, int):
-            raise InvalidArgument('Expected int for ``days``, received {0.__class__.__name__} instead.'.format(days))
-
-        if roles:
-            roles = [str(role.id) for role in roles]
-
-        data = await self._state.http.estimate_pruned_members(self.id, days, roles)
-        return data['pruned']
-
-    async def invites(self):
-        """|coro|
-
-        Returns a list of all active instant invites from the guild.
-
-        You must have the :attr:`~Permissions.manage_guild` permission to get
-        this information.
-
-        Raises
-        -------
-        Forbidden
-            You do not have proper permissions to get the information.
-        HTTPException
-            An error occurred while fetching the information.
-
-        Returns
-        -------
-        List[:class:`Invite`]
-            The list of invites that are currently active.
-        """
-
-        data = await self._state.http.invites_from(self.id)
-        result = []
-        for invite in data:
-            channel = self.get_channel(int(invite['channel']['id']))
-            invite['channel'] = channel
-            invite['guild'] = self
-            result.append(Invite(state=self._state, data=invite))
-
-        return result
-
-    async def create_template(self, *, name, description=None):
-        """|coro|
-
-        Creates a template for the guild.
-
-        You must have the :attr:`~Permissions.manage_guild` permission to
-        do this.
-
-        .. versionadded:: 1.7
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The name of the template.
-        description: Optional[:class:`str`]
-            The description of the template.
-        """
-        from .template import Template
-
-        payload = {
-            'name': name
-        }
-
-        if description:
-            payload['description'] = description
-
-        data = await self._state.http.create_template(self.id, payload)
-
-        return Template(state=self._state, data=data)
-
-    async def create_integration(self, *, type, id):
-        """|coro|
-
-        Attaches an integration to the guild.
-
-        You must have the :attr:`~Permissions.manage_guild` permission to
-        do this.
-
-        .. versionadded:: 1.4
-
-        Parameters
-        -----------
-        type: :class:`str`
-            The integration type (e.g. Twitch).
-        id: :class:`int`
-            The integration ID.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permission to create the integration.
-        HTTPException
-            The account could not be found.
-        """
-        await self._state.http.create_integration(self.id, type, id)
-
-    async def integrations(self, *, with_applications):
-        """|coro|
-
-        Returns a list of all integrations attached to the guild.
-
-        You must have the :attr:`~Permissions.manage_guild` permission to
-        do this.
-
-        .. versionadded:: 1.4
-
-        Parameters
-        -----------
-        with_applications: :class:`bool`
-            Whether to include applications.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permission to create the integration.
-        HTTPException
-            Fetching the integrations failed.
-
-        Returns
-        --------
-        List[:class:`Integration`]
-            The list of integrations that are attached to the guild.
-        """
-        data = await self._state.http.get_all_integrations(self.id, with_applications=with_applications)
-        return [Integration(guild=self, data=d) for d in data]
-
-    fetch_integrations = integrations
-
-    async def fetch_emojis(self):
-        r"""|coro|
-
-        Retrieves all custom :class:`Emoji`\s from the guild.
-
-        .. note::
-
-            This method is an API call. For general usage, consider :attr:`emojis` instead.
-
-        Raises
-        ---------
-        HTTPException
-            An error occurred fetching the emojis.
-
-        Returns
-        --------
-        List[:class:`Emoji`]
-            The retrieved emojis.
-        """
-        data = await self._state.http.get_all_custom_emojis(self.id)
-        return [Emoji(guild=self, state=self._state, data=d) for d in data]
-
-    async def fetch_emoji(self, emoji_id):
-        """|coro|
-
-        Retrieves a custom :class:`Emoji` from the guild.
-
-        .. note::
-
-            This method is an API call.
-            For general usage, consider iterating over :attr:`emojis` instead.
-
-        Parameters
-        -------------
-        emoji_id: :class:`int`
-            The emoji's ID.
-
-        Raises
-        ---------
-        NotFound
-            The emoji requested could not be found.
-        HTTPException
-            An error occurred fetching the emoji.
-
-        Returns
-        --------
-        :class:`Emoji`
-            The retrieved emoji.
-        """
-        data = await self._state.http.get_custom_emoji(self.id, emoji_id)
-        return Emoji(guild=self, state=self._state, data=data)
-
-    async def create_custom_emoji(self, *, name, image):
-        r"""|coro|
-
-        Creates a custom :class:`Emoji` for the guild.
-
-        There is currently a limit of 50 static and animated emojis respectively per guild,
-        unless the guild has the ``MORE_EMOJI`` feature which extends the limit to 200.
-
-        You must have the :attr:`~Permissions.manage_emojis` permission to
-        do this.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The emoji name. Must be at least 2 characters.
-        image: :class:`bytes`
-            The :term:`py:bytes-like object` representing the image data to use.
-            Only JPG, PNG and GIF images are supported.
-
-        Raises
-        -------
-        Forbidden
-            You are not allowed to create emojis.
-        HTTPException
-            An error occurred creating an emoji.
-
-        Returns
-        --------
-        :class:`Emoji`
-            The created emoji.
-        """
-
-        img = utils._bytes_to_base64_data(image)
-        data = await self._state.http.create_custom_emoji(self.id, name, img)
-        return self._state.store_emoji(self, data)
-
-    async def fetch_roles(self):
-        """|coro|
-
-        Retrieves all :class:`Role` that the guild has.
-
-        .. note::
-
-            This method is an API call. For general usage, consider :attr:`roles` instead.
-
-        .. versionadded:: 1.3
-
-        Raises
-        -------
-        HTTPException
-            Retrieving the roles failed.
-
-        Returns
-        -------
-        List[:class:`Role`]
-            All roles in the guild.
-        """
-
-        data = await self._state.http.get_roles(self.id)
-        return [Role(guild=self, state=self._state, data=d) for d in data]
-
-    async def create_role(self, **fields):
-        """|coro|
-
-        Creates a :class:`Role` for the guild.
-
-        All fields are optional.
-
-        You must have the :attr:`~Permissions.manage_roles` permission to
-        do this.
-
-        .. versionchanged:: 1.6
-            Can now pass ``int`` to ``colour`` keyword-only parameter.
-
-        Parameters
-        -----------
-        name: :class:`str`
-            The role name. Defaults to 'new role'.
-        permissions: :class:`Permissions`
-            The permissions to have. Defaults to no permissions.
-        colour: Union[:class:`Colour`, :class:`int`]
-            The colour for the role. Defaults to :meth:`Colour.default`.
-            This is aliased to ``color`` as well.
-        hoist: :class:`bool`
-            Indicates if the role should be shown separately in the member list.
-            Defaults to ``False``.
-        mentionable: :class:`bool`
-            Indicates if the role should be mentionable by others.
-            Defaults to ``False``.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to create the role.
-        HTTPException
-            Creating the role failed.
-        InvalidArgument
-            An invalid keyword argument was given.
-
-        Returns
-        --------
-        :class:`Role`
-            The newly created role.
-        """
-
-        try:
-            perms = fields.pop('permissions')
-        except KeyError:
-            fields['permissions'] = 0
-        else:
-            fields['permissions'] = perms.value
-
-        try:
-            colour = fields.pop('colour')
-        except KeyError:
-            colour = fields.get('color', Colour.default())
-        finally:
-            if isinstance(colour, int):
-                colour = Colour(value=colour)
-            fields['color'] = colour.value
-
-        valid_keys = ('name', 'permissions', 'color', 'hoist', 'mentionable')
-        for key in fields:
-            if key not in valid_keys:
-                raise InvalidArgument('%r is not a valid field.' % key)
-
-        data = await self._state.http.create_role(self.id, **fields)
-        role = Role(guild=self, data=data, state=self._state)
-
-        # TODO: add to cache
-        return role
-
-    async def edit_role_positions(self, positions):
-        """|coro|
-
-        Bulk edits a list of :class:`Role` in the guild.
-
-        You must have the :attr:`~Permissions.manage_roles` permission to
-        do this.
-
-        .. versionadded:: 1.4
-
-        Example:
-
-        .. code-block:: python3
-
-            positions = {
-                bots_role: 1, # penultimate role
-                tester_role: 2,
-                admin_role: 6
-            }
-
-            await guild.edit_role_positions(positions=positions)
-
-        Parameters
-        -----------
-        positions
-            A :class:`dict` of :class:`Role` to :class:`int` to change the positions
-            of each given role.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to move the roles.
-        HTTPException
-            Moving the roles failed.
-        InvalidArgument
-            An invalid keyword argument was given.
-
-        Returns
-        --------
-        List[:class:`Role`]
-            A list of all the roles in the guild.
-        """
-        if not isinstance(positions, dict):
-            raise InvalidArgument('positions parameter expects a dict.')
-
-        role_positions = []
-        for role, position in positions.items():
-
-            payload = {
-                'id': role.id,
-                'position': position
-            }
-
-            role_positions.append(payload)
-
-        data = await self._state.http.move_role_position(self.id, role_positions)
-        roles = []
-        for d in data:
-            role = Role(guild=self, data=d, state=self._state)
-            roles.append(role)
-            self._roles[role.id] = role
-
-        return roles
-
-    async def kick(self, user, *, reason=None):
-        """|coro|
-
-        Kicks a user from the guild.
-
-        The user must meet the :class:`abc.Snowflake` abc.
-
-        You must have the :attr:`~Permissions.kick_members` permission to
-        do this.
-
-        Parameters
-        -----------
-        user: :class:`abc.Snowflake`
-            The user to kick from their guild.
-        reason: Optional[:class:`str`]
-            The reason the user got kicked.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to kick.
-        HTTPException
-            Kicking failed.
-        """
-        await self._state.http.kick(self.id, user.id, reason=reason)
-
-    async def ban(self, user, *, reason=None, delete_message_days=1):
-        """|coro|
-
-        Bans a user from the guild.
-
-        The user must meet the :class:`abc.Snowflake` abc.
-
-        You must have the :attr:`~Permissions.ban_members` permission to
-        do this.
-
-        Parameters
-        -----------
-        user: :class:`abc.Snowflake`
-            The user to ban from their guild.
-        delete_message_days: :class:`int`
-            The number of days worth of messages to delete from the user
-            in the guild. The minimum is 0 and the maximum is 7.
-        reason: Optional[:class:`str`]
-            The reason the user got banned.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to ban.
-        HTTPException
-            Banning failed.
-        """
-        await self._state.http.ban(self.id, user.id, delete_message_days, reason=reason)
-
-    async def unban(self, user):
-        """|coro|
-
-        Unbans a user from the guild.
-
-        The user must meet the :class:`abc.Snowflake` abc.
-
-        You must have the :attr:`~Permissions.ban_members` permission to
-        do this.
-
-        Parameters
-        -----------
-        user: :class:`abc.Snowflake`
-            The user to unban.
-        reason: Optional[:class:`str`]
-            The reason for doing this action. Shows up on the audit log.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to unban.
-        HTTPException
-            Unbanning failed.
-        """
-        await self._state.http.unban(self.id, user.id)
-
-    async def vanity_invite(self):
-        """|coro|
-
-        Returns the guild's special vanity invite.
-
-        The guild must have ``VANITY_URL`` in :attr:`~Guild.features`.
-
-        You must have the :attr:`~Permissions.manage_guild` permission to use
-        this as well.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to get this.
-        HTTPException
-            Retrieving the vanity invite failed.
-
-        Returns
-        --------
-        :class:`Invite`
-            The special vanity invite.
-        """
-
-        state = self._state
-
-        # we start with { code: abc }
-        payload = await state.http.get_vanity_code(self.id)
-
-        # get the vanity URL channel since default channels aren't
-        # reliable or a thing anymore
-        data = await state.http.get_invite(payload['code'])
-
-        payload['guild'] = self
-        payload['channel'] = self.get_channel(int(data['channel']['id']))
-        payload['revoked'] = False
-        payload['temporary'] = False
-        payload['max_uses'] = 0
-        payload['max_age'] = 0
-        return Invite(state=state, data=payload)
-
-    def ack(self):
-        """|coro|
-
-        Marks every message in this guild as read.
-
-        Raises
-        -------
-        HTTPException
-            Acking failed.
-        """
-
-        return self._state.http.ack_guild(self.id)
-
-    def audit_logs(self, *, limit=100, before=None, after=None, oldest_first=None, user=None, action=None):
-        """Returns an :class:`AsyncIterator` that enables receiving the guild's audit logs.
-
-        You must have the :attr:`~Permissions.view_audit_log` permission to use this.
-
-        Examples
-        ----------
-
-        Getting the first 100 entries: ::
-
-            async for entry in guild.audit_logs(limit=100):
-                print('{0.user} did {0.action} to {0.target}'.format(entry))
-
-        Getting entries for a specific action: ::
-
-            async for entry in guild.audit_logs(action=discord.AuditLogAction.ban):
-                print('{0.user} banned {0.target}'.format(entry))
-
-        Getting entries made by a specific user: ::
-
-            entries = await guild.audit_logs(limit=None, user=guild.me).flatten()
-            await channel.send('I made {} moderation actions.'.format(len(entries)))
-
-        Parameters
-        -----------
-        limit: Optional[:class:`int`]
-            The number of entries to retrieve. If ``None`` retrieve all entries.
-        before: Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]
-            Retrieve entries before this date or entry.
-            If a date is provided it must be a timezone-naive datetime representing UTC time.
-        after: Union[:class:`abc.Snowflake`, :class:`datetime.datetime`]
-            Retrieve entries after this date or entry.
-            If a date is provided it must be a timezone-naive datetime representing UTC time.
-        oldest_first: :class:`bool`
-            If set to ``True``, return entries in oldest->newest order. Defaults to ``True`` if
-            ``after`` is specified, otherwise ``False``.
-        user: :class:`abc.Snowflake`
-            The moderator to filter entries from.
-        action: :class:`AuditLogAction`
-            The action to filter with.
-
-        Raises
-        -------
-        Forbidden
-            You are not allowed to fetch audit logs
-        HTTPException
-            An error occurred while fetching the audit logs.
-
-        Yields
-        --------
-        :class:`AuditLogEntry`
-            The audit log entry.
-        """
-        if user:
-            user = user.id
-
-        if action:
-            action = action.value
-
-        return AuditLogIterator(self, before=before, after=after, limit=limit,
-                                oldest_first=oldest_first, user_id=user, action_type=action)
-
-    async def widget(self):
-        """|coro|
-
-        Returns the widget of the guild.
-
-        .. note::
-
-            The guild must have the widget enabled to get this information.
-
-        Raises
-        -------
-        Forbidden
-            The widget for this guild is disabled.
-        HTTPException
-            Retrieving the widget failed.
-
-        Returns
-        --------
-        :class:`Widget`
-            The guild's widget.
-        """
-        data = await self._state.http.get_widget(self.id)
-
-        return Widget(state=self._state, data=data)
-
-    async def chunk(self, *, cache=True):
-        """|coro|
-
-        Requests all members that belong to this guild. In order to use this,
-        you must have :attr:`Permission.manage_guild`.
-
-        This is a websocket operation and can be slow.
-
-        .. versionadded:: 1.5
-
-        Parameters
-        -----------
-        cache: :class:`bool`
-            Whether to cache the members as well.
-
-        Raises
-        -------
-        ClientException
-            You do not have :attr:`Permission.manage_guild`.
-        """
-
-        if not self.me.guild_permissions.manage_guild:
-            raise ClientException('`manage_guild` permission is required to use this.')
-
-        if not self._state.is_guild_evicted(self):
-            return await self._state.chunk_guild(self, cache=cache)
-
-    async def query_members(self, query=None, *, limit=5, user_ids=None, presences=True, cache=True):
-        """|coro|
-
-        Request members that belong to this guild whose username starts with
-        the query given.
-
-        This is a websocket operation and can be slow.
-
-        .. versionadded:: 1.3
-
-        Parameters
-        -----------
-        query: Optional[:class:`str`]
-            The string that the username's start with.
-        limit: :class:`int`
-            The maximum number of members to send back. This must be
-            a number between 5 and 100.
-        presences: :class:`bool`
-            Whether to request for presences to be provided. This defaults
-            to ``False``.
-
-            .. versionadded:: 1.6
-
-        cache: :class:`bool`
-            Whether to cache the members internally. This makes operations
-            such as :meth:`get_member` work for those that matched.
-        user_ids: Optional[List[:class:`int`]]
-            List of user IDs to search for. If the user ID is not in the guild then it won't be returned.
-
-            .. versionadded:: 1.4
-
-
-        Raises
-        -------
-        asyncio.TimeoutError
-            The query timed out waiting for the members.
-        ValueError
-            Invalid parameters were passed to the function
-
-        Returns
-        --------
-        List[:class:`Member`]
-            The list of members that have matched the query.
-        """
-
-        if not query and not user_ids:
-            raise ValueError('Must pass either query or user_ids')
-
-        if user_ids and query:
-            raise ValueError('Cannot pass both query and user_ids')
-
-        limit = min(100, limit or 5) if query else None
-        return await self._state.query_members(self, query=query, limit=limit, user_ids=user_ids, presences=presences, cache=cache)
-
-    async def change_voice_state(self, *, channel, self_mute=False, self_deaf=False, self_video=None, self_stream=None, preferred_region=''):
-        """|coro|
-
-        Changes client's voice state in the guild.
-
-        .. versionadded:: 1.4
-
-        Parameters
-        -----------
-        channel: Optional[:class:`VoiceChannel`]
-            Channel the client wants to join. Use ``None`` to disconnect.
-        self_mute: :class:`bool`
-            Indicates if the client should be self-muted.
-        self_deaf: :class:`bool`
-            Indicates if the client should be self-deafened.
-        self_video :class:`bool`
-            Indicates if the client is using video. Untested & unconfirmed
-            (do not use).
-
-            .. versionadded:: 1.9
-        self_stream :class:`bool`
-            Indicates if the client is sharing its screen via the Go Live
-            feature. Untested & unconfirmed (do not use).
-
-            .. versionadded:: 1.9
-        """
-
-        state = self._state
-        ws = state._get_websocket()
-        channel_id = channel.id if channel else None
-
-        if channel_id and preferred_region == '':
-            preferred_region = state.preferred_region
-
-        await ws.voice_state(self.id, channel_id, self_mute, self_deaf, self_video, self_stream, preferred_region=str(preferred_region))
-
-    async def mute(self, *, duration=None):
-        """|coro|
-
-        Mutes the guild.
-
-        .. versionadded:: 1.9
-
-        Parameters
-        -----------
-        duration: Optional[:class:`int`]
-            The duration (in hours) of the mute. Defaults to
-            ``None`` for an indefinite mute.
-
-        Raises
-        -------
-        HTTPException
-            Muting failed.
-        """
-
-        fields = {
-            'muted': True
-        }
-
-        if duration is not None:
-            mute_config = {
-                'selected_time_window': duration * 3600,
-                'end_time': (datetime.utcnow() + timedelta(hours=duration)).isoformat()
-            }
-            fields['mute_config'] = mute_config
-
-        await self._state.http.edit_guild_settings(self.id, **fields)
-
-    async def unmute(self):
-        """|coro|
-
-        Unmutes the guild.
-
-        .. versionadded:: 1.9
-
-        Raises
-        -------
-        HTTPException
-            Unmuting failed.
-        """
-
-        await self._state.http.edit_guild_settings(self.id, muted=False)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import copy
+import asyncio
+from datetime import datetime
+from typing import (
+    Any,
+    AsyncIterator,
+    Callable,
+    Collection,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    TYPE_CHECKING,
+    Protocol,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    overload,
+    runtime_checkable,
+)
+
+from .object import OLDEST_OBJECT, Object
+from .context_managers import Typing
+from .enums import AppCommandType, ChannelType
+from .errors import ClientException
+from .mentions import AllowedMentions
+from .permissions import PermissionOverwrite, Permissions
+from .role import Role
+from .invite import Invite
+from .file import File
+from .http import handle_message_parameters
+from .voice_client import VoiceClient, VoiceProtocol
+from .sticker import GuildSticker, StickerItem
+from .settings import ChannelSettings
+from .commands import ApplicationCommand, BaseCommand, SlashCommand, UserCommand, MessageCommand, _command_factory
+from . import utils
+
+__all__ = (
+    'Snowflake',
+    'User',
+    'PrivateChannel',
+    'GuildChannel',
+    'Messageable',
+    'Connectable',
+    'ApplicationCommand',
+)
+
+T = TypeVar('T', bound=VoiceProtocol)
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+    from .client import Client
+    from .user import ClientUser, User
+    from .asset import Asset
+    from .state import ConnectionState
+    from .guild import Guild
+    from .member import Member
+    from .message import Message, MessageReference, PartialMessage
+    from .channel import (
+        TextChannel,
+        DMChannel,
+        GroupChannel,
+        PartialMessageable,
+        VocalGuildChannel,
+        VoiceChannel,
+        StageChannel,
+        CategoryChannel,
+    )
+    from .threads import Thread
+    from .enums import InviteTarget
+    from .types.channel import (
+        PermissionOverwrite as PermissionOverwritePayload,
+        Channel as ChannelPayload,
+        GuildChannel as GuildChannelPayload,
+        OverwriteType,
+    )
+    from .types.snowflake import (
+        SnowflakeList,
+    )
+
+    MessageableChannel = Union[TextChannel, VoiceChannel, StageChannel, Thread, DMChannel, PartialMessageable, GroupChannel]
+    VocalChannel = Union[VoiceChannel, StageChannel, DMChannel, GroupChannel]
+    SnowflakeTime = Union["Snowflake", datetime]
+
+MISSING = utils.MISSING
+
+
+class _Undefined:
+    def __repr__(self) -> str:
+        return 'see-below'
+
+
+_undefined: Any = _Undefined()
+
+
+async def _purge_helper(
+    channel: Union[Thread, TextChannel, VocalGuildChannel],
+    *,
+    limit: Optional[int] = 100,
+    check: Callable[[Message], bool] = MISSING,
+    before: Optional[SnowflakeTime] = None,
+    after: Optional[SnowflakeTime] = None,
+    around: Optional[SnowflakeTime] = None,
+    oldest_first: Optional[bool] = None,
+    reason: Optional[str] = None,
+) -> List[Message]:
+    if check is MISSING:
+        check = lambda m: True
+
+    state = channel._state
+    channel_id = channel.id
+    iterator = channel.history(limit=limit, before=before, after=after, oldest_first=oldest_first, around=around)
+    ret: List[Message] = []
+    count = 0
+
+    async for message in iterator:
+        if count == 50:
+            to_delete = ret[-50:]
+            await state._delete_messages(channel_id, to_delete, reason=reason)
+            count = 0
+        if not check(message):
+            continue
+
+        count += 1
+        ret.append(message)
+
+    # Some messages remaining to poll
+    to_delete = ret[-count:]
+    await state._delete_messages(channel_id, to_delete, reason=reason)
+    return ret
+
+
+@overload
+def _handle_commands(
+    messageable: Messageable,
+    type: Literal[AppCommandType.chat_input],
+    *,
+    query: Optional[str] = ...,
+    limit: Optional[int] = ...,
+    command_ids: Optional[Collection[int]] = ...,
+    application: Optional[Snowflake] = ...,
+    with_applications: bool = ...,
+    target: Optional[Snowflake] = ...,
+) -> AsyncIterator[SlashCommand]:
+    ...
+
+
+@overload
+def _handle_commands(
+    messageable: Messageable,
+    type: Literal[AppCommandType.user],
+    *,
+    query: Optional[str] = ...,
+    limit: Optional[int] = ...,
+    command_ids: Optional[Collection[int]] = ...,
+    application: Optional[Snowflake] = ...,
+    with_applications: bool = ...,
+    target: Optional[Snowflake] = ...,
+) -> AsyncIterator[UserCommand]:
+    ...
+
+
+@overload
+def _handle_commands(
+    messageable: Message,
+    type: Literal[AppCommandType.message],
+    *,
+    query: Optional[str] = ...,
+    limit: Optional[int] = ...,
+    command_ids: Optional[Collection[int]] = ...,
+    application: Optional[Snowflake] = ...,
+    with_applications: bool = ...,
+    target: Optional[Snowflake] = ...,
+) -> AsyncIterator[MessageCommand]:
+    ...
+
+
+async def _handle_commands(
+    messageable: Union[Messageable, Message],
+    type: AppCommandType,
+    *,
+    query: Optional[str] = None,
+    limit: Optional[int] = None,
+    command_ids: Optional[Collection[int]] = None,
+    application: Optional[Snowflake] = None,
+    with_applications: bool = True,
+    target: Optional[Snowflake] = None,
+) -> AsyncIterator[BaseCommand]:
+    if limit is not None and limit < 0:
+        raise ValueError('limit must be greater than or equal to 0')
+    if query and command_ids:
+        raise TypeError('Cannot specify both query and command_ids')
+
+    state = messageable._state
+    endpoint = state.http.search_application_commands
+    channel = await messageable._get_channel()
+    _, cls = _command_factory(type.value)
+    cmd_ids = list(command_ids) if command_ids else None
+
+    application_id = application.id if application else None
+    if channel.type == ChannelType.private:
+        recipient: User = channel.recipient  # type: ignore
+        if not recipient.bot:
+            raise TypeError('Cannot fetch commands in a DM with a non-bot user')
+        application_id = recipient.id
+        target = recipient
+    elif channel.type == ChannelType.group:
+        return
+
+    prev_cursor = MISSING
+    cursor = MISSING
+    while True:
+        # We keep two cursors because Discord just sends us an infinite loop sometimes
+        retrieve = min((25 if not cmd_ids else 0) if limit is None else limit, 25)
+
+        if not application_id and limit is not None:
+            limit -= retrieve
+        if (not cmd_ids and retrieve < 1) or cursor is None or (prev_cursor is not MISSING and prev_cursor == cursor):
+            return
+
+        data = await endpoint(
+            channel.id,
+            type.value,
+            limit=retrieve if not application_id else None,
+            query=query if not cmd_ids and not application_id else None,
+            command_ids=cmd_ids if not application_id and not cursor else None,  # type: ignore
+            application_id=application_id,
+            include_applications=with_applications if (not application_id or with_applications) else None,
+            cursor=cursor,
+        )
+        prev_cursor = cursor
+        cursor = data['cursor'].get('next')
+        cmds = data['application_commands']
+        apps: Dict[int, dict] = {int(app['id']): app for app in data.get('applications') or []}
+
+        for cmd in cmds:
+            # Handle faked parameters
+            if application_id and query and query.lower() not in cmd['name']:
+                continue
+            elif application_id and (not cmd_ids or int(cmd['id']) not in cmd_ids) and limit == 0:
+                continue
+
+            # We follow Discord behavior
+            if application_id and limit is not None and (not cmd_ids or int(cmd['id']) not in cmd_ids):
+                limit -= 1
+
+            try:
+                cmd_ids.remove(int(cmd['id'])) if cmd_ids else None
+            except ValueError:
+                pass
+
+            cmd['application'] = apps.get(int(cmd['application_id']))
+            yield cls(state=state, data=cmd, channel=channel, target=target)
+
+        cmd_ids = None
+        if application_id or len(cmds) < min(limit if limit else 25, 25) or len(cmds) == limit == 25:
+            return
+
+
+@runtime_checkable
+class Snowflake(Protocol):
+    """An ABC that details the common operations on a Discord model.
+
+    Almost all :ref:`Discord models <discord_api_models>` meet this
+    abstract base class.
+
+    If you want to create a snowflake on your own, consider using
+    :class:`.Object`.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The model's unique ID.
+    """
+
+    id: int
+
+
+@runtime_checkable
+class User(Snowflake, Protocol):
+    """An ABC that details the common operations on a Discord user.
+
+    The following implement this ABC:
+
+    - :class:`~discord.User`
+    - :class:`~discord.ClientUser`
+    - :class:`~discord.Member`
+
+    This ABC must also implement :class:`~discord.abc.Snowflake`.
+
+    Attributes
+    -----------
+    name: :class:`str`
+        The user's username.
+    discriminator: :class:`str`
+        The user's discriminator.
+    bot: :class:`bool`
+        If the user is a bot account.
+    system: :class:`bool`
+        If the user is a system account.
+    """
+
+    name: str
+    discriminator: str
+    bot: bool
+    system: bool
+
+    @property
+    def display_name(self) -> str:
+        """:class:`str`: Returns the user's display name."""
+        raise NotImplementedError
+
+    @property
+    def mention(self) -> str:
+        """:class:`str`: Returns a string that allows you to mention the given user."""
+        raise NotImplementedError
+
+    @property
+    def avatar(self) -> Optional[Asset]:
+        """Optional[:class:`~discord.Asset`]: Returns an Asset that represents the user's avatar, if present."""
+        raise NotImplementedError
+
+    @property
+    def avatar_decoration(self) -> Optional[Asset]:
+        """Optional[:class:`~discord.Asset`]: Returns an Asset that represents the user's avatar decoration, if present.
+
+        .. versionadded:: 2.0
+        """
+        raise NotImplementedError
+
+    @property
+    def default_avatar(self) -> Asset:
+        """:class:`~discord.Asset`: Returns the default avatar for a given user. This is calculated by the user's discriminator."""
+        raise NotImplementedError
+
+    @property
+    def display_avatar(self) -> Asset:
+        """:class:`~discord.Asset`: Returns the user's display avatar.
+
+        For regular users this is just their default avatar or uploaded avatar.
+
+        .. versionadded:: 2.0
+        """
+        raise NotImplementedError
+
+    def mentioned_in(self, message: Message) -> bool:
+        """Checks if the user is mentioned in the specified message.
+
+        Parameters
+        -----------
+        message: :class:`~discord.Message`
+            The message to check if you're mentioned in.
+
+        Returns
+        -------
+        :class:`bool`
+            Indicates if the user is mentioned in the message.
+        """
+        raise NotImplementedError
+
+
+class PrivateChannel:
+    """An ABC that details the common operations on a private Discord channel.
+
+    The following implement this ABC:
+
+    - :class:`~discord.DMChannel`
+    - :class:`~discord.GroupChannel`
+
+    This ABC must also implement :class:`~discord.abc.Snowflake`.
+
+    Attributes
+    -----------
+    me: :class:`~discord.ClientUser`
+        The user presenting yourself.
+    """
+
+    __slots__ = ()
+
+    id: int
+    me: ClientUser
+
+    def _add_call(self, **kwargs):
+        raise NotImplementedError
+
+    def _update(self, *args) -> None:
+        raise NotImplementedError
+
+
+class _Overwrites:
+    __slots__ = ('id', 'allow', 'deny', 'type')
+
+    ROLE = 0
+    MEMBER = 1
+
+    def __init__(self, data: PermissionOverwritePayload):
+        self.id: int = int(data['id'])
+        self.allow: int = int(data.get('allow', 0))
+        self.deny: int = int(data.get('deny', 0))
+        self.type: OverwriteType = data['type']
+
+    def _asdict(self) -> PermissionOverwritePayload:
+        return {
+            'id': self.id,
+            'allow': str(self.allow),
+            'deny': str(self.deny),
+            'type': self.type,
+        }
+
+    def is_role(self) -> bool:
+        return self.type == 0
+
+    def is_member(self) -> bool:
+        return self.type == 1
+
+
+class GuildChannel:
+    """An ABC that details the common operations on a Discord guild channel.
+
+    The following implement this ABC:
+
+    - :class:`~discord.TextChannel`
+    - :class:`~discord.VoiceChannel`
+    - :class:`~discord.CategoryChannel`
+    - :class:`~discord.StageChannel`
+    - :class:`~discord.ForumChannel`
+
+    This ABC must also implement :class:`~discord.abc.Snowflake`.
+
+    Attributes
+    -----------
+    name: :class:`str`
+        The channel name.
+    guild: :class:`~discord.Guild`
+        The guild the channel belongs to.
+    position: :class:`int`
+        The position in the channel list. This is a number that starts at 0.
+        e.g. the top channel is position 0.
+    """
+
+    __slots__ = ()
+
+    id: int
+    name: str
+    guild: Guild
+    type: ChannelType
+    position: int
+    category_id: Optional[int]
+    _state: ConnectionState
+    _overwrites: List[_Overwrites]
+
+    if TYPE_CHECKING:
+
+        def __init__(self, *, state: ConnectionState, guild: Guild, data: GuildChannelPayload):
+            ...
+
+    def __str__(self) -> str:
+        return self.name
+
+    @property
+    def _sorting_bucket(self) -> int:
+        raise NotImplementedError
+
+    def _update(self, guild: Guild, data: Dict[str, Any]) -> None:
+        raise NotImplementedError
+
+    async def _move(
+        self,
+        position: int,
+        parent_id: Optional[Any] = None,
+        lock_permissions: bool = False,
+        *,
+        reason: Optional[str],
+    ) -> None:
+        if position < 0:
+            raise ValueError('Channel position cannot be less than 0.')
+
+        http = self._state.http
+        bucket = self._sorting_bucket
+        channels: List[GuildChannel] = [c for c in self.guild.channels if c._sorting_bucket == bucket]
+
+        channels.sort(key=lambda c: c.position)
+
+        try:
+            # remove ourselves from the channel list
+            channels.remove(self)
+        except ValueError:
+            # not there somehow lol
+            return
+        else:
+            index = next((i for i, c in enumerate(channels) if c.position >= position), len(channels))
+            # add ourselves at our designated position
+            channels.insert(index, self)
+
+        payload = []
+        for index, c in enumerate(channels):
+            d: Dict[str, Any] = {'id': c.id, 'position': index}
+            if parent_id is not _undefined and c.id == self.id:
+                d.update(parent_id=parent_id, lock_permissions=lock_permissions)
+            payload.append(d)
+
+        await http.bulk_channel_update(self.guild.id, payload, reason=reason)
+
+    async def _edit(self, options: Dict[str, Any], reason: Optional[str]) -> Optional[ChannelPayload]:
+        try:
+            parent = options.pop('category')
+        except KeyError:
+            parent_id = _undefined
+        else:
+            parent_id = parent and parent.id
+
+        try:
+            options['rate_limit_per_user'] = options.pop('slowmode_delay')
+        except KeyError:
+            pass
+
+        try:
+            options['default_thread_rate_limit_per_user'] = options.pop('default_thread_slowmode_delay')
+        except KeyError:
+            pass
+
+        try:
+            rtc_region = options.pop('rtc_region')
+        except KeyError:
+            pass
+        else:
+            options['rtc_region'] = None if rtc_region is None else str(rtc_region)
+
+        try:
+            video_quality_mode = options.pop('video_quality_mode')
+        except KeyError:
+            pass
+        else:
+            options['video_quality_mode'] = int(video_quality_mode)
+
+        lock_permissions = options.pop('sync_permissions', False)
+
+        try:
+            position = options.pop('position')
+        except KeyError:
+            if parent_id is not _undefined:
+                if lock_permissions:
+                    category = self.guild.get_channel(parent_id)
+                    if category:
+                        options['permission_overwrites'] = [c._asdict() for c in category._overwrites]
+                options['parent_id'] = parent_id
+            elif lock_permissions and self.category_id is not None:
+                # If we're syncing permissions on a pre-existing channel category without changing it
+                # we need to update the permissions to point to the pre-existing category
+                category = self.guild.get_channel(self.category_id)
+                if category:
+                    options['permission_overwrites'] = [c._asdict() for c in category._overwrites]
+        else:
+            await self._move(position, parent_id=parent_id, lock_permissions=lock_permissions, reason=reason)
+
+        overwrites = options.get('overwrites', None)
+        if overwrites is not None:
+            perms = []
+            for target, perm in overwrites.items():
+                if not isinstance(perm, PermissionOverwrite):
+                    raise TypeError(f'Expected PermissionOverwrite received {perm.__class__.__name__}')
+
+                allow, deny = perm.pair()
+                payload = {
+                    'allow': allow.value,
+                    'deny': deny.value,
+                    'id': target.id,
+                }
+
+                if isinstance(target, Role):
+                    payload['type'] = _Overwrites.ROLE
+                elif isinstance(target, Object):
+                    payload['type'] = _Overwrites.ROLE if target.type is Role else _Overwrites.MEMBER
+                else:
+                    payload['type'] = _Overwrites.MEMBER
+
+                perms.append(payload)
+            options['permission_overwrites'] = perms
+
+        try:
+            ch_type = options['type']
+        except KeyError:
+            pass
+        else:
+            if not isinstance(ch_type, ChannelType):
+                raise TypeError('type field must be of type ChannelType')
+            options['type'] = ch_type.value
+
+        if options:
+            return await self._state.http.edit_channel(self.id, reason=reason, **options)
+
+    def _fill_overwrites(self, data: GuildChannelPayload) -> None:
+        self._overwrites = []
+        everyone_index = 0
+        everyone_id = self.guild.id
+
+        for index, overridden in enumerate(data.get('permission_overwrites', [])):
+            overwrite = _Overwrites(overridden)
+            self._overwrites.append(overwrite)
+
+            if overwrite.type == _Overwrites.MEMBER:
+                continue
+
+            if overwrite.id == everyone_id:
+                # the @everyone role is not guaranteed to be the first one
+                # in the list of permission overwrites, however the permission
+                # resolution code kind of requires that it is the first one in
+                # the list since it is special. So we need the index so we can
+                # swap it to be the first one.
+                everyone_index = index
+
+        # do the swap
+        tmp = self._overwrites
+        if tmp:
+            tmp[everyone_index], tmp[0] = tmp[0], tmp[everyone_index]
+
+    @property
+    def notification_settings(self) -> ChannelSettings:
+        """:class:`~discord.ChannelSettings`: Returns the notification settings for this channel.
+
+        If not found, an instance is created with defaults applied. This follows Discord behaviour.
+
+        .. versionadded:: 2.0
+        """
+        guild = self.guild
+        return guild.notification_settings._channel_overrides.get(
+            self.id, self._state.default_channel_settings(guild.id, self.id)
+        )
+
+    @property
+    def changed_roles(self) -> List[Role]:
+        """List[:class:`~discord.Role`]: Returns a list of roles that have been overridden from
+        their default values in the :attr:`~discord.Guild.roles` attribute."""
+        ret = []
+        g = self.guild
+        for overwrite in filter(lambda o: o.is_role(), self._overwrites):
+            role = g.get_role(overwrite.id)
+            if role is None:
+                continue
+
+            role = copy.copy(role)
+            role.permissions.handle_overwrite(overwrite.allow, overwrite.deny)
+            ret.append(role)
+        return ret
+
+    @property
+    def mention(self) -> str:
+        """:class:`str`: The string that allows you to mention the channel."""
+        return f'<#{self.id}>'
+
+    @property
+    def created_at(self) -> datetime:
+        """:class:`datetime.datetime`: Returns the channel's creation time in UTC."""
+        return utils.snowflake_time(self.id)
+
+    @property
+    def jump_url(self) -> str:
+        """:class:`str`: Returns a URL that allows the client to jump to the channel.
+
+        .. versionadded:: 2.0
+        """
+        return f'https://discord.com/channels/{self.guild.id}/{self.id}'
+
+    def overwrites_for(self, obj: Union[Role, User, Object]) -> PermissionOverwrite:
+        """Returns the channel-specific overwrites for a member or a role.
+
+        Parameters
+        -----------
+        obj: Union[:class:`~discord.Role`, :class:`~discord.abc.User`, :class:`~discord.Object`]
+            The role or user denoting whose overwrite to get.
+
+        Returns
+        ---------
+        :class:`~discord.PermissionOverwrite`
+            The permission overwrites for this object.
+        """
+
+        if isinstance(obj, User):
+            predicate = lambda p: p.is_member()
+        elif isinstance(obj, Role):
+            predicate = lambda p: p.is_role()
+        else:
+            predicate = lambda p: True
+
+        for overwrite in filter(predicate, self._overwrites):
+            if overwrite.id == obj.id:
+                allow = Permissions(overwrite.allow)
+                deny = Permissions(overwrite.deny)
+                return PermissionOverwrite.from_pair(allow, deny)
+
+        return PermissionOverwrite()
+
+    @property
+    def overwrites(self) -> Dict[Union[Role, Member, Object], PermissionOverwrite]:
+        """Returns all of the channel's overwrites.
+
+        This is returned as a dictionary where the key contains the target which
+        can be either a :class:`~discord.Role` or a :class:`~discord.Member` and the value is the
+        overwrite as a :class:`~discord.PermissionOverwrite`.
+
+        .. versionchanged:: 2.0
+            Overwrites can now be type-aware :class:`~discord.Object` in case of cache lookup failure
+
+        Returns
+        --------
+        Dict[Union[:class:`~discord.Role`, :class:`~discord.Member`, :class:`~discord.Object`], :class:`~discord.PermissionOverwrite`]
+            The channel's permission overwrites.
+        """
+        ret = {}
+        for ow in self._overwrites:
+            allow = Permissions(ow.allow)
+            deny = Permissions(ow.deny)
+            overwrite = PermissionOverwrite.from_pair(allow, deny)
+            target = None
+
+            if ow.is_role():
+                target = self.guild.get_role(ow.id)
+            elif ow.is_member():
+                target = self.guild.get_member(ow.id)
+
+            if target is None:
+                target_type = Role if ow.is_role() else User
+                target = Object(id=ow.id, type=target_type)  # type: ignore
+
+            ret[target] = overwrite
+        return ret
+
+    @property
+    def category(self) -> Optional[CategoryChannel]:
+        """Optional[:class:`~discord.CategoryChannel`]: The category this channel belongs to.
+
+        If there is no category then this is ``None``.
+        """
+        return self.guild.get_channel(self.category_id)  # type: ignore # These are coerced into CategoryChannel
+
+    @property
+    def permissions_synced(self) -> bool:
+        """:class:`bool`: Whether or not the permissions for this channel are synced with the
+        category it belongs to.
+
+        If there is no category then this is ``False``.
+
+        .. versionadded:: 1.3
+        """
+        if self.category_id is None:
+            return False
+
+        category = self.guild.get_channel(self.category_id)
+        return bool(category and category.overwrites == self.overwrites)
+
+    def _apply_implicit_permissions(self, base: Permissions) -> None:
+        # if you can't send a message in a channel then you can't have certain
+        # permissions as well
+        if not base.send_messages:
+            base.send_tts_messages = False
+            base.mention_everyone = False
+            base.embed_links = False
+            base.attach_files = False
+
+        # if you can't read a channel then you have no permissions there
+        if not base.read_messages:
+            denied = Permissions.all_channel()
+            base.value &= ~denied.value
+
+    def permissions_for(self, obj: Union[Member, Role], /) -> Permissions:
+        """Handles permission resolution for the :class:`~discord.Member`
+        or :class:`~discord.Role`.
+
+        This function takes into consideration the following cases:
+
+        - Guild owner
+        - Guild roles
+        - Channel overrides
+        - Member overrides
+        - Implicit permissions
+        - Member timeout
+
+        If a :class:`~discord.Role` is passed, then it checks the permissions
+        someone with that role would have, which is essentially:
+
+        - The default role permissions
+        - The permissions of the role used as a parameter
+        - The default role permission overwrites
+        - The permission overwrites of the role used as a parameter
+
+        .. versionchanged:: 2.0
+            The object passed in can now be a role object.
+
+        .. versionchanged:: 2.0
+            ``obj`` parameter is now positional-only.
+
+        Parameters
+        ----------
+        obj: Union[:class:`~discord.Member`, :class:`~discord.Role`]
+            The object to resolve permissions for. This could be either
+            a member or a role. If it's a role then member overwrites
+            are not computed.
+
+        Returns
+        -------
+        :class:`~discord.Permissions`
+            The resolved permissions for the member or role.
+        """
+
+        # The current cases can be explained as:
+        # Guild owner get all permissions -- no questions asked
+        # The @everyone role gets the first application
+        # After that, the applied roles that the user has in the channel
+        # (or otherwise) are then OR'd together
+        # After the role permissions are resolved, the member permissions
+        # have to take into effect
+        # After all that is done, you have to do the following:
+
+        # If manage permissions is True, then all permissions are set to True
+
+        # The operation first takes into consideration the denied
+        # and then the allowed
+
+        if self.guild.owner_id == obj.id:
+            return Permissions.all()
+
+        default = self.guild.default_role
+        base = Permissions(default.permissions.value)
+
+        # Handle the role case first
+        if isinstance(obj, Role):
+            base.value |= obj._permissions
+
+            if base.administrator:
+                return Permissions.all()
+
+            # Apply @everyone allow/deny first since it's special
+            try:
+                maybe_everyone = self._overwrites[0]
+                if maybe_everyone.id == self.guild.id:
+                    base.handle_overwrite(allow=maybe_everyone.allow, deny=maybe_everyone.deny)
+            except IndexError:
+                pass
+
+            if obj.is_default():
+                return base
+
+            overwrite = utils.get(self._overwrites, type=_Overwrites.ROLE, id=obj.id)
+            if overwrite is not None:
+                base.handle_overwrite(overwrite.allow, overwrite.deny)
+
+            return base
+
+        roles = obj._roles
+        get_role = self.guild.get_role
+
+        # Apply guild roles that the member has.
+        for role_id in roles:
+            role = get_role(role_id)
+            if role is not None:
+                base.value |= role._permissions
+
+        # Guild-wide Administrator -> True for everything
+        # Bypass all channel-specific overrides
+        if base.administrator:
+            return Permissions.all()
+
+        # Apply @everyone allow/deny first since it's special
+        try:
+            maybe_everyone = self._overwrites[0]
+            if maybe_everyone.id == self.guild.id:
+                base.handle_overwrite(allow=maybe_everyone.allow, deny=maybe_everyone.deny)
+                remaining_overwrites = self._overwrites[1:]
+            else:
+                remaining_overwrites = self._overwrites
+        except IndexError:
+            remaining_overwrites = self._overwrites
+
+        denies = 0
+        allows = 0
+
+        # Apply channel specific role permission overwrites
+        for overwrite in remaining_overwrites:
+            if overwrite.is_role() and roles.has(overwrite.id):
+                denies |= overwrite.deny
+                allows |= overwrite.allow
+
+        base.handle_overwrite(allow=allows, deny=denies)
+
+        # Apply member specific permission overwrites
+        for overwrite in remaining_overwrites:
+            if overwrite.is_member() and overwrite.id == obj.id:
+                base.handle_overwrite(allow=overwrite.allow, deny=overwrite.deny)
+                break
+
+        if obj.is_timed_out():
+            # Timeout leads to every permission except VIEW_CHANNEL and READ_MESSAGE_HISTORY
+            # being explicitly denied
+            # N.B.: This *must* come last, because it's a conclusive mask
+            base.value &= Permissions._timeout_mask()
+
+        return base
+
+    async def delete(self, *, reason: Optional[str] = None) -> None:
+        """|coro|
+
+        Deletes the channel.
+
+        You must have :attr:`~discord.Permissions.manage_channels` to do this.
+
+        Parameters
+        -----------
+        reason: Optional[:class:`str`]
+            The reason for deleting this channel.
+            Shows up on the audit log.
+
+        Raises
+        -------
+        ~discord.Forbidden
+            You do not have proper permissions to delete the channel.
+        ~discord.NotFound
+            The channel was not found or was already deleted.
+        ~discord.HTTPException
+            Deleting the channel failed.
+        """
+        await self._state.http.delete_channel(self.id, reason=reason)
+
+    @overload
+    async def set_permissions(
+        self,
+        target: Union[Member, Role],
+        *,
+        overwrite: Optional[Union[PermissionOverwrite, _Undefined]] = ...,
+        reason: Optional[str] = ...,
+    ) -> None:
+        ...
+
+    @overload
+    async def set_permissions(
+        self,
+        target: Union[Member, Role],
+        *,
+        reason: Optional[str] = ...,
+        **permissions: Optional[bool],
+    ) -> None:
+        ...
+
+    async def set_permissions(
+        self,
+        target: Union[Member, Role],
+        *,
+        overwrite: Any = _undefined,
+        reason: Optional[str] = None,
+        **permissions: Optional[bool],
+    ) -> None:
+        r"""|coro|
+
+        Sets the channel specific permission overwrites for a target in the
+        channel.
+
+        The ``target`` parameter should either be a :class:`~discord.Member` or a
+        :class:`~discord.Role` that belongs to guild.
+
+        The ``overwrite`` parameter, if given, must either be ``None`` or
+        :class:`~discord.PermissionOverwrite`. For convenience, you can pass in
+        keyword arguments denoting :class:`~discord.Permissions` attributes. If this is
+        done, then you cannot mix the keyword arguments with the ``overwrite``
+        parameter.
+
+        If the ``overwrite`` parameter is ``None``, then the permission
+        overwrites are deleted.
+
+        You must have :attr:`~discord.Permissions.manage_roles` to do this.
+
+        .. note::
+
+            This method *replaces* the old overwrites with the ones given.
+
+        Examples
+        ----------
+
+        Setting allow and deny: ::
+
+            await message.channel.set_permissions(message.author, read_messages=True,
+                                                                  send_messages=False)
+
+        Deleting overwrites ::
+
+            await channel.set_permissions(member, overwrite=None)
+
+        Using :class:`~discord.PermissionOverwrite` ::
+
+            overwrite = discord.PermissionOverwrite()
+            overwrite.send_messages = False
+            overwrite.read_messages = True
+            await channel.set_permissions(member, overwrite=overwrite)
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+
+        Parameters
+        -----------
+        target: Union[:class:`~discord.Member`, :class:`~discord.Role`]
+            The member or role to overwrite permissions for.
+        overwrite: Optional[:class:`~discord.PermissionOverwrite`]
+            The permissions to allow and deny to the target, or ``None`` to
+            delete the overwrite.
+        \*\*permissions
+            A keyword argument list of permissions to set for ease of use.
+            Cannot be mixed with ``overwrite``.
+        reason: Optional[:class:`str`]
+            The reason for doing this action. Shows up on the audit log.
+
+        Raises
+        -------
+        ~discord.Forbidden
+            You do not have permissions to edit channel specific permissions.
+        ~discord.HTTPException
+            Editing channel specific permissions failed.
+        ~discord.NotFound
+            The role or member being edited is not part of the guild.
+        TypeError
+            The ``overwrite`` parameter was invalid or the target type was not
+            :class:`~discord.Role` or :class:`~discord.Member`.
+        ValueError
+            The ``overwrite`` parameter and ``positions`` parameters were both
+            unset.
+        """
+
+        http = self._state.http
+
+        if isinstance(target, User):
+            perm_type = _Overwrites.MEMBER
+        elif isinstance(target, Role):
+            perm_type = _Overwrites.ROLE
+        else:
+            raise ValueError('target parameter must be either Member or Role')
+
+        if overwrite is _undefined:
+            if len(permissions) == 0:
+                raise ValueError('No overwrite provided.')
+            try:
+                overwrite = PermissionOverwrite(**permissions)
+            except (ValueError, TypeError):
+                raise TypeError('Invalid permissions given to keyword arguments.')
+        else:
+            if len(permissions) > 0:
+                raise TypeError('Cannot mix overwrite and keyword arguments.')
+
+        # TODO: wait for event
+
+        if overwrite is None:
+            await http.delete_channel_permissions(self.id, target.id, reason=reason)
+        elif isinstance(overwrite, PermissionOverwrite):
+            (allow, deny) = overwrite.pair()
+            await http.edit_channel_permissions(
+                self.id, target.id, str(allow.value), str(deny.value), perm_type, reason=reason
+            )
+        else:
+            raise TypeError('Invalid overwrite type provided.')
+
+    async def _clone_impl(
+        self,
+        base_attrs: Dict[str, Any],
+        *,
+        name: Optional[str] = None,
+        reason: Optional[str] = None,
+    ) -> Self:
+        base_attrs['permission_overwrites'] = [x._asdict() for x in self._overwrites]
+        base_attrs['parent_id'] = self.category_id
+        base_attrs['name'] = name or self.name
+        guild_id = self.guild.id
+        cls = self.__class__
+        data = await self._state.http.create_channel(guild_id, self.type.value, reason=reason, **base_attrs)
+        obj = cls(state=self._state, guild=self.guild, data=data)
+
+        # Temporarily add it to the cache
+        self.guild._channels[obj.id] = obj  # type: ignore # obj is a GuildChannel
+        return obj
+
+    async def clone(self, *, name: Optional[str] = None, reason: Optional[str] = None) -> Self:
+        """|coro|
+
+        Clones this channel. This creates a channel with the same properties
+        as this channel.
+
+        You must have :attr:`~discord.Permissions.manage_channels` to do this.
+
+        .. versionadded:: 1.1
+
+        Parameters
+        ------------
+        name: Optional[:class:`str`]
+            The name of the new channel. If not provided, defaults to this
+            channel name.
+        reason: Optional[:class:`str`]
+            The reason for cloning this channel. Shows up on the audit log.
+
+        Raises
+        -------
+        ~discord.Forbidden
+            You do not have the proper permissions to create this channel.
+        ~discord.HTTPException
+            Creating the channel failed.
+
+        Returns
+        --------
+        :class:`.abc.GuildChannel`
+            The channel that was created.
+        """
+        raise NotImplementedError
+
+    @overload
+    async def move(
+        self,
+        *,
+        beginning: bool,
+        offset: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        sync_permissions: bool = MISSING,
+        reason: Optional[str] = MISSING,
+    ) -> None:
+        ...
+
+    @overload
+    async def move(
+        self,
+        *,
+        end: bool,
+        offset: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        sync_permissions: bool = MISSING,
+        reason: str = MISSING,
+    ) -> None:
+        ...
+
+    @overload
+    async def move(
+        self,
+        *,
+        before: Snowflake,
+        offset: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        sync_permissions: bool = MISSING,
+        reason: str = MISSING,
+    ) -> None:
+        ...
+
+    @overload
+    async def move(
+        self,
+        *,
+        after: Snowflake,
+        offset: int = MISSING,
+        category: Optional[Snowflake] = MISSING,
+        sync_permissions: bool = MISSING,
+        reason: str = MISSING,
+    ) -> None:
+        ...
+
+    async def move(self, **kwargs: Any) -> None:
+        """|coro|
+
+        A rich interface to help move a channel relative to other channels.
+
+        If exact position movement is required, ``edit`` should be used instead.
+
+        You must have :attr:`~discord.Permissions.manage_channels` to do this.
+
+        .. note::
+
+            Voice channels will always be sorted below text channels.
+            This is a Discord limitation.
+
+        .. versionadded:: 1.7
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` or
+            :exc:`ValueError` instead of ``InvalidArgument``.
+
+        Parameters
+        ------------
+        beginning: :class:`bool`
+            Whether to move the channel to the beginning of the
+            channel list (or category if given).
+            This is mutually exclusive with ``end``, ``before``, and ``after``.
+        end: :class:`bool`
+            Whether to move the channel to the end of the
+            channel list (or category if given).
+            This is mutually exclusive with ``beginning``, ``before``, and ``after``.
+        before: :class:`~discord.abc.Snowflake`
+            The channel that should be before our current channel.
+            This is mutually exclusive with ``beginning``, ``end``, and ``after``.
+        after: :class:`~discord.abc.Snowflake`
+            The channel that should be after our current channel.
+            This is mutually exclusive with ``beginning``, ``end``, and ``before``.
+        offset: :class:`int`
+            The number of channels to offset the move by. For example,
+            an offset of ``2`` with ``beginning=True`` would move
+            it 2 after the beginning. A positive number moves it below
+            while a negative number moves it above. Note that this
+            number is relative and computed after the ``beginning``,
+            ``end``, ``before``, and ``after`` parameters.
+        category: Optional[:class:`~discord.abc.Snowflake`]
+            The category to move this channel under.
+            If ``None`` is given then it moves it out of the category.
+            This parameter is ignored if moving a category channel.
+        sync_permissions: :class:`bool`
+            Whether to sync the permissions with the category (if given).
+        reason: :class:`str`
+            The reason for the move.
+
+        Raises
+        -------
+        ValueError
+            An invalid position was given.
+        TypeError
+            A bad mix of arguments were passed.
+        Forbidden
+            You do not have permissions to move the channel.
+        HTTPException
+            Moving the channel failed.
+        """
+
+        if not kwargs:
+            return
+
+        beginning, end = kwargs.get('beginning'), kwargs.get('end')
+        before, after = kwargs.get('before'), kwargs.get('after')
+        offset = kwargs.get('offset', 0)
+        if sum(bool(a) for a in (beginning, end, before, after)) > 1:
+            raise TypeError('Only one of [before, after, end, beginning] can be used.')
+
+        bucket = self._sorting_bucket
+        parent_id = kwargs.get('category', MISSING)
+        # fmt: off
+        channels: List[GuildChannel]
+        if parent_id not in (MISSING, None):
+            parent_id = parent_id.id
+            channels = [
+                ch
+                for ch in self.guild.channels
+                if ch._sorting_bucket == bucket
+                and ch.category_id == parent_id
+            ]
+        else:
+            channels = [
+                ch
+                for ch in self.guild.channels
+                if ch._sorting_bucket == bucket
+                and ch.category_id == self.category_id
+            ]
+        # fmt: on
+
+        channels.sort(key=lambda c: (c.position, c.id))
+
+        try:
+            # Try to remove ourselves from the channel list
+            channels.remove(self)
+        except ValueError:
+            # If we're not there then it's probably due to not being in the category
+            pass
+
+        index = None
+        if beginning:
+            index = 0
+        elif end:
+            index = len(channels)
+        elif before:
+            index = next((i for i, c in enumerate(channels) if c.id == before.id), None)
+        elif after:
+            index = next((i + 1 for i, c in enumerate(channels) if c.id == after.id), None)
+
+        if index is None:
+            raise ValueError('Could not resolve appropriate move position')
+
+        channels.insert(max((index + offset), 0), self)
+        payload = []
+        lock_permissions = kwargs.get('sync_permissions', False)
+        reason = kwargs.get('reason')
+        for index, channel in enumerate(channels):
+            d = {'id': channel.id, 'position': index}
+            if parent_id is not MISSING and channel.id == self.id:
+                d.update(parent_id=parent_id, lock_permissions=lock_permissions)
+            payload.append(d)
+
+        await self._state.http.bulk_channel_update(self.guild.id, payload, reason=reason)
+
+    async def create_invite(  # TODO: add validate
+        self,
+        *,
+        reason: Optional[str] = None,
+        max_age: int = 0,
+        max_uses: int = 0,
+        temporary: bool = False,
+        unique: bool = True,
+        validate: Optional[Union[Invite, str]],
+        target_type: Optional[InviteTarget] = None,
+        target_user: Optional[User] = None,
+        target_application: Optional[Snowflake] = None,
+    ) -> Invite:
+        """|coro|
+
+        Creates an instant invite from a text or voice channel.
+
+        You must have :attr:`~discord.Permissions.create_instant_invite` to do this.
+
+        Parameters
+        ------------
+        max_age: :class:`int`
+            How long the invite should last in seconds. If it's 0 then the invite
+            doesn't expire. Defaults to ``0``.
+        max_uses: :class:`int`
+            How many uses the invite could be used for. If it's 0 then there
+            are unlimited uses. Defaults to ``0``.
+        temporary: :class:`bool`
+            Denotes that the invite grants temporary membership
+            (i.e. they get kicked after they disconnect). Defaults to ``False``.
+        unique: :class:`bool`
+            Indicates if a unique invite URL should be created. Defaults to True.
+            If this is set to ``False`` then it will return a previously created
+            invite.
+        validate: Union[:class:`.Invite`, :class:`str`]
+            The existing channel invite to validate and return for reuse.
+            If this invite is invalid, a new invite will be created according to the parameters and returned.
+
+            .. versionadded:: 2.0
+        target_type: Optional[:class:`.InviteTarget`]
+            The type of target for the voice channel invite, if any.
+
+            .. versionadded:: 2.0
+
+        target_user: Optional[:class:`User`]
+            The user whose stream to display for this invite, required if ``target_type`` is :attr:`.InviteTarget.stream`. The user must be streaming in the channel.
+
+            .. versionadded:: 2.0
+
+        target_application:: Optional[:class:`.Application`]
+            The embedded application for the invite, required if ``target_type`` is :attr:`.InviteTarget.embedded_application`.
+
+            .. versionadded:: 2.0
+
+        reason: Optional[:class:`str`]
+            The reason for creating this invite. Shows up on the audit log.
+
+        Raises
+        -------
+        ~discord.HTTPException
+            Invite creation failed.
+        ~discord.NotFound
+            The channel that was passed is a category or an invalid channel.
+
+        Returns
+        --------
+        :class:`~discord.Invite`
+            The invite that was created.
+        """
+
+        data = await self._state.http.create_invite(
+            self.id,
+            reason=reason,
+            max_age=max_age,
+            max_uses=max_uses,
+            temporary=temporary,
+            unique=unique,
+            validate=utils.resolve_invite(validate).code if validate else None,
+            target_type=target_type.value if target_type else None,
+            target_user_id=target_user.id if target_user else None,
+            target_application_id=target_application.id if target_application else None,
+        )
+        return Invite.from_incomplete(data=data, state=self._state)
+
+    async def invites(self) -> List[Invite]:
+        """|coro|
+
+        Returns a list of all active instant invites from this channel.
+
+        You must have :attr:`~discord.Permissions.manage_channels` to get this information.
+
+        Raises
+        -------
+        ~discord.Forbidden
+            You do not have proper permissions to get the information.
+        ~discord.HTTPException
+            An error occurred while fetching the information.
+
+        Returns
+        -------
+        List[:class:`~discord.Invite`]
+            The list of invites that are currently active.
+        """
+
+        state = self._state
+        data = await state.http.invites_from_channel(self.id)
+        guild = self.guild
+        return [Invite(state=state, data=invite, channel=self, guild=guild) for invite in data]
+
+
+class Messageable:
+    """An ABC that details the common operations on a model that can send messages.
+
+    The following implement this ABC:
+
+    - :class:`~discord.TextChannel`
+    - :class:`~discord.VoiceChannel`
+    - :class:`~discord.StageChannel`
+    - :class:`~discord.DMChannel`
+    - :class:`~discord.GroupChannel`
+    - :class:`~discord.User`
+    - :class:`~discord.Member`
+    - :class:`~discord.ext.commands.Context`
+    - :class:`~discord.Thread`
+    """
+
+    __slots__ = ()
+    _state: ConnectionState
+
+    async def _get_channel(self) -> MessageableChannel:
+        raise NotImplementedError
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    async def send(
+        self,
+        content: Optional[str] = None,
+        *,
+        tts: bool = False,
+        file: Optional[File] = None,
+        files: Optional[Sequence[File]] = None,
+        stickers: Optional[Sequence[Union[GuildSticker, StickerItem]]] = None,
+        delete_after: Optional[float] = None,
+        nonce: Optional[Union[str, int]] = MISSING,
+        allowed_mentions: Optional[AllowedMentions] = None,
+        reference: Optional[Union[Message, MessageReference, PartialMessage]] = None,
+        mention_author: Optional[bool] = None,
+        suppress_embeds: bool = False,
+        silent: bool = False,
+    ) -> Message:
+        """|coro|
+
+        Sends a message to the destination with the content given.
+
+        The content must be a type that can convert to a string through ``str(content)``.
+        If the content is set to ``None`` (the default), then a sticker or file must be sent.
+
+        To upload a single file, the ``file`` parameter should be used with a
+        single :class:`~discord.File` object. To upload multiple files, the ``files``
+        parameter should be used with a :class:`list` of :class:`~discord.File` objects.
+        **Specifying both parameters will lead to an exception**.
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` or
+            :exc:`ValueError` instead of ``InvalidArgument``.
+
+        Parameters
+        ------------
+        content: Optional[:class:`str`]
+            The content of the message to send.
+        tts: :class:`bool`
+            Indicates if the message should be sent using text-to-speech.
+        file: :class:`~discord.File`
+            The file to upload.
+        files: List[:class:`~discord.File`]
+            A list of files to upload. Must be a maximum of 10.
+        nonce: :class:`int`
+            The nonce to use for sending this message. If the message was successfully sent,
+            then the message will have a nonce with this value. Generates one by default.
+        delete_after: :class:`float`
+            If provided, the number of seconds to wait in the background
+            before deleting the message we just sent. If the deletion fails,
+            then it is silently ignored.
+        allowed_mentions: :class:`~discord.AllowedMentions`
+            Controls the mentions being processed in this message. If this is
+            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
+            The merging behaviour only overrides attributes that have been explicitly passed
+            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
+            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
+            are used instead.
+
+            .. versionadded:: 1.4
+
+        reference: Union[:class:`~discord.Message`, :class:`~discord.MessageReference`, :class:`~discord.PartialMessage`]
+            A reference to the :class:`~discord.Message` to which you are replying, this can be created using
+            :meth:`~discord.Message.to_reference` or passed directly as a :class:`~discord.Message`. You can control
+            whether this mentions the author of the referenced message using the :attr:`~discord.AllowedMentions.replied_user`
+            attribute of ``allowed_mentions`` or by setting ``mention_author``.
+
+            .. versionadded:: 1.6
+
+        mention_author: Optional[:class:`bool`]
+            If set, overrides the :attr:`~discord.AllowedMentions.replied_user` attribute of ``allowed_mentions``.
+
+            .. versionadded:: 1.6
+        stickers: Sequence[Union[:class:`~discord.GuildSticker`, :class:`~discord.StickerItem`]]
+            A list of stickers to upload. Must be a maximum of 3.
+
+            .. versionadded:: 2.0
+        suppress_embeds: :class:`bool`
+            Whether to suppress embeds for the message. This sends the message without any embeds if set to ``True``.
+
+            .. versionadded:: 2.0
+        silent: :class:`bool`
+            Whether to suppress push and desktop notifications for the message. This will increment the mention counter
+            in the UI, but will not actually send a notification.
+
+            .. versionadded:: 2.0
+
+        Raises
+        --------
+        ~discord.HTTPException
+            Sending the message failed.
+        ~discord.Forbidden
+            You do not have the proper permissions to send the message.
+        ValueError
+            The ``files`` list is not of the appropriate size.
+        TypeError
+            You specified both ``file`` and ``files``,
+            or the ``reference`` object is not a :class:`~discord.Message`,
+            :class:`~discord.MessageReference` or :class:`~discord.PartialMessage`.
+
+        Returns
+        ---------
+        :class:`~discord.Message`
+            The message that was sent.
+        """
+
+        channel = await self._get_channel()
+        state = self._state
+        content = str(content) if content is not None else None
+        previous_allowed_mention = state.allowed_mentions
+
+        if nonce is MISSING:
+            nonce = utils._generate_nonce()
+
+        if stickers is not None:
+            sticker_ids: SnowflakeList = [sticker.id for sticker in stickers]
+        else:
+            sticker_ids = MISSING
+
+        if reference is not None:
+            try:
+                reference_dict = reference.to_message_reference_dict()
+            except AttributeError:
+                raise TypeError('reference parameter must be Message, MessageReference, or PartialMessage') from None
+        else:
+            reference_dict = MISSING
+
+        if suppress_embeds or silent:
+            from .message import MessageFlags  # circular import
+
+            flags = MessageFlags._from_value(0)
+            flags.suppress_embeds = suppress_embeds
+            flags.suppress_notifications = silent
+        else:
+            flags = MISSING
+
+        with handle_message_parameters(
+            content=content,
+            tts=tts,
+            file=file if file is not None else MISSING,
+            files=files if files is not None else MISSING,
+            nonce=nonce,
+            allowed_mentions=allowed_mentions,
+            message_reference=reference_dict,
+            previous_allowed_mentions=previous_allowed_mention,
+            mention_author=mention_author,
+            stickers=sticker_ids,
+            flags=flags,
+        ) as params:
+            data = await state.http.send_message(channel.id, params=params)
+
+        ret = state.create_message(channel=channel, data=data)
+
+        if delete_after is not None:
+            await ret.delete(delay=delete_after)
+        return ret
+
+    async def greet(
+        self,
+        sticker: Union[GuildSticker, StickerItem],
+        *,
+        allowed_mentions: AllowedMentions = MISSING,
+        reference: Union[Message, MessageReference, PartialMessage] = MISSING,
+        mention_author: bool = MISSING,
+    ) -> Message:
+        """|coro|
+
+        Sends a sticker greeting to the destination.
+
+        A sticker greeting is used to begin a new DM or reply to a system message.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        ------------
+        sticker: Union[:class:`~discord.GuildSticker`, :class:`~discord.StickerItem`]
+            The sticker to greet with.
+        allowed_mentions: :class:`~discord.AllowedMentions`
+            Controls the mentions being processed in this message. If this is
+            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
+            The merging behaviour only overrides attributes that have been explicitly passed
+            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
+            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
+            are used instead. In the case of greeting, only :attr:`~discord.AllowedMentions.replied_user` is
+            considered.
+        reference: Union[:class:`~discord.Message`, :class:`~discord.MessageReference`, :class:`~discord.PartialMessage`]
+            A reference to the :class:`~discord.Message` to which you are replying, this can be created using
+            :meth:`~discord.Message.to_reference` or passed directly as a :class:`~discord.Message`. You can control
+            whether this mentions the author of the referenced message using the :attr:`~discord.AllowedMentions.replied_user`
+            attribute of ``allowed_mentions`` or by setting ``mention_author``.
+        mention_author: :class:`bool`
+            If set, overrides the :attr:`~discord.AllowedMentions.replied_user` attribute of ``allowed_mentions``.
+
+        Raises
+        --------
+        ~discord.HTTPException
+            Sending the message failed.
+        ~discord.Forbidden
+            You do not have the proper permissions to send the message, or this is not a valid greet context.
+        TypeError
+            The ``reference`` object is not a :class:`~discord.Message`,
+            :class:`~discord.MessageReference` or :class:`~discord.PartialMessage`.
+
+        Returns
+        ---------
+        :class:`~discord.Message`
+            The sticker greeting that was sent.
+        """
+        channel = await self._get_channel()
+        state = self._state
+        previous_allowed_mention = state.allowed_mentions
+
+        if reference:
+            try:
+                reference_dict = reference.to_message_reference_dict()
+            except AttributeError:
+                raise TypeError('reference parameter must be Message, MessageReference, or PartialMessage') from None
+        else:
+            reference_dict = MISSING
+
+        if allowed_mentions:
+            if previous_allowed_mention:
+                allowed_mentions = previous_allowed_mention.merge(allowed_mentions)
+        if mention_author is not MISSING:
+            if not allowed_mentions:
+                allowed_mentions = AllowedMentions()
+            allowed_mentions.replied_user = mention_author
+        if allowed_mentions and allowed_mentions.replied_user:
+            # No point sending them
+            allowed_mentions = MISSING
+
+        data = await state.http.send_greet(
+            channel.id, sticker.id, message_reference=reference_dict, allowed_mentions=allowed_mentions
+        )
+        return state.create_message(channel=channel, data=data)
+
+    def typing(self) -> Typing:
+        """Returns an asynchronous context manager that allows you to send a typing indicator to
+        the destination for an indefinite period of time, or 10 seconds if the context manager
+        is called using ``await``.
+
+        Example Usage: ::
+
+            async with channel.typing():
+                # simulate something heavy
+                await asyncio.sleep(20)
+
+            await channel.send('Done!')
+
+        Example Usage: ::
+
+            await channel.typing()
+            # Do some computational magic for about 10 seconds
+            await channel.send('Done!')
+
+        .. versionchanged:: 2.0
+            This no longer works with the ``with`` syntax, ``async with`` must be used instead.
+
+        .. versionchanged:: 2.0
+            Added functionality to ``await`` the context manager to send a typing indicator for 10 seconds.
+        """
+        return Typing(self)
+
+    async def fetch_message(self, id: int, /) -> Message:
+        """|coro|
+
+        Retrieves a single :class:`~discord.Message` from the destination.
+
+        Parameters
+        ------------
+        id: :class:`int`
+            The message ID to look for.
+
+        Raises
+        --------
+        ~discord.NotFound
+            The specified message was not found.
+        ~discord.Forbidden
+            You do not have the permissions required to get a message.
+        ~discord.HTTPException
+            Retrieving the message failed.
+
+        Returns
+        --------
+        :class:`~discord.Message`
+            The message asked for.
+        """
+        channel = await self._get_channel()
+        data = await self._state.http.get_message(channel.id, id)
+        return self._state.create_message(channel=channel, data=data)
+
+    async def ack(self) -> None:
+        """|coro|
+
+        Marks every message in this channel as read.
+
+        Raises
+        -------
+        ~discord.HTTPException
+            Acking the channel failed.
+        """
+        channel = await self._get_channel()
+        await self._state.http.ack_message(channel.id, channel.last_message_id or utils.time_snowflake(utils.utcnow()))
+
+    async def ack_pins(self) -> None:
+        """|coro|
+
+        Marks a channel's pins as viewed.
+
+        Raises
+        -------
+        ~discord.HTTPException
+            Acking the pinned messages failed.
+        """
+        channel = await self._get_channel()
+        await self._state.http.ack_pins(channel.id)
+
+    async def pins(self) -> List[Message]:
+        """|coro|
+
+        Retrieves all messages that are currently pinned in the channel.
+
+        .. note::
+
+            Due to a limitation with the Discord API, the :class:`.Message`
+            objects returned by this method do not contain complete
+            :attr:`.Message.reactions` data.
+
+        Raises
+        -------
+        ~discord.Forbidden
+            You do not have the permission to retrieve pinned messages.
+        ~discord.HTTPException
+            Retrieving the pinned messages failed.
+
+        Returns
+        --------
+        List[:class:`~discord.Message`]
+            The messages that are currently pinned.
+        """
+        channel = await self._get_channel()
+        state = self._state
+        data = await state.http.pins_from(channel.id)
+        return [state.create_message(channel=channel, data=m) for m in data]
+
+    async def history(
+        self,
+        *,
+        limit: Optional[int] = 100,
+        before: Optional[SnowflakeTime] = None,
+        after: Optional[SnowflakeTime] = None,
+        around: Optional[SnowflakeTime] = None,
+        oldest_first: Optional[bool] = None,
+    ) -> AsyncIterator[Message]:
+        """Returns an :term:`asynchronous iterator` that enables receiving the destination's message history.
+
+        You must have :attr:`~discord.Permissions.read_message_history` to do this.
+
+        Examples
+        ---------
+
+        Usage ::
+
+            counter = 0
+            async for message in channel.history(limit=200):
+                if message.author == client.user:
+                    counter += 1
+
+        Flattening into a list: ::
+
+            messages = [message async for message in channel.history(limit=123)]
+            # messages is now a list of Message...
+
+        All parameters are optional.
+
+        Parameters
+        -----------
+        limit: Optional[:class:`int`]
+            The number of messages to retrieve.
+            If ``None``, retrieves every message in the channel. Note, however,
+            that this would make it a slow operation.
+        before: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
+            Retrieve messages before this date or message.
+            If a datetime is provided, it is recommended to use a UTC aware datetime.
+            If the datetime is naive, it is assumed to be local time.
+        after: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
+            Retrieve messages after this date or message.
+            If a datetime is provided, it is recommended to use a UTC aware datetime.
+            If the datetime is naive, it is assumed to be local time.
+        around: Optional[Union[:class:`~discord.abc.Snowflake`, :class:`datetime.datetime`]]
+            Retrieve messages around this date or message.
+            If a datetime is provided, it is recommended to use a UTC aware datetime.
+            If the datetime is naive, it is assumed to be local time.
+            When using this argument, the maximum limit is 101. Note that if the limit is an
+            even number then this will return at most limit + 1 messages.
+        oldest_first: Optional[:class:`bool`]
+            If set to ``True``, return messages in oldest->newest order. Defaults to ``True`` if
+            ``after`` is specified, otherwise ``False``.
+
+        Raises
+        ------
+        ~discord.Forbidden
+            You do not have permissions to get channel message history.
+        ~discord.HTTPException
+            The request to get message history failed.
+
+        Yields
+        -------
+        :class:`~discord.Message`
+            The message with the message data parsed.
+        """
+
+        async def _around_strategy(retrieve: int, around: Optional[Snowflake], limit: Optional[int]):
+            if not around:
+                return []
+
+            around_id = around.id if around else None
+            data = await self._state.http.logs_from(channel.id, retrieve, around=around_id)
+
+            return data, None, limit
+
+        async def _after_strategy(retrieve: int, after: Optional[Snowflake], limit: Optional[int]):
+            after_id = after.id if after else None
+            data = await self._state.http.logs_from(channel.id, retrieve, after=after_id)
+
+            if data:
+                if limit is not None:
+                    limit -= len(data)
+
+                after = Object(id=int(data[0]['id']))
+
+            return data, after, limit
+
+        async def _before_strategy(retrieve: int, before: Optional[Snowflake], limit: Optional[int]):
+            before_id = before.id if before else None
+            data = await self._state.http.logs_from(channel.id, retrieve, before=before_id)
+
+            if data:
+                if limit is not None:
+                    limit -= len(data)
+
+                before = Object(id=int(data[-1]['id']))
+
+            return data, before, limit
+
+        if isinstance(before, datetime):
+            before = Object(id=utils.time_snowflake(before, high=False))
+        if isinstance(after, datetime):
+            after = Object(id=utils.time_snowflake(after, high=True))
+        if isinstance(around, datetime):
+            around = Object(id=utils.time_snowflake(around))
+
+        if oldest_first is None:
+            reverse = after is not None
+        else:
+            reverse = oldest_first
+
+        after = after or OLDEST_OBJECT
+        predicate = None
+
+        if around:
+            if limit is None:
+                raise ValueError('history does not support around with limit=None')
+            if limit > 101:
+                raise ValueError("history max limit 101 when specifying around parameter")
+
+            # Strange Discord quirk
+            limit = 100 if limit == 101 else limit
+
+            strategy, state = _around_strategy, around
+
+            if before and after:
+                predicate = lambda m: after.id < int(m['id']) < before.id
+            elif before:
+                predicate = lambda m: int(m['id']) < before.id
+            elif after:
+                predicate = lambda m: after.id < int(m['id'])
+        elif reverse:
+            strategy, state = _after_strategy, after
+            if before:
+                predicate = lambda m: int(m['id']) < before.id
+        else:
+            strategy, state = _before_strategy, before
+            if after and after != OLDEST_OBJECT:
+                predicate = lambda m: int(m['id']) > after.id
+
+        channel = await self._get_channel()
+
+        while True:
+            retrieve = 100 if limit is None else min(limit, 100)
+            if retrieve < 1:
+                return
+
+            data, state, limit = await strategy(retrieve, state, limit)
+
+            if reverse:
+                data = reversed(data)
+            if predicate:
+                data = filter(predicate, data)
+
+            count = 0
+
+            for count, raw_message in enumerate(data, 1):
+                yield self._state.create_message(channel=channel, data=raw_message)
+
+            if count < 100:
+                # There's no data left after this
+                break
+
+    def slash_commands(
+        self,
+        query: Optional[str] = None,
+        *,
+        limit: Optional[int] = None,
+        command_ids: Optional[Collection[int]] = None,
+        application: Optional[Snowflake] = None,
+        with_applications: bool = True,
+    ) -> AsyncIterator[SlashCommand]:
+        """Returns a :term:`asynchronous iterator` of the slash commands available in the channel.
+
+        Examples
+        ---------
+
+        Usage ::
+
+            async for command in channel.slash_commands():
+                print(command.name)
+
+        Flattening into a list ::
+
+            commands = [command async for command in channel.slash_commands()]
+            # commands is now a list of SlashCommand...
+
+        All parameters are optional.
+
+        Parameters
+        ----------
+        query: Optional[:class:`str`]
+            The query to search for. Specifying this limits results to 25 commands max.
+
+            This parameter is faked if ``application`` is specified.
+        limit: Optional[:class:`int`]
+            The maximum number of commands to send back. Defaults to 0 if ``command_ids`` is passed, else 25.
+            If ``None``, returns all commands.
+
+            This parameter is faked if ``application`` is specified.
+        command_ids: Optional[List[:class:`int`]]
+            List of up to 100 command IDs to search for. If the command doesn't exist, it won't be returned.
+
+            If ``limit`` is passed alongside this parameter, this parameter will serve as a "preferred commands" list.
+            This means that the endpoint will return the found commands + up to ``limit`` more, if available.
+        application: Optional[:class:`~discord.abc.Snowflake`]
+            Whether to return this application's commands. Always set to DM recipient in a private channel context.
+        with_applications: :class:`bool`
+            Whether to include applications in the response. Defaults to ``True``.
+
+        Raises
+        ------
+        TypeError
+            Both query and command_ids are passed.
+            Attempted to fetch commands in a DM with a non-bot user.
+        ValueError
+            The limit was not greater than or equal to 0.
+        HTTPException
+            Getting the commands failed.
+        ~discord.Forbidden
+            You do not have permissions to get the commands.
+        ~discord.HTTPException
+            The request to get the commands failed.
+
+        Yields
+        -------
+        :class:`.SlashCommand`
+            A slash command.
+        """
+        return _handle_commands(
+            self,
+            AppCommandType.chat_input,
+            query=query,
+            limit=limit,
+            command_ids=command_ids,
+            application=application,
+            with_applications=with_applications,
+        )
+
+    def user_commands(
+        self,
+        query: Optional[str] = None,
+        *,
+        limit: Optional[int] = None,
+        command_ids: Optional[Collection[int]] = None,
+        application: Optional[Snowflake] = None,
+        with_applications: bool = True,
+    ) -> AsyncIterator[UserCommand]:
+        """Returns a :term:`asynchronous iterator` of the user commands available to use on the user.
+
+        Examples
+        ---------
+
+        Usage ::
+
+            async for command in user.user_commands():
+                print(command.name)
+
+        Flattening into a list ::
+
+            commands = [command async for command in user.user_commands()]
+            # commands is now a list of UserCommand...
+
+        All parameters are optional.
+
+        Parameters
+        ----------
+        query: Optional[:class:`str`]
+            The query to search for. Specifying this limits results to 25 commands max.
+
+            This parameter is faked if ``application`` is specified.
+        limit: Optional[:class:`int`]
+            The maximum number of commands to send back. Defaults to 0 if ``command_ids`` is passed, else 25.
+            If ``None``, returns all commands.
+
+            This parameter is faked if ``application`` is specified.
+        command_ids: Optional[List[:class:`int`]]
+            List of up to 100 command IDs to search for. If the command doesn't exist, it won't be returned.
+
+            If ``limit`` is passed alongside this parameter, this parameter will serve as a "preferred commands" list.
+            This means that the endpoint will return the found commands + up to ``limit`` more, if available.
+        application: Optional[:class:`~discord.abc.Snowflake`]
+            Whether to return this application's commands. Always set to DM recipient in a private channel context.
+        with_applications: :class:`bool`
+            Whether to include applications in the response. Defaults to ``True``.
+
+        Raises
+        ------
+        TypeError
+            Both query and command_ids are passed.
+            Attempted to fetch commands in a DM with a non-bot user.
+        ValueError
+            The limit was not greater than or equal to 0.
+        HTTPException
+            Getting the commands failed.
+        ~discord.Forbidden
+            You do not have permissions to get the commands.
+        ~discord.HTTPException
+            The request to get the commands failed.
+
+        Yields
+        -------
+        :class:`.UserCommand`
+            A user command.
+        """
+        return _handle_commands(
+            self,
+            AppCommandType.user,
+            query=query,
+            limit=limit,
+            command_ids=command_ids,
+            application=application,
+            with_applications=with_applications,
+        )
+
+
+class Connectable(Protocol):
+    """An ABC that details the common operations on a channel that can
+    connect to a voice server.
+
+    The following implement this ABC:
+
+    - :class:`~discord.VoiceChannel`
+    - :class:`~discord.StageChannel`
+    - :class:`~discord.DMChannel`
+    - :class:`~discord.GroupChannel`
+    - :class:`~discord.User`
+    - :class:`~discord.Member`
+    """
+
+    __slots__ = ()
+    _state: ConnectionState
+
+    async def _get_channel(self) -> VocalChannel:
+        raise NotImplementedError
+
+    def _get_voice_client_key(self) -> Tuple[int, str]:
+        raise NotImplementedError
+
+    def _get_voice_state_pair(self) -> Tuple[int, int]:
+        raise NotImplementedError
+
+    async def connect(
+        self,
+        *,
+        timeout: float = 60.0,
+        reconnect: bool = True,
+        cls: Callable[[Client, VocalChannel], T] = VoiceClient,
+        _channel: Optional[Connectable] = None,
+        self_deaf: bool = False,
+        self_mute: bool = False,
+    ) -> T:
+        """|coro|
+
+        Connects to voice and creates a :class:`~discord.VoiceClient` to establish
+        your connection to the voice server.
+
+        Parameters
+        -----------
+        timeout: :class:`float`
+            The timeout in seconds to wait for the voice endpoint.
+        reconnect: :class:`bool`
+            Whether the bot should automatically attempt
+            a reconnect if a part of the handshake fails
+            or the gateway goes down.
+        cls: Type[:class:`~discord.VoiceProtocol`]
+            A type that subclasses :class:`~discord.VoiceProtocol` to connect with.
+            Defaults to :class:`~discord.VoiceClient`.
+        self_mute: :class:`bool`
+            Indicates if the client should be self-muted.
+
+            .. versionadded:: 2.0
+        self_deaf: :class:`bool`
+            Indicates if the client should be self-deafened.
+
+            .. versionadded:: 2.0
+
+        Raises
+        -------
+        asyncio.TimeoutError
+            Could not connect to the voice channel in time.
+        ~discord.ClientException
+            You are already connected to a voice channel.
+        ~discord.opus.OpusNotLoaded
+            The opus library has not been loaded.
+
+        Returns
+        --------
+        :class:`~discord.VoiceProtocol`
+            A voice client that is fully connected to the voice server.
+        """
+
+        key_id, _ = self._get_voice_client_key()
+        state = self._state
+        connectable = _channel or self
+        channel = await connectable._get_channel()
+
+        if state._get_voice_client(key_id):
+            raise ClientException('Already connected to a voice channel')
+
+        voice: T = cls(state.client, channel)
+
+        if not isinstance(voice, VoiceProtocol):
+            raise TypeError('Type must meet VoiceProtocol abstract base class')
+
+        state._add_voice_client(key_id, voice)
+
+        try:
+            await voice.connect(timeout=timeout, reconnect=reconnect, self_deaf=self_deaf, self_mute=self_mute)
+        except asyncio.TimeoutError:
+            try:
+                await voice.disconnect(force=True)
+            except Exception:
+                pass  # We don't care if disconnect failed because connection failed
+            raise  # Re-raise
+
+        return voice
```

### Comparing `discord.py-self-1.9.2/discord/invite.py` & `discord.py-self-2.0.0/discord/calls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,442 +1,495 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .asset import Asset
-from .utils import parse_time, snowflake_time, _get_as_snowflake
-from .object import Object
-from .mixins import Hashable
-from .enums import ChannelType, VerificationLevel, try_enum
-from .errors import InvalidArgument
-
-class PartialInviteChannel:
-    """Represents a "partial" invite channel.
-
-    This model will be given when the user is not part of the
-    guild the :class:`Invite` resolves to.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two partial channels are the same.
-
-        .. describe:: x != y
-
-            Checks if two partial channels are not the same.
-
-        .. describe:: hash(x)
-
-            Return the partial channel's hash.
-
-        .. describe:: str(x)
-
-            Returns the partial channel's name.
-
-    Attributes
-    -----------
-    name: :class:`str`
-        The partial channel's name.
-    id: :class:`int`
-        The partial channel's ID.
-    type: :class:`ChannelType`
-        The partial channel's type.
-    """
-
-    __slots__ = ('id', 'name', 'type')
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop('id')
-        self.name = kwargs.pop('name')
-        self.type = kwargs.pop('type')
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return '<PartialInviteChannel id={0.id} name={0.name} type={0.type!r}>'.format(self)
-
-    @property
-    def mention(self):
-        """:class:`str`: The string that allows you to mention the channel."""
-        return '<#%s>' % self.id
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the channel's creation time in UTC."""
-        return snowflake_time(self.id)
-
-class PartialInviteGuild:
-    """Represents a "partial" invite guild.
-
-    This model will be given when the user is not part of the
-    guild the :class:`Invite` resolves to.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two partial guilds are the same.
-
-        .. describe:: x != y
-
-            Checks if two partial guilds are not the same.
-
-        .. describe:: hash(x)
-
-            Return the partial guild's hash.
-
-        .. describe:: str(x)
-
-            Returns the partial guild's name.
-
-    Attributes
-    -----------
-    name: :class:`str`
-        The partial guild's name.
-    id: :class:`int`
-        The partial guild's ID.
-    verification_level: :class:`VerificationLevel`
-        The partial guild's verification level.
-    features: List[:class:`str`]
-        A list of features the guild has. See :attr:`Guild.features` for more information.
-    icon: Optional[:class:`str`]
-        The partial guild's icon.
-    banner: Optional[:class:`str`]
-        The partial guild's banner.
-    splash: Optional[:class:`str`]
-        The partial guild's invite splash.
-    description: Optional[:class:`str`]
-        The partial guild's description.
-    """
-
-    __slots__ = ('_state', 'features', 'icon', 'banner', 'id', 'name', 'splash',
-                 'verification_level', 'description')
-
-    def __init__(self, state, data, id):
-        self._state = state
-        self.id = id
-        self.name = data['name']
-        self.features = data.get('features', [])
-        self.icon = data.get('icon')
-        self.banner = data.get('banner')
-        self.splash = data.get('splash')
-        self.verification_level = try_enum(VerificationLevel, data.get('verification_level'))
-        self.description = data.get('description')
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return '<{0.__class__.__name__} id={0.id} name={0.name!r} features={0.features} ' \
-               'description={0.description!r}>'.format(self)
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the guild's creation time in UTC."""
-        return snowflake_time(self.id)
-
-    @property
-    def icon_url(self):
-        """:class:`Asset`: Returns the guild's icon asset."""
-        return self.icon_url_as()
-
-    def is_icon_animated(self):
-        """:class:`bool`: Returns ``True`` if the guild has an animated icon.
-
-        .. versionadded:: 1.4
-        """
-        return bool(self.icon and self.icon.startswith('a_'))
-
-    def icon_url_as(self, *, format=None, static_format='webp', size=1024):
-        """The same operation as :meth:`Guild.icon_url_as`.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_icon(self._state, self, format=format, static_format=static_format, size=size)
-
-    @property
-    def banner_url(self):
-        """:class:`Asset`: Returns the guild's banner asset."""
-        return self.banner_url_as()
-
-    def banner_url_as(self, *, format='webp', size=2048):
-        """The same operation as :meth:`Guild.banner_url_as`.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_image(self._state, self.id, self.banner, 'banners', format=format, size=size)
-
-    @property
-    def splash_url(self):
-        """:class:`Asset`: Returns the guild's invite splash asset."""
-        return self.splash_url_as()
-
-    def splash_url_as(self, *, format='webp', size=2048):
-        """The same operation as :meth:`Guild.splash_url_as`.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_image(self._state, self.id, self.splash, 'splashes', format=format, size=size)
-
-class Invite(Hashable):
-    r"""Represents a Discord :class:`Guild` or :class:`abc.GuildChannel` invite.
-
-    Depending on the way this object was created, some of the attributes can
-    have a value of ``None``.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two invites are equal.
-
-        .. describe:: x != y
-
-            Checks if two invites are not equal.
-
-        .. describe:: hash(x)
-
-            Returns the invite hash.
-
-        .. describe:: str(x)
-
-            Returns the invite URL.
-
-    The following table illustrates what methods will obtain the attributes:
-
-    +------------------------------------+----------------------------------------------------------+
-    |             Attribute              |                          Method                          |
-    +====================================+==========================================================+
-    | :attr:`max_age`                    | :meth:`abc.GuildChannel.invites`\, :meth:`Guild.invites` |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`max_uses`                   | :meth:`abc.GuildChannel.invites`\, :meth:`Guild.invites` |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`created_at`                 | :meth:`abc.GuildChannel.invites`\, :meth:`Guild.invites` |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`temporary`                  | :meth:`abc.GuildChannel.invites`\, :meth:`Guild.invites` |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`uses`                       | :meth:`abc.GuildChannel.invites`\, :meth:`Guild.invites` |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`approximate_member_count`   | :meth:`Client.fetch_invite`                              |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`approximate_presence_count` | :meth:`Client.fetch_invite`                              |
-    +------------------------------------+----------------------------------------------------------+
-    | :attr:`expires_at`                 | :meth:`Client.fetch_invite`                              |
-    +------------------------------------+----------------------------------------------------------+
-
-    If it's not in the table above then it is available by all methods.
-
-    Attributes
-    -----------
-    max_age: :class:`int`
-        How long the before the invite expires in seconds.
-        A value of ``0`` indicates that it doesn't expire.
-    code: :class:`str`
-        The URL fragment used for the invite.
-    guild: Optional[Union[:class:`Guild`, :class:`Object`, :class:`PartialInviteGuild`]]
-        The guild the invite is for. Can be ``None`` if it's from a group direct message.
-    revoked: :class:`bool`
-        Indicates if the invite has been revoked.
-    created_at: :class:`datetime.datetime`
-        A datetime object denoting the time the invite was created.
-    temporary: :class:`bool`
-        Indicates that the invite grants temporary membership.
-        If ``True``, members who joined via this invite will be kicked upon disconnect.
-    uses: :class:`int`
-        How many times the invite has been used.
-    max_uses: :class:`int`
-        How many times the invite can be used.
-        A value of ``0`` indicates that it has unlimited uses.
-    inviter: :class:`User`
-        The user who created the invite.
-    approximate_member_count: Optional[:class:`int`]
-        The approximate number of members in the guild.
-    approximate_presence_count: Optional[:class:`int`]
-        The approximate number of members currently active in the guild.
-        This includes idle, dnd, online, and invisible members. Offline members are excluded.
-    channel: Union[:class:`abc.GuildChannel`, :class:`Object`, :class:`PartialInviteChannel`]
-        The channel the invite is for.
-    expires_at: :class:`datetime.datetime`
-        A datetime object denoting when the invite expires.
-        A value of ``0`` indicates that it doesn't expire.
-
-        .. versionadded:: 1.9
-    """
-
-    __slots__ = ('max_age', 'code', 'guild', 'revoked', 'created_at', 'uses',
-                 'temporary', 'max_uses', 'inviter', 'channel', '_state',
-                 'approximate_member_count', 'approximate_presence_count',
-                 'expires_at', '_message_id')
-
-    BASE = 'https://discord.gg'
-
-    def __init__(self, *, state, data):
-        self._state = state
-
-        self.max_age = data.get('max_age')
-        self.expires_at = parse_time(data.get('expires_at'))
-        self.code = data.get('code')
-        self.guild = data.get('guild')
-        self.revoked = data.get('revoked')
-        self.created_at = parse_time(data.get('created_at'))
-        self.temporary = data.get('temporary')
-        self.uses = data.get('uses')
-        self.max_uses = data.get('max_uses')
-        self.approximate_presence_count = data.get('approximate_presence_count')
-        self.approximate_member_count = data.get('approximate_member_count')
-
-        inviter_data = data.get('inviter')
-        self.inviter = None if inviter_data is None else self._state.store_user(inviter_data)
-        self.channel = data.get('channel')
-        self._message_id = data.get('message_id')
-
-    @classmethod
-    def from_incomplete(cls, *, state, data, message_id=None):
-        try:
-            guild_id = int(data['guild']['id'])
-        except KeyError:
-            # If we're here, then this is a group DM
-            guild = None
-        else:
-            guild = state._get_guild(guild_id)
-            if guild is None:
-                # If it's not cached, then it has to be a partial guild
-                guild_data = data['guild']
-                guild = PartialInviteGuild(state, guild_data, guild_id)
-
-        # As far as I know, invites always need a channel
-        # So this should never raise.
-        channel_data = data['channel']
-        channel_id = int(channel_data['id'])
-        channel_type = try_enum(ChannelType, channel_data['type'])
-        channel = PartialInviteChannel(id=channel_id, name=channel_data['name'], type=channel_type)
-        if guild is not None and not isinstance(guild, PartialInviteGuild):
-            # Upgrade the partial data if applicable
-            channel = guild.get_channel(channel_id) or channel
-
-        if message_id:
-            data['message_id'] = message_id
-
-        data['guild'] = guild
-        data['channel'] = channel
-        return cls(state=state, data=data)
-
-    @classmethod
-    def from_gateway(cls, *, state, data):
-        guild_id = _get_as_snowflake(data, 'guild_id')
-        guild = state._get_guild(guild_id)
-        channel_id = _get_as_snowflake(data, 'channel_id')
-        if guild is not None:
-            channel = guild.get_channel(channel_id) or Object(id=channel_id)
-        else:
-            guild = Object(id=guild_id)
-            channel = Object(id=channel_id)
-
-        data['guild'] = guild
-        data['channel'] = channel
-        return cls(state=state, data=data)
-
-    def __str__(self):
-        return self.url
-
-    def __repr__(self):
-        return '<Invite code={0.code!r} guild={0.guild!r} ' \
-                'online={0.approximate_presence_count} ' \
-                'members={0.approximate_member_count}>'.format(self)
-
-    def __hash__(self):
-        return hash(self.code)
-
-    @property
-    def id(self):
-        """:class:`str`: Returns the proper code portion of the invite."""
-        return self.code
-
-    @property
-    def url(self):
-        """:class:`str`: A property that retrieves the invite URL."""
-        return self.BASE + '/' + self.code
-
-    async def use(self):
-        """|coro|
-
-        Uses the invite (joins the guild)
-
-        .. versionadded:: 1.9
-
-        Raises
-        ------
-        :exc:`.HTTPException`
-            Joining the guild failed.
-        :exc:`.InvalidArgument`
-            Tried to join a guild you're already in.
-
-        Returns
-        -------
-        :class:`.PartialInviteGuild`
-            The guild joined. This is not the same guild that is
-            added to cache.
-        """
-
-        state = self._state
-
-        data = await state.http.join_guild(self.code, guild_id=self.guild.id, channel_id=self.channel.id, channel_type=self.channel.type.value, message_id=self._message_id)
-
-        new_member = data.get('new_member', False)
-        if not new_member:
-            raise InvalidArgument('Tried to join a guild you\'re already in.')
-
-        return self.guild
-
-    accept = use
-
-    async def delete(self):
-        """|coro|
-
-        Revokes the instant invite.
-
-        You must have the :attr:`~Permissions.manage_channels` permission to do this.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to revoke invites.
-        NotFound
-            The invite is invalid or expired.
-        HTTPException
-            Revoking the invite failed.
-        """
-
-        await self._state.http.delete_invite(self.code)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+import datetime
+from typing import Callable, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+
+from . import utils
+from .errors import ClientException
+from .utils import cached_slot_property
+from .voice_client import VoiceClient
+
+if TYPE_CHECKING:
+    from . import abc
+    from .abc import T as ConnectReturn
+    from .channel import DMChannel, GroupChannel
+    from .client import Client
+    from .member import VoiceState
+    from .message import Message
+    from .state import ConnectionState
+    from .user import BaseUser, User
+
+    _PrivateChannel = Union[abc.DMChannel, abc.GroupChannel]
+
+__all__ = (
+    'CallMessage',
+    'PrivateCall',
+    'GroupCall',
+)
+
+
+def _running_only(func: Callable):
+    def decorator(self: Call, *args, **kwargs):
+        if self._ended:
+            raise ClientException('Call is over')
+        else:
+            return func(self, *args, **kwargs)
+
+    return decorator
+
+
+class CallMessage:
+    """Represents a group call message from Discord.
+
+    This is only received in cases where the message type is equivalent to
+    :attr:`MessageType.call`.
+
+    Attributes
+    -----------
+    ended_timestamp: Optional[:class:`datetime.datetime`]
+        An aware UTC datetime object that represents the time that the call has ended.
+    participants: List[:class:`User`]
+        A list of users that participated in the call.
+    message: :class:`Message`
+        The message associated with this call message.
+    """
+
+    __slots__ = ('message', 'ended_timestamp', 'participants')
+
+    def __init__(self, message: Message, *, participants: List[User], ended_timestamp: Optional[str]) -> None:
+        self.message = message
+        self.ended_timestamp = utils.parse_time(ended_timestamp)
+        self.participants = participants
+
+    @property
+    def call_ended(self) -> bool:
+        """:class:`bool`: Indicates if the call has ended."""
+        return self.ended_timestamp is not None
+
+    @property
+    def initiator(self) -> User:
+        """:class:`.abc.User`: Returns the user that started the call."""
+        return self.message.author  # type: ignore # Cannot be a Member in private messages
+
+    @property
+    def channel(self) -> _PrivateChannel:
+        """:class:`.abc.PrivateChannel`: The private channel associated with this message."""
+        return self.message.channel  # type: ignore # Can only be a private channel here
+
+    @property
+    def duration(self) -> datetime.timedelta:
+        """Queries the duration of the call.
+
+        If the call has not ended then the current duration will
+        be returned.
+
+        Returns
+        ---------
+        :class:`datetime.timedelta`
+            The timedelta object representing the duration.
+        """
+        if self.ended_timestamp is None:
+            return utils.utcnow() - self.message.created_at
+        else:
+            return self.ended_timestamp - self.message.created_at
+
+
+class PrivateCall:
+    """Represents the actual group call from Discord.
+
+    This is accompanied with a :class:`CallMessage` denoting the information.
+
+    .. versionadded:: 1.9
+
+    Attributes
+    -----------
+    channel: :class:`DMChannel`
+        The channel the call is in.
+    unavailable: :class:`bool`
+        Denotes if this call is unavailable.
+    region: :class:`str`
+        The region the call is being hosted at.
+
+        .. versionchanged:: 2.0
+            The type of this attribute has changed to :class:`str`.
+    """
+
+    __slots__ = ('_state', '_ended', 'channel', '_cs_message', '_ringing', '_message_id', 'region', 'unavailable')
+
+    if TYPE_CHECKING:
+        channel: DMChannel
+
+    def __init__(
+        self,
+        *,
+        data: dict,
+        state: ConnectionState,
+        message: Optional[Message],
+        channel: abc.PrivateChannel,
+    ) -> None:
+        self._state = state
+        self._cs_message = message
+        self.channel = channel  # type: ignore # Will always be a DMChannel here
+        self._ended: bool = False
+
+        self._update(data)
+
+    def _delete(self) -> None:
+        self._ringing = tuple()
+        self._ended = True
+
+    def _get_recipients(self) -> Tuple[BaseUser, ...]:
+        channel = self.channel
+        return channel.me, channel.recipient
+
+    def _is_participating(self, user: BaseUser) -> bool:
+        state = self.voice_state_for(user)
+        return bool(state and state.channel and state.channel.id == self.channel.id)
+
+    def _update(self, data) -> None:
+        self._message_id = int(data['message_id'])
+        self.unavailable = data.get('unavailable', False)
+        try:
+            self.region: str = data['region']
+        except KeyError:
+            pass
+
+        channel = self.channel
+        recipients = self._get_recipients()
+        lookup = {u.id: u for u in recipients}
+        self._ringing = tuple(filter(None, map(lookup.get, data.get('ringing', []))))
+
+        for vs in data.get('voice_states', []):
+            self._state._update_voice_state(vs, channel.id)
+
+    @property
+    def ringing(self) -> List[BaseUser]:
+        """List[:class:`.abc.User`]: A list of users that are currently being rung to join the call."""
+        return list(self._ringing)
+
+    @property
+    def initiator(self) -> Optional[User]:
+        """Optional[:class:`.abc.User`]: Returns the user that started the call. Returns ``None`` if the message is not cached."""
+        return getattr(self.message, 'author', None)
+
+    @property
+    def connected(self) -> bool:
+        """:class:`bool`: Returns whether you're in the call (this does not mean you're in the call through the library)."""
+        return self._is_participating(self.channel.me)
+
+    @property
+    def members(self) -> List[BaseUser]:
+        """List[:class:`.abc.User`]: Returns all users that are currently in this call."""
+        recipients = self._get_recipients()
+        return [u for u in recipients if self._is_participating(u)]
+
+    @property
+    def voice_states(self) -> Dict[int, VoiceState]:
+        """Mapping[:class:`int`, :class:`VoiceState`]: Returns a mapping of user IDs who have voice states in this call."""
+        return {
+            k: v for k, v in self._state._voice_states.items() if bool(v and v.channel and v.channel.id == self.channel.id)
+        }
+
+    @cached_slot_property('_cs_message')
+    def message(self) -> Optional[Message]:
+        """Optional[:class:`Message`]: The message associated with this call. Sometimes may not be cached."""
+        return self._state._get_message(self._message_id)
+
+    async def fetch_message(self) -> Message:
+        """|coro|
+
+        Fetches and caches the message associated with this call.
+
+        Raises
+        -------
+        HTTPException
+            Retrieving the message failed.
+
+        Returns
+        -------
+        :class:`Message`
+            The message associated with this call.
+        """
+        message = await self.channel.fetch_message(self._message_id)
+        state = self._state
+        if self.message is None:
+            if state._messages is not None:
+                state._messages.append(message)
+            self._cs_message = message
+        return message
+
+    async def change_region(self, region: str) -> None:
+        """|coro|
+
+        Changes the channel's voice region.
+
+        Parameters
+        -----------
+        region: :class:`str`
+            A region to change the voice region to.
+
+            .. versionchanged:: 2.0
+                The type of this parameter has changed to :class:`str`.
+
+        Raises
+        -------
+        HTTPException
+            Failed to change the channel's voice region.
+        """
+        await self._state.http.change_call_voice_region(self.channel.id, region)
+
+    @_running_only
+    async def ring(self) -> None:
+        """|coro|
+
+        Rings the other recipient.
+
+        Raises
+        -------
+        Forbidden
+            Not allowed to ring the other recipient.
+        HTTPException
+            Ringing failed.
+        ClientException
+            The call has ended.
+        """
+        channel = self.channel
+        await self._state.http.ring(channel.id)
+
+    @_running_only
+    async def stop_ringing(self) -> None:
+        """|coro|
+
+        Stops ringing the other recipient.
+
+        Raises
+        -------
+        HTTPException
+            Stopping the ringing failed.
+        ClientException
+            The call has ended.
+        """
+        channel = self.channel
+        await self._state.http.stop_ringing(channel.id, channel.recipient.id)
+
+    @_running_only
+    async def connect(
+        self,
+        *,
+        timeout: float = 60.0,
+        reconnect: bool = True,
+        cls: Callable[[Client, abc.VocalChannel], ConnectReturn] = VoiceClient,
+    ) -> ConnectReturn:
+        """|coro|
+
+        Connects to voice and creates a :class:`~discord.VoiceClient` to establish
+        your connection to the voice server.
+
+        There is an alias of this called :attr:`join`.
+
+        Parameters
+        -----------
+        timeout: :class:`float`
+            The timeout in seconds to wait for the voice endpoint.
+        reconnect: :class:`bool`
+            Whether the bot should automatically attempt
+            a reconnect if a part of the handshake fails
+            or the gateway goes down.
+        cls: Type[:class:`~discord.VoiceProtocol`]
+            A type that subclasses :class:`~discord.VoiceProtocol` to connect with.
+            Defaults to :class:`~discord.VoiceClient`.
+
+        Raises
+        -------
+        asyncio.TimeoutError
+            Could not connect to the voice channel in time.
+        ~discord.ClientException
+            You are already connected to a voice channel.
+        ~discord.opus.OpusNotLoaded
+            The opus library has not been loaded.
+
+        Returns
+        --------
+        :class:`~discord.VoiceProtocol`
+            A voice client that is fully connected to the voice server.
+        """
+        return await self.channel.connect(timeout=timeout, reconnect=reconnect, cls=cls, ring=False)
+
+    @_running_only
+    async def join(
+        self,
+        *,
+        timeout: float = 60.0,
+        reconnect: bool = True,
+        cls: Callable[[Client, abc.VocalChannel], ConnectReturn] = VoiceClient,
+    ) -> ConnectReturn:
+        """|coro|
+
+        Connects to voice and creates a :class:`~discord.VoiceClient` to establish
+        your connection to the voice server.
+
+        This is an alias of :attr:`connect`.
+
+        Parameters
+        -----------
+        timeout: :class:`float`
+            The timeout in seconds to wait for the voice endpoint.
+        reconnect: :class:`bool`
+            Whether the bot should automatically attempt
+            a reconnect if a part of the handshake fails
+            or the gateway goes down.
+        cls: Type[:class:`~discord.VoiceProtocol`]
+            A type that subclasses :class:`~discord.VoiceProtocol` to connect with.
+            Defaults to :class:`~discord.VoiceClient`.
+
+        Raises
+        -------
+        asyncio.TimeoutError
+            Could not connect to the voice channel in time.
+        ~discord.ClientException
+            You are already connected to a voice channel.
+        ~discord.opus.OpusNotLoaded
+            The opus library has not been loaded.
+
+        Returns
+        --------
+        :class:`~discord.VoiceProtocol`
+            A voice client that is fully connected to the voice server.
+        """
+        return await self.connect(timeout=timeout, reconnect=reconnect, cls=cls)
+
+    @_running_only
+    async def disconnect(self, force: bool = False) -> None:
+        """|coro|
+
+        Disconnects this voice client from voice.
+
+        There is an alias of this called :attr:`leave`.
+        """
+        state = self._state
+        if not (client := state._get_voice_client(self.channel.me.id)):
+            return
+
+        return await client.disconnect(force=force)
+
+    @_running_only
+    async def leave(self, force: bool = False) -> None:
+        """|coro|
+
+        Disconnects this voice client from voice.
+
+        This is an alias of :attr:`disconnect`.
+        """
+        return await self.disconnect(force=force)
+
+    def voice_state_for(self, user: abc.Snowflake) -> Optional[VoiceState]:
+        """Retrieves the :class:`VoiceState` for a specified :class:`User`.
+
+        If the :class:`User` has no voice state then this function returns
+        ``None``.
+
+        Parameters
+        ------------
+        user: :class:`User`
+            The user to retrieve the voice state for.
+
+        Returns
+        --------
+        Optional[:class:`VoiceState`]
+            The voice state associated with this user.
+        """
+        return self._state._voice_state_for(user.id)
+
+
+class GroupCall(PrivateCall):
+    """Represents a Discord group call.
+
+    This is accompanied with a :class:`CallMessage` denoting the information.
+
+    Attributes
+    -----------
+    channel: :class:`GroupChannel`
+        The channel the group call is in.
+    unavailable: :class:`bool`
+        Denotes if this group call is unavailable.
+    region: :class:`str`
+        The region the group call is being hosted in.
+
+        .. versionchanged:: 2.0
+            The type of this attribute has changed to :class:`str`.
+    """
+
+    __slots__ = ()
+
+    if TYPE_CHECKING:
+        channel: GroupChannel
+
+    def _get_recipients(self) -> Tuple[BaseUser, ...]:
+        channel = self.channel
+        return *channel.recipients, channel.me
+
+    @_running_only
+    async def ring(self, *recipients: abc.Snowflake) -> None:
+        r"""|coro|
+
+        Rings the specified recipients.
+
+        Parameters
+        -----------
+        \*recipients: :class:`User`
+            The recipients to ring. The default is to ring all recipients.
+
+        Raises
+        -------
+        HTTPException
+            Stopping the ringing failed.
+        ClientException
+            The call has ended.
+        """
+        await self._state.http.ring(self.channel.id, *{r.id for r in recipients})
+
+    @_running_only
+    async def stop_ringing(self, *recipients: abc.Snowflake) -> None:
+        r"""|coro|
+
+        Stops ringing the specified recipients.
+
+        Parameters
+        -----------
+        \*recipients: :class:`User`
+            The recipients to stop ringing.
+
+        Raises
+        -------
+        HTTPException
+            Ringing failed.
+        ClientException
+            The call has ended.
+        """
+        channel = self.channel
+        await self._state.http.stop_ringing(channel.id, *{r.id for r in recipients or channel.recipients})
+
+
+Call = Union[PrivateCall, GroupCall]
```

### Comparing `discord.py-self-1.9.2/discord/member.py` & `discord.py-self-2.0.0/discord/player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,890 +1,751 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import datetime
-import inspect
-import itertools
-import sys
-from operator import attrgetter
-
-import discord.abc
-
-from . import utils
-from .user import BaseUser, User
-from .activity import create_activity
-from .permissions import Permissions
-from .enums import RelationshipAction, Status, try_enum
-from .colour import Colour
-from .object import Object
-from .asset import Asset
-
-class VoiceState:
-    """Represents a Discord user's voice state.
-
-    Attributes
-    ------------
-    deaf: :class:`bool`
-        Indicates if the user is currently deafened by the guild.
-    mute: :class:`bool`
-        Indicates if the user is currently muted by the guild.
-    self_mute: :class:`bool`
-        Indicates if the user is currently muted by their own accord.
-    self_deaf: :class:`bool`
-        Indicates if the user is currently deafened by their own accord.
-    self_stream: :class:`bool`
-        Indicates if the user is currently streaming via 'Go Live' feature.
-
-        .. versionadded:: 1.3
-
-    self_video: :class:`bool`
-        Indicates if the user is currently broadcasting video.
-    suppress: :class:`bool`
-        Indicates if the user is suppressed from speaking.
-
-        Only applies to stage channels.
-
-        .. versionadded:: 1.7
-
-    requested_to_speak_at: Optional[:class:`datetime.datetime`]
-        A datetime object that specifies the date and time in UTC that the member
-        requested to speak. It will be ``None`` if they are not requesting to speak
-        anymore or have been accepted to speak.
-
-        Only applicable to stage channels.
-
-        .. versionadded:: 1.7
-
-    afk: :class:`bool`
-        Indicates if the user is currently in the AFK channel in the guild.
-    channel: Optional[Union[:class:`VoiceChannel`, :class:`StageChannel`]]
-        The voice channel that the user is currently connected to. ``None`` if the user
-        is not currently in a voice channel.
-    """
-
-    __slots__ = ('session_id', 'deaf', 'mute', 'self_mute',
-                 'self_stream', 'self_video', 'self_deaf', 'afk', 'channel',
-                 'requested_to_speak_at', 'suppress')
-
-    def __init__(self, *, data, channel=None):
-        self.session_id = data.get('session_id')
-        self._update(data, channel)
-
-    def _update(self, data, channel):
-        self.self_mute = data.get('self_mute', False)
-        self.self_deaf = data.get('self_deaf', False)
-        self.self_stream = data.get('self_stream', False)
-        self.self_video = data.get('self_video', False)
-        self.afk = data.get('suppress', False)
-        self.mute = data.get('mute', False)
-        self.deaf = data.get('deaf', False)
-        self.suppress = data.get('suppress', False)
-        self.requested_to_speak_at = utils.parse_time(data.get('request_to_speak_timestamp'))
-        self.channel = channel
-
-    def __repr__(self):
-        attrs = [
-            ('self_mute', self.self_mute),
-            ('self_deaf', self.self_deaf),
-            ('self_stream', self.self_stream),
-            ('suppress', self.suppress),
-            ('requested_to_speak_at', self.requested_to_speak_at),
-            ('channel', self.channel)
-        ]
-        return '<%s %s>' % (self.__class__.__name__, ' '.join('%s=%r' % t for t in attrs))
-
-def flatten_user(cls):
-    for attr, value in itertools.chain(BaseUser.__dict__.items(), User.__dict__.items()):
-        # ignore private/special methods
-        if attr.startswith('_'):
-            continue
-
-        # don't override what we already have
-        if attr in cls.__dict__:
-            continue
-
-        # if it's a slotted attribute or a property, redirect it
-        # slotted members are implemented as member_descriptors in Type.__dict__
-        if not hasattr(value, '__annotations__'):
-            getter = attrgetter('_user.' + attr)
-            setattr(cls, attr, property(getter, doc='Equivalent to :attr:`User.%s`' % attr))
-        else:
-            # Technically, this can also use attrgetter
-            # However I'm not sure how I feel about "functions" returning properties
-            # It probably breaks something in Sphinx.
-            # probably a member function by now
-            def generate_function(x):
-                # We want sphinx to properly show coroutine functions as coroutines
-                if inspect.iscoroutinefunction(value):
-                    async def general(self, *args, **kwargs):
-                        return await getattr(self._user, x)(*args, **kwargs)
-                else:
-                    def general(self, *args, **kwargs):
-                        return getattr(self._user, x)(*args, **kwargs)
-
-                general.__name__ = x
-                return general
-
-            func = generate_function(attr)
-            func = utils.copy_doc(value)(func)
-            setattr(cls, attr, func)
-
-    return cls
-
-_BaseUser = discord.abc.User
-
-@flatten_user
-class Member(discord.abc.Messageable, _BaseUser):
-    """Represents a Discord member to a :class:`Guild`.
-
-    This implements a lot of the functionality of :class:`User`.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two members are equal.
-            Note that this works with :class:`User` instances too.
-
-        .. describe:: x != y
-
-            Checks if two members are not equal.
-            Note that this works with :class:`User` instances too.
-
-        .. describe:: hash(x)
-
-            Returns the member's hash.
-
-        .. describe:: str(x)
-
-            Returns the member's name with the discriminator.
-
-    Attributes
-    ----------
-    joined_at: Optional[:class:`datetime.datetime`]
-        A datetime object that specifies the date and time in UTC that the member joined the guild.
-        If the member left and rejoined the guild, this will be the latest date. In certain cases, this can be ``None``.
-    activities: Tuple[Union[:class:`BaseActivity`, :class:`Spotify`]]
-        The activities that the user is currently doing.
-
-        .. note::
-
-            Due to a Discord API limitation, a user's Spotify activity may not appear
-            if they are listening to a song with a title longer
-            than 128 characters. See :issue:`1738` for more information.
-
-    guild: :class:`Guild`
-        The guild that the member belongs to.
-    nick: Optional[:class:`str`]
-        The guild specific nickname of the user.
-    pending: :class:`bool`
-        Whether the member is pending member verification.
-
-        .. versionadded:: 1.6
-    premium_since: Optional[:class:`datetime.datetime`]
-        A datetime object that specifies the date and time in UTC when the member used their
-        Nitro boost on the guild, if available. This could be ``None``.
-    guild_avatar: Optional[:class:`str`]
-        The guild avatar hash the member has. Could be None.
-    """
-
-    __slots__ = ('_roles', 'joined_at', 'premium_since', '_client_status',
-                 'activities', 'guild', 'pending', 'nick', '_user', '_state', 'guild_avatar')
-
-    def __init__(self, *, data, guild, state):
-        self._state = state
-        self._user = state.store_user(data['user'])
-        self.guild = guild
-        self.joined_at = utils.parse_time(data.get('joined_at'))
-        self.premium_since = utils.parse_time(data.get('premium_since'))
-        self._update_roles(data)
-        self._client_status = {
-            None: 'offline'
-        }
-        self.activities = tuple(map(create_activity, data.get('activities', [])))
-        self.nick = data.get('nick', None)
-        self.pending = data.get('pending', False)
-        self.guild_avatar = data.get('avatar')
-
-    def __str__(self):
-        return str(self._user)
-
-    def __repr__(self):
-        return '<Member id={1.id} name={1.name!r} discriminator={1.discriminator!r}' \
-               ' bot={1.bot} nick={0.nick!r} guild={0.guild!r}>'.format(self, self._user)
-
-    def __eq__(self, other):
-        return isinstance(other, _BaseUser) and other.id == self.id
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
-        return hash(self._user)
-
-    @classmethod
-    def _from_message(cls, *, message, data):
-        author = message.author
-        data['user'] = author._to_minimal_user_json()
-        return cls(data=data, guild=message.guild, state=message._state)
-
-    def _update_from_message(self, data):
-        self.joined_at = utils.parse_time(data.get('joined_at'))
-        self.premium_since = utils.parse_time(data.get('premium_since'))
-        self._update_roles(data)
-        self.nick = data.get('nick', None)
-        self.pending = data.get('pending', False)
-        self.guild_avatar = data.get('avatar')
-
-    @classmethod
-    def _try_upgrade(cls, *,  data, guild, state):
-        # A User object with a 'member' key
-        try:
-            member_data = data.pop('member')
-        except KeyError:
-            return state.store_user(data)
-        else:
-            member_data['user'] = data
-            return cls(data=member_data, guild=guild, state=state)
-
-    @classmethod
-    def _from_presence_update(cls, *, data, guild, state):
-        clone = cls(data=data, guild=guild, state=state)
-        to_return = cls(data=data, guild=guild, state=state)
-        to_return._client_status = {
-            sys.intern(key): sys.intern(value)
-            for key, value in data.get('client_status', {}).items()
-        }
-        to_return._client_status[None] = sys.intern(data['status'])
-        return to_return, clone
-
-    @classmethod
-    def _copy(cls, member):
-        self = cls.__new__(cls) # to bypass __init__
-
-        self._roles = utils.SnowflakeList(member._roles, is_sorted=True)
-        self.joined_at = member.joined_at
-        self.premium_since = member.premium_since
-        self._client_status = member._client_status.copy()
-        self.guild = member.guild
-        self.nick = member.nick
-        self.pending = member.pending
-        self.activities = member.activities
-        self._state = member._state
-        self.guild_avatar = member.guild_avatar
-
-        # Reference will not be copied unless necessary by PRESENCE_UPDATE
-        # See below
-        self._user = member._user
-        return self
-
-    async def _get_channel(self):
-        ch = await self.create_dm()
-        return ch
-
-    def _update_roles(self, data):
-        self._roles = utils.SnowflakeList(map(int, data['roles']))
-
-    def _update(self, data):
-        # the nickname change is optional,
-        # if it isn't in the payload then it didn't change
-        try:
-            self.nick = data['nick']
-        except KeyError:
-            pass
-
-        try:
-            self.pending = data['pending']
-        except KeyError:
-            pass
-
-        try:
-            self.guild_avatar = data['avatar']
-        except KeyError:
-            pass
-
-        self.premium_since = utils.parse_time(data.get('premium_since'))
-        self._update_roles(data)
-
-    def _presence_update(self, data, user):
-        self.activities = tuple(map(create_activity, data.get('activities', [])))
-        self._client_status = {
-            sys.intern(key): sys.intern(value)
-            for key, value in data.get('client_status', {}).items()
-        }
-        self._client_status[None] = sys.intern(data['status'])
-
-        if len(user) > 1:
-            return self._update_inner_user(user)
-        return False
-
-    def _update_inner_user(self, user):
-        u = self._user
-        original = (u.name, u.avatar, u.discriminator, u._public_flags)
-        # These keys seem to always be available
-        modified = (user['username'], user['avatar'], user['discriminator'], user.get('public_flags', 0))
-        if original != modified:
-            to_return = User._copy(self._user)
-            u.name, u.avatar, u.discriminator, u._public_flags = modified
-            # Signal to dispatch on_user_update
-            return to_return, u
-
-    @property
-    def status(self):
-        """:class:`Status`: The member's overall status. If the value is unknown, then it will be a :class:`str` instead."""
-        return try_enum(Status, self._client_status[None])
-
-    @property
-    def raw_status(self):
-        """:class:`str`: The member's overall status as a string value.
-
-        .. versionadded:: 1.5
-        """
-        return self._client_status[None]
-
-    @status.setter
-    def status(self, value):
-        # internal use only
-        self._client_status[None] = str(value)
-
-    @property
-    def mobile_status(self):
-        """:class:`Status`: The member's status on a mobile device, if applicable."""
-        return try_enum(Status, self._client_status.get('mobile', 'offline'))
-
-    @property
-    def desktop_status(self):
-        """:class:`Status`: The member's status on the desktop client, if applicable."""
-        return try_enum(Status, self._client_status.get('desktop', 'offline'))
-
-    @property
-    def web_status(self):
-        """:class:`Status`: The member's status on the web client, if applicable."""
-        return try_enum(Status, self._client_status.get('web', 'offline'))
-
-    def is_on_mobile(self):
-        """:class:`bool`: A helper function that determines if a member is active on a mobile device."""
-        return 'mobile' in self._client_status
-
-    @property
-    def colour(self):
-        """:class:`Colour`: A property that returns a colour denoting the rendered colour
-        for the member. If the default colour is the one rendered then an instance
-        of :meth:`Colour.default` is returned.
-
-        There is an alias for this named :attr:`color`.
-        """
-
-        roles = self.roles[1:] # remove @everyone
-
-        # highest order of the colour is the one that gets rendered.
-        # if the highest is the default colour then the next one with a colour
-        # is chosen instead
-        for role in reversed(roles):
-            if role.colour.value:
-                return role.colour
-        return Colour.default()
-
-    @property
-    def color(self):
-        """:class:`Colour`: A property that returns a color denoting the rendered color for
-        the member. If the default color is the one rendered then an instance of :meth:`Colour.default`
-        is returned.
-
-        There is an alias for this named :attr:`colour`.
-        """
-        return self.colour
-
-    @property
-    def roles(self):
-        """List[:class:`Role`]: A :class:`list` of :class:`Role` that the member belongs to. Note
-        that the first element of this list is always the default '@everyone'
-        role.
-
-        These roles are sorted by their position in the role hierarchy.
-        """
-        result = []
-        g = self.guild
-        for role_id in self._roles:
-            role = g.get_role(role_id)
-            if role:
-                result.append(role)
-        result.append(g.default_role)
-        result.sort()
-        return result
-
-    @property
-    def mention(self):
-        """:class:`str`: Returns a string that allows you to mention the member."""
-        if self.nick:
-            return '<@!%s>' % self.id
-        return '<@%s>' % self.id
-
-    @property
-    def display_name(self):
-        """:class:`str`: Returns the user's display name.
-
-        For regular users this is just their username, but
-        if they have a guild specific nickname then that
-        is returned instead.
-        """
-        return self.nick or self.name
-
-    @property
-    def activity(self):
-        """Union[:class:`BaseActivity`, :class:`Spotify`]: Returns the primary
-        activity the user is currently doing. Could be ``None`` if no activity is being done.
-
-        .. note::
-
-            Due to a Discord API limitation, this may be ``None`` if 
-            the user is listening to a song on Spotify with a title longer
-            than 128 characters. See :issue:`1738` for more information.
-
-        .. note::
-
-            A user may have multiple activities, these can be accessed under :attr:`activities`.
-        """
-        if self.activities:
-            return self.activities[0]
-
-    def mentioned_in(self, message):
-        """Checks if the member is mentioned in the specified message.
-
-        Parameters
-        -----------
-        message: :class:`Message`
-            The message to check if you're mentioned in.
-
-        Returns
-        -------
-        :class:`bool`
-            Indicates if the member is mentioned in the message.
-        """
-        if message.guild is None or message.guild.id != self.guild.id:
-            return False
-
-        if self._user.mentioned_in(message):
-            return True
-
-        return any(self._roles.has(role.id) for role in message.role_mentions)
-
-    def permissions_in(self, channel):
-        """An alias for :meth:`abc.GuildChannel.permissions_for`.
-
-        Basically equivalent to:
-
-        .. code-block:: python3
-
-            channel.permissions_for(self)
-
-        Parameters
-        -----------
-        channel: :class:`abc.GuildChannel`
-            The channel to check your permissions for.
-
-        Returns
-        -------
-        :class:`Permissions`
-            The resolved permissions for the member.
-        """
-        return channel.permissions_for(self)
-
-    @property
-    def top_role(self):
-        """:class:`Role`: Returns the member's highest role.
-
-        This is useful for figuring where a member stands in the role
-        hierarchy chain.
-        """
-        guild = self.guild
-        if len(self._roles) == 0:
-            return guild.default_role
-
-        return max(guild.get_role(rid) or guild.default_role for rid in self._roles)
-
-    @property
-    def guild_permissions(self):
-        """:class:`Permissions`: Returns the member's guild permissions.
-
-        This only takes into consideration the guild permissions
-        and not most of the implied permissions or any of the
-        channel permission overwrites. For 100% accurate permission
-        calculation, please use either :meth:`permissions_in` or
-        :meth:`abc.GuildChannel.permissions_for`.
-
-        This does take into consideration guild ownership and the
-        administrator implication.
-        """
-
-        if self.guild.owner_id == self.id:
-            return Permissions.all()
-
-        base = Permissions.none()
-        for r in self.roles:
-            base.value |= r.permissions.value
-
-        if base.administrator:
-            return Permissions.all()
-
-        return base
-
-    @property
-    def voice(self):
-        """Optional[:class:`VoiceState`]: Returns the member's current voice state."""
-        return self.guild._voice_state_for(self._user.id)
-
-    @property
-    def guild_avatar_url(self):
-        """:class:`Asset`: Returns an :class:`Asset` for the guild avatar the user has.
-
-        If the user does not have a guild avatar, an asset for
-        the user avatar is returned instead.
-
-        This is equivalent to calling :meth:`guild_avatar_url_as` with
-        the default parameters (i.e. webp/gif detection and a size of 1024).
-        """
-        return self.guild_avatar_url_as(format=None, size=1024)
-
-    def is_guild_avatar_animated(self):
-        """:class:`bool`: Indicates if the user has an animated guild avatar."""
-        return bool(self.guild_avatar and self.guild_avatar.startswith('a_'))
-
-    def guild_avatar_url_as(self, *, format=None, static_format='webp', size=1024):
-        """Returns an :class:`Asset` for the guild avatar the user has.
-
-        If the user does not have a guild avatar, an asset for
-        the user avatar is returned instead.
-
-        The format must be one of 'webp', 'jpeg', 'jpg', 'png' or 'gif', and
-        'gif' is only valid for animated avatars. The size must be a power of 2
-        between 16 and 4096.
-
-        Parameters
-        -----------
-        format: Optional[:class:`str`]
-            The format to attempt to convert the avatar to.
-            If the format is ``None``, then it is automatically
-            detected into either 'gif' or static_format depending on the
-            avatar being animated or not.
-        static_format: Optional[:class:`str`]
-            Format to attempt to convert only non-animated avatars to.
-            Defaults to 'webp'
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or ``static_format``, or
-            invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_guild_avatar(self._state, self, format=format, static_format=static_format, size=size)
-
-    async def ban(self, **kwargs):
-        """|coro|
-
-        Bans this member. Equivalent to :meth:`Guild.ban`.
-        """
-        await self.guild.ban(self, **kwargs)
-
-    async def unban(self):
-        """|coro|
-
-        Unbans this member. Equivalent to :meth:`Guild.unban`.
-        """
-        await self.guild.unban(self)
-
-    async def kick(self, *, reason=None):
-        """|coro|
-
-        Kicks this member. Equivalent to :meth:`Guild.kick`.
-        """
-        await self.guild.kick(self, reason=reason)
-
-    async def edit(self, **fields):
-        """|coro|
-
-        Edits the member's data.
-
-        Depending on the parameter passed, this requires different permissions listed below:
-
-        +---------------+--------------------------------------+
-        |   Parameter   |              Permission              |
-        +---------------+--------------------------------------+
-        | nick          | :attr:`Permissions.manage_nicknames` |
-        +---------------+--------------------------------------+
-        | mute          | :attr:`Permissions.mute_members`     |
-        +---------------+--------------------------------------+
-        | deafen        | :attr:`Permissions.deafen_members`   |
-        +---------------+--------------------------------------+
-        | roles         | :attr:`Permissions.manage_roles`     |
-        +---------------+--------------------------------------+
-        | voice_channel | :attr:`Permissions.move_members`     |
-        +---------------+--------------------------------------+
-
-        All parameters are optional.
-
-        .. versionchanged:: 1.1
-            Can now pass ``None`` to ``voice_channel`` to kick a member from voice.
-
-        Parameters
-        -----------
-        nick: Optional[:class:`str`]
-            The member's new nickname. Use ``None`` to remove the nickname.
-        mute: :class:`bool`
-            Indicates if the member should be guild muted or un-muted.
-        deafen: :class:`bool`
-            Indicates if the member should be guild deafened or un-deafened.
-        suppress: :class:`bool`
-            Indicates if the member should be suppressed in stage channels.
-
-            .. versionadded:: 1.7
-
-        roles: Optional[List[:class:`Role`]]
-            The member's new list of roles. This *replaces* the roles.
-        voice_channel: Optional[:class:`VoiceChannel`]
-            The voice channel to move the member to.
-            Pass ``None`` to kick them from voice.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to the action requested.
-        HTTPException
-            The operation failed.
-        """
-        http = self._state.http
-        guild_id = self.guild.id
-        me = self._state.self_id == self.id
-        payload = {}
-
-        try:
-            nick = fields['nick']
-        except KeyError:
-            # nick not present so...
-            pass
-        else:
-            nick = nick or ''
-            if me:
-                await http.change_my_nickname(guild_id, nick)
-            else:
-                payload['nick'] = nick
-
-        deafen = fields.get('deafen')
-        if deafen is not None:
-            payload['deaf'] = deafen
-
-        mute = fields.get('mute')
-        if mute is not None:
-            payload['mute'] = mute
-
-        suppress = fields.get('suppress')
-        if suppress is not None:
-            voice_state_payload = {
-                'channel_id': self.voice.channel.id,
-                'suppress': suppress,
-            }
-
-            if suppress or self.bot:
-                voice_state_payload['request_to_speak_timestamp'] = None
-
-            if me:
-                await http.edit_my_voice_state(guild_id, voice_state_payload)
-            else:
-                if not suppress:
-                    voice_state_payload['request_to_speak_timestamp'] = datetime.datetime.utcnow().isoformat()
-                await http.edit_voice_state(guild_id, self.id, voice_state_payload)
-
-        try:
-            vc = fields['voice_channel']
-        except KeyError:
-            pass
-        else:
-            payload['channel_id'] = vc and vc.id
-
-        try:
-            roles = fields['roles']
-        except KeyError:
-            pass
-        else:
-            payload['roles'] = tuple(r.id for r in roles)
-
-        if payload:
-            await http.edit_member(guild_id, self.id, **payload)
-
-        # TODO: wait for WS event for modify-in-place behaviour
-
-    async def request_to_speak(self):
-        """|coro|
-
-        Request to speak in the connected channel.
-
-        Only applies to stage channels.
-
-        .. note::
-
-            Requesting members that are not the client is equivalent
-            to :attr:`.edit` providing ``suppress`` as ``False``.
-
-        .. versionadded:: 1.7
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to the action requested.
-        HTTPException
-            The operation failed.
-        """
-        payload = {
-            'channel_id': self.voice.channel.id,
-            'request_to_speak_timestamp': datetime.datetime.utcnow().isoformat(),
-        }
-
-        if self._state.self_id != self.id:
-            payload['suppress'] = False
-            await self._state.http.edit_voice_state(self.guild.id, self.id, payload)
-        else:
-            await self._state.http.edit_my_voice_state(self.guild.id, payload)
-
-    async def move_to(self, channel):
-        """|coro|
-
-        Moves a member to a new voice channel (they must be connected first).
-
-        You must have the :attr:`~Permissions.move_members` permission to
-        use this.
-
-        This raises the same exceptions as :meth:`edit`.
-
-        .. versionchanged:: 1.1
-            Can now pass ``None`` to kick a member from voice.
-
-        Parameters
-        -----------
-        channel: Optional[:class:`VoiceChannel`]
-            The new voice channel to move the member to.
-            Pass ``None`` to kick them from voice.
-        """
-        await self.edit(voice_channel=channel)
-
-    async def add_roles(self, *roles, atomic=True):
-        r"""|coro|
-
-        Gives the member a number of :class:`Role`\s.
-
-        You must have the :attr:`~Permissions.manage_roles` permission to
-        use this, and the added :class:`Role`\s must appear lower in the list
-        of roles than the highest role of the member.
-
-        Parameters
-        -----------
-        \*roles: :class:`abc.Snowflake`
-            An argument list of :class:`abc.Snowflake` representing a :class:`Role`
-            to give to the member.
-        atomic: :class:`bool`
-            Whether to atomically add roles. This will ensure that multiple
-            operations will always be applied regardless of the current
-            state of the cache.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to add these roles.
-        HTTPException
-            Adding roles failed.
-        """
-
-        if not atomic:
-            new_roles = utils._unique(Object(id=r.id) for s in (self.roles[1:], roles) for r in s)
-            await self.edit(roles=new_roles)
-        else:
-            req = self._state.http.add_role
-            guild_id = self.guild.id
-            user_id = self.id
-            for role in roles:
-                await req(guild_id, user_id, role.id)
-
-    async def remove_roles(self, *roles, atomic=True):
-        r"""|coro|
-
-        Removes :class:`Role`\s from this member.
-
-        You must have the :attr:`~Permissions.manage_roles` permission to
-        use this, and the removed :class:`Role`\s must appear lower in the list
-        of roles than the highest role of the member.
-
-        Parameters
-        -----------
-        \*roles: :class:`abc.Snowflake`
-            An argument list of :class:`abc.Snowflake` representing a :class:`Role`
-            to remove from the member.
-        atomic: :class:`bool`
-            Whether to atomically remove roles. This will ensure that multiple
-            operations will always be applied regardless of the current
-            state of the cache.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to remove these roles.
-        HTTPException
-            Removing the roles failed.
-        """
-
-        if not atomic:
-            new_roles = [Object(id=r.id) for r in self.roles[1:]] # remove @everyone
-            for role in roles:
-                try:
-                    new_roles.remove(Object(id=role.id))
-                except ValueError:
-                    pass
-
-            await self.edit(roles=new_roles)
-        else:
-            req = self._state.http.remove_role
-            guild_id = self.guild.id
-            user_id = self.id
-            for role in roles:
-                await req(guild_id, user_id, role.id)
-
-    async def send_friend_request(self):
-        """|coro|
-
-        Sends the member a friend request.
-
-        Raises
-        -------
-        Forbidden
-            Not allowed to send a friend request to the member.
-        HTTPException
-            Sending the friend request failed.
-        """
-        await self._state.http.add_relationship(self._user.id, action=RelationshipAction.send_friend_request)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+import threading
+import subprocess
+import audioop
+import asyncio
+import logging
+import shlex
+import time
+import json
+import sys
+import re
+import io
+
+from typing import Any, Callable, Generic, IO, Optional, TYPE_CHECKING, Tuple, TypeVar, Union
+
+from .enums import SpeakingState
+from .errors import ClientException
+from .opus import Encoder as OpusEncoder
+from .oggparse import OggStream
+from .utils import MISSING
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    from .voice_client import VoiceClient
+
+
+AT = TypeVar('AT', bound='AudioSource')
+
+_log = logging.getLogger(__name__)
+
+__all__ = (
+    'AudioSource',
+    'PCMAudio',
+    'FFmpegAudio',
+    'FFmpegPCMAudio',
+    'FFmpegOpusAudio',
+    'PCMVolumeTransformer',
+)
+
+CREATE_NO_WINDOW: int
+
+if sys.platform != 'win32':
+    CREATE_NO_WINDOW = 0
+else:
+    CREATE_NO_WINDOW = 0x08000000
+
+
+class AudioSource:
+    """Represents an audio stream.
+
+    The audio stream can be Opus encoded or not, however if the audio stream
+    is not Opus encoded then the audio format must be 16-bit 48KHz stereo PCM.
+
+    .. warning::
+
+        The audio source reads are done in a separate thread.
+    """
+
+    def read(self) -> bytes:
+        """Reads 20ms worth of audio.
+
+        Subclasses must implement this.
+
+        If the audio is complete, then returning an empty
+        :term:`py:bytes-like object` to signal this is the way to do so.
+
+        If :meth:`~AudioSource.is_opus` method returns ``True``, then it must return
+        20ms worth of Opus encoded audio. Otherwise, it must be 20ms
+        worth of 16-bit 48KHz stereo PCM, which is about 3,840 bytes
+        per frame (20ms worth of audio).
+
+        Returns
+        --------
+        :class:`bytes`
+            A bytes like object that represents the PCM or Opus data.
+        """
+        raise NotImplementedError
+
+    def is_opus(self) -> bool:
+        """Checks if the audio source is already encoded in Opus."""
+        return False
+
+    def cleanup(self) -> None:
+        """Called when clean-up is needed to be done.
+
+        Useful for clearing buffer data or processes after
+        it is done playing audio.
+        """
+        pass
+
+    def __del__(self) -> None:
+        self.cleanup()
+
+
+class PCMAudio(AudioSource):
+    """Represents raw 16-bit 48KHz stereo PCM audio source.
+
+    Attributes
+    -----------
+    stream: :term:`py:file object`
+        A file-like object that reads byte data representing raw PCM.
+    """
+
+    def __init__(self, stream: io.BufferedIOBase) -> None:
+        self.stream: io.BufferedIOBase = stream
+
+    def read(self) -> bytes:
+        ret = self.stream.read(OpusEncoder.FRAME_SIZE)
+        if len(ret) != OpusEncoder.FRAME_SIZE:
+            return b''
+        return ret
+
+
+class FFmpegAudio(AudioSource):
+    """Represents an FFmpeg (or AVConv) based AudioSource.
+
+    User created AudioSources using FFmpeg differently from how :class:`FFmpegPCMAudio` and
+    :class:`FFmpegOpusAudio` work should subclass this.
+
+    .. versionadded:: 1.3
+    """
+
+    def __init__(
+        self,
+        source: Union[str, io.BufferedIOBase],
+        *,
+        executable: str = 'ffmpeg',
+        args: Any,
+        **subprocess_kwargs: Any,
+    ):
+        piping = subprocess_kwargs.get('stdin') == subprocess.PIPE
+        if piping and isinstance(source, str):
+            raise TypeError("parameter conflict: 'source' parameter cannot be a string when piping to stdin")
+
+        args = [executable, *args]
+        kwargs = {'stdout': subprocess.PIPE}
+        kwargs.update(subprocess_kwargs)
+
+        # Ensure attribute is assigned even in the case of errors
+        self._process: subprocess.Popen = MISSING
+        self._process = self._spawn_process(args, **kwargs)
+        self._stdout: IO[bytes] = self._process.stdout  # type: ignore # process stdout is explicitly set
+        self._stdin: Optional[IO[bytes]] = None
+        self._pipe_thread: Optional[threading.Thread] = None
+
+        if piping:
+            n = f'popen-stdin-writer:{id(self):#x}'
+            self._stdin = self._process.stdin
+            self._pipe_thread = threading.Thread(target=self._pipe_writer, args=(source,), daemon=True, name=n)
+            self._pipe_thread.start()
+
+    def _spawn_process(self, args: Any, **subprocess_kwargs: Any) -> subprocess.Popen:
+        process = None
+        try:
+            process = subprocess.Popen(args, creationflags=CREATE_NO_WINDOW, **subprocess_kwargs)
+        except FileNotFoundError:
+            executable = args.partition(' ')[0] if isinstance(args, str) else args[0]
+            raise ClientException(executable + ' was not found.') from None
+        except subprocess.SubprocessError as exc:
+            raise ClientException(f'Popen failed: {exc.__class__.__name__}: {exc}') from exc
+        else:
+            return process
+
+    def _kill_process(self) -> None:
+        proc = self._process
+        if proc is MISSING:
+            return
+
+        _log.debug('Preparing to terminate ffmpeg process %s.', proc.pid)
+
+        try:
+            proc.kill()
+        except Exception:
+            _log.exception('Ignoring error attempting to kill ffmpeg process %s.', proc.pid)
+
+        if proc.poll() is None:
+            _log.info('ffmpeg process %s has not terminated. Waiting to terminate...', proc.pid)
+            proc.communicate()
+            _log.info('ffmpeg process %s should have terminated with a return code of %s.', proc.pid, proc.returncode)
+        else:
+            _log.info('ffmpeg process %s successfully terminated with return code of %s.', proc.pid, proc.returncode)
+
+    def _pipe_writer(self, source: io.BufferedIOBase) -> None:
+        while self._process:
+            # arbitrarily large read size
+            data = source.read(8192)
+            if not data:
+                self._process.terminate()
+                return
+            try:
+                if self._stdin is not None:
+                    self._stdin.write(data)
+            except Exception:
+                _log.debug('Write error for %s, this is probably not a problem.', self, exc_info=True)
+                # at this point the source data is either exhausted or the process is fubar
+                self._process.terminate()
+                return
+
+    def cleanup(self) -> None:
+        self._kill_process()
+        self._process = self._stdout = self._stdin = MISSING
+
+
+class FFmpegPCMAudio(FFmpegAudio):
+    """An audio source from FFmpeg (or AVConv).
+
+    This launches a sub-process to a specific input file given.
+
+    .. warning::
+
+        You must have the ffmpeg or avconv executable in your path environment
+        variable in order for this to work.
+
+    Parameters
+    ------------
+    source: Union[:class:`str`, :class:`io.BufferedIOBase`]
+        The input that ffmpeg will take and convert to PCM bytes.
+        If ``pipe`` is ``True`` then this is a file-like object that is
+        passed to the stdin of ffmpeg.
+    executable: :class:`str`
+        The executable name (and path) to use. Defaults to ``ffmpeg``.
+    pipe: :class:`bool`
+        If ``True``, denotes that ``source`` parameter will be passed
+        to the stdin of ffmpeg. Defaults to ``False``.
+    stderr: Optional[:term:`py:file object`]
+        A file-like object to pass to the Popen constructor.
+        Could also be an instance of ``subprocess.PIPE``.
+    before_options: Optional[:class:`str`]
+        Extra command line arguments to pass to ffmpeg before the ``-i`` flag.
+    options: Optional[:class:`str`]
+        Extra command line arguments to pass to ffmpeg after the ``-i`` flag.
+
+    Raises
+    --------
+    ClientException
+        The subprocess failed to be created.
+    """
+
+    def __init__(
+        self,
+        source: Union[str, io.BufferedIOBase],
+        *,
+        executable: str = 'ffmpeg',
+        pipe: bool = False,
+        stderr: Optional[IO[str]] = None,
+        before_options: Optional[str] = None,
+        options: Optional[str] = None,
+    ) -> None:
+        args = []
+        subprocess_kwargs = {'stdin': subprocess.PIPE if pipe else subprocess.DEVNULL, 'stderr': stderr}
+
+        if isinstance(before_options, str):
+            args.extend(shlex.split(before_options))
+
+        args.append('-i')
+        args.append('-' if pipe else source)
+        args.extend(('-f', 's16le', '-ar', '48000', '-ac', '2', '-loglevel', 'warning'))
+
+        if isinstance(options, str):
+            args.extend(shlex.split(options))
+
+        args.append('pipe:1')
+
+        super().__init__(source, executable=executable, args=args, **subprocess_kwargs)
+
+    def read(self) -> bytes:
+        ret = self._stdout.read(OpusEncoder.FRAME_SIZE)
+        if len(ret) != OpusEncoder.FRAME_SIZE:
+            return b''
+        return ret
+
+    def is_opus(self) -> bool:
+        return False
+
+
+class FFmpegOpusAudio(FFmpegAudio):
+    """An audio source from FFmpeg (or AVConv).
+
+    This launches a sub-process to a specific input file given.  However, rather than
+    producing PCM packets like :class:`FFmpegPCMAudio` does that need to be encoded to
+    Opus, this class produces Opus packets, skipping the encoding step done by the library.
+
+    Alternatively, instead of instantiating this class directly, you can use
+    :meth:`FFmpegOpusAudio.from_probe` to probe for bitrate and codec information.  This
+    can be used to opportunistically skip pointless re-encoding of existing Opus audio data
+    for a boost in performance at the cost of a short initial delay to gather the information.
+    The same can be achieved by passing ``copy`` to the ``codec`` parameter, but only if you
+    know that the input source is Opus encoded beforehand.
+
+    .. versionadded:: 1.3
+
+    .. warning::
+
+        You must have the ffmpeg or avconv executable in your path environment
+        variable in order for this to work.
+
+    Parameters
+    ------------
+    source: Union[:class:`str`, :class:`io.BufferedIOBase`]
+        The input that ffmpeg will take and convert to Opus bytes.
+        If ``pipe`` is ``True`` then this is a file-like object that is
+        passed to the stdin of ffmpeg.
+    bitrate: :class:`int`
+        The bitrate in kbps to encode the output to.  Defaults to ``128``.
+    codec: Optional[:class:`str`]
+        The codec to use to encode the audio data.  Normally this would be
+        just ``libopus``, but is used by :meth:`FFmpegOpusAudio.from_probe` to
+        opportunistically skip pointlessly re-encoding Opus audio data by passing
+        ``copy`` as the codec value.  Any values other than ``copy``, ``opus``, or
+        ``libopus`` will be considered ``libopus``.  Defaults to ``libopus``.
+
+        .. warning::
+
+            Do not provide this parameter unless you are certain that the audio input is
+            already Opus encoded.  For typical use :meth:`FFmpegOpusAudio.from_probe`
+            should be used to determine the proper value for this parameter.
+
+    executable: :class:`str`
+        The executable name (and path) to use. Defaults to ``ffmpeg``.
+    pipe: :class:`bool`
+        If ``True``, denotes that ``source`` parameter will be passed
+        to the stdin of ffmpeg. Defaults to ``False``.
+    stderr: Optional[:term:`py:file object`]
+        A file-like object to pass to the Popen constructor.
+        Could also be an instance of ``subprocess.PIPE``.
+    before_options: Optional[:class:`str`]
+        Extra command line arguments to pass to ffmpeg before the ``-i`` flag.
+    options: Optional[:class:`str`]
+        Extra command line arguments to pass to ffmpeg after the ``-i`` flag.
+
+    Raises
+    --------
+    ClientException
+        The subprocess failed to be created.
+    """
+
+    def __init__(
+        self,
+        source: Union[str, io.BufferedIOBase],
+        *,
+        bitrate: Optional[int] = None,
+        codec: Optional[str] = None,
+        executable: str = 'ffmpeg',
+        pipe: bool = False,
+        stderr: Optional[IO[bytes]] = None,
+        before_options: Optional[str] = None,
+        options: Optional[str] = None,
+    ) -> None:
+        args = []
+        subprocess_kwargs = {'stdin': subprocess.PIPE if pipe else subprocess.DEVNULL, 'stderr': stderr}
+
+        if isinstance(before_options, str):
+            args.extend(shlex.split(before_options))
+
+        args.append('-i')
+        args.append('-' if pipe else source)
+
+        codec = 'copy' if codec in ('opus', 'libopus') else 'libopus'
+        bitrate = bitrate if bitrate is not None else 128
+
+        # fmt: off
+        args.extend(('-map_metadata', '-1',
+                     '-f', 'opus',
+                     '-c:a', codec,
+                     '-ar', '48000',
+                     '-ac', '2',
+                     '-b:a', f'{bitrate}k',
+                     '-loglevel', 'warning'))
+        # fmt: on
+
+        if isinstance(options, str):
+            args.extend(shlex.split(options))
+
+        args.append('pipe:1')
+
+        super().__init__(source, executable=executable, args=args, **subprocess_kwargs)
+        self._packet_iter = OggStream(self._stdout).iter_packets()
+
+    @classmethod
+    async def from_probe(
+        cls,
+        source: str,
+        *,
+        method: Optional[Union[str, Callable[[str, str], Tuple[Optional[str], Optional[int]]]]] = None,
+        **kwargs: Any,
+    ) -> Self:
+        """|coro|
+
+        A factory method that creates a :class:`FFmpegOpusAudio` after probing
+        the input source for audio codec and bitrate information.
+
+        Examples
+        ----------
+
+        Use this function to create an :class:`FFmpegOpusAudio` instance instead of the constructor: ::
+
+            source = await discord.FFmpegOpusAudio.from_probe("song.webm")
+            voice_client.play(source)
+
+        If you are on Windows and don't have ffprobe installed, use the ``fallback`` method
+        to probe using ffmpeg instead: ::
+
+            source = await discord.FFmpegOpusAudio.from_probe("song.webm", method='fallback')
+            voice_client.play(source)
+
+        Using a custom method of determining codec and bitrate: ::
+
+            def custom_probe(source, executable):
+                # some analysis code here
+                return codec, bitrate
+
+            source = await discord.FFmpegOpusAudio.from_probe("song.webm", method=custom_probe)
+            voice_client.play(source)
+
+        Parameters
+        ------------
+        source
+            Identical to the ``source`` parameter for the constructor.
+        method: Optional[Union[:class:`str`, Callable[:class:`str`, :class:`str`]]]
+            The probing method used to determine bitrate and codec information. As a string, valid
+            values are ``native`` to use ffprobe (or avprobe) and ``fallback`` to use ffmpeg
+            (or avconv).  As a callable, it must take two string arguments, ``source`` and
+            ``executable``.  Both parameters are the same values passed to this factory function.
+            ``executable`` will default to ``ffmpeg`` if not provided as a keyword argument.
+        kwargs
+            The remaining parameters to be passed to the :class:`FFmpegOpusAudio` constructor,
+            excluding ``bitrate`` and ``codec``.
+
+        Raises
+        --------
+        AttributeError
+            Invalid probe method, must be ``'native'`` or ``'fallback'``.
+        TypeError
+            Invalid value for ``probe`` parameter, must be :class:`str` or a callable.
+
+        Returns
+        --------
+        :class:`FFmpegOpusAudio`
+            An instance of this class.
+        """
+
+        executable = kwargs.get('executable')
+        codec, bitrate = await cls.probe(source, method=method, executable=executable)
+        return cls(source, bitrate=bitrate, codec=codec, **kwargs)
+
+    @classmethod
+    async def probe(
+        cls,
+        source: str,
+        *,
+        method: Optional[Union[str, Callable[[str, str], Tuple[Optional[str], Optional[int]]]]] = None,
+        executable: Optional[str] = None,
+    ) -> Tuple[Optional[str], Optional[int]]:
+        """|coro|
+
+        Probes the input source for bitrate and codec information.
+
+        Parameters
+        ------------
+        source
+            Identical to the ``source`` parameter for :class:`FFmpegOpusAudio`.
+        method
+            Identical to the ``method`` parameter for :meth:`FFmpegOpusAudio.from_probe`.
+        executable: :class:`str`
+            Identical to the ``executable`` parameter for :class:`FFmpegOpusAudio`.
+
+        Raises
+        --------
+        AttributeError
+            Invalid probe method, must be ``'native'`` or ``'fallback'``.
+        TypeError
+            Invalid value for ``probe`` parameter, must be :class:`str` or a callable.
+
+        Returns
+        ---------
+        Optional[Tuple[Optional[:class:`str`], :class:`int`]]
+            A 2-tuple with the codec and bitrate of the input source.
+        """
+
+        method = method or 'native'
+        executable = executable or 'ffmpeg'
+        probefunc = fallback = None
+
+        if isinstance(method, str):
+            probefunc = getattr(cls, '_probe_codec_' + method, None)
+            if probefunc is None:
+                raise AttributeError(f'Invalid probe method {method!r}.')
+
+            if probefunc is cls._probe_codec_native:
+                fallback = cls._probe_codec_fallback
+
+        elif callable(method):
+            probefunc = method
+            fallback = cls._probe_codec_fallback
+        else:
+            raise TypeError(f"Expected str or callable for parameter 'probe', not '{method.__class__.__name__}'")
+
+        codec = bitrate = None
+        loop = asyncio.get_running_loop()
+        try:
+            codec, bitrate = await loop.run_in_executor(None, lambda: probefunc(source, executable))
+        except Exception:
+            if not fallback:
+                _log.exception("Probe '%s' using '%s' failed.", method, executable)
+                return  # type: ignore
+
+            _log.exception("Probe '%s' using '%s' failed, trying fallback.", method, executable)
+            try:
+                codec, bitrate = await loop.run_in_executor(None, lambda: fallback(source, executable))
+            except Exception:
+                _log.exception("Fallback probe using '%s' failed.", executable)
+            else:
+                _log.debug('Fallback probe found codec=%s, bitrate=%s.', codec, bitrate)
+        else:
+            _log.debug('Probe found codec=%s, bitrate=%s.', codec, bitrate)
+        finally:
+            return codec, bitrate
+
+    @staticmethod
+    def _probe_codec_native(source, executable: str = 'ffmpeg') -> Tuple[Optional[str], Optional[int]]:
+        exe = executable[:2] + 'probe' if executable in ('ffmpeg', 'avconv') else executable
+        args = [exe, '-v', 'quiet', '-print_format', 'json', '-show_streams', '-select_streams', 'a:0', source]
+        output = subprocess.check_output(args, timeout=20)
+        codec = bitrate = None
+
+        if output:
+            data = json.loads(output)
+            streamdata = data['streams'][0]
+
+            codec = streamdata.get('codec_name')
+            bitrate = int(streamdata.get('bit_rate', 0))
+            bitrate = max(round(bitrate / 1000), 512)
+
+        return codec, bitrate
+
+    @staticmethod
+    def _probe_codec_fallback(source, executable: str = 'ffmpeg') -> Tuple[Optional[str], Optional[int]]:
+        args = [executable, '-hide_banner', '-i', source]
+        proc = subprocess.Popen(args, creationflags=CREATE_NO_WINDOW, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        out, _ = proc.communicate(timeout=20)
+        output = out.decode('utf8')
+        codec = bitrate = None
+
+        codec_match = re.search(r"Stream #0.*?Audio: (\w+)", output)
+        if codec_match:
+            codec = codec_match.group(1)
+
+        br_match = re.search(r"(\d+) [kK]b/s", output)
+        if br_match:
+            bitrate = max(int(br_match.group(1)), 512)
+
+        return codec, bitrate
+
+    def read(self) -> bytes:
+        return next(self._packet_iter, b'')
+
+    def is_opus(self) -> bool:
+        return True
+
+
+class PCMVolumeTransformer(AudioSource, Generic[AT]):
+    """Transforms a previous :class:`AudioSource` to have volume controls.
+
+    This does not work on audio sources that have :meth:`AudioSource.is_opus`
+    set to ``True``.
+
+    Parameters
+    ------------
+    original: :class:`AudioSource`
+        The original AudioSource to transform.
+    volume: :class:`float`
+        The initial volume to set it to.
+        See :attr:`volume` for more info.
+
+    Raises
+    -------
+    TypeError
+        Not an audio source.
+    ClientException
+        The audio source is opus encoded.
+    """
+
+    def __init__(self, original: AT, volume: float = 1.0):
+        if not isinstance(original, AudioSource):
+            raise TypeError(f'expected AudioSource not {original.__class__.__name__}.')
+
+        if original.is_opus():
+            raise ClientException('AudioSource must not be Opus encoded.')
+
+        self.original: AT = original
+        self.volume = volume
+
+    @property
+    def volume(self) -> float:
+        """Retrieves or sets the volume as a floating point percentage (e.g. ``1.0`` for 100%)."""
+        return self._volume
+
+    @volume.setter
+    def volume(self, value: float) -> None:
+        self._volume = max(value, 0.0)
+
+    def cleanup(self) -> None:
+        self.original.cleanup()
+
+    def read(self) -> bytes:
+        ret = self.original.read()
+        return audioop.mul(ret, 2, min(self._volume, 2.0))
+
+
+class AudioPlayer(threading.Thread):
+    DELAY: float = OpusEncoder.FRAME_LENGTH / 1000.0
+
+    def __init__(
+        self,
+        source: AudioSource,
+        client: VoiceClient,
+        *,
+        after: Optional[Callable[[Optional[Exception]], Any]] = None,
+    ) -> None:
+        threading.Thread.__init__(self)
+        self.daemon: bool = True
+        self.source: AudioSource = source
+        self.client: VoiceClient = client
+        self.after: Optional[Callable[[Optional[Exception]], Any]] = after
+
+        self._end: threading.Event = threading.Event()
+        self._resumed: threading.Event = threading.Event()
+        self._resumed.set()  # we are not paused
+        self._current_error: Optional[Exception] = None
+        self._connected: threading.Event = client._connected
+        self._lock: threading.Lock = threading.Lock()
+
+        if after is not None and not callable(after):
+            raise TypeError('Expected a callable for the "after" parameter.')
+
+    def _do_run(self) -> None:
+        self.loops = 0
+        self._start = time.perf_counter()
+
+        # getattr lookup speed ups
+        play_audio = self.client.send_audio_packet
+        self._speak(SpeakingState.voice)
+
+        while not self._end.is_set():
+            # are we paused?
+            if not self._resumed.is_set():
+                # wait until we aren't
+                self._resumed.wait()
+                continue
+
+            # are we disconnected from voice?
+            if not self._connected.is_set():
+                # wait until we are connected
+                self._connected.wait()
+                # reset our internal data
+                self.loops = 0
+                self._start = time.perf_counter()
+
+            self.loops += 1
+            data = self.source.read()
+
+            if not data:
+                self.stop()
+                break
+
+            play_audio(data, encode=not self.source.is_opus())
+            next_time = self._start + self.DELAY * self.loops
+            delay = max(0, self.DELAY + (next_time - time.perf_counter()))
+            time.sleep(delay)
+
+    def run(self) -> None:
+        try:
+            self._do_run()
+        except Exception as exc:
+            self._current_error = exc
+            self.stop()
+        finally:
+            self._call_after()
+            self.source.cleanup()
+
+    def _call_after(self) -> None:
+        error = self._current_error
+
+        if self.after is not None:
+            try:
+                self.after(error)
+            except Exception as exc:
+                exc.__context__ = error
+                _log.exception('Calling the after function failed.', exc_info=exc)
+        elif error:
+            _log.exception('Exception in voice thread %s.', self.name, exc_info=error)
+
+    def stop(self) -> None:
+        self._end.set()
+        self._resumed.set()
+        self._speak(SpeakingState.none)
+
+    def pause(self, *, update_speaking: bool = True) -> None:
+        self._resumed.clear()
+        if update_speaking:
+            self._speak(SpeakingState.none)
+
+    def resume(self, *, update_speaking: bool = True) -> None:
+        self.loops: int = 0
+        self._start: float = time.perf_counter()
+        self._resumed.set()
+        if update_speaking:
+            self._speak(SpeakingState.voice)
+
+    def is_playing(self) -> bool:
+        return self._resumed.is_set() and not self._end.is_set()
+
+    def is_paused(self) -> bool:
+        return not self._end.is_set() and not self._resumed.is_set()
+
+    def _set_source(self, source: AudioSource) -> None:
+        with self._lock:
+            self.pause(update_speaking=False)
+            self.source = source
+            self.resume(update_speaking=False)
+
+    def _speak(self, speaking: SpeakingState) -> None:
+        try:
+            asyncio.run_coroutine_threadsafe(self.client.ws.speak(speaking), self.client.client.loop)
+        except Exception:
+            _log.exception('Speaking call in player failed.')
```

### Comparing `discord.py-self-1.9.2/discord/mentions.py` & `discord.py-self-2.0.0/discord/mentions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,153 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-class _FakeBool:
-    def __repr__(self):
-        return 'True'
-
-    def __eq__(self, other):
-        return other is True
-
-    def __bool__(self):
-        return True
-
-default = _FakeBool()
-
-class AllowedMentions:
-    """A class that represents what mentions are allowed in a message.
-
-    This class can be set during :class:`Client` initialisation to apply
-    to every message sent. It can also be applied on a per message basis
-    via :meth:`abc.Messageable.send` for more fine-grained control.
-
-    Attributes
-    ------------
-    everyone: :class:`bool`
-        Whether to allow everyone and here mentions. Defaults to ``True``.
-    users: Union[:class:`bool`, List[:class:`abc.Snowflake`]]
-        Controls the users being mentioned. If ``True`` (the default) then
-        users are mentioned based on the message content. If ``False`` then
-        users are not mentioned at all. If a list of :class:`abc.Snowflake`
-        is given then only the users provided will be mentioned, provided those
-        users are in the message content.
-    roles: Union[:class:`bool`, List[:class:`abc.Snowflake`]]
-        Controls the roles being mentioned. If ``True`` (the default) then
-        roles are mentioned based on the message content. If ``False`` then
-        roles are not mentioned at all. If a list of :class:`abc.Snowflake`
-        is given then only the roles provided will be mentioned, provided those
-        roles are in the message content.
-    replied_user: :class:`bool`
-        Whether to mention the author of the message being replied to. Defaults
-        to ``True``.
-
-        .. versionadded:: 1.6
-    """
-
-    __slots__ = ('everyone', 'users', 'roles', 'replied_user')
-
-    def __init__(self, *, everyone=default, users=default, roles=default, replied_user=default):
-        self.everyone = everyone
-        self.users = users
-        self.roles = roles
-        self.replied_user = replied_user
-
-    @classmethod
-    def all(cls):
-        """A factory method that returns a :class:`AllowedMentions` with all fields explicitly set to ``True``
-
-        .. versionadded:: 1.5
-        """
-        return cls(everyone=True, users=True, roles=True, replied_user=True)
-
-    @classmethod
-    def none(cls):
-        """A factory method that returns a :class:`AllowedMentions` with all fields set to ``False``
-
-        .. versionadded:: 1.5
-        """
-        return cls(everyone=False, users=False, roles=False, replied_user=False)
-
-    def to_dict(self):
-        parse = []
-        data = {}
-
-        if self.everyone:
-            parse.append('everyone')
-
-        if self.users == True:
-            parse.append('users')
-        elif self.users != False:
-            data['users'] = [x.id for x in self.users]
-
-        if self.roles == True:
-            parse.append('roles')
-        elif self.roles != False:
-            data['roles'] = [x.id for x in self.roles]
-
-        if self.replied_user:
-            data['replied_user'] = True
-
-        data['parse'] = parse
-        return data
-
-    def merge(self, other):
-        # Creates a new AllowedMentions by merging from another one.
-        # Merge is done by using the 'self' values unless explicitly
-        # overridden by the 'other' values.
-        everyone = self.everyone if other.everyone is default else other.everyone
-        users = self.users if other.users is default else other.users
-        roles = self.roles if other.roles is default else other.roles
-        replied_user = self.replied_user if other.replied_user is default else other.replied_user
-        return AllowedMentions(everyone=everyone, roles=roles, users=users, replied_user=replied_user)
-
-    def __repr__(self):
-        return '{0.__class__.__qualname__}(everyone={0.everyone}, users={0.users}, roles={0.roles}, replied_user={0.replied_user})'.format(self)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+from typing import Union, Sequence, TYPE_CHECKING, Any
+
+# fmt: off
+__all__ = (
+    'AllowedMentions',
+)
+# fmt: on
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    from .types.message import AllowedMentions as AllowedMentionsPayload
+    from .abc import Snowflake
+
+
+class _FakeBool:
+    def __repr__(self):
+        return 'True'
+
+    def __eq__(self, other):
+        return other is True
+
+    def __bool__(self):
+        return True
+
+
+default: Any = _FakeBool()
+
+
+class AllowedMentions:
+    """A class that represents what mentions are allowed in a message.
+
+    This class can be set during :class:`Client` initialisation to apply
+    to every message sent. It can also be applied on a per message basis
+    via :meth:`abc.Messageable.send` for more fine-grained control.
+
+    Attributes
+    ------------
+    everyone: :class:`bool`
+        Whether to allow everyone and here mentions. Defaults to ``True``.
+    users: Union[:class:`bool`, Sequence[:class:`abc.Snowflake`]]
+        Controls the users being mentioned. If ``True`` (the default) then
+        users are mentioned based on the message content. If ``False`` then
+        users are not mentioned at all. If a list of :class:`abc.Snowflake`
+        is given then only the users provided will be mentioned, provided those
+        users are in the message content.
+    roles: Union[:class:`bool`, Sequence[:class:`abc.Snowflake`]]
+        Controls the roles being mentioned. If ``True`` (the default) then
+        roles are mentioned based on the message content. If ``False`` then
+        roles are not mentioned at all. If a list of :class:`abc.Snowflake`
+        is given then only the roles provided will be mentioned, provided those
+        roles are in the message content.
+    replied_user: :class:`bool`
+        Whether to mention the author of the message being replied to. Defaults
+        to ``True``.
+
+        .. versionadded:: 1.6
+    """
+
+    __slots__ = ('everyone', 'users', 'roles', 'replied_user')
+
+    def __init__(
+        self,
+        *,
+        everyone: bool = default,
+        users: Union[bool, Sequence[Snowflake]] = default,
+        roles: Union[bool, Sequence[Snowflake]] = default,
+        replied_user: bool = default,
+    ):
+        self.everyone: bool = everyone
+        self.users: Union[bool, Sequence[Snowflake]] = users
+        self.roles: Union[bool, Sequence[Snowflake]] = roles
+        self.replied_user: bool = replied_user
+
+    @classmethod
+    def all(cls) -> Self:
+        """A factory method that returns a :class:`AllowedMentions` with all fields explicitly set to ``True``
+
+        .. versionadded:: 1.5
+        """
+        return cls(everyone=True, users=True, roles=True, replied_user=True)
+
+    @classmethod
+    def none(cls) -> Self:
+        """A factory method that returns a :class:`AllowedMentions` with all fields set to ``False``
+
+        .. versionadded:: 1.5
+        """
+        return cls(everyone=False, users=False, roles=False, replied_user=False)
+
+    def to_dict(self) -> AllowedMentionsPayload:
+        parse = []
+        data = {}
+
+        if self.everyone:
+            parse.append('everyone')
+
+        if self.users == True:
+            parse.append('users')
+        elif self.users != False:
+            data['users'] = [x.id for x in self.users]
+
+        if self.roles == True:
+            parse.append('roles')
+        elif self.roles != False:
+            data['roles'] = [x.id for x in self.roles]
+
+        if self.replied_user:
+            data['replied_user'] = True
+
+        data['parse'] = parse
+        return data  # type: ignore
+
+    def merge(self, other: AllowedMentions) -> AllowedMentions:
+        # Creates a new AllowedMentions by merging from another one
+        # Merge is done by using the 'self' values unless explicitly
+        # overridden by the 'other' values
+        everyone = self.everyone if other.everyone is default else other.everyone
+        users = self.users if other.users is default else other.users
+        roles = self.roles if other.roles is default else other.roles
+        replied_user = self.replied_user if other.replied_user is default else other.replied_user
+        return AllowedMentions(everyone=everyone, roles=roles, users=users, replied_user=replied_user)
+
+    def __repr__(self) -> str:
+        return (
+            f'{self.__class__.__name__}(everyone={self.everyone}, '
+            f'users={self.users}, roles={self.roles}, replied_user={self.replied_user})'
+        )
```

### Comparing `discord.py-self-1.9.2/discord/message.py` & `discord.py-self-2.0.0/discord/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1601 +1,2277 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import asyncio
-import datetime
-import re
-import io
-
-from . import utils
-from .reaction import Reaction
-from .emoji import Emoji
-from .partial_emoji import PartialEmoji
-from .calls import CallMessage
-from .enums import MessageType, ChannelType, try_enum
-from .errors import InvalidArgument, HTTPException, DiscordException
-from .embeds import Embed
-from .member import Member
-from .flags import MessageFlags
-from .file import File
-from .utils import escape_mentions
-from .guild import Guild
-from .mixins import Hashable
-from .sticker import Sticker
-from .invite import Invite
-
-__all__ = (
-    'Attachment',
-    'Message',
-    'PartialMessage',
-    'MessageReference',
-    'DeletedReferencedMessage',
-)
-
-def convert_emoji_reaction(emoji):
-    if isinstance(emoji, Reaction):
-        emoji = emoji.emoji
-
-    if isinstance(emoji, Emoji):
-        return '%s:%s' % (emoji.name, emoji.id)
-    if isinstance(emoji, PartialEmoji):
-        return emoji._as_reaction()
-    if isinstance(emoji, str):
-        # Reactions can be in :name:id format, but not <:name:id>.
-        # No existing emojis have <> in them, so this should be okay.
-        return emoji.strip('<>')
-
-    raise InvalidArgument('emoji argument must be str, Emoji, or Reaction not {.__class__.__name__}.'.format(emoji))
-
-class Attachment(Hashable):
-    """Represents an attachment from Discord.
-
-    .. container:: operations
-
-        .. describe:: str(x)
-
-            Returns the URL of the attachment.
-
-        .. describe:: x == y
-
-            Checks if the attachment is equal to another attachment.
-
-        .. describe:: x != y
-
-            Checks if the attachment is not equal to another attachment.
-
-        .. describe:: hash(x)
-
-            Returns the hash of the attachment.
-
-    .. versionchanged:: 1.7
-        Attachment can now be casted to :class:`str` and is hashable.
-
-    Attributes
-    ------------
-    id: :class:`int`
-        The attachment ID.
-    size: :class:`int`
-        The attachment size in bytes.
-    height: Optional[:class:`int`]
-        The attachment's height, in pixels. Only applicable to images and videos.
-    width: Optional[:class:`int`]
-        The attachment's width, in pixels. Only applicable to images and videos.
-    filename: :class:`str`
-        The attachment's filename.
-    url: :class:`str`
-        The attachment URL. If the message this attachment was attached
-        to is deleted, then this will 404.
-    proxy_url: :class:`str`
-        The proxy URL. This is a cached version of the :attr:`~Attachment.url` in the
-        case of images. When the message is deleted, this URL might be valid for a few
-        minutes or not valid at all.
-    content_type: Optional[:class:`str`]
-        The attachment's `media type <https://en.wikipedia.org/wiki/Media_type>`_
-
-        .. versionadded:: 1.7
-    """
-
-    __slots__ = ('id', 'size', 'height', 'width', 'filename', 'url', 'proxy_url', '_http', 'content_type')
-
-    def __init__(self, *, data, state):
-        self.id = int(data['id'])
-        self.size = data['size']
-        self.height = data.get('height')
-        self.width = data.get('width')
-        self.filename = data['filename']
-        self.url = data.get('url')
-        self.proxy_url = data.get('proxy_url')
-        self._http = state.http
-        self.content_type = data.get('content_type')
-
-    def is_spoiler(self):
-        """:class:`bool`: Whether this attachment contains a spoiler."""
-        return self.filename.startswith('SPOILER_')
-
-    def __repr__(self):
-        return '<Attachment id={0.id} filename={0.filename!r} url={0.url!r}>'.format(self)
-
-    def __str__(self):
-        return self.url or ''
-
-    async def save(self, fp, *, seek_begin=True, use_cached=False):
-        """|coro|
-
-        Saves this attachment into a file-like object.
-
-        Parameters
-        -----------
-        fp: Union[:class:`io.BufferedIOBase`, :class:`os.PathLike`]
-            The file-like object to save this attachment to or the filename
-            to use. If a filename is passed then a file is created with that
-            filename and used instead.
-        seek_begin: :class:`bool`
-            Whether to seek to the beginning of the file after saving is
-            successfully done.
-        use_cached: :class:`bool`
-            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
-            the attachment. This will allow attachments to be saved after deletion
-            more often, compared to the regular URL which is generally deleted right
-            after the message is deleted. Note that this can still fail to download
-            deleted attachments if too much time has passed and it does not work
-            on some types of attachments.
-
-        Raises
-        --------
-        HTTPException
-            Saving the attachment failed.
-        NotFound
-            The attachment was deleted.
-
-        Returns
-        --------
-        :class:`int`
-            The number of bytes written.
-        """
-        data = await self.read(use_cached=use_cached)
-        if isinstance(fp, io.IOBase) and fp.writable():
-            written = fp.write(data)
-            if seek_begin:
-                fp.seek(0)
-            return written
-        else:
-            with open(fp, 'wb') as f:
-                return f.write(data)
-
-    async def read(self, *, use_cached=False):
-        """|coro|
-
-        Retrieves the content of this attachment as a :class:`bytes` object.
-
-        .. versionadded:: 1.1
-
-        Parameters
-        -----------
-        use_cached: :class:`bool`
-            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
-            the attachment. This will allow attachments to be saved after deletion
-            more often, compared to the regular URL which is generally deleted right
-            after the message is deleted. Note that this can still fail to download
-            deleted attachments if too much time has passed and it does not work
-            on some types of attachments.
-
-        Raises
-        ------
-        HTTPException
-            Downloading the attachment failed.
-        Forbidden
-            You do not have permissions to access this attachment
-        NotFound
-            The attachment was deleted.
-
-        Returns
-        -------
-        :class:`bytes`
-            The contents of the attachment.
-        """
-        url = self.proxy_url if use_cached else self.url
-        data = await self._http.get_from_cdn(url)
-        return data
-
-    async def to_file(self, *, use_cached=False, spoiler=False):
-        """|coro|
-
-        Converts the attachment into a :class:`File` suitable for sending via
-        :meth:`abc.Messageable.send`.
-
-        .. versionadded:: 1.3
-
-        Parameters
-        -----------
-        use_cached: :class:`bool`
-            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
-            the attachment. This will allow attachments to be saved after deletion
-            more often, compared to the regular URL which is generally deleted right
-            after the message is deleted. Note that this can still fail to download
-            deleted attachments if too much time has passed and it does not work
-            on some types of attachments.
-
-            .. versionadded:: 1.4
-        spoiler: :class:`bool`
-            Whether the file is a spoiler.
-
-            .. versionadded:: 1.4
-
-        Raises
-        ------
-        HTTPException
-            Downloading the attachment failed.
-        Forbidden
-            You do not have permissions to access this attachment
-        NotFound
-            The attachment was deleted.
-
-        Returns
-        -------
-        :class:`File`
-            The attachment as a file suitable for sending.
-        """
-
-        data = await self.read(use_cached=use_cached)
-        return File(io.BytesIO(data), filename=self.filename, spoiler=spoiler)
-
-class DeletedReferencedMessage:
-    """A special sentinel type that denotes whether the
-    resolved message referenced message had since been deleted.
-
-    The purpose of this class is to separate referenced messages that could not be
-    fetched and those that were previously fetched but have since been deleted.
-
-    .. versionadded:: 1.6
-    """
-
-    __slots__ = ('_parent')
-
-    def __init__(self, parent):
-        self._parent = parent
-
-    @property
-    def id(self):
-        """:class:`int`: The message ID of the deleted referenced message."""
-        return self._parent.message_id
-
-    @property
-    def channel_id(self):
-        """:class:`int`: The channel ID of the deleted referenced message."""
-        return self._parent.channel_id
-
-    @property
-    def guild_id(self):
-        """Optional[:class:`int`]: The guild ID of the deleted referenced message."""
-        return self._parent.guild_id
-
-
-class MessageReference:
-    """Represents a reference to a :class:`~discord.Message`.
-
-    .. versionadded:: 1.5
-
-    .. versionchanged:: 1.6
-        This class can now be constructed by users.
-
-    Attributes
-    -----------
-    message_id: Optional[:class:`int`]
-        The id of the message referenced.
-    channel_id: :class:`int`
-        The channel id of the message referenced.
-    guild_id: Optional[:class:`int`]
-        The guild id of the message referenced.
-    fail_if_not_exists: :class:`bool`
-        Whether replying to the referenced message should raise :class:`HTTPException`
-        if the message no longer exists or Discord could not fetch the message.
-
-        .. versionadded:: 1.7
-
-    resolved: Optional[Union[:class:`Message`, :class:`DeletedReferencedMessage`]]
-        The message that this reference resolved to. If this is ``None``
-        then the original message was not fetched either due to the Discord API
-        not attempting to resolve it or it not being available at the time of creation.
-        If the message was resolved at a prior point but has since been deleted then
-        this will be of type :class:`DeletedReferencedMessage`.
-
-        Currently, this is mainly the replied to message when a user replies to a message.
-
-        .. versionadded:: 1.6
-    """
-
-    __slots__ = ('message_id', 'channel_id', 'guild_id', 'fail_if_not_exists', 'resolved', '_state')
-
-    def __init__(self, *, message_id, channel_id, guild_id=None, fail_if_not_exists=True):
-        self._state = None
-        self.resolved = None
-        self.message_id = message_id
-        self.channel_id = channel_id
-        self.guild_id = guild_id
-        self.fail_if_not_exists = fail_if_not_exists
-
-    @classmethod
-    def with_state(cls, state, data):
-        self = cls.__new__(cls)
-        self.message_id = utils._get_as_snowflake(data, 'message_id')
-        self.channel_id = int(data.pop('channel_id'))
-        self.guild_id = utils._get_as_snowflake(data, 'guild_id')
-        self.fail_if_not_exists = data.get('fail_if_not_exists', True)
-        self._state = state
-        self.resolved = None
-        return self
-
-    @classmethod
-    def from_message(cls, message, *, fail_if_not_exists=True):
-        """Creates a :class:`MessageReference` from an existing :class:`~discord.Message`.
-
-        .. versionadded:: 1.6
-
-        Parameters
-        ----------
-        message: :class:`~discord.Message`
-            The message to be converted into a reference.
-        fail_if_not_exists: :class:`bool`
-            Whether replying to the referenced message should raise :class:`HTTPException`
-            if the message no longer exists or Discord could not fetch the message.
-
-            .. versionadded:: 1.7
-
-        Returns
-        -------
-        :class:`MessageReference`
-            A reference to the message.
-        """
-        self = cls(message_id=message.id, channel_id=message.channel.id, guild_id=getattr(message.guild, 'id', None), fail_if_not_exists=fail_if_not_exists)
-        self._state = message._state
-        return self
-
-    @property
-    def cached_message(self):
-        """Optional[:class:`~discord.Message`]: The cached message, if found in the internal message cache."""
-        return self._state._get_message(self.message_id)
-
-    @property
-    def jump_url(self):
-        """:class:`str`: Returns a URL that allows the client to jump to the referenced message.
-
-        .. versionadded:: 1.7
-        """
-        guild_id = self.guild_id if self.guild_id is not None else '@me'
-        return 'https://discord.com/channels/{0}/{1.channel_id}/{1.message_id}'.format(guild_id, self)
-
-    def __repr__(self):
-        return '<MessageReference message_id={0.message_id!r} channel_id={0.channel_id!r} guild_id={0.guild_id!r}>'.format(self)
-
-    def to_dict(self):
-        result = {'message_id': self.message_id} if self.message_id is not None else {}
-        result['channel_id'] = self.channel_id
-        if self.guild_id is not None:
-            result['guild_id'] = self.guild_id
-        if self.fail_if_not_exists is not None:
-            result['fail_if_not_exists'] = self.fail_if_not_exists
-        return result
-
-    to_message_reference_dict = to_dict
-
-def flatten_handlers(cls):
-    prefix = len('_handle_')
-    handlers = [
-        (key[prefix:], value)
-        for key, value in cls.__dict__.items()
-        if key.startswith('_handle_') and key != '_handle_member'
-    ]
-
-    # store _handle_member last
-    handlers.append(('member', cls._handle_member))
-    cls._HANDLERS = handlers
-    cls._CACHED_SLOTS = [
-        attr for attr in cls.__slots__ if attr.startswith('_cs_')
-    ]
-    return cls
-
-@flatten_handlers
-class Message(Hashable):
-    r"""Represents a message from Discord.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two messages are equal.
-
-        .. describe:: x != y
-
-            Checks if two messages are not equal.
-
-        .. describe:: hash(x)
-
-            Returns the message's hash.
-
-    Attributes
-    -----------
-    tts: :class:`bool`
-        Specifies if the message was done with text-to-speech.
-        This can only be accurately received in :func:`on_message` due to
-        a discord limitation.
-    type: :class:`MessageType`
-        The type of message. In most cases this should not be checked, but it is helpful
-        in cases where it might be a system message for :attr:`system_content`.
-    author: :class:`abc.User`
-        A :class:`Member` that sent the message. If :attr:`channel` is a
-        private channel or the user has the left the guild, then it is a :class:`User` instead.
-    content: :class:`str`
-        The actual contents of the message.
-    nonce
-        The value used by the discord guild and the client to verify that the message is successfully sent.
-        This is not stored long term within Discord's servers and is only used ephemerally.
-    embeds: List[:class:`Embed`]
-        A list of embeds the message has.
-    channel: Union[:class:`abc.Messageable`]
-        The :class:`TextChannel` that the message was sent from.
-        Could be a :class:`DMChannel` or :class:`GroupChannel` if it's a private message.
-    call: Optional[:class:`CallMessage`]
-        The call that the message refers to. This is only applicable to messages of type
-        :attr:`MessageType.call`.
-    reference: Optional[:class:`~discord.MessageReference`]
-        The message that this message references. This is only applicable to messages of
-        type :attr:`MessageType.pins_add`, crossposted messages created by a
-        followed channel integration, or message replies.
-
-        .. versionadded:: 1.5
-
-    mention_everyone: :class:`bool`
-        Specifies if the message mentions everyone.
-
-        .. note::
-
-            This does not check if the ``@everyone`` or the ``@here`` text is in the message itself.
-            Rather this boolean indicates if either the ``@everyone`` or the ``@here`` text is in the message
-            **and** it did end up mentioning.
-    mentions: List[:class:`abc.User`]
-        A list of :class:`Member` that were mentioned. If the message is in a private message
-        then the list will be of :class:`User` instead. For messages that are not of type
-        :attr:`MessageType.default`\, this array can be used to aid in system messages.
-        For more information, see :attr:`system_content`.
-
-        .. warning::
-
-            The order of the mentions list is not in any particular order so you should
-            not rely on it. This is a Discord limitation, not one with the library.
-    channel_mentions: List[:class:`abc.GuildChannel`]
-        A list of :class:`abc.GuildChannel` that were mentioned. If the message is in a private message
-        then the list is always empty.
-    role_mentions: List[:class:`Role`]
-        A list of :class:`Role` that were mentioned. If the message is in a private message
-        then the list is always empty.
-    id: :class:`int`
-        The message ID.
-    webhook_id: Optional[:class:`int`]
-        If this message was sent by a webhook, then this is the webhook ID's that sent this
-        message.
-    attachments: List[:class:`Attachment`]
-        A list of attachments given to a message.
-    pinned: :class:`bool`
-        Specifies if the message is currently pinned.
-    flags: :class:`MessageFlags`
-        Extra features of the message.
-
-        .. versionadded:: 1.3
-
-    reactions : List[:class:`Reaction`]
-        Reactions to a message. Reactions can be either custom emoji or standard unicode emoji.
-    activity: Optional[:class:`dict`]
-        The activity associated with this message. Sent with Rich-Presence related messages that for
-        example, request joining, spectating, or listening to or with another member.
-
-        It is a dictionary with the following optional keys:
-
-        - ``type``: An integer denoting the type of message activity being requested.
-        - ``party_id``: The party ID associated with the party.
-    application: Optional[:class:`dict`]
-        The rich presence enabled application associated with this message.
-
-        It is a dictionary with the following keys:
-
-        - ``id``: A string representing the application's ID.
-        - ``name``: A string representing the application's name.
-        - ``description``: A string representing the application's description.
-        - ``icon``: A string representing the icon ID of the application.
-        - ``cover_image``: A string representing the embed's image asset ID.
-    stickers: List[:class:`Sticker`]
-        A list of stickers given to the message.
-
-        .. versionadded:: 1.6
-    """
-
-    __slots__ = ('_edited_timestamp', 'tts', 'content', 'channel', 'webhook_id',
-                 'mention_everyone', 'embeds', 'id', 'mentions', 'author',
-                 '_cs_channel_mentions', '_cs_raw_mentions', 'attachments',
-                 '_cs_clean_content', '_cs_raw_channel_mentions', 'nonce', 'pinned',
-                 'role_mentions', '_cs_raw_role_mentions', 'type', 'call', 'flags',
-                 '_cs_system_content', '_cs_guild', '_state', 'reactions', 'reference',
-                 'application', 'activity', 'stickers', '_cs_invites')
-
-    def __init__(self, *, state, channel, data):
-        self._state = state
-        self.id = int(data['id'])
-        self.webhook_id = utils._get_as_snowflake(data, 'webhook_id')
-        self.reactions = [Reaction(message=self, data=d) for d in data.get('reactions', [])]
-        self.attachments = [Attachment(data=a, state=self._state) for a in data['attachments']]
-        self.embeds = [Embed.from_dict(a) for a in data['embeds']]
-        self.application = data.get('application')
-        self.activity = data.get('activity')
-        self.channel = channel
-        self.call = None
-        self._edited_timestamp = utils.parse_time(data['edited_timestamp'])
-        self.type = try_enum(MessageType, data['type'])
-        self.pinned = data['pinned']
-        self.flags = MessageFlags._from_value(data.get('flags', 0))
-        self.mention_everyone = data['mention_everyone']
-        self.tts = data['tts']
-        self.content = data['content']
-        self.nonce = data.get('nonce')
-        self.stickers = [Sticker(data=data, state=state) for data in data.get('stickers', [])]
-
-        try:
-            ref = data['message_reference']
-        except KeyError:
-            self.reference = None
-        else:
-            self.reference = ref = MessageReference.with_state(state, ref)
-            try:
-                resolved = data['referenced_message']
-            except KeyError:
-                pass
-            else:
-                if resolved is None:
-                    ref.resolved = DeletedReferencedMessage(ref)
-                else:
-                    # Right now the channel IDs match but maybe in the future they won't.
-                    if ref.channel_id == channel.id:
-                        chan = channel
-                    else:
-                        chan, _ = state._get_guild_channel(resolved)
-
-                    ref.resolved = self.__class__(channel=chan, data=resolved, state=state)
-
-        for handler in ('author', 'member', 'mentions', 'mention_roles', 'call', 'flags'):
-            try:
-                getattr(self, '_handle_%s' % handler)(data[handler])
-            except KeyError:
-                continue
-
-    def __repr__(self):
-        return '<Message id={0.id} channel={0.channel!r} type={0.type!r} author={0.author!r} flags={0.flags!r}>'.format(self)
-
-    def _try_patch(self, data, key, transform=None):
-        try:
-            value = data[key]
-        except KeyError:
-            pass
-        else:
-            if transform is None:
-                setattr(self, key, value)
-            else:
-                setattr(self, key, transform(value))
-
-    def _add_reaction(self, data, emoji, user_id):
-        reaction = utils.find(lambda r: r.emoji == emoji, self.reactions)
-        is_me = data['me'] = user_id == self._state.self_id
-
-        if reaction is None:
-            reaction = Reaction(message=self, data=data, emoji=emoji)
-            self.reactions.append(reaction)
-        else:
-            reaction.count += 1
-            if is_me:
-                reaction.me = is_me
-
-        return reaction
-
-    def _remove_reaction(self, data, emoji, user_id):
-        reaction = utils.find(lambda r: r.emoji == emoji, self.reactions)
-
-        if reaction is None:
-            # already removed?
-            raise ValueError('Emoji already removed?')
-
-        # if reaction isn't in the list, we crash. This means discord
-        # sent bad data, or we stored improperly
-        reaction.count -= 1
-
-        if user_id == self._state.self_id:
-            reaction.me = False
-        if reaction.count == 0:
-            # this raises ValueError if something went wrong as well.
-            self.reactions.remove(reaction)
-
-        return reaction
-
-    def _clear_emoji(self, emoji):
-        to_check = str(emoji)
-        for index, reaction in enumerate(self.reactions):
-            if str(reaction.emoji) == to_check:
-                break
-        else:
-            # didn't find anything so just return
-            return
-
-        del self.reactions[index]
-        return reaction
-
-    def _update(self, data):
-        # In an update scheme, 'author' key has to be handled before 'member'
-        # otherwise they overwrite each other which is undesirable.
-        # Since there's no good way to do this we have to iterate over every
-        # handler rather than iterating over the keys which is a little slower
-        for key, handler in self._HANDLERS:
-            try:
-                value = data[key]
-            except KeyError:
-                continue
-            else:
-                handler(self, value)
-
-        # clear the cached properties
-        for attr in self._CACHED_SLOTS:
-            try:
-                delattr(self, attr)
-            except AttributeError:
-                pass
-
-    def _handle_edited_timestamp(self, value):
-        self._edited_timestamp = utils.parse_time(value)
-
-    def _handle_pinned(self, value):
-        self.pinned = value
-
-    def _handle_flags(self, value):
-        self.flags = MessageFlags._from_value(value)
-
-    def _handle_application(self, value):
-        self.application = value
-
-    def _handle_activity(self, value):
-        self.activity = value
-
-    def _handle_mention_everyone(self, value):
-        self.mention_everyone = value
-
-    def _handle_tts(self, value):
-        self.tts = value
-
-    def _handle_type(self, value):
-        self.type = try_enum(MessageType, value)
-
-    def _handle_content(self, value):
-        self.content = value
-
-    def _handle_attachments(self, value):
-        self.attachments = [Attachment(data=a, state=self._state) for a in value]
-
-    def _handle_embeds(self, value):
-        self.embeds = [Embed.from_dict(data) for data in value]
-
-    def _handle_nonce(self, value):
-        self.nonce = value
-
-    def _handle_author(self, author):
-        self.author = self._state.store_user(author)
-        if isinstance(self.guild, Guild):
-            found = self.guild.get_member(self.author.id)
-            if found is not None:
-                self.author = found
-
-    def _handle_member(self, member):
-        # The gateway now gives us full Member objects sometimes with the following keys
-        # deaf, mute, joined_at, roles
-        # For the sake of performance I'm going to assume that the only
-        # field that needs *updating* would be the joined_at field.
-        # If there is no Member object (for some strange reason), then we can upgrade
-        # ourselves to a more "partial" member object.
-        author = self.author
-        try:
-            # Update member reference
-            author._update_from_message(member)
-        except AttributeError:
-            # It's a user here
-            # TODO: consider adding to cache here
-            self.author = Member._from_message(message=self, data=member)
-
-    def _handle_mentions(self, mentions):
-        self.mentions = r = []
-        guild = self.guild
-        state = self._state
-        if not isinstance(guild, Guild):
-            self.mentions = [state.store_user(m) for m in mentions]
-            return
-
-        for mention in filter(None, mentions):
-            id_search = int(mention['id'])
-            member = guild.get_member(id_search)
-            if member is not None:
-                r.append(member)
-            else:
-                r.append(Member._try_upgrade(data=mention, guild=guild, state=state))
-
-    def _handle_mention_roles(self, role_mentions):
-        self.role_mentions = []
-        if isinstance(self.guild, Guild):
-            for role_id in map(int, role_mentions):
-                role = self.guild.get_role(role_id)
-                if role is not None:
-                    self.role_mentions.append(role)
-
-    def _handle_call(self, call):
-        if call is None or self.type is not MessageType.call:
-            self.call = None
-            return
-
-        # we get the participant source from the mentions array or
-        # the author
-
-        participants = []
-        for uid in map(int, call.get('participants', [])):
-            if uid == self.author.id:
-                participants.append(self.author)
-            else:
-                user = utils.find(lambda u: u.id == uid, self.mentions)
-                if user is not None:
-                    participants.append(user)
-
-        call['participants'] = participants
-        self.call = CallMessage(message=self, **call)
-
-    def _rebind_channel_reference(self, new_channel):
-        self.channel = new_channel
-
-        try:
-            del self._cs_guild
-        except AttributeError:
-            pass
-
-    @utils.cached_slot_property('_cs_guild')
-    def guild(self):
-        """Optional[:class:`Guild`]: The guild that the message belongs to, if applicable."""
-        return getattr(self.channel, 'guild', None)
-
-    @utils.cached_slot_property('_cs_raw_mentions')
-    def raw_mentions(self):
-        """List[:class:`int`]: A property that returns an array of user IDs matched with
-        the syntax of ``<@user_id>`` in the message content.
-
-        This allows you to receive the user IDs of mentioned users
-        even in a private message context.
-        """
-        return [int(x) for x in re.findall(r'<@!?([0-9]+)>', self.content)]
-
-    @utils.cached_slot_property('_cs_raw_channel_mentions')
-    def raw_channel_mentions(self):
-        """List[:class:`int`]: A property that returns an array of channel IDs matched with
-        the syntax of ``<#channel_id>`` in the message content.
-        """
-        return [int(x) for x in re.findall(r'<#([0-9]+)>', self.content)]
-
-    @utils.cached_slot_property('_cs_raw_role_mentions')
-    def raw_role_mentions(self):
-        """List[:class:`int`]: A property that returns an array of role IDs matched with
-        the syntax of ``<@&role_id>`` in the message content.
-        """
-        return [int(x) for x in re.findall(r'<@&([0-9]+)>', self.content)]
-
-    @utils.cached_slot_property('_cs_channel_mentions')
-    def channel_mentions(self):
-        if self.guild is None:
-            return []
-        it = filter(None, map(self.guild.get_channel, self.raw_channel_mentions))
-        return utils._unique(it)
-
-    @utils.cached_slot_property('_cs_clean_content')
-    def clean_content(self):
-        """:class:`str`: A property that returns the content in a "cleaned up"
-        manner. This basically means that mentions are transformed
-        into the way the client shows it. e.g. ``<#id>`` will transform
-        into ``#name``.
-
-        This will also transform @everyone and @here mentions into
-        non-mentions.
-
-        .. note::
-
-            This *does not* affect markdown. If you want to escape
-            or remove markdown then use :func:`utils.escape_markdown` or :func:`utils.remove_markdown` 
-            respectively, along with this function.
-        """
-
-        transformations = {
-            re.escape('<#%s>' % channel.id): '#' + channel.name
-            for channel in self.channel_mentions
-        }
-
-        mention_transforms = {
-            re.escape('<@%s>' % member.id): '@' + member.display_name
-            for member in self.mentions
-        }
-
-        # add the <@!user_id> cases as well..
-        second_mention_transforms = {
-            re.escape('<@!%s>' % member.id): '@' + member.display_name
-            for member in self.mentions
-        }
-
-        transformations.update(mention_transforms)
-        transformations.update(second_mention_transforms)
-
-        if self.guild is not None:
-            role_transforms = {
-                re.escape('<@&%s>' % role.id): '@' + role.name
-                for role in self.role_mentions
-            }
-            transformations.update(role_transforms)
-
-        def repl(obj):
-            return transformations.get(re.escape(obj.group(0)), '')
-
-        pattern = re.compile('|'.join(transformations.keys()))
-        result = pattern.sub(repl, self.content)
-        return escape_mentions(result)
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: The message's creation time in UTC."""
-        return utils.snowflake_time(self.id)
-
-    @property
-    def edited_at(self):
-        """Optional[:class:`datetime.datetime`]: A naive UTC datetime object containing the edited time of the message."""
-        return self._edited_timestamp
-
-    @property
-    def jump_url(self):
-        """:class:`str`: Returns a URL that allows the client to jump to this message."""
-        guild_id = getattr(self.guild, 'id', '@me')
-        return 'https://discord.com/channels/{0}/{1.channel.id}/{1.id}'.format(guild_id, self)
-
-    def is_system(self):
-        """:class:`bool`: Whether the message is a system message.
-
-        .. versionadded:: 1.3
-        """
-        return self.type is not MessageType.default
-
-    @utils.cached_slot_property('_cs_system_content')
-    def system_content(self):
-        r""":class:`str`: A property that returns the content that is rendered
-        regardless of the :attr:`Message.type`.
-
-        In the case of :attr:`MessageType.default`\, this just returns the
-        regular :attr:`Message.content`. Otherwise this returns an English
-        message denoting the contents of the system message.
-        """
-
-        if self.type is MessageType.default:
-            return self.content
-
-        if self.type is MessageType.pins_add:
-            return '{0.name} pinned a message to this channel.'.format(self.author)
-
-        if self.type is MessageType.recipient_add:
-            return '{0.name} added {1.name} to the group.'.format(self.author, self.mentions[0])
-
-        if self.type is MessageType.recipient_remove:
-            return '{0.name} removed {1.name} from the group.'.format(self.author, self.mentions[0])
-
-        if self.type is MessageType.channel_name_change:
-            return '{0.author.name} changed the channel name: {0.content}'.format(self)
-
-        if self.type is MessageType.channel_icon_change:
-            return '{0.author.name} changed the channel icon.'.format(self)
-
-        if self.type is MessageType.new_member:
-            formats = [
-                "{0} joined the party.",
-                "{0} is here.",
-                "Welcome, {0}. We hope you brought pizza.",
-                "A wild {0} appeared.",
-                "{0} just landed.",
-                "{0} just slid into the server.",
-                "{0} just showed up!",
-                "Welcome {0}. Say hi!",
-                "{0} hopped into the server.",
-                "Everyone welcome {0}!",
-                "Glad you're here, {0}.",
-                "Good to see you, {0}.",
-                "Yay you made it, {0}!",
-            ]
-
-            # manually reconstruct the epoch with millisecond precision, because
-            # datetime.datetime.timestamp() doesn't return the exact posix
-            # timestamp with the precision that we need
-            created_at_ms = int((self.created_at - datetime.datetime(1970, 1, 1)).total_seconds() * 1000)
-            return formats[created_at_ms % len(formats)].format(self.author.name)
-
-        if self.type is MessageType.call:
-            # we're at the call message type now, which is a bit more complicated.
-            # we can make the assumption that Message.channel is a PrivateChannel
-            # with the type ChannelType.group or ChannelType.private
-            call_ended = self.call.ended_timestamp is not None
-
-            if self.channel.me in self.call.participants:
-                return '{0.author.name} started a call.'.format(self)
-            elif call_ended:
-                return 'You missed a call from {0.author.name}'.format(self)
-            else:
-                return '{0.author.name} started a call \N{EM DASH} Join the call.'.format(self)
-
-        if self.type is MessageType.premium_guild_subscription:
-            return '{0.author.name} just boosted the server!'.format(self)
-
-        if self.type is MessageType.premium_guild_tier_1:
-            return '{0.author.name} just boosted the server! {0.guild} has achieved **Level 1!**'.format(self)
-
-        if self.type is MessageType.premium_guild_tier_2:
-            return '{0.author.name} just boosted the server! {0.guild} has achieved **Level 2!**'.format(self)
-
-        if self.type is MessageType.premium_guild_tier_3:
-            return '{0.author.name} just boosted the server! {0.guild} has achieved **Level 3!**'.format(self)
-
-        if self.type is MessageType.channel_follow_add:
-            return '{0.author.name} has added {0.content} to this channel'.format(self)
-
-        if self.type is MessageType.guild_stream:
-            return '{0.author.name} is live! Now streaming {0.author.activity.name}'.format(self)
-
-        if self.type is MessageType.guild_discovery_disqualified:
-            return 'This server has been removed from Server Discovery because it no longer passes all the requirements. Check Server Settings for more details.'
-
-        if self.type is MessageType.guild_discovery_requalified:
-            return 'This server is eligible for Server Discovery again and has been automatically relisted!'
-
-        if self.type is MessageType.guild_discovery_grace_period_initial_warning:
-            return 'This server has failed Discovery activity requirements for 1 week. If this server fails for 4 weeks in a row, it will be automatically removed from Discovery.'
-
-        if self.type is MessageType.guild_discovery_grace_period_final_warning:
-            return 'This server has failed Discovery activity requirements for 3 weeks in a row. If this server fails for 1 more week, it will be removed from Discovery.'
-
-    async def invites(self):
-        """|coro|
-
-        Retreives all valid invites in a message.
-
-        The official client does this with every message in the channel you're in.
-
-        Raises
-        ------
-        HTTPException
-            Fetching the invites failed.
-
-        Returns
-        -------
-        List[:class:`Invite`]
-            All valid invites contained in the message.
-        """
-        state = self._state
-        invite_ids = [utils.resolve_invite(match) for match in re.findall('(?:https?://)?discord(?:app)?\.(?:com/invite|gg)/[a-zA-Z0-9]+/?', self.content)]
-        invites = []
-        for id in invite_ids:
-            try:
-                invites.append(await state.http.get_invite(id))
-            except DiscordException:
-                pass
-        return [Invite.from_incomplete(state=state, data=invite, message_id=self.id) for invite in invites]
-
-    async def delete(self, *, delay=None):
-        """|coro|
-
-        Deletes the message.
-
-        Your own messages could be deleted without any proper permissions. However to
-        delete other people's messages, you need the :attr:`~Permissions.manage_messages`
-        permission.
-
-        .. versionchanged:: 1.1
-            Added the new ``delay`` keyword-only parameter.
-
-        Parameters
-        -----------
-        delay: Optional[:class:`float`]
-            If provided, the number of seconds to wait in the background
-            before deleting the message. If the deletion fails then it is silently ignored.
-
-        Raises
-        ------
-        Forbidden
-            You do not have proper permissions to delete the message.
-        NotFound
-            The message was deleted already
-        HTTPException
-            Deleting the message failed.
-        """
-        if delay is not None:
-            async def delete():
-                await asyncio.sleep(delay)
-                try:
-                    await self._state.http.delete_message(self.channel.id, self.id)
-                except HTTPException:
-                    pass
-
-            asyncio.ensure_future(delete(), loop=self._state.loop)
-        else:
-            await self._state.http.delete_message(self.channel.id, self.id)
-
-    async def edit(self, **fields):
-        """|coro|
-
-        Edits the message.
-
-        The content must be able to be transformed into a string via ``str(content)``.
-
-        .. versionchanged:: 1.3
-            The ``suppress`` keyword-only parameter was added.
-
-        Parameters
-        -----------
-        content: Optional[:class:`str`]
-            The new content to replace the message with.
-            Could be ``None`` to remove the content.
-        embed: Optional[:class:`Embed`]
-            The new embed to replace the original with.
-            Could be ``None`` to remove the embed.
-        suppress: :class:`bool`
-            Whether to suppress embeds for the message. This removes
-            all the embeds if set to ``True``. If set to ``False``
-            this brings the embeds back if they were suppressed.
-            Using this parameter requires :attr:`~.Permissions.manage_messages`.
-        delete_after: Optional[:class:`float`]
-            If provided, the number of seconds to wait in the background
-            before deleting the message we just edited. If the deletion fails,
-            then it is silently ignored.
-        allowed_mentions: Optional[:class:`~discord.AllowedMentions`]
-            Controls the mentions being processed in this message. If this is
-            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
-            The merging behaviour only overrides attributes that have been explicitly passed
-            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
-            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
-            are used instead.
-
-            .. versionadded:: 1.4
-
-        Raises
-        -------
-        HTTPException
-            Editing the message failed.
-        Forbidden
-            Tried to suppress a message without permissions or
-            edited a message's content or embed that isn't yours.
-        """
-
-        try:
-            content = fields['content']
-        except KeyError:
-            pass
-        else:
-            if content is not None:
-                fields['content'] = str(content)
-
-        try:
-            embed = fields['embed']
-        except KeyError:
-            pass
-        else:
-            if embed is not None:
-                fields['embed'] = embed.to_dict()
-
-        try:
-            suppress = fields.pop('suppress')
-        except KeyError:
-            pass
-        else:
-             flags = MessageFlags._from_value(self.flags.value)
-             flags.suppress_embeds = suppress
-             fields['flags'] = flags.value
-
-        delete_after = fields.pop('delete_after', None)
-
-        try:
-            allowed_mentions = fields.pop('allowed_mentions')
-        except KeyError:
-            pass
-        else:
-            if allowed_mentions is not None:
-                if self._state.allowed_mentions is not None:
-                    allowed_mentions = self._state.allowed_mentions.merge(allowed_mentions).to_dict()
-                else:
-                    allowed_mentions = allowed_mentions.to_dict()
-                fields['allowed_mentions'] = allowed_mentions
-
-        if fields:
-            data = await self._state.http.edit_message(self.channel.id, self.id, **fields)
-            self._update(data)
-
-        if delete_after is not None:
-            await self.delete(delay=delete_after)
-
-    async def publish(self):
-        """|coro|
-
-        Publishes this message to your announcement channel.
-
-        You must have the :attr:`~Permissions.send_messages` permission to do this.
-
-        If the message is not your own then the :attr:`~Permissions.manage_messages`
-        permission is also needed.
-
-        Raises
-        -------
-        Forbidden
-            You do not have the proper permissions to publish this message.
-        HTTPException
-            Publishing the message failed.
-        """
-
-        await self._state.http.publish_message(self.channel.id, self.id)
-
-    async def pin(self):
-        """|coro|
-
-        Pins the message.
-
-        You must have the :attr:`~Permissions.manage_messages` permission to do
-        this in a non-private channel context.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to pin the message.
-        NotFound
-            The message or channel was not found or deleted.
-        HTTPException
-            Pinning the message failed, probably due to the channel
-            having more than 50 pinned messages.
-        """
-
-        await self._state.http.pin_message(self.channel.id, self.id)
-        self.pinned = True
-
-    async def unpin(self):
-        """|coro|
-
-        Unpins the message.
-
-        You must have the :attr:`~Permissions.manage_messages` permission to do
-        this in a non-private channel context.
-
-        Raises
-        -------
-        Forbidden
-            You do not have permissions to unpin the message.
-        NotFound
-            The message or channel was not found or deleted.
-        HTTPException
-            Unpinning the message failed.
-        """
-
-        await self._state.http.unpin_message(self.channel.id, self.id)
-        self.pinned = False
-
-    async def add_reaction(self, emoji):
-        """|coro|
-
-        Add a reaction to the message.
-
-        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
-
-        You must have the :attr:`~Permissions.read_message_history` permission
-        to use this. If nobody else has reacted to the message using this
-        emoji, the :attr:`~Permissions.add_reactions` permission is required.
-
-        Parameters
-        ------------
-        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
-            The emoji to react with.
-
-        Raises
-        --------
-        HTTPException
-            Adding the reaction failed.
-        Forbidden
-            You do not have the proper permissions to react to the message.
-        NotFound
-            The emoji you specified was not found.
-        InvalidArgument
-            The emoji parameter is invalid.
-        """
-
-        emoji = convert_emoji_reaction(emoji)
-        await self._state.http.add_reaction(self.channel.id, self.id, emoji)
-
-    async def remove_reaction(self, emoji, member):
-        """|coro|
-
-        Remove a reaction by the member from the message.
-
-        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
-
-        If the reaction is not your own (i.e. ``member`` parameter is not you) then
-        the :attr:`~Permissions.manage_messages` permission is needed.
-
-        The ``member`` parameter must represent a member and meet
-        the :class:`abc.Snowflake` abc.
-
-        Parameters
-        ------------
-        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
-            The emoji to remove.
-        member: :class:`abc.Snowflake`
-            The member for which to remove the reaction.
-
-        Raises
-        --------
-        HTTPException
-            Removing the reaction failed.
-        Forbidden
-            You do not have the proper permissions to remove the reaction.
-        NotFound
-            The member or emoji you specified was not found.
-        InvalidArgument
-            The emoji parameter is invalid.
-        """
-
-        emoji = convert_emoji_reaction(emoji)
-
-        if member.id == self._state.self_id:
-            await self._state.http.remove_own_reaction(self.channel.id, self.id, emoji)
-        else:
-            await self._state.http.remove_reaction(self.channel.id, self.id, emoji, member.id)
-
-    async def clear_reaction(self, emoji):
-        """|coro|
-
-        Clears a specific reaction from the message.
-
-        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
-
-        You need the :attr:`~Permissions.manage_messages` permission to use this.
-
-        .. versionadded:: 1.3
-
-        Parameters
-        -----------
-        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
-            The emoji to clear.
-
-        Raises
-        --------
-        HTTPException
-            Clearing the reaction failed.
-        Forbidden
-            You do not have the proper permissions to clear the reaction.
-        NotFound
-            The emoji you specified was not found.
-        InvalidArgument
-            The emoji parameter is invalid.
-        """
-
-        emoji = convert_emoji_reaction(emoji)
-        await self._state.http.clear_single_reaction(self.channel.id, self.id, emoji)
-
-    async def clear_reactions(self):
-        """|coro|
-
-        Removes all the reactions from the message.
-
-        You need the :attr:`~Permissions.manage_messages` permission to use this.
-
-        Raises
-        --------
-        HTTPException
-            Removing the reactions failed.
-        Forbidden
-            You do not have the proper permissions to remove all the reactions.
-        """
-        await self._state.http.clear_reactions(self.channel.id, self.id)
-
-    async def ack(self):
-        """|coro|
-
-        Marks this message as read.
-
-        Raises
-        -------
-        HTTPException
-            Acking failed.
-        """
-        return await self._state.http.ack_message(self.channel.id, self.id)
-
-    async def reply(self, content=None, **kwargs):
-        """|coro|
-
-        A shortcut method to :meth:`.abc.Messageable.send` to reply to the
-        :class:`.Message`.
-
-        .. versionadded:: 1.6
-
-        Raises
-        --------
-        ~discord.HTTPException
-            Sending the message failed.
-        ~discord.Forbidden
-            You do not have the proper permissions to send the message.
-        ~discord.InvalidArgument
-            The ``files`` list is not of the appropriate size or
-            you specified both ``file`` and ``files``.
-
-        Returns
-        ---------
-        :class:`.Message`
-            The message that was sent.
-        """
-
-        return await self.channel.send(content, reference=self, **kwargs)
-
-    def to_reference(self, *, fail_if_not_exists=True):
-        """Creates a :class:`~discord.MessageReference` from the current message.
-
-        .. versionadded:: 1.6
-
-        Parameters
-        ----------
-        fail_if_not_exists: :class:`bool`
-            Whether replying using the message reference should raise :class:`HTTPException`
-            if the message no longer exists or Discord could not fetch the message.
-
-            .. versionadded:: 1.7
-
-        Returns
-        ---------
-        :class:`~discord.MessageReference`
-            The reference to this message.
-        """
-
-        return MessageReference.from_message(self, fail_if_not_exists=fail_if_not_exists)
-
-    def to_message_reference_dict(self):
-        data = {
-            'message_id': self.id,
-            'channel_id': self.channel.id,
-        }
-
-        if self.guild is not None:
-            data['guild_id'] = self.guild.id
-
-        return data
-
-def implement_partial_methods(cls):
-    msg = Message
-    for name in cls._exported_names:
-        func = getattr(msg, name)
-        setattr(cls, name, func)
-    return cls
-
-@implement_partial_methods
-class PartialMessage(Hashable):
-    """Represents a partial message to aid with working messages when only
-    a message and channel ID are present.
-
-    There are two ways to construct this class. The first one is through
-    the constructor itself, and the second is via
-    :meth:`TextChannel.get_partial_message` or :meth:`DMChannel.get_partial_message`.
-
-    Note that this class is trimmed down and has no rich attributes.
-
-    .. versionadded:: 1.6
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two partial messages are equal.
-
-        .. describe:: x != y
-
-            Checks if two partial messages are not equal.
-
-        .. describe:: hash(x)
-
-            Returns the partial message's hash.
-
-    Attributes
-    -----------
-    channel: Union[:class:`TextChannel`, :class:`DMChannel`]
-        The channel associated with this partial message.
-    id: :class:`int`
-        The message ID.
-    """
-
-    __slots__ = ('channel', 'id', '_cs_guild', '_state')
-
-    _exported_names = (
-        'jump_url',
-        'delete',
-        'publish',
-        'pin',
-        'unpin',
-        'add_reaction',
-        'remove_reaction',
-        'clear_reaction',
-        'clear_reactions',
-        'reply',
-        'to_reference',
-        'to_message_reference_dict',
-    )
-
-    def __init__(self, *, channel, id):
-        if channel.type not in (ChannelType.text, ChannelType.news, ChannelType.private):
-            raise TypeError('Expected TextChannel or DMChannel not %r' % type(channel))
-
-        self.channel = channel
-        self._state = channel._state
-        self.id = id
-
-    def _update(self, data):
-        # This is used for duck typing purposes.
-        # Just do nothing with the data.
-        pass
-
-    # Also needed for duck typing purposes
-    # n.b. not exposed
-    pinned = property(None, lambda x, y: ...)
-
-    def __repr__(self):
-        return '<PartialMessage id={0.id} channel={0.channel!r}>'.format(self)
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: The partial message's creation time in UTC."""
-        return utils.snowflake_time(self.id)
-
-    @utils.cached_slot_property('_cs_guild')
-    def guild(self):
-        """Optional[:class:`Guild`]: The guild that the partial message belongs to, if applicable."""
-        return getattr(self.channel, 'guild', None)
-
-    async def fetch(self):
-        """|coro|
-
-        Fetches the partial message to a full :class:`Message`.
-
-        Raises
-        --------
-        NotFound
-            The message was not found.
-        Forbidden
-            You do not have the permissions required to get a message.
-        HTTPException
-            Retrieving the message failed.
-
-        Returns
-        --------
-        :class:`Message`
-            The full message.
-        """
-
-        data = await self._state.http.get_message(self.channel.id, self.id)
-        return self._state.create_message(channel=self.channel, data=data)
-
-    async def edit(self, **fields):
-        """|coro|
-
-        Edits the message.
-
-        The content must be able to be transformed into a string via ``str(content)``.
-
-        .. versionchanged:: 1.7
-            :class:`discord.Message` is returned instead of ``None`` if an edit took place.
-
-        Parameters
-        -----------
-        content: Optional[:class:`str`]
-            The new content to replace the message with.
-            Could be ``None`` to remove the content.
-        embed: Optional[:class:`Embed`]
-            The new embed to replace the original with.
-            Could be ``None`` to remove the embed.
-        suppress: :class:`bool`
-            Whether to suppress embeds for the message. This removes
-            all the embeds if set to ``True``. If set to ``False``
-            this brings the embeds back if they were suppressed.
-            Using this parameter requires :attr:`~.Permissions.manage_messages`.
-        delete_after: Optional[:class:`float`]
-            If provided, the number of seconds to wait in the background
-            before deleting the message we just edited. If the deletion fails,
-            then it is silently ignored.
-        allowed_mentions: Optional[:class:`~discord.AllowedMentions`]
-            Controls the mentions being processed in this message. If this is
-            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
-            The merging behaviour only overrides attributes that have been explicitly passed
-            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
-            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
-            are used instead.
-
-        Raises
-        -------
-        NotFound
-            The message was not found.
-        HTTPException
-            Editing the message failed.
-        Forbidden
-            Tried to suppress a message without permissions or
-            edited a message's content or embed that isn't yours.
-
-        Returns
-        ---------
-        Optional[:class:`Message`]
-            The message that was edited.
-        """
-
-        try:
-            content = fields['content']
-        except KeyError:
-            pass
-        else:
-            if content is not None:
-                fields['content'] = str(content)
-
-        try:
-            embed = fields['embed']
-        except KeyError:
-            pass
-        else:
-            if embed is not None:
-                fields['embed'] = embed.to_dict()
-
-        try:
-            suppress = fields.pop('suppress')
-        except KeyError:
-            pass
-        else:
-             flags = MessageFlags._from_value(0)
-             flags.suppress_embeds = suppress
-             fields['flags'] = flags.value
-
-        delete_after = fields.pop('delete_after', None)
-
-        try:
-            allowed_mentions = fields.pop('allowed_mentions')
-        except KeyError:
-            pass
-        else:
-            if allowed_mentions is not None:
-                if self._state.allowed_mentions is not None:
-                    allowed_mentions = self._state.allowed_mentions.merge(allowed_mentions).to_dict()
-                else:
-                    allowed_mentions = allowed_mentions.to_dict()
-                fields['allowed_mentions'] = allowed_mentions
-
-        if fields:
-            data = await self._state.http.edit_message(self.channel.id, self.id, **fields)
-
-        if delete_after is not None:
-            await self.delete(delay=delete_after)
-
-        if fields:
-            return self._state.create_message(channel=self.channel, data=data)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import asyncio
+import datetime
+import re
+import io
+from os import PathLike
+from typing import (
+    AsyncIterator,
+    Dict,
+    Collection,
+    TYPE_CHECKING,
+    Sequence,
+    Union,
+    List,
+    Optional,
+    Any,
+    Callable,
+    Tuple,
+    ClassVar,
+    Type,
+    overload,
+)
+
+from . import utils
+from .reaction import Reaction
+from .emoji import Emoji
+from .partial_emoji import PartialEmoji
+from .calls import CallMessage
+from .enums import MessageType, ChannelType, AppCommandType, try_enum
+from .errors import HTTPException
+from .components import _component_factory
+from .embeds import Embed
+from .member import Member
+from .flags import MessageFlags
+from .file import File
+from .utils import escape_mentions, MISSING
+from .http import handle_message_parameters
+from .guild import Guild
+from .mixins import Hashable
+from .sticker import StickerItem, GuildSticker
+from .threads import Thread
+from .channel import PartialMessageable
+from .interactions import Interaction
+from .commands import MessageCommand
+from .abc import _handle_commands
+from .application import IntegrationApplication
+
+
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
+    from .types.message import (
+        Message as MessagePayload,
+        Attachment as AttachmentPayload,
+        BaseApplication as MessageApplicationPayload,
+        Call as CallPayload,
+        MessageReference as MessageReferencePayload,
+        MessageActivity as MessageActivityPayload,
+        RoleSubscriptionData as RoleSubscriptionDataPayload,
+    )
+
+    from .types.interactions import MessageInteraction as MessageInteractionPayload
+
+    from .types.components import Component as ComponentPayload
+    from .types.threads import ThreadArchiveDuration
+    from .types.member import (
+        Member as MemberPayload,
+        UserWithMember as UserWithMemberPayload,
+    )
+    from .types.user import User as UserPayload
+    from .types.embed import Embed as EmbedPayload
+    from .types.gateway import MessageReactionRemoveEvent, MessageUpdateEvent
+    from .abc import Snowflake
+    from .abc import GuildChannel, MessageableChannel
+    from .components import ActionRow, ActionRowChildComponentType
+    from .state import ConnectionState
+    from .mentions import AllowedMentions
+    from .sticker import GuildSticker
+    from .user import User
+    from .role import Role
+
+    EmojiInputType = Union[Emoji, PartialEmoji, str]
+    MessageComponentType = Union[ActionRow, ActionRowChildComponentType]
+
+
+__all__ = (
+    'Attachment',
+    'Message',
+    'PartialMessage',
+    'MessageReference',
+    'DeletedReferencedMessage',
+    'RoleSubscriptionInfo',
+)
+
+
+def convert_emoji_reaction(emoji: Union[EmojiInputType, Reaction]) -> str:
+    if isinstance(emoji, Reaction):
+        emoji = emoji.emoji
+
+    if isinstance(emoji, Emoji):
+        return f'{emoji.name}:{emoji.id}'
+    if isinstance(emoji, PartialEmoji):
+        return emoji._as_reaction()
+    if isinstance(emoji, str):
+        # Reactions can be in :name:id format, but not <:name:id>
+        # Emojis can't have <> in them, so this should be okay
+        return emoji.strip('<>')
+
+    raise TypeError(f'emoji argument must be str, Emoji, or Reaction not {emoji.__class__.__name__}.')
+
+
+class Attachment(Hashable):
+    """Represents an attachment from Discord.
+
+    .. container:: operations
+
+        .. describe:: str(x)
+
+            Returns the URL of the attachment.
+
+        .. describe:: x == y
+
+            Checks if the attachment is equal to another attachment.
+
+        .. describe:: x != y
+
+            Checks if the attachment is not equal to another attachment.
+
+        .. describe:: hash(x)
+
+            Returns the hash of the attachment.
+
+    .. versionchanged:: 1.7
+        Attachment can now be casted to :class:`str` and is hashable.
+
+    Attributes
+    ------------
+    id: :class:`int`
+        The attachment ID.
+    size: :class:`int`
+        The attachment size in bytes.
+    height: Optional[:class:`int`]
+        The attachment's height, in pixels. Only applicable to images and videos.
+    width: Optional[:class:`int`]
+        The attachment's width, in pixels. Only applicable to images and videos.
+    filename: :class:`str`
+        The attachment's filename.
+    url: :class:`str`
+        The attachment URL. If the message this attachment was attached
+        to is deleted, then this will 404.
+    proxy_url: :class:`str`
+        The proxy URL. This is a cached version of the :attr:`~Attachment.url` in the
+        case of images. When the message is deleted, this URL might be valid for a few
+        minutes or not valid at all.
+    content_type: Optional[:class:`str`]
+        The attachment's `media type <https://en.wikipedia.org/wiki/Media_type>`_
+
+        .. versionadded:: 1.7
+    description: Optional[:class:`str`]
+        The attachment's description. Only applicable to images.
+
+        .. versionadded:: 2.0
+    ephemeral: :class:`bool`
+        Whether the attachment is ephemeral.
+
+        .. versionadded:: 2.0
+    """
+
+    __slots__ = (
+        'id',
+        'size',
+        'height',
+        'width',
+        'filename',
+        'url',
+        'proxy_url',
+        '_http',
+        'content_type',
+        'description',
+        'ephemeral',
+    )
+
+    def __init__(self, *, data: AttachmentPayload, state: ConnectionState):
+        self.id: int = int(data['id'])
+        self.size: int = data['size']
+        self.height: Optional[int] = data.get('height')
+        self.width: Optional[int] = data.get('width')
+        self.filename: str = data['filename']
+        self.url: str = data['url']
+        self.proxy_url: str = data['proxy_url']
+        self._http = state.http
+        self.content_type: Optional[str] = data.get('content_type')
+        self.description: Optional[str] = data.get('description')
+        self.ephemeral: bool = data.get('ephemeral', False)
+
+    def is_spoiler(self) -> bool:
+        """:class:`bool`: Whether this attachment contains a spoiler."""
+        return self.filename.startswith('SPOILER_')
+
+    def __repr__(self) -> str:
+        return f'<Attachment id={self.id} filename={self.filename!r} url={self.url!r}>'
+
+    def __str__(self) -> str:
+        return self.url or ''
+
+    async def save(
+        self,
+        fp: Union[io.BufferedIOBase, PathLike[Any]],
+        *,
+        seek_begin: bool = True,
+        use_cached: bool = False,
+    ) -> int:
+        """|coro|
+
+        Saves this attachment into a file-like object.
+
+        Parameters
+        -----------
+        fp: Union[:class:`io.BufferedIOBase`, :class:`os.PathLike`]
+            The file-like object to save this attachment to or the filename
+            to use. If a filename is passed then a file is created with that
+            filename and used instead.
+        seek_begin: :class:`bool`
+            Whether to seek to the beginning of the file after saving is
+            successfully done.
+        use_cached: :class:`bool`
+            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
+            the attachment. This will allow attachments to be saved after deletion
+            more often, compared to the regular URL which is generally deleted right
+            after the message is deleted. Note that this can still fail to download
+            deleted attachments if too much time has passed and it does not work
+            on some types of attachments.
+
+        Raises
+        --------
+        HTTPException
+            Saving the attachment failed.
+        NotFound
+            The attachment was deleted.
+
+        Returns
+        --------
+        :class:`int`
+            The number of bytes written.
+        """
+        data = await self.read(use_cached=use_cached)
+        if isinstance(fp, io.BufferedIOBase):
+            written = fp.write(data)
+            if seek_begin:
+                fp.seek(0)
+            return written
+        else:
+            with open(fp, 'wb') as f:
+                return f.write(data)
+
+    async def read(self, *, use_cached: bool = False) -> bytes:
+        """|coro|
+
+        Retrieves the content of this attachment as a :class:`bytes` object.
+
+        .. versionadded:: 1.1
+
+        Parameters
+        -----------
+        use_cached: :class:`bool`
+            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
+            the attachment. This will allow attachments to be saved after deletion
+            more often, compared to the regular URL which is generally deleted right
+            after the message is deleted. Note that this can still fail to download
+            deleted attachments if too much time has passed and it does not work
+            on some types of attachments.
+
+        Raises
+        ------
+        HTTPException
+            Downloading the attachment failed.
+        Forbidden
+            You do not have permissions to access this attachment
+        NotFound
+            The attachment was deleted.
+
+        Returns
+        -------
+        :class:`bytes`
+            The contents of the attachment.
+        """
+        url = self.proxy_url if use_cached else self.url
+        data = await self._http.get_from_cdn(url)
+        return data
+
+    async def to_file(
+        self,
+        *,
+        filename: Optional[str] = MISSING,
+        description: Optional[str] = MISSING,
+        use_cached: bool = False,
+        spoiler: bool = False,
+    ) -> File:
+        """|coro|
+
+        Converts the attachment into a :class:`File` suitable for sending via
+        :meth:`abc.Messageable.send`.
+
+        .. versionadded:: 1.3
+
+        Parameters
+        -----------
+        filename: Optional[:class:`str`]
+            The filename to use for the file. If not specified then the filename
+            of the attachment is used instead.
+
+            .. versionadded:: 2.0
+        description: Optional[:class:`str`]
+            The description to use for the file. If not specified then the
+            description of the attachment is used instead.
+
+            .. versionadded:: 2.0
+        use_cached: :class:`bool`
+            Whether to use :attr:`proxy_url` rather than :attr:`url` when downloading
+            the attachment. This will allow attachments to be saved after deletion
+            more often, compared to the regular URL which is generally deleted right
+            after the message is deleted. Note that this can still fail to download
+            deleted attachments if too much time has passed and it does not work
+            on some types of attachments.
+
+            .. versionadded:: 1.4
+        spoiler: :class:`bool`
+            Whether the file is a spoiler.
+
+            .. versionadded:: 1.4
+
+        Raises
+        ------
+        HTTPException
+            Downloading the attachment failed.
+        Forbidden
+            You do not have permissions to access this attachment
+        NotFound
+            The attachment was deleted.
+
+        Returns
+        -------
+        :class:`File`
+            The attachment as a file suitable for sending.
+        """
+
+        data = await self.read(use_cached=use_cached)
+        file_filename = filename if filename is not MISSING else self.filename
+        file_description = description if description is not MISSING else self.description
+        return File(io.BytesIO(data), filename=file_filename, description=file_description, spoiler=spoiler)
+
+    def to_dict(self) -> AttachmentPayload:
+        result: AttachmentPayload = {
+            'filename': self.filename,
+            'id': self.id,
+            'proxy_url': self.proxy_url,
+            'size': self.size,
+            'url': self.url,
+            'spoiler': self.is_spoiler(),
+        }
+        if self.height:
+            result['height'] = self.height
+        if self.width:
+            result['width'] = self.width
+        if self.content_type:
+            result['content_type'] = self.content_type
+        if self.description is not None:
+            result['description'] = self.description
+        return result
+
+
+class DeletedReferencedMessage:
+    """A special sentinel type given when the resolved message reference
+    points to a deleted message.
+
+    The purpose of this class is to separate referenced messages that could not be
+    fetched and those that were previously fetched but have since been deleted.
+
+    .. versionadded:: 1.6
+    """
+
+    __slots__ = ('_parent',)
+
+    def __init__(self, parent: MessageReference):
+        self._parent: MessageReference = parent
+
+    def __repr__(self) -> str:
+        return f"<DeletedReferencedMessage id={self.id} channel_id={self.channel_id} guild_id={self.guild_id!r}>"
+
+    @property
+    def id(self) -> int:
+        """:class:`int`: The message ID of the deleted referenced message."""
+        # The parent's message id won't be None here
+        return self._parent.message_id  # type: ignore
+
+    @property
+    def channel_id(self) -> int:
+        """:class:`int`: The channel ID of the deleted referenced message."""
+        return self._parent.channel_id
+
+    @property
+    def guild_id(self) -> Optional[int]:
+        """Optional[:class:`int`]: The guild ID of the deleted referenced message."""
+        return self._parent.guild_id
+
+
+class MessageReference:
+    """Represents a reference to a :class:`~discord.Message`.
+
+    .. versionadded:: 1.5
+
+    .. versionchanged:: 1.6
+        This class can now be constructed by users.
+
+    Attributes
+    -----------
+    message_id: Optional[:class:`int`]
+        The id of the message referenced.
+    channel_id: :class:`int`
+        The channel id of the message referenced.
+    guild_id: Optional[:class:`int`]
+        The guild id of the message referenced.
+    fail_if_not_exists: :class:`bool`
+        Whether replying to the referenced message should raise :class:`HTTPException`
+        if the message no longer exists or Discord could not fetch the message.
+
+        .. versionadded:: 1.7
+
+    resolved: Optional[Union[:class:`Message`, :class:`DeletedReferencedMessage`]]
+        The message that this reference resolved to. If this is ``None``
+        then the original message was not fetched either due to the Discord API
+        not attempting to resolve it or it not being available at the time of creation.
+        If the message was resolved at a prior point but has since been deleted then
+        this will be of type :class:`DeletedReferencedMessage`.
+
+        Currently, this is mainly the replied to message when a user replies to a message.
+
+        .. versionadded:: 1.6
+    """
+
+    __slots__ = ('message_id', 'channel_id', 'guild_id', 'fail_if_not_exists', 'resolved', '_state')
+
+    def __init__(self, *, message_id: int, channel_id: int, guild_id: Optional[int] = None, fail_if_not_exists: bool = True):
+        self._state: Optional[ConnectionState] = None
+        self.resolved: Optional[Union[Message, DeletedReferencedMessage]] = None
+        self.message_id: Optional[int] = message_id
+        self.channel_id: int = channel_id
+        self.guild_id: Optional[int] = guild_id
+        self.fail_if_not_exists: bool = fail_if_not_exists
+
+    @classmethod
+    def with_state(cls, state: ConnectionState, data: MessageReferencePayload) -> Self:
+        self = cls.__new__(cls)
+        self.message_id = utils._get_as_snowflake(data, 'message_id')
+        self.channel_id = int(data['channel_id'])
+        self.guild_id = utils._get_as_snowflake(data, 'guild_id')
+        self.fail_if_not_exists = data.get('fail_if_not_exists', True)
+        self._state = state
+        self.resolved = None
+        return self
+
+    @classmethod
+    def from_message(cls, message: PartialMessage, *, fail_if_not_exists: bool = True) -> Self:
+        """Creates a :class:`MessageReference` from an existing :class:`~discord.Message`.
+
+        .. versionadded:: 1.6
+
+        Parameters
+        ----------
+        message: :class:`~discord.Message`
+            The message to be converted into a reference.
+        fail_if_not_exists: :class:`bool`
+            Whether replying to the referenced message should raise :class:`HTTPException`
+            if the message no longer exists or Discord could not fetch the message.
+
+            .. versionadded:: 1.7
+
+        Returns
+        -------
+        :class:`MessageReference`
+            A reference to the message.
+        """
+        self = cls(
+            message_id=message.id,
+            channel_id=message.channel.id,
+            guild_id=getattr(message.guild, 'id', None),
+            fail_if_not_exists=fail_if_not_exists,
+        )
+        self._state = message._state
+        return self
+
+    @property
+    def cached_message(self) -> Optional[Message]:
+        """Optional[:class:`~discord.Message`]: The cached message, if found in the internal message cache."""
+        return self._state and self._state._get_message(self.message_id)
+
+    @property
+    def jump_url(self) -> str:
+        """:class:`str`: Returns a URL that allows the client to jump to the referenced message.
+
+        .. versionadded:: 1.7
+        """
+        guild_id = self.guild_id if self.guild_id is not None else '@me'
+        return f'https://discord.com/channels/{guild_id}/{self.channel_id}/{self.message_id}'
+
+    def __repr__(self) -> str:
+        return f'<MessageReference message_id={self.message_id!r} channel_id={self.channel_id!r} guild_id={self.guild_id!r}>'
+
+    def to_dict(self) -> MessageReferencePayload:
+        result: Dict[str, Any] = {'message_id': self.message_id} if self.message_id is not None else {}
+        result['channel_id'] = self.channel_id
+        if self.guild_id is not None:
+            result['guild_id'] = self.guild_id
+        if self.fail_if_not_exists is not None:
+            result['fail_if_not_exists'] = self.fail_if_not_exists
+        return result  # type: ignore # Type checker doesn't understand these are the same
+
+    to_message_reference_dict = to_dict
+
+
+def flatten_handlers(cls: Type[Message]) -> Type[Message]:
+    prefix = len('_handle_')
+    handlers = [
+        (key[prefix:], value)
+        for key, value in cls.__dict__.items()
+        if key.startswith('_handle_') and key != '_handle_member'
+    ]
+
+    # Store _handle_member last
+    handlers.append(('member', cls._handle_member))
+    cls._HANDLERS = handlers
+    cls._CACHED_SLOTS = [attr for attr in cls.__slots__ if attr.startswith('_cs_')]
+    return cls
+
+
+class RoleSubscriptionInfo:
+    """Represents a message's role subscription information.
+
+    This is currently only attached to messages of type :attr:`MessageType.role_subscription_purchase`.
+
+    .. versionadded:: 2.0
+
+    Attributes
+    -----------
+    role_subscription_listing_id: :class:`int`
+        The ID of the SKU and listing that the user is subscribed to.
+    tier_name: :class:`str`
+        The name of the tier that the user is subscribed to.
+    total_months_subscribed: :class:`int`
+        The cumulative number of months that the user has been subscribed for.
+    is_renewal: :class:`bool`
+        Whether this notification is for a renewal rather than a new purchase.
+    """
+
+    __slots__ = (
+        'role_subscription_listing_id',
+        'tier_name',
+        'total_months_subscribed',
+        'is_renewal',
+    )
+
+    def __init__(self, data: RoleSubscriptionDataPayload) -> None:
+        self.role_subscription_listing_id: int = int(data['role_subscription_listing_id'])
+        self.tier_name: str = data['tier_name']
+        self.total_months_subscribed: int = data['total_months_subscribed']
+        self.is_renewal: bool = data['is_renewal']
+
+
+class PartialMessage(Hashable):
+    """Represents a partial message to aid with working messages when only
+    a message and channel ID are present.
+
+    There are two ways to construct this class. The first one is through
+    the constructor itself, and the second is via the following:
+
+    - :meth:`TextChannel.get_partial_message`
+    - :meth:`VoiceChannel.get_partial_message`
+    - :meth:`StageChannel.get_partial_message`
+    - :meth:`Thread.get_partial_message`
+    - :meth:`DMChannel.get_partial_message`
+
+    Note that this class is trimmed down and has no rich attributes.
+
+    .. versionadded:: 1.6
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two partial messages are equal.
+
+        .. describe:: x != y
+
+            Checks if two partial messages are not equal.
+
+        .. describe:: hash(x)
+
+            Returns the partial message's hash.
+
+    Attributes
+    -----------
+    channel: Union[:class:`PartialMessageable`, :class:`TextChannel`, :class:`StageChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`]
+        The channel associated with this partial message.
+    id: :class:`int`
+        The message ID.
+    guild: Optional[:class:`Guild`]
+        The guild that the partial message belongs to, if applicable.
+    """
+
+    __slots__ = ('channel', 'id', '_cs_guild', '_state', 'guild')
+
+    def __init__(self, *, channel: MessageableChannel, id: int) -> None:
+        if not isinstance(channel, PartialMessageable) and channel.type not in (
+            ChannelType.text,
+            ChannelType.voice,
+            ChannelType.stage_voice,
+            ChannelType.news,
+            ChannelType.private,
+            ChannelType.news_thread,
+            ChannelType.public_thread,
+            ChannelType.private_thread,
+        ):
+            raise TypeError(
+                f'expected PartialMessageable, TextChannel, StageChannel, VoiceChannel, DMChannel or Thread not {type(channel)!r}'
+            )
+
+        self.channel: MessageableChannel = channel
+        self._state: ConnectionState = channel._state
+        self.id: int = id
+
+        self.guild: Optional[Guild] = getattr(channel, 'guild', None)
+
+    def _update(self, data: MessageUpdateEvent) -> None:
+        # This is used for duck typing purposes.
+        # Just do nothing with the data.
+        pass
+
+    # Also needed for duck typing purposes
+    # n.b. not exposed
+    pinned: Any = property(None, lambda x, y: None)
+
+    def __repr__(self) -> str:
+        return f'<PartialMessage id={self.id} channel={self.channel!r}>'
+
+    @property
+    def created_at(self) -> datetime.datetime:
+        """:class:`datetime.datetime`: The partial message's creation time in UTC."""
+        return utils.snowflake_time(self.id)
+
+    @property
+    def jump_url(self) -> str:
+        """:class:`str`: Returns a URL that allows the client to jump to this message."""
+        guild_id = getattr(self.guild, 'id', '@me')
+        return f'https://discord.com/channels/{guild_id}/{self.channel.id}/{self.id}'
+
+    async def fetch(self) -> Message:
+        """|coro|
+
+        Fetches the partial message to a full :class:`Message`.
+
+        Raises
+        --------
+        NotFound
+            The message was not found.
+        Forbidden
+            You do not have the permissions required to get a message.
+        HTTPException
+            Retrieving the message failed.
+
+        Returns
+        --------
+        :class:`Message`
+            The full message.
+        """
+        data = await self._state.http.get_message(self.channel.id, self.id)
+        return self._state.create_message(channel=self.channel, data=data)
+
+    async def delete(self, *, delay: Optional[float] = None) -> None:
+        """|coro|
+
+        Deletes the message.
+
+        Your own messages could be deleted without any proper permissions. However to
+        delete other people's messages, you must have :attr:`~Permissions.manage_messages`.
+
+        .. versionchanged:: 1.1
+            Added the new ``delay`` keyword-only parameter.
+
+        Parameters
+        -----------
+        delay: Optional[:class:`float`]
+            If provided, the number of seconds to wait in the background
+            before deleting the message. If the deletion fails then it is silently ignored.
+
+        Raises
+        ------
+        Forbidden
+            You do not have proper permissions to delete the message.
+        NotFound
+            The message was deleted already
+        HTTPException
+            Deleting the message failed.
+        """
+        if delay is not None:
+
+            async def delete(delay: float):
+                await asyncio.sleep(delay)
+                try:
+                    await self._state.http.delete_message(self.channel.id, self.id)
+                except HTTPException:
+                    pass
+
+            asyncio.create_task(delete(delay))
+        else:
+            await self._state.http.delete_message(self.channel.id, self.id)
+
+    @overload
+    async def edit(
+        self,
+        *,
+        content: Optional[str] = ...,
+        attachments: Sequence[Union[Attachment, File]] = ...,
+        delete_after: Optional[float] = ...,
+        allowed_mentions: Optional[AllowedMentions] = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def edit(
+        self,
+        *,
+        content: Optional[str] = ...,
+        attachments: Sequence[Union[Attachment, File]] = ...,
+        delete_after: Optional[float] = ...,
+        allowed_mentions: Optional[AllowedMentions] = ...,
+    ) -> Message:
+        ...
+
+    async def edit(
+        self,
+        content: Optional[str] = MISSING,
+        attachments: Sequence[Union[Attachment, File]] = MISSING,
+        delete_after: Optional[float] = None,
+        allowed_mentions: Optional[AllowedMentions] = MISSING,
+    ) -> Message:
+        """|coro|
+
+        Edits the message.
+
+        The content must be able to be transformed into a string via ``str(content)``.
+
+        .. versionchanged:: 2.0
+            Edits are no longer in-place, the newly edited message is returned instead.
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+        Parameters
+        -----------
+        content: Optional[:class:`str`]
+            The new content to replace the message with.
+            Could be ``None`` to remove the content.
+        attachments: List[Union[:class:`Attachment`, :class:`File`]]
+            A list of attachments to keep in the message as well as new files to upload. If ``[]`` is passed
+            then all attachments are removed.
+
+            .. note::
+
+                New files will always appear after current attachments.
+
+            .. versionadded:: 2.0
+        delete_after: Optional[:class:`float`]
+            If provided, the number of seconds to wait in the background
+            before deleting the message we just edited. If the deletion fails,
+            then it is silently ignored.
+        allowed_mentions: Optional[:class:`~discord.AllowedMentions`]
+            Controls the mentions being processed in this message. If this is
+            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
+            The merging behaviour only overrides attributes that have been explicitly passed
+            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
+            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
+            are used instead.
+
+            .. versionadded:: 1.4
+
+        Raises
+        -------
+        HTTPException
+            Editing the message failed.
+        Forbidden
+            Tried to suppress a message without permissions or
+            edited a message's content or embed that isn't yours.
+        TypeError
+            You specified both ``embed`` and ``embeds``
+
+        Returns
+        --------
+        :class:`Message`
+            The newly edited message.
+        """
+        if content is not MISSING:
+            previous_allowed_mentions = self._state.allowed_mentions
+        else:
+            previous_allowed_mentions = None
+
+        with handle_message_parameters(
+            content=content,
+            attachments=attachments,
+            allowed_mentions=allowed_mentions,
+            previous_allowed_mentions=previous_allowed_mentions,
+        ) as params:
+            data = await self._state.http.edit_message(self.channel.id, self.id, params=params)
+            message = Message(state=self._state, channel=self.channel, data=data)
+
+        if delete_after is not None:
+            await self.delete(delay=delete_after)
+
+        return message
+
+    async def publish(self) -> None:
+        """|coro|
+
+        Publishes this message to the channel's followers.
+
+        The message must have been sent in a news channel.
+        You must have :attr:`~Permissions.send_messages` to do this.
+
+        If the message is not your own then :attr:`~Permissions.manage_messages`
+        is also needed.
+
+        Raises
+        -------
+        Forbidden
+            You do not have the proper permissions to publish this message
+            or the channel is not a news channel.
+        HTTPException
+            Publishing the message failed.
+        """
+        await self._state.http.publish_message(self.channel.id, self.id)
+
+    async def pin(self, *, reason: Optional[str] = None) -> None:
+        """|coro|
+
+        Pins the message.
+
+        You must have :attr:`~Permissions.manage_messages` to do
+        this in a non-private channel context.
+
+        Parameters
+        -----------
+        reason: Optional[:class:`str`]
+            The reason for pinning the message. Shows up on the audit log.
+
+            .. versionadded:: 1.4
+
+        Raises
+        -------
+        Forbidden
+            You do not have permissions to pin the message.
+        NotFound
+            The message or channel was not found or deleted.
+        HTTPException
+            Pinning the message failed, probably due to the channel
+            having more than 50 pinned messages.
+        """
+        await self._state.http.pin_message(self.channel.id, self.id, reason=reason)
+        # pinned exists on PartialMessage for duck typing purposes
+        self.pinned = True
+
+    async def unpin(self, *, reason: Optional[str] = None) -> None:
+        """|coro|
+
+        Unpins the message.
+
+        You must have :attr:`~Permissions.manage_messages` to do
+        this in a non-private channel context.
+
+        Parameters
+        -----------
+        reason: Optional[:class:`str`]
+            The reason for unpinning the message. Shows up on the audit log.
+
+            .. versionadded:: 1.4
+
+        Raises
+        -------
+        Forbidden
+            You do not have permissions to unpin the message.
+        NotFound
+            The message or channel was not found or deleted.
+        HTTPException
+            Unpinning the message failed.
+        """
+        await self._state.http.unpin_message(self.channel.id, self.id, reason=reason)
+        # pinned exists on PartialMessage for duck typing purposes
+        self.pinned = False
+
+    async def add_reaction(self, emoji: Union[EmojiInputType, Reaction], /) -> None:
+        """|coro|
+
+        Adds a reaction to the message.
+
+        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
+
+        You must have :attr:`~Permissions.read_message_history`
+        to do this. If nobody else has reacted to the message using this
+        emoji, :attr:`~Permissions.add_reactions` is required.
+
+        .. versionchanged:: 2.0
+
+            ``emoji`` parameter is now positional-only.
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+        Parameters
+        ------------
+        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
+            The emoji to react with.
+
+        Raises
+        --------
+        HTTPException
+            Adding the reaction failed.
+        Forbidden
+            You do not have the proper permissions to react to the message.
+        NotFound
+            The emoji you specified was not found.
+        TypeError
+            The emoji parameter is invalid.
+        """
+        emoji = convert_emoji_reaction(emoji)
+        await self._state.http.add_reaction(self.channel.id, self.id, emoji)
+
+    async def remove_reaction(self, emoji: Union[EmojiInputType, Reaction], member: Snowflake) -> None:
+        """|coro|
+
+        Remove a reaction by the member from the message.
+
+        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
+
+        If the reaction is not your own (i.e. ``member`` parameter is not you) then
+        :attr:`~Permissions.manage_messages` is needed.
+
+        The ``member`` parameter must represent a member and meet
+        the :class:`abc.Snowflake` abc.
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+        Parameters
+        ------------
+        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
+            The emoji to remove.
+        member: :class:`abc.Snowflake`
+            The member for which to remove the reaction.
+
+        Raises
+        --------
+        HTTPException
+            Removing the reaction failed.
+        Forbidden
+            You do not have the proper permissions to remove the reaction.
+        NotFound
+            The member or emoji you specified was not found.
+        TypeError
+            The emoji parameter is invalid.
+        """
+        emoji = convert_emoji_reaction(emoji)
+
+        if member.id == self._state.self_id:
+            await self._state.http.remove_own_reaction(self.channel.id, self.id, emoji)
+        else:
+            await self._state.http.remove_reaction(self.channel.id, self.id, emoji, member.id)
+
+    async def clear_reaction(self, emoji: Union[EmojiInputType, Reaction]) -> None:
+        """|coro|
+
+        Clears a specific reaction from the message.
+
+        The emoji may be a unicode emoji or a custom guild :class:`Emoji`.
+
+        You must have :attr:`~Permissions.manage_messages` to do this.
+
+        .. versionadded:: 1.3
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+        Parameters
+        -----------
+        emoji: Union[:class:`Emoji`, :class:`Reaction`, :class:`PartialEmoji`, :class:`str`]
+            The emoji to clear.
+
+        Raises
+        --------
+        HTTPException
+            Clearing the reaction failed.
+        Forbidden
+            You do not have the proper permissions to clear the reaction.
+        NotFound
+            The emoji you specified was not found.
+        TypeError
+            The emoji parameter is invalid.
+        """
+        emoji = convert_emoji_reaction(emoji)
+        await self._state.http.clear_single_reaction(self.channel.id, self.id, emoji)
+
+    async def clear_reactions(self) -> None:
+        """|coro|
+
+        Removes all the reactions from the message.
+
+        You must have :attr:`~Permissions.manage_messages` to do this.
+
+        Raises
+        --------
+        HTTPException
+            Removing the reactions failed.
+        Forbidden
+            You do not have the proper permissions to remove all the reactions.
+        """
+        await self._state.http.clear_reactions(self.channel.id, self.id)
+
+    async def create_thread(
+        self,
+        *,
+        name: str,
+        auto_archive_duration: ThreadArchiveDuration = MISSING,
+        slowmode_delay: Optional[int] = None,
+        reason: Optional[str] = None,
+    ) -> Thread:
+        """|coro|
+
+        Creates a public thread from this message.
+
+        You must have :attr:`~discord.Permissions.create_public_threads` in order to
+        create a public thread from a message.
+
+        The channel this message belongs in must be a :class:`TextChannel`.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the thread.
+        auto_archive_duration: :class:`int`
+            The duration in minutes before a thread is automatically archived for inactivity.
+            If not provided, the channel's default auto archive duration is used.
+
+            Must be one of ``60``, ``1440``, ``4320``, or ``10080``, if provided.
+        slowmode_delay: Optional[:class:`int`]
+            Specifies the slowmode rate limit for user in this channel, in seconds.
+            The maximum value possible is ``21600``. By default no slowmode rate limit
+            if this is ``None``.
+        reason: Optional[:class:`str`]
+            The reason for creating a new thread. Shows up on the audit log.
+
+        Raises
+        -------
+        Forbidden
+            You do not have permissions to create a thread.
+        HTTPException
+            Creating the thread failed.
+        ValueError
+            This message does not have guild info attached.
+
+        Returns
+        --------
+        :class:`.Thread`
+            The created thread.
+        """
+        if self.guild is None:
+            raise ValueError('This message does not have guild info attached')
+
+        default_auto_archive_duration: ThreadArchiveDuration = getattr(self.channel, 'default_auto_archive_duration', 1440)
+        data = await self._state.http.start_thread_with_message(
+            self.channel.id,
+            self.id,
+            name=name,
+            auto_archive_duration=auto_archive_duration or default_auto_archive_duration,
+            rate_limit_per_user=slowmode_delay,
+            reason=reason,
+            location='Message',
+        )
+        return Thread(guild=self.guild, state=self._state, data=data)
+
+    async def ack(self) -> None:
+        """|coro|
+
+        Marks this message as read.
+
+        Raises
+        -------
+        HTTPException
+            Acking failed.
+        """
+        await self._state.http.ack_message(self.channel.id, self.id)
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        mention_author: bool = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    async def reply(self, content: Optional[str] = None, **kwargs: Any) -> Message:
+        """|coro|
+
+        A shortcut method to :meth:`.abc.Messageable.send` to reply to the
+        :class:`.Message`.
+
+        .. versionadded:: 1.6
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` or
+            :exc:`ValueError` instead of ``InvalidArgument``.
+
+        Raises
+        --------
+        ~discord.HTTPException
+            Sending the message failed.
+        ~discord.Forbidden
+            You do not have the proper permissions to send the message.
+        ValueError
+            The ``files`` list is not of the appropriate size
+        TypeError
+            You specified both ``file`` and ``files``.
+
+        Returns
+        ---------
+        :class:`.Message`
+            The message that was sent.
+        """
+        return await self.channel.send(content, reference=self, **kwargs)
+
+    @overload
+    async def greet(
+        self,
+        sticker: Union[GuildSticker, StickerItem],
+        *,
+        allowed_mentions: AllowedMentions = ...,
+        mention_author: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def greet(self, sticker: Union[GuildSticker, StickerItem]) -> Message:
+        ...
+
+    async def greet(self, sticker: Union[GuildSticker, StickerItem], **kwargs: Any) -> Message:
+        """|coro|
+
+        A shortcut method to :meth:`.abc.Messageable.greet` to reply to the
+        :class:`.Message` with a sticker greeting.
+
+        .. versionadded:: 2.0
+
+        Raises
+        --------
+        ~discord.HTTPException
+            Sending the message failed.
+        ~discord.Forbidden
+            You do not have the proper permissions to send the message, or this is not a valid greet context.
+
+        Returns
+        ---------
+        :class:`.Message`
+            The sticker greeting that was sent.
+        """
+        return await self.channel.greet(sticker, reference=self, **kwargs)
+
+    def to_reference(self, *, fail_if_not_exists: bool = True) -> MessageReference:
+        """Creates a :class:`~discord.MessageReference` from the current message.
+
+        .. versionadded:: 1.6
+
+        Parameters
+        ----------
+        fail_if_not_exists: :class:`bool`
+            Whether replying using the message reference should raise :class:`HTTPException`
+            if the message no longer exists or Discord could not fetch the message.
+
+            .. versionadded:: 1.7
+
+        Returns
+        ---------
+        :class:`~discord.MessageReference`
+            The reference to this message.
+        """
+        return MessageReference.from_message(self, fail_if_not_exists=fail_if_not_exists)
+
+    def to_message_reference_dict(self) -> MessageReferencePayload:
+        data: MessageReferencePayload = {
+            'message_id': self.id,
+            'channel_id': self.channel.id,
+        }
+
+        if self.guild is not None:
+            data['guild_id'] = self.guild.id
+
+        return data
+
+
+@flatten_handlers
+class Message(PartialMessage, Hashable):
+    r"""Represents a message from Discord.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two messages are equal.
+
+        .. describe:: x != y
+
+            Checks if two messages are not equal.
+
+        .. describe:: hash(x)
+
+            Returns the message's hash.
+
+    Attributes
+    -----------
+    tts: :class:`bool`
+        Specifies if the message was done with text-to-speech.
+        This can only be accurately received in :func:`on_message` due to
+        a discord limitation.
+    type: :class:`MessageType`
+        The type of message. In most cases this should not be checked, but it is helpful
+        in cases where it might be a system message for :attr:`system_content`.
+    author: Union[:class:`Member`, :class:`abc.User`]
+        A :class:`Member` that sent the message. If :attr:`channel` is a
+        private channel or the user has the left the guild, then it is a :class:`User` instead.
+    content: :class:`str`
+        The actual contents of the message.
+    nonce: Optional[Union[:class:`str`, :class:`int`]]
+        The value used by Discord clients to verify that the message is successfully sent.
+        This is not stored long term within Discord's servers and is only used ephemerally.
+    embeds: List[:class:`Embed`]
+        A list of embeds the message has.
+    channel: Union[:class:`TextChannel`, :class:`StageChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`, :class:`GroupChannel`]
+        The :class:`TextChannel` or :class:`Thread` that the message was sent from.
+        Could be a :class:`DMChannel` or :class:`GroupChannel` if it's a private message.
+    call: Optional[:class:`CallMessage`]
+        The call that the message refers to. This is only applicable to messages of type
+        :attr:`MessageType.call`.
+    reference: Optional[:class:`~discord.MessageReference`]
+        The message that this message references. This is only applicable to messages of
+        type :attr:`MessageType.pins_add`, crossposted messages created by a
+        followed channel integration, or message replies.
+
+        .. versionadded:: 1.5
+
+    mention_everyone: :class:`bool`
+        Specifies if the message mentions everyone.
+
+        .. note::
+
+            This does not check if the ``@everyone`` or the ``@here`` text is in the message itself.
+            Rather this boolean indicates if either the ``@everyone`` or the ``@here`` text is in the message
+            **and** it did end up mentioning.
+    mentions: List[:class:`abc.User`]
+        A list of :class:`Member` that were mentioned. If the message is in a private message
+        then the list will be of :class:`User` instead. For messages that are not of type
+        :attr:`MessageType.default`\, this array can be used to aid in system messages.
+        For more information, see :attr:`system_content`.
+
+        .. warning::
+
+            The order of the mentions list is not in any particular order so you should
+            not rely on it. This is a Discord limitation, not one with the library.
+    channel_mentions: List[Union[:class:`abc.GuildChannel`, :class:`Thread`]]
+        A list of :class:`abc.GuildChannel` or :class:`Thread` that were mentioned. If the message is
+        in a private message then the list is always empty.
+    role_mentions: List[:class:`Role`]
+        A list of :class:`Role` that were mentioned. If the message is in a private message
+        then the list is always empty.
+    id: :class:`int`
+        The message ID.
+    webhook_id: Optional[:class:`int`]
+        If this message was sent by a webhook, then this is the webhook ID's that sent this
+        message.
+    attachments: List[:class:`Attachment`]
+        A list of attachments given to a message.
+    pinned: :class:`bool`
+        Specifies if the message is currently pinned.
+    flags: :class:`MessageFlags`
+        Extra features of the message.
+
+        .. versionadded:: 1.3
+
+    reactions : List[:class:`Reaction`]
+        Reactions to a message. Reactions can be either custom emoji or standard unicode emoji.
+    activity: Optional[:class:`dict`]
+        The activity associated with this message. Sent with Rich-Presence related messages that for
+        example, request joining, spectating, or listening to or with another member.
+
+        It is a dictionary with the following optional keys:
+
+        - ``type``: An integer denoting the type of message activity being requested.
+        - ``party_id``: The party ID associated with the party.
+    application: Optional[:class:`IntegrationApplication`]
+        The rich presence enabled application associated with this message.
+
+        .. versionchanged:: 2.0
+
+            Type is now :class:`IntegrationApplication` instead of :class:`dict`.
+    stickers: List[:class:`StickerItem`]
+        A list of sticker items given to the message.
+
+        .. versionadded:: 1.6
+    components: List[Union[:class:`ActionRow`, :class:`Button`, :class:`SelectMenu`]]
+        A list of components in the message.
+
+        .. versionadded:: 2.0
+    role_subscription: Optional[:class:`RoleSubscriptionInfo`]
+        The data of the role subscription purchase or renewal that prompted this
+        :attr:`MessageType.role_subscription_purchase` message.
+
+        .. versionadded:: 2.0
+    application_id: Optional[:class:`int`]
+        The application ID of the application that created this message if this
+        message was sent by an application-owned webhook or an interaction.
+
+        .. versionadded:: 2.0
+    position: Optional[:class:`int`]
+        A generally increasing integer with potentially gaps or duplicates that represents
+        the approximate position of the message in a thread.
+
+        .. versionadded:: 2.0
+    guild: Optional[:class:`Guild`]
+        The guild that the message belongs to, if applicable.
+    interaction: Optional[:class:`Interaction`]
+        The interaction that this message is a response to.
+
+        .. versionadded:: 2.0
+    """
+
+    __slots__ = (
+        '_edited_timestamp',
+        '_cs_channel_mentions',
+        '_cs_raw_mentions',
+        '_cs_clean_content',
+        '_cs_raw_channel_mentions',
+        '_cs_raw_role_mentions',
+        '_cs_system_content',
+        'tts',
+        'content',
+        'webhook_id',
+        'mention_everyone',
+        'embeds',
+        'mentions',
+        'author',
+        'attachments',
+        'nonce',
+        'pinned',
+        'role_mentions',
+        'type',
+        'flags',
+        'reactions',
+        'reference',
+        'application',
+        'activity',
+        'stickers',
+        'components',
+        'call',
+        'interaction',
+        'role_subscription',
+        'application_id',
+        'position',
+    )
+
+    if TYPE_CHECKING:
+        _HANDLERS: ClassVar[List[Tuple[str, Callable[..., None]]]]
+        _CACHED_SLOTS: ClassVar[List[str]]
+        reference: Optional[MessageReference]
+        mentions: List[Union[User, Member]]
+        author: Union[User, Member]
+        role_mentions: List[Role]
+        components: List[MessageComponentType]
+
+    def __init__(
+        self,
+        *,
+        state: ConnectionState,
+        channel: MessageableChannel,
+        data: MessagePayload,
+    ) -> None:
+        self.channel: MessageableChannel = channel
+        self.id: int = int(data['id'])
+        self._state: ConnectionState = state
+        self.webhook_id: Optional[int] = utils._get_as_snowflake(data, 'webhook_id')
+        self.reactions: List[Reaction] = [Reaction(message=self, data=d) for d in data.get('reactions', [])]
+        self.attachments: List[Attachment] = [Attachment(data=a, state=self._state) for a in data['attachments']]
+        self.embeds: List[Embed] = [Embed.from_dict(a) for a in data['embeds']]
+        self.activity: Optional[MessageActivityPayload] = data.get('activity')
+        self._edited_timestamp: Optional[datetime.datetime] = utils.parse_time(data['edited_timestamp'])
+        self.type: MessageType = try_enum(MessageType, data['type'])
+        self.pinned: bool = data['pinned']
+        self.flags: MessageFlags = MessageFlags._from_value(data.get('flags', 0))
+        self.mention_everyone: bool = data['mention_everyone']
+        self.tts: bool = data['tts']
+        self.content: str = data['content']
+        self.nonce: Optional[Union[int, str]] = data.get('nonce')
+        self.position: Optional[int] = data.get('position')
+        self.application_id: Optional[int] = utils._get_as_snowflake(data, 'application_id')
+        self.stickers: List[StickerItem] = [StickerItem(data=d, state=state) for d in data.get('sticker_items', [])]
+        self.call: Optional[CallMessage] = None
+
+        try:
+            # If the channel doesn't have a guild attribute, we handle that
+            self.guild = channel.guild
+        except AttributeError:
+            self.guild = state._get_guild(utils._get_as_snowflake(data, 'guild_id'))
+
+        self.application: Optional[IntegrationApplication] = None
+        try:
+            application = data['application']
+        except KeyError:
+            pass
+        else:
+            self.application = IntegrationApplication(state=self._state, data=application)
+
+        self.interaction: Optional[Interaction] = None
+        try:
+            interaction = data['interaction']
+        except KeyError:
+            pass
+        else:
+            self.interaction = Interaction._from_message(self, **interaction)
+
+        try:
+            ref = data['message_reference']
+        except KeyError:
+            self.reference = None
+        else:
+            self.reference = ref = MessageReference.with_state(state, ref)
+            try:
+                resolved = data['referenced_message']
+            except KeyError:
+                pass
+            else:
+                if resolved is None:
+                    ref.resolved = DeletedReferencedMessage(ref)
+                else:
+                    # Right now the channel IDs match but maybe in the future they won't
+                    if ref.channel_id == channel.id:
+                        chan = channel
+                    elif isinstance(channel, Thread) and channel.parent_id == ref.channel_id:
+                        chan = channel
+                    else:
+                        chan, _ = state._get_guild_channel(resolved, ref.guild_id)
+
+                    # The channel will be the correct type here
+                    ref.resolved = self.__class__(channel=chan, data=resolved, state=state)  # type: ignore
+
+        self.role_subscription: Optional[RoleSubscriptionInfo] = None
+        try:
+            role_subscription = data['role_subscription_data']
+        except KeyError:
+            pass
+        else:
+            self.role_subscription = RoleSubscriptionInfo(role_subscription)
+
+        for handler in ('author', 'member', 'mentions', 'mention_roles', 'call', 'interaction', 'components'):
+            try:
+                getattr(self, f'_handle_{handler}')(data[handler])
+            except KeyError:
+                continue
+
+    def __repr__(self) -> str:
+        name = self.__class__.__name__
+        return (
+            f'<{name} id={self.id} channel={self.channel!r} type={self.type!r} author={self.author!r} flags={self.flags!r}>'
+        )
+
+    async def _get_channel(self) -> MessageableChannel:
+        return self.channel
+
+    def _try_patch(self, data, key, transform=None) -> None:
+        try:
+            value = data[key]
+        except KeyError:
+            pass
+        else:
+            if transform is None:
+                setattr(self, key, value)
+            else:
+                setattr(self, key, transform(value))
+
+    def _add_reaction(self, data, emoji, user_id) -> Reaction:
+        reaction = utils.find(lambda r: r.emoji == emoji, self.reactions)
+        is_me = data['me'] = user_id == self._state.self_id
+
+        if reaction is None:
+            reaction = Reaction(message=self, data=data, emoji=emoji)
+            self.reactions.append(reaction)
+        else:
+            reaction.count += 1
+            if is_me:
+                reaction.me = is_me
+
+        return reaction
+
+    def _remove_reaction(self, data: MessageReactionRemoveEvent, emoji: EmojiInputType, user_id: int) -> Reaction:
+        reaction = utils.find(lambda r: r.emoji == emoji, self.reactions)
+
+        if reaction is None:
+            # Already removed?
+            raise ValueError('Emoji already removed?')
+
+        # If reaction isn't in the list, we crash; this means Discord
+        # sent bad data, or we stored improperly
+        reaction.count -= 1
+
+        if user_id == self._state.self_id:
+            reaction.me = False
+        if reaction.count == 0:
+            # This raises ValueError if something went wrong as well
+            self.reactions.remove(reaction)
+
+        return reaction
+
+    def _clear_emoji(self, emoji: PartialEmoji) -> Optional[Reaction]:
+        to_check = str(emoji)
+        for index, reaction in enumerate(self.reactions):
+            if str(reaction.emoji) == to_check:
+                break
+        else:
+            # Didn't find anything so just return
+            return
+
+        del self.reactions[index]
+        return reaction
+
+    def _update(self, data: MessageUpdateEvent) -> None:
+        # In an update scheme, 'author' key has to be handled before 'member'
+        # otherwise they overwrite each other which is undesirable
+        # Since there's no good way to do this we have to iterate over every
+        # handler rather than iterating over the keys which is a little slower
+        for key, handler in self._HANDLERS:
+            try:
+                value = data[key]
+            except KeyError:
+                continue
+            else:
+                handler(self, value)
+
+        # Clear the cached properties
+        for attr in self._CACHED_SLOTS:
+            try:
+                delattr(self, attr)
+            except AttributeError:
+                pass
+
+    def _handle_edited_timestamp(self, value: str) -> None:
+        self._edited_timestamp = utils.parse_time(value)
+
+    def _handle_pinned(self, value: bool) -> None:
+        self.pinned = value
+
+    def _handle_flags(self, value: int) -> None:
+        self.flags = MessageFlags._from_value(value)
+
+    def _handle_application(self, value: MessageApplicationPayload) -> None:
+        application = IntegrationApplication(state=self._state, data=value)
+        self.application = application
+
+    def _handle_activity(self, value: MessageActivityPayload) -> None:
+        self.activity = value
+
+    def _handle_mention_everyone(self, value: bool) -> None:
+        self.mention_everyone = value
+
+    def _handle_tts(self, value: bool) -> None:
+        self.tts = value
+
+    def _handle_type(self, value: int) -> None:
+        self.type = try_enum(MessageType, value)
+
+    def _handle_content(self, value: str) -> None:
+        self.content = value
+
+    def _handle_attachments(self, value: List[AttachmentPayload]) -> None:
+        self.attachments = [Attachment(data=a, state=self._state) for a in value]
+
+    def _handle_embeds(self, value: List[EmbedPayload]) -> None:
+        self.embeds = [Embed.from_dict(data) for data in value]
+
+    def _handle_nonce(self, value: Union[str, int]) -> None:
+        self.nonce = value
+
+    def _handle_author(self, author: UserPayload) -> None:
+        self.author = self._state.store_user(author)
+        if isinstance(self.guild, Guild):
+            found = self.guild.get_member(self.author.id)
+            if found is not None:
+                self.author = found
+
+    def _handle_member(self, member: MemberPayload) -> None:
+        # The gateway now gives us full Member objects sometimes with the following keys
+        # deaf, mute, joined_at, roles
+        # For the sake of performance I'm going to assume that the only
+        # field that needs *updating* would be the joined_at field
+        # If there is no Member object (for some strange reason), then we can upgrade
+        # ourselves to a more "partial" member object
+        author = self.author
+        try:
+            # Update member reference
+            author._update_from_message(member)  # type: ignore
+        except AttributeError:
+            # It's a user here
+            # TODO: consider adding to cache here
+            self.author = Member._from_message(message=self, data=member)
+
+    def _handle_mentions(self, mentions: List[UserWithMemberPayload]) -> None:
+        self.mentions = r = []
+        guild = self.guild
+        state = self._state
+        if not isinstance(guild, Guild):
+            self.mentions = [state.store_user(m) for m in mentions]
+            return
+
+        for mention in filter(None, mentions):
+            id_search = int(mention['id'])
+            member = guild.get_member(id_search)
+            if member is not None:
+                r.append(member)
+            else:
+                r.append(Member._try_upgrade(data=mention, guild=guild, state=state))
+
+    def _handle_mention_roles(self, role_mentions: List[int]) -> None:
+        self.role_mentions = []
+        if isinstance(self.guild, Guild):
+            for role_id in map(int, role_mentions):
+                role = self.guild.get_role(role_id)
+                if role is not None:
+                    self.role_mentions.append(role)
+
+    def _handle_call(self, call: Optional[CallPayload]) -> None:
+        if call is None or self.type is not MessageType.call:
+            self.call = None
+            return
+
+        participants = []
+        for uid in map(int, call.get('participants', [])):
+            if uid == self.author.id:
+                participants.append(self.author)
+            else:
+                user = utils.find(lambda u: u.id == uid, self.mentions)
+                if user is not None:
+                    participants.append(user)
+
+        self.call = CallMessage(message=self, ended_timestamp=call.get('ended_timestamp'), participants=participants)
+
+    def _handle_components(self, data: List[ComponentPayload]) -> None:
+        self.components = []
+
+        for component_data in data:
+            component = _component_factory(component_data, self)
+
+            if component is not None:
+                self.components.append(component)
+
+    def _handle_interaction(self, data: MessageInteractionPayload):
+        self.interaction = Interaction._from_message(self, **data)
+
+    def _rebind_cached_references(
+        self,
+        new_guild: Guild,
+        new_channel: Union[GuildChannel, Thread, PartialMessageable],
+    ) -> None:
+        self.guild = new_guild
+        self.channel = new_channel  # type: ignore # Not all "GuildChannel" are messageable at the moment
+
+    @utils.cached_slot_property('_cs_raw_mentions')
+    def raw_mentions(self) -> List[int]:
+        """List[:class:`int`]: A property that returns an array of user IDs matched with
+        the syntax of ``<@user_id>`` in the message content.
+
+        This allows you to receive the user IDs of mentioned users
+        even in a private message context.
+        """
+        return [int(x) for x in re.findall(r'<@!?([0-9]{15,20})>', self.content)]
+
+    @utils.cached_slot_property('_cs_raw_channel_mentions')
+    def raw_channel_mentions(self) -> List[int]:
+        """List[:class:`int`]: A property that returns an array of channel IDs matched with
+        the syntax of ``<#channel_id>`` in the message content.
+        """
+        return [int(x) for x in re.findall(r'<#([0-9]{15,20})>', self.content)]
+
+    @utils.cached_slot_property('_cs_raw_role_mentions')
+    def raw_role_mentions(self) -> List[int]:
+        """List[:class:`int`]: A property that returns an array of role IDs matched with
+        the syntax of ``<@&role_id>`` in the message content.
+        """
+        return [int(x) for x in re.findall(r'<@&([0-9]{15,20})>', self.content)]
+
+    @utils.cached_slot_property('_cs_channel_mentions')
+    def channel_mentions(self) -> List[Union[GuildChannel, Thread]]:
+        if self.guild is None:
+            return []
+        it = filter(None, map(self.guild._resolve_channel, self.raw_channel_mentions))
+        return utils._unique(it)
+
+    @utils.cached_slot_property('_cs_clean_content')
+    def clean_content(self) -> str:
+        """:class:`str`: A property that returns the content in a "cleaned up"
+        manner. This basically means that mentions are transformed
+        into the way the client shows it. e.g. ``<#id>`` will transform
+        into ``#name``.
+
+        This will also transform @everyone and @here mentions into
+        non-mentions.
+
+        .. note::
+
+            This *does not* affect markdown. If you want to escape
+            or remove markdown then use :func:`utils.escape_markdown` or :func:`utils.remove_markdown`
+            respectively, along with this function.
+        """
+
+        if self.guild:
+
+            def resolve_member(id: int) -> str:
+                m = self.guild.get_member(id) or utils.get(self.mentions, id=id)  # type: ignore
+                return f'@{m.display_name}' if m else '@deleted-user'
+
+            def resolve_role(id: int) -> str:
+                r = self.guild.get_role(id) or utils.get(self.role_mentions, id=id)  # type: ignore
+                return f'@{r.name}' if r else '@deleted-role'
+
+            def resolve_channel(id: int) -> str:
+                c = self.guild._resolve_channel(id)  # type: ignore
+                return f'#{c.name}' if c else '#deleted-channel'
+
+        else:
+
+            def resolve_member(id: int) -> str:
+                m = utils.get(self.mentions, id=id)
+                return f'@{m.display_name}' if m else '@deleted-user'
+
+            def resolve_role(id: int) -> str:
+                return '@deleted-role'
+
+            def resolve_channel(id: int) -> str:
+                return '#deleted-channel'
+
+        transforms = {
+            '@': resolve_member,
+            '@!': resolve_member,
+            '#': resolve_channel,
+            '@&': resolve_role,
+        }
+
+        def repl(match: re.Match) -> str:
+            type = match[1]
+            id = int(match[2])
+            transformed = transforms[type](id)
+            return transformed
+
+        result = re.sub(r'<(@[!&]?|#)([0-9]{15,20})>', repl, self.content)
+
+        return escape_mentions(result)
+
+    @property
+    def created_at(self) -> datetime.datetime:
+        """:class:`datetime.datetime`: The message's creation time in UTC."""
+        return utils.snowflake_time(self.id)
+
+    @property
+    def edited_at(self) -> Optional[datetime.datetime]:
+        """Optional[:class:`datetime.datetime`]: An aware UTC datetime object containing the edited time of the message."""
+        return self._edited_timestamp
+
+    def is_system(self) -> bool:
+        """:class:`bool`: Whether the message is a system message.
+
+        A system message is a message that is constructed entirely by the Discord API
+        in response to something.
+
+        .. versionadded:: 1.3
+        """
+        return self.type not in (
+            MessageType.default,
+            MessageType.reply,
+            MessageType.chat_input_command,
+            MessageType.context_menu_command,
+            MessageType.thread_starter_message,
+        )
+
+    @utils.cached_slot_property('_cs_system_content')
+    def system_content(self) -> str:
+        r""":class:`str`: A property that returns the content that is rendered
+        regardless of the :attr:`Message.type`.
+
+        In the case of :attr:`MessageType.default` and :attr:`MessageType.reply`\,
+        this just returns the regular :attr:`Message.content`. Otherwise this
+        returns an English message denoting the contents of the system message.
+        """
+        if self.type is MessageType.recipient_add:
+            if self.channel.type is ChannelType.group:
+                return f'{self.author.name} added {self.mentions[0].name} to the group.'
+            else:
+                return f'{self.author.name} added {self.mentions[0].name} to the thread.'
+
+        if self.type is MessageType.recipient_remove:
+            if self.channel.type is ChannelType.group:
+                return f'{self.author.name} removed {self.mentions[0].name} from the group.'
+            else:
+                return f'{self.author.name} removed {self.mentions[0].name} from the thread.'
+
+        if self.type is MessageType.channel_name_change:
+            if getattr(self.channel, 'parent', self.channel).type is ChannelType.forum:
+                return f'{self.author.name} changed the post title: **{self.content}**'
+            else:
+                return f'{self.author.name} changed the channel name: **{self.content}**'
+
+        if self.type is MessageType.channel_icon_change:
+            return f'{self.author.name} changed the channel icon.'
+
+        if self.type is MessageType.pins_add:
+            return f'{self.author.name} pinned a message to this channel.'
+
+        if self.type is MessageType.new_member:
+            formats = [
+                "{0} joined the party.",
+                "{0} is here.",
+                "Welcome, {0}. We hope you brought pizza.",
+                "A wild {0} appeared.",
+                "{0} just landed.",
+                "{0} just slid into the server.",
+                "{0} just showed up!",
+                "Welcome {0}. Say hi!",
+                "{0} hopped into the server.",
+                "Everyone welcome {0}!",
+                "Glad you're here, {0}.",
+                "Good to see you, {0}.",
+                "Yay you made it, {0}!",
+            ]
+
+            created_at_ms = int(self.created_at.timestamp() * 1000)
+            return formats[created_at_ms % len(formats)].format(self.author.name)
+
+        if self.type is MessageType.call:
+            call_ended = self.call.ended_timestamp is not None  # type: ignore
+
+            if self.channel.me in self.call.participants:  # type: ignore
+                return f'{self.author.name} started a call.'
+            elif call_ended:
+                return f'You missed a call from {self.author.name} that lasted {int((utils.utcnow() - self.call.ended_timestamp).total_seconds())} seconds.'  # type: ignore
+            else:
+                return f'{self.author.name} started a call \N{EM DASH} Join the call.'
+
+        if self.type is MessageType.premium_guild_subscription:
+            if not self.content:
+                return f'{self.author.name} just boosted the server!'
+            else:
+                return f'{self.author.name} just boosted the server **{self.content}** times!'
+
+        if self.type is MessageType.premium_guild_tier_1:
+            if not self.content:
+                return f'{self.author.name} just boosted the server! {self.guild} has achieved **Level 1!**'
+            else:
+                return f'{self.author.name} just boosted the server **{self.content}** times! {self.guild} has achieved **Level 1!**'
+
+        if self.type is MessageType.premium_guild_tier_2:
+            if not self.content:
+                return f'{self.author.name} just boosted the server! {self.guild} has achieved **Level 2!**'
+            else:
+                return f'{self.author.name} just boosted the server **{self.content}** times! {self.guild} has achieved **Level 2!**'
+
+        if self.type is MessageType.premium_guild_tier_3:
+            if not self.content:
+                return f'{self.author.name} just boosted the server! {self.guild} has achieved **Level 3!**'
+            else:
+                return f'{self.author.name} just boosted the server **{self.content}** times! {self.guild} has achieved **Level 3!**'
+
+        if self.type is MessageType.channel_follow_add:
+            return (
+                f'{self.author.name} has added {self.content} to this channel. Its most important updates will show up here.'
+            )
+
+        if self.type is MessageType.guild_discovery_disqualified:
+            return 'This server has been removed from Server Discovery because it no longer passes all the requirements. Check Server Settings for more details.'
+
+        if self.type is MessageType.guild_discovery_requalified:
+            return 'This server is eligible for Server Discovery again and has been automatically relisted!'
+
+        if self.type is MessageType.guild_discovery_grace_period_initial_warning:
+            return 'This server has failed Discovery activity requirements for 1 week. If this server fails for 4 weeks in a row, it will be automatically removed from Discovery.'
+
+        if self.type is MessageType.guild_discovery_grace_period_final_warning:
+            return 'This server has failed Discovery activity requirements for 3 weeks in a row. If this server fails for 1 more week, it will be removed from Discovery.'
+
+        if self.type is MessageType.thread_created:
+            return f'{self.author.name} started a thread: **{self.content}**. See all threads.'
+
+        if self.type is MessageType.thread_starter_message:
+            if self.reference is None or self.reference.resolved is None:
+                return 'Sorry, we couldn\'t load the first message in this thread'
+
+            # The resolved message for the reference will be a Message
+            return self.reference.resolved.content  # type: ignore
+
+        if self.type is MessageType.guild_invite_reminder:
+            return 'Wondering who to invite?\nStart by inviting anyone who can help you build the server!'
+
+        if self.type is MessageType.role_subscription_purchase and self.role_subscription is not None:
+            total_months = self.role_subscription.total_months_subscribed
+            months = '1 month' if total_months == 1 else f'{total_months} months'
+            action = 'renewed' if self.role_subscription.is_renewal else 'subscribed'
+            return f'{self.author.name} {action} **{self.role_subscription.tier_name}** and has been a subscriber of {self.guild} for {months}!'
+
+        if self.type is MessageType.stage_start:
+            return f'{self.author.name} started **{self.content}**'
+
+        if self.type is MessageType.stage_end:
+            return f'{self.author.name} ended **{self.content}**'
+
+        if self.type is MessageType.stage_speaker:
+            return f'{self.author.name} is now a speaker.'
+
+        if self.type is MessageType.stage_raise_hand:
+            return f'{self.author.name} requested to speak.'
+
+        if self.type is MessageType.stage_topic:
+            return f'{self.author.name} changed the Stage topic: **{self.content}**'
+
+        if self.type is MessageType.guild_application_premium_subscription:
+            return f'{self.author.name} upgraded {self.application.name if self.application else "a deleted application"} to premium for this server!'
+
+        # Fallback for unknown message types
+        return self.content
+
+    @overload
+    async def edit(
+        self,
+        *,
+        content: Optional[str] = ...,
+        attachments: Sequence[Union[Attachment, File]] = ...,
+        suppress: bool = ...,
+        delete_after: Optional[float] = ...,
+        allowed_mentions: Optional[AllowedMentions] = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def edit(
+        self,
+        *,
+        content: Optional[str] = ...,
+        attachments: Sequence[Union[Attachment, File]] = ...,
+        suppress: bool = ...,
+        delete_after: Optional[float] = ...,
+        allowed_mentions: Optional[AllowedMentions] = ...,
+    ) -> Message:
+        ...
+
+    async def edit(
+        self,
+        content: Optional[str] = MISSING,
+        attachments: Sequence[Union[Attachment, File]] = MISSING,
+        suppress: bool = False,
+        delete_after: Optional[float] = None,
+        allowed_mentions: Optional[AllowedMentions] = MISSING,
+    ) -> Message:
+        """|coro|
+
+        Edits the message.
+
+        The content must be able to be transformed into a string via ``str(content)``.
+
+        .. versionchanged:: 1.3
+            The ``suppress`` keyword-only parameter was added.
+
+        .. versionchanged:: 2.0
+            Edits are no longer in-place, the newly edited message is returned instead.
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`TypeError` instead of
+            ``InvalidArgument``.
+
+        Parameters
+        -----------
+        content: Optional[:class:`str`]
+            The new content to replace the message with.
+            Could be ``None`` to remove the content.
+        attachments: List[Union[:class:`Attachment`, :class:`File`]]
+            A list of attachments to keep in the message as well as new files to upload. If ``[]`` is passed
+            then all attachments are removed.
+
+            .. note::
+
+                New files will always appear after current attachments.
+
+            .. versionadded:: 2.0
+        suppress: :class:`bool`
+            Whether to suppress embeds for the message. This removes
+            all the embeds if set to ``True``. If set to ``False``
+            this brings the embeds back if they were suppressed.
+            Using this parameter requires :attr:`~.Permissions.manage_messages`.
+        delete_after: Optional[:class:`float`]
+            If provided, the number of seconds to wait in the background
+            before deleting the message we just edited. If the deletion fails,
+            then it is silently ignored.
+        allowed_mentions: Optional[:class:`~discord.AllowedMentions`]
+            Controls the mentions being processed in this message. If this is
+            passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
+            The merging behaviour only overrides attributes that have been explicitly passed
+            to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
+            If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
+            are used instead.
+
+            .. versionadded:: 1.4
+
+        Raises
+        -------
+        HTTPException
+            Editing the message failed.
+        Forbidden
+            Tried to suppress a message without permissions or
+            edit a message that isn't yours.
+
+        Returns
+        --------
+        :class:`Message`
+            The newly edited message.
+        """
+
+        if content is not MISSING:
+            previous_allowed_mentions = self._state.allowed_mentions
+        else:
+            previous_allowed_mentions = None
+
+        if suppress is not MISSING:
+            flags = MessageFlags._from_value(self.flags.value)
+            flags.suppress_embeds = suppress
+        else:
+            flags = MISSING
+
+        with handle_message_parameters(
+            content=content,
+            flags=flags,
+            attachments=attachments,
+            allowed_mentions=allowed_mentions,
+            previous_allowed_mentions=previous_allowed_mentions,
+        ) as params:
+            data = await self._state.http.edit_message(self.channel.id, self.id, params=params)
+            message = Message(state=self._state, channel=self.channel, data=data)
+
+        if delete_after is not None:
+            await self.delete(delay=delete_after)
+
+        return message
+
+    async def add_files(self, *files: File) -> Message:
+        r"""|coro|
+
+        Adds new files to the end of the message attachments.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        -----------
+        \*files: :class:`File`
+            New files to add to the message.
+
+        Raises
+        -------
+        HTTPException
+            Editing the message failed.
+        Forbidden
+            Tried to edit a message that isn't yours.
+
+        Returns
+        --------
+        :class:`Message`
+            The newly edited message.
+        """
+        return await self.edit(attachments=[*self.attachments, *files])
+
+    async def remove_attachments(self, *attachments: Attachment) -> Message:
+        r"""|coro|
+
+        Removes attachments from the message.
+
+        .. versionadded:: 2.0
+
+        Parameters
+        -----------
+        \*attachments: :class:`Attachment`
+            Attachments to remove from the message.
+
+        Raises
+        -------
+        HTTPException
+            Editing the message failed.
+        Forbidden
+            Tried to edit a message that isn't yours.
+
+        Returns
+        --------
+        :class:`Message`
+            The newly edited message.
+        """
+        return await self.edit(attachments=[a for a in self.attachments if a not in attachments])
+
+    def message_commands(
+        self,
+        query: Optional[str] = None,
+        *,
+        limit: Optional[int] = None,
+        command_ids: Optional[Collection[int]] = None,
+        application: Optional[Snowflake] = None,
+        with_applications: bool = True,
+    ) -> AsyncIterator[MessageCommand]:
+        """Returns a :term:`asynchronous iterator` of the message commands available to use on the message.
+
+        Examples
+        ---------
+
+        Usage ::
+
+            async for command in message.message_commands():
+                print(command.name)
+
+        Flattening into a list ::
+
+            commands = [command async for command in message.message_commands()]
+            # commands is now a list of MessageCommand...
+
+        All parameters are optional.
+
+        Parameters
+        ----------
+        query: Optional[:class:`str`]
+            The query to search for. Specifying this limits results to 25 commands max.
+
+            This parameter is faked if ``application`` is specified.
+        limit: Optional[:class:`int`]
+            The maximum number of commands to send back. Defaults to 0 if ``command_ids`` is passed, else 25.
+            If ``None``, returns all commands.
+
+            This parameter is faked if ``application`` is specified.
+        command_ids: Optional[List[:class:`int`]]
+            List of up to 100 command IDs to search for. If the command doesn't exist, it won't be returned.
+
+            If ``limit`` is passed alongside this parameter, this parameter will serve as a "preferred commands" list.
+            This means that the endpoint will return the found commands + up to ``limit`` more, if available.
+        application: Optional[:class:`~discord.abc.Snowflake`]
+            Whether to return this application's commands. Always set to DM recipient in a private channel context.
+        with_applications: :class:`bool`
+            Whether to include applications in the response. Defaults to ``True``.
+
+        Raises
+        ------
+        TypeError
+            Both query and command_ids are passed.
+            Attempted to fetch commands in a DM with a non-bot user.
+        ValueError
+            The limit was not greater than or equal to 0.
+        HTTPException
+            Getting the commands failed.
+        ~discord.Forbidden
+            You do not have permissions to get the commands.
+        ~discord.HTTPException
+            The request to get the commands failed.
+
+        Yields
+        -------
+        :class:`.MessageCommand`
+            A message command.
+        """
+        return _handle_commands(
+            self,
+            AppCommandType.message,
+            query=query,
+            limit=limit,
+            command_ids=command_ids,
+            application=application,
+            with_applications=with_applications,
+            target=self,
+        )
```

### Comparing `discord.py-self-1.9.2/discord/mixins.py` & `discord.py-self-2.0.0/discord/types/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-class EqualityComparable:
-    __slots__ = ()
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and other.id == self.id
-
-    def __ne__(self, other):
-        if isinstance(other, self.__class__):
-            return other.id != self.id
-        return True
-
-class Hashable(EqualityComparable):
-    __slots__ = ()
-
-    def __hash__(self):
-        return self.id >> 22
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import Optional, TypedDict
+from .snowflake import Snowflake
+from .user import User
+from .guild import Guild
+
+
+class CreateTemplate(TypedDict):
+    name: str
+    icon: Optional[bytes]
+
+
+class Template(TypedDict):
+    code: str
+    name: str
+    description: Optional[str]
+    usage_count: int
+    creator_id: Snowflake
+    creator: User
+    created_at: str
+    updated_at: str
+    source_guild_id: Snowflake
+    serialized_source_guild: Guild
+    is_dirty: Optional[bool]
```

### Comparing `discord.py-self-1.9.2/discord/oggparse.py` & `discord.py-self-2.0.0/discord/oggparse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,117 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-import struct
-
-from .errors import DiscordException
-
-class OggError(DiscordException):
-    """An exception that is thrown for Ogg stream parsing errors."""
-    pass
-
-# https://tools.ietf.org/html/rfc3533
-# https://tools.ietf.org/html/rfc7845
-
-class OggPage:
-    _header = struct.Struct('<xBQIIIB')
-
-    def __init__(self, stream):
-        try:
-            header = stream.read(struct.calcsize(self._header.format))
-
-            self.flag, self.gran_pos, self.serial, \
-            self.pagenum, self.crc, self.segnum = self._header.unpack(header)
-
-            self.segtable = stream.read(self.segnum)
-            bodylen = sum(struct.unpack('B'*self.segnum, self.segtable))
-            self.data = stream.read(bodylen)
-        except Exception:
-            raise OggError('bad data stream') from None
-
-    def iter_packets(self):
-        packetlen = offset = 0
-        partial = True
-
-        for seg in self.segtable:
-            if seg == 255:
-                packetlen += 255
-                partial = True
-            else:
-                packetlen += seg
-                yield self.data[offset:offset+packetlen], True
-                offset += packetlen
-                packetlen = 0
-                partial = False
-
-        if partial:
-            yield self.data[offset:], False
-
-class OggStream:
-    def __init__(self, stream):
-        self.stream = stream
-
-    def _next_page(self):
-        head = self.stream.read(4)
-        if head == b'OggS':
-            return OggPage(self.stream)
-        elif not head:
-            return None
-        else:
-            raise OggError('invalid header magic')
-
-    def _iter_pages(self):
-        page = self._next_page()
-        while page:
-            yield page
-            page = self._next_page()
-
-    def iter_packets(self):
-        partial = b''
-        for page in self._iter_pages():
-            for data, complete in page.iter_packets():
-                partial += data
-                if complete:
-                    yield partial
-                    partial = b''
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import struct
+
+from typing import TYPE_CHECKING, ClassVar, IO, Generator, Tuple, Optional
+
+from .errors import DiscordException
+
+__all__ = (
+    'OggError',
+    'OggPage',
+    'OggStream',
+)
+
+
+class OggError(DiscordException):
+    """An exception that is thrown for Ogg stream parsing errors."""
+
+    pass
+
+
+# https://tools.ietf.org/html/rfc3533
+# https://tools.ietf.org/html/rfc7845
+
+
+class OggPage:
+    _header: ClassVar[struct.Struct] = struct.Struct('<xBQIIIB')
+    if TYPE_CHECKING:
+        flag: int
+        gran_pos: int
+        serial: int
+        pagenum: int
+        crc: int
+        segnum: int
+
+    def __init__(self, stream: IO[bytes]) -> None:
+        try:
+            header = stream.read(struct.calcsize(self._header.format))
+
+            self.flag, self.gran_pos, self.serial, self.pagenum, self.crc, self.segnum = self._header.unpack(header)
+
+            self.segtable: bytes = stream.read(self.segnum)
+            bodylen = sum(struct.unpack('B' * self.segnum, self.segtable))
+            self.data: bytes = stream.read(bodylen)
+        except Exception:
+            raise OggError('bad data stream') from None
+
+    def iter_packets(self) -> Generator[Tuple[bytes, bool], None, None]:
+        packetlen = offset = 0
+        partial = True
+
+        for seg in self.segtable:
+            if seg == 255:
+                packetlen += 255
+                partial = True
+            else:
+                packetlen += seg
+                yield self.data[offset : offset + packetlen], True
+                offset += packetlen
+                packetlen = 0
+                partial = False
+
+        if partial:
+            yield self.data[offset:], False
+
+
+class OggStream:
+    def __init__(self, stream: IO[bytes]) -> None:
+        self.stream: IO[bytes] = stream
+
+    def _next_page(self) -> Optional[OggPage]:
+        head = self.stream.read(4)
+        if head == b'OggS':
+            return OggPage(self.stream)
+        elif not head:
+            return None
+        else:
+            raise OggError('invalid header magic')
+
+    def _iter_pages(self) -> Generator[OggPage, None, None]:
+        page = self._next_page()
+        while page:
+            yield page
+            page = self._next_page()
+
+    def iter_packets(self) -> Generator[bytes, None, None]:
+        partial = b''
+        for page in self._iter_pages():
+            for data, complete in page.iter_packets():
+                partial += data
+                if complete:
+                    yield partial
+                    partial = b''
```

### Comparing `discord.py-self-1.9.2/discord/reaction.py` & `discord.py-self-2.0.0/discord/reaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,254 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .iterators import ReactionIterator
-
-class Reaction:
-    """Represents a reaction to a message.
-
-    Depending on the way this object was created, some of the attributes can
-    have a value of ``None``.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two reactions are equal. This works by checking if the emoji
-            is the same. So two messages with the same reaction will be considered
-            "equal".
-
-        .. describe:: x != y
-
-            Checks if two reactions are not equal.
-
-        .. describe:: hash(x)
-
-            Returns the reaction's hash.
-
-        .. describe:: str(x)
-
-            Returns the string form of the reaction's emoji.
-
-    Attributes
-    -----------
-    emoji: Union[:class:`Emoji`, :class:`PartialEmoji`, :class:`str`]
-        The reaction emoji. May be a custom emoji, or a unicode emoji.
-    count: :class:`int`
-        Number of times this reaction was made
-    me: :class:`bool`
-        If the user sent this reaction.
-    message: :class:`Message`
-        Message this reaction is for.
-    """
-    __slots__ = ('message', 'count', 'emoji', 'me')
-
-    def __init__(self, *, message, data, emoji=None):
-        self.message = message
-        self.emoji = emoji or message._state.get_reaction_emoji(data['emoji'])
-        self.count = data.get('count', 1)
-        self.me = data.get('me')
-
-    @property
-    def custom_emoji(self):
-        """:class:`bool`: If this is a custom emoji."""
-        return not isinstance(self.emoji, str)
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and other.emoji == self.emoji
-
-    def __ne__(self, other):
-        if isinstance(other, self.__class__):
-            return other.emoji != self.emoji
-        return True
-
-    def __hash__(self):
-        return hash(self.emoji)
-
-    def __str__(self):
-        return str(self.emoji)
-
-    def __repr__(self):
-        return '<Reaction emoji={0.emoji!r} me={0.me} count={0.count}>'.format(self)
-
-    async def remove(self, user):
-        """|coro|
-
-        Remove the reaction by the provided :class:`User` from the message.
-
-        If the reaction is not your own (i.e. ``user`` parameter is not you) then
-        the :attr:`~Permissions.manage_messages` permission is needed.
-
-        The ``user`` parameter must represent a user or member and meet
-        the :class:`abc.Snowflake` abc.
-
-        Parameters
-        -----------
-        user: :class:`abc.Snowflake`
-             The user or member from which to remove the reaction.
-
-        Raises
-        -------
-        HTTPException
-            Removing the reaction failed.
-        Forbidden
-            You do not have the proper permissions to remove the reaction.
-        NotFound
-            The user you specified, or the reaction's message was not found.
-        """
-
-        await self.message.remove_reaction(self.emoji, user)
-
-    async def clear(self):
-        """|coro|
-
-        Clears this reaction from the message.
-
-        You need the :attr:`~Permissions.manage_messages` permission to use this.
-
-        .. versionadded:: 1.3
-
-        Raises
-        --------
-        HTTPException
-            Clearing the reaction failed.
-        Forbidden
-            You do not have the proper permissions to clear the reaction.
-        NotFound
-            The emoji you specified was not found.
-        InvalidArgument
-            The emoji parameter is invalid.
-        """
-        await self.message.clear_reaction(self.emoji)
-
-    def users(self, limit=None, after=None):
-        """Returns an :class:`AsyncIterator` representing the users that have reacted to the message.
-
-        The ``after`` parameter must represent a member
-        and meet the :class:`abc.Snowflake` abc.
-
-        Examples
-        ---------
-
-        Usage ::
-
-            # I do not actually recommend doing this.
-            async for user in reaction.users():
-                await channel.send('{0} has reacted with {1.emoji}!'.format(user, reaction))
-
-        Flattening into a list: ::
-
-            users = await reaction.users().flatten()
-            # users is now a list of User...
-            winner = random.choice(users)
-            await channel.send('{} has won the raffle.'.format(winner))
-
-        Parameters
-        ------------
-        limit: :class:`int`
-            The maximum number of results to return.
-            If not provided, returns all the users who
-            reacted to the message.
-        after: :class:`abc.Snowflake`
-            For pagination, reactions are sorted by member.
-
-        Raises
-        --------
-        HTTPException
-            Getting the users for the reaction failed.
-
-        Yields
-        --------
-        Union[:class:`User`, :class:`Member`]
-            The member (if retrievable) or the user that has reacted
-            to this message. The case where it can be a :class:`Member` is
-            in a guild message context. Sometimes it can be a :class:`User`
-            if the member has left the guild.
-        """
-
-        if self.custom_emoji:
-            emoji = '{0.name}:{0.id}'.format(self.emoji)
-        else:
-            emoji = self.emoji
-
-        if limit is None:
-            limit = self.count
-
-        return ReactionIterator(self.message, emoji, limit, after)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+from typing import TYPE_CHECKING, AsyncIterator, Union, Optional
+
+from .user import User
+from .object import Object
+
+# fmt: off
+__all__ = (
+    'Reaction',
+)
+# fmt: on
+
+if TYPE_CHECKING:
+    from .member import Member
+    from .types.message import Reaction as ReactionPayload
+    from .message import Message
+    from .partial_emoji import PartialEmoji
+    from .emoji import Emoji
+    from .abc import Snowflake
+
+
+class Reaction:
+    """Represents a reaction to a message.
+
+    Depending on the way this object was created, some of the attributes can
+    have a value of ``None``.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two reactions are equal. This works by checking if the emoji
+            is the same. So two messages with the same reaction will be considered
+            "equal".
+
+        .. describe:: x != y
+
+            Checks if two reactions are not equal.
+
+        .. describe:: hash(x)
+
+            Returns the reaction's hash.
+
+        .. describe:: str(x)
+
+            Returns the string form of the reaction's emoji.
+
+    Attributes
+    -----------
+    emoji: Union[:class:`Emoji`, :class:`PartialEmoji`, :class:`str`]
+        The reaction emoji. May be a custom emoji, or a unicode emoji.
+    count: :class:`int`
+        Number of times this reaction was made
+    me: :class:`bool`
+        If the user sent this reaction.
+    message: :class:`Message`
+        Message this reaction is for.
+    """
+
+    __slots__ = ('message', 'count', 'emoji', 'me')
+
+    def __init__(self, *, message: Message, data: ReactionPayload, emoji: Optional[Union[PartialEmoji, Emoji, str]] = None):
+        self.message: Message = message
+        self.emoji: Union[PartialEmoji, Emoji, str] = emoji or message._state.get_reaction_emoji(data['emoji'])
+        self.count: int = data.get('count', 1)
+        self.me: bool = data['me']
+
+    # TODO: typeguard
+    def is_custom_emoji(self) -> bool:
+        """:class:`bool`: If this is a custom emoji."""
+        return not isinstance(self.emoji, str)
+
+    def __eq__(self, other: object) -> bool:
+        return isinstance(other, self.__class__) and other.emoji == self.emoji
+
+    def __ne__(self, other: object) -> bool:
+        if isinstance(other, self.__class__):
+            return other.emoji != self.emoji
+        return True
+
+    def __hash__(self) -> int:
+        return hash(self.emoji)
+
+    def __str__(self) -> str:
+        return str(self.emoji)
+
+    def __repr__(self) -> str:
+        return f'<Reaction emoji={self.emoji!r} me={self.me} count={self.count}>'
+
+    async def remove(self, user: Snowflake) -> None:
+        """|coro|
+
+        Remove the reaction by the provided :class:`User` from the message.
+
+        If the reaction is not your own (i.e. ``user`` parameter is not you) then
+        :attr:`~Permissions.manage_messages` is needed.
+
+        The ``user`` parameter must represent a user or member and meet
+        the :class:`abc.Snowflake` abc.
+
+        Parameters
+        -----------
+        user: :class:`abc.Snowflake`
+             The user or member from which to remove the reaction.
+
+        Raises
+        -------
+        HTTPException
+            Removing the reaction failed.
+        Forbidden
+            You do not have the proper permissions to remove the reaction.
+        NotFound
+            The user you specified, or the reaction's message was not found.
+        """
+
+        await self.message.remove_reaction(self.emoji, user)
+
+    async def clear(self) -> None:
+        """|coro|
+
+        Clears this reaction from the message.
+
+        You must have :attr:`~Permissions.manage_messages` to do this.
+
+        .. versionadded:: 1.3
+
+        .. versionchanged:: 2.0
+            This function will now raise :exc:`ValueError` instead of
+            ``InvalidArgument``.
+
+        Raises
+        --------
+        HTTPException
+            Clearing the reaction failed.
+        Forbidden
+            You do not have the proper permissions to clear the reaction.
+        NotFound
+            The emoji you specified was not found.
+        TypeError
+            The emoji parameter is invalid.
+        """
+        await self.message.clear_reaction(self.emoji)
+
+    async def users(
+        self, *, limit: Optional[int] = None, after: Optional[Snowflake] = None
+    ) -> AsyncIterator[Union[Member, User]]:
+        """Returns an :term:`asynchronous iterator` representing the users that have reacted to the message.
+
+        The ``after`` parameter must represent a member
+        and meet the :class:`abc.Snowflake` abc.
+
+        .. versionchanged:: 2.0
+
+            ``limit`` and ``after`` parameters are now keyword-only.
+
+        Examples
+        ---------
+
+        Usage ::
+
+            # I do not actually recommend doing this
+            async for user in reaction.users():
+                await channel.send(f'{user} has reacted with {reaction.emoji}!')
+
+        Flattening into a list: ::
+
+            users = [user async for user in reaction.users()]
+            # users is now a list of User...
+            winner = random.choice(users)
+            await channel.send(f'{winner} has won the raffle.')
+
+        Parameters
+        ------------
+        limit: Optional[:class:`int`]
+            The maximum number of results to return.
+            If not provided, returns all the users who
+            reacted to the message.
+        after: Optional[:class:`abc.Snowflake`]
+            For pagination, reactions are sorted by member.
+
+        Raises
+        --------
+        HTTPException
+            Getting the users for the reaction failed.
+
+        Yields
+        --------
+        Union[:class:`User`, :class:`Member`]
+            The member (if retrievable) or the user that has reacted
+            to this message. The case where it can be a :class:`Member` is
+            in a guild message context. Sometimes it can be a :class:`User`
+            if the member has left the guild.
+        """
+
+        if not isinstance(self.emoji, str):
+            emoji = f'{self.emoji.name}:{self.emoji.id}'
+        else:
+            emoji = self.emoji
+
+        if limit is None:
+            limit = self.count
+
+        while limit > 0:
+            retrieve = min(limit, 100)
+
+            message = self.message
+            guild = message.guild
+            state = message._state
+            after_id = after.id if after else None
+
+            data = await state.http.get_reaction_users(message.channel.id, message.id, emoji, retrieve, after=after_id)
+
+            if data:
+                limit -= len(data)
+                after = Object(id=int(data[-1]['id']))
+            else:
+                # Terminate loop if we received no data
+                limit = 0
+
+            if guild is None or isinstance(guild, Object):
+                for raw_user in reversed(data):
+                    yield User(state=state, data=raw_user)
+
+                continue
+
+            for raw_user in reversed(data):
+                member_id = int(raw_user['id'])
+                member = guild.get_member(member_id)
+
+                yield member or User(state=state, data=raw_user)
```

### Comparing `discord.py-self-1.9.2/discord/sticker.py` & `discord.py-self-2.0.0/discord/modal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,138 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .mixins import Hashable
-from .asset import Asset
-from .utils import snowflake_time
-from .enums import StickerType, try_enum
-
-class Sticker(Hashable):
-    """Represents a sticker.
-
-    .. versionadded:: 1.6
-
-    .. container:: operations
-
-        .. describe:: str(x)
-
-            Returns the name of the sticker.
-
-        .. describe:: x == y
-
-           Checks if the sticker is equal to another sticker.
-
-        .. describe:: x != y
-
-           Checks if the sticker is not equal to another sticker.
-
-    Attributes
-    ----------
-    name: :class:`str`
-        The sticker's name.
-    id: :class:`int`
-        The id of the sticker.
-    description: :class:`str`
-        The description of the sticker.
-    pack_id: :class:`int`
-        The id of the sticker's pack.
-    format: :class:`StickerType`
-        The format for the sticker's image.
-    image: :class:`str`
-        The sticker's image.
-    tags: List[:class:`str`]
-        A list of tags for the sticker.
-    preview_image: Optional[:class:`str`]
-        The sticker's preview asset hash.
-    """
-    __slots__ = ('_state', 'id', 'name', 'description', 'pack_id', 'format', 'image', 'tags', 'preview_image')
-
-    def __init__(self, *, state, data):
-        self._state = state
-        self.id = int(data['id'])
-        self.name = data['name']
-        self.description = data['description']
-        self.pack_id = int(data.get('pack_id', 0))
-        self.format = try_enum(StickerType, data['format_type'])
-        self.image = data['asset']
-
-        try:
-            self.tags = [tag.strip() for tag in data['tags'].split(',')]
-        except KeyError:
-            self.tags = []
-
-        self.preview_image = data.get('preview_asset')
-
-    def __repr__(self):
-        return '<{0.__class__.__name__} id={0.id} name={0.name!r}>'.format(self)
-
-    def __str__(self):
-        return self.name
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the sticker's creation time in UTC as a naive datetime."""
-        return snowflake_time(self.id)
-
-    @property
-    def image_url(self):
-        """Returns an :class:`Asset` for the sticker's image.
-
-        .. note::
-            This will return ``None`` if the format is ``StickerType.lottie``.
-
-        Returns
-        -------
-        Optional[:class:`Asset`]
-            The resulting CDN asset.
-        """
-        return self.image_url_as()
-
-    def image_url_as(self, *, size=1024):
-        """Optionally returns an :class:`Asset` for the sticker's image.
-
-        The size must be a power of 2 between 16 and 4096.
-
-        .. note::
-            This will return ``None`` if the format is ``StickerType.lottie``.
-
-        Parameters
-        -----------
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Invalid ``size``.
-
-        Returns
-        -------
-        Optional[:class:`Asset`]
-            The resulting CDN asset or ``None``.
-        """
-        if self.format is StickerType.lottie:
-            return None
-
-        return Asset._from_sticker_url(self._state, self, size=size)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2021-present Dolfies
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List, Optional, Union
+
+from .components import _component_factory
+from .enums import InteractionType
+from .interactions import _wrapped_interaction
+from .mixins import Hashable
+from .utils import _generate_nonce
+
+if TYPE_CHECKING:
+    from .application import IntegrationApplication
+    from .components import ActionRow
+    from .interactions import Interaction
+
+# fmt: off
+__all__ = (
+    'Modal',
+)
+# fmt: on
+
+
+class Modal(Hashable):
+    """Represents a modal from the Discord Bot UI Kit.
+
+    .. versionadded:: 2.0
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two modals are equal.
+
+        .. describe:: x != y
+
+            Checks if two modals are not equal.
+
+        .. describe:: hash(x)
+
+            Return the modal's hash.
+
+        .. describe:: str(x)
+
+            Returns the modal's title.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The modal's ID. This is the same as the interaction ID.
+    nonce: Optional[Union[:class:`int`, :class:`str`]]
+        The modal's nonce. May not be present.
+    title: :class:`str`
+        The modal's title.
+    custom_id: :class:`str`
+        The ID of the modal that gets received during an interaction.
+    components: List[:class:`Component`]
+        A list of components in the modal.
+    application: :class:`IntegrationApplication`
+        The application that sent the modal.
+    """
+
+    __slots__ = ('_state', 'interaction', 'id', 'nonce', 'title', 'custom_id', 'components', 'application')
+
+    def __init__(self, *, data: dict, interaction: Interaction):
+        self._state = interaction._state
+        self.interaction = interaction
+        self.id = int(data['id'])
+        self.nonce: Optional[Union[int, str]] = data.get('nonce')
+        self.title: str = data.get('title', '')
+        self.custom_id: str = data.get('custom_id', '')
+        self.components: List[ActionRow] = [_component_factory(d) for d in data.get('components', [])]  # type: ignore # Will always be rows here
+        self.application: IntegrationApplication = interaction._state.create_integration_application(data['application'])
+
+    def __str__(self) -> str:
+        return self.title
+
+    def to_dict(self) -> dict:
+        return {
+            'id': str(self.id),
+            'custom_id': self.custom_id,
+            'components': [c.to_dict() for c in self.components],
+        }
+
+    async def submit(self):
+        """|coro|
+
+        Submits the modal.
+
+        All required components must be already answered.
+
+        Raises
+        -------
+        InvalidData
+            Didn't receive a response from Discord
+            (doesn't mean the interaction failed).
+        NotFound
+            The originating message was not found.
+        HTTPException
+            Choosing the options failed.
+
+        Returns
+        --------
+        :class:`Interaction`
+            The interaction that was created.
+        """
+        interaction = self.interaction
+        return await _wrapped_interaction(
+            self._state,
+            _generate_nonce(),
+            InteractionType.modal_submit,
+            None,
+            interaction.channel,
+            self.to_dict(),
+            application_id=self.application.id,
+        )
```

### Comparing `discord.py-self-1.9.2/discord/team.py` & `discord.py-self-2.0.0/discord/metadata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,160 +1,134 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from . import utils
-from .user import BaseUser
-from .asset import Asset
-from .enums import TeamMembershipState, try_enum
-
-__all__ = (
-    'Team',
-    'TeamMember',
-)
-
-class Team:
-    """Represents an application team for a bot provided by Discord.
-
-    Attributes
-    -------------
-    id: :class:`int`
-        The team ID.
-    name: :class:`str`
-        The team name
-    icon: Optional[:class:`str`]
-        The icon hash, if it exists.
-    owner_id: :class:`int`
-        The team's owner ID.
-    members: List[:class:`TeamMember`]
-        A list of the members in the team
-
-        .. versionadded:: 1.3
-    """
-    __slots__ = ('_state', 'id', 'name', 'icon', 'owner_id', 'members')
-
-    def __init__(self, state, data):
-        self._state = state
-
-        self.id = utils._get_as_snowflake(data, 'id')
-        self.name = data['name']
-        self.icon = data['icon']
-        self.owner_id = utils._get_as_snowflake(data, 'owner_user_id')
-        self.members = [TeamMember(self, self._state, member) for member in data['members']]
-
-    def __repr__(self):
-        return '<{0.__class__.__name__} id={0.id} name={0.name}>'.format(self)
-
-    @property
-    def icon_url(self):
-        """:class:`.Asset`: Retrieves the team's icon asset.
-
-        This is equivalent to calling :meth:`icon_url_as` with
-        the default parameters ('webp' format and a size of 1024).
-        """
-        return self.icon_url_as()
-
-    def icon_url_as(self, *, format='webp', size=1024):
-        """Returns an :class:`Asset` for the icon the team has.
-
-        The format must be one of 'webp', 'jpeg', 'jpg' or 'png'.
-        The size must be a power of 2 between 16 and 4096.
-
-        .. versionadded:: 2.0
-
-        Parameters
-        -----------
-        format: :class:`str`
-            The format to attempt to convert the icon to. Defaults to 'webp'.
-        size: :class:`int`
-            The size of the image to display.
-
-        Raises
-        ------
-        InvalidArgument
-            Bad image format passed to ``format`` or invalid ``size``.
-
-        Returns
-        --------
-        :class:`Asset`
-            The resulting CDN asset.
-        """
-        return Asset._from_icon(self._state, self, 'team', format=format, size=size)
-
-    @property
-    def owner(self):
-        """Optional[:class:`TeamMember`]: The team's owner."""
-        return utils.get(self.members, id=self.owner_id)
-
-class TeamMember(BaseUser):
-    """Represents a team member in a team.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two team members are equal.
-
-        .. describe:: x != y
-
-            Checks if two team members are not equal.
-
-        .. describe:: hash(x)
-
-            Return the team member's hash.
-
-        .. describe:: str(x)
-
-            Returns the team member's name with discriminator.
-
-    .. versionadded:: 1.3
-
-    Attributes
-    -------------
-    name: :class:`str`
-        The team member's username.
-    id: :class:`int`
-        The team member's unique ID.
-    discriminator: :class:`str`
-        The team member's discriminator. This is given when the username has conflicts.
-    avatar: Optional[:class:`str`]
-        The avatar hash the team member has. Could be None.
-    bot: :class:`bool`
-        Specifies if the user is a bot account.
-    team: :class:`Team`
-        The team that the member is from.
-    membership_state: :class:`TeamMembershipState`
-        The membership state of the member (e.g. invited or accepted)
-    """
-    __slots__ = BaseUser.__slots__ + ('team', 'membership_state', 'permissions')
-
-    def __init__(self, team, state, data):
-        self.team = team
-        self.membership_state = try_enum(TeamMembershipState, data['membership_state'])
-        self.permissions = data['permissions']
-        super().__init__(state=state, data=data['user'])
-
-    def __repr__(self):
-        return '<{0.__class__.__name__} id={0.id} name={0.name!r} ' \
-               'discriminator={0.discriminator!r} membership_state={0.membership_state!r}>'.format(self)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2021-present Dolfies
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Dict, Iterator, Optional, Tuple, Union
+
+from .utils import parse_time
+
+
+class Metadata:
+    """Represents a raw model from Discord.
+
+    Because of how unstable and wildly varying some metadata in Discord can be, this is a simple class
+    that just provides access to the raw data using dot notation. This means that ``None`` is returned
+    for unknown attributes instead of raising an exception. This class can be used similarly to a dictionary.
+
+    .. versionadded:: 2.0
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two metadata objects are equal.
+
+        .. describe:: x != y
+
+            Checks if two metadata objects are not equal.
+
+        .. describe:: x[key]
+
+            Returns a metadata value if it is found, otherwise raises a :exc:`KeyError`.
+
+        .. describe:: key in x
+
+            Checks if a metadata value is present.
+
+        .. describe:: len(x)
+
+            Returns the number of metadata values present.
+
+        .. describe:: iter(x)
+            Returns an iterator of ``(field, value)`` pairs. This allows this class
+            to be used as an iterable in list/dict/etc constructions.
+    """
+
+    def __init__(self, data: Optional[MetadataObject] = None) -> None:
+        if not data:
+            return
+
+        for key, value in data.items():
+            if isinstance(value, dict):
+                value = Metadata(value)
+            elif key.endswith('_id') and isinstance(value, str) and value.isdigit():
+                value = int(value)
+            elif (key.endswith('_at') or key.endswith('_date')) and isinstance(value, str):
+                try:
+                    value = parse_time(value)
+                except ValueError:
+                    pass
+            elif isinstance(value, list):
+                value = [Metadata(x) if isinstance(x, dict) else x for x in value]
+
+            self.__dict__[key] = value
+
+    def __repr__(self) -> str:
+        if not self.__dict__:
+            return '<Metadata>'
+        return f'<Metadata {" ".join(f"{k}={v!r}" for k, v in self.__dict__.items())}>'
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Metadata):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: object) -> bool:
+        if not isinstance(other, Metadata):
+            return True
+        return self.__dict__ != other.__dict__
+
+    def __iter__(self) -> Iterator[Tuple[str, Any]]:
+        yield from self.__dict__.items()
+
+    def __getitem__(self, key: str) -> Any:
+        return self.__dict__[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.__dict__[key] = value
+
+    def __getattr__(self, _) -> Any:
+        return None
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.__dict__
+
+    def __len__(self) -> int:
+        return len(self.__dict__)
+
+    def keys(self):
+        """A set-like object providing a view on the metadata's keys."""
+        return self.__dict__.keys()
+
+    def values(self):
+        """A set-like object providing a view on the metadata's values."""
+        return self.__dict__.values()
+
+    def items(self):
+        """A set-like object providing a view on the metadata's items."""
+        return self.__dict__.items()
+
+
+if TYPE_CHECKING:
+    MetadataObject = Union[Metadata, Dict[str, Any]]
```

### Comparing `discord.py-self-1.9.2/discord/template.py` & `discord.py-self-2.0.0/discord/stage_instance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,231 +1,196 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .utils import parse_time, _get_as_snowflake, _bytes_to_base64_data
-from .guild import Guild
-
-__all__ = (
-    'Template',
-)
-
-class _FriendlyHttpAttributeErrorHelper:
-    __slots__ = ()
-
-    def __getattr__(self, attr):
-        raise AttributeError('PartialTemplateState does not support http methods.')
-
-class _PartialTemplateState:
-    def __init__(self, *, state):
-        self.__state = state
-        self.http = _FriendlyHttpAttributeErrorHelper()
-
-    @property
-    def user(self):
-        return self.__state.user
-
-    @property
-    def self_id(self):
-        return self.__state.user.id
-
-    @property
-    def member_cache_flags(self):
-        return self.__state.member_cache_flags
-
-    def store_emoji(self, guild, packet):
-        return None
-
-    def _get_voice_client(self, id):
-        return None
-
-    def _get_message(self, id):
-        return None
-
-    async def query_members(self, **kwargs):
-        return []
-
-    def __getattr__(self, attr):
-        raise AttributeError('PartialTemplateState does not support {0!r}.'.format(attr))
-
-class Template:
-    """Represents a Discord template.
-
-    .. versionadded:: 1.4
-
-    Attributes
-    -----------
-    code: :class:`str`
-        The template code.
-    uses: :class:`int`
-        How many times the template has been used.
-    name: :class:`str`
-        The name of the template.
-    description: :class:`str`
-        The description of the template.
-    creator: :class:`User`
-        The creator of the template.
-    created_at: :class:`datetime.datetime`
-        When the template was created.
-    updated_at: :class:`datetime.datetime`
-        When the template was last updated (referred to as "last synced" in the client).
-    source_guild: :class:`Guild`
-        The source guild.
-    """
-
-    def __init__(self, *, state, data):
-        self._state = state
-        self._store(data)
-
-    def _store(self, data):
-        self.code = data['code']
-        self.uses = data['usage_count']
-        self.name =  data['name']
-        self.description = data['description']
-        creator_data = data.get('creator')
-        self.creator = None if creator_data is None else self._state.store_user(creator_data)
-
-        self.created_at = parse_time(data.get('created_at'))
-        self.updated_at = parse_time(data.get('updated_at'))
-
-        id = _get_as_snowflake(data, 'source_guild_id')
-
-        guild = self._state._get_guild(id)
-
-        if guild is None:
-            source_serialised = data['serialized_source_guild']
-            source_serialised['id'] = id
-            state = _PartialTemplateState(state=self._state)
-            guild = Guild(data=source_serialised, state=state)
-        
-        self.source_guild = guild
-
-    def __repr__(self):
-        return '<Template code={0.code!r} uses={0.uses} name={0.name!r}' \
-               ' creator={0.creator!r} source_guild={0.source_guild!r}>'.format(self)
-
-    async def create_guild(self, name, icon=None):
-        """|coro|
-
-        Creates a :class:`.Guild` using the template.
-
-        Parameters
-        ----------
-        name: :class:`str`
-            The name of the guild.
-        icon: :class:`bytes`
-            The :term:`py:bytes-like object` representing the icon. See :meth:`.ClientUser.edit`
-            for more details on what is expected.
-
-        Raises
-        ------
-        HTTPException
-            Guild creation failed.
-        InvalidArgument
-            Invalid icon image format given. Must be PNG or JPG.
-
-        Returns
-        -------
-        :class:`.Guild`
-            The guild created. This is not the same guild that is
-            added to cache.
-        """
-        if icon is not None:
-            icon = _bytes_to_base64_data(icon)
-
-        data = await self._state.http.create_from_template(self.code, name, icon)
-        return Guild(data=data, state=self._state)
-
-    async def sync(self):
-        """|coro|
-
-        Sync the template to the guild's current state.
-
-        You must have the :attr:`~Permissions.manage_guild` permission in the
-        source guild to do this.
-
-        .. versionadded:: 1.7
-
-        Raises
-        -------
-        HTTPException
-            Editing the template failed.
-        Forbidden
-            You don't have permissions to edit the template.
-        NotFound
-            This template does not exist.
-        """
-
-        data = await self._state.http.sync_template(self.source_guild.id, self.code)
-        self._store(data)
-
-    async def edit(self, **kwargs):
-        """|coro|
-
-        Edit the template metadata.
-
-        You must have the :attr:`~Permissions.manage_guild` permission in the
-        source guild to do this.
-
-        .. versionadded:: 1.7
-
-        Parameters
-        ------------
-        name: Optional[:class:`str`]
-            The template's new name.
-        description: Optional[:class:`str`]
-            The template's description.
-
-        Raises
-        -------
-        HTTPException
-            Editing the template failed.
-        Forbidden
-            You don't have permissions to edit the template.
-        NotFound
-            This template does not exist.
-        """
-        data = await self._state.http.edit_template(self.source_guild.id, self.code, kwargs)
-        self._store(data)
-
-    async def delete(self):
-        """|coro|
-
-        Delete the template.
-
-        You must have the :attr:`~Permissions.manage_guild` permission in the
-        source guild to do this.
-
-        .. versionadded:: 1.7
-
-        Raises
-        -------
-        HTTPException
-            Editing the template failed.
-        Forbidden
-            You don't have permissions to edit the template.
-        NotFound
-            This template does not exist.
-        """
-        await self._state.http.delete_template(self.source_guild.id, self.code)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import Optional, TYPE_CHECKING
+
+from .utils import MISSING, cached_slot_property, _get_as_snowflake
+from .mixins import Hashable
+from .enums import PrivacyLevel, try_enum
+
+# fmt: off
+__all__ = (
+    'StageInstance',
+)
+# fmt: on
+
+if TYPE_CHECKING:
+    from .types.channel import StageInstance as StageInstancePayload
+    from .state import ConnectionState
+    from .channel import StageChannel
+    from .guild import Guild
+    from .scheduled_event import ScheduledEvent
+
+
+class StageInstance(Hashable):
+    """Represents a stage instance of a stage channel in a guild.
+
+    .. versionadded:: 2.0
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two stage instances are equal.
+
+        .. describe:: x != y
+
+            Checks if two stage instances are not equal.
+
+        .. describe:: hash(x)
+
+            Returns the stage instance's hash.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The stage instance's ID.
+    guild: :class:`Guild`
+        The guild that the stage instance is running in.
+    channel_id: :class:`int`
+        The ID of the channel that the stage instance is running in.
+    topic: :class:`str`
+        The topic of the stage instance.
+    privacy_level: :class:`PrivacyLevel`
+        The privacy level of the stage instance.
+    discoverable_disabled: :class:`bool`
+        Whether discoverability for the stage instance is disabled.
+    scheduled_event_id: Optional[:class:`int`]
+        The ID of scheduled event that belongs to the stage instance if any.
+
+        .. versionadded:: 2.0
+    """
+
+    __slots__ = (
+        '_state',
+        'id',
+        'guild',
+        'channel_id',
+        'topic',
+        'privacy_level',
+        'discoverable_disabled',
+        'scheduled_event_id',
+        '_cs_channel',
+        '_cs_scheduled_event',
+    )
+
+    def __init__(self, *, state: ConnectionState, guild: Guild, data: StageInstancePayload) -> None:
+        self._state: ConnectionState = state
+        self.guild: Guild = guild
+        self._update(data)
+
+    def _update(self, data: StageInstancePayload) -> None:
+        self.id: int = int(data['id'])
+        self.channel_id: int = int(data['channel_id'])
+        self.topic: str = data['topic']
+        self.privacy_level: PrivacyLevel = try_enum(PrivacyLevel, data['privacy_level'])
+        self.discoverable_disabled: bool = data.get('discoverable_disabled', False)
+        self.scheduled_event_id: Optional[int] = _get_as_snowflake(data, 'guild_scheduled_event_id')
+
+    def __repr__(self) -> str:
+        return f'<StageInstance id={self.id} guild={self.guild!r} channel_id={self.channel_id} topic={self.topic!r}>'
+
+    @property
+    def discoverable(self) -> bool:
+        """Whether the stage instance is discoverable."""
+        return not self.discoverable_disabled
+
+    @cached_slot_property('_cs_channel')
+    def channel(self) -> Optional[StageChannel]:
+        """Optional[:class:`StageChannel`]: The channel that stage instance is running in."""
+        # The returned channel will always be a StageChannel or None
+        return self._state.get_channel(self.channel_id)  # type: ignore
+
+    @cached_slot_property('_cs_scheduled_event')
+    def scheduled_event(self) -> Optional[ScheduledEvent]:
+        """Optional[:class:`ScheduledEvent`]: The scheduled event that belongs to the stage instance."""
+        # Guild.get_scheduled_event() expects an int, we are passing Optional[int]
+        return self.guild.get_scheduled_event(self.scheduled_event_id)  # type: ignore
+
+    async def edit(
+        self,
+        *,
+        topic: str = MISSING,
+        privacy_level: PrivacyLevel = MISSING,
+        reason: Optional[str] = None,
+    ) -> None:
+        """|coro|
+
+        Edits the stage instance.
+
+        You must have :attr:`~Permissions.manage_channels` to do this.
+
+        Parameters
+        -----------
+        topic: :class:`str`
+            The stage instance's new topic.
+        privacy_level: :class:`PrivacyLevel`
+            The stage instance's new privacy level.
+        reason: :class:`str`
+            The reason the stage instance was edited. Shows up on the audit log.
+
+        Raises
+        ------
+        TypeError
+            If the ``privacy_level`` parameter is not the proper type.
+        Forbidden
+            You do not have permissions to edit the stage instance.
+        HTTPException
+            Editing a stage instance failed.
+        """
+        payload = {}
+
+        if topic is not MISSING:
+            payload['topic'] = topic
+
+        if privacy_level is not MISSING:
+            if not isinstance(privacy_level, PrivacyLevel):
+                raise TypeError('privacy_level field must be of type PrivacyLevel')
+
+            payload['privacy_level'] = privacy_level.value
+
+        if payload:
+            await self._state.http.edit_stage_instance(self.channel_id, **payload, reason=reason)
+
+    async def delete(self, *, reason: Optional[str] = None) -> None:
+        """|coro|
+
+        Deletes the stage instance.
+
+        You must have :attr:`~Permissions.manage_channels` to do this.
+
+        Parameters
+        -----------
+        reason: :class:`str`
+            The reason the stage instance was deleted. Shows up on the audit log.
+
+        Raises
+        ------
+        Forbidden
+            You do not have permissions to delete the stage instance.
+        HTTPException
+            Deleting the stage instance failed.
+        """
+        await self._state.http.delete_stage_instance(self.channel_id, reason=reason)
```

### Comparing `discord.py-self-1.9.2/discord/voice_client.py` & `discord.py-self-2.0.0/discord/voice_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,642 +1,701 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-"""Some documentation to refer to:
-
-- Our main web socket (mWS) sends opcode 4 with a guild ID and channel ID.
-- The mWS receives VOICE_STATE_UPDATE and VOICE_SERVER_UPDATE.
-- We pull the session_id from VOICE_STATE_UPDATE.
-- We pull the token, endpoint and server_id from VOICE_SERVER_UPDATE.
-- Then we initiate the voice web socket (vWS) pointing to the endpoint.
-- We send opcode 0 with the user_id, server_id, session_id and token using the vWS.
-- The vWS sends back opcode 2 with an ssrc, port, modes(array) and hearbeat_interval.
-- We send a UDP discovery packet to endpoint:port and receive our IP and our port in LE.
-- Then we send our IP and port via vWS with opcode 1.
-- When that's all done, we receive opcode 4 from the vWS.
-- Finally we can transmit data to endpoint:port.
-"""
-
-import asyncio
-import socket
-import logging
-import struct
-import threading
-
-from . import opus, utils
-from .backoff import ExponentialBackoff
-from .gateway import *
-from .errors import ClientException, ConnectionClosed
-from .player import AudioPlayer, AudioSource
-
-try:
-    import nacl.secret
-    has_nacl = True
-except ImportError:
-    has_nacl = False
-
-log = logging.getLogger(__name__)
-
-class VoiceProtocol:
-    """A class that represents the Discord voice protocol.
-
-    This is an abstract class. The library provides a concrete implementation
-    under :class:`VoiceClient`.
-
-    This class allows you to implement a protocol to allow for an external
-    method of sending voice, such as Lavalink_ or a native library implementation.
-
-    These classes are passed to :meth:`abc.Connectable.connect`.
-
-    .. _Lavalink: https://github.com/freyacodes/Lavalink
-
-    Parameters
-    ------------
-    client: :class:`Client`
-        The client (or its subclasses) that started the connection request.
-    channel: :class:`abc.Connectable`
-        The voice channel that is being connected to.
-    """
-
-    def __init__(self, client, channel):
-        self.client = client
-        self.channel = channel
-
-    async def on_voice_state_update(self, data):
-        """|coro|
-
-        An abstract method that is called when the client's voice state
-        has changed. This corresponds to ``VOICE_STATE_UPDATE``.
-
-        Parameters
-        ------------
-        data: :class:`dict`
-            The raw `voice state payload`__.
-
-            .. _voice_state_update_payload: https://discord.com/developers/docs/resources/voice#voice-state-object
-
-            __ voice_state_update_payload_
-        """
-        raise NotImplementedError
-
-    async def on_voice_server_update(self, data):
-        """|coro|
-
-        An abstract method that is called when initially connecting to voice.
-        This corresponds to ``VOICE_SERVER_UPDATE``.
-
-        Parameters
-        ------------
-        data: :class:`dict`
-            The raw `voice server update payload`__.
-
-            .. _voice_server_update_payload: https://discord.com/developers/docs/topics/gateway#voice-server-update-voice-server-update-event-fields
-
-            __ voice_server_update_payload_
-        """
-        raise NotImplementedError
-
-    async def connect(self, *, timeout, reconnect):
-        """|coro|
-
-        An abstract method called when the client initiates the connection request.
-
-        When a connection is requested initially, the library calls the constructor
-        under ``__init__`` and then calls :meth:`connect`. If :meth:`connect` fails at
-        some point then :meth:`disconnect` is called.
-
-        Within this method, to start the voice connection flow it is recommended to
-        use :meth:`Guild.change_voice_state` to start the flow. After which,
-        :meth:`on_voice_server_update` and :meth:`on_voice_state_update` will be called.
-        The order that these two are called is unspecified.
-
-        Parameters
-        ------------
-        timeout: :class:`float`
-            The timeout for the connection.
-        reconnect: :class:`bool`
-            Whether reconnection is expected.
-        """
-        raise NotImplementedError
-
-    async def disconnect(self, *, force):
-        """|coro|
-
-        An abstract method called when the client terminates the connection.
-
-        See :meth:`cleanup`.
-
-        Parameters
-        ------------
-        force: :class:`bool`
-            Whether the disconnection was forced.
-        """
-        raise NotImplementedError
-
-    def cleanup(self):
-        """This method *must* be called to ensure proper clean-up during a disconnect.
-
-        It is advisable to call this from within :meth:`disconnect` when you are
-        completely done with the voice protocol instance.
-
-        This method removes it from the internal state cache that keeps track of
-        currently alive voice clients. Failure to clean-up will cause subsequent
-        connections to report that it's still connected.
-        """
-        key_id, _ = self.channel._get_voice_client_key()
-        self.client._connection._remove_voice_client(key_id)
-
-class VoiceClient(VoiceProtocol):
-    """Represents a Discord voice connection.
-
-    You do not create these, you typically get them from
-    e.g. :meth:`VoiceChannel.connect`.
-
-    Warning
-    --------
-    In order to use PCM based AudioSources, you must have the opus library
-    installed on your system and loaded through :func:`opus.load_opus`.
-    Otherwise, your AudioSources must be opus encoded (e.g. using :class:`FFmpegOpusAudio`)
-    or the library will not be able to transmit audio.
-
-    Attributes
-    -----------
-    session_id: :class:`str`
-        The voice connection session ID.
-    token: :class:`str`
-        The voice connection token.
-    endpoint: :class:`str`
-        The endpoint we are connecting to.
-    channel: :class:`abc.Connectable`
-        The voice channel connected to.
-    loop: :class:`asyncio.AbstractEventLoop`
-        The event loop that the voice client is running on.
-    """
-    def __init__(self, client, channel):
-        if not has_nacl:
-            raise RuntimeError("PyNaCl library needed in order to use voice")
-
-        super().__init__(client, channel)
-        state = client._connection
-        self.token = None
-        self.socket = None
-        self.loop = state.loop
-        self._state = state
-        # this will be used in the AudioPlayer thread
-        self._connected = threading.Event()
-
-        self._handshaking = False
-        self._potentially_reconnecting = False
-        self._voice_state_complete = asyncio.Event()
-        self._voice_server_complete = asyncio.Event()
-
-        self.mode = None
-        self._connections = 0
-        self.sequence = 0
-        self.timestamp = 0
-        self._runner = None
-        self._player = None
-        self.encoder = None
-        self._lite_nonce = 0
-        self.ws = None
-
-    warn_nacl = not has_nacl
-    supported_modes = (
-        'xsalsa20_poly1305_lite',
-        'xsalsa20_poly1305_suffix',
-        'xsalsa20_poly1305',
-    )
-
-    @property
-    def guild(self):
-        """Optional[:class:`Guild`]: The guild we're connected to, if applicable."""
-        return getattr(self.channel, 'guild', None)
-
-    @property
-    def user(self):
-        """:class:`ClientUser`: The user connected to voice (i.e. ourselves)."""
-        return self._state.user
-
-    def checked_add(self, attr, value, limit):
-        val = getattr(self, attr)
-        if val + value > limit:
-            setattr(self, attr, 0)
-        else:
-            setattr(self, attr, val + value)
-
-    # connection related
-
-    async def on_voice_state_update(self, data):
-        self.session_id = data['session_id']
-        channel_id = data['channel_id']
-
-        if not self._handshaking or self._potentially_reconnecting:
-            # If we're done handshaking then we just need to update ourselves
-            # If we're potentially reconnecting due to a 4014, then we need to differentiate
-            # a channel move and an actual force disconnect
-            if channel_id is None:
-                # We're being disconnected so cleanup
-                await self.disconnect()
-            else:
-                guild = self.guild
-                self.channel = channel_id and guild and guild.get_channel(int(channel_id))
-        else:
-            self._voice_state_complete.set()
-
-    async def on_voice_server_update(self, data):
-        if self._voice_server_complete.is_set():
-            log.info('Ignoring extraneous voice server update.')
-            return
-
-        self.token = data.get('token')
-        self.server_id = int(data['guild_id'])
-        endpoint = data.get('endpoint')
-
-        if endpoint is None or self.token is None:
-            log.warning('Awaiting endpoint... This requires waiting. ' \
-                        'If timeout occurred considering raising the timeout and reconnecting.')
-            return
-
-        self.endpoint, _, _ = endpoint.rpartition(':')
-        if self.endpoint.startswith('wss://'):
-            # Just in case, strip it off since we're going to add it later
-            self.endpoint = self.endpoint[6:]
-
-        # This gets set later
-        self.endpoint_ip = None
-
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.socket.setblocking(False)
-
-        if not self._handshaking:
-            # If we're not handshaking then we need to terminate our previous connection in the websocket
-            await self.ws.close(4000)
-            return
-
-        self._voice_server_complete.set()
-
-    async def voice_connect(self):
-        await self.channel.guild.change_voice_state(channel=self.channel)
-
-    async def voice_disconnect(self):
-        log.info('The voice handshake is being terminated for Channel ID %s (Guild ID %s)', self.channel.id, self.guild.id)
-        await self.channel.guild.change_voice_state(channel=None)
-
-    def prepare_handshake(self):
-        self._voice_state_complete.clear()
-        self._voice_server_complete.clear()
-        self._handshaking = True
-        log.info('Starting voice handshake... (connection attempt %d)', self._connections + 1)
-        self._connections += 1
-
-    def finish_handshake(self):
-        log.info('Voice handshake complete. Endpoint found %s', self.endpoint)
-        self._handshaking = False
-        self._voice_server_complete.clear()
-        self._voice_state_complete.clear()
-
-    async def connect_websocket(self):
-        ws = await DiscordVoiceWebSocket.from_client(self)
-        self._connected.clear()
-        while ws.secret_key is None:
-            await ws.poll_event()
-        self._connected.set()
-        return ws
-
-    async def connect(self, *, reconnect, timeout):
-        log.info('Connecting to voice...')
-        self.timeout = timeout
-
-        for i in range(5):
-            self.prepare_handshake()
-
-            # This has to be created before we start the flow.
-            futures = [
-                self._voice_state_complete.wait(),
-                self._voice_server_complete.wait(),
-            ]
-
-            # Start the connection flow
-            await self.voice_connect()
-
-            try:
-                await utils.sane_wait_for(futures, timeout=timeout)
-            except asyncio.TimeoutError:
-                await self.disconnect(force=True)
-                raise
-
-            self.finish_handshake()
-
-            try:
-                self.ws = await self.connect_websocket()
-                break
-            except (ConnectionClosed, asyncio.TimeoutError):
-                if reconnect:
-                    log.exception('Failed to connect to voice... Retrying...')
-                    await asyncio.sleep(1 + i * 2.0)
-                    await self.voice_disconnect()
-                    continue
-                else:
-                    raise
-
-        if self._runner is None:
-            self._runner = self.loop.create_task(self.poll_voice_ws(reconnect))
-
-    async def potential_reconnect(self):
-        # Attempt to stop the player thread from playing early
-        self._connected.clear()
-        self.prepare_handshake()
-        self._potentially_reconnecting = True
-        try:
-            # We only care about VOICE_SERVER_UPDATE since VOICE_STATE_UPDATE can come before we get disconnected
-            await asyncio.wait_for(self._voice_server_complete.wait(), timeout=self.timeout)
-        except asyncio.TimeoutError:
-            self._potentially_reconnecting = False
-            await self.disconnect(force=True)
-            return False
-
-        self.finish_handshake()
-        self._potentially_reconnecting = False
-        try:
-            self.ws = await self.connect_websocket()
-        except (ConnectionClosed, asyncio.TimeoutError):
-            return False
-        else:
-            return True
-
-    @property
-    def latency(self):
-        """:class:`float`: Latency between a HEARTBEAT and a HEARTBEAT_ACK in seconds.
-
-        This could be referred to as the Discord Voice WebSocket latency and is
-        an analogue of user's voice latencies as seen in the Discord client.
-
-        .. versionadded:: 1.4
-        """
-        ws = self.ws
-        return float("inf") if not ws else ws.latency
-
-    @property
-    def average_latency(self):
-        """:class:`float`: Average of most recent 20 HEARTBEAT latencies in seconds.
-
-        .. versionadded:: 1.4
-        """
-        ws = self.ws
-        return float("inf") if not ws else ws.average_latency
-
-    async def poll_voice_ws(self, reconnect):
-        backoff = ExponentialBackoff()
-        while True:
-            try:
-                await self.ws.poll_event()
-            except (ConnectionClosed, asyncio.TimeoutError) as exc:
-                if isinstance(exc, ConnectionClosed):
-                    # The following close codes are undocumented so I will document them here.
-                    # 1000 - normal closure (obviously)
-                    # 4014 - voice channel has been deleted.
-                    # 4015 - voice server has crashed
-                    if exc.code in (1000, 4015):
-                        log.info('Disconnecting from voice normally, close code %d.', exc.code)
-                        await self.disconnect()
-                        break
-                    if exc.code == 4014:
-                        log.info('Disconnected from voice by force... potentially reconnecting.')
-                        successful = await self.potential_reconnect()
-                        if not successful:
-                            log.info('Reconnect was unsuccessful, disconnecting from voice normally...')
-                            await self.disconnect()
-                            break
-                        else:
-                            continue
-
-                if not reconnect:
-                    await self.disconnect()
-                    raise
-
-                retry = backoff.delay()
-                log.exception('Disconnected from voice... Reconnecting in %.2fs.', retry)
-                self._connected.clear()
-                await asyncio.sleep(retry)
-                await self.voice_disconnect()
-                try:
-                    await self.connect(reconnect=True, timeout=self.timeout)
-                except asyncio.TimeoutError:
-                    # at this point we've retried 5 times... let's continue the loop.
-                    log.warning('Could not connect to voice... Retrying...')
-                    continue
-
-    async def disconnect(self, *, force=False):
-        """|coro|
-
-        Disconnects this voice client from voice.
-        """
-        if not force and not self.is_connected():
-            return
-
-        self.stop()
-        self._connected.clear()
-
-        try:
-            if self.ws:
-                await self.ws.close()
-
-            await self.voice_disconnect()
-        finally:
-            self.cleanup()
-            if self.socket:
-                self.socket.close()
-
-    async def move_to(self, channel):
-        """|coro|
-
-        Moves you to a different voice channel.
-
-        Parameters
-        -----------
-        channel: :class:`abc.Snowflake`
-            The channel to move to. Must be a voice channel.
-        """
-        await self.channel.guild.change_voice_state(channel=channel)
-
-    def is_connected(self):
-        """Indicates if the voice client is connected to voice."""
-        return self._connected.is_set()
-
-    # audio related
-
-    def _get_voice_packet(self, data):
-        header = bytearray(12)
-
-        # Formulate rtp header
-        header[0] = 0x80
-        header[1] = 0x78
-        struct.pack_into('>H', header, 2, self.sequence)
-        struct.pack_into('>I', header, 4, self.timestamp)
-        struct.pack_into('>I', header, 8, self.ssrc)
-
-        encrypt_packet = getattr(self, '_encrypt_' + self.mode)
-        return encrypt_packet(header, data)
-
-    def _encrypt_xsalsa20_poly1305(self, header, data):
-        box = nacl.secret.SecretBox(bytes(self.secret_key))
-        nonce = bytearray(24)
-        nonce[:12] = header
-
-        return header + box.encrypt(bytes(data), bytes(nonce)).ciphertext
-
-    def _encrypt_xsalsa20_poly1305_suffix(self, header, data):
-        box = nacl.secret.SecretBox(bytes(self.secret_key))
-        nonce = nacl.utils.random(nacl.secret.SecretBox.NONCE_SIZE)
-
-        return header + box.encrypt(bytes(data), nonce).ciphertext + nonce
-
-    def _encrypt_xsalsa20_poly1305_lite(self, header, data):
-        box = nacl.secret.SecretBox(bytes(self.secret_key))
-        nonce = bytearray(24)
-
-        nonce[:4] = struct.pack('>I', self._lite_nonce)
-        self.checked_add('_lite_nonce', 1, 4294967295)
-
-        return header + box.encrypt(bytes(data), bytes(nonce)).ciphertext + nonce[:4]
-
-    def play(self, source, *, after=None):
-        """Plays an :class:`AudioSource`.
-
-        The finalizer, ``after`` is called after the source has been exhausted
-        or an error occurred.
-
-        If an error happens while the audio player is running, the exception is
-        caught and the audio player is then stopped.  If no after callback is
-        passed, any caught exception will be displayed as if it were raised.
-
-        Parameters
-        -----------
-        source: :class:`AudioSource`
-            The audio source we're reading from.
-        after: Callable[[:class:`Exception`], Any]
-            The finalizer that is called after the stream is exhausted.
-            This function must have a single parameter, ``error``, that
-            denotes an optional exception that was raised during playing.
-
-        Raises
-        -------
-        ClientException
-            Already playing audio or not connected.
-        TypeError
-            Source is not a :class:`AudioSource` or after is not a callable.
-        OpusNotLoaded
-            Source is not opus encoded and opus is not loaded.
-        """
-
-        if not self.is_connected():
-            raise ClientException('Not connected to voice.')
-
-        if self.is_playing():
-            raise ClientException('Already playing audio.')
-
-        if not isinstance(source, AudioSource):
-            raise TypeError('source must an AudioSource not {0.__class__.__name__}'.format(source))
-
-        if not self.encoder and not source.is_opus():
-            self.encoder = opus.Encoder()
-
-        self._player = AudioPlayer(source, self, after=after)
-        self._player.start()
-
-    def is_playing(self):
-        """Indicates if we're currently playing audio."""
-        return self._player is not None and self._player.is_playing()
-
-    def is_paused(self):
-        """Indicates if we're playing audio, but if we're paused."""
-        return self._player is not None and self._player.is_paused()
-
-    def stop(self):
-        """Stops playing audio."""
-        if self._player:
-            self._player.stop()
-            self._player = None
-
-    def pause(self):
-        """Pauses the audio playing."""
-        if self._player:
-            self._player.pause()
-
-    def resume(self):
-        """Resumes the audio playing."""
-        if self._player:
-            self._player.resume()
-
-    @property
-    def source(self):
-        """Optional[:class:`AudioSource`]: The audio source being played, if playing.
-
-        This property can also be used to change the audio source currently being played.
-        """
-        return self._player.source if self._player else None
-
-    @source.setter
-    def source(self, value):
-        if not isinstance(value, AudioSource):
-            raise TypeError('expected AudioSource not {0.__class__.__name__}.'.format(value))
-
-        if self._player is None:
-            raise ValueError('Not playing anything.')
-
-        self._player._set_source(value)
-
-    def send_audio_packet(self, data, *, encode=True):
-        """Sends an audio packet composed of the data.
-
-        You must be connected to play audio.
-
-        Parameters
-        ----------
-        data: :class:`bytes`
-            The :term:`py:bytes-like object` denoting PCM or Opus voice data.
-        encode: :class:`bool`
-            Indicates if ``data`` should be encoded into Opus.
-
-        Raises
-        -------
-        ClientException
-            You are not connected.
-        opus.OpusError
-            Encoding the data failed.
-        """
-
-        self.checked_add('sequence', 1, 65535)
-        if encode:
-            encoded_data = self.encoder.encode(data, self.encoder.SAMPLES_PER_FRAME)
-        else:
-            encoded_data = data
-        packet = self._get_voice_packet(encoded_data)
-        try:
-            self.socket.sendto(packet, (self.endpoint_ip, self.voice_port))
-        except BlockingIOError:
-            log.warning('A packet has been dropped (seq: %s, timestamp: %s)', self.sequence, self.timestamp)
-
-        self.checked_add('timestamp', opus.Encoder.SAMPLES_PER_FRAME, 4294967295)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+Some documentation to refer to:
+
+- Our main web socket (mWS) sends opcode 4 with a guild ID and channel ID.
+- The mWS receives VOICE_STATE_UPDATE and VOICE_SERVER_UPDATE.
+- We pull the session_id from VOICE_STATE_UPDATE.
+- We pull the token, endpoint and server_id from VOICE_SERVER_UPDATE.
+- Then we initiate the voice web socket (vWS) pointing to the endpoint.
+- We send opcode 0 with the user_id, server_id, session_id and token using the vWS.
+- The vWS sends back opcode 2 with an ssrc, port, modes(array) and hearbeat_interval.
+- We send a UDP discovery packet to endpoint:port and receive our IP and our port in LE.
+- Then we send our IP and port via vWS with opcode 1.
+- When that's all done, we receive opcode 4 from the vWS.
+- Finally we can transmit data to endpoint:port.
+"""
+
+from __future__ import annotations
+
+import asyncio
+import socket
+import logging
+import struct
+import threading
+from typing import Any, Callable, List, Optional, TYPE_CHECKING, Tuple
+
+from . import opus, utils
+from .backoff import ExponentialBackoff
+from .gateway import *
+from .errors import ClientException, ConnectionClosed
+from .player import AudioPlayer, AudioSource
+from .utils import _get_as_snowflake, MISSING
+
+if TYPE_CHECKING:
+    from .client import Client
+    from .guild import Guild
+    from .state import ConnectionState
+    from .user import ClientUser
+    from .opus import Encoder
+    from . import abc
+
+    from .types.voice import (
+        GuildVoiceState as GuildVoiceStatePayload,
+        VoiceServerUpdate as VoiceServerUpdatePayload,
+        SupportedModes,
+    )
+
+    VocalChannel = abc.VocalChannel
+
+
+has_nacl: bool
+
+try:
+    import nacl.secret  # type: ignore
+    import nacl.utils  # type: ignore
+
+    has_nacl = True
+except ImportError:
+    has_nacl = False
+
+__all__ = (
+    'VoiceProtocol',
+    'VoiceClient',
+)
+
+
+_log = logging.getLogger(__name__)
+
+
+class VoiceProtocol:
+    """A class that represents the Discord voice protocol.
+
+    This is an abstract class. The library provides a concrete implementation
+    under :class:`VoiceClient`.
+
+    This class allows you to implement a protocol to allow for an external
+    method of sending voice, such as Lavalink_ or a native library implementation.
+
+    These classes are passed to :meth:`abc.Connectable.connect <VoiceChannel.connect>`.
+
+    .. _Lavalink: https://github.com/freyacodes/Lavalink
+
+    Parameters
+    ------------
+    client: :class:`Client`
+        The client (or its subclasses) that started the connection request.
+    channel: Union[:class:`VoiceChannel`, :class:`StageChannel`, :class:`DMChannel`, :class:`GroupChannel`]
+        The voice channel that is being connected to.
+    """
+
+    def __init__(self, client: Client, channel: VocalChannel) -> None:
+        self.client: Client = client
+        self.channel: VocalChannel = channel
+
+    async def on_voice_state_update(self, data: GuildVoiceStatePayload, /) -> None:
+        """|coro|
+
+        An abstract method that is called when the client's voice state
+        has changed. This corresponds to ``VOICE_STATE_UPDATE``.
+
+        Parameters
+        ------------
+        data: :class:`dict`
+            The raw :ddocs:`voice state payload <resources/voice#voice-state-object>`.
+        """
+        raise NotImplementedError
+
+    async def on_voice_server_update(self, data: VoiceServerUpdatePayload, /) -> None:
+        """|coro|
+
+        An abstract method that is called when initially connecting to voice.
+        This corresponds to ``VOICE_SERVER_UPDATE``.
+
+        Parameters
+        ------------
+        data: :class:`dict`
+            The raw :ddocs:`voice server update payload <topics/gateway#voice-server-update>`.
+        """
+        raise NotImplementedError
+
+    async def connect(self, *, timeout: float, reconnect: bool, self_deaf: bool = False, self_mute: bool = False) -> None:
+        """|coro|
+
+        An abstract method called when the client initiates the connection request.
+
+        When a connection is requested initially, the library calls the constructor
+        under ``__init__`` and then calls :meth:`connect`. If :meth:`connect` fails at
+        some point then :meth:`disconnect` is called.
+
+        Within this method, to start the voice connection flow it is recommended to
+        use :meth:`Guild.change_voice_state` to start the flow. After which,
+        :meth:`on_voice_server_update` and :meth:`on_voice_state_update` will be called.
+        The order that these two are called is unspecified.
+
+        Parameters
+        ------------
+        timeout: :class:`float`
+            The timeout for the connection.
+        reconnect: :class:`bool`
+            Whether reconnection is expected.
+        self_mute: :class:`bool`
+            Indicates if the client should be self-muted.
+
+            .. versionadded:: 2.0
+        self_deaf: :class:`bool`
+            Indicates if the client should be self-deafened.
+
+            .. versionadded:: 2.0
+        """
+        raise NotImplementedError
+
+    async def disconnect(self, *, force: bool) -> None:
+        """|coro|
+
+        An abstract method called when the client terminates the connection.
+
+        See :meth:`cleanup`.
+
+        Parameters
+        ------------
+        force: :class:`bool`
+            Whether the disconnection was forced.
+        """
+        raise NotImplementedError
+
+    def cleanup(self) -> None:
+        """This method *must* be called to ensure proper clean-up during a disconnect.
+
+        It is advisable to call this from within :meth:`disconnect` when you are
+        completely done with the voice protocol instance.
+
+        This method removes it from the internal state cache that keeps track of
+        currently alive voice clients. Failure to clean-up will cause subsequent
+        connections to report that it's still connected.
+        """
+        key_id, _ = self.channel._get_voice_client_key()
+        self.client._connection._remove_voice_client(key_id)
+
+
+class VoiceClient(VoiceProtocol):
+    """Represents a Discord voice connection.
+
+    You do not create these, you typically get them from
+    e.g. :meth:`VoiceChannel.connect`.
+
+    Warning
+    --------
+    In order to use PCM based AudioSources, you must have the opus library
+    installed on your system and loaded through :func:`opus.load_opus`.
+    Otherwise, your AudioSources must be opus encoded (e.g. using :class:`FFmpegOpusAudio`)
+    or the library will not be able to transmit audio.
+
+    Attributes
+    -----------
+    session_id: :class:`str`
+        The voice connection session ID.
+    token: :class:`str`
+        The voice connection token.
+    endpoint: :class:`str`
+        The endpoint we are connecting to.
+    channel: Union[:class:`VoiceChannel`, :class:`StageChannel`, :class:`DMChannel`, :class:`GroupChannel`]
+        The voice channel connected to.
+    """
+
+    channel: VocalChannel
+    endpoint_ip: str
+    voice_port: int
+    ip: str
+    port: int
+    secret_key: List[int]
+    ssrc: int
+
+    def __init__(self, client: Client, channel: VocalChannel) -> None:
+        if not has_nacl:
+            raise RuntimeError("PyNaCl library needed in order to use voice")
+
+        super().__init__(client, channel)
+        state = client._connection
+        self.token: str = MISSING
+        self.server_id: int = MISSING
+        self.socket = MISSING
+        self.loop: asyncio.AbstractEventLoop = state.loop
+        self._state: ConnectionState = state
+        # this will be used in the AudioPlayer thread
+        self._connected: threading.Event = threading.Event()
+
+        self._handshaking: bool = False
+        self._potentially_reconnecting: bool = False
+        self._voice_state_complete: asyncio.Event = asyncio.Event()
+        self._voice_server_complete: asyncio.Event = asyncio.Event()
+
+        self.mode: str = MISSING
+        self._connections: int = 0
+        self.sequence: int = 0
+        self.timestamp: int = 0
+        self.timeout: float = 0
+        self._runner: asyncio.Task = MISSING
+        self._player: Optional[AudioPlayer] = None
+        self.encoder: Encoder = MISSING
+        self._lite_nonce: int = 0
+        self.ws: DiscordVoiceWebSocket = MISSING
+
+    warn_nacl: bool = not has_nacl
+    supported_modes: Tuple[SupportedModes, ...] = (
+        'xsalsa20_poly1305_lite',
+        'xsalsa20_poly1305_suffix',
+        'xsalsa20_poly1305',
+    )
+
+    @property
+    def guild(self) -> Optional[Guild]:
+        """Optional[:class:`Guild`]: The guild we're connected to, if applicable."""
+        return getattr(self.channel, 'guild', None)
+
+    @property
+    def user(self) -> ClientUser:
+        """:class:`ClientUser`: The user connected to voice (i.e. ourselves)."""
+        return self._state.user  # type: ignore
+
+    def checked_add(self, attr: str, value: int, limit: int) -> None:
+        val = getattr(self, attr)
+        if val + value > limit:
+            setattr(self, attr, 0)
+        else:
+            setattr(self, attr, val + value)
+
+    # connection related
+
+    async def on_voice_state_update(self, data: GuildVoiceStatePayload) -> None:
+        self.session_id: str = data['session_id']
+        channel_id = data['channel_id']
+
+        if not self._handshaking or self._potentially_reconnecting:
+            # If we're done handshaking then we just need to update ourselves
+            # If we're potentially reconnecting due to a 4014, then we need to differentiate
+            # a channel move and an actual force disconnect
+            if channel_id is None:
+                # We're being disconnected so cleanup
+                await self.disconnect()
+            else:
+                self.channel = channel_id and self.guild.get_channel(int(channel_id))  # type: ignore
+        else:
+            self._voice_state_complete.set()
+
+    async def on_voice_server_update(self, data: VoiceServerUpdatePayload) -> None:
+        if self._voice_server_complete.is_set():
+            _log.warning('Ignoring extraneous voice server update.')
+            return
+
+        self.token = data['token']
+        self.server_id = _get_as_snowflake(data, 'guild_id') or int(data['channel_id'])
+        endpoint = data.get('endpoint')
+
+        if endpoint is None or self.token is None:
+            _log.warning(
+                'Awaiting endpoint... This requires waiting. '
+                'If timeout occurred considering raising the timeout and reconnecting.'
+            )
+            return
+
+        self.endpoint, _, _ = endpoint.rpartition(':')
+        if self.endpoint.startswith('wss://'):
+            # Just in case, strip it off since we're going to add it later
+            self.endpoint: str = self.endpoint[6:]
+
+        # This gets set later
+        self.endpoint_ip = MISSING
+
+        self.socket: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.socket.setblocking(False)
+
+        if not self._handshaking:
+            # If we're not handshaking then we need to terminate our previous connection in the websocket
+            await self.ws.close(4000)
+            return
+
+        self._voice_server_complete.set()
+
+    async def voice_connect(self, self_deaf: bool = False, self_mute: bool = False) -> None:
+        channel = self.channel
+        if self.guild:
+            await self.guild.change_voice_state(channel=channel, self_deaf=self_deaf, self_mute=self_mute)
+        else:
+            await self._state.client.change_voice_state(channel=channel, self_deaf=self_deaf, self_mute=self_mute)
+
+    async def voice_disconnect(self) -> None:
+        guild = self.guild
+        _log.info(
+            'The voice handshake is being terminated for channel ID %s (guild ID %s).',
+            self.channel.id,
+            getattr(guild, 'id', None),
+        )
+        if guild:
+            await guild.change_voice_state(channel=None)
+        else:
+            await self._state.client.change_voice_state(channel=None)
+
+    def prepare_handshake(self) -> None:
+        self._voice_state_complete.clear()
+        self._voice_server_complete.clear()
+        self._handshaking = True
+        _log.info('Starting voice handshake (connection attempt %d)...', self._connections + 1)
+        self._connections += 1
+
+    def finish_handshake(self) -> None:
+        _log.info('Voice handshake complete. Endpoint found: %s.', self.endpoint)
+        self._handshaking = False
+        self._voice_server_complete.clear()
+        self._voice_state_complete.clear()
+
+    async def connect_websocket(self) -> DiscordVoiceWebSocket:
+        ws = await DiscordVoiceWebSocket.from_client(self)
+        self._connected.clear()
+        while ws.secret_key is None:
+            await ws.poll_event()
+        self._connected.set()
+        return ws
+
+    async def connect(self, *, reconnect: bool, timeout: float, self_deaf: bool = False, self_mute: bool = False) -> None:
+        _log.info('Connecting to voice...')
+        self.timeout = timeout
+
+        for i in range(5):
+            self.prepare_handshake()
+
+            # This has to be created before we start the flow
+            futures = [
+                self._voice_state_complete.wait(),
+                self._voice_server_complete.wait(),
+            ]
+
+            # Start the connection flow
+            await self.voice_connect(self_deaf=self_deaf, self_mute=self_mute)
+
+            try:
+                await utils.sane_wait_for(futures, timeout=timeout)
+            except asyncio.TimeoutError:
+                await self.disconnect(force=True)
+                raise
+
+            self.finish_handshake()
+
+            try:
+                self.ws = await self.connect_websocket()
+                break
+            except (ConnectionClosed, asyncio.TimeoutError):
+                if reconnect:
+                    _log.exception('Failed to connect to voice... Retrying...')
+                    await asyncio.sleep(1 + i * 2.0)
+                    await self.voice_disconnect()
+                    continue
+                else:
+                    raise
+
+        if self._runner is MISSING:
+            self._runner = self.client.loop.create_task(self.poll_voice_ws(reconnect))
+
+    async def potential_reconnect(self) -> bool:
+        # Attempt to stop the player thread from playing early
+        self._connected.clear()
+        self.prepare_handshake()
+        self._potentially_reconnecting = True
+        try:
+            # We only care about VOICE_SERVER_UPDATE since VOICE_STATE_UPDATE can come before we get disconnected
+            await asyncio.wait_for(self._voice_server_complete.wait(), timeout=self.timeout)
+        except asyncio.TimeoutError:
+            self._potentially_reconnecting = False
+            await self.disconnect(force=True)
+            return False
+
+        self.finish_handshake()
+        self._potentially_reconnecting = False
+        try:
+            self.ws = await self.connect_websocket()
+        except (ConnectionClosed, asyncio.TimeoutError):
+            return False
+        else:
+            return True
+
+    @property
+    def latency(self) -> float:
+        """:class:`float`: Latency between a HEARTBEAT and a HEARTBEAT_ACK in seconds.
+
+        This could be referred to as the Discord Voice WebSocket latency and is
+        an analogue of user's voice latencies as seen in the Discord client.
+
+        .. versionadded:: 1.4
+        """
+        ws = self.ws
+        return float("inf") if not ws else ws.latency
+
+    @property
+    def average_latency(self) -> float:
+        """:class:`float`: Average of most recent 20 HEARTBEAT latencies in seconds.
+
+        .. versionadded:: 1.4
+        """
+        ws = self.ws
+        return float("inf") if not ws else ws.average_latency
+
+    async def poll_voice_ws(self, reconnect: bool) -> None:
+        backoff = ExponentialBackoff()
+        while True:
+            try:
+                await self.ws.poll_event()
+            except (ConnectionClosed, asyncio.TimeoutError) as exc:
+                if isinstance(exc, ConnectionClosed):
+                    # The following close codes are undocumented so I will document them here.
+                    # 1000 - normal closure (obviously)
+                    # 4014 - voice channel has been deleted.
+                    # 4015 - voice server has crashed
+                    if exc.code in (1000, 4015):
+                        _log.info('Disconnecting from voice normally, close code %d.', exc.code)
+                        await self.disconnect()
+                        break
+                    if exc.code == 4014:
+                        _log.info('Disconnected from voice by force... potentially reconnecting.')
+                        successful = await self.potential_reconnect()
+                        if not successful:
+                            _log.info('Reconnect was unsuccessful, disconnecting from voice normally...')
+                            await self.disconnect()
+                            break
+                        else:
+                            continue
+
+                if not reconnect:
+                    await self.disconnect()
+                    raise
+
+                retry = backoff.delay()
+                _log.exception('Disconnected from voice... Reconnecting in %.2fs.', retry)
+                self._connected.clear()
+                await asyncio.sleep(retry)
+                await self.voice_disconnect()
+                try:
+                    await self.connect(reconnect=True, timeout=self.timeout)
+                except asyncio.TimeoutError:
+                    # at this point we've retried 5 times... let's continue the loop.
+                    _log.warning('Could not connect to voice... Retrying...')
+                    continue
+
+    async def disconnect(self, *, force: bool = False) -> None:
+        """|coro|
+
+        Disconnects this voice client from voice.
+        """
+        if not force and not self.is_connected():
+            return
+
+        self.stop()
+        self._connected.clear()
+
+        try:
+            if self.ws:
+                await self.ws.close()
+
+            await self.voice_disconnect()
+        finally:
+            self.cleanup()
+            if self.socket:
+                self.socket.close()
+
+    async def move_to(self, channel: Optional[abc.Snowflake]) -> None:
+        """|coro|
+
+        Moves you to a different voice channel.
+
+        Parameters
+        -----------
+        channel: Optional[:class:`~abc.Snowflake`]
+            The channel to move to. Must be a voice channel.
+        """
+        if self.guild:
+            await self.guild.change_voice_state(channel=channel)
+        else:
+            await self._state.client.change_voice_state(channel=channel)
+
+    def is_connected(self) -> bool:
+        """Indicates if the voice client is connected to voice."""
+        return self._connected.is_set()
+
+    # audio related
+
+    def _get_voice_packet(self, data):
+        header = bytearray(12)
+
+        # Formulate rtp header
+        header[0] = 0x80
+        header[1] = 0x78
+        struct.pack_into('>H', header, 2, self.sequence)
+        struct.pack_into('>I', header, 4, self.timestamp)
+        struct.pack_into('>I', header, 8, self.ssrc)
+
+        encrypt_packet = getattr(self, '_encrypt_' + self.mode)
+        return encrypt_packet(header, data)
+
+    def _encrypt_xsalsa20_poly1305(self, header: bytes, data) -> bytes:
+        box = nacl.secret.SecretBox(bytes(self.secret_key))
+        nonce = bytearray(24)
+        nonce[:12] = header
+
+        return header + box.encrypt(bytes(data), bytes(nonce)).ciphertext
+
+    def _encrypt_xsalsa20_poly1305_suffix(self, header: bytes, data) -> bytes:
+        box = nacl.secret.SecretBox(bytes(self.secret_key))
+        nonce = nacl.utils.random(nacl.secret.SecretBox.NONCE_SIZE)
+
+        return header + box.encrypt(bytes(data), nonce).ciphertext + nonce
+
+    def _encrypt_xsalsa20_poly1305_lite(self, header: bytes, data) -> bytes:
+        box = nacl.secret.SecretBox(bytes(self.secret_key))
+        nonce = bytearray(24)
+
+        nonce[:4] = struct.pack('>I', self._lite_nonce)
+        self.checked_add('_lite_nonce', 1, 4294967295)
+
+        return header + box.encrypt(bytes(data), bytes(nonce)).ciphertext + nonce[:4]
+
+    def play(self, source: AudioSource, *, after: Optional[Callable[[Optional[Exception]], Any]] = None) -> None:
+        """Plays an :class:`AudioSource`.
+
+        The finalizer, ``after`` is called after the source has been exhausted
+        or an error occurred.
+
+        If an error happens while the audio player is running, the exception is
+        caught and the audio player is then stopped.  If no after callback is
+        passed, any caught exception will be logged using the library logger.
+
+        .. versionchanged:: 2.0
+            Instead of writing to ``sys.stderr``, the library's logger is used.
+
+        Parameters
+        -----------
+        source: :class:`AudioSource`
+            The audio source we're reading from.
+        after: Callable[[Optional[:class:`Exception`]], Any]
+            The finalizer that is called after the stream is exhausted.
+            This function must have a single parameter, ``error``, that
+            denotes an optional exception that was raised during playing.
+
+        Raises
+        -------
+        ClientException
+            Already playing audio or not connected.
+        TypeError
+            Source is not a :class:`AudioSource` or after is not a callable.
+        OpusNotLoaded
+            Source is not opus encoded and opus is not loaded.
+        """
+
+        if not self.is_connected():
+            raise ClientException('Not connected to voice.')
+
+        if self.is_playing():
+            raise ClientException('Already playing audio.')
+
+        if not isinstance(source, AudioSource):
+            raise TypeError(f'source must be an AudioSource not {source.__class__.__name__}')
+
+        if not self.encoder and not source.is_opus():
+            self.encoder = opus.Encoder()
+
+        self._player = AudioPlayer(source, self, after=after)
+        self._player.start()
+
+    def is_playing(self) -> bool:
+        """Indicates if we're currently playing audio."""
+        return self._player is not None and self._player.is_playing()
+
+    def is_paused(self) -> bool:
+        """Indicates if we're playing audio, but if we're paused."""
+        return self._player is not None and self._player.is_paused()
+
+    def stop(self) -> None:
+        """Stops playing audio."""
+        if self._player:
+            self._player.stop()
+            self._player = None
+
+    def pause(self) -> None:
+        """Pauses the audio playing."""
+        if self._player:
+            self._player.pause()
+
+    def resume(self) -> None:
+        """Resumes the audio playing."""
+        if self._player:
+            self._player.resume()
+
+    @property
+    def source(self) -> Optional[AudioSource]:
+        """Optional[:class:`AudioSource`]: The audio source being played, if playing.
+
+        This property can also be used to change the audio source currently being played.
+        """
+        return self._player.source if self._player else None
+
+    @source.setter
+    def source(self, value: AudioSource) -> None:
+        if not isinstance(value, AudioSource):
+            raise TypeError(f'expected AudioSource not {value.__class__.__name__}.')
+
+        if self._player is None:
+            raise ValueError('Not playing anything.')
+
+        self._player._set_source(value)
+
+    def send_audio_packet(self, data: bytes, *, encode: bool = True) -> None:
+        """Sends an audio packet composed of the data.
+
+        You must be connected to play audio.
+
+        Parameters
+        ----------
+        data: :class:`bytes`
+            The :term:`py:bytes-like object` denoting PCM or Opus voice data.
+        encode: :class:`bool`
+            Indicates if ``data`` should be encoded into Opus.
+
+        Raises
+        -------
+        ClientException
+            You are not connected.
+        opus.OpusError
+            Encoding the data failed.
+        """
+
+        self.checked_add('sequence', 1, 65535)
+        if encode:
+            encoded_data = self.encoder.encode(data, self.encoder.SAMPLES_PER_FRAME)
+        else:
+            encoded_data = data
+        packet = self._get_voice_packet(encoded_data)
+        try:
+            self.socket.sendto(packet, (self.endpoint_ip, self.voice_port))
+        except BlockingIOError:
+            _log.warning('A packet has been dropped (seq: %s, timestamp: %s)', self.sequence, self.timestamp)
+
+        self.checked_add('timestamp', opus.Encoder.SAMPLES_PER_FRAME, 4294967295)
```

### Comparing `discord.py-self-1.9.2/discord/widget.py` & `discord.py-self-2.0.0/discord/widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,268 +1,321 @@
-# -*- coding: utf-8 -*-
-
-"""
-The MIT License (MIT)
-
-Copyright (c) 2015-present Rapptz
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
-from .utils import snowflake_time, _get_as_snowflake, resolve_invite
-from .user import BaseUser
-from .activity import create_activity
-from .invite import Invite
-from .enums import Status, try_enum
-
-class WidgetChannel:
-    """Represents a "partial" widget channel.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two partial channels are the same.
-
-        .. describe:: x != y
-
-            Checks if two partial channels are not the same.
-
-        .. describe:: hash(x)
-
-            Return the partial channel's hash.
-
-        .. describe:: str(x)
-
-            Returns the partial channel's name.
-
-    Attributes
-    -----------
-    id: :class:`int`
-        The channel's ID.
-    name: :class:`str`
-        The channel's name.
-    position: :class:`int`
-        The channel's position
-    """
-    __slots__ = ('id', 'name', 'position')
-
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.pop('id')
-        self.name = kwargs.pop('name')
-        self.position = kwargs.pop('position')
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return '<WidgetChannel id={0.id} name={0.name!r} position={0.position!r}>'.format(self)
-
-    @property
-    def mention(self):
-        """:class:`str`: The string that allows you to mention the channel."""
-        return '<#%s>' % self.id
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the channel's creation time in UTC."""
-        return snowflake_time(self.id)
-
-class WidgetMember(BaseUser):
-    """Represents a "partial" member of the widget's guild.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two widget members are the same.
-
-        .. describe:: x != y
-
-            Checks if two widget members are not the same.
-
-        .. describe:: hash(x)
-
-            Return the widget member's hash.
-
-        .. describe:: str(x)
-
-            Returns the widget member's `name#discriminator`.
-
-    Attributes
-    -----------
-    id: :class:`int`
-        The member's ID.
-    name: :class:`str`
-        The member's username.
-    discriminator: :class:`str`
-        The member's discriminator.
-    bot: :class:`bool`
-        Whether the member is a bot.
-    status: :class:`Status`
-        The member's status.
-    nick: Optional[:class:`str`]
-        The member's nickname.
-    avatar: Optional[:class:`str`]
-        The member's avatar hash.
-    activity: Optional[Union[:class:`BaseActivity`, :class:`Spotify`]]
-        The member's activity.
-    deafened: Optional[:class:`bool`]
-        Whether the member is currently deafened.
-    muted: Optional[:class:`bool`]
-        Whether the member is currently muted.
-    suppress: Optional[:class:`bool`]
-        Whether the member is currently being suppressed.
-    connected_channel: Optional[:class:`VoiceChannel`]
-        Which channel the member is connected to.
-    """
-    __slots__ = ('name', 'status', 'nick', 'avatar', 'discriminator',
-                 'id', 'bot', 'activity', 'deafened', 'suppress', 'muted',
-                 'connected_channel')
-
-    def __init__(self, *, state, data, connected_channel=None):
-        super().__init__(state=state, data=data)
-        self.nick = data.get('nick')
-        self.status = try_enum(Status, data.get('status'))
-        self.deafened = data.get('deaf', False) or data.get('self_deaf', False)
-        self.muted = data.get('mute', False) or data.get('self_mute', False)
-        self.suppress = data.get('suppress', False)
-
-        try:
-            game = data['game']
-        except KeyError:
-            self.activity = None
-        else:
-            self.activity = create_activity(game)
-
-        self.connected_channel = connected_channel
-
-    @property
-    def display_name(self):
-        """:class:`str`: Returns the member's display name."""
-        return self.nick or self.name
-
-class Widget:
-    """Represents a :class:`Guild` widget.
-
-    .. container:: operations
-
-        .. describe:: x == y
-
-            Checks if two widgets are the same.
-
-        .. describe:: x != y
-
-            Checks if two widgets are not the same.
-
-        .. describe:: str(x)
-
-            Returns the widget's JSON URL.
-
-    Attributes
-    -----------
-    id: :class:`int`
-        The guild's ID.
-    name: :class:`str`
-        The guild's name.
-    channels: Optional[List[:class:`WidgetChannel`]]
-        The accessible voice channels in the guild.
-    members: Optional[List[:class:`Member`]]
-        The online members in the server. Offline members
-        do not appear in the widget.
-
-        .. note::
-
-            Due to a Discord limitation, if this data is available
-            the users will be "anonymized" with linear IDs and discriminator
-            information being incorrect. Likewise, the number of members
-            retrieved is capped.
-
-    """
-    __slots__ = ('_state', 'channels', '_invite', 'id', 'members', 'name')
-
-    def __init__(self, *, state, data):
-        self._state = state
-        self._invite = data['instant_invite']
-        self.name = data['name']
-        self.id = int(data['id'])
-
-        self.channels = []
-        for channel in data.get('channels', []):
-            _id = int(channel['id'])
-            self.channels.append(WidgetChannel(id=_id, name=channel['name'], position=channel['position']))
-
-        self.members = []
-        channels = {channel.id: channel for channel in self.channels}
-        for member in data.get('members', []):
-            connected_channel = _get_as_snowflake(member, 'channel_id')
-            if connected_channel in channels:
-                connected_channel = channels[connected_channel]
-            elif connected_channel:
-                connected_channel = WidgetChannel(id=connected_channel, name='', position=0)
-
-            self.members.append(WidgetMember(state=self._state, data=member, connected_channel=connected_channel))
-
-    def __str__(self):
-        return self.json_url
-
-    def __eq__(self, other):
-        return self.id == other.id
-
-    def __repr__(self):
-        return '<Widget id={0.id} name={0.name!r} invite_url={0.invite_url!r}>'.format(self)
-
-    @property
-    def created_at(self):
-        """:class:`datetime.datetime`: Returns the member's creation time in UTC."""
-        return snowflake_time(self.id)
-
-    @property
-    def json_url(self):
-        """:class:`str`: The JSON URL of the widget."""
-        return "https://discord.com/api/guilds/{0.id}/widget.json".format(self)
-
-    @property
-    def invite_url(self):
-        """Optional[:class:`str`]: The invite URL for the guild, if available."""
-        return self._invite
-
-    async def fetch_invite(self, *, with_counts=True):
-        """|coro|
-
-        Retrieves an :class:`Invite` from a invite URL or ID.
-        This is the same as :meth:`Client.fetch_invite`; the invite
-        code is abstracted away.
-
-        Parameters
-        -----------
-        with_counts: :class:`bool`
-            Whether to include count information in the invite. This fills the
-            :attr:`Invite.approximate_member_count` and :attr:`Invite.approximate_presence_count`
-            fields.
-
-        Returns
-        --------
-        :class:`Invite`
-            The invite from the URL/ID.
-        """
-        if self._invite:
-            invite_id = resolve_invite(self._invite)
-            data = await self._state.http.get_invite(invite_id, with_counts=with_counts)
-            return Invite.from_incomplete(state=self._state, data=data)
+"""
+The MIT License (MIT)
+
+Copyright (c) 2015-present Rapptz
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import List, Optional, TYPE_CHECKING, Union
+
+from .utils import snowflake_time, _get_as_snowflake, resolve_invite
+from .user import BaseUser
+from .activity import BaseActivity, Spotify, create_activity
+from .invite import Invite
+from .enums import Status, try_enum
+
+if TYPE_CHECKING:
+    import datetime
+    from .state import ConnectionState
+    from .types.widget import (
+        WidgetMember as WidgetMemberPayload,
+        Widget as WidgetPayload,
+    )
+
+__all__ = (
+    'WidgetChannel',
+    'WidgetMember',
+    'Widget',
+)
+
+
+class WidgetChannel:
+    """Represents a "partial" widget channel.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two partial channels are the same.
+
+        .. describe:: x != y
+
+            Checks if two partial channels are not the same.
+
+        .. describe:: hash(x)
+
+            Return the partial channel's hash.
+
+        .. describe:: str(x)
+
+            Returns the partial channel's name.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The channel's ID.
+    name: :class:`str`
+        The channel's name.
+    position: :class:`int`
+        The channel's position
+    """
+
+    __slots__ = ('id', 'name', 'position')
+
+    def __init__(self, id: int, name: str, position: int) -> None:
+        self.id: int = id
+        self.name: str = name
+        self.position: int = position
+
+    def __str__(self) -> str:
+        return self.name
+
+    def __repr__(self) -> str:
+        return f'<WidgetChannel id={self.id} name={self.name!r} position={self.position!r}>'
+
+    @property
+    def mention(self) -> str:
+        """:class:`str`: The string that allows you to mention the channel."""
+        return f'<#{self.id}>'
+
+    @property
+    def created_at(self) -> datetime.datetime:
+        """:class:`datetime.datetime`: Returns the channel's creation time in UTC."""
+        return snowflake_time(self.id)
+
+
+class WidgetMember(BaseUser):
+    """Represents a "partial" member of the widget's guild.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two widget members are the same.
+
+        .. describe:: x != y
+
+            Checks if two widget members are not the same.
+
+        .. describe:: hash(x)
+
+            Return the widget member's hash.
+
+        .. describe:: str(x)
+
+            Returns the widget member's ``name#discriminator``.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The member's ID.
+    name: :class:`str`
+        The member's username.
+    discriminator: :class:`str`
+        The member's discriminator.
+    bot: :class:`bool`
+        Whether the member is a bot.
+    status: :class:`Status`
+        The member's status.
+    nick: Optional[:class:`str`]
+        The member's nickname.
+    activity: Optional[Union[:class:`BaseActivity`, :class:`Spotify`]]
+        The member's activity.
+    deafened: Optional[:class:`bool`]
+        Whether the member is currently deafened.
+    muted: Optional[:class:`bool`]
+        Whether the member is currently muted.
+    suppress: Optional[:class:`bool`]
+        Whether the member is currently being suppressed.
+    connected_channel: Optional[:class:`WidgetChannel`]
+        Which channel the member is connected to.
+    """
+
+    __slots__ = (
+        'status',
+        'nick',
+        'avatar',
+        'activity',
+        'deafened',
+        'suppress',
+        'muted',
+        'connected_channel',
+    )
+
+    if TYPE_CHECKING:
+        activity: Optional[Union[BaseActivity, Spotify]]
+
+    def __init__(
+        self,
+        *,
+        state: ConnectionState,
+        data: WidgetMemberPayload,
+        connected_channel: Optional[WidgetChannel] = None,
+    ) -> None:
+        super().__init__(state=state, data=data)
+        self.nick: Optional[str] = data.get('nick')
+        self.status: Status = try_enum(Status, data.get('status'))
+        self.deafened: Optional[bool] = data.get('deaf', False) or data.get('self_deaf', False)
+        self.muted: Optional[bool] = data.get('mute', False) or data.get('self_mute', False)
+        self.suppress: Optional[bool] = data.get('suppress', False)
+
+        try:
+            game = data['game']
+        except KeyError:
+            activity = None
+        else:
+            activity = create_activity(game, state)
+
+        self.activity: Optional[Union[BaseActivity, Spotify]] = activity
+
+        self.connected_channel: Optional[WidgetChannel] = connected_channel
+
+    def __repr__(self) -> str:
+        return (
+            f"<WidgetMember name={self.name!r} discriminator={self.discriminator!r}" f" bot={self.bot} nick={self.nick!r}>"
+        )
+
+    @property
+    def display_name(self) -> str:
+        """:class:`str`: Returns the member's display name."""
+        return self.nick or self.name
+
+
+class Widget:
+    """Represents a :class:`Guild` widget.
+
+    .. container:: operations
+
+        .. describe:: x == y
+
+            Checks if two widgets are the same.
+
+        .. describe:: x != y
+
+            Checks if two widgets are not the same.
+
+        .. describe:: str(x)
+
+            Returns the widget's JSON URL.
+
+    Attributes
+    -----------
+    id: :class:`int`
+        The guild's ID.
+    name: :class:`str`
+        The guild's name.
+    channels: List[:class:`WidgetChannel`]
+        The accessible voice channels in the guild.
+    members: List[:class:`WidgetMember`]
+        The online members in the guild. Offline members
+        do not appear in the widget.
+
+        .. note::
+
+            Due to a Discord limitation, if this data is available
+            the users will be "anonymized" with linear IDs and discriminator
+            information being incorrect. Likewise, the number of members
+            retrieved is capped.
+    presence_count: :class:`int`
+        The approximate number of online members in the guild.
+        Offline members are not included in this count.
+
+        .. versionadded:: 2.0
+
+    """
+
+    __slots__ = ('_state', 'channels', '_invite', 'id', 'members', 'name', 'presence_count')
+
+    def __init__(self, *, state: ConnectionState, data: WidgetPayload) -> None:
+        self._state = state
+        self._invite = data['instant_invite']
+        self.name: str = data['name']
+        self.id: int = int(data['id'])
+
+        self.channels: List[WidgetChannel] = []
+        for channel in data.get('channels', []):
+            _id = int(channel['id'])
+            self.channels.append(WidgetChannel(id=_id, name=channel['name'], position=channel['position']))
+
+        self.members: List[WidgetMember] = []
+        channels = {channel.id: channel for channel in self.channels}
+        for member in data.get('members', []):
+            connected_channel = _get_as_snowflake(member, 'channel_id')
+            if connected_channel is not None:
+                if connected_channel in channels:
+                    connected_channel = channels[connected_channel]
+                else:
+                    connected_channel = WidgetChannel(id=connected_channel, name='', position=0)
+
+            self.members.append(WidgetMember(state=self._state, data=member, connected_channel=connected_channel))
+
+        self.presence_count: int = data['presence_count']
+
+    def __str__(self) -> str:
+        return self.json_url
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, Widget):
+            return self.id == other.id
+        return False
+
+    def __repr__(self) -> str:
+        return f'<Widget id={self.id} name={self.name!r} invite_url={self.invite_url!r}>'
+
+    @property
+    def created_at(self) -> datetime.datetime:
+        """:class:`datetime.datetime`: Returns the member's creation time in UTC."""
+        return snowflake_time(self.id)
+
+    @property
+    def json_url(self) -> str:
+        """:class:`str`: The JSON URL of the widget."""
+        return f"https://discord.com/api/guilds/{self.id}/widget.json"
+
+    @property
+    def invite_url(self) -> Optional[str]:
+        """Optional[:class:`str`]: The invite URL for the guild, if available."""
+        return self._invite
+
+    async def fetch_invite(self, *, with_counts: bool = True) -> Optional[Invite]:
+        """|coro|
+
+        Retrieves an :class:`Invite` from the widget's invite URL.
+        This is the same as :meth:`Client.fetch_invite`; the invite
+        code is abstracted away.
+
+        Parameters
+        -----------
+        with_counts: :class:`bool`
+            Whether to include count information in the invite. This fills the
+            :attr:`Invite.approximate_member_count` and :attr:`Invite.approximate_presence_count`
+            fields.
+
+        Returns
+        --------
+        Optional[:class:`Invite`]
+            The invite from the widget's invite URL, if available.
+        """
+        if self._invite:
+            resolved = resolve_invite(self._invite)
+            data = await self._state.http.get_invite(resolved.code, with_counts=with_counts)
+            return Invite.from_incomplete(state=self._state, data=data)
+        return None
```

