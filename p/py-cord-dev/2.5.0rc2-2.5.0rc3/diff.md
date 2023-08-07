# Comparing `tmp/py-cord-dev-2.5.0rc2.tar.gz` & `tmp/py-cord-dev-2.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-cord-dev-2.5.0rc2.tar", last modified: Sun Aug  6 18:48:44 2023, max compression
+gzip compressed data, was "py-cord-dev-2.5.0rc3.tar", last modified: Mon Aug  7 17:27:40 2023, max compression
```

## Comparing `py-cord-dev-2.5.0rc2.tar` & `py-cord-dev-2.5.0rc3.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.930996 py-cord-dev-2.5.0rc2/
--rw-rw-rw-   0        0        0       13 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/.gitattributes
--rw-rw-rw-   0        0        0     4191 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1146 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/LICENSE
--rw-rw-rw-   0        0        0      393 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/MANIFEST.in
--rw-rw-rw-   0        0        0     5949 2023-08-06 18:48:44.930996 py-cord-dev-2.5.0rc2/PKG-INFO
--rw-rw-rw-   0        0        0     4592 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/README.rst
--rw-rw-rw-   0        0        0      357 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/codecov.yml
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.715330 py-cord-dev-2.5.0rc2/discord/
--rw-rw-rw-   0        0        0     1822 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/__init__.py
--rw-rw-rw-   0        0        0    11015 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/discord/__main__.py
--rw-rw-rw-   0        0        0     1540 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/_typed_dict.py
--rw-rw-rw-   0        0        0     4918 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/discord/_version.py
--rw-rw-rw-   0        0        0    67010 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/abc.py
--rw-rw-rw-   0        0        0    27361 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/activity.py
--rw-rw-rw-   0        0        0     9033 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/appinfo.py
--rw-rw-rw-   0        0        0     5016 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/application_role_connection.py
--rw-rw-rw-   0        0        0    13736 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/asset.py
--rw-rw-rw-   0        0        0    25325 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/audit_logs.py
--rw-rw-rw-   0        0        0    19206 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/automod.py
--rw-rw-rw-   0        0        0     3861 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/backoff.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.741958 py-cord-dev-2.5.0rc2/discord/bin/
--rw-rw-rw-   0        0        0   441856 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/discord/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/discord/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0    59151 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/bot.py
--rw-rw-rw-   0        0        0   109587 2023-06-14 01:02:16.000000 py-cord-dev-2.5.0rc2/discord/channel.py
--rw-rw-rw-   0        0        0    67238 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/client.py
--rw-rw-rw-   0        0        0    42772 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/cog.py
--rw-rw-rw-   0        0        0    11443 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/colour.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.771614 py-cord-dev-2.5.0rc2/discord/commands/
--rw-rw-rw-   0        0        0     1255 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc2/discord/commands/__init__.py
--rw-rw-rw-   0        0        0    13905 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/commands/context.py
--rw-rw-rw-   0        0        0    74246 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/commands/core.py
--rw-rw-rw-   0        0        0    17719 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/commands/options.py
--rw-rw-rw-   0        0        0     4532 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/commands/permissions.py
--rw-rw-rw-   0        0        0    16676 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/components.py
--rw-rw-rw-   0        0        0     3029 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/context_managers.py
--rw-rw-rw-   0        0        0    31823 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/discord/embeds.py
--rw-rw-rw-   0        0        0     8563 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/emoji.py
--rw-rw-rw-   0        0        0    27260 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/enums.py
--rw-rw-rw-   0        0        0    13270 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/errors.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.546416 py-cord-dev-2.5.0rc2/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.778140 py-cord-dev-2.5.0rc2/discord/ext/bridge/
--rw-rw-rw-   0        0        0     1223 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc2/discord/ext/bridge/__init__.py
--rw-rw-rw-   0        0        0     8136 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ext/bridge/bot.py
--rw-rw-rw-   0        0        0     8308 2023-06-12 14:17:39.000000 py-cord-dev-2.5.0rc2/discord/ext/bridge/context.py
--rw-rw-rw-   0        0        0    22210 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ext/bridge/core.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.820099 py-cord-dev-2.5.0rc2/discord/ext/commands/
--rw-rw-rw-   0        0        0      443 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1857 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    16614 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0     3149 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    14930 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0    41377 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0    13211 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    84560 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0    30390 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22700 2023-06-12 14:17:39.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    50152 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0     6282 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.823475 py-cord-dev-2.5.0rc2/discord/ext/pages/
--rw-rw-rw-   0        0        0      227 2022-01-28 03:12:53.000000 py-cord-dev-2.5.0rc2/discord/ext/pages/__init__.py
--rw-rw-rw-   0        0        0    54300 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/ext/pages/pagination.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.825492 py-cord-dev-2.5.0rc2/discord/ext/tasks/
--rw-rw-rw-   0        0        0    27566 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     4963 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/file.py
--rw-rw-rw-   0        0        0    48121 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/flags.py
--rw-rw-rw-   0        0        0    33282 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/gateway.py
--rw-rw-rw-   0        0        0   131780 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/guild.py
--rw-rw-rw-   0        0        0    94082 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/http.py
--rw-rw-rw-   0        0        0    12173 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/integrations.py
--rw-rw-rw-   0        0        0    49768 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/interactions.py
--rw-rw-rw-   0        0        0    19718 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/invite.py
--rw-rw-rw-   0        0        0    31379 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/iterators.py
--rw-rw-rw-   0        0        0    39029 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/member.py
--rw-rw-rw-   0        0        0     5907 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/mentions.py
--rw-rw-rw-   0        0        0    74885 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/message.py
--rw-rw-rw-   0        0        0     1618 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/mixins.py
--rw-rw-rw-   0        0        0     3496 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/object.py
--rw-rw-rw-   0        0        0     3893 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/oggparse.py
--rw-rw-rw-   0        0        0    17472 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/opus.py
--rw-rw-rw-   0        0        0     7578 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    28130 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/permissions.py
--rw-rw-rw-   0        0        0    27838 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/player.py
--rw-rw-rw-   0        0        0        0 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/discord/py.typed
--rw-rw-rw-   0        0        0    26527 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/raw_models.py
--rw-rw-rw-   0        0        0     7286 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/reaction.py
--rw-rw-rw-   0        0        0    16751 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/role.py
--rw-rw-rw-   0        0        0    19178 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/scheduled_events.py
--rw-rw-rw-   0        0        0    20306 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/shard.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.839069 py-cord-dev-2.5.0rc2/discord/sinks/
--rw-rw-rw-   0        0        0      392 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc2/discord/sinks/__init__.py
--rw-rw-rw-   0        0        0     6483 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/sinks/core.py
--rw-rw-rw-   0        0        0     2539 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/sinks/errors.py
--rw-rw-rw-   0        0        0     3317 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/m4a.py
--rw-rw-rw-   0        0        0     3084 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/mka.py
--rw-rw-rw-   0        0        0     3052 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/mkv.py
--rw-rw-rw-   0        0        0     3079 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/mp3.py
--rw-rw-rw-   0        0        0     3316 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/mp4.py
--rw-rw-rw-   0        0        0     3079 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc2/discord/sinks/ogg.py
--rw-rw-rw-   0        0        0     1610 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc2/discord/sinks/pcm.py
--rw-rw-rw-   0        0        0     2385 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/sinks/wave.py
--rw-rw-rw-   0        0        0     6523 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/stage_instance.py
--rw-rw-rw-   0        0        0    75924 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/state.py
--rw-rw-rw-   0        0        0    16774 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/sticker.py
--rw-rw-rw-   0        0        0     5563 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/team.py
--rw-rw-rw-   0        0        0     9590 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/template.py
--rw-rw-rw-   0        0        0    31552 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/threads.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.888411 py-cord-dev-2.5.0rc2/discord/types/
--rw-rw-rw-   0        0        0      192 2022-02-05 14:29:40.000000 py-cord-dev-2.5.0rc2/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2864 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/activity.py
--rw-rw-rw-   0        0        0     2053 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/appinfo.py
--rw-rw-rw-   0        0        0     1589 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc2/discord/types/application_role_connection.py
--rw-rw-rw-   0        0        0     6992 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     2881 2023-04-25 15:17:38.000000 py-cord-dev-2.5.0rc2/discord/types/automod.py
--rw-rw-rw-   0        0        0     4835 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/channel.py
--rw-rw-rw-   0        0        0     2630 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/components.py
--rw-rw-rw-   0        0        0     2486 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/embed.py
--rw-rw-rw-   0        0        0     1637 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/emoji.py
--rw-rw-rw-   0        0        0     1451 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5555 2023-01-30 15:33:07.000000 py-cord-dev-2.5.0rc2/discord/types/guild.py
--rw-rw-rw-   0        0        0     2341 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/integration.py
--rw-rw-rw-   0        0        0     7121 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2853 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/invite.py
--rw-rw-rw-   0        0        0     1925 2022-07-04 17:05:58.000000 py-cord-dev-2.5.0rc2/discord/types/member.py
--rw-rw-rw-   0        0        0     4083 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/types/message.py
--rw-rw-rw-   0        0        0     4011 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/types/raw_models.py
--rw-rw-rw-   0        0        0     1620 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/role.py
--rw-rw-rw-   0        0        0     2141 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/scheduled_events.py
--rw-rw-rw-   0        0        0     1254 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc2/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2449 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/sticker.py
--rw-rw-rw-   0        0        0     1569 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/team.py
--rw-rw-rw-   0        0        0     1685 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/template.py
--rw-rw-rw-   0        0        0     2387 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/threads.py
--rw-rw-rw-   0        0        0     1686 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/types/user.py
--rw-rw-rw-   0        0        0     2412 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/voice.py
--rw-rw-rw-   0        0        0     2046 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1524 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1947 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.900007 py-cord-dev-2.5.0rc2/discord/ui/
--rw-rw-rw-   0        0        0      330 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/ui/__init__.py
--rw-rw-rw-   0        0        0    11075 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ui/button.py
--rw-rw-rw-   0        0        0     8368 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ui/input_text.py
--rw-rw-rw-   0        0        0     4334 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ui/item.py
--rw-rw-rw-   0        0        0    11652 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/ui/modal.py
--rw-rw-rw-   0        0        0    25702 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ui/select.py
--rw-rw-rw-   0        0        0    22215 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/ui/view.py
--rw-rw-rw-   0        0        0    18286 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/user.py
--rw-rw-rw-   0        0        0    43348 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/utils.py
--rw-rw-rw-   0        0        0    33725 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.907179 py-cord-dev-2.5.0rc2/discord/webhook/
--rw-rw-rw-   0        0        0      249 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc2/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    66862 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    42708 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     8034 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc2/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10838 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc2/discord/widget.py
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.916834 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/
--rw-rw-rw-   0        0        0     5949 2023-08-06 18:48:44.000000 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-08-06 18:48:44.000000 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 18:48:44.000000 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      345 2023-08-06 18:48:44.000000 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-06 18:48:44.000000 py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2592 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-06 18:48:44.928977 py-cord-dev-2.5.0rc2/requirements/
--rw-rw-rw-   0        0        0       73 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc2/requirements/_.txt
--rw-rw-rw-   0        0        0       53 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc2/requirements/all.txt
--rw-rw-rw-   0        0        0      183 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/requirements/dev.txt
--rw-rw-rw-   0        0        0      200 2023-08-06 18:44:47.000000 py-cord-dev-2.5.0rc2/requirements/docs.txt
--rw-rw-rw-   0        0        0       36 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc2/requirements/speed.txt
--rw-rw-rw-   0        0        0       20 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc2/requirements/voice.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 18:48:44.932002 py-cord-dev-2.5.0rc2/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.527505 py-cord-dev-2.5.0rc3/
+-rw-rw-rw-   0        0        0       13 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/.gitattributes
+-rw-rw-rw-   0        0        0     4191 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1146 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/LICENSE
+-rw-rw-rw-   0        0        0      393 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5949 2023-08-07 17:27:40.526497 py-cord-dev-2.5.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     4592 2023-08-07 01:56:46.000000 py-cord-dev-2.5.0rc3/README.rst
+-rw-rw-rw-   0        0        0      357 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.408921 py-cord-dev-2.5.0rc3/discord/
+-rw-rw-rw-   0        0        0     1822 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/__init__.py
+-rw-rw-rw-   0        0        0    11015 2023-08-07 01:56:46.000000 py-cord-dev-2.5.0rc3/discord/__main__.py
+-rw-rw-rw-   0        0        0     1540 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/_typed_dict.py
+-rw-rw-rw-   0        0        0     4918 2023-08-07 01:56:46.000000 py-cord-dev-2.5.0rc3/discord/_version.py
+-rw-rw-rw-   0        0        0    67010 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/abc.py
+-rw-rw-rw-   0        0        0    27361 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/activity.py
+-rw-rw-rw-   0        0        0     9033 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/appinfo.py
+-rw-rw-rw-   0        0        0     5016 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/application_role_connection.py
+-rw-rw-rw-   0        0        0    13736 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/asset.py
+-rw-rw-rw-   0        0        0    25325 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    19206 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/automod.py
+-rw-rw-rw-   0        0        0     3861 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/backoff.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.411439 py-cord-dev-2.5.0rc3/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0    59151 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/bot.py
+-rw-rw-rw-   0        0        0   109587 2023-06-14 01:02:16.000000 py-cord-dev-2.5.0rc3/discord/channel.py
+-rw-rw-rw-   0        0        0    67238 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/client.py
+-rw-rw-rw-   0        0        0    42772 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/cog.py
+-rw-rw-rw-   0        0        0    11443 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/colour.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.418517 py-cord-dev-2.5.0rc3/discord/commands/
+-rw-rw-rw-   0        0        0     1255 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc3/discord/commands/__init__.py
+-rw-rw-rw-   0        0        0    13905 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/commands/context.py
+-rw-rw-rw-   0        0        0    74246 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/commands/core.py
+-rw-rw-rw-   0        0        0    17719 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/commands/options.py
+-rw-rw-rw-   0        0        0     4532 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/commands/permissions.py
+-rw-rw-rw-   0        0        0    16676 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/components.py
+-rw-rw-rw-   0        0        0     3029 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/context_managers.py
+-rw-rw-rw-   0        0        0    32097 2023-08-07 17:11:15.000000 py-cord-dev-2.5.0rc3/discord/embeds.py
+-rw-rw-rw-   0        0        0     8563 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/emoji.py
+-rw-rw-rw-   0        0        0    27260 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/enums.py
+-rw-rw-rw-   0        0        0    13270 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.298548 py-cord-dev-2.5.0rc3/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.423042 py-cord-dev-2.5.0rc3/discord/ext/bridge/
+-rw-rw-rw-   0        0        0     1223 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc3/discord/ext/bridge/__init__.py
+-rw-rw-rw-   0        0        0     8136 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ext/bridge/bot.py
+-rw-rw-rw-   0        0        0     8308 2023-06-12 14:17:39.000000 py-cord-dev-2.5.0rc3/discord/ext/bridge/context.py
+-rw-rw-rw-   0        0        0    22210 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ext/bridge/core.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.444672 py-cord-dev-2.5.0rc3/discord/ext/commands/
+-rw-rw-rw-   0        0        0      443 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1857 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    16614 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0     3149 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    14930 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    41377 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    13211 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    84560 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30390 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22700 2023-06-12 14:17:39.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    50152 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0     6282 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.447692 py-cord-dev-2.5.0rc3/discord/ext/pages/
+-rw-rw-rw-   0        0        0      227 2022-01-28 03:12:53.000000 py-cord-dev-2.5.0rc3/discord/ext/pages/__init__.py
+-rw-rw-rw-   0        0        0    58037 2023-08-07 01:56:50.000000 py-cord-dev-2.5.0rc3/discord/ext/pages/pagination.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.448690 py-cord-dev-2.5.0rc3/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    27566 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4963 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/file.py
+-rw-rw-rw-   0        0        0    48121 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/flags.py
+-rw-rw-rw-   0        0        0    33282 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/gateway.py
+-rw-rw-rw-   0        0        0   131780 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/guild.py
+-rw-rw-rw-   0        0        0    94082 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/http.py
+-rw-rw-rw-   0        0        0    12173 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/integrations.py
+-rw-rw-rw-   0        0        0    49768 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/interactions.py
+-rw-rw-rw-   0        0        0    19718 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/invite.py
+-rw-rw-rw-   0        0        0    31379 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/iterators.py
+-rw-rw-rw-   0        0        0    39029 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/member.py
+-rw-rw-rw-   0        0        0     5907 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/mentions.py
+-rw-rw-rw-   0        0        0    74885 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/message.py
+-rw-rw-rw-   0        0        0     1618 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/mixins.py
+-rw-rw-rw-   0        0        0     3496 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/object.py
+-rw-rw-rw-   0        0        0     3893 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/oggparse.py
+-rw-rw-rw-   0        0        0    17472 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/opus.py
+-rw-rw-rw-   0        0        0     7578 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    28130 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/permissions.py
+-rw-rw-rw-   0        0        0    27838 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/player.py
+-rw-rw-rw-   0        0        0        0 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/discord/py.typed
+-rw-rw-rw-   0        0        0    26527 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/raw_models.py
+-rw-rw-rw-   0        0        0     7286 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/reaction.py
+-rw-rw-rw-   0        0        0    16751 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/role.py
+-rw-rw-rw-   0        0        0    19178 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/scheduled_events.py
+-rw-rw-rw-   0        0        0    20306 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/shard.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.462791 py-cord-dev-2.5.0rc3/discord/sinks/
+-rw-rw-rw-   0        0        0      392 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc3/discord/sinks/__init__.py
+-rw-rw-rw-   0        0        0     6483 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/sinks/core.py
+-rw-rw-rw-   0        0        0     2539 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/sinks/errors.py
+-rw-rw-rw-   0        0        0     3317 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/m4a.py
+-rw-rw-rw-   0        0        0     3084 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/mka.py
+-rw-rw-rw-   0        0        0     3052 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/mkv.py
+-rw-rw-rw-   0        0        0     3079 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/mp3.py
+-rw-rw-rw-   0        0        0     3316 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/mp4.py
+-rw-rw-rw-   0        0        0     3079 2023-04-25 15:14:24.000000 py-cord-dev-2.5.0rc3/discord/sinks/ogg.py
+-rw-rw-rw-   0        0        0     1610 2022-05-18 00:57:34.000000 py-cord-dev-2.5.0rc3/discord/sinks/pcm.py
+-rw-rw-rw-   0        0        0     2385 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/sinks/wave.py
+-rw-rw-rw-   0        0        0     6523 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    75924 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/state.py
+-rw-rw-rw-   0        0        0    16774 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/sticker.py
+-rw-rw-rw-   0        0        0     5563 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/team.py
+-rw-rw-rw-   0        0        0     9590 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/template.py
+-rw-rw-rw-   0        0        0    31552 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.499188 py-cord-dev-2.5.0rc3/discord/types/
+-rw-rw-rw-   0        0        0      192 2022-02-05 14:29:40.000000 py-cord-dev-2.5.0rc3/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2864 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2053 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     1589 2023-04-17 16:47:17.000000 py-cord-dev-2.5.0rc3/discord/types/application_role_connection.py
+-rw-rw-rw-   0        0        0     6992 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     2881 2023-04-25 15:17:38.000000 py-cord-dev-2.5.0rc3/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4835 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/channel.py
+-rw-rw-rw-   0        0        0     2630 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/components.py
+-rw-rw-rw-   0        0        0     2486 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1637 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     1451 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5555 2023-01-30 15:33:07.000000 py-cord-dev-2.5.0rc3/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2341 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7121 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2853 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1925 2022-07-04 17:05:58.000000 py-cord-dev-2.5.0rc3/discord/types/member.py
+-rw-rw-rw-   0        0        0     4083 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/types/message.py
+-rw-rw-rw-   0        0        0     4011 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/types/raw_models.py
+-rw-rw-rw-   0        0        0     1620 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/role.py
+-rw-rw-rw-   0        0        0     2141 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/scheduled_events.py
+-rw-rw-rw-   0        0        0     1254 2021-11-04 00:43:45.000000 py-cord-dev-2.5.0rc3/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2449 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1569 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/team.py
+-rw-rw-rw-   0        0        0     1685 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/template.py
+-rw-rw-rw-   0        0        0     2387 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1686 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/types/user.py
+-rw-rw-rw-   0        0        0     2412 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/voice.py
+-rw-rw-rw-   0        0        0     2046 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1524 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1947 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.508883 py-cord-dev-2.5.0rc3/discord/ui/
+-rw-rw-rw-   0        0        0      330 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    11075 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ui/button.py
+-rw-rw-rw-   0        0        0     8368 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ui/input_text.py
+-rw-rw-rw-   0        0        0     4334 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ui/item.py
+-rw-rw-rw-   0        0        0    11652 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    25702 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ui/select.py
+-rw-rw-rw-   0        0        0    22215 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/ui/view.py
+-rw-rw-rw-   0        0        0    18286 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/user.py
+-rw-rw-rw-   0        0        0    43348 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/utils.py
+-rw-rw-rw-   0        0        0    33725 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.512913 py-cord-dev-2.5.0rc3/discord/webhook/
+-rw-rw-rw-   0        0        0      249 2022-11-20 16:02:16.000000 py-cord-dev-2.5.0rc3/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    66862 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42708 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     8034 2022-11-28 18:07:53.000000 py-cord-dev-2.5.0rc3/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10838 2023-06-11 21:44:02.000000 py-cord-dev-2.5.0rc3/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.518453 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/
+-rw-rw-rw-   0        0        0     5949 2023-08-07 17:27:39.000000 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-08-07 17:27:40.000000 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:27:39.000000 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      345 2023-08-07 17:27:39.000000 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 17:27:39.000000 py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2592 2023-08-07 01:56:46.000000 py-cord-dev-2.5.0rc3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-07 17:27:40.524485 py-cord-dev-2.5.0rc3/requirements/
+-rw-rw-rw-   0        0        0       73 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc3/requirements/_.txt
+-rw-rw-rw-   0        0        0       53 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc3/requirements/all.txt
+-rw-rw-rw-   0        0        0      183 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/requirements/dev.txt
+-rw-rw-rw-   0        0        0      200 2023-08-07 01:56:46.000000 py-cord-dev-2.5.0rc3/requirements/docs.txt
+-rw-rw-rw-   0        0        0       36 2023-08-06 02:02:28.000000 py-cord-dev-2.5.0rc3/requirements/speed.txt
+-rw-rw-rw-   0        0        0       20 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc3/requirements/voice.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 17:27:40.528509 py-cord-dev-2.5.0rc3/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-11-20 16:02:17.000000 py-cord-dev-2.5.0rc3/setup.py
```

### Comparing `py-cord-dev-2.5.0rc2/CONTRIBUTING.md` & `py-cord-dev-2.5.0rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/LICENSE` & `py-cord-dev-2.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/PKG-INFO` & `py-cord-dev-2.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-cord-dev
-Version: 2.5.0rc2
+Version: 2.5.0rc3
 Summary: A Python wrapper for the Discord API. Temporary release
 Author: Pycord Development
 License: MIT
 Project-URL: Homepage, https://pycord.dev
 Project-URL: Changelog, https://docs.pycord.dev/en/master/changelog.html
 Project-URL: Source, https://github.com/Pycord-Development/pycord
 Project-URL: Documentation, https://docs.pycord.dev
```

### Comparing `py-cord-dev-2.5.0rc2/README.rst` & `py-cord-dev-2.5.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/__init__.py` & `py-cord-dev-2.5.0rc3/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/__main__.py` & `py-cord-dev-2.5.0rc3/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/_typed_dict.py` & `py-cord-dev-2.5.0rc3/discord/_typed_dict.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/_version.py` & `py-cord-dev-2.5.0rc3/discord/_version.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/abc.py` & `py-cord-dev-2.5.0rc3/discord/abc.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/activity.py` & `py-cord-dev-2.5.0rc3/discord/activity.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/appinfo.py` & `py-cord-dev-2.5.0rc3/discord/appinfo.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/application_role_connection.py` & `py-cord-dev-2.5.0rc3/discord/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/asset.py` & `py-cord-dev-2.5.0rc3/discord/asset.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/audit_logs.py` & `py-cord-dev-2.5.0rc3/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/automod.py` & `py-cord-dev-2.5.0rc3/discord/automod.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/backoff.py` & `py-cord-dev-2.5.0rc3/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/bin/libopus-0.x64.dll` & `py-cord-dev-2.5.0rc3/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/bin/libopus-0.x86.dll` & `py-cord-dev-2.5.0rc3/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/bot.py` & `py-cord-dev-2.5.0rc3/discord/bot.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/channel.py` & `py-cord-dev-2.5.0rc3/discord/channel.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/client.py` & `py-cord-dev-2.5.0rc3/discord/client.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/cog.py` & `py-cord-dev-2.5.0rc3/discord/cog.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/colour.py` & `py-cord-dev-2.5.0rc3/discord/colour.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/commands/__init__.py` & `py-cord-dev-2.5.0rc3/discord/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/commands/context.py` & `py-cord-dev-2.5.0rc3/discord/commands/context.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/commands/core.py` & `py-cord-dev-2.5.0rc3/discord/commands/core.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/commands/options.py` & `py-cord-dev-2.5.0rc3/discord/commands/options.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/commands/permissions.py` & `py-cord-dev-2.5.0rc3/discord/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/components.py` & `py-cord-dev-2.5.0rc3/discord/components.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/context_managers.py` & `py-cord-dev-2.5.0rc3/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/embeds.py` & `py-cord-dev-2.5.0rc3/discord/embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,16 +357,16 @@
         type: EmbedType = "rich",
         url: Any | None = None,
         description: Any | None = None,
         timestamp: datetime.datetime | None = None,
         fields: list[EmbedField] | None = None,
         author: EmbedAuthor | None = None,
         footer: EmbedFooter | None = None,
-        image: str | None = None,
-        thumbnail: str | None = None,
+        image: str | EmbedMedia | None = None,
+        thumbnail: str | EmbedMedia | None = None,
     ):
         self.colour = colour if colour else color
         self.title = title
         self.type = type
         self.url = url
         self.description = description
 
@@ -382,16 +382,19 @@
         if timestamp:
             self.timestamp = timestamp
 
         self._fields: list[EmbedField] = fields if fields is not None else []
 
         self.author = author
         self.footer = footer
-        self.image = image
-        self.thumbnail = thumbnail
+        
+        if image:
+            self.set_image(url=image.url)
+        if thumbnail:
+            self.set_thumbnail(url=image.url)
 
     @classmethod
     def from_dict(cls: type[E], data: Mapping[str, Any]) -> E:
         """Converts a :class:`dict` to a :class:`Embed` provided it is in the
         format that Discord expects it to be in.
 
         You can find out about this format in the `official Discord documentation`__.
@@ -636,17 +639,19 @@
         """
         img = getattr(self, "_image", None)
         if not img:
             return None
         return EmbedMedia.from_dict(img)
 
     @image.setter
-    def image(self, value: EmbedMedia | None):
+    def image(self, value: str | EmbedMedia | None):
         if value is None:
             self.remove_image()
+        elif isinstance(value, str):
+            self.set_image(url=value)
         elif isinstance(value, EmbedMedia):
             self.set_image(url=value.url)
         else:
             raise TypeError(
                 "Expected discord.EmbedMedia, or None but received"
                 f" {value.__class__.__name__} instead."
             )
@@ -708,17 +713,19 @@
         """
         thumb = getattr(self, "_thumbnail", None)
         if not thumb:
             return None
         return EmbedMedia.from_dict(thumb)
 
     @thumbnail.setter
-    def thumbnail(self, value: EmbedMedia | None):
+    def thumbnail(self, value: str | EmbedMedia | None):
         if value is None:
             self.remove_thumbnail()
+        elif isinstance(value, str):
+            self.set_thumbnail(url=value)
         elif isinstance(value, EmbedMedia):
             self.set_thumbnail(url=value.url)
         else:
             raise TypeError(
                 "Expected discord.EmbedMedia, or None but received"
                 f" {value.__class__.__name__} instead."
             )
```

### Comparing `py-cord-dev-2.5.0rc2/discord/emoji.py` & `py-cord-dev-2.5.0rc3/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/enums.py` & `py-cord-dev-2.5.0rc3/discord/enums.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/errors.py` & `py-cord-dev-2.5.0rc3/discord/errors.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/bridge/__init__.py` & `py-cord-dev-2.5.0rc3/discord/ext/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/bridge/bot.py` & `py-cord-dev-2.5.0rc3/discord/ext/bridge/bot.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/bridge/context.py` & `py-cord-dev-2.5.0rc3/discord/ext/bridge/context.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/bridge/core.py` & `py-cord-dev-2.5.0rc3/discord/ext/bridge/core.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/_types.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/bot.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/cog.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/context.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/converter.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/cooldowns.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/core.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/errors.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/flags.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/help.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/commands/view.py` & `py-cord-dev-2.5.0rc3/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/pages/pagination.py` & `py-cord-dev-2.5.0rc3/discord/ext/pages/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 from __future__ import annotations
 
-from typing import List
+from typing import List, overload
 
 import discord
-from discord.ext.bridge import BridgeContext
+from discord.ext.bridge import BridgeApplicationContext, BridgeContext, BridgeExtContext
 from discord.ext.commands import Context
 
 __all__ = (
     "PaginatorButton",
     "Paginator",
     "PageGroup",
     "PaginatorMenu",
@@ -424,15 +424,17 @@
         self.show_indicator = show_indicator
         self.disable_on_timeout = disable_on_timeout
         self.use_default_buttons = use_default_buttons
         self.default_button_row = default_button_row
         self.loop_pages = loop_pages
         self.custom_view: discord.ui.View = custom_view
         self.trigger_on_display = trigger_on_display
-        self.message: discord.Message | discord.WebhookMessage | None = None
+        self.message: discord.Message | discord.WebhookMessage | discord.InteractionMessage | None = (
+            None
+        )
 
         if self.custom_buttons and not self.use_default_buttons:
             for button in custom_buttons:
                 self.add_button(button)
         elif not self.custom_buttons and self.use_default_buttons:
             self.add_default_buttons()
 
@@ -1016,30 +1018,91 @@
             allowed_mentions=allowed_mentions,
             mention_author=mention_author,
             delete_after=delete_after,
         )
 
         return self.message
 
+    @overload
+    async def edit(
+        self,
+        message: discord.PartialMessage,
+        suppress: bool | None = ...,
+        allowed_mentions: discord.AllowedMentions | None = ...,
+        delete_after: float | None = ...,
+        user: discord.User | discord.Member = ...,
+    ) -> discord.Message:
+        ...
+
+    @overload
     async def edit(
         self,
         message: discord.Message,
+        suppress: bool | None = ...,
+        allowed_mentions: discord.AllowedMentions | None = ...,
+        delete_after: float | None = ...,
+        user: discord.User | discord.Member = ...,
+    ) -> discord.Message | None:
+        ...
+
+    @overload
+    async def edit(
+        self,
+        message: discord.ApplicationContext | BridgeApplicationContext,
+        suppress: bool | None = ...,
+        allowed_mentions: discord.AllowedMentions | None = ...,
+        delete_after: float | None = ...,
+        user: None = ...,
+    ) -> discord.InteractionMessage:
+        ...
+
+    @overload
+    async def edit(
+        self,
+        message: BridgeExtContext,
+        suppress: bool | None = ...,
+        allowed_mentions: discord.AllowedMentions | None = ...,
+        delete_after: float | None = ...,
+        user: None = ...,
+    ) -> discord.Message | None:
+        ...
+
+    @overload
+    async def edit(
+        self,
+        message: discord.Interaction,
+        suppress: bool | None = ...,
+        allowed_mentions: discord.AllowedMentions | None = ...,
+        delete_after: float | None = ...,
+        user: None = ...,
+    ) -> discord.InteractionMessage | None:
+        ...
+
+    async def edit(
+        self,
+        message: discord.PartialMessage
+        | discord.Message
+        | discord.Interaction
+        | discord.ApplicationContext
+        | BridgeApplicationContext
+        | BridgeExtContext,
         suppress: bool | None = None,
         allowed_mentions: discord.AllowedMentions | None = None,
         delete_after: float | None = None,
-    ) -> discord.Message | None:
-        """Edits an existing message to replace it with the paginator contents.
+        user: discord.User | discord.Member | None = None,
+    ) -> discord.Message | discord.InteractionMessage | None:
+        """Edits an existing message to replace it with the paginator.
 
         .. note::
 
-            If invoked from an interaction, you will still need to respond to the interaction.
+            If a view was previously present on the message, it will be removed.
 
         Parameters
         ----------
-        message: :class:`discord.Message`
+        message: Union[:class:`~discord.PartialMessage`, :class:`~discord.Message`, :class:`~discord.Interaction`, :class:`~discord.ApplicationContext`, :class:`~discord.ext.bridge.Context`]
             The message to edit with the paginator.
         suppress: :class:`bool`
             Whether to suppress embeds for the message. This removes
             all the embeds if set to ``True``. If set to ``False``
             this brings the embeds back if they were suppressed.
             Using this parameter requires :attr:`~.Permissions.manage_messages`.
         allowed_mentions: Optional[:class:`~discord.AllowedMentions`]
@@ -1047,63 +1110,85 @@
             passed, then the object is merged with :attr:`~discord.Client.allowed_mentions`.
             The merging behaviour only overrides attributes that have been explicitly passed
             to the object, otherwise it uses the attributes set in :attr:`~discord.Client.allowed_mentions`.
             If no object is passed at all then the defaults given by :attr:`~discord.Client.allowed_mentions`
             are used instead.
         delete_after: Optional[:class:`float`]
             If set, deletes the paginator after the specified time.
+        user: Optional[Union[:class:`~discord.User`, :class:`~discord.Member`]]
+            The user to set as the paginator's user, if target message is of type :class:`~discord.Message` or :class:`~discord.PartialMessage`.
 
         Returns
         -------
-        Optional[:class:`discord.Message`]
+        :class:`~discord.Message` | :class:`~discord.InteractionMessage` | ``None``
             The message that was edited. Returns ``None`` if the operation failed.
         """
-        if not isinstance(message, discord.Message):
-            raise TypeError(f"expected Message not {message.__class__!r}")
 
         self.update_buttons()
 
         page: Page | str | discord.Embed | list[discord.Embed] = self.pages[
             self.current_page
         ]
         page_content: Page = self.get_page_content(page)
 
         if page_content.custom_view:
             self.update_custom_view(page_content.custom_view)
 
-        self.user = message.author
+        if isinstance(message, discord.Interaction):
+            self.user = message.user
+        elif isinstance(message, (discord.Message, discord.PartialMessage)):
+            if not isinstance(user, (discord.User, discord.Member)):
+                raise TypeError(
+                    f"expected class discord.User or discord.Member for user parameter. Not {user.__class__.__name__!r}"
+                )
+            self.user = user
+        else:
+            self.user = message.author
 
         try:
-            self.message = await message.edit(
+            # pyright thinks the return type of this method can't be assigned to Message attribute for some reason
+            self.message = await message.edit(  # type: ignore
                 content=page_content.content,
                 embeds=page_content.embeds,
                 files=page_content.files,
                 attachments=[],
                 view=self,
                 suppress=suppress,
                 allowed_mentions=allowed_mentions,
                 delete_after=delete_after,
             )
+            if self.message is None:
+                if isinstance(message, discord.Interaction):
+                    # if the message is None, it means that interaction.response.edit_message was used.
+                    # this can only be done if the interaction was from a component or a modal
+                    # both of which have the message attribute set
+                    self.message: discord.Message = message.message  # type: ignore
+                elif isinstance(
+                    message, discord.Message
+                ):  # isinstance check was added to satisfy type checker. this is the only other case that might return None
+                    # target was discord.Message, and edit was in-place
+                    self.message: discord.Message = message
+
         except (discord.NotFound, discord.Forbidden):
             pass
 
         return self.message
 
     async def respond(
         self,
-        interaction: discord.Interaction | BridgeContext,
+        interaction: discord.Interaction | BridgeApplicationContext | BridgeExtContext,
         ephemeral: bool = False,
         target: discord.abc.Messageable | None = None,
         target_message: str = "Paginator sent!",
     ) -> discord.Message | discord.WebhookMessage:
         """Sends an interaction response or followup with the paginated items.
 
         Parameters
         ----------
-        interaction: Union[:class:`discord.Interaction`, :class:`BridgeContext`]
+        interaction: Union[:class:`discord.Interaction`, :class:`BridgeApplicationContext`, :class:`BridgeExtContext`]
             The interaction or BridgeContext which invoked the paginator.
             If passing a BridgeContext object, you cannot make this an ephemeral paginator.
         ephemeral: :class:`bool`
             Whether the paginator message and its components are ephemeral.
             If ``target`` is specified, the ephemeral message content will be ``target_message`` instead.
 
             .. warning::
```

### Comparing `py-cord-dev-2.5.0rc2/discord/ext/tasks/__init__.py` & `py-cord-dev-2.5.0rc3/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/file.py` & `py-cord-dev-2.5.0rc3/discord/file.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/flags.py` & `py-cord-dev-2.5.0rc3/discord/flags.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/gateway.py` & `py-cord-dev-2.5.0rc3/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/guild.py` & `py-cord-dev-2.5.0rc3/discord/guild.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/http.py` & `py-cord-dev-2.5.0rc3/discord/http.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/integrations.py` & `py-cord-dev-2.5.0rc3/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/interactions.py` & `py-cord-dev-2.5.0rc3/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/invite.py` & `py-cord-dev-2.5.0rc3/discord/invite.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/iterators.py` & `py-cord-dev-2.5.0rc3/discord/iterators.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/member.py` & `py-cord-dev-2.5.0rc3/discord/member.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/mentions.py` & `py-cord-dev-2.5.0rc3/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/message.py` & `py-cord-dev-2.5.0rc3/discord/message.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/mixins.py` & `py-cord-dev-2.5.0rc3/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/object.py` & `py-cord-dev-2.5.0rc3/discord/object.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/oggparse.py` & `py-cord-dev-2.5.0rc3/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/opus.py` & `py-cord-dev-2.5.0rc3/discord/opus.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/partial_emoji.py` & `py-cord-dev-2.5.0rc3/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/permissions.py` & `py-cord-dev-2.5.0rc3/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/player.py` & `py-cord-dev-2.5.0rc3/discord/player.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/raw_models.py` & `py-cord-dev-2.5.0rc3/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/reaction.py` & `py-cord-dev-2.5.0rc3/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/role.py` & `py-cord-dev-2.5.0rc3/discord/role.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/scheduled_events.py` & `py-cord-dev-2.5.0rc3/discord/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/shard.py` & `py-cord-dev-2.5.0rc3/discord/shard.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/core.py` & `py-cord-dev-2.5.0rc3/discord/sinks/core.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/errors.py` & `py-cord-dev-2.5.0rc3/discord/sinks/errors.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/m4a.py` & `py-cord-dev-2.5.0rc3/discord/sinks/m4a.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/mka.py` & `py-cord-dev-2.5.0rc3/discord/sinks/mka.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/mkv.py` & `py-cord-dev-2.5.0rc3/discord/sinks/mkv.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/mp3.py` & `py-cord-dev-2.5.0rc3/discord/sinks/mp3.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/mp4.py` & `py-cord-dev-2.5.0rc3/discord/sinks/mp4.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/ogg.py` & `py-cord-dev-2.5.0rc3/discord/sinks/ogg.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/pcm.py` & `py-cord-dev-2.5.0rc3/discord/sinks/pcm.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sinks/wave.py` & `py-cord-dev-2.5.0rc3/discord/sinks/wave.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/stage_instance.py` & `py-cord-dev-2.5.0rc3/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/state.py` & `py-cord-dev-2.5.0rc3/discord/state.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/sticker.py` & `py-cord-dev-2.5.0rc3/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/team.py` & `py-cord-dev-2.5.0rc3/discord/team.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/template.py` & `py-cord-dev-2.5.0rc3/discord/template.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/threads.py` & `py-cord-dev-2.5.0rc3/discord/threads.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/activity.py` & `py-cord-dev-2.5.0rc3/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/appinfo.py` & `py-cord-dev-2.5.0rc3/discord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/application_role_connection.py` & `py-cord-dev-2.5.0rc3/discord/types/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/audit_log.py` & `py-cord-dev-2.5.0rc3/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/automod.py` & `py-cord-dev-2.5.0rc3/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/channel.py` & `py-cord-dev-2.5.0rc3/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/components.py` & `py-cord-dev-2.5.0rc3/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/embed.py` & `py-cord-dev-2.5.0rc3/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/emoji.py` & `py-cord-dev-2.5.0rc3/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/gateway.py` & `py-cord-dev-2.5.0rc3/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/guild.py` & `py-cord-dev-2.5.0rc3/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/integration.py` & `py-cord-dev-2.5.0rc3/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/interactions.py` & `py-cord-dev-2.5.0rc3/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/invite.py` & `py-cord-dev-2.5.0rc3/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/member.py` & `py-cord-dev-2.5.0rc3/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/message.py` & `py-cord-dev-2.5.0rc3/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/raw_models.py` & `py-cord-dev-2.5.0rc3/discord/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/role.py` & `py-cord-dev-2.5.0rc3/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/scheduled_events.py` & `py-cord-dev-2.5.0rc3/discord/types/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/snowflake.py` & `py-cord-dev-2.5.0rc3/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/sticker.py` & `py-cord-dev-2.5.0rc3/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/team.py` & `py-cord-dev-2.5.0rc3/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/template.py` & `py-cord-dev-2.5.0rc3/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/threads.py` & `py-cord-dev-2.5.0rc3/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/user.py` & `py-cord-dev-2.5.0rc3/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/voice.py` & `py-cord-dev-2.5.0rc3/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/webhook.py` & `py-cord-dev-2.5.0rc3/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/welcome_screen.py` & `py-cord-dev-2.5.0rc3/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/types/widget.py` & `py-cord-dev-2.5.0rc3/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/button.py` & `py-cord-dev-2.5.0rc3/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/input_text.py` & `py-cord-dev-2.5.0rc3/discord/ui/input_text.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/item.py` & `py-cord-dev-2.5.0rc3/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/modal.py` & `py-cord-dev-2.5.0rc3/discord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/select.py` & `py-cord-dev-2.5.0rc3/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/ui/view.py` & `py-cord-dev-2.5.0rc3/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/user.py` & `py-cord-dev-2.5.0rc3/discord/user.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/utils.py` & `py-cord-dev-2.5.0rc3/discord/utils.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/voice_client.py` & `py-cord-dev-2.5.0rc3/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/webhook/async_.py` & `py-cord-dev-2.5.0rc3/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/webhook/sync.py` & `py-cord-dev-2.5.0rc3/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/welcome_screen.py` & `py-cord-dev-2.5.0rc3/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/discord/widget.py` & `py-cord-dev-2.5.0rc3/discord/widget.py`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/PKG-INFO` & `py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-cord-dev
-Version: 2.5.0rc2
+Version: 2.5.0rc3
 Summary: A Python wrapper for the Discord API. Temporary release
 Author: Pycord Development
 License: MIT
 Project-URL: Homepage, https://pycord.dev
 Project-URL: Changelog, https://docs.pycord.dev/en/master/changelog.html
 Project-URL: Source, https://github.com/Pycord-Development/pycord
 Project-URL: Documentation, https://docs.pycord.dev
```

### Comparing `py-cord-dev-2.5.0rc2/py_cord_dev.egg-info/SOURCES.txt` & `py-cord-dev-2.5.0rc3/py_cord_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-cord-dev-2.5.0rc2/pyproject.toml` & `py-cord-dev-2.5.0rc3/pyproject.toml`

 * *Files identical despite different names*

